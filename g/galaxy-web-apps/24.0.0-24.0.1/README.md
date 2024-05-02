# Comparing `tmp/galaxy-web-apps-24.0.0.tar.gz` & `tmp/galaxy_web_apps-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-web-apps-24.0.0.tar", last modified: Wed Apr  3 02:46:50 2024, max compression
+gzip compressed data, was "galaxy_web_apps-24.0.1.tar", last modified: Thu May  2 13:49:55 2024, max compression
```

## Comparing `galaxy-web-apps-24.0.0.tar` & `galaxy_web_apps-24.0.1.tar`

### file list

```diff
@@ -1,518 +1,518 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    31959 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34337 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.916463 galaxy-web-apps-24.0.0/galaxy/datatypes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.916463 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/biom/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/biom/biom_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/icn3d/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/icn3d/icn3d_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bb.xml
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/gtf.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/wig.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/genbank.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/image/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/image/avivator.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/intermine/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/intermine/intermine_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/iobio/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/iobio/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/iobio/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/minerva/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/minerva/tabular.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/trackhub.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.936464 galaxy-web-apps-24.0.0/galaxy/webapps/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.936464 galaxy-web-apps-24.0.0/galaxy/webapps/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    63303 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.936464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/erricon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20770 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/formatHelp.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.940464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/delete.gif
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/delete_tag_icon_gray.png
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/dw.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.944464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   134808 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.956464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/application-dock-270-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      516 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/application-dock-270.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-000-small-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      553 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-090.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-circle.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-resize-090-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      403 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-resize-090.png
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-split-bw.png
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-split.png
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-transition-270-bw.png
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-transition-bw.png
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/block--plus-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/block--plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bookmarks-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bookmarks.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bug.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chart.png
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chevron-expand-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      490 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chevron-expand.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      493 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chevron.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/control-270.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      555 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-button.png
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-circle-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-circle.png
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-small-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross.png
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk--arrow-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      603 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk--arrow.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      613 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/exclamation.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/external.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      536 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/eye.png
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/gear-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      721 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/globe-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/globe.png
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/hammer-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      575 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/hammer.png
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/information-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layer-transparent-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      566 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layer-transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layers-stack-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      664 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layers-stack.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-left.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      736 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-zoom-out.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/navigation.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      309 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/pencil-small.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/pencil.png
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-button-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-button.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-circle.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/sticky-note-text.png
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tag--plus.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tag-label.png
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tags.png
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-bw.png
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-expand-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-expand.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1243 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toolbox-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toolbox.png
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/ui-slider-050-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      454 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/ui-slider-050.png
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/hatch-fade-023858.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.960464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon_grey.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.960464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_empty.png
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_error.png
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_ok.png
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_queued.png
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history.gif
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history_down_arrow.gif
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history_up_arrow.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_error_lrg.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_error_sml.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_info_lrg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_info_sml.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_success_lrg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_success_sml.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_warning_lrg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_warning_sml.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/loading_large_white_bg.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/loading_small_white_bg.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.960464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/
--rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/interval2maf.png
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/stitchMaf.png
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/openid-16x16.gif
--rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/rgWebLogo3_test.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_empty.gif
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_error.gif
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_ok.gif
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_queued.gif
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_running.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/star.gif
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tool_menu_down_arrow.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.964464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/
--rw-r--r--   0 runner    (1001) docker     (127)   257713 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/build_list.svg
--rw-r--r--   0 runner    (1001) docker     (127)    81633 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/filter_empty.svg
--rw-r--r--   0 runner    (1001) docker     (127)    72821 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/filter_error.svg
--rw-r--r--   0 runner    (1001) docker     (127)    92949 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/flatten.svg
--rw-r--r--   0 runner    (1001) docker     (127)   108978 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/unzip.svg
--rw-r--r--   0 runner    (1001) docker     (127)   109459 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.964464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/
--rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/first_matrix_generator_example_file.png
--rw-r--r--   0 runner    (1001) docker     (127)    23673 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/second_matrix_generator_example_file.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.964464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/block.png
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/close_btn.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/diag_bg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/go_btn.gif
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/handle-left.gif
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/handle-right.gif
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/pan_left.gif
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/pan_right.gif
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/show_history.gif
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/zoom_in.gif
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/zoom_in_full.gif
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/zoom_out.gif
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/zoom_out_full.gif
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/up.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.968464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/draggable_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/draggable_vertical.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/strand_left.png
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/strand_left_inv.png
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/strand_right.png
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/strand_right_inv.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.968464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/yui/
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/yui/rel_interstitial_loading.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/incompatible-browser.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.968464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/patmat/
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/patmat/findcluster.png
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.972464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/circster.css
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/data_running.gif
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/data_upload.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.972464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4046 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/icons-rtl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     4041 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/icons.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/loading.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     9902 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/ui.dynatree.css
--rwxr-xr-x   0 runner    (1001) docker     (127)      842 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/vline-rtl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/vline.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/embed_item.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/history.css
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/info_icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.972464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.972464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      110 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_222222_256x240.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     5355 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_2e83ff_256x240.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_454545_256x240.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_888888_256x240.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)    20147 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery.rating.css
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/library.css
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/masthead.css
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/ok_small.png
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/question-octagon-frame.png
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/reports.css
--rw-r--r--   0 runner    (1001) docker     (127)    31536 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-fugue.png
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-history-buttons.png
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-history-states.png
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/trackster.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.976464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.976464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-detail-view.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-list-view.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-listrow-view.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-model.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/test-file.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/toolshed.groups.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.976464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.924464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.976464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-detail-view.js
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-list-view.js
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-listrow-view.js
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-model.js
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/toolshed.groups.js
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/user_disabled.html
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/welcome.html.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base/base_panels.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/display_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/display_common.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/embed_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/galaxy_client_app.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/js-app.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/legacy/grid_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/legacy/grid_base_async.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/message.mako
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/no_access.mako
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/page_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/refresh_frames.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/slug_editing_js.mako
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/sorting_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/spark_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/tagging_common.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/tool_shed_rating.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.924464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.924464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/root/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.988464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/base_panels.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/dataset_info.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_per_user.mako
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/index.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/job_info.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_errors_per_tool.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_all.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_by_user_and_destination.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_in_error.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_tool.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_user.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_user_by_destination.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_all.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_in_error.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_tool_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month_by_destination.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_date.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/run_stats.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/system.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_error_messages.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_execution_time.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_execution_time_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/users_last_access_date.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/users_user_disk_usage.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_month_all.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_user.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_workflow.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_user_per_month.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.924464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.988464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/common/
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/common/common.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.988464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/repository/
--rw-r--r--   0 runner    (1001) docker     (127)    57351 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/repository/common.mako
--rw-r--r--   0 runner    (1001) docker     (127)    51314 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.988464 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.004465 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cbv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cloudauthz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/container_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/dataset_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    18059 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/display_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/drs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/dynamic_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/extended_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/folder_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/genomes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    28672 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    39822 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    22023 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/library_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    38850 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/library_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/page_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/remote_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/roles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4090 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/sanitize_allow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/short_term_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/storage_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    22679 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_shed_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    23930 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/toolshed.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tours.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/trs_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/trs_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)    49922 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    71507 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)    41693 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/buildapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.008465 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51510 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/admin_toolshed.py
--rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/async.py
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/authnz.py
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    52721 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/shed_tool_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/tool_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    20164 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/fast_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/fast_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.012465 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/_fetch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/dataset_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    39171 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    34805 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    66849 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/invocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/library_folder_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/library_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/sharable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/storage_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/tool_shed_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.012465 galaxy-web-apps-24.0.0/galaxy/webapps/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/openapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.012465 galaxy-web-apps-24.0.0/galaxy/webapps/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.012465 galaxy-web-apps-24.0.0/galaxy/webapps/reports/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/buildapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/home.py
--rw-r--r--   0 runner    (1001) docker     (127)    46704 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    17898 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/fast_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/fast_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34337 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24368 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.138289 galaxy_web_apps-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35266 2024-05-02 13:49:55.134289 galaxy_web_apps-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.046288 galaxy_web_apps-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.038288 galaxy_web_apps-24.0.1/galaxy/datatypes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.038288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.038288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.046288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/biom/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/biom/biom_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.046288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ensembl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.050288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/gbrowse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.050288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/icn3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/icn3d/icn3d_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.050288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bb.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/gtf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/wig.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.050288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/genbank.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.050288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/image/avivator.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.050288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/intermine/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/intermine/intermine_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.050288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/iobio/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/iobio/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/iobio/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.050288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/minerva/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/minerva/tabular.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.054288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/rviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/rviewer/bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.054288 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/trackhub.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.054288 galaxy_web_apps-24.0.1/galaxy/webapps/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.054288 galaxy_web_apps-24.0.1/galaxy/webapps/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63303 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.058288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/erricon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20770 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/formatHelp.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.062288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/delete_tag_icon_gray.png
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/dw.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.066288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   134808 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.078288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/application-dock-270-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      516 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/application-dock-270.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-000-small-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      553 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-090.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-circle.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-resize-090-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      403 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-resize-090.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-split-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-split.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-transition-270-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-transition-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/block--plus-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/block--plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/bookmarks-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/bookmarks.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/bug.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/chart.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/chevron-expand-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      490 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/chevron-expand.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      493 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/chevron.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/control-270.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      555 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross-circle-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross-circle.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross-small-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/disk--arrow-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      603 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/disk--arrow.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/disk.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      613 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/exclamation.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/external.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      536 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/eye.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/gear-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      721 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/globe-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/globe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/hammer-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      575 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/hammer.png
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/information-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/layer-transparent-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      566 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/layer-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/layers-stack-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      664 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/layers-stack.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/magnifier-left.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      736 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/magnifier-zoom-out.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/magnifier-zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/navigation.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      309 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/pencil-small.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/plus-button-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/plus-button.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/plus-circle.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/sticky-note-text.png
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/tag--plus.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/tag-label.png
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/tags.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toggle-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toggle-expand-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toggle-expand.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toggle.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1243 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toolbox-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toolbox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/ui-slider-050-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      454 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/ui-slider-050.png
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/hatch-fade-023858.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.078288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/delete_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/delete_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/delete_icon_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/eye_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/eye_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/eye_icon_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon_grey.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.078288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-states/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-states/data_empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-states/data_error.png
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-states/data_ok.png
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-states/data_queued.png
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history_down_arrow.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history_up_arrow.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_error_lrg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_error_sml.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_info_lrg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_info_sml.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_success_lrg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_success_sml.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_warning_lrg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_warning_sml.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/loading_large_white_bg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/loading_small_white_bg.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.078288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/maf_icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/maf_icons/interval2maf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/maf_icons/stitchMaf.png
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/openid-16x16.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/rgWebLogo3_test.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/square_empty.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/square_error.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/square_ok.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/square_queued.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/square_running.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/star.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tool_menu_down_arrow.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.038288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.082288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)   257713 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/build_list.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    81633 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/filter_empty.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    72821 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/filter_error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    92949 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/flatten.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   108978 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/unzip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   109459 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.082288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/lda/
+-rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/lda/first_matrix_generator_example_file.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23673 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/lda/second_matrix_generator_example_file.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.086288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/block.png
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/close_btn.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/diag_bg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/go_btn.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/handle-left.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/handle-right.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/pan_left.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/pan_right.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/show_history.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/zoom_in.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/zoom_in_full.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/zoom_out.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/zoom_out_full.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/up.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.086288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/visualization/draggable_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/visualization/draggable_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/visualization/strand_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/visualization/strand_left_inv.png
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/visualization/strand_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/visualization/strand_right_inv.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.086288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/yui/
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/yui/rel_interstitial_loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/incompatible-browser.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.086288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/patmat/
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/patmat/findcluster.png
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.090288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/circster.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/data_running.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/data_upload.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.090288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4046 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/icons-rtl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4041 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/icons.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/loading.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9902 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/ui.dynatree.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)      842 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/vline-rtl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/vline.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/embed_item.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/history.css
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/info_icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.042288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.090288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.094288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      110 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_222222_256x240.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5355 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_2e83ff_256x240.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_454545_256x240.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_888888_256x240.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20147 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery.rating.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/library.css
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/masthead.css
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/ok_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/question-octagon-frame.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/reports.css
+-rw-r--r--   0 runner    (1001) docker     (127)    31536 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/sprite-fugue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/sprite-history-buttons.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/sprite-history-states.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/trackster.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.042288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.094288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.042288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.094288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-detail-view.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-list-view.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-listrow-view.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-model.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/test-file.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/toolshed.groups.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.094288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.042288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.094288 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-detail-view.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-list-view.js
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-listrow-view.js
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-model.js
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/toolshed.groups.js
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/user_disabled.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/static/welcome.html.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.098288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.098288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/base/base_panels.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/display_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/display_common.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/embed_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/galaxy_client_app.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/js-app.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.098288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/legacy/grid_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/legacy/grid_base_async.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/message.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/no_access.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/page_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/refresh_frames.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/slug_editing_js.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/sorting_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/spark_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/tagging_common.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/tool_shed_rating.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.042288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.042288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.098288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.102288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.102288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/root/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.102288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.102288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.106289 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/base_panels.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/dataset_info.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/history_per_user.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/index.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/job_info.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_errors_per_tool.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_all.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_by_user_and_destination.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_in_error.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_tool.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_user.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_user_by_destination.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_all.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_in_error.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_tool_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month_by_destination.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/registered_users.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/registered_users_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_date.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/run_stats.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/system.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tool_error_messages.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tool_execution_time.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tool_execution_time_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/users_last_access_date.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/users_user_disk_usage.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_month_all.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_user.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_workflow.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/workflows_user_per_month.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.042288 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/tool_shed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.106289 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/tool_shed/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/tool_shed/common/common.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.106289 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/tool_shed/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)    57351 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/tool_shed/repository/common.mako
+-rw-r--r--   0 runner    (1001) docker     (127)    51314 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/base/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.110288 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.122289 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/cbv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/cloudauthz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/container_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/dataset_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18059 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/display_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/dynamic_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/extended_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/folder_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/genomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28672 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39822 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/job_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/job_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/job_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/job_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22039 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/library_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38850 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/library_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/page_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/remote_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4090 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/sanitize_allow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/short_term_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/storage_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tool_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tool_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tool_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22679 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tool_shed_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23930 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/toolshed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tours.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/trs_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/trs_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49922 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71672 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41693 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/buildapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.126289 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51510 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/admin_toolshed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/authnz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52721 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/shed_tool_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/tool_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20155 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/fast_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/fast_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.130288 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/_fetch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/dataset_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39171 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34805 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67056 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/library_folder_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/library_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/sharable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/storage_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/tool_shed_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.130288 galaxy_web_apps-24.0.1/galaxy/webapps/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/openapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.130288 galaxy_web_apps-24.0.1/galaxy/webapps/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.130288 galaxy_web_apps-24.0.1/galaxy/webapps/reports/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/buildapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.134289 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46704 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17898 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/fast_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/reports/fast_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/galaxy/webapps/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:55.134289 galaxy_web_apps-24.0.1/galaxy_web_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35266 2024-05-02 13:49:55.000000 galaxy_web_apps-24.0.1/galaxy_web_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24368 2024-05-02 13:49:55.000000 galaxy_web_apps-24.0.1/galaxy_web_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:55.000000 galaxy_web_apps-24.0.1/galaxy_web_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-02 13:49:55.000000 galaxy_web_apps-24.0.1/galaxy_web_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:49:55.000000 galaxy_web_apps-24.0.1/galaxy_web_apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-02 13:49:55.138289 galaxy_web_apps-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 13:46:45.000000 galaxy_web_apps-24.0.1/test-requirements.txt
```

### Comparing `galaxy-web-apps-24.0.0/HISTORY.rst` & `galaxy_web_apps-24.0.1/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Ensure that offset and limit are never negative by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18044 <https://github.com/galaxyproject/galaxy/pull/18044>`_
+* Fix history update time after bulk operation by `@davelopez <https://github.com/davelopez>`_ in `#18068 <https://github.com/galaxyproject/galaxy/pull/18068>`_
+
+============
+Enhancements
+============
+
+* Add middleware for logging start and end of request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18046 <https://github.com/galaxyproject/galaxy/pull/18046>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-web-apps-24.0.0/LICENSE` & `galaxy_web_apps-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/PKG-INFO` & `galaxy_web_apps-24.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-apps
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy web apps
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -78,14 +78,34 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Ensure that offset and limit are never negative by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18044 <https://github.com/galaxyproject/galaxy/pull/18044>`_
+* Fix history update time after bulk operation by `@davelopez <https://github.com/davelopez>`_ in `#18068 <https://github.com/galaxyproject/galaxy/pull/18068>`_
+
+============
+Enhancements
+============
+
+* Add middleware for logging start and end of request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18046 <https://github.com/galaxyproject/galaxy/pull/18046>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bam.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bb.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bb.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bed.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bigwig.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/gtf.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/gtf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/wig.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igb/wig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/bam.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/bigwig.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/genbank.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/genbank.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/gff.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/vcf.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/igv/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/bed.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/rviewer/bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bam.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml` & `galaxy_web_apps-24.0.1/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/api.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import os
 import stat
 import typing
