# Comparing `tmp/sound_source_id-0.2.0.tar.gz` & `tmp/sound_source_id-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sound_source_id-0.2.0.tar", last modified: Mon Jun 19 14:24:00 2023, max compression
+gzip compressed data, was "sound_source_id-0.2.2.tar", last modified: Thu May  2 20:34:48 2024, max compression
```

## Comparing `sound_source_id-0.2.0.tar` & `sound_source_id-0.2.2.tar`

### file list

```diff
@@ -1,162 +1,164 @@
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:24:00.229461 sound_source_id-0.2.0/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.2.0/COPYING.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.2.0/MANIFEST.in
--rw-r--r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-19 14:24:00.229461 sound_source_id-0.2.0/PKG-INFO
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.2.0/README.md
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.765459 sound_source_id-0.2.0/icons/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.2.0/icons/audio-headphones.svgz
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 sound_source_id-0.2.0/icons/exit.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.2.0/icons/help-about.svgz
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.2.0/icons/help-contents.svgz
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.2.0/icons/help-contextual.svgz
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.2.0/icons/point-left.svg
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    21662 2023-06-06 21:15:49.000000 sound_source_id-0.2.0/icons/point-right.ico
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.2.0/icons/point-right.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.2.0/icons/preferences-other.svgz
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.765459 sound_source_id-0.2.0/make_noises/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.2.0/make_noises/make_pink_noises.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.2.0/make_noises/sndlib.py
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.781459 sound_source_id-0.2.0/prep-release/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2023-06-19 14:23:16.000000 sound_source_id-0.2.0/prep-release/minor_minor_number.txt
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.2.0/prep-release/mkupdate_pyqt5.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      547 2023-06-12 14:48:08.000000 sound_source_id-0.2.0/prep-release/mkupdate_pyqt6.sh
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      184 2023-06-08 21:48:18.000000 sound_source_id-0.2.0/prep-release/pypi_build.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3825 2023-06-19 14:22:29.000000 sound_source_id-0.2.0/prep-release/release.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      478 2023-06-12 14:47:06.000000 sound_source_id-0.2.0/prep-release/sound_source_id.pro
--rw-r--r--   0 sam       (1000) extdrive  (1777)    22230 2023-06-19 14:23:36.000000 sound_source_id-0.2.0/prep-release/sound_source_id_el.ts
--rw-r--r--   0 sam       (1000) extdrive  (1777)    22230 2023-06-19 14:23:36.000000 sound_source_id-0.2.0/prep-release/sound_source_id_en_GB.ts
--rw-r--r--   0 sam       (1000) extdrive  (1777)    22230 2023-06-19 14:23:36.000000 sound_source_id-0.2.0/prep-release/sound_source_id_en_US.ts
--rw-r--r--   0 sam       (1000) extdrive  (1777)    22230 2023-06-19 14:23:36.000000 sound_source_id-0.2.0/prep-release/sound_source_id_es.ts
--rw-r--r--   0 sam       (1000) extdrive  (1777)    22850 2023-06-19 14:23:36.000000 sound_source_id-0.2.0/prep-release/sound_source_id_fr.ts
--rw-r--r--   0 sam       (1000) extdrive  (1777)    22235 2023-06-19 14:23:36.000000 sound_source_id-0.2.0/prep-release/sound_source_id_it.ts
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.2.0/prep-release/switch_pyqt5.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.2.0/prep-release/switch_pyqt6.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      217 2023-06-08 21:49:59.000000 sound_source_id-0.2.0/prep-release/win_installer_readme.md
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      146 2023-06-07 10:17:57.000000 sound_source_id-0.2.0/prep-release/win_launch_iss_compiler.bat
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-07 17:49:12.000000 sound_source_id-0.2.0/prep-release/win_launch_iss_compiler.sh
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     3982 2023-06-19 14:23:17.000000 sound_source_id-0.2.0/prep-release/win_sound_source_id.iss
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      773 2023-06-12 15:13:58.000000 sound_source_id-0.2.0/prep-release/winbuild.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1307 2023-06-19 14:23:17.000000 sound_source_id-0.2.0/pyproject.toml
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.2.0/resources.qrc
--rw-r--r--   0 sam       (1000) extdrive  (1777)       38 2023-06-19 14:24:00.229461 sound_source_id-0.2.0/setup.cfg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      925 2023-06-19 14:23:17.000000 sound_source_id-0.2.0/setup_cx.py
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.789459 sound_source_id-0.2.0/sound_source_id/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.2.0/sound_source_id/__init__.py
--rwxr-xr-x   0 sam       (1000) extdrive  (1777)    65067 2023-06-19 14:14:26.000000 sound_source_id-0.2.0/sound_source_id/__main__.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2023-06-19 14:23:17.000000 sound_source_id-0.2.0/sound_source_id/_version_info.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.2.0/sound_source_id/audio_manager.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    19849 2023-06-11 08:20:40.000000 sound_source_id-0.2.0/sound_source_id/dialog_edit_preferences.py
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    15831 2023-06-11 08:22:26.000000 sound_source_id-0.2.0/sound_source_id/dialog_edit_transducers.py
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.801459 sound_source_id-0.2.0/sound_source_id/doc/
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.801459 sound_source_id-0.2.0/sound_source_id/doc/Figures/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.0/sound_source_id/doc/Figures/edit_transducers.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.0/sound_source_id/doc/Figures/sound_source_id_screenshot.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.0/sound_source_id/doc/Figures/stim_file.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.2.0/sound_source_id/doc/Makefile
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:58.381452 sound_source_id-0.2.0/sound_source_id/doc/_build/
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.805459 sound_source_id-0.2.0/sound_source_id/doc/_build/html/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/.buildinfo
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.837459 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_images/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_images/edit_transducers.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_images/stim_file.png
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.877460 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/calibration.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/index.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/installation.rst.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/intro.rst.txt
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:24:00.009460 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/basic.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/doctools.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/documentation_options.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/file.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/jquery.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/language_data.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/minus.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/plus.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/pygments.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/searchtools.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/underscore.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     7861 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/calibration.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    11522 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/experiment_setup.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     3976 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/genindex.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6000 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/index.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     7384 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/installation.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6034 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/intro.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      492 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/objects.inv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4375 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/search.html
--rw-r--r--   0 sam       (1000) extdrive  (1777)     5362 2023-06-19 14:23:39.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/html/searchindex.js
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:24:00.025460 sound_source_id-0.2.0/sound_source_id/doc/_build/latex/
--rw-r--r--   0 sam       (1000) extdrive  (1777)   223073 2023-06-19 14:23:47.000000 sound_source_id-0.2.0/sound_source_id/doc/_build/latex/sound_source_id.pdf
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.0/sound_source_id/doc/calibration.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2023-06-19 14:23:17.000000 sound_source_id-0.2.0/sound_source_id/doc/conf.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-11 14:03:05.000000 sound_source_id-0.2.0/sound_source_id/doc/experiment_setup.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.0/sound_source_id/doc/index.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.2.0/sound_source_id/doc/installation.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.0/sound_source_id/doc/intro.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.2.0/sound_source_id/doc/make.bat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.2.0/sound_source_id/doc/mkdoc.sh
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10178 2023-06-11 08:22:53.000000 sound_source_id-0.2.0/sound_source_id/global_parameters.py
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:24:00.033460 sound_source_id-0.2.0/sound_source_id/prm_files/
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:24:00.229461 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise1.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise10.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise11.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise12.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise13.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise14.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise15.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise16.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise17.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise18.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise19.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise2.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise20.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise21.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise22.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise23.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise24.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise25.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise26.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise27.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise28.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise29.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise3.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise30.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise4.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise5.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise6.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise7.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise8.wav
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise9.wav
--rw-r--r--   0 sam       (1000) extdrive  (1777)      389 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      198 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm_2_targets.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      624 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm_circle_36_targets.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      421 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm_virtual.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      326 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm_virtual_2_targets.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      356 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm_virtual_4_front_back.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      427 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm_virtual_circle_12_targets.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      751 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      646 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)     1257 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/stim_list.csv
--rw-r--r--   0 sam       (1000) extdrive  (1777)      459 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_2_speak.csv
--rw-r--r--   0 sam       (1000) extdrive  (1777)      759 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_4_front_back.csv
--rw-r--r--   0 sam       (1000) extdrive  (1777)      710 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_8_az_2_elev.csv
--rw-r--r--   0 sam       (1000) extdrive  (1777)     1521 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_circle.csv
--rw-r--r--   0 sam       (1000) extdrive  (1777)      541 2023-06-19 10:37:35.000000 sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_circle_12_tgs.csv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2023-06-19 14:20:35.000000 sound_source_id-0.2.0/sound_source_id/pyqtver.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)  4039631 2023-06-19 14:23:36.000000 sound_source_id-0.2.0/sound_source_id/qrc_resources.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   175964 2023-05-04 21:44:23.000000 sound_source_id-0.2.0/sound_source_id/sndlib.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      991 2023-06-11 08:24:39.000000 sound_source_id-0.2.0/sound_source_id/utils.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.2.0/sound_source_id/wavpy.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.2.0/sound_source_id/wavpy_sndf.py
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-19 14:23:59.789459 sound_source_id-0.2.0/sound_source_id.egg-info/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    41505 2023-06-19 14:23:58.000000 sound_source_id-0.2.0/sound_source_id.egg-info/PKG-INFO
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6031 2023-06-19 14:23:58.000000 sound_source_id-0.2.0/sound_source_id.egg-info/SOURCES.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2023-06-19 14:23:58.000000 sound_source_id-0.2.0/sound_source_id.egg-info/dependency_links.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       62 2023-06-19 14:23:58.000000 sound_source_id-0.2.0/sound_source_id.egg-info/entry_points.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       86 2023-06-19 14:23:58.000000 sound_source_id-0.2.0/sound_source_id.egg-info/requires.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       16 2023-06-19 14:23:58.000000 sound_source_id-0.2.0/sound_source_id.egg-info/top_level.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1054 2024-02-05 09:35:07.000000 sound_source_id-0.2.2/.readthedocs.yaml
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.2.2/COPYING.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.2.2/MANIFEST.in
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    41711 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/PKG-INFO
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.2.2/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.812944 sound_source_id-0.2.2/icons/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.2.2/icons/audio-headphones.svgz
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 sound_source_id-0.2.2/icons/exit.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.2.2/icons/help-about.svgz
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.2.2/icons/help-contents.svgz
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.2.2/icons/help-contextual.svgz
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.2.2/icons/point-left.svg
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    21662 2023-06-06 21:15:49.000000 sound_source_id-0.2.2/icons/point-right.ico
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.2.2/icons/point-right.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.2.2/icons/preferences-other.svgz
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.812944 sound_source_id-0.2.2/make_noises/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.2.2/make_noises/make_pink_noises.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.2.2/make_noises/sndlib.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.912944 sound_source_id-0.2.2/prep-release/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/prep-release/minor_minor_number.txt
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.2.2/prep-release/mkupdate_pyqt5.sh
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2023-06-12 14:48:08.000000 sound_source_id-0.2.2/prep-release/mkupdate_pyqt6.sh
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      184 2023-06-08 21:48:18.000000 sound_source_id-0.2.2/prep-release/pypi_build.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3821 2024-05-02 15:25:43.000000 sound_source_id-0.2.2/prep-release/release.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      478 2023-06-12 14:47:06.000000 sound_source_id-0.2.2/prep-release/sound_source_id.pro
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    22230 2023-06-19 21:36:07.000000 sound_source_id-0.2.2/prep-release/sound_source_id_el.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-02 20:34:25.000000 sound_source_id-0.2.2/prep-release/sound_source_id_en_GB.ts
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    22230 2023-06-19 21:36:07.000000 sound_source_id-0.2.2/prep-release/sound_source_id_en_US.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    20770 2024-05-02 20:34:25.000000 sound_source_id-0.2.2/prep-release/sound_source_id_es.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    21950 2024-05-02 20:34:25.000000 sound_source_id-0.2.2/prep-release/sound_source_id_fr.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    21015 2024-05-02 20:34:25.000000 sound_source_id-0.2.2/prep-release/sound_source_id_it.ts
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.2.2/prep-release/switch_pyqt5.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.2.2/prep-release/switch_pyqt6.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      217 2023-06-08 21:49:59.000000 sound_source_id-0.2.2/prep-release/win_installer_readme.md
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      146 2023-06-07 10:17:57.000000 sound_source_id-0.2.2/prep-release/win_launch_iss_compiler.bat
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-07 17:49:12.000000 sound_source_id-0.2.2/prep-release/win_launch_iss_compiler.sh
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     3982 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/prep-release/win_sound_source_id.iss
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      773 2023-06-12 15:13:58.000000 sound_source_id-0.2.2/prep-release/winbuild.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1330 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/pyproject.toml
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.2.2/resources.qrc
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/setup.cfg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1847 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/setup_cx.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.920944 sound_source_id-0.2.2/sound_source_id/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.2.2/sound_source_id/__init__.py
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)    65651 2024-05-02 19:48:18.000000 sound_source_id-0.2.2/sound_source_id/__main__.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/sound_source_id/_version_info.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.2.2/sound_source_id/audio_manager.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    19849 2023-06-11 08:20:40.000000 sound_source_id-0.2.2/sound_source_id/dialog_edit_preferences.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    15831 2023-06-11 08:22:26.000000 sound_source_id-0.2.2/sound_source_id/dialog_edit_transducers.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.960944 sound_source_id-0.2.2/sound_source_id/doc/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.996945 sound_source_id-0.2.2/sound_source_id/doc/Figures/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.2/sound_source_id/doc/Figures/edit_transducers.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.2/sound_source_id/doc/Figures/sound_source_id_screenshot.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.2/sound_source_id/doc/Figures/stim_file.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.2.2/sound_source_id/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:46.736943 sound_source_id-0.2.2/sound_source_id/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.000944 sound_source_id-0.2.2/sound_source_id/doc/_build/html/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.052945 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    20275 2023-06-11 13:37:55.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/edit_transducers.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/stim_file.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.336946 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/calibration.rst.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/index.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/installation.rst.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/intro.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.680948 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/basic.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/doctools.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/documentation_options.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/file.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/jquery.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/language_data.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/minus.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/plus.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/pygments.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/searchtools.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/underscore.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7861 2024-05-02 20:34:31.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/calibration.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    11522 2024-05-02 20:34:31.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/experiment_setup.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     3976 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/genindex.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6000 2024-05-02 20:34:31.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/index.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7384 2024-05-02 20:34:31.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/installation.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6034 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/intro.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      492 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/objects.inv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4375 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5375 2024-05-02 20:34:32.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/html/searchindex.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:47.728948 sound_source_id-0.2.2/sound_source_id/doc/_build/latex/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   223206 2024-05-02 20:34:36.000000 sound_source_id-0.2.2/sound_source_id/doc/_build/latex/sound_source_id.pdf
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2248 2023-06-11 14:05:30.000000 sound_source_id-0.2.2/sound_source_id/doc/calibration.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2024-05-02 20:34:16.000000 sound_source_id-0.2.2/sound_source_id/doc/conf.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-11 14:03:05.000000 sound_source_id-0.2.2/sound_source_id/doc/experiment_setup.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      521 2023-06-11 14:02:33.000000 sound_source_id-0.2.2/sound_source_id/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2024-05-02 15:24:49.000000 sound_source_id-0.2.2/sound_source_id/doc/installation.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.2.2/sound_source_id/doc/intro.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.2.2/sound_source_id/doc/make.bat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.2.2/sound_source_id/doc/mkdoc.sh
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       18 2024-02-05 09:32:26.000000 sound_source_id-0.2.2/sound_source_id/doc/requirements.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9341 2024-04-25 10:53:08.000000 sound_source_id-0.2.2/sound_source_id/global_parameters.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:48.124950 sound_source_id-0.2.2/sound_source_id/prm_files/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise1.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise10.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise11.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise12.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise13.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise14.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise15.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise16.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise17.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise18.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise19.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise2.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise20.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise21.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise22.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise23.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise24.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise25.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise26.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise27.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise28.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise29.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise3.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise30.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise4.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise5.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise6.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise7.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise8.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise9.wav
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      389 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      198 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_2_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      624 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_circle_36_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      421 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      326 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_2_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      356 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_4_front_back.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      427 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_12_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      751 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      646 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1257 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      459 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_2_speak.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      759 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_4_front_back.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      710 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_8_az_2_elev.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1521 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_circle.csv
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      541 2023-06-19 10:37:35.000000 sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_circle_12_tgs.csv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2024-05-02 20:34:12.000000 sound_source_id-0.2.2/sound_source_id/pyqtver.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)  2972123 2024-05-02 20:34:29.000000 sound_source_id-0.2.2/sound_source_id/qrc_resources.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   175964 2023-05-04 21:44:23.000000 sound_source_id-0.2.2/sound_source_id/sndlib.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      991 2023-06-11 08:24:39.000000 sound_source_id-0.2.2/sound_source_id/utils.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.2.2/sound_source_id/wavpy.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.2.2/sound_source_id/wavpy_sndf.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:34:48.732953 sound_source_id-0.2.2/sound_source_id.egg-info/
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    41711 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/PKG-INFO
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6086 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/SOURCES.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/dependency_links.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       62 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/entry_points.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      101 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/requires.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       16 2024-05-02 20:34:46.000000 sound_source_id-0.2.2/sound_source_id.egg-info/top_level.txt
```

### Comparing `sound_source_id-0.2.0/COPYING.txt` & `sound_source_id-0.2.2/COPYING.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/PKG-INFO` & `sound_source_id-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound_source_id
-Version: 0.2.0
+Version: 0.2.2
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,9 +689,16 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING.txt
+Requires-Dist: matplotlib>=3.0.0
+Requires-Dist: numpy>=1.0.0
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: PyAudio>=0.2.11
+Requires-Dist: PyQt6>=6.6.0
+Requires-Dist: scipy>=1.0.1
+Requires-Dist: pysofa>=0.1.1
 
 Python program for sound localization tests.
```

### Comparing `sound_source_id-0.2.0/icons/audio-headphones.svgz` & `sound_source_id-0.2.2/icons/audio-headphones.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/icons/exit.svg` & `sound_source_id-0.2.2/icons/exit.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/icons/help-about.svgz` & `sound_source_id-0.2.2/icons/help-about.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/icons/help-contents.svgz` & `sound_source_id-0.2.2/icons/help-contents.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/icons/help-contextual.svgz` & `sound_source_id-0.2.2/icons/help-contextual.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/icons/point-left.svg` & `sound_source_id-0.2.2/icons/point-left.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/icons/point-right.ico` & `sound_source_id-0.2.2/icons/point-right.ico`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/icons/point-right.svg` & `sound_source_id-0.2.2/icons/point-right.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/icons/preferences-other.svgz` & `sound_source_id-0.2.2/icons/preferences-other.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/make_noises/make_pink_noises.py` & `sound_source_id-0.2.2/make_noises/make_pink_noises.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/make_noises/sndlib.py` & `sound_source_id-0.2.2/make_noises/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/prep-release/mkupdate_pyqt6.sh` & `sound_source_id-0.2.2/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/prep-release/release.py` & `sound_source_id-0.2.2/prep-release/release.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,22 @@
     for opt, arg in opts:
         if opt in ("-m", "--message"):
             message = arg
     major_v = 0
     minor_v = 2
 
     pyqtver = input('pyqtver: ')
-    if pyqtver == 5:
-        os.system("python3 prep-release/switch_pyqt5.py")
-        os.system("python3 prep-release/mkupdate_pyqt5")
-    elif pyqtver == 6:
-        os.system("python3 prep-release/switch_pyqt6.py")
-        os.system("python3 prep-release/mkupdate_pyqt6")
+    os.chdir('prep-release/')
+    if pyqtver == '5':
+        os.system("python3 switch_pyqt5.py")
+        os.system("./mkupdate_pyqt5.sh")
+    elif pyqtver == '6':
+        os.system("python3 switch_pyqt6.py")
+        os.system("./mkupdate_pyqt6.sh")
+    os.chdir('../')
         
     #read minor minor release number
     f = open('prep-release/minor_minor_number.txt', 'r')
     ln = f.readlines()
     f.close()
     minor_minor_v = int(ln[0].strip()) + 1
     #write incremented minor minor release number
```

### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_el.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_el.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_en_GB.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_en_US.ts`

 * *Files 0% similar despite different names*

#### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_en_GB.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_en_US.ts`

 * *Ordering differences only*