+import uuid
+from logging import getLogger
 
 import anyio
 from fastapi import (
     FastAPI,
     HTTPException,
     Request,
     status,
 )
 from fastapi.exceptions import RequestValidationError
 from fastapi.responses import JSONResponse
 from starlette.responses import (
     FileResponse,
     Response,
 )
+from starlette_context import context
 from starlette_context.middleware import RawContextMiddleware
-from starlette_context.plugins import RequestIdPlugin
+from starlette_context.plugins import (
+    Plugin,
+    RequestIdPlugin,
+)
 
 from galaxy.exceptions import MessageException
 from galaxy.exceptions.utils import api_error_to_dict
 from galaxy.web.framework.base import walk_controller_modules
 from galaxy.web.framework.decorators import validation_error_to_message_exception
 
 if typing.TYPE_CHECKING:
@@ -28,14 +34,17 @@
     from starlette.types import (
         Receive,
         Scope,
         Send,
     )
 
 
+log = getLogger(__name__)
+
+
 # Copied from https://github.com/tiangolo/fastapi/issues/1240#issuecomment-1055396884
 def _get_range_header(range_header: str, file_size: int) -> typing.Tuple[int, int]:
     def _invalid_range():
         return HTTPException(
             status.HTTP_416_REQUESTED_RANGE_NOT_SATISFIABLE,
             detail=f"Invalid request range (Range:{range_header!r})",
         )