```diff
@@ -136,19 +136,14 @@
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="187"/>
       <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="191"/>
-      <source>Transducers</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
       <location filename="../sound_source_id/__main__.py" line="196"/>
       <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="198"/>
       <source>Manual (html)</source>
@@ -161,44 +156,14 @@
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="952"/>
       <source>About sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="210"/>
-      <source>Show Play Buttons</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
-      <source>Warning</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="248"/>
-      <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="263"/>
-      <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="603"/>
-      <source>Start</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="288"/>
-      <source>Run Demo</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
       <location filename="../sound_source_id/__main__.py" line="411"/>
       <source>Loaded</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="411"/>
       <source>parameter file</source>
@@ -216,14 +181,19 @@
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="536"/>
       <source>Choose file to write results</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../sound_source_id/__main__.py" line="591"/>
+      <source>Warning</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../sound_source_id/__main__.py" line="569"/>
       <source>You need to select a file where to save the results to proceed</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="573"/>
       <source>Please, enter the listener's name:</source>
@@ -268,14 +238,44 @@
                               &lt;p&gt;
                               You should have received a copy of the GNU General Public License
                               along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
                               &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <source>Start</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="288"/>
+      <source>Run Demo</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="248"/>
+      <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="263"/>
+      <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="210"/>
+      <source>Show Play Buttons</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="191"/>
+      <source>Transducers</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../sound_source_id/__main__.py" line="225"/>
       <source>Listener:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="214"/>
       <source>Show Response Buttons</source>
@@ -341,19 +341,14 @@
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="91"/>
       <source>CSV separator:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/dialog_edit_preferences.py" line="113"/>
-      <source>Transducers:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="122"/>
       <source>Play Command:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="127"/>
       <source>Command:</source>
@@ -410,14 +405,19 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="349"/>
       <source>There are unsaved changes. Apply Changes?</source>
       <translation type="unfinished"/>
     </message>
+    <message>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="113"/>
+      <source>Transducers:</source>
+      <translation type="unfinished"/>
+    </message>
   </context>
   <context>
     <name>responseLight</name>
     <message>
       <location filename="../sound_source_id/__main__.py" line="1134"/>
       <source>Light &amp; Text</source>
       <translation type="unfinished"/>
```

### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_en_US.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_it.ts`

 * *Files 22% similar despite different names*

#### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_en_US.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_it.ts`

```diff
@@ -1,328 +1,265 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1">
+<TS version="2.1" language="it_IT" sourcelanguage="en_US">
   <context>
     <name/>
     <message>
       <location filename="../sound_source_id/global_parameters.py" line="167"/>
+      <location filename="../sound_source_id/global_parameters.py" line="164"/>
+      <location filename="../sound_source_id/global_parameters.py" line="87"/>
       <source>custom</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
-    <name>Preferences Window</name>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="91"/>
-      <source>System Settings</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="92"/>
-      <source>en</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="93"/>
-      <source>it</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="94"/>
-      <source>fr</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="95"/>
-      <source>es</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="96"/>
-      <source>el</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="99"/>
-      <source>US</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="100"/>
-      <source>GB</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="102"/>
-      <source>IT</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="103"/>
-      <source>CH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="104"/>
-      <source>FR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="105"/>
-      <source>CA</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="107"/>
-      <source>ES</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="108"/>
-      <source>BO</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="109"/>
-      <source>CL</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="111"/>
-      <source>GR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="112"/>
-      <source>CY</source>
-      <translation type="unfinished"/>
-    </message>
-  </context>
-  <context>
     <name>applicationWindow</name>
     <message>
       <location filename="../sound_source_id/__main__.py" line="149"/>
       <source>sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="169"/>
       <source>&amp;File</source>
-      <translation type="unfinished"/>
+      <translation>&amp;File</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="272"/>
+      <location filename="../sound_source_id/__main__.py" line="277"/>
+      <location filename="../sound_source_id/__main__.py" line="171"/>
       <source>Load Parameters</source>
-      <translation type="unfinished"/>
+      <translation>Carica parametri</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="173"/>
       <source>Load Parameters File</source>
-      <translation type="unfinished"/>
+      <translation>Carica file dei parametri</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="178"/>
       <source>Exit</source>
-      <translation type="unfinished"/>
+      <translation>Esci</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="180"/>
       <source>Exit application</source>
-      <translation type="unfinished"/>
+      <translation>Esci dall'applicazione</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="186"/>
       <source>&amp;Edit</source>
-      <translation type="unfinished"/>
+      <translation>&amp;Modifica</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="187"/>
       <source>Preferences</source>
+      <translation>Preferenze</translation>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="191"/>
+      <source>Transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="196"/>
       <source>&amp;Help</source>
-      <translation type="unfinished"/>
+      <translation>&amp;Aiuto</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="198"/>
       <source>Manual (html)</source>
-      <translation type="unfinished"/>
+      <translation>Manuale (html)</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="202"/>
       <source>Manual (pdf)</source>
-      <translation type="unfinished"/>
+      <translation>Manuale (pdf)</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="964"/>
+      <location filename="../sound_source_id/__main__.py" line="206"/>
       <source>About sound_source_id</source>
-      <translation type="unfinished"/>
+      <translation>A proposito di sound_source_id</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
-      <source>Loaded</source>
+      <location filename="../sound_source_id/__main__.py" line="210"/>
+      <source>Show Play Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
-      <source>parameter file</source>
+      <location filename="../sound_source_id/__main__.py" line="214"/>
+      <source>Show Response Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
-      <source>Choose parameters file to load</source>
+      <location filename="../sound_source_id/__main__.py" line="219"/>
+      <source>Show Response Lights</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
-      <source>All Files (*)</source>
+      <location filename="../sound_source_id/__main__.py" line="224"/>
+      <source>Show Control Panel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
-      <source>Choose file to write results</source>
+      <location filename="../sound_source_id/__main__.py" line="230"/>
+      <source>Listener:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <location filename="../sound_source_id/__main__.py" line="427"/>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="569"/>
-      <source>You need to select a file where to save the results to proceed</source>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
+      <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="573"/>
-      <source>Please, enter the listener's name:</source>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
+      <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="574"/>
-      <source>Input Dialog:</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="615"/>
+      <location filename="../sound_source_id/__main__.py" line="602"/>
+      <location filename="../sound_source_id/__main__.py" line="426"/>
+      <location filename="../sound_source_id/__main__.py" line="272"/>
+      <source>Start</source>
+      <translation>Inizia</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="729"/>
-      <source>Running</source>
+      <location filename="../sound_source_id/__main__.py" line="282"/>
+      <source>Choose Results File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="841"/>
-      <source>Run Block</source>
+      <location filename="../sound_source_id/__main__.py" line="288"/>
+      <source>Reset</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="844"/>
-      <source>Finished</source>
+      <location filename="../sound_source_id/__main__.py" line="293"/>
+      <source>Run Demo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
-      <source>&lt;b&gt;sound_source_id - Python app for sound localization experiments&lt;/b&gt; &lt;br&gt;
-                              - version: {0}; &lt;br&gt;
-                              - build date: {1} &lt;br&gt;
-                              &lt;p&gt; Copyright &amp;copy; 2022-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
-                              All rights reserved. &lt;p&gt;
-                              This program is free software: you can redistribute it and/or modify
-                              it under the terms of the GNU General Public License as published by
-                              the Free Software Foundation, either version 3 of the License, or
-                              (at your option) any later version.
-                              &lt;p&gt;
-                              This program is distributed in the hope that it will be useful,
-                              but WITHOUT ANY WARRANTY; without even the implied warranty of
-                              MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-                              GNU General Public License for more details.
-                              &lt;p&gt;
-                              You should have received a copy of the GNU General Public License
-                              along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
-                              &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
+      <source>Loaded</source>
+      <translation>Caricati</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="603"/>
-      <source>Start</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
+      <source>parameter file</source>
+      <translation>file dei parametri</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="288"/>
-      <source>Run Demo</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="856"/>
+      <location filename="../sound_source_id/__main__.py" line="602"/>
+      <location filename="../sound_source_id/__main__.py" line="426"/>
+      <source>Finished</source>
+      <translation>Finito</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="248"/>
-      <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="427"/>
+      <source>This will stop the current test. Are you sure you want to proceed?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="263"/>
-      <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
+      <location filename="../sound_source_id/__main__.py" line="431"/>
+      <source>Choose parameters file to load</source>
+      <translation>Scegli il file dei parametri da caricare</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="210"/>
-      <source>Show Play Buttons</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
+      <location filename="../sound_source_id/__main__.py" line="431"/>
+      <source>All Files (*)</source>
+      <translation>Tutti i file (*)</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="191"/>
-      <source>Transducers</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
+      <source>Choose file to write results</source>
+      <translation>Scegli il file dove salvare i risultati</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="225"/>
-      <source>Listener:</source>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
+      <source>csv (*.csv)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="214"/>
-      <source>Show Response Buttons</source>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <source>File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="219"/>
-      <source>Show Response Lights</source>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <source>already exists. Do you want to overwrite it?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="277"/>
-      <source>Choose Results File</source>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
+      <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="283"/>
-      <source>Reset</source>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
+      <source>You need to select a file where to save the results to proceed</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
-      <source>This will stop the current test. Are you sure you want to proceed?</source>
+      <location filename="../sound_source_id/__main__.py" line="585"/>
+      <source>Please, enter the listener's name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="560"/>
-      <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
+      <location filename="../sound_source_id/__main__.py" line="586"/>
+      <source>Input Dialog:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
-      <source>csv (*.csv)</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="741"/>
+      <location filename="../sound_source_id/__main__.py" line="597"/>
+      <location filename="../sound_source_id/__main__.py" line="593"/>
+      <source>Running</source>
+      <translation>In esecuzione</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
-      <source>File</source>
-      <translation type="unfinished"/>
+      <location filename="../sound_source_id/__main__.py" line="853"/>
+      <source>Run Block</source>
+      <translation>Inizia blocco</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
-      <source>already exists. Do you want to overwrite it?</source>
+      <location filename="../sound_source_id/__main__.py" line="965"/>
+      <source>&lt;b&gt;sound_source_id - Python app for sound localization experiments&lt;/b&gt; &lt;br&gt;
+                              - version: {0}; &lt;br&gt;
+                              - build date: {1} &lt;br&gt;
+                              &lt;p&gt; Copyright &amp;copy; 2022-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
+                              All rights reserved. &lt;p&gt;
+                              This program is free software: you can redistribute it and/or modify
+                              it under the terms of the GNU General Public License as published by
+                              the Free Software Foundation, either version 3 of the License, or
+                              (at your option) any later version.
+                              &lt;p&gt;
+                              This program is distributed in the hope that it will be useful,
+                              but WITHOUT ANY WARRANTY; without even the implied warranty of
+                              MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+                              GNU General Public License for more details.
+                              &lt;p&gt;
+                              You should have received a copy of the GNU General Public License
+                              along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
+                              &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>preferencesDialog</name>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="65"/>
@@ -341,30 +278,39 @@
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="91"/>
       <source>CSV separator:</source>
       <translation type="unfinished"/>
     </message>
     <message>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="113"/>
+      <source>Transducers:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="122"/>
       <source>Play Command:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="127"/>
       <source>Command:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="329"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="135"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="130"/>
       <source>custom</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="156"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="142"/>
       <source>Device:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="173"/>
       <source>Buffer Size (samples):</source>
       <translation type="unfinished"/>
@@ -405,54 +351,63 @@
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="349"/>
       <source>There are unsaved changes. Apply Changes?</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../sound_source_id/dialog_edit_preferences.py" line="113"/>
-      <source>Transducers:</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>responseLight</name>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1134"/>
+      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
+      <location filename="../sound_source_id/__main__.py" line="1062"/>
+      <location filename="../sound_source_id/__main__.py" line="1049"/>
       <source>Light &amp; Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1122"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1158"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1168"/>
+      <location filename="../sound_source_id/__main__.py" line="1180"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light &amp; Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1116"/>
+      <location filename="../sound_source_id/__main__.py" line="1128"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
       <source>Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1153"/>
+      <location filename="../sound_source_id/__main__.py" line="1165"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
       <source>Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1127"/>
+      <location filename="../sound_source_id/__main__.py" line="1139"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
       <source>Smiley</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>transducersDialog</name>
     <message>
@@ -488,14 +443,16 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="167"/>
       <source>Edit Transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="192"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="179"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="179"/>
       <source>Only one label can be renamed at a time</source>
       <translation type="unfinished"/>
@@ -503,27 +460,28 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="184"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="198"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="185"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="192"/>
       <source>Only one item can be edited at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="197"/>
       <source>Level:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/dialog_edit_transducers.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="250"/>
       <source>Only one transducer left. Cannot remove!</source>
       <translation type="unfinished"/>
     </message>
   </context>
 </TS>
```

### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_es.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_en_GB.ts`

 * *Files 27% similar despite different names*

#### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_es.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_en_GB.ts`

```diff
@@ -1,120 +1,35 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
 <TS version="2.1">
   <context>
     <name/>
     <message>
       <location filename="../sound_source_id/global_parameters.py" line="167"/>
+      <location filename="../sound_source_id/global_parameters.py" line="164"/>
+      <location filename="../sound_source_id/global_parameters.py" line="87"/>
       <source>custom</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
-    <name>Preferences Window</name>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="91"/>
-      <source>System Settings</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="92"/>
-      <source>en</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="93"/>
-      <source>it</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="94"/>
-      <source>fr</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="95"/>
-      <source>es</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="96"/>
-      <source>el</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="99"/>
-      <source>US</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="100"/>
-      <source>GB</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="102"/>
-      <source>IT</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="103"/>
-      <source>CH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="104"/>
-      <source>FR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="105"/>
-      <source>CA</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="107"/>
-      <source>ES</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="108"/>
-      <source>BO</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="109"/>
-      <source>CL</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="111"/>
-      <source>GR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="112"/>
-      <source>CY</source>
-      <translation type="unfinished"/>
-    </message>
-  </context>
-  <context>
     <name>applicationWindow</name>
     <message>
       <location filename="../sound_source_id/__main__.py" line="149"/>
       <source>sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="169"/>
       <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="272"/>
+      <location filename="../sound_source_id/__main__.py" line="277"/>
+      <location filename="../sound_source_id/__main__.py" line="171"/>
       <source>Load Parameters</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="173"/>
       <source>Load Parameters File</source>
       <translation type="unfinished"/>
@@ -156,173 +71,195 @@
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="202"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="964"/>
+      <location filename="../sound_source_id/__main__.py" line="206"/>
       <source>About sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="210"/>
       <source>Show Play Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
-      <source>Warning</source>
+      <location filename="../sound_source_id/__main__.py" line="214"/>
+      <source>Show Response Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="248"/>
-      <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
+      <location filename="../sound_source_id/__main__.py" line="219"/>
+      <source>Show Response Lights</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="263"/>
-      <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
+      <location filename="../sound_source_id/__main__.py" line="224"/>
+      <source>Show Control Panel</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="230"/>
+      <source>Listener:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="603"/>
-      <source>Start</source>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <location filename="../sound_source_id/__main__.py" line="427"/>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
+      <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="288"/>
-      <source>Run Demo</source>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
+      <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
-      <source>Loaded</source>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
+      <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
-      <source>parameter file</source>
+      <location filename="../sound_source_id/__main__.py" line="615"/>
+      <location filename="../sound_source_id/__main__.py" line="602"/>
+      <location filename="../sound_source_id/__main__.py" line="426"/>
+      <location filename="../sound_source_id/__main__.py" line="272"/>
+      <source>Start</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
-      <source>Choose parameters file to load</source>
+      <location filename="../sound_source_id/__main__.py" line="282"/>
+      <source>Choose Results File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
-      <source>All Files (*)</source>
+      <location filename="../sound_source_id/__main__.py" line="288"/>
+      <source>Reset</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
-      <source>Choose file to write results</source>
+      <location filename="../sound_source_id/__main__.py" line="293"/>
+      <source>Run Demo</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="569"/>
-      <source>You need to select a file where to save the results to proceed</source>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
+      <source>Loaded</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="573"/>
-      <source>Please, enter the listener's name:</source>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
+      <source>parameter file</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="574"/>
-      <source>Input Dialog:</source>
+      <location filename="../sound_source_id/__main__.py" line="856"/>
+      <location filename="../sound_source_id/__main__.py" line="602"/>
+      <location filename="../sound_source_id/__main__.py" line="426"/>
+      <source>Finished</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="729"/>
-      <source>Running</source>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="427"/>
+      <source>This will stop the current test. Are you sure you want to proceed?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="841"/>
-      <source>Run Block</source>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
+      <location filename="../sound_source_id/__main__.py" line="431"/>
+      <source>Choose parameters file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="844"/>
-      <source>Finished</source>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
+      <location filename="../sound_source_id/__main__.py" line="431"/>
+      <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
-      <source>&lt;b&gt;sound_source_id - Python app for sound localization experiments&lt;/b&gt; &lt;br&gt;
-                              - version: {0}; &lt;br&gt;
-                              - build date: {1} &lt;br&gt;
-                              &lt;p&gt; Copyright &amp;copy; 2022-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
-                              All rights reserved. &lt;p&gt;
-                              This program is free software: you can redistribute it and/or modify
-                              it under the terms of the GNU General Public License as published by
-                              the Free Software Foundation, either version 3 of the License, or
-                              (at your option) any later version.
-                              &lt;p&gt;
-                              This program is distributed in the hope that it will be useful,
-                              but WITHOUT ANY WARRANTY; without even the implied warranty of
-                              MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-                              GNU General Public License for more details.
-                              &lt;p&gt;
-                              You should have received a copy of the GNU General Public License
-                              along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
-                              &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
+      <source>Choose file to write results</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="225"/>
-      <source>Listener:</source>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
+      <source>csv (*.csv)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="214"/>
-      <source>Show Response Buttons</source>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <source>File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="219"/>
-      <source>Show Response Lights</source>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <source>already exists. Do you want to overwrite it?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="277"/>
-      <source>Choose Results File</source>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
+      <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="283"/>
-      <source>Reset</source>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
+      <source>You need to select a file where to save the results to proceed</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
-      <source>This will stop the current test. Are you sure you want to proceed?</source>
+      <location filename="../sound_source_id/__main__.py" line="585"/>
+      <source>Please, enter the listener's name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="560"/>
-      <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
+      <location filename="../sound_source_id/__main__.py" line="586"/>
+      <source>Input Dialog:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
-      <source>csv (*.csv)</source>
+      <location filename="../sound_source_id/__main__.py" line="741"/>
+      <location filename="../sound_source_id/__main__.py" line="597"/>
+      <location filename="../sound_source_id/__main__.py" line="593"/>
+      <source>Running</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
-      <source>File</source>
+      <location filename="../sound_source_id/__main__.py" line="853"/>
+      <source>Run Block</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
-      <source>already exists. Do you want to overwrite it?</source>
+      <location filename="../sound_source_id/__main__.py" line="965"/>
+      <source>&lt;b&gt;sound_source_id - Python app for sound localization experiments&lt;/b&gt; &lt;br&gt;
+                              - version: {0}; &lt;br&gt;
+                              - build date: {1} &lt;br&gt;
+                              &lt;p&gt; Copyright &amp;copy; 2022-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
+                              All rights reserved. &lt;p&gt;
+                              This program is free software: you can redistribute it and/or modify
+                              it under the terms of the GNU General Public License as published by
+                              the Free Software Foundation, either version 3 of the License, or
+                              (at your option) any later version.
+                              &lt;p&gt;
+                              This program is distributed in the hope that it will be useful,
+                              but WITHOUT ANY WARRANTY; without even the implied warranty of
+                              MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+                              GNU General Public License for more details.
+                              &lt;p&gt;
+                              You should have received a copy of the GNU General Public License
+                              along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
+                              &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>preferencesDialog</name>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="65"/>
@@ -357,19 +294,23 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="127"/>
       <source>Command:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="329"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="135"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="130"/>
       <source>custom</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="156"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="142"/>
       <source>Device:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="173"/>
       <source>Buffer Size (samples):</source>
       <translation type="unfinished"/>
@@ -414,45 +355,59 @@
       <source>There are unsaved changes. Apply Changes?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>responseLight</name>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1134"/>
+      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
+      <location filename="../sound_source_id/__main__.py" line="1062"/>
+      <location filename="../sound_source_id/__main__.py" line="1049"/>
       <source>Light &amp; Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1122"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1158"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1168"/>
+      <location filename="../sound_source_id/__main__.py" line="1180"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light &amp; Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1116"/>
+      <location filename="../sound_source_id/__main__.py" line="1128"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
       <source>Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1153"/>
+      <location filename="../sound_source_id/__main__.py" line="1165"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
       <source>Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1127"/>
+      <location filename="../sound_source_id/__main__.py" line="1139"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
       <source>Smiley</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>transducersDialog</name>
     <message>
@@ -488,14 +443,16 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="167"/>
       <source>Edit Transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="192"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="179"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="179"/>
       <source>Only one label can be renamed at a time</source>
       <translation type="unfinished"/>
@@ -503,27 +460,28 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="184"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="198"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="185"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="192"/>
       <source>Only one item can be edited at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="197"/>
       <source>Level:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/dialog_edit_transducers.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="250"/>
       <source>Only one transducer left. Cannot remove!</source>
       <translation type="unfinished"/>
     </message>
   </context>
 </TS>
```

### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_fr.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_fr.ts`

 * *Files 17% similar despite different names*

#### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_fr.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_fr.ts`