@@ -188,14 +197,39 @@
         return get_error_response_for_request(request, message_exception)
 
     @app.exception_handler(MessageException)
     async def message_exception_middleware(request: Request, exc: MessageException) -> Response:
         return get_error_response_for_request(request, exc)
 
 
+class AccessLoggingMiddleware(Plugin):
+
+    key = "access_line"
+
+    async def process_request(self, request):
+        scope = request.scope
+        path = scope["root_path"] + scope["path"]
+        if scope["query_string"]:
+            path = f"{path}?{scope['query_string'].decode('ascii')}"
+        access_line = f"{scope['method']} {path} {uuid.uuid4()}"
+        log.debug(access_line)
+        return access_line
+
+    async def enrich_response(self, response) -> None:
+        access_line = context.get("access_line")
+        if status := response.get("status"):
+            log.debug(f"{access_line} {status}")
+
+
+def add_raw_context_middlewares(app: FastAPI):
+    getLogger("uvicorn.access").handlers = []
+    plugins = (RequestIdPlugin(force_new_uuid=True), AccessLoggingMiddleware())
+    app.add_middleware(RawContextMiddleware, plugins=plugins)
+
+
 def add_request_id_middleware(app: FastAPI):
     app.add_middleware(RawContextMiddleware, plugins=(RequestIdPlugin(force_new_uuid=True),))
 
 
 def include_all_package_routers(app: FastAPI, package_name: str):
     for _, module in walk_controller_modules(package_name):
         router = getattr(module, "router", None)
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/controller.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/controller.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/erricon.ico` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/erricon.ico`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/favicon.ico` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/favicon.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/formatHelp.html` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/formatHelp.html`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/delete.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/delete.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/dw.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/dw.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/FontAwesome.otf` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.eot` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.ttf` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff2` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/application-dock-270-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/application-dock-270-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/application-dock-270.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/application-dock-270.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-000-small-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-000-small-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-090.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-090.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-circle.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-circle.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-resize-090-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-resize-090-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-split-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-split-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-split.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-split.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-transition-270-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-transition-270-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-transition-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/arrow-transition-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/block--plus-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/block--plus-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/block--plus.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/block--plus.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bookmarks-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/bookmarks-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bookmarks.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/bookmarks.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bug.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/bug.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chevron-expand-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/chevron-expand-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-button.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross-button.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-circle-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross-circle-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-circle.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross-circle.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-small-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/cross-small-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk--arrow-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/disk--arrow-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk--arrow.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/disk--arrow.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/exclamation.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/exclamation.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/external.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/external.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/eye.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/eye.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/gear-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/gear-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/gear.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/gear.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/globe-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/globe-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/globe.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/globe.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/hammer-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/hammer-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/hammer.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/hammer.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/information-white.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/information-white.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layer-transparent-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/layer-transparent-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layer-transparent.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/layer-transparent.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layers-stack-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/layers-stack-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layers-stack.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/layers-stack.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-left.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/magnifier-left.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-zoom-out.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/magnifier-zoom-out.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-zoom.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/magnifier-zoom.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/navigation.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/navigation.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-button-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/plus-button-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-button.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/plus-button.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-circle.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/plus-circle.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/sticky-note-text.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/sticky-note-text.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tag--plus.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/tag--plus.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tag-label.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/tag-label.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tags.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/tags.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toggle-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-expand-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toggle-expand-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-expand.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toggle-expand.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toolbox-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/toolbox-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/ui-slider-050-bw.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/fugue/ui-slider-050-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/delete_icon.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon_dark.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/delete_icon_dark.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/eye_icon.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon_dark.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/eye_icon_dark.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon_dark.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon_dark.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_queued.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history-states/data_queued.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/history.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_error_lrg.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_error_lrg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_error_sml.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_error_sml.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_info_lrg.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_info_lrg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_info_sml.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_info_sml.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_success_lrg.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_success_lrg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_success_sml.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_success_sml.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_warning_lrg.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_warning_lrg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_warning_sml.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/icon_warning_sml.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/loading_large_white_bg.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/loading_large_white_bg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/loading_small_white_bg.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/loading_small_white_bg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/interval2maf.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/maf_icons/interval2maf.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/stitchMaf.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/maf_icons/stitchMaf.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/rgWebLogo3_test.jpg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/rgWebLogo3_test.jpg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/star.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/star.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/build_list.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/build_list.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/filter_empty.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/filter_empty.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/filter_error.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/filter_error.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/flatten.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/flatten.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/unzip.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/unzip.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/zip.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/collection_ops/zip.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/first_matrix_generator_example_file.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/lda/first_matrix_generator_example_file.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/second_matrix_generator_example_file.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tools/lda/second_matrix_generator_example_file.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/block.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/block.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/diag_bg.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/diag_bg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/show_history.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/tracks/show_history.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/up.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/up.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/yui/rel_interstitial_loading.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/images/yui/rel_interstitial_loading.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/incompatible-browser.html` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/incompatible-browser.html`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/patmat/findcluster.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/patmat/findcluster.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/data_running.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/data_running.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/data_upload.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/data_upload.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/icons-rtl.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/icons-rtl.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/icons.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/icons.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/loading.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/loading.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/ui.dynatree.css` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/ui.dynatree.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/vline-rtl.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/vline-rtl.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/vline.gif` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/dynatree_skin/vline.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/embed_item.css` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/embed_item.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/info_icon.svg` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/info_icon.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_222222_256x240.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_2e83ff_256x240.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_454545_256x240.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_888888_256x240.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_cd0a0a_256x240.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/jquery-ui.css` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery.rating.css` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/jquery.rating.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/library.css` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/library.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/masthead.css` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/masthead.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/question-octagon-frame.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/question-octagon-frame.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/reports.css` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/reports.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-fugue.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/sprite-fugue.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-history-buttons.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/sprite-history-buttons.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-history-states.png` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/sprite-history-states.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/trackster.css` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/style/trackster.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-detail-view.js.map` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-detail-view.js.map`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-list-view.js.map` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-list-view.js.map`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-listrow-view.js.map` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-listrow-view.js.map`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/toolshed.groups.js.map` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/maps/toolshed.groups.js.map`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-detail-view.js` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-detail-view.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-list-view.js` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-list-view.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-listrow-view.js` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-listrow-view.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/toolshed.groups.js` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/toolshed/scripts/toolshed.groups.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/user_disabled.html` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/user_disabled.html`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/welcome.html.sample` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/static/welcome.html.sample`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base/base_panels.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/base/base_panels.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/display_base.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/display_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/display_common.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/display_common.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/embed_base.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/embed_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/galaxy_client_app.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/galaxy_client_app.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/js-app.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/js-app.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/legacy/grid_base.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/legacy/grid_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/message.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/message.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/no_access.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/no_access.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/page_base.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/page_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/refresh_frames.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/refresh_frames.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/slug_editing_js.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/slug_editing_js.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/sorting_base.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/sorting_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/spark_base.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/spark_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/tagging_common.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/tagging_common.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/tool_shed_rating.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/tool_shed_rating.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/base_panels.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/base_panels.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/dataset_info.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/dataset_info.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_per_user.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/history_per_user.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/index.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/index.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/job_info.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/job_info.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_errors_per_tool.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_errors_per_tool.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_all.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_all.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_by_user_and_destination.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_by_user_and_destination.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_in_error.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_in_error.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_tool.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_tool.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_user.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_user.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_user_by_destination.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_user_by_destination.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_all.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_all.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_in_error.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_in_error.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_tool_per_month.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_tool_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month_by_destination.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month_by_destination.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/registered_users.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_per_month.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/registered_users_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_date.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_date.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_month.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/run_stats.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/run_stats.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/system.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/system.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_error_messages.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tool_error_messages.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_execution_time.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tool_execution_time.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_execution_time_per_month.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tool_execution_time_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state_per_month.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/users_last_access_date.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/users_last_access_date.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/users_user_disk_usage.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/users_user_disk_usage.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_month_all.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_month_all.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_user.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_user.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_workflow.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_workflow.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_user_per_month.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/reports/workflows_user_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/common/common.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/tool_shed/common/common.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/repository/common.mako` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/templates/webapps/tool_shed/repository/common.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/base/webapp.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/base/webapp.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/__init__.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/annotations.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/annotations.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/authenticate.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/authenticate.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cbv.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/cbv.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cloud.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/cloud.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cloudauthz.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/cloudauthz.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/common.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/common.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/configuration.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/configuration.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/container_resolution.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/container_resolution.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/dataset_collections.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/dataset_collections.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/datasets.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/datatypes.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/datatypes.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/display_applications.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/display_applications.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/drs.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/drs.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/dynamic_tools.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/dynamic_tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/extended_metadata.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/extended_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/folder_contents.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/folder_contents.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,19 @@
 router = Router(tags=["data libraries folders"])
 
 FolderIdPathParam = Annotated[
     LibraryFolderDatabaseIdField,
     Path(..., title="Folder ID", description="The encoded identifier of the library folder."),
 ]
 
-LimitQueryParam: int = Query(default=10, title="Limit", description="Maximum number of contents to return.")
+LimitQueryParam: int = Query(default=10, ge=1, title="Limit", description="Maximum number of contents to return.")
 
 OffsetQueryParam: int = Query(
     default=0,
+    ge=0,
     title="Offset",
     description="Return contents from this specified position. For example, if ``limit`` is set to 100 and ``offset`` to 200, contents between position 200-299 will be returned.",
 )
 
 SearchQueryParam: Optional[str] = Query(
     default=None,
     title="Search Text",
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/folders.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/folders.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/forms.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/forms.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/genomes.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/genomes.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/group_roles.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/group_roles.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/group_users.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/group_users.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/groups.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/groups.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/help.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/help.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/histories.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/histories.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/history_contents.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/history_contents.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/item_tags.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/item_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_files.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/job_files.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_lock.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/job_lock.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_ports.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/job_ports.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_tokens.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/job_tokens.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/jobs.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,18 +157,19 @@
 
 SortByQueryParam: JobIndexSortByEnum = Query(
     default=JobIndexSortByEnum.update_time,
     title="Sort By",
     description="Sort results by specified field.",
 )
 
-LimitQueryParam: int = Query(default=500, title="Limit", description="Maximum number of jobs to return.")
+LimitQueryParam: int = Query(default=500, ge=1, title="Limit", description="Maximum number of jobs to return.")
 
 OffsetQueryParam: int = Query(
     default=0,
+    ge=0,
     title="Offset",
     description="Return jobs starting from this specified position. For example, if ``limit`` is set to 100 and ``offset`` to 200, jobs 200-299 will be returned.",
 )
 
 query_tags = [
     IndexQueryTag("user", "The user email of the user that executed the Job.", "u"),
     IndexQueryTag("tool_id", "The tool ID corresponding to the job.", "t"),
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/libraries.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/libraries.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/library_contents.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/library_contents.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/library_datasets.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/library_datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/licenses.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/licenses.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/metrics.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/metrics.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/notifications.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/notifications.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/object_store.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/object_store.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/page_revisions.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/page_revisions.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/pages.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,18 +68,19 @@
 
 SortDescQueryParam: bool = Query(
     default=False,
     title="Sort Descending",
     description="Sort in descending order?",
 )
 
-LimitQueryParam: int = Query(default=100, lt=1000, title="Limit number of queries.")
+LimitQueryParam: int = Query(default=100, ge=1, lt=1000, title="Limit number of queries.")
 
 OffsetQueryParam: int = Query(
     default=0,
+    ge=0,
     title="Number of pages to skip in sorted query (to enable pagination).",
 )
 
 query_tags = [
     IndexQueryTag("title", "The page's title."),
     IndexQueryTag("slug", "The page's slug.", "s"),
     IndexQueryTag("tag", "The page's tags.", "t"),
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/plugins.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/plugins.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/provenance.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/provenance.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/quotas.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/quotas.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/remote_files.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/remote_files.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/roles.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/roles.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/sanitize_allow.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/sanitize_allow.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/short_term_storage.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/short_term_storage.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/storage_cleaner.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/storage_cleaner.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tags.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tasks.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tasks.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_data.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tool_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_dependencies.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tool_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_entry_points.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tool_entry_points.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_shed_repositories.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tool_shed_repositories.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tools.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/toolshed.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/toolshed.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tours.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/tours.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/trs_consumer.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/trs_consumer.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/trs_search.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/trs_search.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/uploads.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/uploads.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/users.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/users.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/visualizations.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/visualizations.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/webhooks.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/webhooks.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/workflows.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/api/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     InvokeWorkflowPayload,
     StoredWorkflowDetailed,
 )
 from galaxy.structured_app import StructuredApp
 from galaxy.tool_shed.galaxy_install.install_manager import InstallRepositoryManager
 from galaxy.tools import recommendations
 from galaxy.tools.parameters import populate_state
-from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.tools.parameters.workflow_utils import workflow_building_modes
 from galaxy.util.sanitize_html import sanitize_html
 from galaxy.version import VERSION
 from galaxy.web import (
     expose_api,
     expose_api_raw_anonymous_and_sessionless,
     format_return_as_json,
 )
@@ -537,23 +537,26 @@
         if payload is None:
             payload = {}
         inputs = payload.get("inputs", {})
         trans.workflow_building_mode = workflow_building_modes.ENABLED
         module = module_factory.from_dict(trans, payload, from_tool_form=True)
         if "tool_state" not in payload:
             module_state: Dict[str, Any] = {}
-            populate_state(trans, module.get_inputs(), inputs, module_state, check=False)
+            errors: Dict[str, str] = {}
+            populate_state(trans, module.get_inputs(), inputs, module_state, errors=errors, check=True)
             module.recover_state(module_state, from_tool_form=True)
+            module.check_and_update_state()
         step_dict = {
             "name": module.get_name(),
-            "tool_state": module.get_state(),
+            "tool_state": module_state,
             "content_id": module.get_content_id(),
             "inputs": module.get_all_inputs(connectable_only=True),
             "outputs": module.get_all_outputs(),
             "config_form": module.get_config_form(),
+            "errors": errors or None,
         }
         if payload["type"] == "tool":
             step_dict["tool_version"] = module.get_version()
         return step_dict
 
     @expose_api
     def get_tool_predictions(self, trans: ProvidesUserContext, payload, **kwd):
@@ -808,18 +811,19 @@
 
 SortDescQueryParam: Optional[bool] = Query(
     default=None,
     title="Sort Descending",
     description="Sort in descending order?",
 )
 
-LimitQueryParam: Optional[int] = Query(default=None, title="Limit number of queries.")
+LimitQueryParam: Optional[int] = Query(default=None, ge=1, title="Limit number of queries.")
 
 OffsetQueryParam: Optional[int] = Query(
     default=0,
+    ge=0,
     title="Number of workflows to skip in sorted query (to enable pagination).",
 )
 
 InstanceQueryParam = Annotated[
     Optional[bool],
     Query(
         title="True when fetching by Workflow ID, False when fetching by StoredWorkflow ID.",
@@ -1222,22 +1226,24 @@
         description="Set to false to only include terminal Invocations.",
     ),
 ]
 
 InvocationsLimitQueryParam = Annotated[
     Optional[int],
     Query(
+        ge=1,
         title="Limit",
         description="Limit the number of invocations to return.",
     ),
 ]
 
 InvocationsOffsetQueryParam = Annotated[
     Optional[int],
     Query(
+        ge=0,
         title="Offset",
         description="Number of invocations to skip.",
     ),
 ]
 
 
 CreateInvocationsFromStoreBody = Annotated[
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/buildapp.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/buildapp.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/admin.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/admin.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/admin_toolshed.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/admin_toolshed.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/async.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/async.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/authnz.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/authnz.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/data_manager.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/data_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/dataset.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/dataset.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/forms.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/forms.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/history.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/history.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/page.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/page.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/root.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/root.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/shed_tool_static.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/shed_tool_static.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/tag.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/tag.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/tool_runner.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/tool_runner.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/user.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/user.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/visualization.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/visualization.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/workflow.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/controllers/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from galaxy.managers.sharable import SlugBuilder
 from galaxy.managers.workflows import (
     MissingToolsException,
     WorkflowUpdateOptions,
 )
 from galaxy.model.base import transaction
 from galaxy.model.item_attrs import UsesItemRatings
-from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.tools.parameters.workflow_utils import workflow_building_modes
 from galaxy.util import FILENAME_VALID_CHARS
 from galaxy.util.sanitize_html import sanitize_html
 from galaxy.web import url_for
 from galaxy.webapps.base.controller import (
     BaseUIController,
     SharableMixin,
     UsesStoredWorkflowMixin,
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/fast_app.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/fast_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from starlette.middleware.cors import CORSMiddleware
 from starlette.responses import Response
 
 from galaxy.schema.invocation import CustomJsonSchema
 from galaxy.version import VERSION
 from galaxy.webapps.base.api import (
     add_exception_handler,
+    add_raw_context_middlewares,
     add_request_id_middleware,
     GalaxyFileResponse,
     include_all_package_routers,
 )
 from galaxy.webapps.base.webapp import config_allows_origin
 from galaxy.webapps.openapi.utils import get_openapi
 
@@ -175,15 +176,18 @@
 
 
 def initialize_fast_app(gx_wsgi_webapp, gx_app):
     root_path = "" if gx_app.config.galaxy_url_prefix == "/" else gx_app.config.galaxy_url_prefix
     app = get_fastapi_instance(root_path=root_path)
     add_exception_handler(app)
     add_galaxy_middleware(app, gx_app)
-    add_request_id_middleware(app)
+    if gx_app.config.use_access_logging_middleware:
+        add_raw_context_middlewares(app)
+    else:
+        add_request_id_middleware(app)
     include_all_package_routers(app, "galaxy.webapps.galaxy.api")
     include_legacy_openapi(app, gx_app)
     wsgi_handler = WSGIMiddleware(gx_wsgi_webapp)
     gx_app.haltables.append(("WSGI Middleware threadpool", wsgi_handler.executor.shutdown))
     app.mount("/", wsgi_handler)  # type: ignore[arg-type]
     if gx_app.config.galaxy_url_prefix != "/":
         parent_app = FastAPI()
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/fast_factory.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/fast_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/_fetch_util.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/_fetch_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/authenticate.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/authenticate.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/base.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/base.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/dataset_collections.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/dataset_collections.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/datasets.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/help.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/help.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/histories.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/histories.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/history_contents.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/history_contents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1441,14 +1441,17 @@
         item.update()
 
     def _undelete(self, item: HistoryItemModel):
         if getattr(item, "purged", False):
             raise exceptions.ItemDeletionException("This item has been permanently deleted and cannot be recovered.")
         manager = self._get_item_manager(item)
         manager.undelete(item, flush=self.flush)
+        # Again, we need to force an update in the edge case where all selected items are already undeleted
+        # or when the item was purged as undelete will not trigger an update
+        item.update()
 
     def _purge(self, item: HistoryItemModel, trans: ProvidesHistoryContext):
         if getattr(item, "purged", False):
             # TODO: remove this `update` when we can properly track the operation results to notify the history
             item.update()
             return
         if isinstance(item, HistoryDatasetCollectionAssociation):
```

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/invocations.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/invocations.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/jobs.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/jobs.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/libraries.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/libraries.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/library_folder_contents.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/library_folder_contents.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/library_folders.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/library_folders.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/notifications.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/notifications.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/pages.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/pages.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/quotas.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/quotas.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/sharable.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/sharable.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/storage_cleaner.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/storage_cleaner.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/tool_shed_repositories.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/tool_shed_repositories.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/tools.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/users.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/users.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/visualizations.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/visualizations.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/workflows.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/galaxy/services/workflows.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/openapi/utils.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/app.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/app.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/buildapp.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/buildapp.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/config.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/config.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/history.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/history.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/home.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/home.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/jobs.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/jobs.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/query.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/query.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/system.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/system.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/tools.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/users.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/users.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/workflows.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/controllers/workflows.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/fast_app.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/fast_app.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/reports/fast_factory.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/reports/fast_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy/webapps/util.py` & `galaxy_web_apps-24.0.1/galaxy/webapps/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/PKG-INFO` & `galaxy_web_apps-24.0.1/galaxy_web_apps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-apps
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy web apps
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -78,14 +78,34 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Ensure that offset and limit are never negative by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18044 <https://github.com/galaxyproject/galaxy/pull/18044>`_
+* Fix history update time after bulk operation by `@davelopez <https://github.com/davelopez>`_ in `#18068 <https://github.com/galaxyproject/galaxy/pull/18068>`_
+
+============
+Enhancements
+============
+
+* Add middleware for logging start and end of request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18046 <https://github.com/galaxyproject/galaxy/pull/18046>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/SOURCES.txt` & `galaxy_web_apps-24.0.1/galaxy_web_apps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-24.0.0/setup.cfg` & `galaxy_web_apps-24.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-apps
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-app
 	galaxy-data
 	galaxy-job-execution
```