```diff
@@ -1,104 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
 <TS version="2.1" language="fr_FR">
   <context>
     <name/>
     <message>
       <location filename="../sound_source_id/global_parameters.py" line="167"/>
+      <location filename="../sound_source_id/global_parameters.py" line="164"/>
+      <location filename="../sound_source_id/global_parameters.py" line="87"/>
       <source>custom</source>
       <translation type="unfinished">personnalisé</translation>
     </message>
   </context>
   <context>
     <name>Preferences Window</name>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="91"/>
       <source>System Settings</source>
-      <translation>Paramètre du système</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="92"/>
-      <source>en</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="93"/>
-      <source>it</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="94"/>
-      <source>fr</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="95"/>
-      <source>es</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="96"/>
-      <source>el</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="99"/>
-      <source>US</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="100"/>
-      <source>GB</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="102"/>
-      <source>IT</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="103"/>
-      <source>CH</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="104"/>
-      <source>FR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="105"/>
-      <source>CA</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="107"/>
-      <source>ES</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="108"/>
-      <source>BO</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="109"/>
-      <source>CL</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="111"/>
-      <source>GR</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/global_parameters.py" line="112"/>
-      <source>CY</source>
-      <translation type="unfinished"/>
+      <translation type="vanished">Paramètre du système</translation>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
       <location filename="../sound_source_id/__main__.py" line="149"/>
       <source>sound_source_id</source>
@@ -106,15 +27,16 @@
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="169"/>
       <source>&amp;File</source>
       <translation>&amp;Fichier</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="272"/>
+      <location filename="../sound_source_id/__main__.py" line="277"/>
+      <location filename="../sound_source_id/__main__.py" line="171"/>
       <source>Load Parameters</source>
       <translation>Charger les paramètres</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="173"/>
       <source>Load Parameters File</source>
       <translation>Charger le fichier des paramètres</translation>
@@ -156,105 +78,177 @@
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="202"/>
       <source>Manual (pdf)</source>
       <translation>Manuel (pdf)</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="964"/>
+      <location filename="../sound_source_id/__main__.py" line="206"/>
       <source>About sound_source_id</source>
       <translation>À propos de sound_source_id</translation>
     </message>
     <message>
       <location filename="../sound_source_id/__main__.py" line="210"/>
       <source>Show Play Buttons</source>
       <translation>Afficher les boutons de lecture</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
+      <location filename="../sound_source_id/__main__.py" line="214"/>
+      <source>Show Response Buttons</source>
+      <translation>Afficher les boutons de réponse</translation>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="219"/>
+      <source>Show Response Lights</source>
+      <translation>Affichier les lumières de réponse</translation>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="224"/>
+      <source>Show Control Panel</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="230"/>
+      <source>Listener:</source>
+      <translation>Participant :</translation>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <location filename="../sound_source_id/__main__.py" line="427"/>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
       <source>Warning</source>
       <translation>Avertissement</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="248"/>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
       <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="263"/>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
       <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="615"/>
+      <location filename="../sound_source_id/__main__.py" line="602"/>
+      <location filename="../sound_source_id/__main__.py" line="426"/>
+      <location filename="../sound_source_id/__main__.py" line="272"/>
       <source>Start</source>
       <translation>Commencer</translation>
     </message>
     <message>
+      <location filename="../sound_source_id/__main__.py" line="282"/>
+      <source>Choose Results File</source>
+      <translation>Choisir le fichier des résultats</translation>
+    </message>
+    <message>
       <location filename="../sound_source_id/__main__.py" line="288"/>
+      <source>Reset</source>
+      <translation>Réinitialiser</translation>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="293"/>
       <source>Run Demo</source>
       <translation>Démo</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
       <source>Loaded</source>
       <translation>Chargé</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
       <source>parameter file</source>
       <translation>fichier des paramètres</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
+      <location filename="../sound_source_id/__main__.py" line="856"/>
+      <location filename="../sound_source_id/__main__.py" line="602"/>
+      <location filename="../sound_source_id/__main__.py" line="426"/>
+      <source>Finished</source>
+      <translation>Fini</translation>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="427"/>
+      <source>This will stop the current test. Are you sure you want to proceed?</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
+      <location filename="../sound_source_id/__main__.py" line="431"/>
       <source>Choose parameters file to load</source>
       <translation>Choisir le fichier des paramètres à charger</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
+      <location filename="../sound_source_id/__main__.py" line="431"/>
       <source>All Files (*)</source>
       <translation>Tous les fichier (*)</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
       <source>Choose file to write results</source>
       <translation>Choisir le fichier des résultats</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="569"/>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
+      <source>csv (*.csv)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <source>File</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <source>already exists. Do you want to overwrite it?</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
+      <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
       <source>You need to select a file where to save the results to proceed</source>
       <translation>Vous devez choisir un fichier où sauvegarder les résultats</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="573"/>
+      <location filename="../sound_source_id/__main__.py" line="585"/>
       <source>Please, enter the listener's name:</source>
       <translation>S'il vous plaît de saisir l'identifiant du sujet</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="574"/>
+      <location filename="../sound_source_id/__main__.py" line="586"/>
       <source>Input Dialog:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="729"/>
+      <location filename="../sound_source_id/__main__.py" line="741"/>
+      <location filename="../sound_source_id/__main__.py" line="597"/>
+      <location filename="../sound_source_id/__main__.py" line="593"/>
       <source>Running</source>
       <translation>En exécution</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="841"/>
+      <location filename="../sound_source_id/__main__.py" line="853"/>
       <source>Run Block</source>
       <translation>Lancer Bloc</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="844"/>
-      <source>Finished</source>
-      <translation>Fini</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="965"/>
       <source>&lt;b&gt;sound_source_id - Python app for sound localization experiments&lt;/b&gt; &lt;br&gt;
                               - version: {0}; &lt;br&gt;
                               - build date: {1} &lt;br&gt;
                               &lt;p&gt; Copyright &amp;copy; 2022-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                               All rights reserved. &lt;p&gt;
                               This program is free software: you can redistribute it and/or modify
                               it under the terms of the GNU General Public License as published by
@@ -267,71 +261,20 @@
                               GNU General Public License for more details.
                               &lt;p&gt;
                               You should have received a copy of the GNU General Public License
                               along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
                               &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="225"/>
-      <source>Listener:</source>
-      <translation>Participant :</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="214"/>
-      <source>Show Response Buttons</source>
-      <translation>Afficher les boutons de réponse</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="219"/>
-      <source>Show Response Lights</source>
-      <translation>Affichier les lumières de réponse</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="277"/>
-      <source>Choose Results File</source>
-      <translation>Choisir le fichier des résultats</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="283"/>
-      <source>Reset</source>
-      <translation>Réinitialiser</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
-      <source>This will stop the current test. Are you sure you want to proceed?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="560"/>
-      <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
-      <source>csv (*.csv)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
-      <source>File</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
-      <source>already exists. Do you want to overwrite it?</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>phonesDialog</name>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="657"/>
       <source>Warning</source>
-      <translation type="obsolete">Avertissement</translation>
+      <translation type="vanished">Avertissement</translation>
     </message>
   </context>
   <context>
     <name>preferencesDialog</name>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="65"/>
       <source>Language (requires restart):</source>
@@ -365,19 +308,23 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="127"/>
       <source>Command:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="329"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="135"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="130"/>
       <source>custom</source>
       <translation type="unfinished">personnalisé</translation>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="156"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="142"/>
       <source>Device:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="173"/>
       <source>Buffer Size (samples):</source>
       <translation type="unfinished"/>
@@ -419,53 +366,66 @@
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="349"/>
       <source>There are unsaved changes. Apply Changes?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/dialog_edit_preferences.py" line="349"/>
       <source>Phones:</source>
-      <translation type="obsolete">Phones:</translation>
+      <translation type="vanished">Phones:</translation>
     </message>
   </context>
   <context>
     <name>responseLight</name>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1134"/>
+      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
+      <location filename="../sound_source_id/__main__.py" line="1062"/>
+      <location filename="../sound_source_id/__main__.py" line="1049"/>
       <source>Light &amp; Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1122"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1158"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1168"/>
+      <location filename="../sound_source_id/__main__.py" line="1180"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light &amp; Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1116"/>
+      <location filename="../sound_source_id/__main__.py" line="1128"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
       <source>Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1153"/>
+      <location filename="../sound_source_id/__main__.py" line="1165"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
       <source>Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1127"/>
+      <location filename="../sound_source_id/__main__.py" line="1139"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
       <source>Smiley</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>transducersDialog</name>
     <message>
@@ -501,14 +461,16 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="167"/>
       <source>Edit Transducers</source>
       <translation>Modifier les transducteurs</translation>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="192"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="179"/>
       <source>Warning</source>
       <translation>Avertissement</translation>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="179"/>
       <source>Only one label can be renamed at a time</source>
       <translation type="unfinished"/>
@@ -516,27 +478,28 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="184"/>
       <source>New name:</source>
       <translation>Nouveau nom :</translation>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="198"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="185"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="192"/>
       <source>Only one item can be edited at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="197"/>
       <source>Level:</source>
       <translation>Niveau :</translation>
     </message>
     <message>
-      <location filename="../sound_source_id/dialog_edit_transducers.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="250"/>
       <source>Only one transducer left. Cannot remove!</source>
       <translation type="unfinished"/>
     </message>
   </context>
 </TS>
```

### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_it.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_es.ts`

 * *Files 21% similar despite different names*

#### Comparing `sound_source_id-0.2.0/prep-release/sound_source_id_it.ts` & `sound_source_id-0.2.2/prep-release/sound_source_id_es.ts`

```diff
@@ -1,260 +1,247 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="it_IT" sourcelanguage="en_US">
+<TS version="2.1">
   <context>
     <name/>
     <message>
       <location filename="../sound_source_id/global_parameters.py" line="167"/>
+      <location filename="../sound_source_id/global_parameters.py" line="164"/>
+      <location filename="../sound_source_id/global_parameters.py" line="87"/>
       <source>custom</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
-    <name>Preferences Window</name>
+    <name>applicationWindow</name>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="91"/>
-      <source>System Settings</source>
+      <location filename="../sound_source_id/__main__.py" line="149"/>
+      <source>sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="92"/>
-      <source>en</source>
+      <location filename="../sound_source_id/__main__.py" line="169"/>
+      <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="93"/>
-      <source>it</source>
+      <location filename="../sound_source_id/__main__.py" line="277"/>
+      <location filename="../sound_source_id/__main__.py" line="171"/>
+      <source>Load Parameters</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="94"/>
-      <source>fr</source>
+      <location filename="../sound_source_id/__main__.py" line="173"/>
+      <source>Load Parameters File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="95"/>
-      <source>es</source>
+      <location filename="../sound_source_id/__main__.py" line="178"/>
+      <source>Exit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="96"/>
-      <source>el</source>
+      <location filename="../sound_source_id/__main__.py" line="180"/>
+      <source>Exit application</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="99"/>
-      <source>US</source>
+      <location filename="../sound_source_id/__main__.py" line="186"/>
+      <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="100"/>
-      <source>GB</source>
+      <location filename="../sound_source_id/__main__.py" line="187"/>
+      <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="102"/>
-      <source>IT</source>
+      <location filename="../sound_source_id/__main__.py" line="191"/>
+      <source>Transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="103"/>
-      <source>CH</source>
+      <location filename="../sound_source_id/__main__.py" line="196"/>
+      <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="104"/>
-      <source>FR</source>
+      <location filename="../sound_source_id/__main__.py" line="198"/>
+      <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="105"/>
-      <source>CA</source>
+      <location filename="../sound_source_id/__main__.py" line="202"/>
+      <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="107"/>
-      <source>ES</source>
+      <location filename="../sound_source_id/__main__.py" line="964"/>
+      <location filename="../sound_source_id/__main__.py" line="206"/>
+      <source>About sound_source_id</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="108"/>
-      <source>BO</source>
+      <location filename="../sound_source_id/__main__.py" line="210"/>
+      <source>Show Play Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="109"/>
-      <source>CL</source>
+      <location filename="../sound_source_id/__main__.py" line="214"/>
+      <source>Show Response Buttons</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="111"/>
-      <source>GR</source>
+      <location filename="../sound_source_id/__main__.py" line="219"/>
+      <source>Show Response Lights</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/global_parameters.py" line="112"/>
-      <source>CY</source>
+      <location filename="../sound_source_id/__main__.py" line="224"/>
+      <source>Show Control Panel</source>
       <translation type="unfinished"/>
     </message>
-  </context>
-  <context>
-    <name>applicationWindow</name>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="149"/>
-      <source>sound_source_id</source>
+      <location filename="../sound_source_id/__main__.py" line="230"/>
+      <source>Listener:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="169"/>
-      <source>&amp;File</source>
-      <translation>&amp;File</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="272"/>
-      <source>Load Parameters</source>
-      <translation>Carica parametri</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="173"/>
-      <source>Load Parameters File</source>
-      <translation>Carica file dei parametri</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="178"/>
-      <source>Exit</source>
-      <translation>Esci</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="180"/>
-      <source>Exit application</source>
-      <translation>Esci dall'applicazione</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="186"/>
-      <source>&amp;Edit</source>
-      <translation>&amp;Modifica</translation>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <location filename="../sound_source_id/__main__.py" line="427"/>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
+      <source>Warning</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="187"/>
-      <source>Preferences</source>
-      <translation>Preferenze</translation>
+      <location filename="../sound_source_id/__main__.py" line="253"/>
+      <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="191"/>
-      <source>Transducers</source>
+      <location filename="../sound_source_id/__main__.py" line="268"/>
+      <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="196"/>
-      <source>&amp;Help</source>
-      <translation>&amp;Aiuto</translation>
+      <location filename="../sound_source_id/__main__.py" line="615"/>
+      <location filename="../sound_source_id/__main__.py" line="602"/>
+      <location filename="../sound_source_id/__main__.py" line="426"/>
+      <location filename="../sound_source_id/__main__.py" line="272"/>
+      <source>Start</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="198"/>
-      <source>Manual (html)</source>
-      <translation>Manuale (html)</translation>
+      <location filename="../sound_source_id/__main__.py" line="282"/>
+      <source>Choose Results File</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="202"/>
-      <source>Manual (pdf)</source>
-      <translation>Manuale (pdf)</translation>
+      <location filename="../sound_source_id/__main__.py" line="288"/>
+      <source>Reset</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
-      <source>About sound_source_id</source>
-      <translation>A proposito di sound_source_id</translation>
+      <location filename="../sound_source_id/__main__.py" line="293"/>
+      <source>Run Demo</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="210"/>
-      <source>Show Play Buttons</source>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
+      <source>Loaded</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
-      <source>Warning</source>
+      <location filename="../sound_source_id/__main__.py" line="423"/>
+      <source>parameter file</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="248"/>
-      <source>There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program.</source>
+      <location filename="../sound_source_id/__main__.py" line="856"/>
+      <location filename="../sound_source_id/__main__.py" line="602"/>
+      <location filename="../sound_source_id/__main__.py" line="426"/>
+      <source>Finished</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="263"/>
-      <source>The default parameters file could not be found. Please select a new default parameters file and restart the program.</source>
+      <location filename="../sound_source_id/__main__.py" line="603"/>
+      <location filename="../sound_source_id/__main__.py" line="427"/>
+      <source>This will stop the current test. Are you sure you want to proceed?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="603"/>
-      <source>Start</source>
-      <translation>Inizia</translation>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
+      <location filename="../sound_source_id/__main__.py" line="431"/>
+      <source>Choose parameters file to load</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="288"/>
-      <source>Run Demo</source>
+      <location filename="../sound_source_id/__main__.py" line="436"/>
+      <location filename="../sound_source_id/__main__.py" line="431"/>
+      <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
-      <source>Loaded</source>
-      <translation>Caricati</translation>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
+      <source>Choose file to write results</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="411"/>
-      <source>parameter file</source>
-      <translation>file dei parametri</translation>
+      <location filename="../sound_source_id/__main__.py" line="548"/>
+      <source>csv (*.csv)</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
-      <source>Choose parameters file to load</source>
-      <translation>Scegli il file dei parametri da caricare</translation>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <source>File</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="424"/>
-      <source>All Files (*)</source>
-      <translation>Tutti i file (*)</translation>
+      <location filename="../sound_source_id/__main__.py" line="553"/>
+      <source>already exists. Do you want to overwrite it?</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
-      <source>Choose file to write results</source>
-      <translation>Scegli il file dove salvare i risultati</translation>
+      <location filename="../sound_source_id/__main__.py" line="572"/>
+      <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="569"/>
+      <location filename="../sound_source_id/__main__.py" line="581"/>
       <source>You need to select a file where to save the results to proceed</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="573"/>
+      <location filename="../sound_source_id/__main__.py" line="585"/>
       <source>Please, enter the listener's name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="574"/>
+      <location filename="../sound_source_id/__main__.py" line="586"/>
       <source>Input Dialog:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="729"/>
+      <location filename="../sound_source_id/__main__.py" line="741"/>
+      <location filename="../sound_source_id/__main__.py" line="597"/>
+      <location filename="../sound_source_id/__main__.py" line="593"/>
       <source>Running</source>
-      <translation>In esecuzione</translation>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="841"/>
+      <location filename="../sound_source_id/__main__.py" line="853"/>
       <source>Run Block</source>
-      <translation>Inizia blocco</translation>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="844"/>
-      <source>Finished</source>
-      <translation>Finito</translation>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="952"/>
+      <location filename="../sound_source_id/__main__.py" line="965"/>
       <source>&lt;b&gt;sound_source_id - Python app for sound localization experiments&lt;/b&gt; &lt;br&gt;
                               - version: {0}; &lt;br&gt;
                               - build date: {1} &lt;br&gt;
                               &lt;p&gt; Copyright &amp;copy; 2022-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                               All rights reserved. &lt;p&gt;
                               This program is free software: you can redistribute it and/or modify
                               it under the terms of the GNU General Public License as published by
@@ -267,64 +254,14 @@
                               GNU General Public License for more details.
                               &lt;p&gt;
                               You should have received a copy of the GNU General Public License
                               along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
                               &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="225"/>
-      <source>Listener:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="214"/>
-      <source>Show Response Buttons</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="219"/>
-      <source>Show Response Lights</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="277"/>
-      <source>Choose Results File</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="283"/>
-      <source>Reset</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="591"/>
-      <source>This will stop the current test. Are you sure you want to proceed?</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="560"/>
-      <source>The results file cannot be changed while a test is running. Reset the test and then choose a new results file.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="536"/>
-      <source>csv (*.csv)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
-      <source>File</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../sound_source_id/__main__.py" line="541"/>
-      <source>already exists. Do you want to overwrite it?</source>
-      <translation type="unfinished"/>
-    </message>
   </context>
   <context>
     <name>preferencesDialog</name>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="65"/>
       <source>Language (requires restart):</source>
       <translation type="unfinished"/>
@@ -357,19 +294,23 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="127"/>
       <source>Command:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="329"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="135"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="130"/>
       <source>custom</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="156"/>
+      <location filename="../sound_source_id/dialog_edit_preferences.py" line="142"/>
       <source>Device:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_preferences.py" line="173"/>
       <source>Buffer Size (samples):</source>
       <translation type="unfinished"/>
@@ -414,45 +355,59 @@
       <source>There are unsaved changes. Apply Changes?</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>responseLight</name>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1134"/>
+      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
+      <location filename="../sound_source_id/__main__.py" line="1062"/>
+      <location filename="../sound_source_id/__main__.py" line="1049"/>
       <source>Light &amp; Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1122"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1146"/>
+      <location filename="../sound_source_id/__main__.py" line="1158"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1168"/>
+      <location filename="../sound_source_id/__main__.py" line="1180"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
+      <location filename="../sound_source_id/__main__.py" line="1076"/>
       <source>Light &amp; Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1116"/>
+      <location filename="../sound_source_id/__main__.py" line="1128"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
       <source>Text</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1153"/>
+      <location filename="../sound_source_id/__main__.py" line="1165"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
+      <location filename="../sound_source_id/__main__.py" line="1085"/>
       <source>Text &amp; Smiley</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/__main__.py" line="1127"/>
+      <location filename="../sound_source_id/__main__.py" line="1139"/>
+      <location filename="../sound_source_id/__main__.py" line="1110"/>
       <source>Smiley</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>transducersDialog</name>
     <message>
@@ -488,14 +443,16 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="167"/>
       <source>Edit Transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="192"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="179"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="179"/>
       <source>Only one label can be renamed at a time</source>
       <translation type="unfinished"/>
@@ -503,27 +460,28 @@
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="184"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="198"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="185"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="192"/>
       <source>Only one item can be edited at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../sound_source_id/dialog_edit_transducers.py" line="197"/>
       <source>Level:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../sound_source_id/dialog_edit_transducers.py" line="249"/>
+      <location filename="../sound_source_id/dialog_edit_transducers.py" line="250"/>
       <source>Only one transducer left. Cannot remove!</source>
       <translation type="unfinished"/>
     </message>
   </context>
 </TS>
```

### Comparing `sound_source_id-0.2.0/prep-release/switch_pyqt5.py` & `sound_source_id-0.2.2/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/prep-release/switch_pyqt6.py` & `sound_source_id-0.2.2/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/prep-release/win_launch_iss_compiler.sh` & `sound_source_id-0.2.2/prep-release/win_launch_iss_compiler.sh`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/prep-release/win_sound_source_id.iss` & `sound_source_id-0.2.2/prep-release/win_sound_source_id.iss`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "sound_source_id"
-#define MyAppVersion "0.2.0"
+#define MyAppVersion "0.2.2"
 #define MyAppPublisher "Samuele Carcagno"
 #define MyAppURL "https://samcarcagno.altervista.org/sound_source_id/sound_source_id.html"
 #define MyAppExeName "sound_source_id.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application. Do not use the same AppId value in installers for other applications.
 ; (To generate a new GUID, click Tools | Generate GUID inside the IDE.)
```

### Comparing `sound_source_id-0.2.0/prep-release/winbuild.py` & `sound_source_id-0.2.2/prep-release/winbuild.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/pyproject.toml` & `sound_source_id-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sound_source_id"
-    version="0.2.0"
+    version="0.2.2"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Python application for running sound localization experiments"
 license = {file = "COPYING.txt"}
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["matplotlib (>=3.0.0)",
                 "numpy (>=1.0.0)",
 		"pandas (>=1.0.0)",
 		"PyAudio (>=0.2.11)",
-		"PyQt5 (>=5.12)",
-		"scipy (>=1.0.1)"
+		"PyQt6 (>=6.6.0)",
+		"scipy (>=1.0.1)",
+		"pysofa (>=0.1.1)"
 		]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
```

### Comparing `sound_source_id-0.2.0/resources.qrc` & `sound_source_id-0.2.2/resources.qrc`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/__main__.py` & `sound_source_id-0.2.2/sound_source_id/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,19 @@
         self.showRespBtnAction.triggered.connect(self.onToggleShowRespBtnAction)
 
         self.showRespLightAction = QAction(self.tr('Show Response Lights'), self, checkable=True)
         self.showRespLightAction.setChecked(True)
         self.editMenu.addAction(self.showRespLightAction)
         self.showRespLightAction.triggered.connect(self.onToggleShowRespLightAction)
 
+        self.showControlPanelAction = QAction(self.tr('Show Control Panel'), self, checkable=True)
+        self.showControlPanelAction.setChecked(True)
+        self.editMenu.addAction(self.showControlPanelAction)
+        self.showControlPanelAction.triggered.connect(self.onToggleShowControlPanelAction)
+
         n = 0
         self.listenerLabel = QLabel(self.tr('Listener:'), self)
         self.f2_grid_sizer.addWidget(self.listenerLabel, n, 0)
         self.listenerTF = QLineEdit("")
         self.f2_grid_sizer.addWidget(self.listenerTF, n, 1)
         self.listenerTF.editingFinished.connect(self.onListenerChange)
 
@@ -308,26 +313,33 @@
         
     def onToggleShowPlayBtnAction(self):
         for pb in self.play_btn:
             if self.showPlayBtnAction.isChecked() == True:
                 pb.show()
             else:
                 pb.hide()
+                
     def onToggleShowRespBtnAction(self):
         for pb in self.rsp_btn:
             if self.showRespBtnAction.isChecked() == True:
                 pb.show()
             else:
                 pb.hide()
+                
     def onToggleShowRespLightAction(self):
         for lt in self.rsp_light:
             if self.showRespLightAction.isChecked() == True:
                 lt.show()
             else:
                 lt.hide()
+    def onToggleShowControlPanelAction(self):
+        if self.showControlPanelAction.isChecked() == True:
+            self.f2.show()
+        else:
+            self.f2.hide()
 
     def loadParameters(self, fName):
         self.parametersFile = fName
         fStream = open(fName, 'r')
         allLines = fStream.readlines()
         fStream.close()
         self.az_angles = np.zeros(0)
@@ -1238,14 +1250,16 @@
     ## Look and feel changed to CleanLooks
     #QApplication.setStyle(QStyleFactory.create("QtCurve"))
     #QApplication.setPalette(QApplication.style().standardPalette())
     #qApp.currentLocale = locale
     # instantiate the ApplicationWindow widget
     qApp.currentLocale = locale
     qApp.setApplicationName('sound_source_id')
+    if platform.system() == "Windows":
+        qApp.setStyle('Fusion')
     aw = applicationWindow(prm)
 
 
     # show the widget
     #aw.show()
     # start the Qt main loop execution, exiting from this script
     # with the same return code of Qt application
```

### Comparing `sound_source_id-0.2.0/sound_source_id/audio_manager.py` & `sound_source_id-0.2.2/sound_source_id/audio_manager.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/dialog_edit_preferences.py` & `sound_source_id-0.2.2/sound_source_id/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/dialog_edit_transducers.py` & `sound_source_id-0.2.2/sound_source_id/dialog_edit_transducers.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/Figures/edit_transducers.png` & `sound_source_id-0.2.2/sound_source_id/doc/Figures/edit_transducers.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/Figures/sound_source_id_screenshot.png` & `sound_source_id-0.2.2/sound_source_id/doc/Figures/sound_source_id_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/Figures/stim_file.png` & `sound_source_id-0.2.2/sound_source_id/doc/Figures/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/Makefile` & `sound_source_id-0.2.2/sound_source_id/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_images/edit_transducers.png` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/edit_transducers.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_images/stim_file.png` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_images/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/calibration.rst.txt` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/calibration.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/index.rst.txt` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_sources/installation.rst.txt` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_sources/installation.rst.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 .. code-block:: bash
 
 		pip install sound_source_id
 
 
 ``sound_source_id`` depends on a few Python modules including:
 
-  * PyQt5
+  * PyQt6
   * numpy
   * scipy
   * matplotlib
   * pandas
   * PyAudio https://pypi.org/project/PyAudio/
 
 depending on your Python distribution you may want to install these dependecies before installing ``sound_source_id`` via pip (e.g. through conda if you're using the Anaconda Python distribution or through your Linux distribution package manager if you're using the Python installation that comes with your Linux distribution), otherwise pip will attempt to automatically pull in and install these dependencies. If the program is successfully installed you should be able to start it from a bash/DOS terminal with the command:
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/basic.css` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/doctools.js` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/jquery.js` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/language_data.js` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/pygments.css` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/searchtools.js` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/sphinx_highlight.js` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/_static/underscore.js` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/calibration.html` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/calibration.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Sound Level Calibration &mdash; sound_source_id 0.2.0 documentation</title>
+  <title>Sound Level Calibration &mdash; sound_source_id 0.2.2 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.0
+                0.2.2
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.0
+0.2.2
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/experiment_setup.html` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/experiment_setup.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Parameters file &mdash; sound_source_id 0.2.0 documentation</title>
+  <title>Parameters file &mdash; sound_source_id 0.2.2 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.0
+                0.2.2
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.0
+0.2.2
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/genindex.html` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; sound_source_id 0.2.0 documentation</title>
+  <title>Index &mdash; sound_source_id 0.2.2 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -26,15 +26,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.0
+                0.2.2
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.0
+0.2.2
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/index.html` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to sound_source_id’s documentation! &mdash; sound_source_id 0.2.0 documentation</title>
+  <title>Welcome to sound_source_id’s documentation! &mdash; sound_source_id 0.2.2 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.0
+                0.2.2
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.0
+0.2.2
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/installation.html` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/installation.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; sound_source_id 0.2.0 documentation</title>
+  <title>Installation &mdash; sound_source_id 0.2.2 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.0
+                0.2.2
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -81,15 +81,15 @@
 <p><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. <code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> is written in Python and can be installed via pip:</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>pip<span class="w"> </span>install<span class="w"> </span>sound_source_id
 </pre></div>
 </div>
 <p><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> depends on a few Python modules including:</p>
 <blockquote>
 <div><ul class="simple">
-<li><p>PyQt5</p></li>
+<li><p>PyQt6</p></li>
 <li><p>numpy</p></li>
 <li><p>scipy</p></li>
 <li><p>matplotlib</p></li>
 <li><p>pandas</p></li>
 <li><p>PyAudio <a class="reference external" href="https://pypi.org/project/PyAudio/">https://pypi.org/project/PyAudio/</a></p></li>
 </ul>
 </div></blockquote>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.0
+0.2.2
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
@@ -13,15 +13,15 @@
 ===============================================================================
 ************ IInnssttaallllaattiioonn_? ************
 sound_source_id has been successfully installed and used on Linux and Windows.
 It should also work on Mac platforms, but this has not been tested.
 sound_source_id is written in Python and can be installed via pip:
 pip install sound_source_id
 sound_source_id depends on a few Python modules including:
-         * PyQt5
+         * PyQt6
          * numpy
          * scipy
          * matplotlib
          * pandas
          * PyAudio _h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_P_y_A_u_d_i_o_/
 depending on your Python distribution you may want to install these dependecies
 before installing sound_source_id via pip (e.g. through conda if you’re using
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/intro.html` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/intro.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>sound_source_id &mdash; sound_source_id 0.2.0 documentation</title>
+  <title>sound_source_id &mdash; sound_source_id 0.2.2 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.0
+                0.2.2
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.0
+0.2.2
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/search.html` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; sound_source_id 0.2.0 documentation</title>
+  <title>Search &mdash; sound_source_id 0.2.2 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             sound_source_id
           </a>
               <div class="version">
-                0.2.0
+                0.2.2
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _s_o_u_n_d___s_o_u_r_c_e___i_d
-0.2.0
+0.2.2
 [q                   ]
 Contents:
     * _s_o_u_n_d___s_o_u_r_c_e___i_d
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _P_a_r_a_m_e_t_e_r_s_ _f_i_l_e
     * _S_t_i_m_u_l_a_t_i_o_n_ _f_i_l_e
     * _S_o_u_n_d_ _L_e_v_e_l_ _C_a_l_i_b_r_a_t_i_o_n
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/html/searchindex.js` & `sound_source_id-0.2.2/sound_source_id/doc/_build/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -156,15 +156,15 @@
         "written": 3,
         "python": 3,
         "via": 3,
         "pip": 3,
         "depend": 3,
         "few": 3,
         "includ": 3,
-        "pyqt5": 3,
+        "pyqt5": [],
         "numpi": 3,
         "scipi": 3,
         "matplotlib": 3,
         "panda": 3,
         "pyaudio": 3,
         "http": 3,
         "pypi": 3,
@@ -303,15 +303,16 @@
         "dbdiff": 0,
         "log10": 0,
         "had": 0,
         "x": 0,
         "have": 0,
         "maxlev": 0,
         "tabl": 0,
-        "question": 0
+        "question": 0,
+        "pyqt6": 3
     },
     "objects": {},
     "objtypes": {},
     "objnames": {},
     "titleterms": {
         "paramet": 1,
         "file": 1,
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/latex/sound_source_id.pdf` & `sound_source_id-0.2.2/sound_source_id/doc/_build/latex/sound_source_id.pdf`

 * *Files 11% similar despite different names*

#### Comparing `sound_source_id-0.2.0/sound_source_id/doc/_build/latex/sound_source_id.pdf` & `sound_source_id-0.2.2/sound_source_id/doc/_build/latex/sound_source_id.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: 'Samuele Carcagno'
-CreationDate: "D:20230619162343+02'00'"
+CreationDate: "D:20240502223433+02'00'"
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: "D:20230619162343+02'00'"
+ModDate: "D:20240502223433+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.24 (TeX Live 2022/Debian) kpathsea version 6.3.4'
 Producer: 'pdfTeX-1.40.24'
 Subject: ''
 Title: 'sound_source_id'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 sound_source_id
-Release 0.2.0
+Release 0.2.2
 
 Samuele Carcagno
 
-Jun 19, 2023
+May 02, 2024
 
 CONTENTS:
 
 1
 
 sound_source_id
 
@@ -56,15 +56,15 @@
 sound_source_id is program for testing static sound localization. The interface is shown in Figure Screenshot of the
 sound_source_id interface..
 
 Fig. 1: Screenshot of the sound_source_id interface.
 
 1
 
-sound_source_id, Release 0.2.0
+sound_source_id, Release 0.2.2
 
 2
 
 Chapter 1. sound_source_id
 
 CHAPTER
 
@@ -72,15 +72,15 @@
 
 INSTALLATION
 
 sound_source_id has been successfully installed and used on Linux and Windows. It should also work on Mac
 platforms, but this has not been tested. sound_source_id is written in Python and can be installed via pip:
 pip install sound_source_id
 sound_source_id depends on a few Python modules including:
-• PyQt5
+• PyQt6
 • numpy
 • scipy
 • matplotlib
 • pandas
 • PyAudio https://pypi.org/project/PyAudio/
 depending on your Python distribution you may want to install these dependecies before installing sound_source_id
 via pip (e.g. through conda if you’re using the Anaconda Python distribution or through your Linux distribution package
@@ -94,15 +94,15 @@
 on how you want sound to be played, you need to install:
 • pyalsaaudio https://pypi.org/project/pyalsaaudio/
 or SoX:
 • https://sox.sourceforge.net/
 
 3
 
-sound_source_id, Release 0.2.0
+sound_source_id, Release 0.2.2
 
 4
 
 Chapter 2. Installation
 
 CHAPTER
 
@@ -131,15 +131,15 @@
 • stim_list_file: the path (absolute or relative) to the file containing the stimulation list (see below)
 • randomize: if true the stim_list_file will be shuffled before each block repetition
 • demo_stim: the path to the WAV file to be used for the demo
 • demo_stim_lev: the sound level (in dB SPL) to be used for the demo
 
 5
 
-sound_source_id, Release 0.2.0
+sound_source_id, Release 0.2.2
 
 6
 
 Chapter 3. Parameters file
 
 CHAPTER
 
@@ -160,15 +160,15 @@
 has been correctly calibrated)
 • roving: a level rove, actual sound level will be euqual to the base level plus a value drawn from a random uniform
 distribution between +/- the roving level
 • feedback: if true, feedback will be given to the listener at the end of each trial
 
 7
 
-sound_source_id, Release 0.2.0
+sound_source_id, Release 0.2.2
 
 8
 
 Chapter 4. Stimulation file
 
 CHAPTER
 
@@ -194,15 +194,15 @@
 We can measure the RMS level of the WAV file with the noise used for calibration, let’s call it 𝑟𝑚𝑠𝑛𝑜𝑖𝑠𝑒. A full
 amplitude sinusoid has a root-mean-square amplitude of 1/sqrt(2) = 0.707. The difference in dB between the level of
 a sinusoid at max amplitude and our calibration noise will be equal to:
 𝑑𝑏𝑑𝑖𝑓 𝑓 = 20 * 𝑙𝑜𝑔10((1/𝑠𝑞𝑟𝑡(2))/𝑟𝑚𝑠𝑛𝑜𝑖𝑠𝑒)
 
 9
 
-sound_source_id, Release 0.2.0
+sound_source_id, Release 0.2.2
 
 Therefore, if our calibration noise had a level (measured with the SPL meter) or 𝑥 dB SPL, a sinusoid at max amplitude
 would have a level of:
 𝑚𝑎𝑥𝑙𝑒𝑣 = 𝑥 + 𝑑𝑏𝑑𝑖𝑓 𝑓
 this is the value that you need to enter in the Max Level field of the transducers calibration table for the loudspeakers
 in question.
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/calibration.rst` & `sound_source_id-0.2.2/sound_source_id/doc/calibration.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/conf.py` & `sound_source_id-0.2.2/sound_source_id/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 author = 'Samuele Carcagno'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "0.2.0"
+version = "0.2.2"
 # The full version, including alpha/beta/rc tags.
-release = "0.2.0"
+release = "0.2.2"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/experiment_setup.rst` & `sound_source_id-0.2.2/sound_source_id/doc/experiment_setup.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/index.rst` & `sound_source_id-0.2.2/sound_source_id/doc/index.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/installation.rst` & `sound_source_id-0.2.2/sound_source_id/doc/installation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 .. code-block:: bash
 
 		pip install sound_source_id
 
 
 ``sound_source_id`` depends on a few Python modules including:
 
-  * PyQt5
+  * PyQt6
   * numpy
   * scipy
   * matplotlib
   * pandas
   * PyAudio https://pypi.org/project/PyAudio/
 
 depending on your Python distribution you may want to install these dependecies before installing ``sound_source_id`` via pip (e.g. through conda if you're using the Anaconda Python distribution or through your Linux distribution package manager if you're using the Python installation that comes with your Linux distribution), otherwise pip will attempt to automatically pull in and install these dependencies. If the program is successfully installed you should be able to start it from a bash/DOS terminal with the command:
```

### Comparing `sound_source_id-0.2.0/sound_source_id/doc/make.bat` & `sound_source_id-0.2.2/sound_source_id/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/global_parameters.py` & `sound_source_id-0.2.2/sound_source_id/global_parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -84,36 +84,36 @@
         prm['appData']['available_play_commands'].append("alsaaudio")
     if pyaudioAvailable == True:
         prm['appData']['available_play_commands'].append("pyaudio")
     prm['appData']['available_play_commands'].append(QApplication.translate("","custom",""))
 
     prm['appData']['wavmanagers'] = ["wavpy", "wavpy_sndf"]
 
-    prm['appData']['available_languages'] = [QApplication.translate("Preferences Window","System Settings",""),
-                                          QApplication.translate("Preferences Window","en",""),
-                                          QApplication.translate("Preferences Window","it",""),
-                                          QApplication.translate("Preferences Window","fr",""),
-                                          QApplication.translate("Preferences Window","es",""),
-                                          QApplication.translate("Preferences Window","el","")]
+    prm['appData']['available_languages'] = ["System Settings",
+                                             "en",
+                                             "it",
+                                             "fr",
+                                             "es",
+                                             "el"]
     prm['appData']['available_countries'] = {}
     prm['appData']['available_countries']['System Settings'] = ["System Settings"]
-    prm['appData']['available_countries']['en'] = [QApplication.translate("Preferences Window","US",""),
-                                                         QApplication.translate("Preferences Window","GB","")]
+    prm['appData']['available_countries']['en'] = ["US",
+                                                   "GB"]
 
-    prm['appData']['available_countries']['it'] = [QApplication.translate("Preferences Window","IT",""),
-                                                         QApplication.translate("Preferences Window","CH","")]
-    prm['appData']['available_countries']['fr'] = [QApplication.translate("Preferences Window","FR",""),
-                                                         QApplication.translate("Preferences Window","CA","")]
-
-    prm['appData']['available_countries']['es'] = [QApplication.translate("Preferences Window","ES",""),
-                                                         QApplication.translate("Preferences Window","BO",""),
-                                                         QApplication.translate("Preferences Window","CL","")]
+    prm['appData']['available_countries']['it'] = ["IT",
+                                                   "CH"]
+    prm['appData']['available_countries']['fr'] = ["FR",
+                                                   "CA"]
+
+    prm['appData']['available_countries']['es'] = ["ES",
+                                                   "BO",
+                                                   "CL"]
 
-    prm['appData']['available_countries']['el'] = [QApplication.translate("Preferences Window","GR",""),
-                                                         QApplication.translate("Preferences Window","CY","")]
+    prm['appData']['available_countries']['el'] = ["GR",
+                                                   "CY"]
 
 
 
     return prm
 
 
 def def_prefs(prm):
```

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise1.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise1.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise10.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise10.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise11.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise11.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise12.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise12.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise13.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise13.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise14.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise14.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise15.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise15.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise16.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise16.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise17.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise17.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise18.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise18.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise19.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise19.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise2.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise2.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise20.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise20.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise21.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise21.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise22.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise22.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise23.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise23.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise24.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise24.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise25.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise25.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise26.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise26.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise27.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise27.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise28.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise28.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise29.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise29.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise3.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise3.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise30.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise30.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise4.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise4.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise5.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise5.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise6.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise6.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise7.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise7.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise8.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise8.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/pink_noises/noise9.wav` & `sound_source_id-0.2.2/sound_source_id/prm_files/pink_noises/noise9.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/prm_circle_36_targets.txt` & `sound_source_id-0.2.2/sound_source_id/prm_files/prm_circle_36_targets.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt` & `sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_36_targets.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt` & `sound_source_id-0.2.2/sound_source_id/prm_files/prm_virtual_circle_8_az_2_elev.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/stim_list.csv` & `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_4_front_back.csv` & `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_4_front_back.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_8_az_2_elev.csv` & `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_8_az_2_elev.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_circle.csv` & `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_circle.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/prm_files/stim_list_circle_12_tgs.csv` & `sound_source_id-0.2.2/sound_source_id/prm_files/stim_list_circle_12_tgs.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/pyqtver.py` & `sound_source_id-0.2.2/sound_source_id/pyqtver.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
 #    You should have received a copy of the GNU General Public License
 #    along with sound_source_id.  If not, see <http://www.gnu.org/licenses/>.
 
-pyqtversion = 5
+pyqtversion = 6
```

### Comparing `sound_source_id-0.2.0/sound_source_id/sndlib.py` & `sound_source_id-0.2.2/sound_source_id/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/utils.py` & `sound_source_id-0.2.2/sound_source_id/utils.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/wavpy.py` & `sound_source_id-0.2.2/sound_source_id/wavpy.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id/wavpy_sndf.py` & `sound_source_id-0.2.2/sound_source_id/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.2.0/sound_source_id.egg-info/PKG-INFO` & `sound_source_id-0.2.2/sound_source_id.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sound-source-id
-Version: 0.2.0
+Name: sound_source_id
+Version: 0.2.2
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,9 +689,16 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING.txt
+Requires-Dist: matplotlib>=3.0.0
+Requires-Dist: numpy>=1.0.0
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: PyAudio>=0.2.11
+Requires-Dist: PyQt6>=6.6.0
+Requires-Dist: scipy>=1.0.1
+Requires-Dist: pysofa>=0.1.1
 
 Python program for sound localization tests.
```

### Comparing `sound_source_id-0.2.0/sound_source_id.egg-info/SOURCES.txt` & `sound_source_id-0.2.2/sound_source_id.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.readthedocs.yaml
 COPYING.txt
 MANIFEST.in
 README.md
 pyproject.toml
 resources.qrc
 setup_cx.py
 icons/audio-headphones.svgz
@@ -58,14 +59,15 @@
 sound_source_id/doc/conf.py
 sound_source_id/doc/experiment_setup.rst
 sound_source_id/doc/index.rst
 sound_source_id/doc/installation.rst
 sound_source_id/doc/intro.rst
 sound_source_id/doc/make.bat
 sound_source_id/doc/mkdoc.sh
+sound_source_id/doc/requirements.txt
 sound_source_id/doc/Figures/edit_transducers.png
 sound_source_id/doc/Figures/sound_source_id_screenshot.png
 sound_source_id/doc/Figures/stim_file.png
 sound_source_id/doc/_build/html/.buildinfo
 sound_source_id/doc/_build/html/calibration.html
 sound_source_id/doc/_build/html/experiment_setup.html
 sound_source_id/doc/_build/html/genindex.html
```

