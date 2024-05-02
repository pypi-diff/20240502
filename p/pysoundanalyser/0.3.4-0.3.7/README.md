# Comparing `tmp/pysoundanalyser-0.3.4.tar.gz` & `tmp/pysoundanalyser-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysoundanalyser-0.3.4.tar", last modified: Fri Jun  9 09:50:17 2023, max compression
+gzip compressed data, was "pysoundanalyser-0.3.7.tar", last modified: Thu May  2 20:32:30 2024, max compression
```

## Comparing `pysoundanalyser-0.3.4.tar` & `pysoundanalyser-0.3.7.tar`

### file list

```diff
@@ -1,169 +1,171 @@
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.393622 pysoundanalyser-0.3.4/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 pysoundanalyser-0.3.4/COPYING.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      183 2015-11-13 01:18:22.000000 pysoundanalyser-0.3.4/CREDITS.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2015-09-08 22:01:46.000000 pysoundanalyser-0.3.4/INSTALL.txt
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      696 2023-06-03 16:00:04.000000 pysoundanalyser-0.3.4/MANIFEST.in
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-09 09:50:17.392622 pysoundanalyser-0.3.4/PKG-INFO
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      370 2022-07-18 13:01:39.000000 pysoundanalyser-0.3.4/README.md
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.724605 pysoundanalyser-0.3.4/icons/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 pysoundanalyser-0.3.4/icons/exit.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    24750 2012-04-19 09:34:44.000000 pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.ico
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    45168 2015-09-29 11:52:50.000000 pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.png
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    14143 2010-05-31 11:23:42.000000 pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.svg
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.778607 pysoundanalyser-0.3.4/prep-release/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.830608 pysoundanalyser-0.3.4/prep-release/debian/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9879 2020-05-28 09:36:16.000000 pysoundanalyser-0.3.4/prep-release/debian/changelog
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.4/prep-release/debian/compat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      849 2015-09-21 10:20:50.000000 pysoundanalyser-0.3.4/prep-release/debian/control
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.4/prep-release/debian/copyright
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.4/prep-release/debian/docs
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.4/prep-release/debian/links
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.4/prep-release/debian/rules
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.506599 pysoundanalyser-0.3.4/prep-release/launchpad/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.876609 pysoundanalyser-0.3.4/prep-release/launchpad/debian/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10985 2020-05-28 13:40:27.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/changelog
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/compat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1077 2020-05-28 13:40:20.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/control
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/copyright
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/docs
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/links
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/rules
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2171 2020-05-28 13:36:12.000000 pysoundanalyser-0.3.4/prep-release/launchpad_build.py
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     3051 2015-10-13 17:39:53.000000 pysoundanalyser-0.3.4/prep-release/make_deb.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)        1 2023-06-09 09:49:37.000000 pysoundanalyser-0.3.4/prep-release/minor_minor_number.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      178 2022-09-23 15:23:28.000000 pysoundanalyser-0.3.4/prep-release/mkupdate_pyqt5.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1122 2023-06-03 15:25:11.000000 pysoundanalyser-0.3.4/prep-release/mkupdate_pyqt6.sh
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      185 2023-06-08 22:08:52.000000 pysoundanalyser-0.3.4/prep-release/pypi_build.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1185 2023-06-03 15:23:52.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser.pro
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77410 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_de.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77410 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_el.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77438 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_en_GB.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77410 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_es.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    79003 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_fr.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93374 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_it.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77427 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_ru.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3671 2023-06-08 22:19:59.000000 pysoundanalyser-0.3.4/prep-release/release.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:38:46.000000 pysoundanalyser-0.3.4/prep-release/switch_pyqt5.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:37:31.000000 pysoundanalyser-0.3.4/prep-release/switch_pyqt6.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2875 2019-02-12 09:45:06.000000 pysoundanalyser-0.3.4/prep-release/uploadToWebsite.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      206 2023-06-08 22:09:58.000000 pysoundanalyser-0.3.4/prep-release/win_installer_readme.md
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      146 2023-06-08 22:10:19.000000 pysoundanalyser-0.3.4/prep-release/win_launch_iss_compiler.bat
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-08 22:10:33.000000 pysoundanalyser-0.3.4/prep-release/win_launch_iss_compiler.sh
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3930 2023-06-09 09:49:38.000000 pysoundanalyser-0.3.4/prep-release/win_pysoundanalyser.iss
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      768 2023-06-08 22:16:33.000000 pysoundanalyser-0.3.4/prep-release/winbuild.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1527 2023-06-09 09:49:37.000000 pysoundanalyser-0.3.4/pyproject.toml
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.908610 pysoundanalyser-0.3.4/pysoundanalyser/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 pysoundanalyser-0.3.4/pysoundanalyser/__init__.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    82246 2023-06-09 09:38:11.000000 pysoundanalyser-0.3.4/pysoundanalyser/__main__.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      107 2023-06-09 09:49:37.000000 pysoundanalyser-0.3.4/pysoundanalyser/_version_info.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    13121 2023-05-20 15:42:12.000000 pysoundanalyser-0.3.4/pysoundanalyser/audio_manager.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11329 2023-05-20 15:31:32.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_apply_filter.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1993 2023-05-08 21:53:20.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_change_channel.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     4556 2023-05-20 15:31:53.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_concatenate.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2832 2023-05-20 15:32:08.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_cut.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    24487 2023-05-20 17:31:33.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_edit_preferences.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5932 2023-05-20 15:32:35.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_noise.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8214 2023-05-20 15:41:21.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_sinusoid.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    34378 2023-05-20 15:32:58.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_sound.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     6397 2023-05-20 15:33:11.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_get_font.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3684 2023-05-20 15:33:26.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_resample.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3287 2023-05-08 21:46:08.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_save_sound.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.925610 pysoundanalyser-0.3.4/pysoundanalyser/doc/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      634 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/Makefile
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.507599 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.928610 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      230 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/.buildinfo
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.972612 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.313620 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    11185 2023-06-04 19:56:48.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alabaster.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1128 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alert_info_32.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      944 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       78 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/background_b01.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    14810 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/basic.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       82 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bg-page.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9827 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bizstyle.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1145 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bizstyle.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      165 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bullet_orange.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      107 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/contents.png
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.326620 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/badge_only.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/theme.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    14940 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       42 2017-05-15 18:58:47.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/custom.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/doctools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/documentation_options.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/file.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     6714 2023-06-04 19:58:28.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/haiku.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/jquery.js
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.352621 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/js/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/js/theme.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4758 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/language_data.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/minus.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      120 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/navigation.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/plus.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4819 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/pygments.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/searchtools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     6263 2023-06-04 20:00:19.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/underscore.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3668 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/genindex.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5481 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/index.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     6262 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/installation.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5815 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/intro.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      351 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/objects.inv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4067 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/search.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4231 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/searchindex.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9618 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/user_interface.html
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.365622 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/latex/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   144833 2023-06-09 09:50:09.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      989 2023-06-09 09:49:38.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/conf.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/index.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/installation.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/intro.rst
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      800 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/make.bat
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      103 2015-09-27 14:19:28.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/mkdoc.sh
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/user_interface.rst
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11077 2023-05-21 07:35:18.000000 pysoundanalyser-0.3.4/pysoundanalyser/global_parameters.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       41 2023-06-09 09:38:00.000000 pysoundanalyser-0.3.4/pysoundanalyser/pyqtver.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   109505 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/pysoundanalyser/qrc_resources.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1296 2023-04-30 11:36:30.000000 pysoundanalyser-0.3.4/pysoundanalyser/random_id.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   171752 2023-04-30 11:36:45.000000 pysoundanalyser-0.3.4/pysoundanalyser/sndlib.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1598 2023-04-30 11:36:57.000000 pysoundanalyser-0.3.4/pysoundanalyser/threaded_plotters.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1432 2023-04-30 11:37:09.000000 pysoundanalyser-0.3.4/pysoundanalyser/utilities_open_manual.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10331 2023-05-20 14:57:23.000000 pysoundanalyser-0.3.4/pysoundanalyser/utility_functions.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 07:48:46.000000 pysoundanalyser-0.3.4/pysoundanalyser/wavpy.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 pysoundanalyser-0.3.4/pysoundanalyser/wavpy_sndf.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7514 2023-05-20 15:34:46.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_acf_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     9305 2023-05-20 15:34:59.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_autocorrelogram_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    20600 2023-05-20 15:35:22.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_generic_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11904 2023-05-20 15:35:37.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_spectrogram_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8447 2023-05-20 15:35:51.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_spectrum_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5635 2023-05-20 15:36:13.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_waveform_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      397 2023-06-09 09:49:38.000000 pysoundanalyser-0.3.4/pysoundanalyser.desktop
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.910610 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5809 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/top_level.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2013-02-19 11:18:49.000000 pysoundanalyser-0.3.4/resources.qrc
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.366622 pysoundanalyser-0.3.4/scripts/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       94 2015-10-11 12:48:00.000000 pysoundanalyser-0.3.4/scripts/pysoundanalyser-launcher.bat
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-09 09:50:17.393622 pysoundanalyser-0.3.4/setup.cfg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      961 2023-06-09 09:49:38.000000 pysoundanalyser-0.3.4/setup_cx.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.392622 pysoundanalyser-0.3.4/translations/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_de.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_el.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      122 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_en_GB.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_es.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      235 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_fr.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    28965 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_it.qm
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    17558 2013-02-19 23:27:27.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_it_IT.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       44 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_ru.qm
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:30.524268 pysoundanalyser-0.3.7/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1054 2024-02-05 09:44:10.000000 pysoundanalyser-0.3.7/.readthedocs.yaml
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 pysoundanalyser-0.3.7/COPYING.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      183 2015-11-13 01:18:22.000000 pysoundanalyser-0.3.7/CREDITS.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2015-09-08 22:01:46.000000 pysoundanalyser-0.3.7/INSTALL.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      696 2023-06-03 16:00:04.000000 pysoundanalyser-0.3.7/MANIFEST.in
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    42245 2024-05-02 20:32:30.524268 pysoundanalyser-0.3.7/PKG-INFO
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      370 2022-07-18 13:01:39.000000 pysoundanalyser-0.3.7/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.188261 pysoundanalyser-0.3.7/icons/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 pysoundanalyser-0.3.7/icons/exit.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    24750 2012-04-19 09:34:44.000000 pysoundanalyser-0.3.7/icons/johnny_automatic_crashing_wave.ico
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    45168 2015-09-29 11:52:50.000000 pysoundanalyser-0.3.7/icons/johnny_automatic_crashing_wave.png
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    14143 2010-05-31 11:23:42.000000 pysoundanalyser-0.3.7/icons/johnny_automatic_crashing_wave.svg
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.244261 pysoundanalyser-0.3.7/prep-release/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.304262 pysoundanalyser-0.3.7/prep-release/debian/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9879 2020-05-28 09:36:16.000000 pysoundanalyser-0.3.7/prep-release/debian/changelog
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.7/prep-release/debian/compat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      849 2015-09-21 10:20:50.000000 pysoundanalyser-0.3.7/prep-release/debian/control
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.7/prep-release/debian/copyright
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.7/prep-release/debian/docs
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.7/prep-release/debian/links
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.7/prep-release/debian/rules
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.092261 pysoundanalyser-0.3.7/prep-release/launchpad/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.472262 pysoundanalyser-0.3.7/prep-release/launchpad/debian/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10985 2020-05-28 13:40:27.000000 pysoundanalyser-0.3.7/prep-release/launchpad/debian/changelog
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.7/prep-release/launchpad/debian/compat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1077 2020-05-28 13:40:20.000000 pysoundanalyser-0.3.7/prep-release/launchpad/debian/control
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.7/prep-release/launchpad/debian/copyright
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.7/prep-release/launchpad/debian/docs
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.7/prep-release/launchpad/debian/links
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.7/prep-release/launchpad/debian/rules
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2171 2020-05-28 13:36:12.000000 pysoundanalyser-0.3.7/prep-release/launchpad_build.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     3051 2015-10-13 17:39:53.000000 pysoundanalyser-0.3.7/prep-release/make_deb.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)        1 2024-05-02 20:31:59.000000 pysoundanalyser-0.3.7/prep-release/minor_minor_number.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      178 2022-09-23 15:23:28.000000 pysoundanalyser-0.3.7/prep-release/mkupdate_pyqt5.sh
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1122 2023-06-03 15:25:11.000000 pysoundanalyser-0.3.7/prep-release/mkupdate_pyqt6.sh
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      185 2023-06-08 22:08:52.000000 pysoundanalyser-0.3.7/prep-release/pypi_build.sh
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1185 2023-06-03 15:23:52.000000 pysoundanalyser-0.3.7/prep-release/pysoundanalyser.pro
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93451 2024-05-02 20:32:08.000000 pysoundanalyser-0.3.7/prep-release/pysoundanalyser_de.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93451 2024-05-02 20:32:08.000000 pysoundanalyser-0.3.7/prep-release/pysoundanalyser_el.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93491 2024-05-02 20:32:08.000000 pysoundanalyser-0.3.7/prep-release/pysoundanalyser_en_GB.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93451 2024-05-02 20:32:08.000000 pysoundanalyser-0.3.7/prep-release/pysoundanalyser_es.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    94400 2024-05-02 20:32:08.000000 pysoundanalyser-0.3.7/prep-release/pysoundanalyser_fr.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)   107491 2024-05-02 20:32:08.000000 pysoundanalyser-0.3.7/prep-release/pysoundanalyser_it.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93468 2024-05-02 20:32:08.000000 pysoundanalyser-0.3.7/prep-release/pysoundanalyser_ru.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3667 2024-05-02 15:20:11.000000 pysoundanalyser-0.3.7/prep-release/release.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:38:46.000000 pysoundanalyser-0.3.7/prep-release/switch_pyqt5.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:37:31.000000 pysoundanalyser-0.3.7/prep-release/switch_pyqt6.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2875 2019-02-12 09:45:06.000000 pysoundanalyser-0.3.7/prep-release/uploadToWebsite.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      206 2023-06-08 22:09:58.000000 pysoundanalyser-0.3.7/prep-release/win_installer_readme.md
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      146 2023-06-08 22:10:19.000000 pysoundanalyser-0.3.7/prep-release/win_launch_iss_compiler.bat
+-rwxrwsr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-08 22:10:33.000000 pysoundanalyser-0.3.7/prep-release/win_launch_iss_compiler.sh
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4096 2024-05-02 20:31:59.000000 pysoundanalyser-0.3.7/prep-release/win_pysoundanalyser.iss
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      768 2023-06-08 22:16:33.000000 pysoundanalyser-0.3.7/prep-release/winbuild.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1528 2024-05-02 20:31:59.000000 pysoundanalyser-0.3.7/pyproject.toml
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.504263 pysoundanalyser-0.3.7/pysoundanalyser/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 pysoundanalyser-0.3.7/pysoundanalyser/__init__.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    82416 2024-05-02 19:47:23.000000 pysoundanalyser-0.3.7/pysoundanalyser/__main__.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      107 2024-05-02 20:31:59.000000 pysoundanalyser-0.3.7/pysoundanalyser/_version_info.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    13121 2024-02-18 09:32:26.000000 pysoundanalyser-0.3.7/pysoundanalyser/audio_manager.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    11329 2024-02-18 09:32:43.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_apply_filter.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1993 2024-02-18 09:32:56.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_change_channel.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     4556 2024-02-18 09:33:07.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_concatenate.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2832 2024-02-18 09:33:19.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_cut.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    24487 2024-02-18 09:33:28.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_edit_preferences.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     5932 2024-02-18 09:33:43.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_generate_noise.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     8214 2024-02-18 09:33:59.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_generate_sinusoid.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    34378 2024-02-18 09:34:13.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_generate_sound.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     8308 2024-02-18 09:25:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_get_font.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     3684 2024-02-18 09:34:25.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_resample.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     3287 2024-02-18 09:34:37.000000 pysoundanalyser-0.3.7/pysoundanalyser/dialog_save_sound.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.568263 pysoundanalyser-0.3.7/pysoundanalyser/doc/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      634 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.092261 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.572263 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:29.680264 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_sources/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_sources/index.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1277 2024-05-02 15:18:59.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2928 2023-06-11 14:10:17.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:30.444267 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    11185 2023-06-04 19:56:48.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/alabaster.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1128 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/alert_info_32.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      944 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       78 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/background_b01.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/basic.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       82 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/bg-page.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     9827 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/bizstyle.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1145 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/bizstyle.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      165 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/bullet_orange.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      107 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/contents.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:30.456267 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/css/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/css/badge_only.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/css/theme.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    14940 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       42 2017-05-15 18:58:47.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/custom.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/doctools.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/documentation_options.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/file.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     6714 2023-06-04 19:58:28.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/haiku.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/jquery.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:30.484268 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/js/
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/js/theme.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/language_data.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/minus.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      120 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/navigation.png
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/plus.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/pygments.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/searchtools.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     6263 2023-06-04 20:00:19.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/underscore.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     3668 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/genindex.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     5481 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/index.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6262 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/installation.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     5815 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/intro.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      351 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/objects.inv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4067 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4253 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/searchindex.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     9627 2024-05-02 20:32:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/user_interface.html
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:30.496268 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/latex/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   144656 2024-05-02 20:32:17.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      989 2024-05-02 20:31:59.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/conf.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1277 2024-05-02 15:18:59.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/installation.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/intro.rst
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)      800 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/make.bat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      103 2015-09-27 14:19:28.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/mkdoc.sh
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)       18 2024-02-05 09:44:53.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/requirements.txt
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2928 2023-06-11 14:10:17.000000 pysoundanalyser-0.3.7/pysoundanalyser/doc/user_interface.rst
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10240 2024-04-25 10:50:36.000000 pysoundanalyser-0.3.7/pysoundanalyser/global_parameters.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       41 2024-05-02 20:31:56.000000 pysoundanalyser-0.3.7/pysoundanalyser/pyqtver.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    53773 2024-05-02 20:32:09.000000 pysoundanalyser-0.3.7/pysoundanalyser/qrc_resources.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1296 2024-02-18 09:35:03.000000 pysoundanalyser-0.3.7/pysoundanalyser/random_id.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)   171752 2023-04-30 11:36:45.000000 pysoundanalyser-0.3.7/pysoundanalyser/sndlib.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     1598 2024-02-18 09:35:29.000000 pysoundanalyser-0.3.7/pysoundanalyser/threaded_plotters.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1432 2024-02-18 09:35:41.000000 pysoundanalyser-0.3.7/pysoundanalyser/utilities_open_manual.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10331 2024-02-18 09:35:53.000000 pysoundanalyser-0.3.7/pysoundanalyser/utility_functions.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 07:48:46.000000 pysoundanalyser-0.3.7/pysoundanalyser/wavpy.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 pysoundanalyser-0.3.7/pysoundanalyser/wavpy_sndf.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     7514 2024-02-18 09:36:26.000000 pysoundanalyser-0.3.7/pysoundanalyser/win_acf_plot.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9305 2024-02-18 09:36:39.000000 pysoundanalyser-0.3.7/pysoundanalyser/win_autocorrelogram_plot.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    20600 2024-02-18 09:36:49.000000 pysoundanalyser-0.3.7/pysoundanalyser/win_generic_plot.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    11904 2024-02-18 09:36:57.000000 pysoundanalyser-0.3.7/pysoundanalyser/win_spectrogram_plot.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     8447 2024-02-18 09:37:11.000000 pysoundanalyser-0.3.7/pysoundanalyser/win_spectrum_plot.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     5635 2024-02-18 09:37:22.000000 pysoundanalyser-0.3.7/pysoundanalyser/win_waveform_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      397 2024-05-02 20:31:59.000000 pysoundanalyser-0.3.7/pysoundanalyser.desktop
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:30.524268 pysoundanalyser-0.3.7/pysoundanalyser.egg-info/
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    42245 2024-05-02 20:32:29.000000 pysoundanalyser-0.3.7/pysoundanalyser.egg-info/PKG-INFO
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     5864 2024-05-02 20:32:29.000000 pysoundanalyser-0.3.7/pysoundanalyser.egg-info/SOURCES.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-05-02 20:32:29.000000 pysoundanalyser-0.3.7/pysoundanalyser.egg-info/dependency_links.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       62 2024-05-02 20:32:29.000000 pysoundanalyser-0.3.7/pysoundanalyser.egg-info/entry_points.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       87 2024-05-02 20:32:29.000000 pysoundanalyser-0.3.7/pysoundanalyser.egg-info/requires.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       16 2024-05-02 20:32:29.000000 pysoundanalyser-0.3.7/pysoundanalyser.egg-info/top_level.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2013-02-19 11:18:49.000000 pysoundanalyser-0.3.7/resources.qrc
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:30.496268 pysoundanalyser-0.3.7/scripts/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       94 2015-10-11 12:48:00.000000 pysoundanalyser-0.3.7/scripts/pysoundanalyser-launcher.bat
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2024-05-02 20:32:30.524268 pysoundanalyser-0.3.7/setup.cfg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1883 2024-05-02 20:31:59.000000 pysoundanalyser-0.3.7/setup_cx.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-05-02 20:32:30.524268 pysoundanalyser-0.3.7/translations/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2024-05-02 20:32:09.000000 pysoundanalyser-0.3.7/translations/pysoundanalyser_de.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2024-05-02 20:32:09.000000 pysoundanalyser-0.3.7/translations/pysoundanalyser_el.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      122 2024-05-02 20:32:09.000000 pysoundanalyser-0.3.7/translations/pysoundanalyser_en_GB.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2024-05-02 20:32:09.000000 pysoundanalyser-0.3.7/translations/pysoundanalyser_es.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      235 2024-05-02 20:32:09.000000 pysoundanalyser-0.3.7/translations/pysoundanalyser_fr.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    25701 2024-05-02 20:32:09.000000 pysoundanalyser-0.3.7/translations/pysoundanalyser_it.qm
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    17558 2013-02-19 23:27:27.000000 pysoundanalyser-0.3.7/translations/pysoundanalyser_it_IT.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       44 2024-05-02 20:32:09.000000 pysoundanalyser-0.3.7/translations/pysoundanalyser_ru.qm
```

### Comparing `pysoundanalyser-0.3.4/COPYING.txt` & `pysoundanalyser-0.3.7/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/MANIFEST.in` & `pysoundanalyser-0.3.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/PKG-INFO` & `pysoundanalyser-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoundanalyser
-Version: 0.3.4
+Version: 0.3.7
 Summary: Python program for visualizing short sounds (waveform, spectrum, etc...)
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,11 +693,17 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING.txt
+Requires-Dist: matplotlib>=3.0.0
+Requires-Dist: numpy>=1.0.0
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: PyAudio>=0.2.11
+Requires-Dist: PyQt6>=6.6.0
+Requires-Dist: scipy>=1.0.1
 
 [![Project Status: Unsupported – The project has reached a stable, usable state but the author(s) have ceased all work on it. A new maintainer may be desired.](https://www.repostatus.org/badges/latest/unsupported.svg)](https://www.repostatus.org/#unsupported)
 
 `pysoundanalyser` is an application which provides a graphical user interface to analyse short wav files.
```

### Comparing `pysoundanalyser-0.3.4/icons/exit.svg` & `pysoundanalyser-0.3.7/icons/exit.svg`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.ico` & `pysoundanalyser-0.3.7/icons/johnny_automatic_crashing_wave.ico`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.png` & `pysoundanalyser-0.3.7/icons/johnny_automatic_crashing_wave.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.svg` & `pysoundanalyser-0.3.7/icons/johnny_automatic_crashing_wave.svg`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/debian/changelog` & `pysoundanalyser-0.3.7/prep-release/debian/changelog`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/debian/control` & `pysoundanalyser-0.3.7/prep-release/debian/control`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/debian/copyright` & `pysoundanalyser-0.3.7/prep-release/debian/copyright`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/debian/rules` & `pysoundanalyser-0.3.7/prep-release/debian/rules`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/launchpad/debian/changelog` & `pysoundanalyser-0.3.7/prep-release/launchpad/debian/changelog`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/launchpad/debian/control` & `pysoundanalyser-0.3.7/prep-release/launchpad/debian/control`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/launchpad/debian/copyright` & `pysoundanalyser-0.3.7/prep-release/launchpad/debian/copyright`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/launchpad/debian/rules` & `pysoundanalyser-0.3.7/prep-release/launchpad/debian/rules`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/launchpad_build.py` & `pysoundanalyser-0.3.7/prep-release/launchpad_build.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/make_deb.py` & `pysoundanalyser-0.3.7/prep-release/make_deb.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/mkupdate_pyqt6.sh` & `pysoundanalyser-0.3.7/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/pysoundanalyser.pro` & `pysoundanalyser-0.3.7/prep-release/pysoundanalyser.pro`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_it.ts` & `pysoundanalyser-0.3.7/prep-release/pysoundanalyser_it.ts`

 * *Files 14% similar despite different names*

#### Comparing `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_it.ts` & `pysoundanalyser-0.3.7/prep-release/pysoundanalyser_it.ts`

```diff
@@ -1,14 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
 <TS version="2.1" language="it_IT">
   <context>
     <name/>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="376"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="349"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="327"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="305"/>
       <source>Type:</source>
       <translation type="unfinished">Tipo:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="305"/>
       <source>Sinusoid</source>
       <translation type="unfinished">Sinusoide</translation>
@@ -26,14 +29,15 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="376"/>
       <source>Huggins Pitch</source>
       <translation type="unfinished">Pitch di Huggins</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="400"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="397"/>
       <source>Dichotic Difference:</source>
       <translation type="unfinished">Differenza dicotica:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="397"/>
       <source>IPD Linear</source>
       <translation type="unfinished">IPD Lineare</translation>
@@ -46,14 +50,16 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="400"/>
       <source>ITD</source>
       <translation type="unfinished">ITD</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="457"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="454"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="451"/>
       <source>Harmonicity:</source>
       <translation type="unfinished">Armonicità:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="451"/>
       <source>Harmonic</source>
       <translation type="unfinished">Armonico:</translation>
@@ -78,22 +84,20 @@
       <source>None</source>
       <translation type="unfinished">Nessuno</translation>
     </message>
   </context>
   <context>
     <name>Preferences Window</name>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="462"/>
       <source>custom</source>
-      <translation type="obsolete">personalizzato</translation>
+      <translation type="vanished">personalizzato</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="462"/>
       <source>System Settings</source>
-      <translation type="obsolete">Setting del sistema</translation>
+      <translation type="vanished">Setting del sistema</translation>
     </message>
   </context>
   <context>
     <name>acfPlot</name>
     <message>
       <location filename="../pysoundanalyser/win_acf_plot.py" line="84"/>
       <source>Window:</source>
@@ -126,17 +130,16 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/win_acf_plot.py" line="153"/>
       <source>Input Dialog</source>
       <translation>Dialogo di input</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_acf_plot.py" line="153"/>
       <source>Grid</source>
-      <translation type="obsolete">Griglia</translation>
+      <translation type="vanished">Griglia</translation>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="148"/>
       <source>Python Sound Analyser</source>
@@ -174,15 +177,16 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="177"/>
       <source>&amp;Get</source>
       <translation>&amp;Ottieni</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="802"/>
+      <location filename="../pysoundanalyser/__main__.py" line="803"/>
+      <location filename="../pysoundanalyser/__main__.py" line="178"/>
       <source>Root Mean Square</source>
       <translation/>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="183"/>
       <source>&amp;Process</source>
       <translation>&amp;Trasforma</translation>
@@ -224,15 +228,16 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="204"/>
       <source>Silence</source>
       <translation>Silenzio</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1263"/>
+      <location filename="../pysoundanalyser/__main__.py" line="207"/>
       <source>Sinusoid</source>
       <translation>Sinusoide</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="212"/>
       <source>&amp;Plot</source>
       <translation/>
@@ -240,29 +245,33 @@
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="213"/>
       <source>Waveform</source>
       <translation>Onda sonora</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="276"/>
+      <location filename="../pysoundanalyser/__main__.py" line="217"/>
       <source>Spectrum</source>
       <translation>Spettro</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="279"/>
+      <location filename="../pysoundanalyser/__main__.py" line="221"/>
       <source>Spectrogram</source>
       <translation>Spettrogramma</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="283"/>
+      <location filename="../pysoundanalyser/__main__.py" line="225"/>
       <source>Autocorrelation</source>
       <translation>Autocorrelazione</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="286"/>
+      <location filename="../pysoundanalyser/__main__.py" line="229"/>
       <source>Autocorrelogram</source>
       <translation>Autocorrelogramma</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="234"/>
       <source>&amp;Help</source>
       <translation>&amp;Aiuto</translation>
@@ -274,15 +283,16 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="240"/>
       <source>Manual (pdf)</source>
       <translation>Manuale (pdf)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1476"/>
+      <location filename="../pysoundanalyser/__main__.py" line="244"/>
       <source>About pysoundanalyser</source>
       <translation>Riguardo pysoundanalyser</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="253"/>
       <source>Load Sound</source>
       <translation>Carica suono</translation>
@@ -329,15 +339,17 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="297"/>
       <source>Scale</source>
       <translation>Scalare</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="758"/>
+      <location filename="../pysoundanalyser/__main__.py" line="762"/>
+      <location filename="../pysoundanalyser/__main__.py" line="750"/>
+      <location filename="../pysoundanalyser/__main__.py" line="301"/>
       <source>Level Difference</source>
       <translation>Differenza di livello</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="305"/>
       <source>Concatenate</source>
       <translation>Concatena</translation>
@@ -354,98 +366,159 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="315"/>
       <source>Move Up</source>
       <translation>Sposta su</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="326"/>
+      <location filename="../pysoundanalyser/__main__.py" line="324"/>
       <source>Label</source>
       <translation>Etichetta</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="326"/>
+      <location filename="../pysoundanalyser/__main__.py" line="324"/>
       <source>Channel</source>
       <translation>Canale</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="356"/>
+      <location filename="../pysoundanalyser/__main__.py" line="353"/>
       <source>No Selection</source>
       <translation>Nessuna Selezione</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="978"/>
+      <location filename="../pysoundanalyser/__main__.py" line="976"/>
+      <location filename="../pysoundanalyser/__main__.py" line="945"/>
+      <location filename="../pysoundanalyser/__main__.py" line="894"/>
+      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="816"/>
+      <location filename="../pysoundanalyser/__main__.py" line="808"/>
+      <location filename="../pysoundanalyser/__main__.py" line="795"/>
+      <location filename="../pysoundanalyser/__main__.py" line="778"/>
+      <location filename="../pysoundanalyser/__main__.py" line="767"/>
+      <location filename="../pysoundanalyser/__main__.py" line="747"/>
+      <location filename="../pysoundanalyser/__main__.py" line="733"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
+      <location filename="../pysoundanalyser/__main__.py" line="718"/>
+      <location filename="../pysoundanalyser/__main__.py" line="709"/>
+      <location filename="../pysoundanalyser/__main__.py" line="700"/>
+      <location filename="../pysoundanalyser/__main__.py" line="691"/>
+      <location filename="../pysoundanalyser/__main__.py" line="682"/>
+      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="643"/>
+      <location filename="../pysoundanalyser/__main__.py" line="610"/>
+      <location filename="../pysoundanalyser/__main__.py" line="602"/>
+      <location filename="../pysoundanalyser/__main__.py" line="534"/>
+      <location filename="../pysoundanalyser/__main__.py" line="418"/>
+      <location filename="../pysoundanalyser/__main__.py" line="405"/>
       <source>Warning</source>
       <translation>Avviso</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="420"/>
+      <location filename="../pysoundanalyser/__main__.py" line="418"/>
+      <location filename="../pysoundanalyser/__main__.py" line="405"/>
       <source>Only one sound can be moved at a time</source>
       <translation>Si può spostare solo un suono alla volta</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="433"/>
+      <location filename="../pysoundanalyser/__main__.py" line="430"/>
       <source>pysoundanalyser - Choose file to load</source>
       <translation>pysoundanalyser - Scegli file da caricare</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="433"/>
+      <location filename="../pysoundanalyser/__main__.py" line="430"/>
       <source>Supported Sound Files (*.wav);;All Files (*)</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1428"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1424"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1353"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1320"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1127"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1089"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1025"/>
+      <location filename="../pysoundanalyser/__main__.py" line="827"/>
+      <location filename="../pysoundanalyser/__main__.py" line="622"/>
+      <location filename="../pysoundanalyser/__main__.py" line="449"/>
       <source>Left</source>
       <translation>Sinistro</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1425"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1421"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1374"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1351"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1318"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1125"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1086"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1023"/>
+      <location filename="../pysoundanalyser/__main__.py" line="825"/>
+      <location filename="../pysoundanalyser/__main__.py" line="620"/>
+      <location filename="../pysoundanalyser/__main__.py" line="486"/>
       <source>Right</source>
       <translation>Destro</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="530"/>
+      <location filename="../pysoundanalyser/__main__.py" line="528"/>
       <source>Cannot open %1 IOError</source>
       <translation>Impossibile aprire %1 IOError</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="547"/>
+      <location filename="../pysoundanalyser/__main__.py" line="546"/>
       <source>No Selection</source>
       <translation>Nessuna selezione</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="558"/>
+      <location filename="../pysoundanalyser/__main__.py" line="557"/>
       <source>{0} is 
  {1} {2} dB than 
  {3}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="560"/>
+      <location filename="../pysoundanalyser/__main__.py" line="559"/>
       <source>Multiple Selection</source>
       <translation>Selezione multipla</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="572"/>
+      <location filename="../pysoundanalyser/__main__.py" line="571"/>
       <source>Duration: {0} sec.
 
 Channel: {1} 
 
 Samp. Freq.: {2} 
 
 Bits: {3}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="978"/>
+      <location filename="../pysoundanalyser/__main__.py" line="976"/>
+      <location filename="../pysoundanalyser/__main__.py" line="945"/>
+      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="808"/>
+      <location filename="../pysoundanalyser/__main__.py" line="795"/>
+      <location filename="../pysoundanalyser/__main__.py" line="778"/>
+      <location filename="../pysoundanalyser/__main__.py" line="767"/>
+      <location filename="../pysoundanalyser/__main__.py" line="747"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
+      <location filename="../pysoundanalyser/__main__.py" line="709"/>
+      <location filename="../pysoundanalyser/__main__.py" line="700"/>
+      <location filename="../pysoundanalyser/__main__.py" line="691"/>
+      <location filename="../pysoundanalyser/__main__.py" line="682"/>
+      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="643"/>
+      <location filename="../pysoundanalyser/__main__.py" line="602"/>
       <source>No sound selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="609"/>
+      <location filename="../pysoundanalyser/__main__.py" line="610"/>
       <source>Cannot write sounds with different sample rates</source>
       <translation>Impossibile salvare suoni con frequenze di campionamento diverse</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="628"/>
       <source>Mono</source>
       <translation/>
@@ -462,385 +535,453 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>All Files (*)</source>
       <translation>Tutti i file (*)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="713"/>
+      <location filename="../pysoundanalyser/__main__.py" line="718"/>
       <source>Only one sound can be renamed at a time</source>
       <translation>Si può cambiare solo il nome di un suono alla volta</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="719"/>
+      <location filename="../pysoundanalyser/__main__.py" line="724"/>
       <source>New name:</source>
       <translation>Nuovo nome:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="720"/>
+      <location filename="../pysoundanalyser/__main__.py" line="725"/>
       <source>Input Dialog</source>
       <translation>Dialogo di input</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="728"/>
+      <location filename="../pysoundanalyser/__main__.py" line="733"/>
       <source>Only sound can be changed at a time</source>
       <translation>Si può cambiare solo un suono alla volta</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="746"/>
+      <location filename="../pysoundanalyser/__main__.py" line="750"/>
       <source>Only two sounds can be compared at a time</source>
       <translation>Solo due suoni alla volta possono essere comparati</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="758"/>
+      <location filename="../pysoundanalyser/__main__.py" line="762"/>
       <source>{0} is {1} {2} dB than {3}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="766"/>
+      <location filename="../pysoundanalyser/__main__.py" line="769"/>
       <source>Scale Level</source>
       <translation>Scalare il livello</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="766"/>
+      <location filename="../pysoundanalyser/__main__.py" line="769"/>
       <source>Add or subtract decibels</source>
       <translation>Aggiungi o rimuovi decibel</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="801"/>
+      <location filename="../pysoundanalyser/__main__.py" line="802"/>
       <source>{0} {1} : {2}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="817"/>
+      <location filename="../pysoundanalyser/__main__.py" line="816"/>
       <source>Cannot play sounds with different sample rates</source>
       <translation>Non è possibile riprodurre suoni con frequenza di campionamento diversa</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="879"/>
+      <location filename="../pysoundanalyser/__main__.py" line="878"/>
       <source>none</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="895"/>
+      <location filename="../pysoundanalyser/__main__.py" line="894"/>
       <source>No sounds selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="904"/>
+      <location filename="../pysoundanalyser/__main__.py" line="903"/>
+      <location filename="../pysoundanalyser/__main__.py" line="897"/>
       <source>Concatenate Sounds</source>
       <translation>Concatena suoni</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="898"/>
+      <location filename="../pysoundanalyser/__main__.py" line="897"/>
       <source>Only two sounds can be concatenated at a time</source>
       <translation>Solo due suoni alla volta possono essere concatenati</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="904"/>
+      <location filename="../pysoundanalyser/__main__.py" line="903"/>
       <source>Cannot concatenate sounds with different sampling rates</source>
       <translation>Impossibile concatenare suoni con frequenze di campionamento differenti</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="968"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
+      <location filename="../pysoundanalyser/__main__.py" line="964"/>
       <source>Cut Sound</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="966"/>
+      <location filename="../pysoundanalyser/__main__.py" line="964"/>
       <source>Values out of range</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="968"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
       <source>Cannot cut entire sound, please use remove button</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="983"/>
+      <location filename="../pysoundanalyser/__main__.py" line="981"/>
       <source>lowpass</source>
       <translation>passabasso</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="990"/>
+      <location filename="../pysoundanalyser/__main__.py" line="988"/>
       <source>highpass</source>
       <translation>passaalto</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="997"/>
+      <location filename="../pysoundanalyser/__main__.py" line="995"/>
       <source>bandpass</source>
       <translation>passabanda</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1006"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1004"/>
       <source>bandstop</source>
       <translation>fermabanda</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1381"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1378"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1355"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1322"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1276"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1129"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1027"/>
       <source>Both</source>
       <translation>Entrambe</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1029"/>
       <source>White</source>
       <translation>Bianco</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1287"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
       <source>Pink</source>
       <translation>Rosa</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1037"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1035"/>
       <source>Red</source>
       <translation>Rosso</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1041"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1039"/>
       <source>Blue</source>
       <translation>Blu</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1045"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1043"/>
       <source>Violet</source>
       <translation>Viola</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1181"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1220"/>
       <source>F0 (Hz)</source>
       <translation type="obsolete">F0 (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1221"/>
       <source>Bandwidth (Hz)</source>
       <translation type="obsolete">Larghezza di banda (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1183"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>Bandwidth (Cents)</source>
       <translation type="obsolete">Larghezza di banda (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1184"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Spacing (Cents)</source>
       <translation type="obsolete">Intervallo (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>ITD (micro s)</source>
       <translation type="obsolete">ITD (micro s)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1186"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>IPD (radians)</source>
       <translation type="obsolete">IPD (radianti)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1187"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation type="obsolete">Livello componenti banda stretta (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1188"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>Iterations</source>
       <translation type="obsolete">Iterazioni</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1189"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Gain</source>
       <translation type="obsolete">Gain</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1190"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Low Harmonic</source>
       <translation type="obsolete">Armonica inferiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1191"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>High Harmonic</source>
       <translation type="obsolete">Armonica superiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1192"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Freq. (Hz)</source>
       <translation type="obsolete">Frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Freq. (Hz)</source>
       <translation type="obsolete">Frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1194"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Stop</source>
       <translation type="obsolete">Stop inferiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Stop</source>
       <translation type="obsolete">Stop superiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1196"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation type="obsolete">Livello armonico (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1197"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation type="obsolete">Livello spettrale (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1198"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Component Level (dB SPL)</source>
       <translation type="obsolete">Livello componente (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1199"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1372"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1314"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Duration (ms)</source>
       <translation type="obsolete">Durata (ms)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1200"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Ramp (ms)</source>
       <translation type="obsolete">Rampa (sm)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1201"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation type="obsolete">Rumore 1 frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1202"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1241"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation type="obsolete">Rumore 1 frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1203"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation type="obsolete">Livello rumore 1 (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1204"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation type="obsolete">Rumore 2 frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1205"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation type="obsolete">Rumore 1 frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1206"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation type="obsolete">Livello rumore 2 (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1207"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>Stretch (%)</source>
       <translation type="obsolete">Allungamento (%)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1208"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation type="obsolete">Intervallo armonico (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1210"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1373"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1317"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Ear:</source>
       <translation type="obsolete">Orecchio:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1211"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1250"/>
       <source>Type:</source>
       <translation type="obsolete">Tipo:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1251"/>
       <source>Phase:</source>
       <translation type="obsolete">Fase:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1213"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Noise Type:</source>
       <translation type="obsolete">Tipo rumore:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
+      <source>Dichotic Noise Type:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>IRN Type:</source>
       <translation type="obsolete">Tipo IRN:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1216"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
       <source>Phase relationship:</source>
       <translation type="obsolete">Relazione di fase:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1217"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>Dichotic Difference:</source>
       <translation type="obsolete">Differenza dicotica:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1218"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Harmonicity:</source>
       <translation type="obsolete">Armonicità:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
+      <source>Bandwidth Unit:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
       <source>Narrowband Noise</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1269"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
       <source>IRN</source>
       <translation>IRN</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
       <source>Huggins Pitch</source>
       <translation>Pitch di Huggins</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
       <source>IPD Linear</source>
       <translation>IPD Lineare</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
       <source>IPD Stepped</source>
       <translation>IPD a scalino</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1275"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>ITD</source>
       <translation>ITD</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1278"/>
       <source>None</source>
       <translation>Nessuno</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1279"/>
       <source>Odd Left</source>
       <translation>Dispari a sinistra</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1279"/>
       <source>Odd Right</source>
       <translation>Dispari a destra</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1309"/>
       <source>Frequency (Hz)</source>
       <translation type="obsolete">Frequenza (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1310"/>
+      <source>AM Frequency (Hz)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
+      <source>AM Depth</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
+      <source>Carrier Phase (radians)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
+      <source>Modulation Phase (radians)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1348"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1316"/>
+      <source>Level (dB SPL)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1342"/>
+      <source>Carrier Frequency (Hz)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1343"/>
+      <source>Modulation Frequency (Hz)</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
+      <source>Modulation Index</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../pysoundanalyser/__main__.py" line="1477"/>
       <source>&lt;b&gt;pysoundanalyser - Python Sound Analyser&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2010-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -854,88 +995,76 @@
                 &lt;p&gt;
                 You should have received a copy of the GNU General Public License
                 along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
                 &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>Python Sound Analyzer</source>
-      <translation type="obsolete">Python Analizzatore di suoni</translation>
+      <translation type="vanished">Python Analizzatore di suoni</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>Supported Sound Files (*.wav *.flac *.aiff *.aif *.ogg *.au *.snd *.caf *.avr *.mat);;All Files (*)</source>
-      <translation type="obsolete">File sonori supportati (*.wav *.flac *.aiff *.aif *.ogg *.au *.snd *.caf *.avr *.mat);;Titti i File (*)</translation>
+      <translation type="vanished">File sonori supportati (*.wav *.flac *.aiff *.aif *.ogg *.au *.snd *.caf *.avr *.mat);;Titti i File (*)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>R</source>
-      <translation type="obsolete">D</translation>
+      <translation type="vanished">D</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>L</source>
-      <translation type="obsolete">S</translation>
+      <translation type="vanished">S</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>%1 is %2 %L3 dB than %4</source>
-      <translation type="obsolete">%1 è %2 %L3 dB di %4</translation>
+      <translation type="vanished">%1 è %2 %L3 dB di %4</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>%1 is 
  %2 %L3 dB than 
  %4</source>
-      <translation type="obsolete">%1 è 
+      <translation type="vanished">%1 è 
  %2 %L3 dB di 
  %4</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>.%1</source>
-      <translation type="obsolete">.%1</translation>
+      <translation type="vanished">.%1</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>Duration: %L1 sec.
 
 Channel: %2 
 
 Samp. Freq.: %L3 
 
 Format: %4</source>
-      <translation type="obsolete">Durata: %L1 sec.
+      <translation type="vanished">Durata: %L1 sec.
 
 Canale: %2 
 
 Freq. Campionamento: %L3 
 
 Formato: %4</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>white</source>
-      <translation type="obsolete">bianco</translation>
+      <translation type="vanished">bianco</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>pink</source>
-      <translation type="obsolete">rosa</translation>
+      <translation type="vanished">rosa</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>Simple Dichotic</source>
-      <translation type="obsolete">Dicotico semplice</translation>
+      <translation type="vanished">Dicotico semplice</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1441"/>
       <source>Narrowband Noise 2</source>
-      <translation type="obsolete">Rumore a banda stretta 2</translation>
+      <translation type="vanished">Rumore a banda stretta 2</translation>
     </message>
   </context>
   <context>
     <name>applyChanges</name>
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="469"/>
       <source>There are unsaved changes. Apply Changes?</source>
@@ -952,64 +1081,82 @@
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="38"/>
       <source>Filter Type:</source>
       <translation>Tipo di filtro:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="133"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="79"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="50"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="40"/>
       <source>lowpass</source>
       <translation>passabasso</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="145"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="93"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="40"/>
       <source>highpass</source>
       <translation>passaalto</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="157"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="106"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="40"/>
       <source>bandpass</source>
       <translation>passabanda</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="181"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="106"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="40"/>
       <source>bandstop</source>
       <translation>fermabanda</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="44"/>
       <source>Filter Order:</source>
       <translation>Ordine filtro:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="146"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="134"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="51"/>
       <source>Cutoff:</source>
       <translation>Cutoff:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="183"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="171"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="135"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="52"/>
       <source>End Transition Band = Cutoff *</source>
       <translation/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="72"/>
       <source>Apply Filter</source>
       <translation>Applica Filtro</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="195"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="159"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="147"/>
       <source>Start Transition Band = Cutoff *</source>
       <translation>Inizio banda di transizione = Cutoff*</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="182"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="158"/>
       <source>Lower Cutoff:</source>
       <translation>Cutoff inferiore:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_apply_filter.py" line="194"/>
+      <location filename="../pysoundanalyser/dialog_apply_filter.py" line="170"/>
       <source>Higher Cutoff:</source>
       <translation>Cutoff superiore:</translation>
     </message>
   </context>
   <context>
     <name>autocorrelogramPlot</name>
     <message>
@@ -1029,27 +1176,24 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/win_autocorrelogram_plot.py" line="123"/>
       <source>Color Map:</source>
       <translation>Mappa colori:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_autocorrelogram_plot.py" line="123"/>
       <source>Time (s)</source>
-      <translation type="obsolete">Tempo (s)</translation>
+      <translation type="vanished">Tempo (s)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_autocorrelogram_plot.py" line="123"/>
       <source>Lag (s)</source>
-      <translation type="obsolete">Ritardo (s)</translation>
+      <translation type="vanished">Ritardo (s)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_autocorrelogram_plot.py" line="123"/>
       <source>Grid</source>
-      <translation type="obsolete">Griglia</translation>
+      <translation type="vanished">Griglia</translation>
     </message>
   </context>
   <context>
     <name>changeChannelDialog</name>
     <message>
       <location filename="../pysoundanalyser/dialog_change_channel.py" line="32"/>
       <source>Channel:</source>
@@ -1067,22 +1211,20 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_change_channel.py" line="47"/>
       <source>Change Channel</source>
       <translation>Cambia canale</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_change_channel.py" line="47"/>
       <source>R</source>
-      <translation type="obsolete">D</translation>
+      <translation type="vanished">D</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_change_channel.py" line="47"/>
       <source>L</source>
-      <translation type="obsolete">S</translation>
+      <translation type="vanished">S</translation>
     </message>
   </context>
   <context>
     <name>concatenateDialog</name>
     <message>
       <location filename="../pysoundanalyser/dialog_concatenate.py" line="41"/>
       <source>Sound 1:</source>
@@ -1130,291 +1272,212 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_concatenate.py" line="101"/>
       <source>Concatenate</source>
       <translation>Concatena</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_concatenate.py" line="101"/>
       <source>R</source>
-      <translation type="obsolete">D</translation>
+      <translation type="vanished">D</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_concatenate.py" line="101"/>
       <source>L</source>
-      <translation type="obsolete">S</translation>
+      <translation type="vanished">S</translation>
     </message>
   </context>
   <context>
     <name>dialog</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>F0 (Hz)</source>
-      <translation>F0 (Hz)</translation>
+      <translation type="vanished">F0 (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Bandwidth (Hz)</source>
-      <translation>Larghezza di banda (Hz)</translation>
+      <translation type="vanished">Larghezza di banda (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>Bandwidth (Cents)</source>
-      <translation>Larghezza di banda (centesimi)</translation>
+      <translation type="vanished">Larghezza di banda (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>Spacing (Cents)</source>
-      <translation>Intervallo (centesimi)</translation>
+      <translation type="vanished">Intervallo (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>ITD (micro s)</source>
-      <translation>ITD (micro s)</translation>
+      <translation type="vanished">ITD (micro s)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>IPD (radians)</source>
-      <translation>IPD (radianti)</translation>
+      <translation type="vanished">IPD (radianti)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Narrow Band Component Level (dB SPL)</source>
-      <translation>Livello componenti banda stretta (dB SPL)</translation>
+      <translation type="vanished">Livello componenti banda stretta (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Iterations</source>
-      <translation>Iterazioni</translation>
+      <translation type="vanished">Iterazioni</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>Gain</source>
-      <translation>Gain</translation>
+      <translation type="vanished">Gain</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Harmonic</source>
-      <translation>Armonica inferiore</translation>
+      <translation type="vanished">Armonica inferiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Harmonic</source>
-      <translation>Armonica superiore</translation>
+      <translation type="vanished">Armonica superiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Freq. (Hz)</source>
-      <translation>Frequenza inferiore (Hz)</translation>
+      <translation type="vanished">Frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Freq. (Hz)</source>
-      <translation>Frequenza superiore (Hz)</translation>
+      <translation type="vanished">Frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Low Stop</source>
-      <translation>Stop inferiore</translation>
+      <translation type="vanished">Stop inferiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>High Stop</source>
-      <translation>Stop superiore</translation>
+      <translation type="vanished">Stop superiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Harmonic Level (dB SPL)</source>
-      <translation>Livello armonico (dB SPL)</translation>
+      <translation type="vanished">Livello armonico (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Spectrum Level (dB SPL)</source>
-      <translation>Livello spettrale (dB SPL)</translation>
+      <translation type="vanished">Livello spettrale (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Component Level (dB SPL)</source>
-      <translation>Livello componente (dB SPL)</translation>
+      <translation type="vanished">Livello componente (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1375"/>
       <source>Duration (ms)</source>
-      <translation>Durata (ms)</translation>
+      <translation type="vanished">Durata (ms)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
       <source>Ramp (ms)</source>
-      <translation>Rampa (sm)</translation>
+      <translation type="vanished">Rampa (sm)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 Low Freq. (Hz)</source>
-      <translation>Rumore 1 frequenza inferiore (Hz)</translation>
+      <translation type="vanished">Rumore 1 frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 1 High Freq. (Hz)</source>
-      <translation>Rumore 1 frequenza superiore (Hz)</translation>
+      <translation type="vanished">Rumore 1 frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 1 S. Level (dB SPL)</source>
-      <translation>Livello rumore 1 (dB SPL)</translation>
+      <translation type="vanished">Livello rumore 1 (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 Low Freq. (Hz)</source>
-      <translation>Rumore 2 frequenza inferiore (Hz)</translation>
+      <translation type="vanished">Rumore 2 frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>No. 2 High Freq. (Hz)</source>
-      <translation>Rumore 1 frequenza superiore (Hz)</translation>
+      <translation type="vanished">Rumore 1 frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>No. 2 S. Level (dB SPL)</source>
-      <translation>Livello rumore 2 (dB SPL)</translation>
+      <translation type="vanished">Livello rumore 2 (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1248"/>
       <source>Stretch (%)</source>
-      <translation>Allungamento (%)</translation>
+      <translation type="vanished">Allungamento (%)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Harmonic Spacing (Cents)</source>
-      <translation>Intervallo armonico (centesimi)</translation>
+      <translation type="vanished">Intervallo armonico (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
       <source>Ear:</source>
-      <translation>Orecchio:</translation>
+      <translation type="vanished">Orecchio:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Type:</source>
-      <translation>Tipo:</translation>
+      <translation type="vanished">Tipo:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
       <source>Phase:</source>
-      <translation>Fase:</translation>
+      <translation type="vanished">Fase:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>Noise Type:</source>
-      <translation>Tipo rumore:</translation>
+      <translation type="vanished">Tipo rumore:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>IRN Type:</source>
-      <translation>Tipo IRN:</translation>
+      <translation type="vanished">Tipo IRN:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Phase relationship:</source>
-      <translation>Relazione di fase:</translation>
+      <translation type="vanished">Relazione di fase:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
       <source>Dichotic Difference:</source>
-      <translation>Differenza dicotica:</translation>
+      <translation type="vanished">Differenza dicotica:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1259"/>
       <source>Harmonicity:</source>
-      <translation>Armonicità:</translation>
+      <translation type="vanished">Armonicità:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
       <source>Frequency (Hz)</source>
-      <translation>Frequenza (Hz)</translation>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
-      <source>Dichotic Noise Type:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1260"/>
-      <source>Bandwidth Unit:</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
-      <source>AM Frequency (Hz)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
-      <source>AM Depth</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
-      <source>Carrier Phase (radians)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
-      <source>Modulation Phase (radians)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1350"/>
-      <source>Level (dB SPL)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
-      <source>Carrier Frequency (Hz)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
-      <source>Modulation Frequency (Hz)</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
-      <source>Modulation Index</source>
-      <translation type="unfinished"/>
+      <translation type="vanished">Frequenza (Hz)</translation>
     </message>
   </context>
   <context>
     <name>generateNoiseDialog</name>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_noise.py" line="38"/>
       <source>Noise Type:</source>
       <translation>Tipo di rumore:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_noise.py" line="102"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="85"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="40"/>
       <source>White</source>
       <translation>Bianco</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_noise.py" line="113"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="104"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="40"/>
       <source>Pink</source>
       <translation>Rosa</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_noise.py" line="113"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="104"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="40"/>
       <source>Red</source>
       <translation>Rosso</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_noise.py" line="113"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="104"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="40"/>
       <source>Blue</source>
       <translation>Blu</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_noise.py" line="113"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="104"/>
+      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="40"/>
       <source>Violet</source>
       <translation>Viola</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_noise.py" line="46"/>
       <source>Sound Label:</source>
       <translation>Nome Suono:</translation>
@@ -1471,17 +1534,16 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_noise.py" line="114"/>
       <source>re. (Hz):</source>
       <translation>re. (Hz):</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_noise.py" line="114"/>
       <source>pink</source>
-      <translation type="obsolete">rosa</translation>
+      <translation type="vanished">rosa</translation>
     </message>
   </context>
   <context>
     <name>generateSinusoidDialog</name>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="38"/>
       <source>Sound Label:</source>
@@ -1525,24 +1587,33 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="85"/>
       <source>Ear:</source>
       <translation>Orecchio:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="169"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="155"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="143"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="92"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="87"/>
       <source>Right</source>
       <translation>Destro</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="169"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="155"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="143"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="87"/>
       <source>Left</source>
       <translation>Sinistro</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="145"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="112"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="87"/>
       <source>Both</source>
       <translation>Entrambe</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="103"/>
       <source>Generate Sinusoid</source>
       <translation>Genera sinusoide</translation>
@@ -1550,14 +1621,15 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="146"/>
       <source>ITD (us)</source>
       <translation>ITD (us)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="167"/>
+      <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="153"/>
       <source>Reference</source>
       <translation>Referenza</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sinusoid.py" line="160"/>
       <source>ILD (dB)</source>
       <translation>ILD (dB)</translation>
@@ -1583,59 +1655,97 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="176"/>
       <source>F0 (Hz)</source>
       <translation>F0 (Hz)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="386"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="352"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="337"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="306"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="179"/>
       <source>Bandwidth (Hz)</source>
       <translation>Larghezza di banda (Hz)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="377"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="353"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="328"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="307"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="182"/>
       <source>Bandwidth (Cents)</source>
       <translation>Larghezza di banda (centesimi)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="378"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="354"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="329"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="308"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="185"/>
       <source>Spacing (Cents)</source>
       <translation>Intervallo (centesimi)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="402"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="398"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="379"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="355"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="330"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="309"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="188"/>
       <source>ITD (micro s)</source>
       <translation>ITD (micro s)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="401"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="399"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="380"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="356"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="331"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="310"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="191"/>
       <source>IPD (radians)</source>
       <translation>IPD (radianti)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="381"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="357"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="332"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="311"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="194"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation>Livello componenti banda stretta (dB SPL)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="382"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="362"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="333"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="312"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="197"/>
       <source>Iterations</source>
       <translation>Iterazioni</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="383"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="363"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="334"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="313"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="200"/>
       <source>Gain</source>
       <translation>Gain</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="350"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="203"/>
       <source>Low Harmonic</source>
       <translation>Armonica inferiore</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="351"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="206"/>
       <source>High Harmonic</source>
       <translation>Armonica superiore</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="209"/>
       <source>Low Freq. (Hz)</source>
       <translation>Frequenza inferiore (Hz)</translation>
@@ -1653,89 +1763,138 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="218"/>
       <source>High Stop</source>
       <translation>Stop superiore</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="384"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="358"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="335"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="316"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="221"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation>Livello armonico (dB SPL)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="387"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="364"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="338"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="314"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="224"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation>Livello spettrale (dB SPL)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="385"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="359"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="336"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="315"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="227"/>
       <source>Component Level (dB SPL)</source>
       <translation>Livello componente (dB SPL)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="591"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="554"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="503"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="230"/>
       <source>Duration (ms)</source>
       <translation>Durata (ms)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="557"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="506"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="233"/>
       <source>Ramp (ms)</source>
       <translation>Rampa (sm)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="470"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="463"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="236"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation>Rumore 1 frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="470"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="471"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="464"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="239"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation>Rumore 1 frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="470"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="472"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="465"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="242"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation>Livello rumore 1 (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="470"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="473"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="466"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="245"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation>Rumore 2 frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="470"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="474"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="467"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="248"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation>Rumore 1 frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="470"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="475"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="468"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="251"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation>Livello rumore 2 (dB SPL)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="456"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="453"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="360"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="254"/>
       <source>Stretch (%)</source>
       <translation>Allungamento (%)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="458"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="455"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="452"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="361"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="257"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation>Intervallo armonico (centesimi)</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="595"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="564"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="513"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="262"/>
       <source>Right</source>
       <translation>Destro</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="595"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="564"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="513"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="262"/>
       <source>Left</source>
       <translation>Sinistro</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="597"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="595"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="566"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="564"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="515"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="513"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="264"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="262"/>
       <source>Both</source>
       <translation>Entrambe</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="262"/>
       <source>Odd Left</source>
       <translation>Dispari a sinistra</translation>
@@ -1743,19 +1902,27 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="262"/>
       <source>Odd Right</source>
       <translation>Dispari a destra</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="596"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="565"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="514"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="393"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="365"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="343"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="322"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="263"/>
       <source>Ear:</source>
       <translation>Orecchio:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="267"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="265"/>
       <source>Sinusoid</source>
       <translation>Sinusoide</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="265"/>
       <source>Narrowband Noise</source>
       <translation>Rumore a banda stretta</translation>
@@ -1773,14 +1940,15 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="266"/>
       <source>Type:</source>
       <translation>Tipo:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="270"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="268"/>
       <source>Sine</source>
       <translation>Sin</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="268"/>
       <source>Cosine</source>
       <translation>Cos</translation>
@@ -1798,109 +1966,146 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="268"/>
       <source>Random</source>
       <translation>Randomizzata</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="394"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="368"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="339"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="323"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="269"/>
       <source>Phase:</source>
       <translation>Fase:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="277"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="275"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="273"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="271"/>
       <source>White</source>
       <translation>Bianco</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="275"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="271"/>
       <source>Pink</source>
       <translation>Rosa</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="271"/>
       <source>None</source>
       <translation>Nessuno</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="366"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="344"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="324"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="272"/>
       <source>Noise Type:</source>
       <translation>Tipo rumore:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="391"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="372"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="345"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="320"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="276"/>
       <source>Dichotic Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="280"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="278"/>
       <source>Add Same</source>
       <translation>Somma uguale</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="278"/>
       <source>Add Original</source>
       <translation>Somma originale</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="395"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="367"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="340"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="317"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="279"/>
       <source>IRN Type:</source>
       <translation>Tipo IRN:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="283"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="281"/>
       <source>NoSpi</source>
       <translation>NoSpi</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="281"/>
       <source>NpiSo</source>
       <translation>NpiSo</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="388"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="369"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="341"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="318"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="282"/>
       <source>Phase relationship:</source>
       <translation>Relazione di fase:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="284"/>
       <source>IPD Linear</source>
       <translation type="unfinished">IPD Lineare</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="286"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="284"/>
       <source>IPD Stepped</source>
       <translation type="unfinished">IPD a scalino</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="284"/>
       <source>ITD</source>
       <translation>ITD</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="396"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="390"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="370"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="342"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="321"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="285"/>
       <source>Dichotic Difference:</source>
       <translation>Differenza dicotica:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="289"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="287"/>
       <source>Harmonic</source>
       <translation>Armonico:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="287"/>
       <source>Harmonic Stretched</source>
       <translation>Armonico allungato</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="392"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="373"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="347"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="325"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="288"/>
       <source>Harmonicity:</source>
       <translation>Armonicità:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="292"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="290"/>
       <source>Hz</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="290"/>
       <source>Cent</source>
       <translation type="unfinished"/>
@@ -1908,14 +2113,18 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="290"/>
       <source>ERB</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="389"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="371"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="346"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="319"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="291"/>
       <source>Bandwidth Unit:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="491"/>
       <source>Carrier Frequency (Hz)</source>
       <translation type="unfinished"/>
@@ -1928,19 +2137,21 @@
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="497"/>
       <source>Modulation Index</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="548"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="500"/>
       <source>Carrier Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="560"/>
+      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="509"/>
       <source>Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="539"/>
       <source>Frequency (Hz)</source>
       <translation>Frequenza (Hz)</translation>
@@ -1957,32 +2168,28 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_generate_sound.py" line="551"/>
       <source>Modulation Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="551"/>
       <source>Harmonic Complex</source>
-      <translation type="obsolete">Complesso Armonico</translation>
+      <translation type="vanished">Complesso Armonico</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="551"/>
       <source>Simple Dichotic</source>
-      <translation type="obsolete">Dicotico semplice</translation>
+      <translation type="vanished">Dicotico semplice</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="551"/>
       <source>Narrowband Noise 2</source>
-      <translation type="obsolete">Rumore a banda stretta 2</translation>
+      <translation type="vanished">Rumore a banda stretta 2</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_generate_sound.py" line="551"/>
       <source>IPD</source>
-      <translation type="obsolete">IPD</translation>
+      <translation type="vanished">IPD</translation>
     </message>
   </context>
   <context>
     <name>preferencesDialog</name>
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="68"/>
       <source>Language (requires restart):</source>
@@ -2041,19 +2248,23 @@
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="178"/>
       <source>Command:</source>
       <translation>Comando:</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="407"/>
+      <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="325"/>
+      <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="186"/>
+      <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="181"/>
       <source>custom</source>
       <translation>personalizzato</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="207"/>
+      <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="193"/>
       <source>Device:</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="224"/>
       <source>Buffer Size (samples):</source>
       <translation type="unfinished"/>
@@ -2086,14 +2297,15 @@
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="279"/>
       <source>Soun&amp;d</source>
       <translation>Suon&amp;o</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="301"/>
+      <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="296"/>
       <source>Warning</source>
       <translation>Avviso</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_edit_preferences.py" line="296"/>
       <source>dpi value not valid</source>
       <translation>valore dpi non valido</translation>
@@ -2171,17 +2383,16 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/dialog_save_sound.py" line="65"/>
       <source>Save Sound Options</source>
       <translation>Opzioni salvataggio del suono</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/dialog_save_sound.py" line="65"/>
       <source>File Encoding:</source>
-      <translation type="obsolete">Codifica file:</translation>
+      <translation type="vanished">Codifica file:</translation>
     </message>
   </context>
   <context>
     <name>spectrogramPlot</name>
     <message>
       <location filename="../pysoundanalyser/win_spectrogram_plot.py" line="126"/>
       <source>Window:</source>
@@ -2209,22 +2420,20 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/win_spectrogram_plot.py" line="155"/>
       <source>Log axis</source>
       <translation type="unfinished">Tempo (s)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrogram_plot.py" line="155"/>
       <source>Frequency (Hz)</source>
-      <translation type="obsolete">Frequenza (Hz)</translation>
+      <translation type="vanished">Frequenza (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrogram_plot.py" line="155"/>
       <source>Grid</source>
-      <translation type="obsolete">Griglia</translation>
+      <translation type="vanished">Griglia</translation>
     </message>
   </context>
   <context>
     <name>spectrumPlot</name>
     <message>
       <location filename="../pysoundanalyser/win_spectrum_plot.py" line="101"/>
       <source>Window:</source>
@@ -2257,57 +2466,48 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>Input Dialog</source>
       <translation>Dialogo di input</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>Exit</source>
-      <translation type="obsolete">Esci</translation>
+      <translation type="vanished">Esci</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>Exit application</source>
-      <translation type="obsolete">Chiudi programma</translation>
+      <translation type="vanished">Chiudi programma</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>&amp;File</source>
-      <translation type="obsolete">&amp;File</translation>
+      <translation type="vanished">&amp;File</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>&amp;Edit</source>
-      <translation type="obsolete">&amp;Modifica</translation>
+      <translation type="vanished">&amp;Modifica</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>Background Color</source>
-      <translation type="obsolete">Colore sfondo</translation>
+      <translation type="vanished">Colore sfondo</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>Canvas Color</source>
-      <translation type="obsolete">Colore canovaccio</translation>
+      <translation type="vanished">Colore canovaccio</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>Frequency (Hz)</source>
-      <translation type="obsolete">Frequenza (Hz)</translation>
+      <translation type="vanished">Frequenza (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>Level (dB)</source>
-      <translation type="obsolete">Livello (dB)</translation>
+      <translation type="vanished">Livello (dB)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_spectrum_plot.py" line="167"/>
       <source>Grid</source>
-      <translation type="obsolete">Griglia</translation>
+      <translation type="vanished">Griglia</translation>
     </message>
   </context>
   <context>
     <name>waveformPlot</name>
     <message>
       <location filename="../pysoundanalyser/win_waveform_plot.py" line="73"/>
       <source>Line Width</source>
@@ -2325,18 +2525,16 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/win_waveform_plot.py" line="106"/>
       <source>Input Dialog</source>
       <translation>Dialogo di input</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_waveform_plot.py" line="106"/>
       <source>Time (s)</source>
-      <translation type="obsolete">Tempo (s)</translation>
+      <translation type="vanished">Tempo (s)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/win_waveform_plot.py" line="106"/>
       <source>Amplitude</source>
-      <translation type="obsolete">Ampiezza</translation>
+      <translation type="vanished">Ampiezza</translation>
     </message>
   </context>
 </TS>
```

### Comparing `pysoundanalyser-0.3.4/prep-release/release.py` & `pysoundanalyser-0.3.7/prep-release/release.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,22 @@
     for opt, arg in opts:
         if opt in ("-m", "--message"):
             message = arg
     major_v = 0
     minor_v = 3
 
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

### Comparing `pysoundanalyser-0.3.4/prep-release/switch_pyqt5.py` & `pysoundanalyser-0.3.7/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/switch_pyqt6.py` & `pysoundanalyser-0.3.7/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/uploadToWebsite.py` & `pysoundanalyser-0.3.7/prep-release/uploadToWebsite.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/win_launch_iss_compiler.sh` & `pysoundanalyser-0.3.7/prep-release/win_launch_iss_compiler.sh`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/prep-release/win_pysoundanalyser.iss` & `pysoundanalyser-0.3.7/prep-release/win_pysoundanalyser.iss`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "pysoundanalyser"
-#define MyAppVersion "0.3.4"
+#define MyAppVersion "0.3.7"
 #define MyAppPublisher "Samuele Carcagno"
 #define MyAppURL "https://samcarcagno.altervista.org/pysoundanalyser/pysoundanalyser.html"
 #define MyAppExeName "pysoundanalyser.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application. Do not use the same AppId value in installers for other applications.
 ; (To generate a new GUID, click Tools | Generate GUID inside the IDE.)
@@ -26,14 +26,15 @@
 ;PrivilegesRequired=lowest
 PrivilegesRequiredOverridesAllowed=dialog
 OutputDir=Z:\media\ntfsShared\lin_home\auditory\code\pysoundanalyser\windows_installer\
 OutputBaseFilename=pysoundanalyser-{#MyAppVersion}_setup
 Compression=lzma
 SolidCompression=yes
 WizardStyle=modern
+SetupIconFile=Z:\media\ntfsShared\lin_home\auditory\code\pysoundanalyser\icons\johnny_automatic_crashing_wave.ico
 
 [Languages]
 Name: "english"; MessagesFile: "compiler:Default.isl"
 Name: "armenian"; MessagesFile: "compiler:Languages\Armenian.isl"
 Name: "brazilianportuguese"; MessagesFile: "compiler:Languages\BrazilianPortuguese.isl"
 Name: "bulgarian"; MessagesFile: "compiler:Languages\Bulgarian.isl"
 Name: "catalan"; MessagesFile: "compiler:Languages\Catalan.isl"
@@ -63,13 +64,13 @@
 Name: "desktopicon"; Description: "{cm:CreateDesktopIcon}"; GroupDescription: "{cm:AdditionalIcons}"; Flags: unchecked
 
 [Files]
 Source: "Z:\media\ntfsShared\lin_home\auditory\code\pysoundanalyser\windows_installer\pysoundanalyser\build\exe.win-amd64-3.11\*"; DestDir: "{app}"; Flags: ignoreversion recursesubdirs createallsubdirs
 ; NOTE: Don't use "Flags: ignoreversion" on any shared system files
 
 [Icons]
-Name: "{autoprograms}\{#MyAppName}"; Filename: "{app}\{#MyAppExeName}"
-Name: "{autodesktop}\{#MyAppName}"; Filename: "{app}\{#MyAppExeName}"; Tasks: desktopicon
+Name: "{autoprograms}\{#MyAppName}"; Filename: "{app}\{#MyAppExeName}"; WorkingDir: "{autodocs}"
+Name: "{autodesktop}\{#MyAppName}"; Filename: "{app}\{#MyAppExeName}"; WorkingDir: "{autodocs}"; Tasks: desktopicon
 
 [Run]
-Filename: "{app}\{#MyAppExeName}"; WorkingDir: "{userdocs}"; Description: "{cm:LaunchProgram,{#StringChange(MyAppName, '&', '&&')}}"; Flags: nowait postinstall skipifsilent
+Filename: "{app}\{#MyAppExeName}"; WorkingDir: "{autodocs}"; Description: "{cm:LaunchProgram,{#StringChange(MyAppName, '&', '&&')}}"; Flags: nowait postinstall skipifsilent
```

### Comparing `pysoundanalyser-0.3.4/prep-release/winbuild.py` & `pysoundanalyser-0.3.7/prep-release/winbuild.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pyproject.toml` & `pysoundanalyser-0.3.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysoundanalyser"
-    version="0.3.4"
+    version="0.3.7"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Python program for visualizing short sounds (waveform, spectrum, etc...)"
 license = {file = "COPYING.txt"}
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["matplotlib (>=3.0.0)",
                 "numpy (>=1.0.0)",
 		"pandas (>=1.0.0)",
 		"PyAudio (>=0.2.11)",
-		"PyQt5 (>=5.12)",
+		"PyQt6 (>=6.6.0)",
 		"scipy (>=1.0.1)"
 		]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/__main__.py` & `pysoundanalyser-0.3.7/pysoundanalyser/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 
@@ -12,15 +12,15 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
 #    You should have received a copy of the GNU General Public License
 #    along with pysoundanalyser.  If not, see <http://www.gnu.org/licenses/>.
 
-import argparse, sys, platform, os, copy, logging, pickle, signal, scipy, time, traceback
+import argparse, sys, platform, os, copy, logging, pickle, platform, signal, scipy, time, traceback
 from pysoundanalyser.pyqtver import*
 if pyqtversion == 5:
     from PyQt5 import QtGui, QtCore
     from PyQt5.QtGui import QIcon
     from PyQt5.QtWidgets import QAbstractItemView, QAction, QApplication, QDialog, QDialogButtonBox, QGridLayout, QFileDialog, QInputDialog, QLabel, QMainWindow, QMessageBox, QPushButton, QScrollArea, QTableWidget, QTableWidgetItem, QVBoxLayout, QWidget
 elif pyqtversion == 6:
     from PyQt6 import QtGui, QtCore
@@ -311,16 +311,14 @@
         #MOVE DOWN BUTTON
         moveDownButton = QPushButton(self.tr("Move Down"), self)
         moveDownButton.clicked.connect(self.onClickMoveDownButton)
         #MOVE UP BUTTON
         moveUpButton = QPushButton(self.tr("Move Up"), self)
         moveUpButton.clicked.connect(self.onClickMoveUpButton)
 
-
-
         self.sndTableWidget = QTableWidget()
         #self.sndTableWidget.setSortingEnabled(True)
         self.sndTableWidget.setColumnCount(3)
         self.sndTableWidget.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
         self.sndTableWidget.setSelectionMode(QAbstractItemView.SelectionMode.ExtendedSelection)
         
         self.sndTableWidget.setHorizontalHeaderLabels([self.tr('Label'), self.tr('Channel'), 'id'])
@@ -343,15 +341,14 @@
         vbl.addWidget(levelDiffButton)
         vbl.addWidget(scaleButton)
         vbl.addWidget(resampleButton)
         vbl.addWidget(renameButton)
         vbl.addWidget(removeButton)
         vbl.addWidget(removeAllButton)
         
-        
         vbl.addStretch(1)
 
         vbl3 = QVBoxLayout()
         vbl3.addWidget(moveUpButton)
         vbl3.addWidget(moveDownButton)
         self.infoPane = QLabel(self.tr('No Selection                                           '))
         vbl3.addWidget(self.infoPane)
@@ -410,27 +407,27 @@
             pass
         else:
             row = rows[0]
             if row == lastRow:
                 pass
             else:
                 self.swapRow(row, row+1)
+                
     def onClickMoveUpButton(self):
         rows = self.findSelectedItemRows()
         if len(rows) > 1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('Only one sound can be moved at a time'))
         elif len(rows) < 1:
             pass
         else:
             row = rows[0]
             if row == 0:
                 pass
             else:
-                self.swapRow(row, row-1)
-        
+                self.swapRow(row, row-1)        
         
     def onClickLoadButton(self):
         #self.sndTableWidget.setSortingEnabled(False)
         files = QFileDialog.getOpenFileNames(self, self.tr("pysoundanalyser - Choose file to load"), '',self.tr("Supported Sound Files (*.wav);;All Files (*)"))[0]
         self.loadFiles(files)
         
     def loadFiles(self, files):
@@ -511,14 +508,15 @@
 
        
                 
             else:
                 pass
         selItems = self.sndTableWidget.selectedItems()
         #self.sndTableWidget.setSortingEnabled(True)
+        
     def loadFileValid(self, sndFile):
         #xxxxxxxxxxxxxxx
         # need to update this function
         if len(sndFile) == 0:
             fileValid = False
             msg = None
         else:
@@ -532,14 +530,15 @@
         #else:
         #    fileValid = False
         #    msg = 'cannot open' + sndFile + ' only wav supported at the moment'
         if fileValid == False and msg != None:
             QMessageBox.warning(self, self.tr('Warning'), msg)
 
         return fileValid
+    
     def loadWav(self,fName):
         snd, fs, nbits = wavread(fName)
 
         return snd, fs, nbits
     
     def onSelectionChanged(self):
         ids = self.findSelectedItemIds()
@@ -578,21 +577,23 @@
         for i in range(len(selItems)):
             selItemsRows.append(selItems[i].row())
         selItemsRows = unique(selItemsRows)
         selItemsIds = []
         for i in range(len(selItemsRows)):
             selItemsIds.append(str(self.sndTableWidget.item(selItemsRows[i], 2).text()))
         return selItemsIds
+    
     def findSelectedItemRows(self):
         selItems = self.sndTableWidget.selectedItems()
         selItemsRows = []
         for i in range(len(selItems)):
             selItemsRows.append(selItems[i].row())
         selItemsRows = unique(selItemsRows)
         return selItemsRows
+    
     def onCellDoubleClicked(self, row, col):
         if col == 0:
             self.onClickRenameButton()
         elif col == 1:
             self.onDoubleClickChannelCell()
 
     def onClickSaveButton(self):
@@ -616,30 +617,28 @@
             for i in range(len(ids)):
                 selectedSound = ids[i]
                 nSampDiff = max(nSampList) - len(self.sndList[selectedSound]['wave'])
                 if self.sndList[selectedSound]['chan'] == self.tr('Right'):
                     snd[:,1] =  snd[:,1] + concatenate((self.sndList[selectedSound]['wave'], zeros(nSampDiff)), axis=0)
                 elif self.sndList[selectedSound]['chan'] == self.tr('Left'):
                     snd[:,0] =  snd[:,0] + concatenate((self.sndList[selectedSound]['wave'], zeros(nSampDiff)), axis=0)
-
        
         dialog = saveSoundDialog(self)
         if dialog.exec():
             fs = sampRate
             if dialog.channelChooser.currentText() == self.tr('Mono'):
                 wave = snd[:,0] + snd[:,1]
                 nChannels = 1
             else:
                 wave = snd
                 nChannels = 2
             ftow = QFileDialog.getSaveFileName(self, self.tr('Choose file to write'), self.tr('.{0}').format(dialog.suggestedExtension), self.tr('All Files (*)'))[0]
             if len(ftow) > 0:
 
                 wavwrite(wave, fs, int(dialog.encodingChooser.currentText()), ftow)              
-
     
     def onClickCloneButton(self):
         #self.sndTableWidget.setSortingEnabled(False)
         ids = self.findSelectedItemIds()
         if len(ids)<1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
             return
@@ -662,55 +661,61 @@
             self.sndTableWidget.setItem(currCount-1, 0, newItem)
             newItem = QTableWidgetItem(thisSnd['chan'])
             #newItem.setFlags(QtCore.Qt.ItemFlag.ItemIsSelectable | QtCore.Qt.ItemFlag.ItemIsEnabled)
             self.sndTableWidget.setItem(currCount-1, 1, newItem)
             self.sndList[tmp_id]['qid'] = QTableWidgetItem(tmp_id)
             self.sndTableWidget.setItem(currCount-1, 2, self.sndList[tmp_id]['qid'])
             #self.sndTableWidget.setSortingEnabled(True)
+            
     def onClickPlotButton(self):
         ids = self.findSelectedItemIds()
         if len(ids)<1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
             return
         for i in range(len(ids)):
            selectedSound = ids[i]
            waveformPlot(self, self.sndList[selectedSound], self.prm)
            #self.waveformPlotter.plotWaveformThreaded(self.sndList[selectedSound], self.prm)
+           
     def onClickSpectrumButton(self):
        ids = self.findSelectedItemIds()
        if len(ids)<1:
            QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
            return
        for i in range(len(ids)):
            selectedSound = ids[i]
            spectrumPlot(self, self.sndList[selectedSound], self.prm)
+           
     def onClickAutocorrelationButton(self):
        ids = self.findSelectedItemIds()
        if len(ids)<1:
            QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
            return
        for i in range(len(ids)):
            selectedSound = ids[i]
            acfPlot(self, self.sndList[selectedSound], self.prm)
+           
     def onClickAutocorrelogramButton(self):
        ids = self.findSelectedItemIds()
        if len(ids)<1:
            QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
            return
        for i in range(len(ids)):
            selectedSound = ids[i]
            autocorrelogramPlot(self, self.sndList[selectedSound], self.prm)
+           
     def onClickSpectrogramButton(self):
        ids = self.findSelectedItemIds()
        if len(ids)<1:
            QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
            return
        for i in range(len(ids)):
            selectedSound = ids[i]
            spectrogramPlot(self, self.sndList[selectedSound], self.prm)
+           
     def onClickRenameButton(self):
         ids = self.findSelectedItemIds()
         if len(ids) > 1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('Only one sound can be renamed at a time'))
         elif len(ids) < 1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
             return
@@ -731,15 +736,14 @@
             multipleSelection = False
             currChan = self.sndList[selectedSound]['chan']
             dialog = changeChannelDialog(self, multipleSelection, currChan)
             if dialog.exec():
                 newChan = dialog.chooser.currentText()
                 self.sndTableWidget.item(self.sndList[selectedSound]['qid'].row(), 1).setText(newChan)
                 self.sndList[selectedSound]['chan'] = newChan
-
           
     def onClickLevelDiffButton(self):
         ids = self.findSelectedItemIds()
         if len(ids)<2:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
             return
         if len(ids) > 2:
@@ -753,28 +757,25 @@
             if dbDiff >= 0:
                 w = '+'
             elif dbDiff < 0:
                 w = ''
 
             QMessageBox.information(self, self.tr('Level Difference'), self.tr('{0} is {1} {2} dB than {3}').format(snd1['label'], w, self.currLocale.toString(dbDiff), snd2['label']))
 
-
     def onClickScaleButton(self):
         ids = self.findSelectedItemIds()
         if len(ids)<1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
             return
         val, ok = QInputDialog.getDouble(self, self.tr('Scale Level'), self.tr('Add or subtract decibels'))
         if ok:
             for i in range(len(ids)):
                 selectedSound = ids[i]
                 self.sndList[selectedSound]['wave'] = sndlib.scale(val, self.sndList[selectedSound]['wave'])
        
-
-
     def onClickRemoveButton(self):
         ids = self.findSelectedItemIds()
         if len(ids)<1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
             return
         for i in range(len(ids)):
             selectedSound = ids[i]
@@ -796,17 +797,15 @@
         rmsVals = []
         msg = self.tr('')
         for i in range(len(ids)):
             selectedSound = ids[i]
             rmsVals.append(sndlib.getRMS(self.sndList[selectedSound]['wave'], channel=0))
             msg = self.tr('{0} {1} : {2} \n').format(msg, self.sndList[selectedSound]['label'], self.currLocale.toString(rmsVals[i])) 
         QMessageBox.information(self, self.tr('Root Mean Square'), msg)
-      
-        
-       
+                     
     def onClickPlayButton(self):
         ids = self.findSelectedItemIds()
         if len(ids)<1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
             return
         sampRate = self.sndList[ids[0]]['fs']
         condition = True
@@ -936,15 +935,14 @@
                      self.sndTableWidget.setItem(currCount-1, 0, newItem)
                      newItem = QTableWidgetItem(thisSnd['chan'])
                      
                      self.sndTableWidget.setItem(currCount-1, 1, newItem)
                      self.sndList[tmp_id]['qid'] = QTableWidgetItem(tmp_id)
                      self.sndTableWidget.setItem(currCount-1, 2, self.sndList[tmp_id]['qid'])
                      
-
     def onClickCutButton(self):
         ids = self.findSelectedItemIds()
         if len(ids)<1:
             QMessageBox.warning(self, self.tr('Warning'), self.tr('No sound selected.'))
             return
         for i in range(len(ids)):
             snd = self.sndList[ids[i]]
@@ -1356,15 +1354,14 @@
                 channel = 'Left'
             elif channel == self.tr('Both'):
                 channel = 'Both'
             
             thisSound = sndlib.FMTone(fc=carrFreq, fm=modFreq, mi=modInd, phase=carrPhase, level=level, duration=duration, ramp=ramp, channel=channel, fs=fs, maxLevel=self.prm['pref']['sound']['maxLevel'])
             self.setupNewSound(sndData=thisSound, label=label, channel=channel, fs=fs)
 
-
     def onClickGenerateSilence(self):
         dialog = generateSoundDialog(self, "Silence")
         if dialog.exec():
 
             for i in range(dialog.sndPrm['nFields']):
                 dialog.sndPrm['field'][i] = self.currLocale.toDouble(dialog.field[i].text())[0]
             for i in range(dialog.sndPrm['nChoosers']):
@@ -1379,15 +1376,14 @@
             elif channel == self.tr('Left'):
                 channel = 'Left'
             elif channel == self.tr('Both'):
                 channel = 'Both'
             
             thisSound = sndlib.makeSilence(duration=duration, fs=fs)
             self.setupNewSound(sndData=thisSound, label=label, channel=channel, fs=fs)
-
            
     def setupNewSound(self, sndData, label, channel, fs):
         if channel in ['Right', 'Left']:
                 thisSnd = {}
                 if channel == 'Right':
                     thisSnd['wave'] = sndData[:,1]
                 elif channel == 'Left':
@@ -1462,15 +1458,14 @@
             l = []
             for url in event.mimeData().urls():
                 l.append(str(url.toLocalFile()))
             self.loadFiles(l)
         else:
             event.ignore()
 
-
     def onAbout(self):
         if pyqtversion in [4,5,6]:
             qt_compiled_ver = QtCore.QT_VERSION_STR
             qt_runtime_ver = QtCore.qVersion()
             qt_pybackend_ver = QtCore.PYQT_VERSION_STR
             qt_pybackend = "PyQt"
         elif pyqtversion == -4:
@@ -1517,15 +1512,14 @@
             l = []
             for url in event.mimeData().urls():
                 l.append(str(url.toLocalFile()))
                 self.drpd.emit(l[len(l)-1])
         else:
             event.ignore()
 
-
 def main():
     
     prm = {}
     prm['appData'] = {}
     #prm['appData'] = {}; prm['prefs'] = {}
     # create the GUI application
     qApp = QApplication(sys.argv)
@@ -1574,14 +1568,16 @@
     qApp.setWindowIcon(QIcon(":/johnny_automatic_crashing_wave.svg"))
     ## Look and feel changed to CleanLooks
     #QApplication.setStyle(QStyleFactory.create("QtCurve"))
     #QApplication.setPalette(QApplication.style().standardPalette())
     #qApp.currentLocale = locale
     # instantiate the ApplicationWindow widget
     qApp.setApplicationName('pysoundanalyser')
+    if platform.system() == "Windows":
+        qApp.setStyle('Fusion')
     aw = applicationWindow(prm)
 
 
     # show the widget
     aw.show()
     # start the Qt main loop execution, exiting from this script
     # with the same return code of Qt application
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/audio_manager.py` & `pysoundanalyser-0.3.7/pysoundanalyser/audio_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_apply_filter.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_apply_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_change_channel.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_change_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_concatenate.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_concatenate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_cut.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_cut.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_edit_preferences.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_edit_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_noise.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_generate_noise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_sinusoid.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_generate_sinusoid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_sound.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_generate_sound.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_get_font.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_get_font.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 
@@ -15,19 +15,19 @@
 #    You should have received a copy of the GNU General Public License
 #    along with pysoundanalyser. If not, see <http://www.gnu.org/licenses/>.
 
 import matplotlib
 from .pyqtver import*
 if pyqtversion == 5:
     from PyQt5 import QtGui, QtCore
-    from PyQt5.QtWidgets import QDialog, QDialogButtonBox, QGridLayout, QLabel, QListWidget
+    from PyQt5.QtWidgets import QDialog, QDialogButtonBox, QGridLayout, QLabel, QListWidget, QPushButton
     matplotlib.rcParams['backend'] = "Qt5Agg"
 elif pyqtversion == 6:
     from PyQt6 import QtGui, QtCore
-    from PyQt6.QtWidgets import QDialog, QDialogButtonBox, QGridLayout, QLabel, QListWidget
+    from PyQt6.QtWidgets import QDialog, QDialogButtonBox, QGridLayout, QLabel, QListWidget, QPushButton
     matplotlib.rcParams['backend'] = "Qt5Agg"
 import matplotlib.font_manager as fm
 from numpy import unique
 
 import os, pickle
  
 class getFontDialog(QDialog):
@@ -51,95 +51,131 @@
             
         self.fontsCacheFile = os.path.expanduser("~") +'/.config/pysoundanalyser/fontsCache'
         if os.path.exists(self.fontsCacheFile):
             fIn = open(self.fontsCacheFile, 'rb')
             self.fontsDic = pickle.load(fIn)
             fIn.close()
         else:
-        
-            x = fm.FontManager()
-            weight_lookup = {
-                '100': 'ultralight',
-                '200': 'light',
-                '400': 'normal',    
-                '500': 'medium',     
-                '600': 'demibold',   
-                '700': 'bold',       
-                '800': 'extra bold', 
-                '900': 'black'}
-
-            fontList = x.ttflist
-            fontNamesAll = []
-            for i in range(len(x.ttflist)):
-                fontNamesAll.append(x.ttflist[i].name)
-            fontNames = unique(fontNamesAll)
-
-            self.fontsDic = {}
-            for i in range(len(fontNames)):
-                self.fontsDic[fontNames[i]] = {}
-                self.fontsDic[fontNames[i]]['style'] = []
-                self.fontsDic[fontNames[i]]['styleAbb'] = []
-
-            for font in fontList:
-                style = font.style
-                weight = font.weight
-                self.fontsDic[font.name]['style'].append(style + ':' + str(weight) + ':' + font.fname)
-                weightName = weight_lookup[str(weight)]
-                styleName = style + ' ' + weightName
-                self.fontsDic[font.name]['styleAbb'].append(styleName)
-
-            f = open(self.fontsCacheFile, 'wb')
-            pickle.dump(self.fontsDic, f)
-            f.close()
-        #---------------------
+            self.refreshFontsCache()
         
         self.currLocale = self.parent().prm['appData']['currentLocale']
         self.currLocale.setNumberOptions(self.currLocale.NumberOption.OmitGroupSeparator | self.currLocale.NumberOption.RejectGroupSeparator)
         grid = QGridLayout()
       
         fontNameLabel = QLabel(self.tr('Font Name'))
         grid.addWidget(fontNameLabel, 0, 0)
-
         
         fontStyleLabel = QLabel(self.tr('Font Style'))
         grid.addWidget(fontStyleLabel, 0, 1)
-
         
         fontSizeLabel = QLabel(self.tr('Font Size'))
         grid.addWidget(fontSizeLabel, 0, 2)
         ind = sorted(self.fontsDic.keys()).index(self.currFontFamily)
         self.fontListWidget = QListWidget(self)
         self.fontListWidget.insertItems(0, sorted(self.fontsDic.keys()))
         self.fontListWidget.setCurrentRow(ind)
         self.fontListWidget.itemClicked.connect(self.onChangeFontName)
         grid.addWidget(self.fontListWidget, 1, 0)
 
         self.fontStylesWidget = QListWidget(self)
         self.fontStylesWidget.insertItems(0, self.fontsDic[sorted(self.fontsDic.keys())[ind]]['styleAbb'])
-      
         indStyle = self.fontsDic[sorted(self.fontsDic.keys())[ind]]['styleAbb'].index(self.currFontStyle + ' ' + self.currFontWeight)
         self.fontStylesWidget.setCurrentRow(indStyle)
         grid.addWidget(self.fontStylesWidget, 1, 1)
 
         self.fontSizeWidget = QListWidget(self)
         self.pointSizeList = ['4', '5', '6', '7', '8', '9', '10', '11', '12', '13', '14', '15', '16', '17', '18', '19', '20', '22', '24', '26', '28', '32', '48', '64', '72', '80', '96', '128']
         self.fontSizeWidget.insertItems(0, self.pointSizeList)
         self.fontSizeWidget.setCurrentRow(self.pointSizeList.index(str(int(self.currFontSize))))
         grid.addWidget(self.fontSizeWidget, 1, 2)
        
-
-            
-        
         buttonBox = QDialogButtonBox(QDialogButtonBox.StandardButton.Ok|
                                      QDialogButtonBox.StandardButton.Cancel)
         buttonBox.accepted.connect(self.accept)
         buttonBox.rejected.connect(self.reject)
        
         grid.addWidget(buttonBox, 3, 2)
+
+        refreshFontsCacheButton = QPushButton(self.tr("Refresh fonts cache"), self)
+        refreshFontsCacheButton.clicked.connect(self.onClickRefreshFontsCacheButton)
+        grid.addWidget(refreshFontsCacheButton, 3, 0)
+        
         self.setLayout(grid)
         self.setWindowTitle(self.tr("Choose Font"))
 
     def onChangeFontName(self):
         currFontName = str(self.fontListWidget.currentItem().text())
         self.fontStylesWidget.clear()
         self.fontStylesWidget.insertItems(0, self.fontsDic[currFontName]['styleAbb'])
         self.fontStylesWidget.setCurrentRow(0)
+
+    def onClickRefreshFontsCacheButton(self):
+        #ind = sorted(self.fontsDic.keys()).index(self.currFontFamily)
+        #indStyle = self.fontsDic[sorted(self.fontsDic.keys())[ind]]['styleAbb'].index(self.currFontStyle + ' ' + self.currFontWeight)
+        ind = self.fontListWidget.currentRow() #sorted(self.fontsDic.keys()).index(self.currFontFamily)
+        indStyle = self.fontStylesWidget.currentRow() #self.fontsDic[sorted(self.fontsDic.keys())[ind]]['styleAbb'].index(self.currFontStyle + ' ' + self.currFontWeight)
+        self.refreshFontsCache()
+        self.fontListWidget.clear()
+        self.fontStylesWidget.clear()
+        self.fontListWidget.insertItems(0, sorted(self.fontsDic.keys()))
+        self.fontListWidget.setCurrentRow(ind)
+        self.fontStylesWidget.insertItems(0, self.fontsDic[sorted(self.fontsDic.keys())[ind]]['styleAbb'])
+        self.fontStylesWidget.setCurrentRow(indStyle)
+        
+    def refreshFontsCache(self):
+        x = fm.FontManager()
+        weight_lookup = {
+            '100': 'ultralight',
+            '200': 'light',
+            '400': 'normal',    
+            '500': 'medium',     
+            '600': 'demibold',   
+            '700': 'bold',       
+            '800': 'extra bold', 
+            '900': 'black'}
+
+        fontList = x.ttflist
+        fontNamesAll = []
+        for i in range(len(x.ttflist)):
+            fontNamesAll.append(x.ttflist[i].name)
+        fontNames = unique(fontNamesAll)
+
+        self.fontsDic = {}
+        for i in range(len(fontNames)):
+            self.fontsDic[fontNames[i]] = {}
+            self.fontsDic[fontNames[i]]['style'] = []
+            self.fontsDic[fontNames[i]]['styleAbb'] = []
+
+        for font in fontList:
+            style = font.style
+            weight = font.weight
+            self.fontsDic[font.name]['style'].append(style + ':' + str(weight) + ':' + font.fname)
+            try:
+                weightName = weight_lookup[str(weight)]
+            except:
+                if weight <= 100:
+                    weightName = 'ultralight'
+                elif weight <= 200:
+                    weightName = 'light'
+                elif weight <= 400:
+                    weightName = 'normal'
+                elif weight <= 500:
+                    weightName = 'medium'
+                elif weight <= 600:
+                    weightName = 'demibold'
+                elif weight <= 700:
+                    weightName = 'bold'
+                elif weight <= 800:
+                    weightName = 'extra bold'
+                elif weight <= 900:
+                    weightName = 'black'
+                    # print(font.name)
+                    # print(weightName)
+                    # print(weight)
+
+            styleName = style + ' ' + weightName #+ ' (weight' + str(weight) + ')'
+            self.fontsDic[font.name]['styleAbb'].append(styleName)
+
+        f = open(self.fontsCacheFile, 'wb')
+        pickle.dump(self.fontsDic, f)
+        f.close()
+        #---------------------
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_resample.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_resample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/dialog_save_sound.py` & `pysoundanalyser-0.3.7/pysoundanalyser/dialog_save_sound.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/Makefile` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ::
    
    pysoundanalyser
 
 Note that the program needs to be launched in the same Python environment in which it has been installed. The program has been tested on Linux and Windows. It should work also on Mac computers but this has not been tested. Depending on your Python distribution you may want to install the python modules pysoundanalyser depends on before installing pysoundanalyser (e.g. via the conda package manager if you're using the Anaconda Python distribution). The dependencies are:
 
-- PyQt5 
+- PyQt6 
 - numpy 
 - scipy 
 - pandas 
 - matplotlib 
 - PyAudio 
 
 if you're using Linux you can also install `pyalsaaudio` to have an addition sound output option. If you're using conda on Windows I'd recommend installing PyAudio via pip because the PyAudio version available on conda is not built with support for the WASAPI output interface (at least that was the case the last time I checked).
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 .. _sec-user_interface:
 
 ****************
 User Interface
 ****************
 
-- **Load Sound** The ``Load Sound`` button allows you to load a wav file into the program. Currently only 16 and 32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is fine and fast for wav files of short durations (tens of seconds), but longer sound files are going to consume huge amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other software, like audacity.  
+- **Load Sound** The ``Load Sound`` button allows you to load a wav file into the program. Currently only 16, 24, and 32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is fine and fast for wav files of short duration (tens of seconds), but longer sound files are going to consume huge amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other software, like audacity.  
 
-  - **Save As** The ``Save As`` button allows you to save PSA sound objects as wav files. Currently it is only possible to save sounds as 16 or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format, and multiple PSA sound objects have been selected for saving, they will be summed together before saving. If you choose a stereo (2-channels) format, "right" and "left" PSA sound objects will be saved to their respective channels in the wav file; if multiple "right" or "left" PSA sound objects have been selected, they will be summed before saving.
+  - **Save As** The ``Save As`` button allows you to save PSA sound objects as wav files. Currently it is only possible to save sounds as 16, 24, or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format, and multiple PSA sound objects have been selected for saving, they will be summed together before saving. If you choose a stereo (2-channels) format, "right" and "left" PSA sound objects will be saved to their respective channels in the wav file; if multiple "right" or "left" PSA sound objects have been selected, they will be summed before saving.
 
 - **Clone Sound**
       
 - **Concatenate**
   
 - **Cut** The ``Cut`` button allows you to remove segments of a sound waveform. The starting and ending points of the segments to be cut off can be specified in seconds, milliseconds, or sample numbers. When working with sample numbers, note that PSA indexing works exactly like numpy indexing. Examples:
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alabaster.css` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alert_info_32.png` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/alert_info_32.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/basic.css` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bizstyle.css` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bizstyle.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/badge_only.css` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/theme.css` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/doctools.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/haiku.css` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/haiku.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/jquery.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/js/theme.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/language_data.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/pygments.css` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/searchtools.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/underscore.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/genindex.html` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; pysoundanalyser 0.3.4 documentation</title>
+  <title>Index &mdash; pysoundanalyser 0.3.7 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/index.html` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to pysoundanalyser’s documentation! &mdash; pysoundanalyser 0.3.4 documentation</title>
+  <title>Welcome to pysoundanalyser’s documentation! &mdash; pysoundanalyser 0.3.7 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/installation.html` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/installation.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; pysoundanalyser 0.3.4 documentation</title>
+  <title>Installation &mdash; pysoundanalyser 0.3.7 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -79,15 +79,15 @@
 </div>
 <p>once pysoundanalyser is installed you can launch it from a bash/DOS terminal with the command</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pysoundanalyser</span>
 </pre></div>
 </div>
 <p>Note that the program needs to be launched in the same Python environment in which it has been installed. The program has been tested on Linux and Windows. It should work also on Mac computers but this has not been tested. Depending on your Python distribution you may want to install the python modules pysoundanalyser depends on before installing pysoundanalyser (e.g. via the conda package manager if you’re using the Anaconda Python distribution). The dependencies are:</p>
 <ul class="simple">
-<li><p>PyQt5</p></li>
+<li><p>PyQt6</p></li>
 <li><p>numpy</p></li>
 <li><p>scipy</p></li>
 <li><p>pandas</p></li>
 <li><p>matplotlib</p></li>
 <li><p>PyAudio</p></li>
 </ul>
 <p>if you’re using Linux you can also install <cite>pyalsaaudio</cite> to have an addition sound output option. If you’re using conda on Windows I’d recommend installing PyAudio via pip because the PyAudio version available on conda is not built with support for the WASAPI output interface (at least that was the case the last time I checked).</p>
```

#### html2text {}

```diff
@@ -19,15 +19,15 @@
 Note that the program needs to be launched in the same Python environment in
 which it has been installed. The program has been tested on Linux and Windows.
 It should work also on Mac computers but this has not been tested. Depending on
 your Python distribution you may want to install the python modules
 pysoundanalyser depends on before installing pysoundanalyser (e.g. via the
 conda package manager if you’re using the Anaconda Python distribution). The
 dependencies are:
-    * PyQt5
+    * PyQt6
     * numpy
     * scipy
     * pandas
     * matplotlib
     * PyAudio
 if you’re using Linux you can also installpyalsaaudioto have an addition sound
 output option. If you’re using conda on Windows I’d recommend installing
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/intro.html` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/intro.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>What is pysoundanalyser? &mdash; pysoundanalyser 0.3.4 documentation</title>
+  <title>What is pysoundanalyser? &mdash; pysoundanalyser 0.3.7 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/search.html` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; pysoundanalyser 0.3.4 documentation</title>
+  <title>Search &mdash; pysoundanalyser 0.3.7 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/searchindex.js` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -58,15 +58,15 @@
         "conda": 1,
         "packag": 1,
         "manag": 1,
         "re": 1,
         "us": [1, 2, 3],
         "anaconda": 1,
         "ar": [1, 3],
-        "pyqt5": 1,
+        "pyqt5": [],
         "numpi": [1, 3],
         "scipi": 1,
         "panda": 1,
         "matplotlib": 1,
         "pyaudio": 1,
         "pyalsaaudio": 1,
         "have": [1, 3],
@@ -226,15 +226,17 @@
         "show": 3,
         "between": 3,
         "scale": 3,
         "chang": 3,
         "resampl": 3,
         "renam": 3,
         "workspac": 3,
-        "all": 3
+        "all": 3,
+        "pyqt6": 1,
+        "24": 3
     },
     "objects": {},
     "objtypes": {},
     "objnames": {},
     "titleterms": {
         "welcom": 0,
         "pysoundanalys": [0, 2],
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/user_interface.html` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/html/user_interface.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>User Interface &mdash; pysoundanalyser 0.3.4 documentation</title>
+  <title>User Interface &mdash; pysoundanalyser 0.3.7 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -69,17 +69,17 @@
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="user-interface">
 <span id="sec-user-interface"></span><h1>User Interface<a class="headerlink" href="#user-interface" title="Permalink to this heading"></a></h1>
 <ul>
-<li><p><strong>Load Sound</strong> The <code class="docutils literal notranslate"><span class="pre">Load</span> <span class="pre">Sound</span></code> button allows you to load a wav file into the program. Currently only 16 and 32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is fine and fast for wav files of short durations (tens of seconds), but longer sound files are going to consume huge amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other software, like audacity.</p>
+<li><p><strong>Load Sound</strong> The <code class="docutils literal notranslate"><span class="pre">Load</span> <span class="pre">Sound</span></code> button allows you to load a wav file into the program. Currently only 16, 24, and 32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is fine and fast for wav files of short duration (tens of seconds), but longer sound files are going to consume huge amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other software, like audacity.</p>
 <ul class="simple">
-<li><p><strong>Save As</strong> The <code class="docutils literal notranslate"><span class="pre">Save</span> <span class="pre">As</span></code> button allows you to save PSA sound objects as wav files. Currently it is only possible to save sounds as 16 or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format, and multiple PSA sound objects have been selected for saving, they will be summed together before saving. If you choose a stereo (2-channels) format, “right” and “left” PSA sound objects will be saved to their respective channels in the wav file; if multiple “right” or “left” PSA sound objects have been selected, they will be summed before saving.</p></li>
+<li><p><strong>Save As</strong> The <code class="docutils literal notranslate"><span class="pre">Save</span> <span class="pre">As</span></code> button allows you to save PSA sound objects as wav files. Currently it is only possible to save sounds as 16, 24, or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format, and multiple PSA sound objects have been selected for saving, they will be summed together before saving. If you choose a stereo (2-channels) format, “right” and “left” PSA sound objects will be saved to their respective channels in the wav file; if multiple “right” or “left” PSA sound objects have been selected, they will be summed before saving.</p></li>
 </ul>
 </li>
 <li><p><strong>Clone Sound</strong></p></li>
 <li><p><strong>Concatenate</strong></p></li>
 <li><p><strong>Cut</strong> The <code class="docutils literal notranslate"><span class="pre">Cut</span></code> button allows you to remove segments of a sound waveform. The starting and ending points of the segments to be cut off can be specified in seconds, milliseconds, or sample numbers. When working with sample numbers, note that PSA indexing works exactly like numpy indexing. Examples:</p>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span> <span class="c1">#import numpy</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">sig</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span> <span class="c1">#generate a 10-elements array</span>
```

#### html2text {}

```diff
@@ -6,29 +6,29 @@
     * _U_s_e_r_ _I_n_t_e_r_f_a_c_e
 _p_y_s_o_u_n_d_a_n_a_l_y_s_e_r
     * User Interface
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ UUsseerr IInntteerrffaaccee_? ************
     * LLooaadd SSoouunndd The Load Sound button allows you to load a wav file into the
-      program. Currently only 16 and 32 bit wav files with one or two channels
-      are supported. Note that the entire wav file is loaded in memory, this is
-      fine and fast for wav files of short durations (tens of seconds), but
-      longer sound files are going to consume huge amounts of RAM and may even
-      halt your computer. If you need to work on long sound files, please use
-      other software, like audacity.
+      program. Currently only 16, 24, and 32 bit wav files with one or two
+      channels are supported. Note that the entire wav file is loaded in
+      memory, this is fine and fast for wav files of short duration (tens of
+      seconds), but longer sound files are going to consume huge amounts of RAM
+      and may even halt your computer. If you need to work on long sound files,
+      please use other software, like audacity.
           o SSaavvee AAss The Save As button allows you to save PSA sound objects as
-            wav files. Currently it is only possible to save sounds as 16 or 32
-            bit wav files with one or two channels. If you choose a mono (1-
-            channel) format, and multiple PSA sound objects have been selected
-            for saving, they will be summed together before saving. If you
-            choose a stereo (2-channels) format, “right” and “left” PSA sound
-            objects will be saved to their respective channels in the wav file;
-            if multiple “right” or “left” PSA sound objects have been selected,
-            they will be summed before saving.
+            wav files. Currently it is only possible to save sounds as 16, 24,
+            or 32 bit wav files with one or two channels. If you choose a mono
+            (1-channel) format, and multiple PSA sound objects have been
+            selected for saving, they will be summed together before saving. If
+            you choose a stereo (2-channels) format, “right” and “left” PSA
+            sound objects will be saved to their respective channels in the wav
+            file; if multiple “right” or “left” PSA sound objects have been
+            selected, they will be summed before saving.
     * CClloonnee SSoouunndd
     * CCoonnccaatteennaattee
     * CCuutt The Cut button allows you to remove segments of a sound waveform. The
       starting and ending points of the segments to be cut off can be specified
       in seconds, milliseconds, or sample numbers. When working with sample
       numbers, note that PSA indexing works exactly like numpy indexing.
       Examples:
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf`

 * *Files 24% similar despite different names*

#### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: 'Samuele Carcagno'
-CreationDate: "D:20230609115005+02'00'"
+CreationDate: "D:20240502223213+02'00'"
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: "D:20230609115005+02'00'"
+ModDate: "D:20240502223213+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.24 (TeX Live 2022/Debian) kpathsea version 6.3.4'
 Producer: 'pdfTeX-1.40.24'
 Subject: ''
 Title: 'pysoundanalyser'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 pysoundanalyser
-Release 0.3.4
+Release 0.3.7
 
 Samuele Carcagno
 
-Jun 09, 2023
+May 02, 2024
 
 CONTENTS:
 
 1
 
 What is pysoundanalyser?
 
@@ -46,15 +46,15 @@
 sounds generated for psychoacoustics research. pysoundanalyser can also generate some types of sounds used in
 psychoacoustics research (e.g. pure tones, amplitude modulated tones, frequency modulated tones, different colors of
 noise, etc. . . ).
 The repository of pysoundanalyser is hosted on GitHub. If you find bugs, please report them there.
 
 1
 
-pysoundanalyser, Release 0.3.4
+pysoundanalyser, Release 0.3.7
 
 2
 
 Chapter 1. What is pysoundanalyser?
 
 CHAPTER
 
@@ -68,49 +68,49 @@
 once pysoundanalyser is installed you can launch it from a bash/DOS terminal with the command
 pysoundanalyser
 Note that the program needs to be launched in the same Python environment in which it has been installed. The
 program has been tested on Linux and Windows. It should work also on Mac computers but this has not been tested.
 Depending on your Python distribution you may want to install the python modules pysoundanalyser depends on before
 installing pysoundanalyser (e.g. via the conda package manager if you’re using the Anaconda Python distribution). The
 dependencies are:
-• PyQt5
+• PyQt6
 • numpy
 • scipy
 • pandas
 • matplotlib
 • PyAudio
 if you’re using Linux you can also install pyalsaaudio to have an addition sound output option. If you’re using conda
 on Windows I’d recommend installing PyAudio via pip because the PyAudio version available on conda is not built
 with support for the WASAPI output interface (at least that was the case the last time I checked).
 
 3
 
-pysoundanalyser, Release 0.3.4
+pysoundanalyser, Release 0.3.7
 
 4
 
 Chapter 2. Installation
 
 CHAPTER
 
 THREE
 
 USER INTERFACE
 
-• Load Sound The Load Sound button allows you to load a wav file into the program. Currently only 16 and 32
-bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is
-fine and fast for wav files of short durations (tens of seconds), but longer sound files are going to consume huge
+• Load Sound The Load Sound button allows you to load a wav file into the program. Currently only 16, 24, and
+32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is
+fine and fast for wav files of short duration (tens of seconds), but longer sound files are going to consume huge
 amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other
 software, like audacity.
 – Save As The Save As button allows you to save PSA sound objects as wav files. Currently it is only possible
-to save sounds as 16 or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format,
-and multiple PSA sound objects have been selected for saving, they will be summed together before saving.
-If you choose a stereo (2-channels) format, “right” and “left” PSA sound objects will be saved to their
-respective channels in the wav file; if multiple “right” or “left” PSA sound objects have been selected, they
-will be summed before saving.
+to save sounds as 16, 24, or 32 bit wav files with one or two channels. If you choose a mono (1-channel)
+format, and multiple PSA sound objects have been selected for saving, they will be summed together before
+saving. If you choose a stereo (2-channels) format, “right” and “left” PSA sound objects will be saved to
+their respective channels in the wav file; if multiple “right” or “left” PSA sound objects have been selected,
+they will be summed before saving.
 • Clone Sound
 • Concatenate
 • Cut The Cut button allows you to remove segments of a sound waveform. The starting and ending points of the
 segments to be cut off can be specified in seconds, milliseconds, or sample numbers. When working with sample
 numbers, note that PSA indexing works exactly like numpy indexing. Examples:
 >>> import numpy as np #import numpy
 >>> sig = np.arange(10) #generate a 10-elements array
@@ -129,15 +129,15 @@
 • Spectrum Plot the spectrum of the currently selected sound.
 • Spectrogram Plot the spectrogram of the currently selected sound.
 • Autocorrelation Plot the autocorrelation function of the currently selected sound.
 • Autocorrelogram Plot the autocorrelogram of the currently selected sound.
 
 5
 
-pysoundanalyser, Release 0.3.4
+pysoundanalyser, Release 0.3.7
 
 • Level Difference Show the difference in level between two selected sounds.
 • Scale Change the level of the currently selected sound.
 • Resample Resample the currently selected sound.
 • Rename Rename the currently selected sound.
 • Remove Remove the currently selected sound from the workspace.
 • Remove All Remove all sounds from the workspace.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/conf.py` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'pysoundanalyser'
 copyright = '2010-2023, Samuele Carcagno'
 author = 'Samuele Carcagno'
-release = "0.3.4"
+release = "0.3.7"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
 
 templates_path = ['_templates']
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/installation.rst` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/installation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ::
    
    pysoundanalyser
 
 Note that the program needs to be launched in the same Python environment in which it has been installed. The program has been tested on Linux and Windows. It should work also on Mac computers but this has not been tested. Depending on your Python distribution you may want to install the python modules pysoundanalyser depends on before installing pysoundanalyser (e.g. via the conda package manager if you're using the Anaconda Python distribution). The dependencies are:
 
-- PyQt5 
+- PyQt6 
 - numpy 
 - scipy 
 - pandas 
 - matplotlib 
 - PyAudio 
 
 if you're using Linux you can also install `pyalsaaudio` to have an addition sound output option. If you're using conda on Windows I'd recommend installing PyAudio via pip because the PyAudio version available on conda is not built with support for the WASAPI output interface (at least that was the case the last time I checked).
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/intro.rst` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/make.bat` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/doc/user_interface.rst` & `pysoundanalyser-0.3.7/pysoundanalyser/doc/user_interface.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 .. _sec-user_interface:
 
 ****************
 User Interface
 ****************
 
-- **Load Sound** The ``Load Sound`` button allows you to load a wav file into the program. Currently only 16 and 32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is fine and fast for wav files of short durations (tens of seconds), but longer sound files are going to consume huge amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other software, like audacity.  
+- **Load Sound** The ``Load Sound`` button allows you to load a wav file into the program. Currently only 16, 24, and 32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is fine and fast for wav files of short duration (tens of seconds), but longer sound files are going to consume huge amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other software, like audacity.  
 
-  - **Save As** The ``Save As`` button allows you to save PSA sound objects as wav files. Currently it is only possible to save sounds as 16 or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format, and multiple PSA sound objects have been selected for saving, they will be summed together before saving. If you choose a stereo (2-channels) format, "right" and "left" PSA sound objects will be saved to their respective channels in the wav file; if multiple "right" or "left" PSA sound objects have been selected, they will be summed before saving.
+  - **Save As** The ``Save As`` button allows you to save PSA sound objects as wav files. Currently it is only possible to save sounds as 16, 24, or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format, and multiple PSA sound objects have been selected for saving, they will be summed together before saving. If you choose a stereo (2-channels) format, "right" and "left" PSA sound objects will be saved to their respective channels in the wav file; if multiple "right" or "left" PSA sound objects have been selected, they will be summed before saving.
 
 - **Clone Sound**
       
 - **Concatenate**
   
 - **Cut** The ``Cut`` button allows you to remove segments of a sound waveform. The starting and ending points of the segments to be cut off can be specified in seconds, milliseconds, or sample numbers. When working with sample numbers, note that PSA indexing works exactly like numpy indexing. Examples:
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/global_parameters.py` & `pysoundanalyser-0.3.7/pysoundanalyser/global_parameters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 
@@ -59,36 +59,36 @@
 import platform, os, pickle
 
 
 def set_global_parameters(prm):
     prm['appData']['available_colormaps'] = [m for m in matplotlib.cm.datad if not m.endswith("_r")]
     prm['appData']['available_windows'] = ['none', 'hamming', 'hanning', 'blackman', 'bartlett']
     prm['appData']['available_filters'] = ['fir2_presets']
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
 
     prm['appData']['alsaaudioAvailable'] = alsaaudioAvailable
     prm['appData']['pyaudioAvailable'] = pyaudioAvailable
 
     if platform.system() == 'Linux':
         prm['appData']['available_play_commands'] = []
         if os.system("which aplay") == 0:
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/random_id.py` & `pysoundanalyser-0.3.7/pysoundanalyser/random_id.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2017 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/sndlib.py` & `pysoundanalyser-0.3.7/pysoundanalyser/sndlib.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/threaded_plotters.py` & `pysoundanalyser-0.3.7/pysoundanalyser/threaded_plotters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/utilities_open_manual.py` & `pysoundanalyser-0.3.7/pysoundanalyser/utilities_open_manual.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/utility_functions.py` & `pysoundanalyser-0.3.7/pysoundanalyser/utility_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/wavpy.py` & `pysoundanalyser-0.3.7/pysoundanalyser/wavpy.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/wavpy_sndf.py` & `pysoundanalyser-0.3.7/pysoundanalyser/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/win_acf_plot.py` & `pysoundanalyser-0.3.7/pysoundanalyser/win_acf_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/win_autocorrelogram_plot.py` & `pysoundanalyser-0.3.7/pysoundanalyser/win_autocorrelogram_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/win_generic_plot.py` & `pysoundanalyser-0.3.7/pysoundanalyser/win_generic_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/win_spectrogram_plot.py` & `pysoundanalyser-0.3.7/pysoundanalyser/win_spectrogram_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/win_spectrum_plot.py` & `pysoundanalyser-0.3.7/pysoundanalyser/win_spectrum_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser/win_waveform_plot.py` & `pysoundanalyser-0.3.7/pysoundanalyser/win_waveform_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- 
-#   Copyright (C) 2010-2023 Samuele Carcagno <sam.carcagno@gmail.com>
+#   Copyright (C) 2010-2024 Samuele Carcagno <sam.carcagno@gmail.com>
 #   This file is part of pysoundanalyser
 
 #    pysoundanalyser is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser.egg-info/PKG-INFO` & `pysoundanalyser-0.3.7/pysoundanalyser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoundanalyser
-Version: 0.3.4
+Version: 0.3.7
 Summary: Python program for visualizing short sounds (waveform, spectrum, etc...)
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,11 +693,17 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING.txt
+Requires-Dist: matplotlib>=3.0.0
+Requires-Dist: numpy>=1.0.0
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: PyAudio>=0.2.11
+Requires-Dist: PyQt6>=6.6.0
+Requires-Dist: scipy>=1.0.1
 
 [![Project Status: Unsupported – The project has reached a stable, usable state but the author(s) have ceased all work on it. A new maintainer may be desired.](https://www.repostatus.org/badges/latest/unsupported.svg)](https://www.repostatus.org/#unsupported)
 
 `pysoundanalyser` is an application which provides a graphical user interface to analyse short wav files.
```

### Comparing `pysoundanalyser-0.3.4/pysoundanalyser.egg-info/SOURCES.txt` & `pysoundanalyser-0.3.7/pysoundanalyser.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.readthedocs.yaml
 COPYING.txt
 CREDITS.txt
 INSTALL.txt
 MANIFEST.in
 README.md
 pyproject.toml
 pysoundanalyser.desktop
@@ -88,14 +89,15 @@
 pysoundanalyser/doc/Makefile
 pysoundanalyser/doc/conf.py
 pysoundanalyser/doc/index.rst
 pysoundanalyser/doc/installation.rst
 pysoundanalyser/doc/intro.rst
 pysoundanalyser/doc/make.bat
 pysoundanalyser/doc/mkdoc.sh
+pysoundanalyser/doc/requirements.txt
 pysoundanalyser/doc/user_interface.rst
 pysoundanalyser/doc/_build/html/.buildinfo
 pysoundanalyser/doc/_build/html/genindex.html
 pysoundanalyser/doc/_build/html/index.html
 pysoundanalyser/doc/_build/html/installation.html
 pysoundanalyser/doc/_build/html/intro.html
 pysoundanalyser/doc/_build/html/objects.inv
```

### Comparing `pysoundanalyser-0.3.4/resources.qrc` & `pysoundanalyser-0.3.7/resources.qrc`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.4/translations/pysoundanalyser_it.qm` & `pysoundanalyser-0.3.7/translations/pysoundanalyser_it.qm`

 * *Files 16% similar despite different names*

```diff
@@ -1,1811 +1,1607 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0569 745f 4954 4200 000a 9000  .....it_ITB.....
+00000010: a700 0000 0569 745f 4954 4200 0009 6800  .....it_ITB...h.
 00000020: 004a c400 000e 2b00 004e 6e00 0001 b300  .J....+..Nn.....
-00000030: 004e 6e00 0010 ff00 004e 6e00 004b 3600  .Nn......Nn..K6.
+00000030: 004e 6e00 0010 ff00 004e 6e00 003f 9e00  .Nn......Nn..?..
 00000040: 004e 8400 0001 d100 004e 8400 0011 2e00  .N.......N......
-00000050: 004e 8400 004b aa00 0058 b400 001b 6b00  .N...K...X....k.
-00000060: 0058 b400 003b 7700 02ad c400 0005 ac00  .X...;w.........
+00000050: 004e 8400 0040 1200 0058 b400 001b 6b00  .N...@...X....k.
+00000060: 0058 b400 002f df00 02ad c400 0005 ac00  .X.../..........
 00000070: 035e 7d00 0006 8a00 0493 b500 0008 cd00  .^}.............
-00000080: 0493 b500 0038 e800 0496 a800 0008 fd00  .....8..........
-00000090: 0496 a800 0039 1a00 0496 a800 003d b800  .....9.......=..
-000000a0: 0496 a800 0044 3100 04b8 5a00 002f 0d00  .....D1...Z../..
-000000b0: 04b8 5a00 0045 c600 04cf 0400 000e e800  ..Z..E..........
-000000c0: 04d7 fe00 002f b300 04d7 fe00 0046 9300  ...../.......F..
-000000d0: 04e8 f400 0059 bf00 052b d400 0011 ec00  .....Y...+......
-000000e0: 052b d400 002a 1500 052b d400 002b 7700  .+...*...+...+w.
-000000f0: 052b d400 003a 3300 052b d400 003f c400  .+...:3..+...?..
-00000100: 052b d400 004c 7000 0546 4f00 0013 6900  .+...Lp..FO...i.
-00000110: 0546 4f00 0060 f700 0556 4500 0002 7800  .FO..`...VE...x.
-00000120: 0556 4500 0015 f600 0556 4500 0052 1600  .VE......VE..R..
-00000130: 0570 4b00 001a 2400 0570 4b00 003a fa00  .pK...$..pK..:..
-00000140: 0570 4b00 0053 c300 0572 8900 001a 5600  .pK..S...r....V.
-00000150: 05a0 4500 0055 6700 0756 4500 0021 c800  ..E..Ug..VE..!..
-00000160: 129f aa00 0000 cb00 129f aa00 0030 af00  .............0..
-00000170: 129f aa00 0048 a400 2abb 0400 0004 fd00  .....H..*.......
-00000180: 2ad0 2500 0005 3a00 2aec 3000 0005 e600  *.%...:.*.0.....
-00000190: 2b73 6400 0006 1d00 4949 7200 0024 5400  +sd.....IIr..$T.
-000001a0: 4b85 c000 0039 a400 4b85 c000 003e 4800  K....9..K....>H.
-000001b0: 4f19 f500 0018 b600 5278 bc00 0011 af00  O.......Rx......
-000001c0: 554a 6900 0051 9400 5560 9500 0015 bf00  UJi..Q..U`......
-000001d0: 5560 9500 003a 6f00 556e 9f00 0052 5000  U`...:o.Un...RP.
-000001e0: 58fd f400 001c c000 58fd f400 002a 5100  X.......X....*Q.
-000001f0: 58fd f400 002c 0300 58fd f400 003b ac00  X....,..X....;..
-00000200: 58fd f400 0041 3e00 58fd f400 0054 8200  X....A>.X....T..
-00000210: 5998 2500 001d 6e00 5c06 8a00 0002 ce00  Y.%...n.\.......
-00000220: 5c06 8a00 0038 be00 5c06 8a00 0057 4f00  \....8..\....WO.
-00000230: 5c48 fa00 0032 1600 5c48 fa00 004b 6700  \H...2..\H...Kg.
-00000240: 5ca0 5400 0002 9f00 5ca0 5400 001e 8700  \.T.....\.T.....
-00000250: 5ca0 5400 0041 e600 5ca0 5400 0055 9900  \.T..A..\.T..U..
-00000260: 5df0 a500 0020 8c00 5df0 a500 003d 3b00  ].... ..]....=;.
-00000270: 5df0 a500 0057 8600 5ed4 9500 0017 6a00  ]....W..^.....j.
-00000280: 62ec a900 003f 3e00 8f43 1900 0036 6500  b....?>..C...6e.
-00000290: 8f43 1900 0051 2300 f661 b000 003a a801  .C...Q#..a...:..
-000002a0: 2975 c900 002d 5001 2975 c900 0043 5801  )u...-P.)u...CX.
-000002b0: 2c40 7000 002b 1f01 2f38 2900 0032 4c01  ,@p..+../8)..2L.
-000002c0: 2f38 2900 004b db01 59c3 9000 0025 dc01  /8)..K..Y....%..
-000002d0: 6a24 5900 0012 ce01 728f 1e00 0008 2101  j$Y.....r.....!.
-000002e0: 8fc9 3d00 0008 7601 9176 c300 0023 4801  ..=...v..v...#H.
-000002f0: 979a 9000 002b b101 aa1f 3700 0003 3101  .....+....7...1.
-00000300: aa1f 3700 0011 5d01 aa1f 3700 0063 7201  ..7...]...7..cr.
-00000310: aa1f 3700 0065 4901 bab5 4a00 0058 eb01  ..7..eI...J..X..
-00000320: d21f e200 0058 0f02 44ea 5c00 005e 7d02  .....X..D.\..^}.
-00000330: 792f 0900 0003 7902 7a0f 5900 002f 6e02  y/....y.z.Y../n.
-00000340: 7a0f 5900 0046 4102 8fb8 6900 002f da02  z.Y..FA...i../..
-00000350: 8fb8 6900 0047 5702 c844 c000 003d 7402  ..i..GW..D...=t.
-00000360: d4e6 e900 0028 8d02 d4e6 e900 0062 3f02  .....(.......b?.
-00000370: da74 c500 000c df02 e914 f900 002d b802  .t...........-..
-00000380: e914 f900 0043 cd03 006e 4a00 0023 1303  .....C...nJ..#..
-00000390: 22c8 e300 000f 5803 2bd0 aa00 005a ff03  ".....X.+....Z..
-000003a0: 539b 6a00 0059 f703 5d16 1200 000a 7903  S.j..Y..].....y.
-000003b0: 6e68 d300 0021 8703 6e68 d300 0027 fb03  nh...!..nh...'..
-000003c0: 81c3 3a00 0040 5103 97bf 8500 001f a003  ..:..@Q.........
-000003d0: 9f59 6a00 005c 4603 e534 4300 0007 5c03  .Yj..\F..4C...\.
-000003e0: fe9a e500 001c f704 22cc d900 0037 8404  ........"....7..
-000003f0: 22cc d900 0053 f704 26f4 6a00 003c 9904  "....S..&.j..<..
-00000400: 46c3 0900 001f 4e04 6c75 9000 0013 d604  F.....N.lu......
-00000410: 90b6 c000 0060 4704 a6a0 4500 0044 e304  .....`G...E..D..
-00000420: ad42 4900 002e 0f04 ad42 4900 0044 6d04  .BI......BI..Dm.
-00000430: ee72 2200 0006 f105 29f3 5a00 005a b705  .r".....).Z..Z..
-00000440: 2caf e200 0001 4405 2caf e200 0010 6e05  ,.....D.,.....n.
-00000450: 2caf e200 004a a105 3315 6000 005e 0b05  ,....J..3.`..^..
-00000460: 6e89 8a00 0037 5905 6e89 8a00 0053 8b05  n....7Y.n....S..
-00000470: 7366 d300 005b 5c05 77c1 ba00 003b 2e05  sf...[\.w....;..
-00000480: 77c1 ba00 0040 ac05 884b 5d00 0054 3c05  w....@...K]..T<.
-00000490: 8c46 c500 001b 9e05 8c48 3500 001c 2205  .F.......H5...".
-000004a0: 8cbe ca00 0004 3205 8cbe ca00 0064 4905  ......2......dI.
-000004b0: 8cbe ca00 0066 2005 968c 3300 0062 0105  .....f ...3..b..
-000004c0: 968c 3300 0064 9305 a6c0 c400 005b d505  ..3..d.......[..
-000004d0: aac8 bf00 0061 8f05 bb74 5a00 0026 9305  .....a...tZ..&..
-000004e0: d062 c400 001f d905 d062 c400 003d 0305  .b.......b...=..
-000004f0: dc7c 9300 002d 0105 dec6 0d00 0022 8f05  .|...-......."..
-00000500: f5b6 0500 0006 b406 0c4a 1300 0009 3706  .........J....7.
-00000510: 419e 0a00 0028 4106 419e 0a00 0058 6306  A....(A.A....Xc.
-00000520: 419e 0a00 0061 b906 4380 da00 0058 ad06  A....a..C....X..
-00000530: 5874 7000 002a cd06 58a8 5400 0016 8006  Xtp..*..X.T.....
-00000540: 58a8 5400 0052 db06 5a22 8400 000e 5406  X.T..R..Z"....T.
-00000550: 5d5f 3400 0012 8606 5fdb 1a00 0000 0006  ]_4....._.......
-00000560: 5fdb 1a00 002e 7806 5fdb 1a00 0045 1706  _.....x._....E..
-00000570: 9000 5300 0031 4606 9000 5300 0049 5506  ..S..1F...S..IU.
-00000580: 95b0 5000 0033 6b06 95b0 5000 004d 6a06  ..P..3k...P..Mj.
-00000590: 9612 3900 0032 c706 9612 3900 004c ac06  ..9..2....9..L..
-000005a0: acab 5d00 005c f506 b005 6000 0025 3106  ..]..\....`..%1.
-000005b0: babc 1d00 001f 1206 c2cc 6c00 001b d806  ..........l.....
-000005c0: d1ce 9e00 0014 1507 0f66 1a00 0002 4007  .........f....@.
-000005d0: 0f66 1a00 0036 c907 0f66 1a00 0051 cb07  .f...6...f...Q..
-000005e0: 145e 0400 000d 4b07 2947 9500 0012 2607  .^....K.)G....&.
-000005f0: 2b54 9c00 001d a707 4d73 2200 0003 b207  +T......Ms".....
-00000600: 4d73 2200 005a 6f07 4d73 2200 0063 bf07  Ms"..Zo.Ms"..c..
-00000610: 4d73 2200 0065 9607 58cb e800 0003 f007  Ms"..e..X.......
-00000620: 58cb e800 0064 0207 58cb e800 0065 d907  X....d..X....e..
-00000630: 64a7 6c00 0029 8607 8f43 1900 0035 1e07  d.l..)...C...5..
-00000640: 8f43 1900 004f b507 959e 1300 0006 4807  .C...O........H.
-00000650: a0f5 ea00 003e 8a07 a5d0 8200 0057 bf07  .....>.......W..
-00000660: ebf7 9e00 0014 ec08 14f9 e000 002c b808  .............,..
-00000670: 14f9 e000 003c 4e08 14f9 e000 0042 2b08  .....<N......B+.
-00000680: 14f9 e000 0055 db08 3230 2200 001b 3008  .....U..20"...0.
-00000690: 4b6e 2300 0020 c308 4b6e 2300 0027 2808  Kn#.. ..Kn#..'(.
-000006a0: 4bad e000 0021 0508 4bad e000 0027 6f08  K....!..K....'o.
-000006b0: 54f6 2000 0029 d608 54f6 2000 0060 7108  T. ..)..T. ..`q.
-000006c0: 611f a900 0028 e608 611f a900 0062 da08  a....(..a....b..
-000006d0: 62f8 b900 003f 8108 7045 0d00 0022 d308  b....?..pE..."..
-000006e0: 9010 9300 0032 8e08 9010 9300 004c 2a08  .....2.......L*.
-000006f0: 9460 1300 0000 5108 9460 1300 0047 1508  .`....Q..`...G..
-00000700: 9525 8900 0034 ad08 9525 8900 004f 3708  .%...4...%...O7.
-00000710: 9555 8900 0035 f408 9555 8900 0050 a508  .U...5...U...P..
-00000720: 9b34 a400 003e e208 adbf 4900 0033 aa08  .4...>....I..3..
-00000730: adbf 4900 004d b608 c3c4 c000 0025 8608  ..I..M.......%..
-00000740: cbd3 5d00 0020 4808 d750 6400 0000 8008  ..].. H..Pd.....
-00000750: d750 6400 0048 4608 e22c 3500 000d 9208  .Pd..HF..,5.....
-00000760: e22c 3500 002a 8a09 0096 8700 0043 1309  .,5..*.......C..
-00000770: 22cf 8900 002f 3e09 22cf 8900 0046 0409  "..../>."....F..
-00000780: 7437 4a00 0014 a709 8c74 d300 001d 2d09  t7J......t....-.
-00000790: a631 ac00 005d a009 e854 fc00 000c a609  .1...]...T......
-000007a0: e96a 9900 0031 d209 e96a 9900 004a 5009  .j...1...j...JP.
-000007b0: f416 7e00 000f 1a09 fe43 9c00 005b 980a  ..~......C...[..
-000007c0: 02c4 c500 001e 4a0a 0e7a 7000 005f 4a0a  ......J..zp.._J.
-000007d0: 4413 8500 0016 cf0a 652e 8400 0016 2e0a  D.......e.......
-000007e0: 652e 8400 0052 870a 6594 4500 0042 cb0a  e....R..e.E..B..
-000007f0: 8988 5000 0026 380a c092 b900 0038 780a  ..P..&8......8x.
-00000800: c092 b900 0056 fc0a e230 e400 0001 790a  .....V...0....y.
-00000810: e230 e400 0010 b40a e230 e400 004a e90a  .0.......0...J..
-00000820: e309 fe00 000a 220a eb66 0900 0007 ce0a  ......"..f......
-00000830: ecea 8800 0001 020a ecea 8800 0010 1b0a  ................
-00000840: ecea 8800 0049 fb0a f5b6 0500 000f aa0b  .....I..........
-00000850: 16e8 3400 0046 c70b 1731 f900 0013 1d0b  ..4..F...1......
-00000860: 19dc 7900 0030 3e0b 19dc 7900 0047 c80b  ..y..0>...y..G..
-00000870: 19ec e500 0039 e30b 3c48 1900 0037 bc0b  .....9..<H...7..
-00000880: 3c48 1900 0056 260b 8e85 7300 0061 1f0b  <H...V&...s..a..
-00000890: 91f3 5000 0060 ac0b a3dc 0c00 001d fc0b  ..P..`..........
-000008a0: c487 4300 000d d50b c4de 0000 005f f30b  ..C.........._..
-000008b0: ef83 dd00 001e c70c 254e 0500 0019 690c  ........%N....i.
-000008c0: 340d da00 0037 070c 340d da00 0053 2c0c  4....7..4....S,.
-000008d0: 442e e200 0062 940c 442e e200 0064 cc0c  D....b..D....d..
-000008e0: 466e a000 002c 3a0c 466f a000 002c 790c  Fn...,:.Fo...,y.
-000008f0: 4ca2 7500 0005 6f0c 62c7 de00 0002 f20c  L.u...o.b.......
-00000900: 7471 fa00 0024 e80c 7502 be00 0013 930c  tq...$..u.......
-00000910: 87a1 1c00 0042 790c 9844 a500 001c 5e0c  .....By..D....^.
-00000920: 9844 a500 005f 0b0c 9d58 5000 0015 400c  .D..._...XP...@.
-00000930: a7e9 3a00 0039 560c a7e9 3a00 003d f70c  ..:..9V...:..=..
-00000940: b5cd 6000 0024 a70c c8fc 2500 0040 f80c  ..`..$....%..@..
-00000950: db87 9a00 0059 640c ddc2 0300 001a eb0d  .....Yd.........
-00000960: 11fa 1500 003b e50d 11fa 1500 0041 7a0d  .....;.......Az.
-00000970: 11fa 1500 0054 bb0d 8950 1700 0020 0f0d  .....T...P... ..
-00000980: 8950 1700 005c 0d0d 8950 1700 005f bd0d  .P...\...P..._..
-00000990: a0d1 4500 0018 1d0d a5e5 9000 0031 920d  ..E..........1..
-000009a0: a5e5 9000 0049 ae0d c6d0 1300 0033 200d  .....I.......3 .
-000009b0: c6d0 1300 004d 120e 04b6 fa00 0004 770e  .....M........w.
-000009c0: 04b6 fa00 0029 450e 04b6 fa00 005c b60e  .....)E......\..
-000009d0: 04b6 fa00 0063 350e 04b6 fa00 0065 0f0e  .....c5......e..
-000009e0: 448f 1800 000f e50e 4949 5200 0004 ac0e  D.......IIR.....
-000009f0: 6fb1 b300 000b d10e 7c48 7a00 0040 030e  o.......|Hz..@..
-00000a00: a06b b400 005d 3d0e b163 bd00 000e 830f  .k...]=..c......
-00000a10: 0784 0400 0021 f20f 3d90 4500 0001 ef0f  .....!..=.E.....
-00000a20: 3d90 4500 0014 710f 3d90 4500 004e 540f  =.E...q.=.E..NT.
-00000a30: 4fc6 8900 0038 120f 4fc6 8900 0056 890f  O....8..O....V..
-00000a40: 920c d900 0035 820f 920c d900 0050 260f  .....5.......P&.
-00000a50: 950c d900 0034 3b0f 950c d900 004e b80f  .....4;......N..
-00000a60: 95e3 5200 0055 240f a659 f900 0030 ec0f  ..R..U$..Y...0..
-00000a70: a659 f900 0048 ee0f ca7e 9900 002e cf0f  .Y...H...~......
-00000a80: ca7e 9900 0045 7b0f df6d 7f00 0023 9e0f  .~...E{..m...#..
-00000a90: df6e 4300 0021 470f df6e 4300 0027 b60f  .nC..!G..nC..'..
-00000aa0: e230 9300 000a ef0f fdb3 0d00 001a 9269  .0.............i
-00000ab0: 0000 666a 0300 0000 2800 4400 6900 6600  ..fj....(.D.i.f.
-00000ac0: 6600 6500 7200 6500 6e00 7a00 6100 2000  f.e.r.e.n.z.a. .
-00000ad0: 6400 6900 6300 6f00 7400 6900 6300 6100  d.i.c.o.t.i.c.a.
-00000ae0: 3a08 0000 0000 0600 0000 1444 6963 686f  :..........Dicho
-00000af0: 7469 6320 4469 6666 6572 656e 6365 3a07  tic Difference:.
-00000b00: 0000 0000 0103 0000 0012 0041 0072 006d  ...........A.r.m
-00000b10: 006f 006e 0069 0063 006f 003a 0800 0000  .o.n.i.c.o.:....
-00000b20: 0006 0000 0008 4861 726d 6f6e 6963 0700  ......Harmonic..
-00000b30: 0000 0001 0300 0000 2400 4100 7200 6d00  ........$.A.r.m.
-00000b40: 6f00 6e00 6900 6300 6f00 2000 6100 6c00  o.n.i.c.o. .a.l.
-00000b50: 6c00 7500 6e00 6700 6100 7400 6f08 0000  l.u.n.g.a.t.o...
-00000b60: 0000 0600 0000 1248 6172 6d6f 6e69 6320  .......Harmonic 
-00000b70: 5374 7265 7463 6865 6407 0000 0000 0103  Stretched.......
-00000b80: 0000 0016 0041 0072 006d 006f 006e 0069  .....A.r.m.o.n.i
-00000b90: 0063 0069 0074 00e0 003a 0800 0000 0006  .c.i.t...:......
-00000ba0: 0000 000c 4861 726d 6f6e 6963 6974 793a  ....Harmonicity:
-00000bb0: 0700 0000 0001 0300 0000 2000 5000 6900  .......... .P.i.
-00000bc0: 7400 6300 6800 2000 6400 6900 2000 4800  t.c.h. .d.i. .H.
-00000bd0: 7500 6700 6700 6900 6e00 7308 0000 0000  u.g.g.i.n.s.....
-00000be0: 0600 0000 0d48 7567 6769 6e73 2050 6974  .....Huggins Pit
-00000bf0: 6368 0700 0000 0001 0300 0000 1600 4900  ch............I.
-00000c00: 5000 4400 2000 4c00 6900 6e00 6500 6100  P.D. .L.i.n.e.a.
-00000c10: 7200 6508 0000 0000 0600 0000 0a49 5044  r.e..........IPD
-00000c20: 204c 696e 6561 7207 0000 0000 0103 0000   Linear.........
-00000c30: 001a 0049 0050 0044 0020 0061 0020 0073  ...I.P.D. .a. .s
-00000c40: 0063 0061 006c 0069 006e 006f 0800 0000  .c.a.l.i.n.o....
-00000c50: 0006 0000 000b 4950 4420 5374 6570 7065  ......IPD Steppe
-00000c60: 6407 0000 0000 0103 0000 0006 0049 0052  d............I.R
-00000c70: 004e 0800 0000 0006 0000 0003 4952 4e07  .N..........IRN.
-00000c80: 0000 0000 0103 0000 0006 0049 0054 0044  ...........I.T.D
-00000c90: 0800 0000 0006 0000 0003 4954 4407 0000  ..........ITD...
-00000ca0: 0000 0103 0000 002c 0052 0075 006d 006f  .......,.R.u.m.o
-00000cb0: 0072 0065 0020 0061 0020 0062 0061 006e  .r.e. .a. .b.a.n
-00000cc0: 0064 0061 0020 0073 0074 0072 0065 0074  .d.a. .s.t.r.e.t
-00000cd0: 0074 0061 0800 0000 0006 0000 0010 4e61  .t.a..........Na
-00000ce0: 7272 6f77 6261 6e64 204e 6f69 7365 0700  rrowband Noise..
-00000cf0: 0000 0001 0300 0000 1800 5400 6900 7000  ..........T.i.p.
-00000d00: 6f00 2000 7200 7500 6d00 6f00 7200 6500  o. .r.u.m.o.r.e.
-00000d10: 3a08 0000 0000 0600 0000 0b4e 6f69 7365  :..........Noise
-00000d20: 2054 7970 653a 0700 0000 0001 0300 0000   Type:..........
-00000d30: 0e00 4e00 6500 7300 7300 7500 6e00 6f08  ..N.e.s.s.u.n.o.
-00000d40: 0000 0000 0600 0000 044e 6f6e 6507 0000  .........None...
-00000d50: 0000 0103 0000 0012 0053 0069 006e 0075  .........S.i.n.u
-00000d60: 0073 006f 0069 0064 0065 0800 0000 0006  .s.o.i.d.e......
-00000d70: 0000 0008 5369 6e75 736f 6964 0700 0000  ....Sinusoid....
-00000d80: 0001 0300 0000 0a00 5400 6900 7000 6f00  ........T.i.p.o.
-00000d90: 3a08 0000 0000 0600 0000 0554 7970 653a  :..........Type:
-00000da0: 0700 0000 0001 0300 0000 1800 4300 6f00  ............C.o.
-00000db0: 7200 7200 6500 6c00 6100 7a00 6900 6f00  r.r.e.l.a.z.i.o.
-00000dc0: 6e00 6508 0000 0000 0600 0000 0b43 6f72  n.e..........Cor
-00000dd0: 7265 6c61 7469 6f6e 0700 0000 0761 6366  relation.....acf
-00000de0: 506c 6f74 0103 0000 0020 0044 0069 0061  Plot..... .D.i.a
-00000df0: 006c 006f 0067 006f 0020 0064 0069 0020  .l.o.g.o. .d.i. 
-00000e00: 0069 006e 0070 0075 0074 0800 0000 0006  .i.n.p.u.t......
-00000e10: 0000 000c 496e 7075 7420 4469 616c 6f67  ....Input Dialog
-00000e20: 0700 0000 0761 6366 506c 6f74 0103 0000  .....acfPlot....
-00000e30: 0016 0052 0069 0074 0061 0072 0064 006f  ...R.i.t.a.r.d.o
-00000e40: 0020 0028 0073 0029 0800 0000 0006 0000  . .(.s.)........
-00000e50: 0007 4c61 6720 2873 2907 0000 0007 6163  ..Lag (s).....ac
-00000e60: 6650 6c6f 7401 0300 0000 1800 4300 6f00  fPlot.......C.o.
-00000e70: 6c00 6f00 7200 6500 2000 6c00 6900 6e00  l.o.r.e. .l.i.n.
-00000e80: 6500 6108 0000 0000 0600 0000 0a4c 696e  e.a..........Lin
-00000e90: 6520 436f 6c6f 7207 0000 0007 6163 6650  e Color.....acfP
-00000ea0: 6c6f 7401 0300 0000 1c00 5300 7000 6500  lot.......S.p.e.
-00000eb0: 7300 7300 6f00 7200 6500 2000 4c00 6900  s.s.o.r.e. .L.i.
-00000ec0: 6e00 6500 6108 0000 0000 0600 0000 0a4c  n.e.a..........L
-00000ed0: 696e 6520 5769 6474 6807 0000 0007 6163  ine Width.....ac
-00000ee0: 6650 6c6f 7401 0300 0000 1e00 5300 7000  fPlot.......S.p.
-00000ef0: 6500 7300 7300 6f00 7200 6500 2000 4c00  e.s.s.o.r.e. .L.
-00000f00: 6900 6e00 6500 6100 3a08 0000 0000 0600  i.n.e.a.:.......
-00000f10: 0000 0b4c 696e 6520 5769 6474 683a 0700  ...Line Width:..
-00000f20: 0000 0761 6366 506c 6f74 0103 0000 0012  ...acfPlot......
-00000f30: 0046 0069 006e 0065 0073 0074 0072 0061  .F.i.n.e.s.t.r.a
-00000f40: 003a 0800 0000 0006 0000 0007 5769 6e64  .:..........Wind
-00000f50: 6f77 3a07 0000 0007 6163 6650 6c6f 7401  ow:.....acfPlot.
-00000f60: 0300 0000 1e00 2600 4100 7000 7000 6c00  ......&.A.p.p.l.
-00000f70: 6900 6300 6100 2000 4600 6900 6c00 7400  i.c.a. .F.i.l.t.
-00000f80: 7200 6f08 0000 0000 0600 0000 0d26 4170  r.o..........&Ap
-00000f90: 706c 7920 4669 6c74 6572 0700 0000 1161  ply Filter.....a
-00000fa0: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
-00000fb0: 0103 0000 0012 0026 004d 006f 0064 0069  .......&.M.o.d.i
-00000fc0: 0066 0069 0063 0061 0800 0000 0006 0000  .f.i.c.a........
-00000fd0: 0005 2645 6469 7407 0000 0011 6170 706c  ..&Edit.....appl
-00000fe0: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
-00000ff0: 0000 0a00 2600 4600 6900 6c00 6508 0000  ....&.F.i.l.e...
-00001000: 0000 0600 0000 0526 4669 6c65 0700 0000  .......&File....
-00001010: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-00001020: 6f77 0103 0000 000e 0026 0047 0065 006e  ow.......&.G.e.n
-00001030: 0065 0072 0061 0800 0000 0006 0000 0009  .e.r.a..........
-00001040: 2647 656e 6572 6174 6507 0000 0011 6170  &Generate.....ap
-00001050: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
-00001060: 0300 0000 1000 2600 4f00 7400 7400 6900  ......&.O.t.t.i.
-00001070: 6500 6e00 6908 0000 0000 0600 0000 0426  e.n.i..........&
-00001080: 4765 7407 0000 0011 6170 706c 6963 6174  Get.....applicat
-00001090: 696f 6e57 696e 646f 7701 0300 0000 0c00  ionWindow.......
-000010a0: 2600 4100 6900 7500 7400 6f08 0000 0000  &.A.i.u.t.o.....
-000010b0: 0600 0000 0526 4865 6c70 0700 0000 1161  .....&Help.....a
-000010c0: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
-000010d0: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
-000010e0: 2650 6c6f 7407 0000 0011 6170 706c 6963  &Plot.....applic
-000010f0: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
-00001100: 1400 2600 5400 7200 6100 7300 6600 6f00  ..&.T.r.a.s.f.o.
-00001110: 7200 6d00 6108 0000 0000 0600 0000 0826  r.m.a..........&
-00001120: 5072 6f63 6573 7307 0000 0011 6170 706c  Process.....appl
-00001130: 6963 6174 696f 6e57 696e 646f 7701 03ff  icationWindow...
-00001140: ffff ff08 0000 0000 0600 0000 042e 7b30  ..............{0
-00001150: 7d07 0000 0011 6170 706c 6963 6174 696f  }.....applicatio
-00001160: 6e57 696e 646f 7701 0300 0000 1000 5400  nWindow.......T.
-00001170: 6f00 6e00 6f00 2000 4100 4d00 2008 0000  o.n.o. .A.M. ...
-00001180: 0000 0600 0000 0741 4d20 546f 6e65 0700  .......AM Tone..
-00001190: 0000 1161 7070 6c69 6361 7469 6f6e 5769  ...applicationWi
-000011a0: 6e64 6f77 0103 0000 0030 0052 0069 0067  ndow.....0.R.i.g
-000011b0: 0075 0061 0072 0064 006f 0020 0070 0079  .u.a.r.d.o. .p.y
-000011c0: 0073 006f 0075 006e 0064 0061 006e 0061  .s.o.u.n.d.a.n.a
-000011d0: 006c 0079 0073 0065 0072 0800 0000 0006  .l.y.s.e.r......
-000011e0: 0000 0015 4162 6f75 7420 7079 736f 756e  ....About pysoun
-000011f0: 6461 6e61 6c79 7365 7207 0000 0011 6170  danalyser.....ap
-00001200: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
-00001210: 0300 0000 3400 4100 6700 6700 6900 7500  ....4.A.g.g.i.u.
-00001220: 6e00 6700 6900 2000 6f00 2000 7200 6900  n.g.i. .o. .r.i.
-00001230: 6d00 7500 6f00 7600 6900 2000 6400 6500  m.u.o.v.i. .d.e.
-00001240: 6300 6900 6200 6500 6c08 0000 0000 0600  c.i.b.e.l.......
-00001250: 0000 1841 6464 206f 7220 7375 6274 7261  ...Add or subtra
-00001260: 6374 2064 6563 6962 656c 7307 0000 0011  ct decibels.....
-00001270: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-00001280: 7701 0300 0000 2000 5400 7500 7400 7400  w..... .T.u.t.t.
-00001290: 6900 2000 6900 2000 6600 6900 6c00 6500  i. .i. .f.i.l.e.
-000012a0: 2000 2800 2a00 2908 0000 0000 0600 0000   .(.*.).........
-000012b0: 0d41 6c6c 2046 696c 6573 2028 2a29 0700  .All Files (*)..
-000012c0: 0000 1161 7070 6c69 6361 7469 6f6e 5769  ...applicationWi
-000012d0: 6e64 6f77 0103 0000 0020 0041 0075 0074  ndow..... .A.u.t
-000012e0: 006f 0063 006f 0072 0072 0065 006c 0061  .o.c.o.r.r.e.l.a
-000012f0: 007a 0069 006f 006e 0065 0800 0000 0006  .z.i.o.n.e......
-00001300: 0000 000f 4175 746f 636f 7272 656c 6174  ....Autocorrelat
-00001310: 696f 6e07 0000 0011 6170 706c 6963 6174  ion.....applicat
-00001320: 696f 6e57 696e 646f 7701 0300 0000 2200  ionWindow.....".
-00001330: 4100 7500 7400 6f00 6300 6f00 7200 7200  A.u.t.o.c.o.r.r.
-00001340: 6500 6c00 6f00 6700 7200 6100 6d00 6d00  e.l.o.g.r.a.m.m.
-00001350: 6108 0000 0000 0600 0000 0f41 7574 6f63  a..........Autoc
-00001360: 6f72 7265 6c6f 6772 616d 0700 0000 1161  orrelogram.....a
-00001370: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
-00001380: 0103 0000 0006 0042 006c 0075 0800 0000  .......B.l.u....
-00001390: 0006 0000 0004 426c 7565 0700 0000 1161  ......Blue.....a
-000013a0: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
-000013b0: 0103 0000 0010 0045 006e 0074 0072 0061  .......E.n.t.r.a
-000013c0: 006d 0062 0065 0800 0000 0006 0000 0004  .m.b.e..........
-000013d0: 426f 7468 0700 0000 1161 7070 6c69 6361  Both.....applica
-000013e0: 7469 6f6e 5769 6e64 6f77 0103 0000 008e  tionWindow......
-000013f0: 0049 006d 0070 006f 0073 0073 0069 0062  .I.m.p.o.s.s.i.b
-00001400: 0069 006c 0065 0020 0063 006f 006e 0063  .i.l.e. .c.o.n.c
-00001410: 0061 0074 0065 006e 0061 0072 0065 0020  .a.t.e.n.a.r.e. 
-00001420: 0073 0075 006f 006e 0069 0020 0063 006f  .s.u.o.n.i. .c.o
-00001430: 006e 0020 0066 0072 0065 0071 0075 0065  .n. .f.r.e.q.u.e
-00001440: 006e 007a 0065 0020 0064 0069 0020 0063  .n.z.e. .d.i. .c
-00001450: 0061 006d 0070 0069 006f 006e 0061 006d  .a.m.p.i.o.n.a.m
-00001460: 0065 006e 0074 006f 0020 0064 0069 0066  .e.n.t.o. .d.i.f
-00001470: 0066 0065 0072 0065 006e 0074 0069 0800  .f.e.r.e.n.t.i..
-00001480: 0000 0006 0000 0037 4361 6e6e 6f74 2063  .......7Cannot c
-00001490: 6f6e 6361 7465 6e61 7465 2073 6f75 6e64  oncatenate sound
-000014a0: 7320 7769 7468 2064 6966 6665 7265 6e74  s with different
-000014b0: 2073 616d 706c 696e 6720 7261 7465 7307   sampling rates.
-000014c0: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
-000014d0: 696e 646f 7701 03ff ffff ff08 0000 0000  indow...........
-000014e0: 0600 0000 3143 616e 6e6f 7420 6375 7420  ....1Cannot cut 
-000014f0: 656e 7469 7265 2073 6f75 6e64 2c20 706c  entire sound, pl
-00001500: 6561 7365 2075 7365 2072 656d 6f76 6520  ease use remove 
-00001510: 6275 7474 6f6e 0700 0000 1161 7070 6c69  button.....appli
-00001520: 6361 7469 6f6e 5769 6e64 6f77 0103 0000  cationWindow....
-00001530: 003a 0049 006d 0070 006f 0073 0073 0069  .:.I.m.p.o.s.s.i
-00001540: 0062 0069 006c 0065 0020 0061 0070 0072  .b.i.l.e. .a.p.r
-00001550: 0069 0072 0065 0020 0025 0031 0020 0049  .i.r.e. .%.1. .I
-00001560: 004f 0045 0072 0072 006f 0072 0800 0000  .O.E.r.r.o.r....
-00001570: 0006 0000 0016 4361 6e6e 6f74 206f 7065  ......Cannot ope
-00001580: 6e20 2531 2049 4f45 7272 6f72 0700 0000  n %1 IOError....
-00001590: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-000015a0: 6f77 0103 0000 008e 004e 006f 006e 0020  ow.......N.o.n. 
-000015b0: 00e8 0020 0070 006f 0073 0073 0069 0062  ... .p.o.s.s.i.b
-000015c0: 0069 006c 0065 0020 0072 0069 0070 0072  .i.l.e. .r.i.p.r
-000015d0: 006f 0064 0075 0072 0072 0065 0020 0073  .o.d.u.r.r.e. .s
-000015e0: 0075 006f 006e 0069 0020 0063 006f 006e  .u.o.n.i. .c.o.n
-000015f0: 0020 0066 0072 0065 0071 0075 0065 006e  . .f.r.e.q.u.e.n
-00001600: 007a 0061 0020 0064 0069 0020 0063 0061  .z.a. .d.i. .c.a
-00001610: 006d 0070 0069 006f 006e 0061 006d 0065  .m.p.i.o.n.a.m.e
-00001620: 006e 0074 006f 0020 0064 0069 0076 0065  .n.t.o. .d.i.v.e
-00001630: 0072 0073 0061 0800 0000 0006 0000 002e  .r.s.a..........
-00001640: 4361 6e6e 6f74 2070 6c61 7920 736f 756e  Cannot play soun
-00001650: 6473 2077 6974 6820 6469 6666 6572 656e  ds with differen
-00001660: 7420 7361 6d70 6c65 2072 6174 6573 0700  t sample rates..
-00001670: 0000 1161 7070 6c69 6361 7469 6f6e 5769  ...applicationWi
-00001680: 6e64 6f77 0103 0000 0080 0049 006d 0070  ndow.......I.m.p
-00001690: 006f 0073 0073 0069 0062 0069 006c 0065  .o.s.s.i.b.i.l.e
-000016a0: 0020 0073 0061 006c 0076 0061 0072 0065  . .s.a.l.v.a.r.e
-000016b0: 0020 0073 0075 006f 006e 0069 0020 0063  . .s.u.o.n.i. .c
-000016c0: 006f 006e 0020 0066 0072 0065 0071 0075  .o.n. .f.r.e.q.u
-000016d0: 0065 006e 007a 0065 0020 0064 0069 0020  .e.n.z.e. .d.i. 
-000016e0: 0063 0061 006d 0070 0069 006f 006e 0061  .c.a.m.p.i.o.n.a
-000016f0: 006d 0065 006e 0074 006f 0020 0064 0069  .m.e.n.t.o. .d.i
-00001700: 0076 0065 0072 0073 0065 0800 0000 0006  .v.e.r.s.e......
-00001710: 0000 002f 4361 6e6e 6f74 2077 7269 7465  .../Cannot write
-00001720: 2073 6f75 6e64 7320 7769 7468 2064 6966   sounds with dif
-00001730: 6665 7265 6e74 2073 616d 706c 6520 7261  ferent sample ra
-00001740: 7465 7307 0000 0011 6170 706c 6963 6174  tes.....applicat
-00001750: 696f 6e57 696e 646f 7701 0300 0000 0c00  ionWindow.......
-00001760: 4300 6100 6e00 6100 6c00 6508 0000 0000  C.a.n.a.l.e.....
-00001770: 0600 0000 0743 6861 6e6e 656c 0700 0000  .....Channel....
-00001780: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-00001790: 6f77 0103 0000 0032 0053 0063 0065 0067  ow.....2.S.c.e.g
-000017a0: 006c 0069 0020 0069 006c 0020 0066 0069  .l.i. .i.l. .f.i
-000017b0: 006c 0065 0020 0064 0061 0020 0073 0061  .l.e. .d.a. .s.a
-000017c0: 006c 0076 0061 0072 0065 0800 0000 0006  .l.v.a.r.e......
-000017d0: 0000 0014 4368 6f6f 7365 2066 696c 6520  ....Choose file 
-000017e0: 746f 2077 7269 7465 0700 0000 1161 7070  to write.....app
-000017f0: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
-00001800: 0000 0016 0043 006c 006f 006e 0061 0020  .....C.l.o.n.a. 
-00001810: 0073 0075 006f 006e 006f 0800 0000 0006  .s.u.o.n.o......
-00001820: 0000 000b 436c 6f6e 6520 536f 756e 6407  ....Clone Sound.
-00001830: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
-00001840: 696e 646f 7701 0300 0000 1200 4300 6f00  indow.......C.o.
-00001850: 6e00 6300 6100 7400 6500 6e00 6108 0000  n.c.a.t.e.n.a...
-00001860: 0000 0600 0000 0b43 6f6e 6361 7465 6e61  .......Concatena
-00001870: 7465 0700 0000 1161 7070 6c69 6361 7469  te.....applicati
-00001880: 6f6e 5769 6e64 6f77 0103 0000 001e 0043  onWindow.......C
-00001890: 006f 006e 0063 0061 0074 0065 006e 0061  .o.n.c.a.t.e.n.a
-000018a0: 0020 0073 0075 006f 006e 0069 0800 0000  . .s.u.o.n.i....
-000018b0: 0006 0000 0012 436f 6e63 6174 656e 6174  ......Concatenat
-000018c0: 6520 536f 756e 6473 0700 0000 1161 7070  e Sounds.....app
-000018d0: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
-000018e0: ffff ffff 0800 0000 0006 0000 0003 4375  ..............Cu
-000018f0: 7407 0000 0011 6170 706c 6963 6174 696f  t.....applicatio
-00001900: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
-00001910: 0000 0600 0000 0943 7574 2053 6f75 6e64  .......Cut Sound
-00001920: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
-00001930: 5769 6e64 6f77 0103 ffff ffff 0800 0000  Window..........
-00001940: 0006 0000 003f 4475 7261 7469 6f6e 3a20  .....?Duration: 
-00001950: 7b30 7d20 7365 632e 0a0a 4368 616e 6e65  {0} sec...Channe
-00001960: 6c3a 207b 317d 200a 0a53 616d 702e 2046  l: {1} ..Samp. F
-00001970: 7265 712e 3a20 7b32 7d20 0a0a 4269 7473  req.: {2} ..Bits
-00001980: 3a20 7b33 7d07 0000 0011 6170 706c 6963  : {3}.....applic
-00001990: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
-000019a0: 0800 4500 7300 6300 6908 0000 0000 0600  ..E.s.c.i.......
-000019b0: 0000 0445 7869 7407 0000 0011 6170 706c  ...Exit.....appl
-000019c0: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
-000019d0: 0000 0800 4500 7300 6300 6908 0000 0000  ....E.s.c.i.....
-000019e0: 0600 0000 1045 7869 7420 6170 706c 6963  .....Exit applic
-000019f0: 6174 696f 6e07 0000 0011 6170 706c 6963  ation.....applic
-00001a00: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
-00001a10: 2000 4600 4900 5200 3200 2000 5000 7200   .F.I.R.2. .P.r.
-00001a20: 6500 6400 6500 6600 6900 6e00 6900 7400  e.d.e.f.i.n.i.t.
-00001a30: 6908 0000 0000 0600 0000 0c46 4952 3220  i..........FIR2 
-00001a40: 5072 6573 6574 7307 0000 0011 6170 706c  Presets.....appl
-00001a50: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
-00001a60: 0000 0e00 5400 6f00 6e00 6f00 2000 4600  ....T.o.n.o. .F.
-00001a70: 4d08 0000 0000 0600 0000 0746 4d20 546f  M..........FM To
-00001a80: 6e65 0700 0000 1161 7070 6c69 6361 7469  ne.....applicati
-00001a90: 6f6e 5769 6e64 6f77 0103 ffff ffff 0800  onWindow........
-00001aa0: 0000 0006 0000 0010 4861 726d 6f6e 6963  ........Harmonic
-00001ab0: 2043 6f6d 706c 6578 0700 0000 1161 7070   Complex.....app
-00001ac0: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
-00001ad0: 0000 0020 0050 0069 0074 0063 0068 0020  ... .P.i.t.c.h. 
-00001ae0: 0064 0069 0020 0048 0075 0067 0067 0069  .d.i. .H.u.g.g.i
-00001af0: 006e 0073 0800 0000 0006 0000 000d 4875  .n.s..........Hu
-00001b00: 6767 696e 7320 5069 7463 6807 0000 0011  ggins Pitch.....
-00001b10: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-00001b20: 7701 0300 0000 1600 4900 5000 4400 2000  w.......I.P.D. .
-00001b30: 4c00 6900 6e00 6500 6100 7200 6508 0000  L.i.n.e.a.r.e...
-00001b40: 0000 0600 0000 0a49 5044 204c 696e 6561  .......IPD Linea
-00001b50: 7207 0000 0011 6170 706c 6963 6174 696f  r.....applicatio
-00001b60: 6e57 696e 646f 7701 0300 0000 1a00 4900  nWindow.......I.
-00001b70: 5000 4400 2000 6100 2000 7300 6300 6100  P.D. .a. .s.c.a.
-00001b80: 6c00 6900 6e00 6f08 0000 0000 0600 0000  l.i.n.o.........
-00001b90: 0b49 5044 2053 7465 7070 6564 0700 0000  .IPD Stepped....
-00001ba0: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-00001bb0: 6f77 0103 0000 0006 0049 0052 004e 0800  ow.......I.R.N..
-00001bc0: 0000 0006 0000 0003 4952 4e07 0000 0011  ........IRN.....
-00001bd0: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-00001be0: 7701 0300 0000 0600 4900 5400 4408 0000  w.......I.T.D...
-00001bf0: 0000 0600 0000 0349 5444 0700 0000 1161  .......ITD.....a
-00001c00: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
-00001c10: 0103 0000 0020 0044 0069 0061 006c 006f  ..... .D.i.a.l.o
-00001c20: 0067 006f 0020 0064 0069 0020 0069 006e  .g.o. .d.i. .i.n
-00001c30: 0070 0075 0074 0800 0000 0006 0000 000c  .p.u.t..........
-00001c40: 496e 7075 7420 4469 616c 6f67 0700 0000  Input Dialog....
-00001c50: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-00001c60: 6f77 0103 0000 0012 0045 0074 0069 0063  ow.......E.t.i.c
-00001c70: 0068 0065 0074 0074 0061 0800 0000 0006  .h.e.t.t.a......
-00001c80: 0000 0005 4c61 6265 6c07 0000 0011 6170  ....Label.....ap
-00001c90: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
-00001ca0: 0300 0000 1000 5300 6900 6e00 6900 7300  ......S.i.n.i.s.
-00001cb0: 7400 7200 6f08 0000 0000 0600 0000 044c  t.r.o..........L
-00001cc0: 6566 7407 0000 0011 6170 706c 6963 6174  eft.....applicat
-00001cd0: 696f 6e57 696e 646f 7701 0300 0000 2a00  ionWindow.....*.
-00001ce0: 4400 6900 6600 6600 6500 7200 6500 6e00  D.i.f.f.e.r.e.n.
-00001cf0: 7a00 6100 2000 6400 6900 2000 6c00 6900  z.a. .d.i. .l.i.
-00001d00: 7600 6500 6c00 6c00 6f08 0000 0000 0600  v.e.l.l.o.......
-00001d10: 0000 104c 6576 656c 2044 6966 6665 7265  ...Level Differe
-00001d20: 6e63 6507 0000 0011 6170 706c 6963 6174  nce.....applicat
-00001d30: 696f 6e57 696e 646f 7701 0300 0000 1800  ionWindow.......
-00001d40: 4300 6100 7200 6900 6300 6100 2000 7300  C.a.r.i.c.a. .s.
-00001d50: 7500 6f00 6e00 6f08 0000 0000 0600 0000  u.o.n.o.........
-00001d60: 0a4c 6f61 6420 536f 756e 6407 0000 0011  .Load Sound.....
-00001d70: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-00001d80: 7701 0300 0000 1c00 4d00 6100 6e00 7500  w.......M.a.n.u.
-00001d90: 6100 6c00 6500 2000 2800 6800 7400 6d00  a.l.e. .(.h.t.m.
-00001da0: 6c00 2908 0000 0000 0600 0000 0d4d 616e  l.)..........Man
-00001db0: 7561 6c20 2868 746d 6c29 0700 0000 1161  ual (html).....a
-00001dc0: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
-00001dd0: 0103 0000 001a 004d 0061 006e 0075 0061  .......M.a.n.u.a
-00001de0: 006c 0065 0020 0028 0070 0064 0066 0029  .l.e. .(.p.d.f.)
-00001df0: 0800 0000 0006 0000 000c 4d61 6e75 616c  ..........Manual
-00001e00: 2028 7064 6629 0700 0000 1161 7070 6c69   (pdf).....appli
-00001e10: 6361 7469 6f6e 5769 6e64 6f77 0103 ffff  cationWindow....
-00001e20: ffff 0800 0000 0006 0000 0004 4d6f 6e6f  ............Mono
-00001e30: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
-00001e40: 5769 6e64 6f77 0103 0000 0014 0053 0070  Window.......S.p
-00001e50: 006f 0073 0074 0061 0020 0067 0069 00f9  .o.s.t.a. .g.i..
-00001e60: 0800 0000 0006 0000 0009 4d6f 7665 2044  ..........Move D
-00001e70: 6f77 6e07 0000 0011 6170 706c 6963 6174  own.....applicat
-00001e80: 696f 6e57 696e 646f 7701 0300 0000 1200  ionWindow.......
-00001e90: 5300 7000 6f00 7300 7400 6100 2000 7300  S.p.o.s.t.a. .s.
-00001ea0: 7508 0000 0000 0600 0000 074d 6f76 6520  u..........Move 
-00001eb0: 5570 0700 0000 1161 7070 6c69 6361 7469  Up.....applicati
-00001ec0: 6f6e 5769 6e64 6f77 0103 0000 0024 0053  onWindow.....$.S
-00001ed0: 0065 006c 0065 007a 0069 006f 006e 0065  .e.l.e.z.i.o.n.e
-00001ee0: 0020 006d 0075 006c 0074 0069 0070 006c  . .m.u.l.t.i.p.l
-00001ef0: 0061 0800 0000 0006 0000 0012 4d75 6c74  .a..........Mult
-00001f00: 6970 6c65 2053 656c 6563 7469 6f6e 0700  iple Selection..
-00001f10: 0000 1161 7070 6c69 6361 7469 6f6e 5769  ...applicationWi
-00001f20: 6e64 6f77 0103 ffff ffff 0800 0000 0006  ndow............
-00001f30: 0000 0010 4e61 7272 6f77 6261 6e64 204e  ....Narrowband N
-00001f40: 6f69 7365 0700 0000 1161 7070 6c69 6361  oise.....applica
-00001f50: 7469 6f6e 5769 6e64 6f77 0103 0000 0016  tionWindow......
-00001f60: 004e 0075 006f 0076 006f 0020 006e 006f  .N.u.o.v.o. .n.o
-00001f70: 006d 0065 003a 0800 0000 0006 0000 0009  .m.e.:..........
-00001f80: 4e65 7720 6e61 6d65 3a07 0000 0011 6170  New name:.....ap
-00001f90: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
-00001fa0: 0300 0000 2200 4e00 6500 7300 7300 7500  ....".N.e.s.s.u.
-00001fb0: 6e00 6100 2000 7300 6500 6c00 6500 7a00  n.a. .s.e.l.e.z.
-00001fc0: 6900 6f00 6e00 6508 0000 0000 0600 0000  i.o.n.e.........
-00001fd0: 0c4e 6f20 5365 6c65 6374 696f 6e07 0000  .No Selection...
-00001fe0: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
-00001ff0: 646f 7701 0300 0000 2200 4e00 6500 7300  dow.....".N.e.s.
-00002000: 7300 7500 6e00 6100 2000 5300 6500 6c00  s.u.n.a. .S.e.l.
-00002010: 6500 7a00 6900 6f00 6e00 6508 0000 0000  e.z.i.o.n.e.....
-00002020: 0600 0000 374e 6f20 5365 6c65 6374 696f  ....7No Selectio
-00002030: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002050: 2020 2020 2020 2020 2020 2020 0700 0000              ....
-00002060: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-00002070: 6f77 0103 0000 000c 0052 0075 006d 006f  ow.......R.u.m.o
-00002080: 0072 0065 0800 0000 0006 0000 0005 4e6f  .r.e..........No
-00002090: 6973 6507 0000 0011 6170 706c 6963 6174  ise.....applicat
-000020a0: 696f 6e57 696e 646f 7701 0300 0000 0e00  ionWindow.......
-000020b0: 4e00 6500 7300 7300 7500 6e00 6f08 0000  N.e.s.s.u.n.o...
-000020c0: 0000 0600 0000 044e 6f6e 6507 0000 0011  .......None.....
-000020d0: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-000020e0: 7701 0300 0000 2400 4400 6900 7300 7000  w.....$.D.i.s.p.
-000020f0: 6100 7200 6900 2000 6100 2000 7300 6900  a.r.i. .a. .s.i.
-00002100: 6e00 6900 7300 7400 7200 6108 0000 0000  n.i.s.t.r.a.....
-00002110: 0600 0000 084f 6464 204c 6566 7407 0000  .....Odd Left...
-00002120: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
-00002130: 646f 7701 0300 0000 2000 4400 6900 7300  dow..... .D.i.s.
-00002140: 7000 6100 7200 6900 2000 6100 2000 6400  p.a.r.i. .a. .d.
-00002150: 6500 7300 7400 7200 6108 0000 0000 0600  e.s.t.r.a.......
-00002160: 0000 094f 6464 2052 6967 6874 0700 0000  ...Odd Right....
-00002170: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-00002180: 6f77 0103 0000 0050 0053 0069 0020 0070  ow.....P.S.i. .p
-00002190: 0075 00f2 0020 0073 0070 006f 0073 0074  .u... .s.p.o.s.t
-000021a0: 0061 0072 0065 0020 0073 006f 006c 006f  .a.r.e. .s.o.l.o
-000021b0: 0020 0075 006e 0020 0073 0075 006f 006e  . .u.n. .s.u.o.n
-000021c0: 006f 0020 0061 006c 006c 0061 0020 0076  .o. .a.l.l.a. .v
-000021d0: 006f 006c 0074 0061 0800 0000 0006 0000  .o.l.t.a........
-000021e0: 0025 4f6e 6c79 206f 6e65 2073 6f75 6e64  .%Only one sound
-000021f0: 2063 616e 2062 6520 6d6f 7665 6420 6174   can be moved at
-00002200: 2061 2074 696d 6507 0000 0011 6170 706c   a time.....appl
-00002210: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
-00002220: 0000 6600 5300 6900 2000 7000 7500 f200  ..f.S.i. .p.u...
-00002230: 2000 6300 6100 6d00 6200 6900 6100 7200   .c.a.m.b.i.a.r.
-00002240: 6500 2000 7300 6f00 6c00 6f00 2000 6900  e. .s.o.l.o. .i.
-00002250: 6c00 2000 6e00 6f00 6d00 6500 2000 6400  l. .n.o.m.e. .d.
-00002260: 6900 2000 7500 6e00 2000 7300 7500 6f00  i. .u.n. .s.u.o.
-00002270: 6e00 6f00 2000 6100 6c00 6c00 6100 2000  n.o. .a.l.l.a. .
-00002280: 7600 6f00 6c00 7400 6108 0000 0000 0600  v.o.l.t.a.......
-00002290: 0000 274f 6e6c 7920 6f6e 6520 736f 756e  ..'Only one soun
-000022a0: 6420 6361 6e20 6265 2072 656e 616d 6564  d can be renamed
-000022b0: 2061 7420 6120 7469 6d65 0700 0000 1161   at a time.....a
-000022c0: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
-000022d0: 0103 0000 0050 0053 0069 0020 0070 0075  .....P.S.i. .p.u
-000022e0: 00f2 0020 0063 0061 006d 0062 0069 0061  ... .c.a.m.b.i.a
-000022f0: 0072 0065 0020 0073 006f 006c 006f 0020  .r.e. .s.o.l.o. 
-00002300: 0075 006e 0020 0073 0075 006f 006e 006f  .u.n. .s.u.o.n.o
-00002310: 0020 0061 006c 006c 0061 0020 0076 006f  . .a.l.l.a. .v.o
-00002320: 006c 0074 0061 0800 0000 0006 0000 0023  .l.t.a.........#
-00002330: 4f6e 6c79 2073 6f75 6e64 2063 616e 2062  Only sound can b
-00002340: 6520 6368 616e 6765 6420 6174 2061 2074  e changed at a t
-00002350: 696d 6507 0000 0011 6170 706c 6963 6174  ime.....applicat
-00002360: 696f 6e57 696e 646f 7701 0300 0000 6400  ionWindow.....d.
-00002370: 5300 6f00 6c00 6f00 2000 6400 7500 6500  S.o.l.o. .d.u.e.
-00002380: 2000 7300 7500 6f00 6e00 6900 2000 6100   .s.u.o.n.i. .a.
-00002390: 6c00 6c00 6100 2000 7600 6f00 6c00 7400  l.l.a. .v.o.l.t.
-000023a0: 6100 2000 7000 6f00 7300 7300 6f00 6e00  a. .p.o.s.s.o.n.
-000023b0: 6f00 2000 6500 7300 7300 6500 7200 6500  o. .e.s.s.e.r.e.
-000023c0: 2000 6300 6f00 6d00 7000 6100 7200 6100   .c.o.m.p.a.r.a.
-000023d0: 7400 6908 0000 0000 0600 0000 294f 6e6c  t.i.........)Onl
-000023e0: 7920 7477 6f20 736f 756e 6473 2063 616e  y two sounds can
-000023f0: 2062 6520 636f 6d70 6172 6564 2061 7420   be compared at 
-00002400: 6120 7469 6d65 0700 0000 1161 7070 6c69  a time.....appli
-00002410: 6361 7469 6f6e 5769 6e64 6f77 0103 0000  cationWindow....
-00002420: 0068 0053 006f 006c 006f 0020 0064 0075  .h.S.o.l.o. .d.u
-00002430: 0065 0020 0073 0075 006f 006e 0069 0020  .e. .s.u.o.n.i. 
-00002440: 0061 006c 006c 0061 0020 0076 006f 006c  .a.l.l.a. .v.o.l
-00002450: 0074 0061 0020 0070 006f 0073 0073 006f  .t.a. .p.o.s.s.o
-00002460: 006e 006f 0020 0065 0073 0073 0065 0072  .n.o. .e.s.s.e.r
-00002470: 0065 0020 0063 006f 006e 0063 0061 0074  .e. .c.o.n.c.a.t
-00002480: 0065 006e 0061 0074 0069 0800 0000 0006  .e.n.a.t.i......
-00002490: 0000 002d 4f6e 6c79 2074 776f 2073 6f75  ...-Only two sou
-000024a0: 6e64 7320 6361 6e20 6265 2063 6f6e 6361  nds can be conca
-000024b0: 7465 6e61 7465 6420 6174 2061 2074 696d  tenated at a tim
-000024c0: 6507 0000 0011 6170 706c 6963 6174 696f  e.....applicatio
-000024d0: 6e57 696e 646f 7701 0300 0000 0800 5200  nWindow.......R.
-000024e0: 6f00 7300 6108 0000 0000 0600 0000 0450  o.s.a..........P
-000024f0: 696e 6b07 0000 0011 6170 706c 6963 6174  ink.....applicat
-00002500: 696f 6e57 696e 646f 7701 0300 0000 1200  ionWindow.......
-00002510: 5200 6900 7000 7200 6f00 6400 7500 6300  R.i.p.r.o.d.u.c.
-00002520: 6908 0000 0000 0600 0000 0450 6c61 7907  i..........Play.
-00002530: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
-00002540: 696e 646f 7701 0300 0000 2600 4700 7200  indow.....&.G.r.
-00002550: 6100 6600 6900 6300 6f00 2000 6f00 6e00  a.f.i.c.o. .o.n.
-00002560: 6400 6100 2000 7300 6f00 6e00 6f00 7200  d.a. .s.o.n.o.r.
-00002570: 6108 0000 0000 0600 0000 0d50 6c6f 7420  a..........Plot 
-00002580: 5761 7665 666f 726d 0700 0000 1161 7070  Waveform.....app
-00002590: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
-000025a0: 0000 0014 0050 0072 0065 0066 0065 0072  .....P.r.e.f.e.r
-000025b0: 0065 006e 007a 0065 0800 0000 0006 0000  .e.n.z.e........
-000025c0: 000b 5072 6566 6572 656e 6365 7307 0000  ..Preferences...
-000025d0: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
-000025e0: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
-000025f0: 0000 1550 7974 686f 6e20 536f 756e 6420  ...Python Sound 
-00002600: 416e 616c 7973 6572 0700 0000 1161 7070  Analyser.....app
-00002610: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
-00002620: 0000 000a 0052 006f 0073 0073 006f 0800  .....R.o.s.s.o..
-00002630: 0000 0006 0000 0003 5265 6407 0000 0011  ........Red.....
-00002640: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-00002650: 7701 0300 0000 0e00 5200 6900 6d00 7500  w.......R.i.m.u.
-00002660: 6f00 7600 6908 0000 0000 0600 0000 0652  o.v.i..........R
-00002670: 656d 6f76 6507 0000 0011 6170 706c 6963  emove.....applic
-00002680: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
-00002690: 1a00 5200 6900 6d00 7500 6f00 7600 6900  ..R.i.m.u.o.v.i.
-000026a0: 2000 7400 7500 7400 7400 6908 0000 0000   .t.u.t.t.i.....
-000026b0: 0600 0000 0a52 656d 6f76 6520 416c 6c07  .....Remove All.
-000026c0: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
-000026d0: 696e 646f 7701 0300 0000 1000 5200 6900  indow.......R.i.
-000026e0: 6e00 6f00 6d00 6900 6e00 6108 0000 0000  n.o.m.i.n.a.....
-000026f0: 0600 0000 0652 656e 616d 6507 0000 0011  .....Rename.....
-00002700: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-00002710: 7701 0300 0000 3400 4300 6100 6d00 6200  w.....4.C.a.m.b.
-00002720: 6900 6100 2000 4600 7200 6500 7100 2e00  i.a. .F.r.e.q...
-00002730: 2000 4300 6100 6d00 7000 6900 6f00 6e00   .C.a.m.p.i.o.n.
-00002740: 6100 6d00 6500 6e00 7400 6f08 0000 0000  a.m.e.n.t.o.....
-00002750: 0600 0000 0852 6573 616d 706c 6507 0000  .....Resample...
-00002760: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
-00002770: 646f 7701 0300 0000 0c00 4400 6500 7300  dow.......D.e.s.
-00002780: 7400 7200 6f08 0000 0000 0600 0000 0552  t.r.o..........R
-00002790: 6967 6874 0700 0000 1161 7070 6c69 6361  ight.....applica
-000027a0: 7469 6f6e 5769 6e64 6f77 0103 ffff ffff  tionWindow......
-000027b0: 0800 0000 0006 0000 0010 526f 6f74 204d  ..........Root M
-000027c0: 6561 6e20 5371 7561 7265 0700 0000 1161  ean Square.....a
-000027d0: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
-000027e0: 0103 0000 0014 0053 0061 006c 0076 0061  .......S.a.l.v.a
-000027f0: 0020 0063 006f 006d 0065 0800 0000 0006  . .c.o.m.e......
-00002800: 0000 0007 5361 7665 2041 7307 0000 0011  ....Save As.....
-00002810: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-00002820: 7701 0300 0000 0e00 5300 6300 6100 6c00  w.......S.c.a.l.
-00002830: 6100 7200 6508 0000 0000 0600 0000 0553  a.r.e..........S
-00002840: 6361 6c65 0700 0000 1161 7070 6c69 6361  cale.....applica
-00002850: 7469 6f6e 5769 6e64 6f77 0103 0000 0024  tionWindow.....$
-00002860: 0053 0063 0061 006c 0061 0072 0065 0020  .S.c.a.l.a.r.e. 
-00002870: 0069 006c 0020 006c 0069 0076 0065 006c  .i.l. .l.i.v.e.l
-00002880: 006c 006f 0800 0000 0006 0000 000b 5363  .l.o..........Sc
-00002890: 616c 6520 4c65 7665 6c07 0000 0011 6170  ale Level.....ap
-000028a0: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
-000028b0: 0300 0000 1e00 5300 6500 6c00 6500 7a00  ......S.e.l.e.z.
-000028c0: 6900 6f00 6e00 6100 2000 7400 7500 7400  i.o.n.a. .t.u.t.
-000028d0: 7400 6908 0000 0000 0600 0000 0a53 656c  t.i..........Sel
-000028e0: 6563 7420 416c 6c07 0000 0011 6170 706c  ect All.....appl
-000028f0: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
-00002900: 0000 1000 5300 6900 6c00 6500 6e00 7a00  ....S.i.l.e.n.z.
-00002910: 6900 6f08 0000 0000 0600 0000 0753 696c  i.o..........Sil
-00002920: 656e 6365 0700 0000 1161 7070 6c69 6361  ence.....applica
-00002930: 7469 6f6e 5769 6e64 6f77 0103 0000 0012  tionWindow......
-00002940: 0053 0069 006e 0075 0073 006f 0069 0064  .S.i.n.u.s.o.i.d
-00002950: 0065 0800 0000 0006 0000 0008 5369 6e75  .e..........Sinu
-00002960: 736f 6964 0700 0000 1161 7070 6c69 6361  soid.....applica
-00002970: 7469 6f6e 5769 6e64 6f77 0103 0000 001a  tionWindow......
-00002980: 0053 0070 0065 0074 0074 0072 006f 0067  .S.p.e.t.t.r.o.g
-00002990: 0072 0061 006d 006d 0061 0800 0000 0006  .r.a.m.m.a......
-000029a0: 0000 000b 5370 6563 7472 6f67 7261 6d07  ....Spectrogram.
-000029b0: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
-000029c0: 696e 646f 7701 0300 0000 0e00 5300 7000  indow.......S.p.
-000029d0: 6500 7400 7400 7200 6f08 0000 0000 0600  e.t.t.r.o.......
-000029e0: 0000 0853 7065 6374 7275 6d07 0000 0011  ...Spectrum.....
-000029f0: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
-00002a00: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
-00002a10: 2c53 7570 706f 7274 6564 2053 6f75 6e64  ,Supported Sound
-00002a20: 2046 696c 6573 2028 2a2e 7761 7629 3b3b   Files (*.wav);;
-00002a30: 416c 6c20 4669 6c65 7320 282a 2907 0000  All Files (*)...
-00002a40: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
-00002a50: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
-00002a60: 0000 1356 616c 7565 7320 6f75 7420 6f66  ...Values out of
-00002a70: 2072 616e 6765 0700 0000 1161 7070 6c69   range.....appli
-00002a80: 6361 7469 6f6e 5769 6e64 6f77 0103 0000  cationWindow....
-00002a90: 000a 0056 0069 006f 006c 0061 0800 0000  ...V.i.o.l.a....
-00002aa0: 0006 0000 0006 5669 6f6c 6574 0700 0000  ......Violet....
-00002ab0: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-00002ac0: 6f77 0103 0000 000c 0041 0076 0076 0069  ow.......A.v.v.i
-00002ad0: 0073 006f 0800 0000 0006 0000 0007 5761  .s.o..........Wa
-00002ae0: 726e 696e 6707 0000 0011 6170 706c 6963  rning.....applic
-00002af0: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
-00002b00: 1600 4f00 6e00 6400 6100 2000 7300 6f00  ..O.n.d.a. .s.o.
-00002b10: 6e00 6f00 7200 6108 0000 0000 0600 0000  n.o.r.a.........
-00002b20: 0857 6176 6566 6f72 6d07 0000 0011 6170  .Waveform.....ap
-00002b30: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
-00002b40: 0300 0000 0c00 4200 6900 6100 6e00 6300  ......B.i.a.n.c.
-00002b50: 6f08 0000 0000 0600 0000 0557 6869 7465  o..........White
-00002b60: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
-00002b70: 5769 6e64 6f77 0103 0000 0014 0070 0061  Window.......p.a
-00002b80: 0073 0073 0061 0062 0061 006e 0064 0061  .s.s.a.b.a.n.d.a
-00002b90: 0800 0000 0006 0000 0008 6261 6e64 7061  ..........bandpa
-00002ba0: 7373 0700 0000 1161 7070 6c69 6361 7469  ss.....applicati
-00002bb0: 6f6e 5769 6e64 6f77 0103 0000 0014 0066  onWindow.......f
-00002bc0: 0065 0072 006d 0061 0062 0061 006e 0064  .e.r.m.a.b.a.n.d
-00002bd0: 0061 0800 0000 0006 0000 0008 6261 6e64  .a..........band
-00002be0: 7374 6f70 0700 0000 1161 7070 6c69 6361  stop.....applica
-00002bf0: 7469 6f6e 5769 6e64 6f77 0103 0000 0012  tionWindow......
-00002c00: 0070 0061 0073 0073 0061 0061 006c 0074  .p.a.s.s.a.a.l.t
-00002c10: 006f 0800 0000 0006 0000 0008 6869 6768  .o..........high
-00002c20: 7061 7373 0700 0000 1161 7070 6c69 6361  pass.....applica
-00002c30: 7469 6f6e 5769 6e64 6f77 0103 0000 0014  tionWindow......
-00002c40: 0070 0061 0073 0073 0061 0062 0061 0073  .p.a.s.s.a.b.a.s
-00002c50: 0073 006f 0800 0000 0006 0000 0007 6c6f  .s.o..........lo
-00002c60: 7770 6173 7307 0000 0011 6170 706c 6963  wpass.....applic
-00002c70: 6174 696f 6e57 696e 646f 7701 03ff ffff  ationWindow.....
-00002c80: ff08 0000 0000 0600 0000 046e 6f6e 6507  ...........none.
-00002c90: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
-00002ca0: 696e 646f 7701 0300 0000 5200 7000 7900  indow.....R.p.y.
-00002cb0: 7300 6f00 7500 6e00 6400 6100 6e00 6100  s.o.u.n.d.a.n.a.
-00002cc0: 6c00 7900 7300 6500 7200 2000 2d00 2000  l.y.s.e.r. .-. .
-00002cd0: 5300 6300 6500 6700 6c00 6900 2000 6600  S.c.e.g.l.i. .f.
-00002ce0: 6900 6c00 6500 2000 6400 6100 2000 6300  i.l.e. .d.a. .c.
-00002cf0: 6100 7200 6900 6300 6100 7200 6508 0000  a.r.i.c.a.r.e...
-00002d00: 0000 0600 0000 2570 7973 6f75 6e64 616e  ......%pysoundan
-00002d10: 616c 7973 6572 202d 2043 686f 6f73 6520  alyser - Choose 
-00002d20: 6669 6c65 2074 6f20 6c6f 6164 0700 0000  file to load....
-00002d30: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
-00002d40: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
-00002d50: 001e 7b30 7d20 6973 200a 207b 317d 207b  ..{0} is . {1} {
-00002d60: 327d 2064 4220 7468 616e 200a 207b 337d  2} dB than . {3}
-00002d70: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
-00002d80: 5769 6e64 6f77 0103 ffff ffff 0800 0000  Window..........
-00002d90: 0006 0000 001a 7b30 7d20 6973 207b 317d  ......{0} is {1}
-00002da0: 207b 327d 2064 4220 7468 616e 207b 337d   {2} dB than {3}
-00002db0: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
-00002dc0: 5769 6e64 6f77 0103 ffff ffff 0800 0000  Window..........
-00002dd0: 0006 0000 000f 7b30 7d20 7b31 7d20 3a20  ......{0} {1} : 
-00002de0: 7b32 7d20 0a07 0000 0011 6170 706c 6963  {2} ......applic
-00002df0: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
-00002e00: 2800 4100 7000 7000 6c00 6900 6300 6100  (.A.p.p.l.i.c.a.
-00002e10: 2000 6c00 6500 2000 6d00 6f00 6400 6900   .l.e. .m.o.d.i.
-00002e20: 6600 6900 6300 6800 6508 0000 0000 0600  f.i.c.h.e.......
-00002e30: 0000 0d41 7070 6c79 2043 6861 6e67 6573  ...Apply Changes
-00002e40: 0700 0000 0c61 7070 6c79 4368 616e 6765  .....applyChange
-00002e50: 7301 0300 0000 6c00 4300 6900 2000 7300  s.....l.C.i. .s.
-00002e60: 6f00 6e00 6f00 2000 6d00 6f00 6400 6900  o.n.o. .m.o.d.i.
-00002e70: 6600 6900 6300 6800 6500 2000 6e00 6f00  f.i.c.h.e. .n.o.
-00002e80: 6e00 2000 7300 6100 6c00 7600 6100 7400  n. .s.a.l.v.a.t.
-00002e90: 6500 2e00 2000 4100 7000 7000 6c00 6900  e... .A.p.p.l.i.
-00002ea0: 6300 6100 7200 6500 2000 6c00 6500 2000  c.a.r.e. .l.e. .
-00002eb0: 6d00 6f00 6400 6900 6600 6900 6300 6800  m.o.d.i.f.i.c.h.
-00002ec0: 6500 3f08 0000 0000 0600 0000 2954 6865  e.?.........)The
-00002ed0: 7265 2061 7265 2075 6e73 6176 6564 2063  re are unsaved c
-00002ee0: 6861 6e67 6573 2e20 4170 706c 7920 4368  hanges. Apply Ch
-00002ef0: 616e 6765 733f 0700 0000 0c61 7070 6c79  anges?.....apply
-00002f00: 4368 616e 6765 7301 0300 0000 1c00 4100  Changes.......A.
-00002f10: 7000 7000 6c00 6900 6300 6100 2000 4600  p.p.l.i.c.a. .F.
-00002f20: 6900 6c00 7400 7200 6f08 0000 0000 0600  i.l.t.r.o.......
-00002f30: 0000 0c41 7070 6c79 2046 696c 7465 7207  ...Apply Filter.
-00002f40: 0000 0016 6170 706c 7946 4952 3250 7265  ....applyFIR2Pre
-00002f50: 7365 7473 4469 616c 6f67 0103 0000 000e  setsDialog......
-00002f60: 0043 0075 0074 006f 0066 0066 003a 0800  .C.u.t.o.f.f.:..
-00002f70: 0000 0006 0000 0008 4375 746f 6666 3a20  ........Cutoff: 
-00002f80: 0700 0000 1661 7070 6c79 4649 5232 5072  .....applyFIR2Pr
-00002f90: 6573 6574 7344 6961 6c6f 6701 03ff ffff  esetsDialog.....
-00002fa0: ff08 0000 0000 0600 0000 1e45 6e64 2054  ...........End T
-00002fb0: 7261 6e73 6974 696f 6e20 4261 6e64 203d  ransition Band =
-00002fc0: 2043 7574 6f66 6620 2a07 0000 0016 6170   Cutoff *.....ap
-00002fd0: 706c 7946 4952 3250 7265 7365 7473 4469  plyFIR2PresetsDi
-00002fe0: 616c 6f67 0103 0000 001c 004f 0072 0064  alog.......O.r.d
-00002ff0: 0069 006e 0065 0020 0066 0069 006c 0074  .i.n.e. .f.i.l.t
-00003000: 0072 006f 003a 0800 0000 0006 0000 000e  .r.o.:..........
-00003010: 4669 6c74 6572 204f 7264 6572 3a20 0700  Filter Order: ..
-00003020: 0000 1661 7070 6c79 4649 5232 5072 6573  ...applyFIR2Pres
-00003030: 6574 7344 6961 6c6f 6701 0300 0000 1e00  etsDialog.......
-00003040: 5400 6900 7000 6f00 2000 6400 6900 2000  T.i.p.o. .d.i. .
-00003050: 6600 6900 6c00 7400 7200 6f00 3a08 0000  f.i.l.t.r.o.:...
-00003060: 0000 0600 0000 0d46 696c 7465 7220 5479  .......Filter Ty
-00003070: 7065 3a20 0700 0000 1661 7070 6c79 4649  pe: .....applyFI
-00003080: 5232 5072 6573 6574 7344 6961 6c6f 6701  R2PresetsDialog.
-00003090: 0300 0000 2200 4300 7500 7400 6f00 6600  ....".C.u.t.o.f.
-000030a0: 6600 2000 7300 7500 7000 6500 7200 6900  f. .s.u.p.e.r.i.
-000030b0: 6f00 7200 6500 3a08 0000 0000 0600 0000  o.r.e.:.........
-000030c0: 0f48 6967 6865 7220 4375 746f 6666 3a20  .Higher Cutoff: 
-000030d0: 0700 0000 1661 7070 6c79 4649 5232 5072  .....applyFIR2Pr
-000030e0: 6573 6574 7344 6961 6c6f 6701 0300 0000  esetsDialog.....
-000030f0: 2200 4300 7500 7400 6f00 6600 6600 2000  ".C.u.t.o.f.f. .
-00003100: 6900 6e00 6600 6500 7200 6900 6f00 7200  i.n.f.e.r.i.o.r.
-00003110: 6500 3a08 0000 0000 0600 0000 0e4c 6f77  e.:..........Low
-00003120: 6572 2043 7574 6f66 663a 2007 0000 0016  er Cutoff: .....
-00003130: 6170 706c 7946 4952 3250 7265 7365 7473  applyFIR2Presets
-00003140: 4469 616c 6f67 0103 0000 004a 0049 006e  Dialog.....J.I.n
-00003150: 0069 007a 0069 006f 0020 0062 0061 006e  .i.z.i.o. .b.a.n
-00003160: 0064 0061 0020 0064 0069 0020 0074 0072  .d.a. .d.i. .t.r
-00003170: 0061 006e 0073 0069 007a 0069 006f 006e  .a.n.s.i.z.i.o.n
-00003180: 0065 0020 003d 0020 0043 0075 0074 006f  .e. .=. .C.u.t.o
-00003190: 0066 0066 002a 0800 0000 0006 0000 0020  .f.f.*......... 
-000031a0: 5374 6172 7420 5472 616e 7369 7469 6f6e  Start Transition
-000031b0: 2042 616e 6420 3d20 4375 746f 6666 202a   Band = Cutoff *
-000031c0: 0700 0000 1661 7070 6c79 4649 5232 5072  .....applyFIR2Pr
-000031d0: 6573 6574 7344 6961 6c6f 6701 0300 0000  esetsDialog.....
-000031e0: 1400 7000 6100 7300 7300 6100 6200 6100  ..p.a.s.s.a.b.a.
-000031f0: 6e00 6400 6108 0000 0000 0600 0000 0862  n.d.a..........b
-00003200: 616e 6470 6173 7307 0000 0016 6170 706c  andpass.....appl
-00003210: 7946 4952 3250 7265 7365 7473 4469 616c  yFIR2PresetsDial
-00003220: 6f67 0103 0000 0014 0066 0065 0072 006d  og.......f.e.r.m
-00003230: 0061 0062 0061 006e 0064 0061 0800 0000  .a.b.a.n.d.a....
-00003240: 0006 0000 0008 6261 6e64 7374 6f70 0700  ......bandstop..
-00003250: 0000 1661 7070 6c79 4649 5232 5072 6573  ...applyFIR2Pres
-00003260: 6574 7344 6961 6c6f 6701 0300 0000 1200  etsDialog.......
-00003270: 7000 6100 7300 7300 6100 6100 6c00 7400  p.a.s.s.a.a.l.t.
-00003280: 6f08 0000 0000 0600 0000 0868 6967 6870  o..........highp
-00003290: 6173 7307 0000 0016 6170 706c 7946 4952  ass.....applyFIR
-000032a0: 3250 7265 7365 7473 4469 616c 6f67 0103  2PresetsDialog..
-000032b0: 0000 0014 0070 0061 0073 0073 0061 0062  .....p.a.s.s.a.b
-000032c0: 0061 0073 0073 006f 0800 0000 0006 0000  .a.s.s.o........
-000032d0: 0007 6c6f 7770 6173 7307 0000 0016 6170  ..lowpass.....ap
-000032e0: 706c 7946 4952 3250 7265 7365 7473 4469  plyFIR2PresetsDi
-000032f0: 616c 6f67 0103 0000 001a 004d 0061 0070  alog.......M.a.p
-00003300: 0070 0061 0020 0063 006f 006c 006f 0072  .p.a. .c.o.l.o.r
-00003310: 0069 003a 0800 0000 0006 0000 000a 436f  .i.:..........Co
-00003320: 6c6f 7220 4d61 703a 0700 0000 1361 7574  lor Map:.....aut
-00003330: 6f63 6f72 7265 6c6f 6772 616d 506c 6f74  ocorrelogramPlot
-00003340: 0103 0000 0026 0053 006f 0076 0072 0061  .....&.S.o.v.r.a
-00003350: 0070 0070 006f 0073 0069 007a 0069 006f  .p.p.o.s.i.z.i.o
-00003360: 006e 0065 0020 0028 0025 0029 0800 0000  .n.e. .(.%.)....
-00003370: 0006 0000 000b 4f76 6572 6c61 7020 2825  ......Overlap (%
-00003380: 2907 0000 0013 6175 746f 636f 7272 656c  ).....autocorrel
-00003390: 6f67 7261 6d50 6c6f 7401 0300 0000 2600  ogramPlot.....&.
-000033a0: 4400 7500 7200 6100 7400 6100 2000 4600  D.u.r.a.t.a. .F.
-000033b0: 6900 6e00 6500 7300 7400 7200 6100 2000  i.n.e.s.t.r.a. .
-000033c0: 2800 7300 2908 0000 0000 0600 0000 1157  (.s.)..........W
-000033d0: 696e 646f 7720 4c65 6e67 7468 2028 7329  indow Length (s)
-000033e0: 0700 0000 1361 7574 6f63 6f72 7265 6c6f  .....autocorrelo
-000033f0: 6772 616d 506c 6f74 0103 0000 0012 0046  gramPlot.......F
-00003400: 0069 006e 0065 0073 0074 0072 0061 003a  .i.n.e.s.t.r.a.:
-00003410: 0800 0000 0006 0000 0007 5769 6e64 6f77  ..........Window
-00003420: 3a07 0000 0013 6175 746f 636f 7272 656c  :.....autocorrel
-00003430: 6f67 7261 6d50 6c6f 7401 0300 0000 1a00  ogramPlot.......
-00003440: 4300 6100 6d00 6200 6900 6100 2000 6300  C.a.m.b.i.a. .c.
-00003450: 6100 6e00 6100 6c00 6508 0000 0000 0600  a.n.a.l.e.......
-00003460: 0000 0e43 6861 6e67 6520 4368 616e 6e65  ...Change Channe
-00003470: 6c07 0000 0013 6368 616e 6765 4368 616e  l.....changeChan
-00003480: 6e65 6c44 6961 6c6f 6701 0300 0000 0e00  nelDialog.......
-00003490: 4300 6100 6e00 6100 6c00 6500 3a08 0000  C.a.n.a.l.e.:...
-000034a0: 0000 0600 0000 0943 6861 6e6e 656c 3a20  .......Channel: 
-000034b0: 0700 0000 1363 6861 6e67 6543 6861 6e6e  .....changeChann
-000034c0: 656c 4469 616c 6f67 0103 0000 0010 0053  elDialog.......S
-000034d0: 0069 006e 0069 0073 0074 0072 006f 0800  .i.n.i.s.t.r.o..
-000034e0: 0000 0006 0000 0004 4c65 6674 0700 0000  ........Left....
-000034f0: 1363 6861 6e67 6543 6861 6e6e 656c 4469  .changeChannelDi
-00003500: 616c 6f67 0103 0000 000c 0044 0065 0073  alog.......D.e.s
-00003510: 0074 0072 006f 0800 0000 0006 0000 0005  .t.r.o..........
-00003520: 5269 6768 7407 0000 0013 6368 616e 6765  Right.....change
-00003530: 4368 616e 6e65 6c44 6961 6c6f 6701 0300  ChannelDialog...
-00003540: 0000 1200 4300 6f00 6e00 6300 6100 7400  ....C.o.n.c.a.t.
-00003550: 6500 6e00 6108 0000 0000 0600 0000 0b43  e.n.a..........C
-00003560: 6f6e 6361 7465 6e61 7465 0700 0000 1163  oncatenate.....c
-00003570: 6f6e 6361 7465 6e61 7465 4469 616c 6f67  oncatenateDialog
-00003580: 0103 0000 0020 0049 006e 0074 0065 0072  ..... .I.n.t.e.r
-00003590: 0076 0061 006c 006c 006f 0020 0028 006d  .v.a.l.l.o. .(.m
-000035a0: 0073 0029 003a 0800 0000 0006 0000 000c  .s.).:..........
-000035b0: 4465 6c61 7920 286d 7329 3a20 0700 0000  Delay (ms): ....
-000035c0: 1163 6f6e 6361 7465 6e61 7465 4469 616c  .concatenateDial
-000035d0: 6f67 0103 0000 0026 0054 0069 0070 006f  og.....&.T.i.p.o
-000035e0: 0020 0064 0069 0020 0069 006e 0074 0065  . .d.i. .i.n.t.e
-000035f0: 0072 0076 0061 006c 006c 006f 003a 0800  .r.v.a.l.l.o.:..
-00003600: 0000 0006 0000 000c 4465 6c61 7920 5479  ........Delay Ty
-00003610: 7065 3a20 0700 0000 1163 6f6e 6361 7465  pe: .....concate
-00003620: 6e61 7465 4469 616c 6f67 0103 0000 0010  nateDialog......
-00003630: 0053 0069 006e 0069 0073 0074 0072 006f  .S.i.n.i.s.t.r.o
-00003640: 0800 0000 0006 0000 0004 4c65 6674 0700  ..........Left..
-00003650: 0000 1163 6f6e 6361 7465 6e61 7465 4469  ...concatenateDi
-00003660: 616c 6f67 0103 0000 001c 0043 0061 006e  alog.......C.a.n
-00003670: 0061 006c 0065 0020 006f 0075 0074 0070  .a.l.e. .o.u.t.p
-00003680: 0075 0074 003a 0800 0000 0006 0000 0010  .u.t.:..........
-00003690: 4f75 7470 7574 2043 6861 6e6e 656c 3a20  Output Channel: 
-000036a0: 0700 0000 1163 6f6e 6361 7465 6e61 7465  .....concatenate
-000036b0: 4469 616c 6f67 0103 0000 000c 0044 0065  Dialog.......D.e
-000036c0: 0073 0074 0072 006f 0800 0000 0006 0000  .s.t.r.o........
-000036d0: 0005 5269 6768 7407 0000 0011 636f 6e63  ..Right.....conc
-000036e0: 6174 656e 6174 6544 6961 6c6f 6701 0300  atenateDialog...
-000036f0: 0000 1000 5300 7500 6f00 6e00 6f00 2000  ....S.u.o.n.o. .
-00003700: 3100 3a08 0000 0000 0600 0000 0953 6f75  1.:..........Sou
-00003710: 6e64 2031 3a20 0700 0000 1163 6f6e 6361  nd 1: .....conca
-00003720: 7465 6e61 7465 4469 616c 6f67 0103 0000  tenateDialog....
-00003730: 0010 0053 0075 006f 006e 006f 0020 0032  ...S.u.o.n.o. .2
-00003740: 003a 0800 0000 0006 0000 0009 536f 756e  .:..........Soun
-00003750: 6420 323a 2007 0000 0011 636f 6e63 6174  d 2: .....concat
-00003760: 656e 6174 6544 6961 6c6f 6701 0300 0000  enateDialog.....
-00003770: 1600 4e00 6f00 6d00 6500 2000 5300 7500  ..N.o.m.e. .S.u.
-00003780: 6f00 6e00 6f00 3a08 0000 0000 0600 0000  o.n.o.:.........
-00003790: 0d53 6f75 6e64 204c 6162 656c 3a20 0700  .Sound Label: ..
-000037a0: 0000 1163 6f6e 6361 7465 6e61 7465 4469  ...concatenateDi
-000037b0: 616c 6f67 0103 0000 001e 0053 0063 0061  alog.......S.c.a
-000037c0: 006d 0062 0069 0061 0020 0069 0020 0073  .m.b.i.a. .i. .s
-000037d0: 0075 006f 006e 0069 0800 0000 0006 0000  .u.o.n.i........
-000037e0: 000b 5377 6170 2053 6f75 6e64 7307 0000  ..Swap Sounds...
-000037f0: 0011 636f 6e63 6174 656e 6174 6544 6961  ..concatenateDia
-00003800: 6c6f 6701 0300 0000 3c00 4c00 6100 7200  log.....<.L.a.r.
-00003810: 6700 6800 6500 7a00 7a00 6100 2000 6400  g.h.e.z.z.a. .d.
-00003820: 6900 2000 6200 6100 6e00 6400 6100 2000  i. .b.a.n.d.a. .
-00003830: 2800 6300 6500 6e00 7400 6500 7300 6900  (.c.e.n.t.e.s.i.
-00003840: 6d00 6900 2908 0000 0000 0600 0000 1142  m.i.)..........B
-00003850: 616e 6477 6964 7468 2028 4365 6e74 7329  andwidth (Cents)
-00003860: 0700 0000 0664 6961 6c6f 6701 0300 0000  .....dialog.....
-00003870: 2e00 4c00 6100 7200 6700 6800 6500 7a00  ..L.a.r.g.h.e.z.
-00003880: 7a00 6100 2000 6400 6900 2000 6200 6100  z.a. .d.i. .b.a.
-00003890: 6e00 6400 6100 2000 2800 4800 7a00 2908  n.d.a. .(.H.z.).
-000038a0: 0000 0000 0600 0000 0e42 616e 6477 6964  .........Bandwid
-000038b0: 7468 2028 487a 2907 0000 0006 6469 616c  th (Hz).....dial
-000038c0: 6f67 0103 0000 0036 004c 0069 0076 0065  og.....6.L.i.v.e
-000038d0: 006c 006c 006f 0020 0063 006f 006d 0070  .l.l.o. .c.o.m.p
-000038e0: 006f 006e 0065 006e 0074 0065 0020 0028  .o.n.e.n.t.e. .(
-000038f0: 0064 0042 0020 0053 0050 004c 0029 0800  .d.B. .S.P.L.)..
-00003900: 0000 0006 0000 0018 436f 6d70 6f6e 656e  ........Componen
-00003910: 7420 4c65 7665 6c20 2864 4220 5350 4c29  t Level (dB SPL)
-00003920: 0700 0000 0664 6961 6c6f 6701 0300 0000  .....dialog.....
-00003930: 2800 4400 6900 6600 6600 6500 7200 6500  (.D.i.f.f.e.r.e.
-00003940: 6e00 7a00 6100 2000 6400 6900 6300 6f00  n.z.a. .d.i.c.o.
-00003950: 7400 6900 6300 6100 3a08 0000 0000 0600  t.i.c.a.:.......
-00003960: 0000 1444 6963 686f 7469 6320 4469 6666  ...Dichotic Diff
-00003970: 6572 656e 6365 3a07 0000 0006 6469 616c  erence:.....dial
-00003980: 6f67 0103 0000 0016 0044 0075 0072 0061  og.......D.u.r.a
-00003990: 0074 0061 0020 0028 006d 0073 0029 0800  .t.a. .(.m.s.)..
-000039a0: 0000 0006 0000 000d 4475 7261 7469 6f6e  ........Duration
-000039b0: 2028 6d73 2907 0000 0006 6469 616c 6f67   (ms).....dialog
-000039c0: 0103 0000 0012 004f 0072 0065 0063 0063  .......O.r.e.c.c
-000039d0: 0068 0069 006f 003a 0800 0000 0006 0000  .h.i.o.:........
-000039e0: 0004 4561 723a 0700 0000 0664 6961 6c6f  ..Ear:.....dialo
-000039f0: 6701 0300 0000 0e00 4600 3000 2000 2800  g.......F.0. .(.
-00003a00: 4800 7a00 2908 0000 0000 0600 0000 0746  H.z.)..........F
-00003a10: 3020 2848 7a29 0700 0000 0664 6961 6c6f  0 (Hz).....dialo
-00003a20: 6701 0300 0000 1c00 4600 7200 6500 7100  g.......F.r.e.q.
-00003a30: 7500 6500 6e00 7a00 6100 2000 2800 4800  u.e.n.z.a. .(.H.
-00003a40: 7a00 2908 0000 0000 0600 0000 0e46 7265  z.)..........Fre
-00003a50: 7175 656e 6379 2028 487a 2907 0000 0006  quency (Hz).....
-00003a60: 6469 616c 6f67 0103 0000 0008 0047 0061  dialog.......G.a
-00003a70: 0069 006e 0800 0000 0006 0000 0004 4761  .i.n..........Ga
-00003a80: 696e 0700 0000 0664 6961 6c6f 6701 0300  in.....dialog...
-00003a90: 0000 3200 4c00 6900 7600 6500 6c00 6c00  ..2.L.i.v.e.l.l.
-00003aa0: 6f00 2000 6100 7200 6d00 6f00 6e00 6900  o. .a.r.m.o.n.i.
-00003ab0: 6300 6f00 2000 2800 6400 4200 2000 5300  c.o. .(.d.B. .S.
-00003ac0: 5000 4c00 2908 0000 0000 0600 0000 1748  P.L.)..........H
-00003ad0: 6172 6d6f 6e69 6320 4c65 7665 6c20 2864  armonic Level (d
-00003ae0: 4220 5350 4c29 0700 0000 0664 6961 6c6f  B SPL).....dialo
-00003af0: 6701 0300 0000 3e00 4900 6e00 7400 6500  g.....>.I.n.t.e.
-00003b00: 7200 7600 6100 6c00 6c00 6f00 2000 6100  r.v.a.l.l.o. .a.
-00003b10: 7200 6d00 6f00 6e00 6900 6300 6f00 2000  r.m.o.n.i.c.o. .
-00003b20: 2800 6300 6500 6e00 7400 6500 7300 6900  (.c.e.n.t.e.s.i.
-00003b30: 6d00 6900 2908 0000 0000 0600 0000 1848  m.i.)..........H
-00003b40: 6172 6d6f 6e69 6320 5370 6163 696e 6720  armonic Spacing 
-00003b50: 2843 656e 7473 2907 0000 0006 6469 616c  (Cents).....dial
-00003b60: 6f67 0103 0000 0016 0041 0072 006d 006f  og.......A.r.m.o
-00003b70: 006e 0069 0063 0069 0074 00e0 003a 0800  .n.i.c.i.t...:..
-00003b80: 0000 0006 0000 000c 4861 726d 6f6e 6963  ........Harmonic
-00003b90: 6974 793a 0700 0000 0664 6961 6c6f 6701  ity:.....dialog.
-00003ba0: 0300 0000 3000 4600 7200 6500 7100 7500  ....0.F.r.e.q.u.
-00003bb0: 6500 6e00 7a00 6100 2000 7300 7500 7000  e.n.z.a. .s.u.p.
-00003bc0: 6500 7200 6900 6f00 7200 6500 2000 2800  e.r.i.o.r.e. .(.
-00003bd0: 4800 7a00 2908 0000 0000 0600 0000 0f48  H.z.)..........H
-00003be0: 6967 6820 4672 6571 2e20 2848 7a29 0700  igh Freq. (Hz)..
-00003bf0: 0000 0664 6961 6c6f 6701 0300 0000 2400  ...dialog.....$.
-00003c00: 4100 7200 6d00 6f00 6e00 6900 6300 6100  A.r.m.o.n.i.c.a.
-00003c10: 2000 7300 7500 7000 6500 7200 6900 6f00   .s.u.p.e.r.i.o.
-00003c20: 7200 6508 0000 0000 0600 0000 0d48 6967  r.e..........Hig
-00003c30: 6820 4861 726d 6f6e 6963 0700 0000 0664  h Harmonic.....d
-00003c40: 6961 6c6f 6701 0300 0000 1c00 5300 7400  ialog.......S.t.
-00003c50: 6f00 7000 2000 7300 7500 7000 6500 7200  o.p. .s.u.p.e.r.
-00003c60: 6900 6f00 7200 6508 0000 0000 0600 0000  i.o.r.e.........
-00003c70: 0948 6967 6820 5374 6f70 0700 0000 0664  .High Stop.....d
-00003c80: 6961 6c6f 6701 0300 0000 1c00 4900 5000  ialog.......I.P.
-00003c90: 4400 2000 2800 7200 6100 6400 6900 6100  D. .(.r.a.d.i.a.
-00003ca0: 6e00 7400 6900 2908 0000 0000 0600 0000  n.t.i.).........
-00003cb0: 0d49 5044 2028 7261 6469 616e 7329 0700  .IPD (radians)..
-00003cc0: 0000 0664 6961 6c6f 6701 0300 0000 1200  ...dialog.......
-00003cd0: 5400 6900 7000 6f00 2000 4900 5200 4e00  T.i.p.o. .I.R.N.
-00003ce0: 3a08 0000 0000 0600 0000 0949 524e 2054  :..........IRN T
-00003cf0: 7970 653a 0700 0000 0664 6961 6c6f 6701  ype:.....dialog.
-00003d00: 0300 0000 1a00 4900 5400 4400 2000 2800  ......I.T.D. .(.
-00003d10: 6d00 6900 6300 7200 6f00 2000 7300 2908  m.i.c.r.o. .s.).
-00003d20: 0000 0000 0600 0000 0d49 5444 2028 6d69  .........ITD (mi
-00003d30: 6372 6f20 7329 0700 0000 0664 6961 6c6f  cro s).....dialo
-00003d40: 6701 0300 0000 1400 4900 7400 6500 7200  g.......I.t.e.r.
-00003d50: 6100 7a00 6900 6f00 6e00 6908 0000 0000  a.z.i.o.n.i.....
-00003d60: 0600 0000 0a49 7465 7261 7469 6f6e 7307  .....Iterations.
-00003d70: 0000 0006 6469 616c 6f67 0103 0000 0030  ....dialog.....0
-00003d80: 0046 0072 0065 0071 0075 0065 006e 007a  .F.r.e.q.u.e.n.z
-00003d90: 0061 0020 0069 006e 0066 0065 0072 0069  .a. .i.n.f.e.r.i
-00003da0: 006f 0072 0065 0020 0028 0048 007a 0029  .o.r.e. .(.H.z.)
-00003db0: 0800 0000 0006 0000 000e 4c6f 7720 4672  ..........Low Fr
-00003dc0: 6571 2e20 2848 7a29 0700 0000 0664 6961  eq. (Hz).....dia
-00003dd0: 6c6f 6701 0300 0000 2400 4100 7200 6d00  log.....$.A.r.m.
-00003de0: 6f00 6e00 6900 6300 6100 2000 6900 6e00  o.n.i.c.a. .i.n.
-00003df0: 6600 6500 7200 6900 6f00 7200 6508 0000  f.e.r.i.o.r.e...
-00003e00: 0000 0600 0000 0c4c 6f77 2048 6172 6d6f  .......Low Harmo
-00003e10: 6e69 6307 0000 0006 6469 616c 6f67 0103  nic.....dialog..
-00003e20: 0000 001c 0053 0074 006f 0070 0020 0069  .....S.t.o.p. .i
-00003e30: 006e 0066 0065 0072 0069 006f 0072 0065  .n.f.e.r.i.o.r.e
-00003e40: 0800 0000 0006 0000 0008 4c6f 7720 5374  ..........Low St
-00003e50: 6f70 0700 0000 0664 6961 6c6f 6701 0300  op.....dialog...
-00003e60: 0000 5200 4c00 6900 7600 6500 6c00 6c00  ..R.L.i.v.e.l.l.
-00003e70: 6f00 2000 6300 6f00 6d00 7000 6f00 6e00  o. .c.o.m.p.o.n.
-00003e80: 6500 6e00 7400 6900 2000 6200 6100 6e00  e.n.t.i. .b.a.n.
-00003e90: 6400 6100 2000 7300 7400 7200 6500 7400  d.a. .s.t.r.e.t.
-00003ea0: 7400 6100 2000 2800 6400 4200 2000 5300  t.a. .(.d.B. .S.
-00003eb0: 5000 4c00 2908 0000 0000 0600 0000 244e  P.L.).........$N
-00003ec0: 6172 726f 7720 4261 6e64 2043 6f6d 706f  arrow Band Compo
-00003ed0: 6e65 6e74 204c 6576 656c 2028 6442 2053  nent Level (dB S
-00003ee0: 504c 2907 0000 0006 6469 616c 6f67 0103  PL).....dialog..
-00003ef0: 0000 0042 0052 0075 006d 006f 0072 0065  ...B.R.u.m.o.r.e
-00003f00: 0020 0031 0020 0066 0072 0065 0071 0075  . .1. .f.r.e.q.u
-00003f10: 0065 006e 007a 0061 0020 0073 0075 0070  .e.n.z.a. .s.u.p
-00003f20: 0065 0072 0069 006f 0072 0065 0020 0028  .e.r.i.o.r.e. .(
-00003f30: 0048 007a 0029 0800 0000 0006 0000 0015  .H.z.)..........
-00003f40: 4e6f 2e20 3120 4869 6768 2046 7265 712e  No. 1 High Freq.
-00003f50: 2028 487a 2907 0000 0006 6469 616c 6f67   (Hz).....dialog
-00003f60: 0103 0000 0042 0052 0075 006d 006f 0072  .....B.R.u.m.o.r
-00003f70: 0065 0020 0031 0020 0066 0072 0065 0071  .e. .1. .f.r.e.q
-00003f80: 0075 0065 006e 007a 0061 0020 0069 006e  .u.e.n.z.a. .i.n
-00003f90: 0066 0065 0072 0069 006f 0072 0065 0020  .f.e.r.i.o.r.e. 
-00003fa0: 0028 0048 007a 0029 0800 0000 0006 0000  .(.H.z.)........
-00003fb0: 0014 4e6f 2e20 3120 4c6f 7720 4672 6571  ..No. 1 Low Freq
-00003fc0: 2e20 2848 7a29 0700 0000 0664 6961 6c6f  . (Hz).....dialo
-00003fd0: 6701 0300 0000 3200 4c00 6900 7600 6500  g.....2.L.i.v.e.
-00003fe0: 6c00 6c00 6f00 2000 7200 7500 6d00 6f00  l.l.o. .r.u.m.o.
-00003ff0: 7200 6500 2000 3100 2000 2800 6400 4200  r.e. .1. .(.d.B.
-00004000: 2000 5300 5000 4c00 2908 0000 0000 0600   .S.P.L.).......
-00004010: 0000 174e 6f2e 2031 2053 2e20 4c65 7665  ...No. 1 S. Leve
-00004020: 6c20 2864 4220 5350 4c29 0700 0000 0664  l (dB SPL).....d
-00004030: 6961 6c6f 6701 0300 0000 4200 5200 7500  ialog.....B.R.u.
-00004040: 6d00 6f00 7200 6500 2000 3100 2000 6600  m.o.r.e. .1. .f.
-00004050: 7200 6500 7100 7500 6500 6e00 7a00 6100  r.e.q.u.e.n.z.a.
-00004060: 2000 7300 7500 7000 6500 7200 6900 6f00   .s.u.p.e.r.i.o.
-00004070: 7200 6500 2000 2800 4800 7a00 2908 0000  r.e. .(.H.z.)...
-00004080: 0000 0600 0000 154e 6f2e 2032 2048 6967  .......No. 2 Hig
-00004090: 6820 4672 6571 2e20 2848 7a29 0700 0000  h Freq. (Hz)....
-000040a0: 0664 6961 6c6f 6701 0300 0000 4200 5200  .dialog.....B.R.
-000040b0: 7500 6d00 6f00 7200 6500 2000 3200 2000  u.m.o.r.e. .2. .
-000040c0: 6600 7200 6500 7100 7500 6500 6e00 7a00  f.r.e.q.u.e.n.z.
-000040d0: 6100 2000 6900 6e00 6600 6500 7200 6900  a. .i.n.f.e.r.i.
-000040e0: 6f00 7200 6500 2000 2800 4800 7a00 2908  o.r.e. .(.H.z.).
-000040f0: 0000 0000 0600 0000 144e 6f2e 2032 204c  .........No. 2 L
-00004100: 6f77 2046 7265 712e 2028 487a 2907 0000  ow Freq. (Hz)...
-00004110: 0006 6469 616c 6f67 0103 0000 0032 004c  ..dialog.....2.L
-00004120: 0069 0076 0065 006c 006c 006f 0020 0072  .i.v.e.l.l.o. .r
-00004130: 0075 006d 006f 0072 0065 0020 0032 0020  .u.m.o.r.e. .2. 
-00004140: 0028 0064 0042 0020 0053 0050 004c 0029  .(.d.B. .S.P.L.)
-00004150: 0800 0000 0006 0000 0017 4e6f 2e20 3220  ..........No. 2 
-00004160: 532e 204c 6576 656c 2028 6442 2053 504c  S. Level (dB SPL
-00004170: 2907 0000 0006 6469 616c 6f67 0103 0000  ).....dialog....
-00004180: 0018 0054 0069 0070 006f 0020 0072 0075  ...T.i.p.o. .r.u
-00004190: 006d 006f 0072 0065 003a 0800 0000 0006  .m.o.r.e.:......
-000041a0: 0000 000b 4e6f 6973 6520 5479 7065 3a07  ....Noise Type:.
-000041b0: 0000 0006 6469 616c 6f67 0103 0000 0024  ....dialog.....$
-000041c0: 0052 0065 006c 0061 007a 0069 006f 006e  .R.e.l.a.z.i.o.n
-000041d0: 0065 0020 0064 0069 0020 0066 0061 0073  .e. .d.i. .f.a.s
-000041e0: 0065 003a 0800 0000 0006 0000 0013 5068  .e.:..........Ph
-000041f0: 6173 6520 7265 6c61 7469 6f6e 7368 6970  ase relationship
-00004200: 3a07 0000 0006 6469 616c 6f67 0103 0000  :.....dialog....
-00004210: 000a 0046 0061 0073 0065 003a 0800 0000  ...F.a.s.e.:....
-00004220: 0006 0000 0006 5068 6173 653a 0700 0000  ......Phase:....
-00004230: 0664 6961 6c6f 6701 0300 0000 1400 5200  .dialog.......R.
-00004240: 6100 6d00 7000 6100 2000 2800 7300 6d00  a.m.p.a. .(.s.m.
-00004250: 2908 0000 0000 0600 0000 0952 616d 7020  )..........Ramp 
-00004260: 286d 7329 0700 0000 0664 6961 6c6f 6701  (ms).....dialog.
-00004270: 0300 0000 2c00 4900 6e00 7400 6500 7200  ....,.I.n.t.e.r.
-00004280: 7600 6100 6c00 6c00 6f00 2000 2800 6300  v.a.l.l.o. .(.c.
-00004290: 6500 6e00 7400 6500 7300 6900 6d00 6900  e.n.t.e.s.i.m.i.
-000042a0: 2908 0000 0000 0600 0000 0f53 7061 6369  )..........Spaci
-000042b0: 6e67 2028 4365 6e74 7329 0700 0000 0664  ng (Cents).....d
-000042c0: 6961 6c6f 6701 0300 0000 3400 4c00 6900  ialog.....4.L.i.
-000042d0: 7600 6500 6c00 6c00 6f00 2000 7300 7000  v.e.l.l.o. .s.p.
-000042e0: 6500 7400 7400 7200 6100 6c00 6500 2000  e.t.t.r.a.l.e. .
-000042f0: 2800 6400 4200 2000 5300 5000 4c00 2908  (.d.B. .S.P.L.).
-00004300: 0000 0000 0600 0000 1753 7065 6374 7275  .........Spectru
-00004310: 6d20 4c65 7665 6c20 2864 4220 5350 4c29  m Level (dB SPL)
-00004320: 0700 0000 0664 6961 6c6f 6701 0300 0000  .....dialog.....
-00004330: 2000 4100 6c00 6c00 7500 6e00 6700 6100   .A.l.l.u.n.g.a.
-00004340: 6d00 6500 6e00 7400 6f00 2000 2800 2500  m.e.n.t.o. .(.%.
-00004350: 2908 0000 0000 0600 0000 0b53 7472 6574  )..........Stret
-00004360: 6368 2028 2529 0700 0000 0664 6961 6c6f  ch (%).....dialo
-00004370: 6701 0300 0000 0a00 5400 6900 7000 6f00  g.......T.i.p.o.
-00004380: 3a08 0000 0000 0600 0000 0554 7970 653a  :..........Type:
-00004390: 0700 0000 0664 6961 6c6f 6701 0300 0000  .....dialog.....
-000043a0: 0600 4200 6c00 7508 0000 0000 0600 0000  ..B.l.u.........
-000043b0: 0442 6c75 6507 0000 0013 6765 6e65 7261  .Blue.....genera
-000043c0: 7465 4e6f 6973 6544 6961 6c6f 6701 0300  teNoiseDialog...
-000043d0: 0000 1000 4500 6e00 7400 7200 6100 6d00  ....E.n.t.r.a.m.
-000043e0: 6200 6508 0000 0000 0600 0000 0442 6f74  b.e..........Bot
-000043f0: 6807 0000 0013 6765 6e65 7261 7465 4e6f  h.....generateNo
-00004400: 6973 6544 6961 6c6f 6701 0300 0000 1800  iseDialog.......
-00004410: 4400 7500 7200 6100 7400 6100 2000 2800  D.u.r.a.t.a. .(.
-00004420: 6d00 7300 2900 3a08 0000 0000 0600 0000  m.s.).:.........
-00004430: 0e44 7572 6174 696f 6e20 286d 7329 3a07  .Duration (ms):.
-00004440: 0000 0013 6765 6e65 7261 7465 4e6f 6973  ....generateNois
-00004450: 6544 6961 6c6f 6701 0300 0000 1200 4f00  eDialog.......O.
-00004460: 7200 6500 6300 6300 6800 6900 6f00 3a08  r.e.c.c.h.i.o.:.
-00004470: 0000 0000 0600 0000 0545 6172 3a20 0700  .........Ear: ..
-00004480: 0000 1367 656e 6572 6174 654e 6f69 7365  ...generateNoise
-00004490: 4469 616c 6f67 0103 0000 001a 0047 0065  Dialog.......G.e
-000044a0: 006e 0065 0072 0061 0020 0072 0075 006d  .n.e.r.a. .r.u.m
-000044b0: 006f 0072 0065 0800 0000 0006 0000 000e  .o.r.e..........
-000044c0: 4765 6e65 7261 7465 204e 6f69 7365 0700  Generate Noise..
-000044d0: 0000 1367 656e 6572 6174 654e 6f69 7365  ...generateNoise
-000044e0: 4469 616c 6f67 0103 0000 0010 0053 0069  Dialog.......S.i
-000044f0: 006e 0069 0073 0074 0072 006f 0800 0000  .n.i.s.t.r.o....
-00004500: 0006 0000 0004 4c65 6674 0700 0000 1367  ......Left.....g
-00004510: 656e 6572 6174 654e 6f69 7365 4469 616c  enerateNoiseDial
-00004520: 6f67 0103 0000 000c 0052 0075 006d 006f  og.......R.u.m.o
-00004530: 0072 0065 0800 0000 0006 0000 0005 4e6f  .r.e..........No
-00004540: 6973 6507 0000 0013 6765 6e65 7261 7465  ise.....generate
-00004550: 4e6f 6973 6544 6961 6c6f 6701 0300 0000  NoiseDialog.....
-00004560: 1e00 5400 6900 7000 6f00 2000 6400 6900  ..T.i.p.o. .d.i.
-00004570: 2000 7200 7500 6d00 6f00 7200 6500 3a08   .r.u.m.o.r.e.:.
-00004580: 0000 0000 0600 0000 0c4e 6f69 7365 2054  .........Noise T
-00004590: 7970 653a 2007 0000 0013 6765 6e65 7261  ype: .....genera
-000045a0: 7465 4e6f 6973 6544 6961 6c6f 6701 0300  teNoiseDialog...
-000045b0: 0000 0800 5200 6f00 7300 6108 0000 0000  ....R.o.s.a.....
-000045c0: 0600 0000 0450 696e 6b07 0000 0013 6765  .....Pink.....ge
-000045d0: 6e65 7261 7465 4e6f 6973 6544 6961 6c6f  nerateNoiseDialo
-000045e0: 6701 0300 0000 1600 5200 6100 6d00 7000  g.......R.a.m.p.
-000045f0: 6500 2000 2800 6d00 7300 2900 3a08 0000  e. .(.m.s.).:...
-00004600: 0000 0600 0000 0b52 616d 7073 2028 6d73  .......Ramps (ms
-00004610: 293a 0700 0000 1367 656e 6572 6174 654e  ):.....generateN
-00004620: 6f69 7365 4469 616c 6f67 0103 0000 000a  oiseDialog......
-00004630: 0052 006f 0073 0073 006f 0800 0000 0006  .R.o.s.s.o......
-00004640: 0000 0003 5265 6407 0000 0013 6765 6e65  ....Red.....gene
-00004650: 7261 7465 4e6f 6973 6544 6961 6c6f 6701  rateNoiseDialog.
-00004660: 0300 0000 0c00 4400 6500 7300 7400 7200  ......D.e.s.t.r.
-00004670: 6f08 0000 0000 0600 0000 0552 6967 6874  o..........Right
-00004680: 0700 0000 1367 656e 6572 6174 654e 6f69  .....generateNoi
-00004690: 7365 4469 616c 6f67 0103 0000 0034 0046  seDialog.....4.F
-000046a0: 0072 0065 0071 0075 0065 006e 007a 0061  .r.e.q.u.e.n.z.a
-000046b0: 0020 0064 0069 0020 0063 0061 006d 0070  . .d.i. .c.a.m.p
-000046c0: 0069 006f 006e 0061 006d 0065 006e 0074  .i.o.n.a.m.e.n.t
-000046d0: 006f 0800 0000 0006 0000 000d 5361 6d70  .o..........Samp
-000046e0: 6c69 6e67 2052 6174 6507 0000 0013 6765  ling Rate.....ge
-000046f0: 6e65 7261 7465 4e6f 6973 6544 6961 6c6f  nerateNoiseDialo
-00004700: 6701 0300 0000 1600 4e00 6f00 6d00 6500  g.......N.o.m.e.
-00004710: 2000 5300 7500 6f00 6e00 6f00 3a08 0000   .S.u.o.n.o.:...
-00004720: 0000 0600 0000 0d53 6f75 6e64 204c 6162  .......Sound Lab
-00004730: 656c 3a20 0700 0000 1367 656e 6572 6174  el: .....generat
-00004740: 654e 6f69 7365 4469 616c 6f67 0103 0000  eNoiseDialog....
-00004750: 002e 004c 0069 0076 0065 006c 006c 006f  ...L.i.v.e.l.l.o
-00004760: 0020 0073 0070 0065 0074 0074 0072 0061  . .s.p.e.t.t.r.a
-00004770: 006c 0065 0020 0028 0064 0042 0029 003a  .l.e. .(.d.B.).:
-00004780: 0800 0000 0006 0000 0014 5370 6563 7472  ..........Spectr
-00004790: 756d 204c 6576 656c 2028 6442 293a 0700  um Level (dB):..
-000047a0: 0000 1367 656e 6572 6174 654e 6f69 7365  ...generateNoise
-000047b0: 4469 616c 6f67 0103 0000 000a 0056 0069  Dialog.......V.i
-000047c0: 006f 006c 0061 0800 0000 0006 0000 0006  .o.l.a..........
-000047d0: 5669 6f6c 6574 0700 0000 1367 656e 6572  Violet.....gener
-000047e0: 6174 654e 6f69 7365 4469 616c 6f67 0103  ateNoiseDialog..
-000047f0: 0000 000c 0042 0069 0061 006e 0063 006f  .....B.i.a.n.c.o
-00004800: 0800 0000 0006 0000 0005 5768 6974 6507  ..........White.
-00004810: 0000 0013 6765 6e65 7261 7465 4e6f 6973  ....generateNois
-00004820: 6544 6961 6c6f 6701 0300 0000 1200 7200  eDialog.......r.
-00004830: 6500 2e00 2000 2800 4800 7a00 2900 3a08  e... .(.H.z.).:.
-00004840: 0000 0000 0600 0000 0a72 652e 2028 487a  .........re. (Hz
-00004850: 293a 2007 0000 0013 6765 6e65 7261 7465  ): .....generate
-00004860: 4e6f 6973 6544 6961 6c6f 6701 0300 0000  NoiseDialog.....
-00004870: 1000 4500 6e00 7400 7200 6100 6d00 6200  ..E.n.t.r.a.m.b.
-00004880: 6508 0000 0000 0600 0000 0442 6f74 6807  e..........Both.
-00004890: 0000 0016 6765 6e65 7261 7465 5369 6e75  ....generateSinu
-000048a0: 736f 6964 4469 616c 6f67 0103 0000 0018  soidDialog......
-000048b0: 0044 0075 0072 0061 0074 0061 0020 0028  .D.u.r.a.t.a. .(
-000048c0: 006d 0073 0029 003a 0800 0000 0006 0000  .m.s.).:........
-000048d0: 000e 4475 7261 7469 6f6e 2028 6d73 293a  ..Duration (ms):
-000048e0: 0700 0000 1667 656e 6572 6174 6553 696e  .....generateSin
-000048f0: 7573 6f69 6444 6961 6c6f 6701 0300 0000  usoidDialog.....
-00004900: 1200 4f00 7200 6500 6300 6300 6800 6900  ..O.r.e.c.c.h.i.
-00004910: 6f00 3a08 0000 0000 0600 0000 0545 6172  o.:..........Ear
-00004920: 3a20 0700 0000 1667 656e 6572 6174 6553  : .....generateS
-00004930: 696e 7573 6f69 6444 6961 6c6f 6701 0300  inusoidDialog...
-00004940: 0000 1e00 4600 7200 6500 7100 7500 6500  ....F.r.e.q.u.e.
-00004950: 6e00 7a00 6100 2000 2800 4800 7a00 2900  n.z.a. .(.H.z.).
-00004960: 3a08 0000 0000 0600 0000 0f46 7265 7175  :..........Frequ
-00004970: 656e 6379 2028 487a 293a 0700 0000 1667  ency (Hz):.....g
-00004980: 656e 6572 6174 6553 696e 7573 6f69 6444  enerateSinusoidD
-00004990: 6961 6c6f 6701 0300 0000 2000 4700 6500  ialog..... .G.e.
-000049a0: 6e00 6500 7200 6100 2000 7300 6900 6e00  n.e.r.a. .s.i.n.
-000049b0: 7500 7300 6f00 6900 6400 6508 0000 0000  u.s.o.i.d.e.....
-000049c0: 0600 0000 1147 656e 6572 6174 6520 5369  .....Generate Si
-000049d0: 6e75 736f 6964 0700 0000 1667 656e 6572  nusoid.....gener
-000049e0: 6174 6553 696e 7573 6f69 6444 6961 6c6f  ateSinusoidDialo
-000049f0: 6701 0300 0000 1000 4900 4c00 4400 2000  g.......I.L.D. .
-00004a00: 2800 6400 4200 2908 0000 0000 0600 0000  (.d.B.).........
-00004a10: 0849 4c44 2028 6442 2907 0000 0016 6765  .ILD (dB).....ge
-00004a20: 6e65 7261 7465 5369 6e75 736f 6964 4469  nerateSinusoidDi
-00004a30: 616c 6f67 0103 0000 0010 0049 0054 0044  alog.......I.T.D
-00004a40: 0020 0028 0075 0073 0029 0800 0000 0006  . .(.u.s.)......
-00004a50: 0000 0008 4954 4420 2875 7329 0700 0000  ....ITD (us)....
-00004a60: 1667 656e 6572 6174 6553 696e 7573 6f69  .generateSinusoi
-00004a70: 6444 6961 6c6f 6701 0300 0000 1000 5300  dDialog.......S.
-00004a80: 6900 6e00 6900 7300 7400 7200 6f08 0000  i.n.i.s.t.r.o...
-00004a90: 0000 0600 0000 044c 6566 7407 0000 0016  .......Left.....
-00004aa0: 6765 6e65 7261 7465 5369 6e75 736f 6964  generateSinusoid
-00004ab0: 4469 616c 6f67 0103 0000 0018 004c 0069  Dialog.......L.i
-00004ac0: 0076 0065 006c 006c 006f 0020 0028 0064  .v.e.l.l.o. .(.d
-00004ad0: 0042 0029 0800 0000 0006 0000 000b 4c65  .B.)..........Le
-00004ae0: 7665 6c20 2864 4229 3a07 0000 0016 6765  vel (dB):.....ge
-00004af0: 6e65 7261 7465 5369 6e75 736f 6964 4469  nerateSinusoidDi
-00004b00: 616c 6f67 0103 0000 0020 0046 0061 0073  alog..... .F.a.s
-00004b10: 0065 0020 0028 0072 0061 0064 0069 0061  .e. .(.r.a.d.i.a
-00004b20: 006e 0074 0069 0029 003a 0800 0000 0006  .n.t.i.).:......
-00004b30: 0000 0010 5068 6173 6520 2872 6164 6961  ....Phase (radia
-00004b40: 6e73 293a 0700 0000 1667 656e 6572 6174  ns):.....generat
-00004b50: 6553 696e 7573 6f69 6444 6961 6c6f 6701  eSinusoidDialog.
-00004b60: 0300 0000 1600 5200 6100 6d00 7000 6500  ......R.a.m.p.e.
-00004b70: 2000 2800 6d00 7300 2900 3a08 0000 0000   .(.m.s.).:.....
-00004b80: 0600 0000 0b52 616d 7073 2028 6d73 293a  .....Ramps (ms):
-00004b90: 0700 0000 1667 656e 6572 6174 6553 696e  .....generateSin
-00004ba0: 7573 6f69 6444 6961 6c6f 6701 0300 0000  usoidDialog.....
-00004bb0: 1200 5200 6500 6600 6500 7200 6500 6e00  ..R.e.f.e.r.e.n.
-00004bc0: 7a00 6108 0000 0000 0600 0000 0952 6566  z.a..........Ref
-00004bd0: 6572 656e 6365 0700 0000 1667 656e 6572  erence.....gener
-00004be0: 6174 6553 696e 7573 6f69 6444 6961 6c6f  ateSinusoidDialo
-00004bf0: 6701 0300 0000 0c00 4400 6500 7300 7400  g.......D.e.s.t.
-00004c00: 7200 6f08 0000 0000 0600 0000 0552 6967  r.o..........Rig
-00004c10: 6874 0700 0000 1667 656e 6572 6174 6553  ht.....generateS
-00004c20: 696e 7573 6f69 6444 6961 6c6f 6701 0300  inusoidDialog...
-00004c30: 0000 3400 4600 7200 6500 7100 7500 6500  ..4.F.r.e.q.u.e.
-00004c40: 6e00 7a00 6100 2000 6400 6900 2000 6300  n.z.a. .d.i. .c.
-00004c50: 6100 6d00 7000 6900 6f00 6e00 6100 6d00  a.m.p.i.o.n.a.m.
-00004c60: 6500 6e00 7400 6f08 0000 0000 0600 0000  e.n.t.o.........
-00004c70: 0d53 616d 706c 696e 6720 5261 7465 0700  .Sampling Rate..
-00004c80: 0000 1667 656e 6572 6174 6553 696e 7573  ...generateSinus
-00004c90: 6f69 6444 6961 6c6f 6701 0300 0000 1200  oidDialog.......
-00004ca0: 5300 6900 6e00 7500 7300 6f00 6900 6400  S.i.n.u.s.o.i.d.
-00004cb0: 6508 0000 0000 0600 0000 0853 696e 7573  e..........Sinus
-00004cc0: 6f69 6407 0000 0016 6765 6e65 7261 7465  oid.....generate
-00004cd0: 5369 6e75 736f 6964 4469 616c 6f67 0103  SinusoidDialog..
-00004ce0: 0000 0016 004e 006f 006d 0065 0020 0053  .....N.o.m.e. .S
-00004cf0: 0075 006f 006e 006f 003a 0800 0000 0006  .u.o.n.o.:......
-00004d00: 0000 000d 536f 756e 6420 4c61 6265 6c3a  ....Sound Label:
-00004d10: 2007 0000 0016 6765 6e65 7261 7465 5369   .....generateSi
-00004d20: 6e75 736f 6964 4469 616c 6f67 0103 0000  nusoidDialog....
-00004d30: 001e 0053 006f 006d 006d 0061 0020 006f  ...S.o.m.m.a. .o
-00004d40: 0072 0069 0067 0069 006e 0061 006c 0065  .r.i.g.i.n.a.l.e
-00004d50: 0800 0000 0006 0000 000c 4164 6420 4f72  ..........Add Or
-00004d60: 6967 696e 616c 0700 0000 1367 656e 6572  iginal.....gener
-00004d70: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-00004d80: 0000 0018 0053 006f 006d 006d 0061 0020  .....S.o.m.m.a. 
-00004d90: 0075 0067 0075 0061 006c 0065 0800 0000  .u.g.u.a.l.e....
-00004da0: 0006 0000 0008 4164 6420 5361 6d65 0700  ......Add Same..
-00004db0: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
-00004dc0: 4469 616c 6f67 0103 0000 0012 0041 006c  Dialog.......A.l
-00004dd0: 0074 0065 0072 006e 0061 0074 0061 0800  .t.e.r.n.a.t.a..
-00004de0: 0000 0006 0000 000b 416c 7465 726e 6174  ........Alternat
-00004df0: 696e 6707 0000 0013 6765 6e65 7261 7465  ing.....generate
-00004e00: 536f 756e 6444 6961 6c6f 6701 0300 0000  SoundDialog.....
-00004e10: 3c00 4c00 6100 7200 6700 6800 6500 7a00  <.L.a.r.g.h.e.z.
-00004e20: 7a00 6100 2000 6400 6900 2000 6200 6100  z.a. .d.i. .b.a.
-00004e30: 6e00 6400 6100 2000 2800 6300 6500 6e00  n.d.a. .(.c.e.n.
-00004e40: 7400 6500 7300 6900 6d00 6900 2908 0000  t.e.s.i.m.i.)...
-00004e50: 0000 0600 0000 1142 616e 6477 6964 7468  .......Bandwidth
-00004e60: 2028 4365 6e74 7329 0700 0000 1367 656e   (Cents).....gen
-00004e70: 6572 6174 6553 6f75 6e64 4469 616c 6f67  erateSoundDialog
-00004e80: 0103 0000 002e 004c 0061 0072 0067 0068  .......L.a.r.g.h
-00004e90: 0065 007a 007a 0061 0020 0064 0069 0020  .e.z.z.a. .d.i. 
-00004ea0: 0062 0061 006e 0064 0061 0020 0028 0048  .b.a.n.d.a. .(.H
-00004eb0: 007a 0029 0800 0000 0006 0000 000e 4261  .z.)..........Ba
-00004ec0: 6e64 7769 6474 6820 2848 7a29 0700 0000  ndwidth (Hz)....
-00004ed0: 1367 656e 6572 6174 6553 6f75 6e64 4469  .generateSoundDi
-00004ee0: 616c 6f67 0103 0000 0010 0045 006e 0074  alog.......E.n.t
-00004ef0: 0072 0061 006d 0062 0065 0800 0000 0006  .r.a.m.b.e......
-00004f00: 0000 0004 426f 7468 0700 0000 1367 656e  ....Both.....gen
-00004f10: 6572 6174 6553 6f75 6e64 4469 616c 6f67  erateSoundDialog
-00004f20: 0103 0000 0036 004c 0069 0076 0065 006c  .....6.L.i.v.e.l
-00004f30: 006c 006f 0020 0063 006f 006d 0070 006f  .l.o. .c.o.m.p.o
-00004f40: 006e 0065 006e 0074 0065 0020 0028 0064  .n.e.n.t.e. .(.d
-00004f50: 0042 0020 0053 0050 004c 0029 0800 0000  .B. .S.P.L.)....
-00004f60: 0006 0000 0018 436f 6d70 6f6e 656e 7420  ......Component 
-00004f70: 4c65 7665 6c20 2864 4220 5350 4c29 0700  Level (dB SPL)..
-00004f80: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
-00004f90: 4469 616c 6f67 0103 0000 0006 0043 006f  Dialog.......C.o
-00004fa0: 0073 0800 0000 0006 0000 0006 436f 7369  .s..........Cosi
-00004fb0: 6e65 0700 0000 1367 656e 6572 6174 6553  ne.....generateS
-00004fc0: 6f75 6e64 4469 616c 6f67 0103 0000 0028  oundDialog.....(
-00004fd0: 0044 0069 0066 0066 0065 0072 0065 006e  .D.i.f.f.e.r.e.n
-00004fe0: 007a 0061 0020 0064 0069 0063 006f 0074  .z.a. .d.i.c.o.t
-00004ff0: 0069 0063 0061 003a 0800 0000 0006 0000  .i.c.a.:........
-00005000: 0014 4469 6368 6f74 6963 2044 6966 6665  ..Dichotic Diffe
-00005010: 7265 6e63 653a 0700 0000 1367 656e 6572  rence:.....gener
-00005020: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-00005030: 0000 0016 0044 0075 0072 0061 0074 0061  .....D.u.r.a.t.a
-00005040: 0020 0028 006d 0073 0029 0800 0000 0006  . .(.m.s.)......
-00005050: 0000 000d 4475 7261 7469 6f6e 2028 6d73  ....Duration (ms
-00005060: 2907 0000 0013 6765 6e65 7261 7465 536f  ).....generateSo
-00005070: 756e 6444 6961 6c6f 6701 0300 0000 1200  undDialog.......
-00005080: 4f00 7200 6500 6300 6300 6800 6900 6f00  O.r.e.c.c.h.i.o.
-00005090: 3a08 0000 0000 0600 0000 0445 6172 3a07  :..........Ear:.
-000050a0: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
-000050b0: 6444 6961 6c6f 6701 0300 0000 0e00 4600  dDialog.......F.
-000050c0: 3000 2000 2800 4800 7a00 2908 0000 0000  0. .(.H.z.).....
-000050d0: 0600 0000 0746 3020 2848 7a29 0700 0000  .....F0 (Hz)....
-000050e0: 1367 656e 6572 6174 6553 6f75 6e64 4469  .generateSoundDi
-000050f0: 616c 6f67 0103 0000 001c 0046 0072 0065  alog.......F.r.e
-00005100: 0071 0075 0065 006e 007a 0061 0020 0028  .q.u.e.n.z.a. .(
-00005110: 0048 007a 0029 0800 0000 0006 0000 000e  .H.z.)..........
-00005120: 4672 6571 7565 6e63 7920 2848 7a29 0700  Frequency (Hz)..
-00005130: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
-00005140: 4469 616c 6f67 0103 0000 0008 0047 0061  Dialog.......G.a
-00005150: 0069 006e 0800 0000 0006 0000 0004 4761  .i.n..........Ga
-00005160: 696e 0700 0000 1367 656e 6572 6174 6553  in.....generateS
-00005170: 6f75 6e64 4469 616c 6f67 0103 0000 0018  oundDialog......
-00005180: 0047 0065 006e 0065 0072 0061 0020 0073  .G.e.n.e.r.a. .s
-00005190: 0075 006f 006e 006f 0800 0000 0006 0000  .u.o.n.o........
-000051a0: 000e 4765 6e65 7261 7465 2053 6f75 6e64  ..Generate Sound
-000051b0: 0700 0000 1367 656e 6572 6174 6553 6f75  .....generateSou
-000051c0: 6e64 4469 616c 6f67 0103 0000 0012 0041  ndDialog.......A
-000051d0: 0072 006d 006f 006e 0069 0063 006f 003a  .r.m.o.n.i.c.o.:
-000051e0: 0800 0000 0006 0000 0008 4861 726d 6f6e  ..........Harmon
-000051f0: 6963 0700 0000 1367 656e 6572 6174 6553  ic.....generateS
-00005200: 6f75 6e64 4469 616c 6f67 0103 0000 0032  oundDialog.....2
-00005210: 004c 0069 0076 0065 006c 006c 006f 0020  .L.i.v.e.l.l.o. 
-00005220: 0061 0072 006d 006f 006e 0069 0063 006f  .a.r.m.o.n.i.c.o
-00005230: 0020 0028 0064 0042 0020 0053 0050 004c  . .(.d.B. .S.P.L
-00005240: 0029 0800 0000 0006 0000 0017 4861 726d  .)..........Harm
-00005250: 6f6e 6963 204c 6576 656c 2028 6442 2053  onic Level (dB S
-00005260: 504c 2907 0000 0013 6765 6e65 7261 7465  PL).....generate
-00005270: 536f 756e 6444 6961 6c6f 6701 0300 0000  SoundDialog.....
-00005280: 3e00 4900 6e00 7400 6500 7200 7600 6100  >.I.n.t.e.r.v.a.
-00005290: 6c00 6c00 6f00 2000 6100 7200 6d00 6f00  l.l.o. .a.r.m.o.
-000052a0: 6e00 6900 6300 6f00 2000 2800 6300 6500  n.i.c.o. .(.c.e.
-000052b0: 6e00 7400 6500 7300 6900 6d00 6900 2908  n.t.e.s.i.m.i.).
-000052c0: 0000 0000 0600 0000 1848 6172 6d6f 6e69  .........Harmoni
-000052d0: 6320 5370 6163 696e 6720 2843 656e 7473  c Spacing (Cents
-000052e0: 2907 0000 0013 6765 6e65 7261 7465 536f  ).....generateSo
-000052f0: 756e 6444 6961 6c6f 6701 0300 0000 2400  undDialog.....$.
-00005300: 4100 7200 6d00 6f00 6e00 6900 6300 6f00  A.r.m.o.n.i.c.o.
-00005310: 2000 6100 6c00 6c00 7500 6e00 6700 6100   .a.l.l.u.n.g.a.
-00005320: 7400 6f08 0000 0000 0600 0000 1248 6172  t.o..........Har
-00005330: 6d6f 6e69 6320 5374 7265 7463 6865 6407  monic Stretched.
-00005340: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
-00005350: 6444 6961 6c6f 6701 0300 0000 1600 4100  dDialog.......A.
-00005360: 7200 6d00 6f00 6e00 6900 6300 6900 7400  r.m.o.n.i.c.i.t.
-00005370: e000 3a08 0000 0000 0600 0000 0c48 6172  ..:..........Har
-00005380: 6d6f 6e69 6369 7479 3a07 0000 0013 6765  monicity:.....ge
-00005390: 6e65 7261 7465 536f 756e 6444 6961 6c6f  nerateSoundDialo
-000053a0: 6701 0300 0000 3000 4600 7200 6500 7100  g.....0.F.r.e.q.
-000053b0: 7500 6500 6e00 7a00 6100 2000 7300 7500  u.e.n.z.a. .s.u.
-000053c0: 7000 6500 7200 6900 6f00 7200 6500 2000  p.e.r.i.o.r.e. .
-000053d0: 2800 4800 7a00 2908 0000 0000 0600 0000  (.H.z.).........
-000053e0: 0f48 6967 6820 4672 6571 2e20 2848 7a29  .High Freq. (Hz)
-000053f0: 0700 0000 1367 656e 6572 6174 6553 6f75  .....generateSou
-00005400: 6e64 4469 616c 6f67 0103 0000 0024 0041  ndDialog.....$.A
-00005410: 0072 006d 006f 006e 0069 0063 0061 0020  .r.m.o.n.i.c.a. 
-00005420: 0073 0075 0070 0065 0072 0069 006f 0072  .s.u.p.e.r.i.o.r
-00005430: 0065 0800 0000 0006 0000 000d 4869 6768  .e..........High
-00005440: 2048 6172 6d6f 6e69 6307 0000 0013 6765   Harmonic.....ge
-00005450: 6e65 7261 7465 536f 756e 6444 6961 6c6f  nerateSoundDialo
-00005460: 6701 0300 0000 1c00 5300 7400 6f00 7000  g.......S.t.o.p.
-00005470: 2000 7300 7500 7000 6500 7200 6900 6f00   .s.u.p.e.r.i.o.
-00005480: 7200 6508 0000 0000 0600 0000 0948 6967  r.e..........Hig
-00005490: 6820 5374 6f70 0700 0000 1367 656e 6572  h Stop.....gener
-000054a0: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-000054b0: 0000 0020 0050 0069 0074 0063 0068 0020  ... .P.i.t.c.h. 
-000054c0: 0064 0069 0020 0048 0075 0067 0067 0069  .d.i. .H.u.g.g.i
-000054d0: 006e 0073 0800 0000 0006 0000 000d 4875  .n.s..........Hu
-000054e0: 6767 696e 7320 5069 7463 6807 0000 0013  ggins Pitch.....
-000054f0: 6765 6e65 7261 7465 536f 756e 6444 6961  generateSoundDia
-00005500: 6c6f 6701 0300 0000 1c00 4900 5000 4400  log.......I.P.D.
-00005510: 2000 2800 7200 6100 6400 6900 6100 6e00   .(.r.a.d.i.a.n.
-00005520: 7400 6900 2908 0000 0000 0600 0000 0d49  t.i.)..........I
-00005530: 5044 2028 7261 6469 616e 7329 0700 0000  PD (radians)....
-00005540: 1367 656e 6572 6174 6553 6f75 6e64 4469  .generateSoundDi
-00005550: 616c 6f67 0103 0000 0016 0049 0050 0044  alog.......I.P.D
-00005560: 0020 004c 0069 006e 0065 0061 0072 0065  . .L.i.n.e.a.r.e
-00005570: 0800 0000 0006 0000 000a 4950 4420 4c69  ..........IPD Li
-00005580: 6e65 6172 0700 0000 1367 656e 6572 6174  near.....generat
-00005590: 6553 6f75 6e64 4469 616c 6f67 0103 0000  eSoundDialog....
-000055a0: 001a 0049 0050 0044 0020 0061 0020 0073  ...I.P.D. .a. .s
-000055b0: 0063 0061 006c 0069 006e 006f 0800 0000  .c.a.l.i.n.o....
-000055c0: 0006 0000 000b 4950 4420 5374 6570 7065  ......IPD Steppe
-000055d0: 6407 0000 0013 6765 6e65 7261 7465 536f  d.....generateSo
-000055e0: 756e 6444 6961 6c6f 6701 0300 0000 0600  undDialog.......
-000055f0: 4900 5200 4e08 0000 0000 0600 0000 0349  I.R.N..........I
-00005600: 524e 0700 0000 1367 656e 6572 6174 6553  RN.....generateS
-00005610: 6f75 6e64 4469 616c 6f67 0103 0000 0012  oundDialog......
-00005620: 0054 0069 0070 006f 0020 0049 0052 004e  .T.i.p.o. .I.R.N
-00005630: 003a 0800 0000 0006 0000 0009 4952 4e20  .:..........IRN 
-00005640: 5479 7065 3a07 0000 0013 6765 6e65 7261  Type:.....genera
-00005650: 7465 536f 756e 6444 6961 6c6f 6701 0300  teSoundDialog...
-00005660: 0000 0600 4900 5400 4408 0000 0000 0600  ....I.T.D.......
-00005670: 0000 0349 5444 0700 0000 1367 656e 6572  ...ITD.....gener
-00005680: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-00005690: 0000 001a 0049 0054 0044 0020 0028 006d  .....I.T.D. .(.m
-000056a0: 0069 0063 0072 006f 0020 0073 0029 0800  .i.c.r.o. .s.)..
-000056b0: 0000 0006 0000 000d 4954 4420 286d 6963  ........ITD (mic
-000056c0: 726f 2073 2907 0000 0013 6765 6e65 7261  ro s).....genera
-000056d0: 7465 536f 756e 6444 6961 6c6f 6701 0300  teSoundDialog...
-000056e0: 0000 1400 4900 7400 6500 7200 6100 7a00  ....I.t.e.r.a.z.
-000056f0: 6900 6f00 6e00 6908 0000 0000 0600 0000  i.o.n.i.........
-00005700: 0a49 7465 7261 7469 6f6e 7307 0000 0013  .Iterations.....
-00005710: 6765 6e65 7261 7465 536f 756e 6444 6961  generateSoundDia
-00005720: 6c6f 6701 0300 0000 1000 5300 6900 6e00  log.......S.i.n.
-00005730: 6900 7300 7400 7200 6f08 0000 0000 0600  i.s.t.r.o.......
-00005740: 0000 044c 6566 7407 0000 0013 6765 6e65  ...Left.....gene
-00005750: 7261 7465 536f 756e 6444 6961 6c6f 6701  rateSoundDialog.
-00005760: 0300 0000 3000 4600 7200 6500 7100 7500  ....0.F.r.e.q.u.
-00005770: 6500 6e00 7a00 6100 2000 6900 6e00 6600  e.n.z.a. .i.n.f.
-00005780: 6500 7200 6900 6f00 7200 6500 2000 2800  e.r.i.o.r.e. .(.
-00005790: 4800 7a00 2908 0000 0000 0600 0000 0e4c  H.z.)..........L
-000057a0: 6f77 2046 7265 712e 2028 487a 2907 0000  ow Freq. (Hz)...
-000057b0: 0013 6765 6e65 7261 7465 536f 756e 6444  ..generateSoundD
-000057c0: 6961 6c6f 6701 0300 0000 2400 4100 7200  ialog.....$.A.r.
-000057d0: 6d00 6f00 6e00 6900 6300 6100 2000 6900  m.o.n.i.c.a. .i.
-000057e0: 6e00 6600 6500 7200 6900 6f00 7200 6508  n.f.e.r.i.o.r.e.
-000057f0: 0000 0000 0600 0000 0c4c 6f77 2048 6172  .........Low Har
-00005800: 6d6f 6e69 6307 0000 0013 6765 6e65 7261  monic.....genera
-00005810: 7465 536f 756e 6444 6961 6c6f 6701 0300  teSoundDialog...
-00005820: 0000 1c00 5300 7400 6f00 7000 2000 6900  ....S.t.o.p. .i.
-00005830: 6e00 6600 6500 7200 6900 6f00 7200 6508  n.f.e.r.i.o.r.e.
-00005840: 0000 0000 0600 0000 084c 6f77 2053 746f  .........Low Sto
-00005850: 7007 0000 0013 6765 6e65 7261 7465 536f  p.....generateSo
-00005860: 756e 6444 6961 6c6f 6701 0300 0000 5200  undDialog.....R.
-00005870: 4c00 6900 7600 6500 6c00 6c00 6f00 2000  L.i.v.e.l.l.o. .
-00005880: 6300 6f00 6d00 7000 6f00 6e00 6500 6e00  c.o.m.p.o.n.e.n.
-00005890: 7400 6900 2000 6200 6100 6e00 6400 6100  t.i. .b.a.n.d.a.
-000058a0: 2000 7300 7400 7200 6500 7400 7400 6100   .s.t.r.e.t.t.a.
-000058b0: 2000 2800 6400 4200 2000 5300 5000 4c00   .(.d.B. .S.P.L.
-000058c0: 2908 0000 0000 0600 0000 244e 6172 726f  ).........$Narro
-000058d0: 7720 4261 6e64 2043 6f6d 706f 6e65 6e74  w Band Component
-000058e0: 204c 6576 656c 2028 6442 2053 504c 2907   Level (dB SPL).
-000058f0: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
-00005900: 6444 6961 6c6f 6701 0300 0000 2c00 5200  dDialog.....,.R.
-00005910: 7500 6d00 6f00 7200 6500 2000 6100 2000  u.m.o.r.e. .a. .
-00005920: 6200 6100 6e00 6400 6100 2000 7300 7400  b.a.n.d.a. .s.t.
-00005930: 7200 6500 7400 7400 6108 0000 0000 0600  r.e.t.t.a.......
-00005940: 0000 104e 6172 726f 7762 616e 6420 4e6f  ...Narrowband No
-00005950: 6973 6507 0000 0013 6765 6e65 7261 7465  ise.....generate
-00005960: 536f 756e 6444 6961 6c6f 6701 0300 0000  SoundDialog.....
-00005970: 4200 5200 7500 6d00 6f00 7200 6500 2000  B.R.u.m.o.r.e. .
-00005980: 3100 2000 6600 7200 6500 7100 7500 6500  1. .f.r.e.q.u.e.
-00005990: 6e00 7a00 6100 2000 7300 7500 7000 6500  n.z.a. .s.u.p.e.
-000059a0: 7200 6900 6f00 7200 6500 2000 2800 4800  r.i.o.r.e. .(.H.
-000059b0: 7a00 2908 0000 0000 0600 0000 154e 6f2e  z.)..........No.
-000059c0: 2031 2048 6967 6820 4672 6571 2e20 2848   1 High Freq. (H
-000059d0: 7a29 0700 0000 1367 656e 6572 6174 6553  z).....generateS
-000059e0: 6f75 6e64 4469 616c 6f67 0103 0000 0042  oundDialog.....B
-000059f0: 0052 0075 006d 006f 0072 0065 0020 0031  .R.u.m.o.r.e. .1
-00005a00: 0020 0066 0072 0065 0071 0075 0065 006e  . .f.r.e.q.u.e.n
-00005a10: 007a 0061 0020 0069 006e 0066 0065 0072  .z.a. .i.n.f.e.r
-00005a20: 0069 006f 0072 0065 0020 0028 0048 007a  .i.o.r.e. .(.H.z
-00005a30: 0029 0800 0000 0006 0000 0014 4e6f 2e20  .)..........No. 
-00005a40: 3120 4c6f 7720 4672 6571 2e20 2848 7a29  1 Low Freq. (Hz)
-00005a50: 0700 0000 1367 656e 6572 6174 6553 6f75  .....generateSou
-00005a60: 6e64 4469 616c 6f67 0103 0000 0032 004c  ndDialog.....2.L
-00005a70: 0069 0076 0065 006c 006c 006f 0020 0072  .i.v.e.l.l.o. .r
-00005a80: 0075 006d 006f 0072 0065 0020 0031 0020  .u.m.o.r.e. .1. 
-00005a90: 0028 0064 0042 0020 0053 0050 004c 0029  .(.d.B. .S.P.L.)
-00005aa0: 0800 0000 0006 0000 0017 4e6f 2e20 3120  ..........No. 1 
-00005ab0: 532e 204c 6576 656c 2028 6442 2053 504c  S. Level (dB SPL
-00005ac0: 2907 0000 0013 6765 6e65 7261 7465 536f  ).....generateSo
-00005ad0: 756e 6444 6961 6c6f 6701 0300 0000 4200  undDialog.....B.
-00005ae0: 5200 7500 6d00 6f00 7200 6500 2000 3100  R.u.m.o.r.e. .1.
-00005af0: 2000 6600 7200 6500 7100 7500 6500 6e00   .f.r.e.q.u.e.n.
-00005b00: 7a00 6100 2000 7300 7500 7000 6500 7200  z.a. .s.u.p.e.r.
-00005b10: 6900 6f00 7200 6500 2000 2800 4800 7a00  i.o.r.e. .(.H.z.
-00005b20: 2908 0000 0000 0600 0000 154e 6f2e 2032  )..........No. 2
-00005b30: 2048 6967 6820 4672 6571 2e20 2848 7a29   High Freq. (Hz)
-00005b40: 0700 0000 1367 656e 6572 6174 6553 6f75  .....generateSou
-00005b50: 6e64 4469 616c 6f67 0103 0000 0042 0052  ndDialog.....B.R
-00005b60: 0075 006d 006f 0072 0065 0020 0032 0020  .u.m.o.r.e. .2. 
-00005b70: 0066 0072 0065 0071 0075 0065 006e 007a  .f.r.e.q.u.e.n.z
-00005b80: 0061 0020 0069 006e 0066 0065 0072 0069  .a. .i.n.f.e.r.i
-00005b90: 006f 0072 0065 0020 0028 0048 007a 0029  .o.r.e. .(.H.z.)
-00005ba0: 0800 0000 0006 0000 0014 4e6f 2e20 3220  ..........No. 2 
-00005bb0: 4c6f 7720 4672 6571 2e20 2848 7a29 0700  Low Freq. (Hz)..
-00005bc0: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
-00005bd0: 4469 616c 6f67 0103 0000 0032 004c 0069  Dialog.....2.L.i
-00005be0: 0076 0065 006c 006c 006f 0020 0072 0075  .v.e.l.l.o. .r.u
-00005bf0: 006d 006f 0072 0065 0020 0032 0020 0028  .m.o.r.e. .2. .(
-00005c00: 0064 0042 0020 0053 0050 004c 0029 0800  .d.B. .S.P.L.)..
-00005c10: 0000 0006 0000 0017 4e6f 2e20 3220 532e  ........No. 2 S.
-00005c20: 204c 6576 656c 2028 6442 2053 504c 2907   Level (dB SPL).
-00005c30: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
-00005c40: 6444 6961 6c6f 6701 0300 0000 0a00 4e00  dDialog.......N.
-00005c50: 6f00 5300 7000 6908 0000 0000 0600 0000  o.S.p.i.........
-00005c60: 054e 6f53 7069 0700 0000 1367 656e 6572  .NoSpi.....gener
-00005c70: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-00005c80: 0000 0018 0054 0069 0070 006f 0020 0072  .....T.i.p.o. .r
-00005c90: 0075 006d 006f 0072 0065 003a 0800 0000  .u.m.o.r.e.:....
-00005ca0: 0006 0000 000b 4e6f 6973 6520 5479 7065  ......Noise Type
-00005cb0: 3a07 0000 0013 6765 6e65 7261 7465 536f  :.....generateSo
-00005cc0: 756e 6444 6961 6c6f 6701 0300 0000 0e00  undDialog.......
-00005cd0: 4e00 6500 7300 7300 7500 6e00 6f08 0000  N.e.s.s.u.n.o...
-00005ce0: 0000 0600 0000 044e 6f6e 6507 0000 0013  .......None.....
-00005cf0: 6765 6e65 7261 7465 536f 756e 6444 6961  generateSoundDia
-00005d00: 6c6f 6701 0300 0000 0a00 4e00 7000 6900  log.......N.p.i.
-00005d10: 5300 6f08 0000 0000 0600 0000 054e 7069  S.o..........Npi
-00005d20: 536f 0700 0000 1367 656e 6572 6174 6553  So.....generateS
-00005d30: 6f75 6e64 4469 616c 6f67 0103 0000 0024  oundDialog.....$
-00005d40: 0044 0069 0073 0070 0061 0072 0069 0020  .D.i.s.p.a.r.i. 
-00005d50: 0061 0020 0073 0069 006e 0069 0073 0074  .a. .s.i.n.i.s.t
-00005d60: 0072 0061 0800 0000 0006 0000 0008 4f64  .r.a..........Od
-00005d70: 6420 4c65 6674 0700 0000 1367 656e 6572  d Left.....gener
-00005d80: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-00005d90: 0000 0020 0044 0069 0073 0070 0061 0072  ... .D.i.s.p.a.r
-00005da0: 0069 0020 0061 0020 0064 0065 0073 0074  .i. .a. .d.e.s.t
-00005db0: 0072 0061 0800 0000 0006 0000 0009 4f64  .r.a..........Od
-00005dc0: 6420 5269 6768 7407 0000 0013 6765 6e65  d Right.....gene
-00005dd0: 7261 7465 536f 756e 6444 6961 6c6f 6701  rateSoundDialog.
-00005de0: 0300 0000 2400 5200 6500 6c00 6100 7a00  ....$.R.e.l.a.z.
-00005df0: 6900 6f00 6e00 6500 2000 6400 6900 2000  i.o.n.e. .d.i. .
-00005e00: 6600 6100 7300 6500 3a08 0000 0000 0600  f.a.s.e.:.......
-00005e10: 0000 1350 6861 7365 2072 656c 6174 696f  ...Phase relatio
-00005e20: 6e73 6869 703a 0700 0000 1367 656e 6572  nship:.....gener
-00005e30: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-00005e40: 0000 000a 0046 0061 0073 0065 003a 0800  .....F.a.s.e.:..
-00005e50: 0000 0006 0000 0006 5068 6173 653a 0700  ........Phase:..
-00005e60: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
-00005e70: 4469 616c 6f67 0103 0000 0008 0052 006f  Dialog.......R.o
-00005e80: 0073 0061 0800 0000 0006 0000 0004 5069  .s.a..........Pi
-00005e90: 6e6b 0700 0000 1367 656e 6572 6174 6553  nk.....generateS
-00005ea0: 6f75 6e64 4469 616c 6f67 0103 0000 0014  oundDialog......
-00005eb0: 0052 0061 006d 0070 0061 0020 0028 0073  .R.a.m.p.a. .(.s
-00005ec0: 006d 0029 0800 0000 0006 0000 0009 5261  .m.)..........Ra
-00005ed0: 6d70 2028 6d73 2907 0000 0013 6765 6e65  mp (ms).....gene
-00005ee0: 7261 7465 536f 756e 6444 6961 6c6f 6701  rateSoundDialog.
-00005ef0: 0300 0000 1800 5200 6100 6e00 6400 6f00  ......R.a.n.d.o.
-00005f00: 6d00 6900 7a00 7a00 6100 7400 6108 0000  m.i.z.z.a.t.a...
-00005f10: 0000 0600 0000 0652 616e 646f 6d07 0000  .......Random...
-00005f20: 0013 6765 6e65 7261 7465 536f 756e 6444  ..generateSoundD
-00005f30: 6961 6c6f 6701 0300 0000 0c00 4400 6500  ialog.......D.e.
-00005f40: 7300 7400 7200 6f08 0000 0000 0600 0000  s.t.r.o.........
-00005f50: 0552 6967 6874 0700 0000 1367 656e 6572  .Right.....gener
-00005f60: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-00005f70: 0000 0034 0046 0072 0065 0071 0075 0065  ...4.F.r.e.q.u.e
-00005f80: 006e 007a 0061 0020 0064 0069 0020 0063  .n.z.a. .d.i. .c
-00005f90: 0061 006d 0070 0069 006f 006e 0061 006d  .a.m.p.i.o.n.a.m
-00005fa0: 0065 006e 0074 006f 0800 0000 0006 0000  .e.n.t.o........
-00005fb0: 000d 5361 6d70 6c69 6e67 2052 6174 6507  ..Sampling Rate.
-00005fc0: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
-00005fd0: 6444 6961 6c6f 6701 0300 0000 1200 5300  dDialog.......S.
-00005fe0: 6300 6800 7200 6f00 6500 6400 6500 7208  c.h.r.o.e.d.e.r.
-00005ff0: 0000 0000 0600 0000 0953 6368 726f 6564  .........Schroed
-00006000: 6572 0700 0000 1367 656e 6572 6174 6553  er.....generateS
-00006010: 6f75 6e64 4469 616c 6f67 0103 0000 0006  oundDialog......
-00006020: 0053 0069 006e 0800 0000 0006 0000 0004  .S.i.n..........
-00006030: 5369 6e65 0700 0000 1367 656e 6572 6174  Sine.....generat
-00006040: 6553 6f75 6e64 4469 616c 6f67 0103 0000  eSoundDialog....
-00006050: 0012 0053 0069 006e 0075 0073 006f 0069  ...S.i.n.u.s.o.i
-00006060: 0064 0065 0800 0000 0006 0000 0008 5369  .d.e..........Si
-00006070: 6e75 736f 6964 0700 0000 1367 656e 6572  nusoid.....gener
-00006080: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
-00006090: 0000 0016 004e 006f 006d 0065 0020 0053  .....N.o.m.e. .S
-000060a0: 0075 006f 006e 006f 003a 0800 0000 0006  .u.o.n.o.:......
-000060b0: 0000 000d 536f 756e 6420 4c61 6265 6c3a  ....Sound Label:
-000060c0: 2007 0000 0013 6765 6e65 7261 7465 536f   .....generateSo
-000060d0: 756e 6444 6961 6c6f 6701 0300 0000 2c00  undDialog.....,.
-000060e0: 4900 6e00 7400 6500 7200 7600 6100 6c00  I.n.t.e.r.v.a.l.
-000060f0: 6c00 6f00 2000 2800 6300 6500 6e00 7400  l.o. .(.c.e.n.t.
-00006100: 6500 7300 6900 6d00 6900 2908 0000 0000  e.s.i.m.i.).....
-00006110: 0600 0000 0f53 7061 6369 6e67 2028 4365  .....Spacing (Ce
-00006120: 6e74 7329 0700 0000 1367 656e 6572 6174  nts).....generat
-00006130: 6553 6f75 6e64 4469 616c 6f67 0103 0000  eSoundDialog....
-00006140: 0034 004c 0069 0076 0065 006c 006c 006f  .4.L.i.v.e.l.l.o
-00006150: 0020 0073 0070 0065 0074 0074 0072 0061  . .s.p.e.t.t.r.a
-00006160: 006c 0065 0020 0028 0064 0042 0020 0053  .l.e. .(.d.B. .S
-00006170: 0050 004c 0029 0800 0000 0006 0000 0017  .P.L.)..........
-00006180: 5370 6563 7472 756d 204c 6576 656c 2028  Spectrum Level (
-00006190: 6442 2053 504c 2907 0000 0013 6765 6e65  dB SPL).....gene
-000061a0: 7261 7465 536f 756e 6444 6961 6c6f 6701  rateSoundDialog.
-000061b0: 0300 0000 2000 4100 6c00 6c00 7500 6e00  .... .A.l.l.u.n.
-000061c0: 6700 6100 6d00 6500 6e00 7400 6f00 2000  g.a.m.e.n.t.o. .
-000061d0: 2800 2500 2908 0000 0000 0600 0000 0b53  (.%.)..........S
-000061e0: 7472 6574 6368 2028 2529 0700 0000 1367  tretch (%).....g
-000061f0: 656e 6572 6174 6553 6f75 6e64 4469 616c  enerateSoundDial
-00006200: 6f67 0103 0000 000a 0054 0069 0070 006f  og.......T.i.p.o
-00006210: 003a 0800 0000 0006 0000 0005 5479 7065  .:..........Type
-00006220: 3a07 0000 0013 6765 6e65 7261 7465 536f  :.....generateSo
-00006230: 756e 6444 6961 6c6f 6701 0300 0000 0c00  undDialog.......
-00006240: 4200 6900 6100 6e00 6300 6f08 0000 0000  B.i.a.n.c.o.....
-00006250: 0600 0000 0557 6869 7465 0700 0000 1367  .....White.....g
-00006260: 656e 6572 6174 6553 6f75 6e64 4469 616c  enerateSoundDial
-00006270: 6f67 0103 0000 001a 0043 006f 006c 006f  og.......C.o.l.o
-00006280: 0072 0065 0020 0073 0066 006f 006e 0064  .r.e. .s.f.o.n.d
-00006290: 006f 0800 0000 0006 0000 0010 4261 636b  .o..........Back
-000062a0: 6772 6f75 6e64 2043 6f6c 6f72 0700 0000  ground Color....
-000062b0: 1170 7265 6665 7265 6e63 6573 4469 616c  .preferencesDial
-000062c0: 6f67 0103 0000 0022 0043 006f 006c 006f  og.....".C.o.l.o
-000062d0: 0072 0065 0020 0063 0061 006e 006f 0076  .r.e. .c.a.n.o.v
-000062e0: 0061 0063 0063 0069 006f 0800 0000 0006  .a.c.c.i.o......
-000062f0: 0000 000c 4361 6e76 6173 2043 6f6c 6f72  ....Canvas Color
-00006300: 0700 0000 1170 7265 6665 7265 6e63 6573  .....preferences
-00006310: 4469 616c 6f67 0103 0000 001a 004d 0061  Dialog.......M.a
-00006320: 0070 0070 0061 0020 0063 006f 006c 006f  .p.p.a. .c.o.l.o
-00006330: 0072 0065 003a 0800 0000 0006 0000 000a  .r.e.:..........
-00006340: 436f 6c6f 7220 4d61 703a 0700 0000 1170  Color Map:.....p
-00006350: 7265 6665 7265 6e63 6573 4469 616c 6f67  referencesDialog
-00006360: 0103 0000 0010 0043 006f 006d 0061 006e  .......C.o.m.a.n
-00006370: 0064 006f 003a 0800 0000 0006 0000 0008  .d.o.:..........
-00006380: 436f 6d6d 616e 643a 0700 0000 1170 7265  Command:.....pre
-00006390: 6665 7265 6e63 6573 4469 616c 6f67 0103  ferencesDialog..
-000063a0: 0000 0038 004e 0061 007a 0069 006f 006e  ...8.N.a.z.i.o.n
-000063b0: 0065 0020 0028 006e 0065 0063 0065 0073  .e. .(.n.e.c.e.s
-000063c0: 0073 0069 0074 0061 0020 0072 0069 0061  .s.i.t.a. .r.i.a
-000063d0: 0076 0076 0069 006f 0029 003a 0800 0000  .v.v.i.o.).:....
-000063e0: 0006 0000 001b 436f 756e 7472 7920 2872  ......Country (r
-000063f0: 6571 7569 7265 7320 7265 7374 6172 7429  equires restart)
-00006400: 3a07 0000 0011 7072 6566 6572 656e 6365  :.....preference
-00006410: 7344 6961 6c6f 6701 0300 0000 2400 4400  sDialog.....$.D.
-00006420: 5000 4900 2000 2d00 2000 7200 6900 7300  P.I. .-. .r.i.s.
-00006430: 6f00 6c00 7500 7a00 6900 6f00 6e00 6500  o.l.u.z.i.o.n.e.
-00006440: 3a08 0000 0000 0600 0000 1144 5049 202d  :..........DPI -
-00006450: 2052 6573 6f6c 7574 696f 6e3a 0700 0000   Resolution:....
-00006460: 1170 7265 6665 7265 6e63 6573 4469 616c  .preferencesDial
-00006470: 6f67 0103 0000 000e 0047 0072 0069 0067  og.......G.r.i.g
-00006480: 006c 0069 0061 0800 0000 0006 0000 0004  .l.i.a..........
-00006490: 4772 6964 0700 0000 1170 7265 6665 7265  Grid.....prefere
-000064a0: 6e63 6573 4469 616c 6f67 0103 0000 0036  ncesDialog.....6
-000064b0: 004c 0069 006e 0067 0075 0061 0020 0028  .L.i.n.g.u.a. .(
-000064c0: 006e 0065 0063 0065 0073 0073 0069 0074  .n.e.c.e.s.s.i.t
-000064d0: 0061 0020 0072 0069 0061 0076 0076 0069  .a. .r.i.a.v.v.i
-000064e0: 006f 0029 003a 0800 0000 0006 0000 001c  .o.).:..........
-000064f0: 4c61 6e67 7561 6765 2028 7265 7175 6972  Language (requir
-00006500: 6573 2072 6573 7461 7274 293a 0700 0000  es restart):....
-00006510: 1170 7265 6665 7265 6e63 6573 4469 616c  .preferencesDial
-00006520: 6f67 0103 0000 0018 0043 006f 006c 006f  og.......C.o.l.o
-00006530: 0072 0065 0020 006c 0069 006e 0065 0061  .r.e. .l.i.n.e.a
-00006540: 0800 0000 0006 0000 000a 4c69 6e65 2043  ..........Line C
-00006550: 6f6c 6f72 0700 0000 1170 7265 6665 7265  olor.....prefere
-00006560: 6e63 6573 4469 616c 6f67 0103 0000 0018  ncesDialog......
-00006570: 004c 0069 0076 0065 006c 006c 006f 0020  .L.i.v.e.l.l.o. 
-00006580: 004d 0061 0078 003a 0800 0000 0006 0000  .M.a.x.:........
-00006590: 000a 4d61 7820 4c65 7665 6c3a 0700 0000  ..Max Level:....
-000065a0: 1170 7265 6665 7265 6e63 6573 4469 616c  .preferencesDial
-000065b0: 6f67 0103 0000 002a 0043 006f 006d 0061  og.....*.C.o.m.a
-000065c0: 006e 0064 006f 0020 0072 0069 0070 0072  .n.d.o. .r.i.p.r
-000065d0: 006f 0064 0075 007a 0069 006f 006e 0065  .o.d.u.z.i.o.n.e
-000065e0: 003a 0800 0000 0006 0000 000d 506c 6179  .:..........Play
-000065f0: 2043 6f6d 6d61 6e64 3a07 0000 0011 7072   Command:.....pr
-00006600: 6566 6572 656e 6365 7344 6961 6c6f 6701  eferencesDialog.
-00006610: 0300 0000 1000 4700 7200 6100 6600 6900  ......G.r.a.f.i.
-00006620: 6300 2600 6908 0000 0000 0600 0000 0650  c.&.i..........P
-00006630: 6c6f 7426 7307 0000 0011 7072 6566 6572  lot&s.....prefer
-00006640: 656e 6365 7344 6961 6c6f 6701 0300 0000  encesDialog.....
-00006650: 1000 5300 6500 6700 6e00 6100 6c00 2600  ..S.e.g.n.a.l.&.
-00006660: 6508 0000 0000 0600 0000 0753 6967 6e61  e..........Signa
-00006670: 266c 0700 0000 1170 7265 6665 7265 6e63  &l.....preferenc
-00006680: 6573 4469 616c 6f67 0103 0000 000c 0053  esDialog.......S
-00006690: 0075 006f 006e 0026 006f 0800 0000 0006  .u.o.n.&.o......
-000066a0: 0000 0006 536f 756e 2664 0700 0000 1170  ....Soun&d.....p
-000066b0: 7265 6665 7265 6e63 6573 4469 616c 6f67  referencesDialog
-000066c0: 0103 0000 000c 0041 0076 0076 0069 0073  .......A.v.v.i.s
-000066d0: 006f 0800 0000 0006 0000 0007 5761 726e  .o..........Warn
-000066e0: 696e 6707 0000 0011 7072 6566 6572 656e  ing.....preferen
-000066f0: 6365 7344 6961 6c6f 6701 0300 0000 3e00  cesDialog.....>.
-00006700: 5700 6100 7600 2000 4d00 6100 6e00 6100  W.a.v. .M.a.n.a.
-00006710: 6700 6500 7200 2000 2800 7200 6900 6300  g.e.r. .(.r.i.c.
-00006720: 6800 6900 6500 6400 6500 2000 7200 6900  h.i.e.d.e. .r.i.
-00006730: 6100 7600 7600 6900 6f00 2900 3a08 0000  a.v.v.i.o.).:...
-00006740: 0000 0600 0000 0c57 6176 204d 616e 6167  .......Wav Manag
-00006750: 6572 3a07 0000 0011 7072 6566 6572 656e  er:.....preferen
-00006760: 6365 7344 6961 6c6f 6701 0300 0000 1200  cesDialog.......
-00006770: 4600 6900 6e00 6500 7300 7400 7200 6100  F.i.n.e.s.t.r.a.
-00006780: 3a08 0000 0000 0600 0000 0757 696e 646f  :..........Windo
-00006790: 773a 0700 0000 1170 7265 6665 7265 6e63  w:.....preferenc
-000067a0: 6573 4469 616c 6f67 0103 0000 001c 0070  esDialog.......p
-000067b0: 0065 0072 0073 006f 006e 0061 006c 0069  .e.r.s.o.n.a.l.i
-000067c0: 007a 007a 0061 0074 006f 0800 0000 0006  .z.z.a.t.o......
-000067d0: 0000 0006 6375 7374 6f6d 0700 0000 1170  ....custom.....p
-000067e0: 7265 6665 7265 6e63 6573 4469 616c 6f67  referencesDialog
-000067f0: 0103 0000 002a 0076 0061 006c 006f 0072  .....*.v.a.l.o.r
-00006800: 0065 0020 0064 0070 0069 0020 006e 006f  .e. .d.p.i. .n.o
-00006810: 006e 0020 0076 0061 006c 0069 0064 006f  .n. .v.a.l.i.d.o
-00006820: 0800 0000 0006 0000 0013 6470 6920 7661  ..........dpi va
-00006830: 6c75 6520 6e6f 7420 7661 6c69 6407 0000  lue not valid...
-00006840: 0011 7072 6566 6572 656e 6365 7344 6961  ..preferencesDia
-00006850: 6c6f 6701 0300 0000 3200 7600 6100 6c00  log.....2.v.a.l.
-00006860: 6f00 7200 6500 2000 6400 7000 6900 2000  o.r.e. .d.p.i. .
-00006870: 7400 7200 6f00 7000 7000 6f00 2000 7000  t.r.o.p.p.o. .p.
-00006880: 6900 6300 6300 6f00 6c00 6f08 0000 0000  i.c.c.o.l.o.....
-00006890: 0600 0000 1364 7069 2076 616c 7565 2074  .....dpi value t
-000068a0: 6f6f 2073 6d61 6c6c 0700 0000 1170 7265  oo small.....pre
-000068b0: 6665 7265 6e63 6573 4469 616c 6f67 0103  ferencesDialog..
-000068c0: 0000 003c 004e 0075 006f 0076 0061 0020  ...<.N.u.o.v.a. 
-000068d0: 0066 0072 0065 0071 0075 0065 006e 007a  .f.r.e.q.u.e.n.z
-000068e0: 0061 0020 0063 0061 006d 0070 0069 006f  .a. .c.a.m.p.i.o
-000068f0: 006e 0061 006d 0065 006e 0074 006f 003a  .n.a.m.e.n.t.o.:
-00006900: 0800 0000 0006 0000 0013 4e65 7720 5361  ..........New Sa
-00006910: 6d70 6c69 6e67 2052 6174 653a 2007 0000  mpling Rate: ...
-00006920: 000e 7265 7361 6d70 6c65 4469 616c 6f67  ..resampleDialog
-00006930: 0103 0000 0050 0046 0072 0065 0071 0075  .....P.F.r.e.q.u
-00006940: 0065 006e 007a 0061 0020 0064 0069 0020  .e.n.z.a. .d.i. 
-00006950: 0063 0061 006d 0070 0069 006f 006e 0061  .c.a.m.p.i.o.n.a
-00006960: 006d 0065 006e 0074 006f 0020 0063 006f  .m.e.n.t.o. .c.o
-00006970: 0072 0072 0065 006e 0074 0065 003a 0020  .r.r.e.n.t.e.:. 
-00006980: 0025 004c 0031 0800 0000 0006 0000 001b  .%.L.1..........
-00006990: 4e65 7720 7361 6d70 6c69 6e67 2072 6174  New sampling rat
-000069a0: 6520 746f 6f20 736d 616c 6c07 0000 000e  e too small.....
-000069b0: 7265 7361 6d70 6c65 4469 616c 6f67 0103  resampleDialog..
-000069c0: 0000 0014 0052 0069 0063 0061 006d 0070  .....R.i.c.a.m.p
-000069d0: 0069 006f 006e 0061 0800 0000 0006 0000  .i.o.n.a........
-000069e0: 0008 5265 7361 6d70 6c65 0700 0000 0e72  ..Resample.....r
-000069f0: 6573 616d 706c 6544 6961 6c6f 6701 0300  esampleDialog...
-00006a00: 0000 3a00 4100 6c00 6700 6f00 7200 6900  ..:.A.l.g.o.r.i.
-00006a10: 7400 6d00 6f00 2000 6400 6900 2000 7200  t.m.o. .d.i. .r.
-00006a20: 6900 6300 6100 6d00 7000 6900 6f00 6e00  i.c.a.m.p.i.o.n.
-00006a30: 6100 6d00 6500 6e00 7400 6f00 3a08 0000  a.m.e.n.t.o.:...
-00006a40: 0000 0600 0000 1652 6573 616d 706c 696e  .......Resamplin
-00006a50: 6720 416c 676f 7269 7468 6d3a 2007 0000  g Algorithm: ...
-00006a60: 000e 7265 7361 6d70 6c65 4469 616c 6f67  ..resampleDialog
-00006a70: 0103 0000 000c 0041 0076 0076 0069 0073  .......A.v.v.i.s
-00006a80: 006f 0800 0000 0006 0000 0007 5761 726e  .o..........Warn
-00006a90: 696e 6707 0000 000e 7265 7361 6d70 6c65  ing.....resample
-00006aa0: 4469 616c 6f67 0103 0000 0024 0054 0069  Dialog.....$.T.i
-00006ab0: 0070 006f 0020 0064 0069 0020 0066 0069  .p.o. .d.i. .f.i
-00006ac0: 006e 0073 0065 0073 0074 0072 0061 003a  .n.s.e.s.t.r.a.:
-00006ad0: 0800 0000 0006 0000 000d 5769 6e64 6f77  ..........Window
-00006ae0: 2054 7970 653a 2007 0000 000e 7265 7361   Type: .....resa
-00006af0: 6d70 6c65 4469 616c 6f67 0103 ffff ffff  mpleDialog......
-00006b00: 0800 0000 0006 0000 0006 4269 7473 3a20  ..........Bits: 
-00006b10: 0700 0000 0f73 6176 6553 6f75 6e64 4469  .....saveSoundDi
-00006b20: 616c 6f67 0103 0000 000e 0043 0061 006e  alog.......C.a.n
-00006b30: 0061 006c 0065 003a 0800 0000 0006 0000  .a.l.e.:........
-00006b40: 0009 4368 616e 6e65 6c3a 2007 0000 000f  ..Channel: .....
-00006b50: 7361 7665 536f 756e 6444 6961 6c6f 6701  saveSoundDialog.
-00006b60: 0300 0000 1a00 4600 6f00 7200 6d00 6100  ......F.o.r.m.a.
-00006b70: 7400 6f00 2000 6600 6900 6c00 6500 3a08  t.o. .f.i.l.e.:.
-00006b80: 0000 0000 0600 0000 0d46 696c 6520 466f  .........File Fo
-00006b90: 726d 6174 3a20 0700 0000 0f73 6176 6553  rmat: .....saveS
-00006ba0: 6f75 6e64 4469 616c 6f67 0103 ffff ffff  oundDialog......
-00006bb0: 0800 0000 0006 0000 0004 4d6f 6e6f 0700  ..........Mono..
-00006bc0: 0000 0f73 6176 6553 6f75 6e64 4469 616c  ...saveSoundDial
-00006bd0: 6f67 0103 0000 003a 004f 0070 007a 0069  og.....:.O.p.z.i
-00006be0: 006f 006e 0069 0020 0073 0061 006c 0076  .o.n.i. .s.a.l.v
-00006bf0: 0061 0074 0061 0067 0067 0069 006f 0020  .a.t.a.g.g.i.o. 
-00006c00: 0064 0065 006c 0020 0073 0075 006f 006e  .d.e.l. .s.u.o.n
-00006c10: 006f 0800 0000 0006 0000 0012 5361 7665  .o..........Save
-00006c20: 2053 6f75 6e64 204f 7074 696f 6e73 0700   Sound Options..
-00006c30: 0000 0f73 6176 6553 6f75 6e64 4469 616c  ...saveSoundDial
-00006c40: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00006c50: 0006 5374 6572 656f 0700 0000 0f73 6176  ..Stereo.....sav
-00006c60: 6553 6f75 6e64 4469 616c 6f67 0103 0000  eSoundDialog....
-00006c70: 001a 004d 0061 0070 0070 0061 0020 0063  ...M.a.p.p.a. .c
-00006c80: 006f 006c 006f 0072 0069 003a 0800 0000  .o.l.o.r.i.:....
-00006c90: 0006 0000 000a 436f 6c6f 7220 4d61 703a  ......Color Map:
-00006ca0: 0700 0000 0f73 7065 6374 726f 6772 616d  .....spectrogram
-00006cb0: 506c 6f74 0103 0000 0012 0054 0065 006d  Plot.......T.e.m
-00006cc0: 0070 006f 0020 0028 0073 0029 0800 0000  .p.o. .(.s.)....
-00006cd0: 0006 0000 0008 4c6f 6720 6178 6973 0700  ......Log axis..
-00006ce0: 0000 0f73 7065 6374 726f 6772 616d 506c  ...spectrogramPl
-00006cf0: 6f74 0103 0000 0026 0053 006f 0076 0072  ot.....&.S.o.v.r
-00006d00: 0061 0070 0070 006f 0073 0069 007a 0069  .a.p.p.o.s.i.z.i
-00006d10: 006f 006e 0065 0020 0028 0025 0029 0800  .o.n.e. .(.%.)..
-00006d20: 0000 0006 0000 000b 4f76 6572 6c61 7020  ........Overlap 
-00006d30: 2825 2907 0000 000f 7370 6563 7472 6f67  (%).....spectrog
-00006d40: 7261 6d50 6c6f 7401 0300 0000 1800 5000  ramPlot.......P.
-00006d50: 6f00 7400 6500 6e00 7a00 6100 2000 6400  o.t.e.n.z.a. .d.
-00006d60: 6900 2000 3208 0000 0000 0600 0000 0a50  i. .2..........P
-00006d70: 6f77 6572 206f 6620 3207 0000 000f 7370  ower of 2.....sp
-00006d80: 6563 7472 6f67 7261 6d50 6c6f 7401 0300  ectrogramPlot...
-00006d90: 0000 2600 4400 7500 7200 6100 7400 6100  ..&.D.u.r.a.t.a.
-00006da0: 2000 4600 6900 6e00 6500 7300 7400 7200   .F.i.n.e.s.t.r.
-00006db0: 6100 2000 2800 7300 2908 0000 0000 0600  a. .(.s.).......
-00006dc0: 0000 1157 696e 646f 7720 4c65 6e67 7468  ...Window Length
-00006dd0: 2028 7329 0700 0000 0f73 7065 6374 726f   (s).....spectro
-00006de0: 6772 616d 506c 6f74 0103 0000 0012 0046  gramPlot.......F
-00006df0: 0069 006e 0065 0073 0074 0072 0061 003a  .i.n.e.s.t.r.a.:
-00006e00: 0800 0000 0006 0000 0007 5769 6e64 6f77  ..........Window
-00006e10: 3a07 0000 000f 7370 6563 7472 6f67 7261  :.....spectrogra
-00006e20: 6d50 6c6f 7401 0300 0000 2000 4400 6900  mPlot..... .D.i.
-00006e30: 6100 6c00 6f00 6700 6f00 2000 6400 6900  a.l.o.g.o. .d.i.
-00006e40: 2000 6900 6e00 7000 7500 7408 0000 0000   .i.n.p.u.t.....
-00006e50: 0600 0000 0c49 6e70 7574 2044 6961 6c6f  .....Input Dialo
-00006e60: 6707 0000 000c 7370 6563 7472 756d 506c  g.....spectrumPl
-00006e70: 6f74 0103 0000 0018 0043 006f 006c 006f  ot.......C.o.l.o
-00006e80: 0072 0065 0020 006c 0069 006e 0065 0061  .r.e. .l.i.n.e.a
-00006e90: 0800 0000 0006 0000 000a 4c69 6e65 2043  ..........Line C
-00006ea0: 6f6c 6f72 0700 0000 0c73 7065 6374 7275  olor.....spectru
-00006eb0: 6d50 6c6f 7401 0300 0000 1c00 5300 7000  mPlot.......S.p.
-00006ec0: 6500 7300 7300 6f00 7200 6500 2000 4c00  e.s.s.o.r.e. .L.
-00006ed0: 6900 6e00 6500 6108 0000 0000 0600 0000  i.n.e.a.........
-00006ee0: 0a4c 696e 6520 5769 6474 6807 0000 000c  .Line Width.....
-00006ef0: 7370 6563 7472 756d 506c 6f74 0103 0000  spectrumPlot....
-00006f00: 001e 0053 0070 0065 0073 0073 006f 0072  ...S.p.e.s.s.o.r
-00006f10: 0065 0020 004c 0069 006e 0065 0061 003a  .e. .L.i.n.e.a.:
-00006f20: 0800 0000 0006 0000 000b 4c69 6e65 2057  ..........Line W
-00006f30: 6964 7468 3a07 0000 000c 7370 6563 7472  idth:.....spectr
-00006f40: 756d 506c 6f74 0103 0000 0010 004c 006f  umPlot.......L.o
-00006f50: 0067 0020 0061 0073 0073 0065 0800 0000  .g. .a.s.s.e....
-00006f60: 0006 0000 0008 4c6f 6720 6178 6973 0700  ......Log axis..
-00006f70: 0000 0c73 7065 6374 7275 6d50 6c6f 7401  ...spectrumPlot.
-00006f80: 0300 0000 1800 5000 6f00 7400 6500 6e00  ......P.o.t.e.n.
-00006f90: 7a00 6100 2000 6400 6900 2000 3208 0000  z.a. .d.i. .2...
-00006fa0: 0000 0600 0000 0a50 6f77 6572 206f 6620  .......Power of 
-00006fb0: 3207 0000 000c 7370 6563 7472 756d 506c  2.....spectrumPl
-00006fc0: 6f74 0103 0000 0012 0046 0069 006e 0065  ot.......F.i.n.e
-00006fd0: 0073 0074 0072 0061 003a 0800 0000 0006  .s.t.r.a.:......
-00006fe0: 0000 0007 5769 6e64 6f77 3a07 0000 000c  ....Window:.....
-00006ff0: 7370 6563 7472 756d 506c 6f74 0103 0000  spectrumPlot....
-00007000: 0020 0044 0069 0061 006c 006f 0067 006f  . .D.i.a.l.o.g.o
-00007010: 0020 0064 0069 0020 0069 006e 0070 0075  . .d.i. .i.n.p.u
-00007020: 0074 0800 0000 0006 0000 000c 496e 7075  .t..........Inpu
-00007030: 7420 4469 616c 6f67 0700 0000 0c77 6176  t Dialog.....wav
-00007040: 6566 6f72 6d50 6c6f 7401 0300 0000 1800  eformPlot.......
-00007050: 4300 6f00 6c00 6f00 7200 6500 2000 6c00  C.o.l.o.r.e. .l.
-00007060: 6900 6e00 6500 6108 0000 0000 0600 0000  i.n.e.a.........
-00007070: 0a4c 696e 6520 436f 6c6f 7207 0000 000c  .Line Color.....
-00007080: 7761 7665 666f 726d 506c 6f74 0103 0000  waveformPlot....
-00007090: 001c 0053 0070 0065 0073 0073 006f 0072  ...S.p.e.s.s.o.r
-000070a0: 0065 0020 004c 0069 006e 0065 0061 0800  .e. .L.i.n.e.a..
-000070b0: 0000 0006 0000 000a 4c69 6e65 2057 6964  ........Line Wid
-000070c0: 7468 0700 0000 0c77 6176 6566 6f72 6d50  th.....waveformP
-000070d0: 6c6f 7401 0300 0000 1e00 5300 7000 6500  lot.......S.p.e.
-000070e0: 7300 7300 6f00 7200 6500 2000 4c00 6900  s.s.o.r.e. .L.i.
-000070f0: 6e00 6500 6100 3a08 0000 0000 0600 0000  n.e.a.:.........
-00007100: 0b4c 696e 6520 5769 6474 683a 0700 0000  .Line Width:....
-00007110: 0c77 6176 6566 6f72 6d50 6c6f 7401 8800  .waveformPlot...
-00007120: 0000 0201 01                             .....
+00000080: 0493 b500 002d 5000 0496 a800 0008 fd00  .....-P.........
+00000090: 0496 a800 002d 8200 0496 a800 0032 2000  .....-.......2 .
+000000a0: 0496 a800 0038 9900 04b8 5a00 003a 2e00  .....8....Z..:..
+000000b0: 04cf 0400 000e e800 04d7 fe00 003a fb00  .............:..
+000000c0: 04e8 f400 004e 2700 052b d400 0011 ec00  .....N'..+......
+000000d0: 052b d400 002a 1500 052b d400 002b 7700  .+...*...+...+w.
+000000e0: 052b d400 002e 9b00 052b d400 0034 2c00  .+.......+...4,.
+000000f0: 052b d400 0040 d800 0546 4f00 0013 6900  .+...@...FO...i.
+00000100: 0546 4f00 0055 5f00 0556 4500 0002 7800  .FO..U_..VE...x.
+00000110: 0556 4500 0015 f600 0556 4500 0046 7e00  .VE......VE..F~.
+00000120: 0570 4b00 001a 2400 0570 4b00 002f 6200  .pK...$..pK../b.
+00000130: 0570 4b00 0048 2b00 0572 8900 001a 5600  .pK..H+..r....V.
+00000140: 05a0 4500 0049 cf00 0756 4500 0021 c800  ..E..I...VE..!..
+00000150: 129f aa00 0000 cb00 129f aa00 003d 0c00  .............=..
+00000160: 2abb 0400 0004 fd00 2ad0 2500 0005 3a00  *.......*.%...:.
+00000170: 2aec 3000 0005 e600 2b73 6400 0006 1d00  *.0.....+sd.....
+00000180: 4949 7200 0024 5400 4b85 c000 002e 0c00  IIr..$T.K.......
+00000190: 4b85 c000 0032 b000 4f19 f500 0018 b600  K....2..O.......
+000001a0: 5278 bc00 0011 af00 554a 6900 0045 fc00  Rx......UJi..E..
+000001b0: 5560 9500 0015 bf00 5560 9500 002e d700  U`......U`......
+000001c0: 556e 9f00 0046 b800 58fd f400 001c c000  Un...F..X.......
+000001d0: 58fd f400 002a 5100 58fd f400 002c 0300  X....*Q.X....,..
+000001e0: 58fd f400 0030 1400 58fd f400 0035 a600  X....0..X....5..
+000001f0: 58fd f400 0048 ea00 5998 2500 001d 6e00  X....H..Y.%...n.
+00000200: 5c06 8a00 0002 ce00 5c06 8a00 004b b700  \.......\....K..
+00000210: 5c48 fa00 003f cf00 5ca0 5400 0002 9f00  \H...?..\.T.....
+00000220: 5ca0 5400 001e 8700 5ca0 5400 0036 4e00  \.T.....\.T..6N.
+00000230: 5ca0 5400 004a 0100 5df0 a500 0020 8c00  \.T..J..].... ..
+00000240: 5df0 a500 0031 a300 5df0 a500 004b ee00  ]....1..]....K..
+00000250: 5ed4 9500 0017 6a00 62ec a900 0033 a600  ^.....j.b....3..
+00000260: 8f43 1900 0045 8b00 f661 b000 002f 1001  .C...E...a.../..
+00000270: 2975 c900 0037 c001 2c40 7000 002b 1f01  )u...7..,@p..+..
+00000280: 2f38 2900 0040 4301 59c3 9000 0025 dc01  /8)..@C.Y....%..
+00000290: 6a24 5900 0012 ce01 728f 1e00 0008 2101  j$Y.....r.....!.
+000002a0: 8fc9 3d00 0008 7601 9176 c300 0023 4801  ..=...v..v...#H.
+000002b0: 979a 9000 002b b101 aa1f 3700 0003 3101  .....+....7...1.
+000002c0: aa1f 3700 0011 5d01 aa1f 3700 0057 da01  ..7...]...7..W..
+000002d0: aa1f 3700 0059 b101 bab5 4a00 004d 5301  ..7..Y....J..MS.
+000002e0: d21f e200 004c 7702 44ea 5c00 0052 e502  .....Lw.D.\..R..
+000002f0: 792f 0900 0003 7902 7a0f 5900 003a a902  y/....y.z.Y..:..
+00000300: 8fb8 6900 003b bf02 c844 c000 0031 dc02  ..i..;...D...1..
+00000310: d4e6 e900 0028 8d02 d4e6 e900 0056 a702  .....(.......V..
+00000320: da74 c500 000c df02 e914 f900 0038 3503  .t...........85.
+00000330: 006e 4a00 0023 1303 22c8 e300 000f 5803  .nJ..#..".....X.
+00000340: 2bd0 aa00 004f 6703 539b 6a00 004e 5f03  +....Og.S.j..N_.
+00000350: 5d16 1200 000a 7903 6e68 d300 0021 8703  ].....y.nh...!..
+00000360: 6e68 d300 0027 fb03 81c3 3a00 0034 b903  nh...'....:..4..
+00000370: 97bf 8500 001f a003 9f59 6a00 0050 ae03  .........Yj..P..
+00000380: e534 4300 0007 5c03 fe9a e500 001c f704  .4C...\.........
+00000390: 22cc d900 0048 5f04 26f4 6a00 0031 0104  "....H_.&.j..1..
+000003a0: 46c3 0900 001f 4e04 6c75 9000 0013 d604  F.....N.lu......
+000003b0: 90b6 c000 0054 af04 a6a0 4500 0039 4b04  .....T....E..9K.
+000003c0: ad42 4900 0038 d504 ee72 2200 0006 f105  .BI..8...r".....
+000003d0: 29f3 5a00 004f 1f05 2caf e200 0001 4405  ).Z..O..,.....D.
+000003e0: 2caf e200 0010 6e05 2caf e200 003f 0905  ,.....n.,....?..
+000003f0: 3315 6000 0052 7305 6e89 8a00 0047 f305  3.`..Rs.n....G..
+00000400: 7366 d300 004f c405 77c1 ba00 002f 9605  sf...O..w..../..
+00000410: 77c1 ba00 0035 1405 884b 5d00 0048 a405  w....5...K]..H..
+00000420: 8c46 c500 001b 9e05 8c48 3500 001c 2205  .F.......H5...".
+00000430: 8cbe ca00 0004 3205 8cbe ca00 0058 b105  ......2......X..
+00000440: 8cbe ca00 005a 8805 968c 3300 0056 6905  .....Z....3..Vi.
+00000450: 968c 3300 0058 fb05 a6c0 c400 0050 3d05  ..3..X.......P=.
+00000460: aac8 bf00 0055 f705 bb74 5a00 0026 9305  .....U...tZ..&..
+00000470: d062 c400 001f d905 d062 c400 0031 6b05  .b.......b...1k.
+00000480: dc7c 9300 002d 0105 dec6 0d00 0022 8f05  .|...-......."..
+00000490: f5b6 0500 0006 b406 0c4a 1300 0009 3706  .........J....7.
+000004a0: 419e 0a00 0028 4106 419e 0a00 004c cb06  A....(A.A....L..
+000004b0: 419e 0a00 0056 2106 4380 da00 004d 1506  A....V!.C....M..
+000004c0: 5874 7000 002a cd06 58a8 5400 0016 8006  Xtp..*..X.T.....
+000004d0: 58a8 5400 0047 4306 5a22 8400 000e 5406  X.T..GC.Z"....T.
+000004e0: 5d5f 3400 0012 8606 5fdb 1a00 0000 0006  ]_4....._.......
+000004f0: 5fdb 1a00 0039 7f06 9000 5300 003d bd06  _....9....S..=..
+00000500: 95b0 5000 0041 d206 9612 3900 0041 1406  ..P..A....9..A..
+00000510: acab 5d00 0051 5d06 b005 6000 0025 3106  ..]..Q]...`..%1.
+00000520: babc 1d00 001f 1206 c2cc 6c00 001b d806  ..........l.....
+00000530: d1ce 9e00 0014 1507 0f66 1a00 0002 4007  .........f....@.
+00000540: 0f66 1a00 0046 3307 145e 0400 000d 4b07  .f...F3..^....K.
+00000550: 2947 9500 0012 2607 2b54 9c00 001d a707  )G....&.+T......
+00000560: 4d73 2200 0003 b207 4d73 2200 004e d707  Ms".....Ms"..N..
+00000570: 4d73 2200 0058 2707 4d73 2200 0059 fe07  Ms"..X'.Ms"..Y..
+00000580: 58cb e800 0003 f007 58cb e800 0058 6a07  X.......X....Xj.
+00000590: 58cb e800 005a 4107 64a7 6c00 0029 8607  X....ZA.d.l..)..
+000005a0: 8f43 1900 0044 1d07 959e 1300 0006 4807  .C...D........H.
+000005b0: a0f5 ea00 0032 f207 a5d0 8200 004c 2707  .....2.......L'.
+000005c0: ebf7 9e00 0014 ec08 14f9 e000 002c b808  .............,..
+000005d0: 14f9 e000 0030 b608 14f9 e000 0036 9308  .....0.......6..
+000005e0: 14f9 e000 004a 4308 3230 2200 001b 3008  .....JC.20"...0.
+000005f0: 4b6e 2300 0020 c308 4b6e 2300 0027 2808  Kn#.. ..Kn#..'(.
+00000600: 4bad e000 0021 0508 4bad e000 0027 6f08  K....!..K....'o.
+00000610: 54f6 2000 0029 d608 54f6 2000 0054 d908  T. ..)..T. ..T..
+00000620: 611f a900 0028 e608 611f a900 0057 4208  a....(..a....WB.
+00000630: 62f8 b900 0033 e908 7045 0d00 0022 d308  b....3..pE..."..
+00000640: 9010 9300 0040 9208 9460 1300 0000 5108  .....@...`....Q.
+00000650: 9460 1300 003b 7d08 9525 8900 0043 9f08  .`...;}..%...C..
+00000660: 9555 8900 0045 0d08 9b34 a400 0033 4a08  .U...E...4...3J.
+00000670: adbf 4900 0042 1e08 c3c4 c000 0025 8608  ..I..B.......%..
+00000680: cbd3 5d00 0020 4808 d750 6400 0000 8008  ..].. H..Pd.....
+00000690: d750 6400 003c ae08 e22c 3500 000d 9208  .Pd..<...,5.....
+000006a0: e22c 3500 002a 8a09 0096 8700 0037 7b09  .,5..*.......7{.
+000006b0: 22cf 8900 003a 6c09 7437 4a00 0014 a709  "....:l.t7J.....
+000006c0: 8c74 d300 001d 2d09 a631 ac00 0052 0809  .t....-..1...R..
+000006d0: e854 fc00 000c a609 e96a 9900 003e b809  .T.......j...>..
+000006e0: f416 7e00 000f 1a09 fe43 9c00 0050 000a  ..~......C...P..
+000006f0: 02c4 c500 001e 4a0a 0e7a 7000 0053 b20a  ......J..zp..S..
+00000700: 4413 8500 0016 cf0a 652e 8400 0016 2e0a  D.......e.......
+00000710: 652e 8400 0046 ef0a 6594 4500 0037 330a  e....F..e.E..73.
+00000720: 8988 5000 0026 380a c092 b900 004b 640a  ..P..&8......Kd.
+00000730: e230 e400 0001 790a e230 e400 0010 b40a  .0....y..0......
+00000740: e230 e400 003f 510a e309 fe00 000a 220a  .0...?Q.......".
+00000750: eb66 0900 0007 ce0a ecea 8800 0001 020a  .f..............
+00000760: ecea 8800 0010 1b0a ecea 8800 003e 630a  .............>c.
+00000770: f5b6 0500 000f aa0b 16e8 3400 003b 2f0b  ..........4..;/.
+00000780: 1731 f900 0013 1d0b 19dc 7900 003c 300b  .1........y..<0.
+00000790: 19ec e500 002e 4b0b 3c48 1900 004a 8e0b  ......K.<H...J..
+000007a0: 8e85 7300 0055 870b 91f3 5000 0055 140b  ..s..U....P..U..
+000007b0: a3dc 0c00 001d fc0b c487 4300 000d d50b  ..........C.....
+000007c0: c4de 0000 0054 5b0b ef83 dd00 001e c70c  .....T[.........
+000007d0: 254e 0500 0019 690c 340d da00 0047 940c  %N....i.4....G..
+000007e0: 442e e200 0056 fc0c 442e e200 0059 340c  D....V..D....Y4.
+000007f0: 466e a000 002c 3a0c 466f a000 002c 790c  Fn...,:.Fo...,y.
+00000800: 4ca2 7500 0005 6f0c 62c7 de00 0002 f20c  L.u...o.b.......
+00000810: 7471 fa00 0024 e80c 7502 be00 0013 930c  tq...$..u.......
+00000820: 87a1 1c00 0036 e10c 9844 a500 001c 5e0c  .....6...D....^.
+00000830: 9844 a500 0053 730c 9d58 5000 0015 400c  .D...Ss..XP...@.
+00000840: a7e9 3a00 002d be0c a7e9 3a00 0032 5f0c  ..:..-....:..2_.
+00000850: b5cd 6000 0024 a70c c8fc 2500 0035 600c  ..`..$....%..5`.
+00000860: db87 9a00 004d cc0c ddc2 0300 001a eb0d  .....M..........
+00000870: 11fa 1500 0030 4d0d 11fa 1500 0035 e20d  .....0M......5..
+00000880: 11fa 1500 0049 230d 8950 1700 0020 0f0d  .....I#..P... ..
+00000890: 8950 1700 0050 750d 8950 1700 0054 250d  .P...Pu..P...T%.
+000008a0: a0d1 4500 0018 1d0d a5e5 9000 003e 160d  ..E..........>..
+000008b0: c6d0 1300 0041 7a0e 04b6 fa00 0004 770e  .....Az.......w.
+000008c0: 04b6 fa00 0029 450e 04b6 fa00 0051 1e0e  .....)E......Q..
+000008d0: 04b6 fa00 0057 9d0e 04b6 fa00 0059 770e  .....W.......Yw.
+000008e0: 448f 1800 000f e50e 4949 5200 0004 ac0e  D.......IIR.....
+000008f0: 6fb1 b300 000b d10e 7c48 7a00 0034 6b0e  o.......|Hz..4k.
+00000900: a06b b400 0051 a50e b163 bd00 000e 830f  .k...Q...c......
+00000910: 0784 0400 0021 f20f 3d90 4500 0001 ef0f  .....!..=.E.....
+00000920: 3d90 4500 0014 710f 3d90 4500 0042 bc0f  =.E...q.=.E..B..
+00000930: 4fc6 8900 004a f10f 920c d900 0044 8e0f  O....J.......D..
+00000940: 950c d900 0043 200f 95e3 5200 0049 8c0f  .....C ...R..I..
+00000950: a659 f900 003d 560f ca7e 9900 0039 e30f  .Y...=V..~...9..
+00000960: df6d 7f00 0023 9e0f df6e 4300 0021 470f  .m...#...nC..!G.
+00000970: df6e 4300 0027 b60f e230 9300 000a ef0f  .nC..'...0......
+00000980: fdb3 0d00 001a 9269 0000 5ad2 0300 0000  .......i..Z.....
+00000990: 2800 4400 6900 6600 6600 6500 7200 6500  (.D.i.f.f.e.r.e.
+000009a0: 6e00 7a00 6100 2000 6400 6900 6300 6f00  n.z.a. .d.i.c.o.
+000009b0: 7400 6900 6300 6100 3a08 0000 0000 0600  t.i.c.a.:.......
+000009c0: 0000 1444 6963 686f 7469 6320 4469 6666  ...Dichotic Diff
+000009d0: 6572 656e 6365 3a07 0000 0000 0103 0000  erence:.........
+000009e0: 0012 0041 0072 006d 006f 006e 0069 0063  ...A.r.m.o.n.i.c
+000009f0: 006f 003a 0800 0000 0006 0000 0008 4861  .o.:..........Ha
+00000a00: 726d 6f6e 6963 0700 0000 0001 0300 0000  rmonic..........
+00000a10: 2400 4100 7200 6d00 6f00 6e00 6900 6300  $.A.r.m.o.n.i.c.
+00000a20: 6f00 2000 6100 6c00 6c00 7500 6e00 6700  o. .a.l.l.u.n.g.
+00000a30: 6100 7400 6f08 0000 0000 0600 0000 1248  a.t.o..........H
+00000a40: 6172 6d6f 6e69 6320 5374 7265 7463 6865  armonic Stretche
+00000a50: 6407 0000 0000 0103 0000 0016 0041 0072  d............A.r
+00000a60: 006d 006f 006e 0069 0063 0069 0074 00e0  .m.o.n.i.c.i.t..
+00000a70: 003a 0800 0000 0006 0000 000c 4861 726d  .:..........Harm
+00000a80: 6f6e 6963 6974 793a 0700 0000 0001 0300  onicity:........
+00000a90: 0000 2000 5000 6900 7400 6300 6800 2000  .. .P.i.t.c.h. .
+00000aa0: 6400 6900 2000 4800 7500 6700 6700 6900  d.i. .H.u.g.g.i.
+00000ab0: 6e00 7308 0000 0000 0600 0000 0d48 7567  n.s..........Hug
+00000ac0: 6769 6e73 2050 6974 6368 0700 0000 0001  gins Pitch......
+00000ad0: 0300 0000 1600 4900 5000 4400 2000 4c00  ......I.P.D. .L.
+00000ae0: 6900 6e00 6500 6100 7200 6508 0000 0000  i.n.e.a.r.e.....
+00000af0: 0600 0000 0a49 5044 204c 696e 6561 7207  .....IPD Linear.
+00000b00: 0000 0000 0103 0000 001a 0049 0050 0044  ...........I.P.D
+00000b10: 0020 0061 0020 0073 0063 0061 006c 0069  . .a. .s.c.a.l.i
+00000b20: 006e 006f 0800 0000 0006 0000 000b 4950  .n.o..........IP
+00000b30: 4420 5374 6570 7065 6407 0000 0000 0103  D Stepped.......
+00000b40: 0000 0006 0049 0052 004e 0800 0000 0006  .....I.R.N......
+00000b50: 0000 0003 4952 4e07 0000 0000 0103 0000  ....IRN.........
+00000b60: 0006 0049 0054 0044 0800 0000 0006 0000  ...I.T.D........
+00000b70: 0003 4954 4407 0000 0000 0103 0000 002c  ..ITD..........,
+00000b80: 0052 0075 006d 006f 0072 0065 0020 0061  .R.u.m.o.r.e. .a
+00000b90: 0020 0062 0061 006e 0064 0061 0020 0073  . .b.a.n.d.a. .s
+00000ba0: 0074 0072 0065 0074 0074 0061 0800 0000  .t.r.e.t.t.a....
+00000bb0: 0006 0000 0010 4e61 7272 6f77 6261 6e64  ......Narrowband
+00000bc0: 204e 6f69 7365 0700 0000 0001 0300 0000   Noise..........
+00000bd0: 1800 5400 6900 7000 6f00 2000 7200 7500  ..T.i.p.o. .r.u.
+00000be0: 6d00 6f00 7200 6500 3a08 0000 0000 0600  m.o.r.e.:.......
+00000bf0: 0000 0b4e 6f69 7365 2054 7970 653a 0700  ...Noise Type:..
+00000c00: 0000 0001 0300 0000 0e00 4e00 6500 7300  ..........N.e.s.
+00000c10: 7300 7500 6e00 6f08 0000 0000 0600 0000  s.u.n.o.........
+00000c20: 044e 6f6e 6507 0000 0000 0103 0000 0012  .None...........
+00000c30: 0053 0069 006e 0075 0073 006f 0069 0064  .S.i.n.u.s.o.i.d
+00000c40: 0065 0800 0000 0006 0000 0008 5369 6e75  .e..........Sinu
+00000c50: 736f 6964 0700 0000 0001 0300 0000 0a00  soid............
+00000c60: 5400 6900 7000 6f00 3a08 0000 0000 0600  T.i.p.o.:.......
+00000c70: 0000 0554 7970 653a 0700 0000 0001 0300  ...Type:........
+00000c80: 0000 1800 4300 6f00 7200 7200 6500 6c00  ....C.o.r.r.e.l.
+00000c90: 6100 7a00 6900 6f00 6e00 6508 0000 0000  a.z.i.o.n.e.....
+00000ca0: 0600 0000 0b43 6f72 7265 6c61 7469 6f6e  .....Correlation
+00000cb0: 0700 0000 0761 6366 506c 6f74 0103 0000  .....acfPlot....
+00000cc0: 0020 0044 0069 0061 006c 006f 0067 006f  . .D.i.a.l.o.g.o
+00000cd0: 0020 0064 0069 0020 0069 006e 0070 0075  . .d.i. .i.n.p.u
+00000ce0: 0074 0800 0000 0006 0000 000c 496e 7075  .t..........Inpu
+00000cf0: 7420 4469 616c 6f67 0700 0000 0761 6366  t Dialog.....acf
+00000d00: 506c 6f74 0103 0000 0016 0052 0069 0074  Plot.......R.i.t
+00000d10: 0061 0072 0064 006f 0020 0028 0073 0029  .a.r.d.o. .(.s.)
+00000d20: 0800 0000 0006 0000 0007 4c61 6720 2873  ..........Lag (s
+00000d30: 2907 0000 0007 6163 6650 6c6f 7401 0300  ).....acfPlot...
+00000d40: 0000 1800 4300 6f00 6c00 6f00 7200 6500  ....C.o.l.o.r.e.
+00000d50: 2000 6c00 6900 6e00 6500 6108 0000 0000   .l.i.n.e.a.....
+00000d60: 0600 0000 0a4c 696e 6520 436f 6c6f 7207  .....Line Color.
+00000d70: 0000 0007 6163 6650 6c6f 7401 0300 0000  ....acfPlot.....
+00000d80: 1c00 5300 7000 6500 7300 7300 6f00 7200  ..S.p.e.s.s.o.r.
+00000d90: 6500 2000 4c00 6900 6e00 6500 6108 0000  e. .L.i.n.e.a...
+00000da0: 0000 0600 0000 0a4c 696e 6520 5769 6474  .......Line Widt
+00000db0: 6807 0000 0007 6163 6650 6c6f 7401 0300  h.....acfPlot...
+00000dc0: 0000 1e00 5300 7000 6500 7300 7300 6f00  ....S.p.e.s.s.o.
+00000dd0: 7200 6500 2000 4c00 6900 6e00 6500 6100  r.e. .L.i.n.e.a.
+00000de0: 3a08 0000 0000 0600 0000 0b4c 696e 6520  :..........Line 
+00000df0: 5769 6474 683a 0700 0000 0761 6366 506c  Width:.....acfPl
+00000e00: 6f74 0103 0000 0012 0046 0069 006e 0065  ot.......F.i.n.e
+00000e10: 0073 0074 0072 0061 003a 0800 0000 0006  .s.t.r.a.:......
+00000e20: 0000 0007 5769 6e64 6f77 3a07 0000 0007  ....Window:.....
+00000e30: 6163 6650 6c6f 7401 0300 0000 1e00 2600  acfPlot.......&.
+00000e40: 4100 7000 7000 6c00 6900 6300 6100 2000  A.p.p.l.i.c.a. .
+00000e50: 4600 6900 6c00 7400 7200 6f08 0000 0000  F.i.l.t.r.o.....
+00000e60: 0600 0000 0d26 4170 706c 7920 4669 6c74  .....&Apply Filt
+00000e70: 6572 0700 0000 1161 7070 6c69 6361 7469  er.....applicati
+00000e80: 6f6e 5769 6e64 6f77 0103 0000 0012 0026  onWindow.......&
+00000e90: 004d 006f 0064 0069 0066 0069 0063 0061  .M.o.d.i.f.i.c.a
+00000ea0: 0800 0000 0006 0000 0005 2645 6469 7407  ..........&Edit.
+00000eb0: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
+00000ec0: 696e 646f 7701 0300 0000 0a00 2600 4600  indow.......&.F.
+00000ed0: 6900 6c00 6508 0000 0000 0600 0000 0526  i.l.e..........&
+00000ee0: 4669 6c65 0700 0000 1161 7070 6c69 6361  File.....applica
+00000ef0: 7469 6f6e 5769 6e64 6f77 0103 0000 000e  tionWindow......
+00000f00: 0026 0047 0065 006e 0065 0072 0061 0800  .&.G.e.n.e.r.a..
+00000f10: 0000 0006 0000 0009 2647 656e 6572 6174  ........&Generat
+00000f20: 6507 0000 0011 6170 706c 6963 6174 696f  e.....applicatio
+00000f30: 6e57 696e 646f 7701 0300 0000 1000 2600  nWindow.......&.
+00000f40: 4f00 7400 7400 6900 6500 6e00 6908 0000  O.t.t.i.e.n.i...
+00000f50: 0000 0600 0000 0426 4765 7407 0000 0011  .......&Get.....
+00000f60: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+00000f70: 7701 0300 0000 0c00 2600 4100 6900 7500  w.......&.A.i.u.
+00000f80: 7400 6f08 0000 0000 0600 0000 0526 4865  t.o..........&He
+00000f90: 6c70 0700 0000 1161 7070 6c69 6361 7469  lp.....applicati
+00000fa0: 6f6e 5769 6e64 6f77 0103 ffff ffff 0800  onWindow........
+00000fb0: 0000 0006 0000 0005 2650 6c6f 7407 0000  ........&Plot...
+00000fc0: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
+00000fd0: 646f 7701 0300 0000 1400 2600 5400 7200  dow.......&.T.r.
+00000fe0: 6100 7300 6600 6f00 7200 6d00 6108 0000  a.s.f.o.r.m.a...
+00000ff0: 0000 0600 0000 0826 5072 6f63 6573 7307  .......&Process.
+00001000: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
+00001010: 696e 646f 7701 03ff ffff ff08 0000 0000  indow...........
+00001020: 0600 0000 042e 7b30 7d07 0000 0011 6170  ......{0}.....ap
+00001030: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
+00001040: 0300 0000 1000 5400 6f00 6e00 6f00 2000  ......T.o.n.o. .
+00001050: 4100 4d00 2008 0000 0000 0600 0000 0741  A.M. ..........A
+00001060: 4d20 546f 6e65 0700 0000 1161 7070 6c69  M Tone.....appli
+00001070: 6361 7469 6f6e 5769 6e64 6f77 0103 0000  cationWindow....
+00001080: 0030 0052 0069 0067 0075 0061 0072 0064  .0.R.i.g.u.a.r.d
+00001090: 006f 0020 0070 0079 0073 006f 0075 006e  .o. .p.y.s.o.u.n
+000010a0: 0064 0061 006e 0061 006c 0079 0073 0065  .d.a.n.a.l.y.s.e
+000010b0: 0072 0800 0000 0006 0000 0015 4162 6f75  .r..........Abou
+000010c0: 7420 7079 736f 756e 6461 6e61 6c79 7365  t pysoundanalyse
+000010d0: 7207 0000 0011 6170 706c 6963 6174 696f  r.....applicatio
+000010e0: 6e57 696e 646f 7701 0300 0000 3400 4100  nWindow.....4.A.
+000010f0: 6700 6700 6900 7500 6e00 6700 6900 2000  g.g.i.u.n.g.i. .
+00001100: 6f00 2000 7200 6900 6d00 7500 6f00 7600  o. .r.i.m.u.o.v.
+00001110: 6900 2000 6400 6500 6300 6900 6200 6500  i. .d.e.c.i.b.e.
+00001120: 6c08 0000 0000 0600 0000 1841 6464 206f  l..........Add o
+00001130: 7220 7375 6274 7261 6374 2064 6563 6962  r subtract decib
+00001140: 656c 7307 0000 0011 6170 706c 6963 6174  els.....applicat
+00001150: 696f 6e57 696e 646f 7701 0300 0000 2000  ionWindow..... .
+00001160: 5400 7500 7400 7400 6900 2000 6900 2000  T.u.t.t.i. .i. .
+00001170: 6600 6900 6c00 6500 2000 2800 2a00 2908  f.i.l.e. .(.*.).
+00001180: 0000 0000 0600 0000 0d41 6c6c 2046 696c  .........All Fil
+00001190: 6573 2028 2a29 0700 0000 1161 7070 6c69  es (*).....appli
+000011a0: 6361 7469 6f6e 5769 6e64 6f77 0103 0000  cationWindow....
+000011b0: 0020 0041 0075 0074 006f 0063 006f 0072  . .A.u.t.o.c.o.r
+000011c0: 0072 0065 006c 0061 007a 0069 006f 006e  .r.e.l.a.z.i.o.n
+000011d0: 0065 0800 0000 0006 0000 000f 4175 746f  .e..........Auto
+000011e0: 636f 7272 656c 6174 696f 6e07 0000 0011  correlation.....
+000011f0: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+00001200: 7701 0300 0000 2200 4100 7500 7400 6f00  w.....".A.u.t.o.
+00001210: 6300 6f00 7200 7200 6500 6c00 6f00 6700  c.o.r.r.e.l.o.g.
+00001220: 7200 6100 6d00 6d00 6108 0000 0000 0600  r.a.m.m.a.......
+00001230: 0000 0f41 7574 6f63 6f72 7265 6c6f 6772  ...Autocorrelogr
+00001240: 616d 0700 0000 1161 7070 6c69 6361 7469  am.....applicati
+00001250: 6f6e 5769 6e64 6f77 0103 0000 0006 0042  onWindow.......B
+00001260: 006c 0075 0800 0000 0006 0000 0004 426c  .l.u..........Bl
+00001270: 7565 0700 0000 1161 7070 6c69 6361 7469  ue.....applicati
+00001280: 6f6e 5769 6e64 6f77 0103 0000 0010 0045  onWindow.......E
+00001290: 006e 0074 0072 0061 006d 0062 0065 0800  .n.t.r.a.m.b.e..
+000012a0: 0000 0006 0000 0004 426f 7468 0700 0000  ........Both....
+000012b0: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
+000012c0: 6f77 0103 0000 008e 0049 006d 0070 006f  ow.......I.m.p.o
+000012d0: 0073 0073 0069 0062 0069 006c 0065 0020  .s.s.i.b.i.l.e. 
+000012e0: 0063 006f 006e 0063 0061 0074 0065 006e  .c.o.n.c.a.t.e.n
+000012f0: 0061 0072 0065 0020 0073 0075 006f 006e  .a.r.e. .s.u.o.n
+00001300: 0069 0020 0063 006f 006e 0020 0066 0072  .i. .c.o.n. .f.r
+00001310: 0065 0071 0075 0065 006e 007a 0065 0020  .e.q.u.e.n.z.e. 
+00001320: 0064 0069 0020 0063 0061 006d 0070 0069  .d.i. .c.a.m.p.i
+00001330: 006f 006e 0061 006d 0065 006e 0074 006f  .o.n.a.m.e.n.t.o
+00001340: 0020 0064 0069 0066 0066 0065 0072 0065  . .d.i.f.f.e.r.e
+00001350: 006e 0074 0069 0800 0000 0006 0000 0037  .n.t.i.........7
+00001360: 4361 6e6e 6f74 2063 6f6e 6361 7465 6e61  Cannot concatena
+00001370: 7465 2073 6f75 6e64 7320 7769 7468 2064  te sounds with d
+00001380: 6966 6665 7265 6e74 2073 616d 706c 696e  ifferent samplin
+00001390: 6720 7261 7465 7307 0000 0011 6170 706c  g rates.....appl
+000013a0: 6963 6174 696f 6e57 696e 646f 7701 03ff  icationWindow...
+000013b0: ffff ff08 0000 0000 0600 0000 3143 616e  ............1Can
+000013c0: 6e6f 7420 6375 7420 656e 7469 7265 2073  not cut entire s
+000013d0: 6f75 6e64 2c20 706c 6561 7365 2075 7365  ound, please use
+000013e0: 2072 656d 6f76 6520 6275 7474 6f6e 0700   remove button..
+000013f0: 0000 1161 7070 6c69 6361 7469 6f6e 5769  ...applicationWi
+00001400: 6e64 6f77 0103 0000 003a 0049 006d 0070  ndow.....:.I.m.p
+00001410: 006f 0073 0073 0069 0062 0069 006c 0065  .o.s.s.i.b.i.l.e
+00001420: 0020 0061 0070 0072 0069 0072 0065 0020  . .a.p.r.i.r.e. 
+00001430: 0025 0031 0020 0049 004f 0045 0072 0072  .%.1. .I.O.E.r.r
+00001440: 006f 0072 0800 0000 0006 0000 0016 4361  .o.r..........Ca
+00001450: 6e6e 6f74 206f 7065 6e20 2531 2049 4f45  nnot open %1 IOE
+00001460: 7272 6f72 0700 0000 1161 7070 6c69 6361  rror.....applica
+00001470: 7469 6f6e 5769 6e64 6f77 0103 0000 008e  tionWindow......
+00001480: 004e 006f 006e 0020 00e8 0020 0070 006f  .N.o.n. ... .p.o
+00001490: 0073 0073 0069 0062 0069 006c 0065 0020  .s.s.i.b.i.l.e. 
+000014a0: 0072 0069 0070 0072 006f 0064 0075 0072  .r.i.p.r.o.d.u.r
+000014b0: 0072 0065 0020 0073 0075 006f 006e 0069  .r.e. .s.u.o.n.i
+000014c0: 0020 0063 006f 006e 0020 0066 0072 0065  . .c.o.n. .f.r.e
+000014d0: 0071 0075 0065 006e 007a 0061 0020 0064  .q.u.e.n.z.a. .d
+000014e0: 0069 0020 0063 0061 006d 0070 0069 006f  .i. .c.a.m.p.i.o
+000014f0: 006e 0061 006d 0065 006e 0074 006f 0020  .n.a.m.e.n.t.o. 
+00001500: 0064 0069 0076 0065 0072 0073 0061 0800  .d.i.v.e.r.s.a..
+00001510: 0000 0006 0000 002e 4361 6e6e 6f74 2070  ........Cannot p
+00001520: 6c61 7920 736f 756e 6473 2077 6974 6820  lay sounds with 
+00001530: 6469 6666 6572 656e 7420 7361 6d70 6c65  different sample
+00001540: 2072 6174 6573 0700 0000 1161 7070 6c69   rates.....appli
+00001550: 6361 7469 6f6e 5769 6e64 6f77 0103 0000  cationWindow....
+00001560: 0080 0049 006d 0070 006f 0073 0073 0069  ...I.m.p.o.s.s.i
+00001570: 0062 0069 006c 0065 0020 0073 0061 006c  .b.i.l.e. .s.a.l
+00001580: 0076 0061 0072 0065 0020 0073 0075 006f  .v.a.r.e. .s.u.o
+00001590: 006e 0069 0020 0063 006f 006e 0020 0066  .n.i. .c.o.n. .f
+000015a0: 0072 0065 0071 0075 0065 006e 007a 0065  .r.e.q.u.e.n.z.e
+000015b0: 0020 0064 0069 0020 0063 0061 006d 0070  . .d.i. .c.a.m.p
+000015c0: 0069 006f 006e 0061 006d 0065 006e 0074  .i.o.n.a.m.e.n.t
+000015d0: 006f 0020 0064 0069 0076 0065 0072 0073  .o. .d.i.v.e.r.s
+000015e0: 0065 0800 0000 0006 0000 002f 4361 6e6e  .e........./Cann
+000015f0: 6f74 2077 7269 7465 2073 6f75 6e64 7320  ot write sounds 
+00001600: 7769 7468 2064 6966 6665 7265 6e74 2073  with different s
+00001610: 616d 706c 6520 7261 7465 7307 0000 0011  ample rates.....
+00001620: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+00001630: 7701 0300 0000 0c00 4300 6100 6e00 6100  w.......C.a.n.a.
+00001640: 6c00 6508 0000 0000 0600 0000 0743 6861  l.e..........Cha
+00001650: 6e6e 656c 0700 0000 1161 7070 6c69 6361  nnel.....applica
+00001660: 7469 6f6e 5769 6e64 6f77 0103 0000 0032  tionWindow.....2
+00001670: 0053 0063 0065 0067 006c 0069 0020 0069  .S.c.e.g.l.i. .i
+00001680: 006c 0020 0066 0069 006c 0065 0020 0064  .l. .f.i.l.e. .d
+00001690: 0061 0020 0073 0061 006c 0076 0061 0072  .a. .s.a.l.v.a.r
+000016a0: 0065 0800 0000 0006 0000 0014 4368 6f6f  .e..........Choo
+000016b0: 7365 2066 696c 6520 746f 2077 7269 7465  se file to write
+000016c0: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
+000016d0: 5769 6e64 6f77 0103 0000 0016 0043 006c  Window.......C.l
+000016e0: 006f 006e 0061 0020 0073 0075 006f 006e  .o.n.a. .s.u.o.n
+000016f0: 006f 0800 0000 0006 0000 000b 436c 6f6e  .o..........Clon
+00001700: 6520 536f 756e 6407 0000 0011 6170 706c  e Sound.....appl
+00001710: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
+00001720: 0000 1200 4300 6f00 6e00 6300 6100 7400  ....C.o.n.c.a.t.
+00001730: 6500 6e00 6108 0000 0000 0600 0000 0b43  e.n.a..........C
+00001740: 6f6e 6361 7465 6e61 7465 0700 0000 1161  oncatenate.....a
+00001750: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
+00001760: 0103 0000 001e 0043 006f 006e 0063 0061  .......C.o.n.c.a
+00001770: 0074 0065 006e 0061 0020 0073 0075 006f  .t.e.n.a. .s.u.o
+00001780: 006e 0069 0800 0000 0006 0000 0012 436f  .n.i..........Co
+00001790: 6e63 6174 656e 6174 6520 536f 756e 6473  ncatenate Sounds
+000017a0: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
+000017b0: 5769 6e64 6f77 0103 ffff ffff 0800 0000  Window..........
+000017c0: 0006 0000 0003 4375 7407 0000 0011 6170  ......Cut.....ap
+000017d0: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
+000017e0: 03ff ffff ff08 0000 0000 0600 0000 0943  ...............C
+000017f0: 7574 2053 6f75 6e64 0700 0000 1161 7070  ut Sound.....app
+00001800: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
+00001810: ffff ffff 0800 0000 0006 0000 003f 4475  .............?Du
+00001820: 7261 7469 6f6e 3a20 7b30 7d20 7365 632e  ration: {0} sec.
+00001830: 0a0a 4368 616e 6e65 6c3a 207b 317d 200a  ..Channel: {1} .
+00001840: 0a53 616d 702e 2046 7265 712e 3a20 7b32  .Samp. Freq.: {2
+00001850: 7d20 0a0a 4269 7473 3a20 7b33 7d07 0000  } ..Bits: {3}...
+00001860: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
+00001870: 646f 7701 0300 0000 0800 4500 7300 6300  dow.......E.s.c.
+00001880: 6908 0000 0000 0600 0000 0445 7869 7407  i..........Exit.
+00001890: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
+000018a0: 696e 646f 7701 0300 0000 0800 4500 7300  indow.......E.s.
+000018b0: 6300 6908 0000 0000 0600 0000 1045 7869  c.i..........Exi
+000018c0: 7420 6170 706c 6963 6174 696f 6e07 0000  t application...
+000018d0: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
+000018e0: 646f 7701 0300 0000 2000 4600 4900 5200  dow..... .F.I.R.
+000018f0: 3200 2000 5000 7200 6500 6400 6500 6600  2. .P.r.e.d.e.f.
+00001900: 6900 6e00 6900 7400 6908 0000 0000 0600  i.n.i.t.i.......
+00001910: 0000 0c46 4952 3220 5072 6573 6574 7307  ...FIR2 Presets.
+00001920: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
+00001930: 696e 646f 7701 0300 0000 0e00 5400 6f00  indow.......T.o.
+00001940: 6e00 6f00 2000 4600 4d08 0000 0000 0600  n.o. .F.M.......
+00001950: 0000 0746 4d20 546f 6e65 0700 0000 1161  ...FM Tone.....a
+00001960: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
+00001970: 0103 ffff ffff 0800 0000 0006 0000 0010  ................
+00001980: 4861 726d 6f6e 6963 2043 6f6d 706c 6578  Harmonic Complex
+00001990: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
+000019a0: 5769 6e64 6f77 0103 0000 0020 0050 0069  Window..... .P.i
+000019b0: 0074 0063 0068 0020 0064 0069 0020 0048  .t.c.h. .d.i. .H
+000019c0: 0075 0067 0067 0069 006e 0073 0800 0000  .u.g.g.i.n.s....
+000019d0: 0006 0000 000d 4875 6767 696e 7320 5069  ......Huggins Pi
+000019e0: 7463 6807 0000 0011 6170 706c 6963 6174  tch.....applicat
+000019f0: 696f 6e57 696e 646f 7701 0300 0000 1600  ionWindow.......
+00001a00: 4900 5000 4400 2000 4c00 6900 6e00 6500  I.P.D. .L.i.n.e.
+00001a10: 6100 7200 6508 0000 0000 0600 0000 0a49  a.r.e..........I
+00001a20: 5044 204c 696e 6561 7207 0000 0011 6170  PD Linear.....ap
+00001a30: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
+00001a40: 0300 0000 1a00 4900 5000 4400 2000 6100  ......I.P.D. .a.
+00001a50: 2000 7300 6300 6100 6c00 6900 6e00 6f08   .s.c.a.l.i.n.o.
+00001a60: 0000 0000 0600 0000 0b49 5044 2053 7465  .........IPD Ste
+00001a70: 7070 6564 0700 0000 1161 7070 6c69 6361  pped.....applica
+00001a80: 7469 6f6e 5769 6e64 6f77 0103 0000 0006  tionWindow......
+00001a90: 0049 0052 004e 0800 0000 0006 0000 0003  .I.R.N..........
+00001aa0: 4952 4e07 0000 0011 6170 706c 6963 6174  IRN.....applicat
+00001ab0: 696f 6e57 696e 646f 7701 0300 0000 0600  ionWindow.......
+00001ac0: 4900 5400 4408 0000 0000 0600 0000 0349  I.T.D..........I
+00001ad0: 5444 0700 0000 1161 7070 6c69 6361 7469  TD.....applicati
+00001ae0: 6f6e 5769 6e64 6f77 0103 0000 0020 0044  onWindow..... .D
+00001af0: 0069 0061 006c 006f 0067 006f 0020 0064  .i.a.l.o.g.o. .d
+00001b00: 0069 0020 0069 006e 0070 0075 0074 0800  .i. .i.n.p.u.t..
+00001b10: 0000 0006 0000 000c 496e 7075 7420 4469  ........Input Di
+00001b20: 616c 6f67 0700 0000 1161 7070 6c69 6361  alog.....applica
+00001b30: 7469 6f6e 5769 6e64 6f77 0103 0000 0012  tionWindow......
+00001b40: 0045 0074 0069 0063 0068 0065 0074 0074  .E.t.i.c.h.e.t.t
+00001b50: 0061 0800 0000 0006 0000 0005 4c61 6265  .a..........Labe
+00001b60: 6c07 0000 0011 6170 706c 6963 6174 696f  l.....applicatio
+00001b70: 6e57 696e 646f 7701 0300 0000 1000 5300  nWindow.......S.
+00001b80: 6900 6e00 6900 7300 7400 7200 6f08 0000  i.n.i.s.t.r.o...
+00001b90: 0000 0600 0000 044c 6566 7407 0000 0011  .......Left.....
+00001ba0: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+00001bb0: 7701 0300 0000 2a00 4400 6900 6600 6600  w.....*.D.i.f.f.
+00001bc0: 6500 7200 6500 6e00 7a00 6100 2000 6400  e.r.e.n.z.a. .d.
+00001bd0: 6900 2000 6c00 6900 7600 6500 6c00 6c00  i. .l.i.v.e.l.l.
+00001be0: 6f08 0000 0000 0600 0000 104c 6576 656c  o..........Level
+00001bf0: 2044 6966 6665 7265 6e63 6507 0000 0011   Difference.....
+00001c00: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+00001c10: 7701 0300 0000 1800 4300 6100 7200 6900  w.......C.a.r.i.
+00001c20: 6300 6100 2000 7300 7500 6f00 6e00 6f08  c.a. .s.u.o.n.o.
+00001c30: 0000 0000 0600 0000 0a4c 6f61 6420 536f  .........Load So
+00001c40: 756e 6407 0000 0011 6170 706c 6963 6174  und.....applicat
+00001c50: 696f 6e57 696e 646f 7701 0300 0000 1c00  ionWindow.......
+00001c60: 4d00 6100 6e00 7500 6100 6c00 6500 2000  M.a.n.u.a.l.e. .
+00001c70: 2800 6800 7400 6d00 6c00 2908 0000 0000  (.h.t.m.l.).....
+00001c80: 0600 0000 0d4d 616e 7561 6c20 2868 746d  .....Manual (htm
+00001c90: 6c29 0700 0000 1161 7070 6c69 6361 7469  l).....applicati
+00001ca0: 6f6e 5769 6e64 6f77 0103 0000 001a 004d  onWindow.......M
+00001cb0: 0061 006e 0075 0061 006c 0065 0020 0028  .a.n.u.a.l.e. .(
+00001cc0: 0070 0064 0066 0029 0800 0000 0006 0000  .p.d.f.)........
+00001cd0: 000c 4d61 6e75 616c 2028 7064 6629 0700  ..Manual (pdf)..
+00001ce0: 0000 1161 7070 6c69 6361 7469 6f6e 5769  ...applicationWi
+00001cf0: 6e64 6f77 0103 ffff ffff 0800 0000 0006  ndow............
+00001d00: 0000 0004 4d6f 6e6f 0700 0000 1161 7070  ....Mono.....app
+00001d10: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
+00001d20: 0000 0014 0053 0070 006f 0073 0074 0061  .....S.p.o.s.t.a
+00001d30: 0020 0067 0069 00f9 0800 0000 0006 0000  . .g.i..........
+00001d40: 0009 4d6f 7665 2044 6f77 6e07 0000 0011  ..Move Down.....
+00001d50: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+00001d60: 7701 0300 0000 1200 5300 7000 6f00 7300  w.......S.p.o.s.
+00001d70: 7400 6100 2000 7300 7508 0000 0000 0600  t.a. .s.u.......
+00001d80: 0000 074d 6f76 6520 5570 0700 0000 1161  ...Move Up.....a
+00001d90: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
+00001da0: 0103 0000 0024 0053 0065 006c 0065 007a  .....$.S.e.l.e.z
+00001db0: 0069 006f 006e 0065 0020 006d 0075 006c  .i.o.n.e. .m.u.l
+00001dc0: 0074 0069 0070 006c 0061 0800 0000 0006  .t.i.p.l.a......
+00001dd0: 0000 0012 4d75 6c74 6970 6c65 2053 656c  ....Multiple Sel
+00001de0: 6563 7469 6f6e 0700 0000 1161 7070 6c69  ection.....appli
+00001df0: 6361 7469 6f6e 5769 6e64 6f77 0103 ffff  cationWindow....
+00001e00: ffff 0800 0000 0006 0000 0010 4e61 7272  ............Narr
+00001e10: 6f77 6261 6e64 204e 6f69 7365 0700 0000  owband Noise....
+00001e20: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
+00001e30: 6f77 0103 0000 0016 004e 0075 006f 0076  ow.......N.u.o.v
+00001e40: 006f 0020 006e 006f 006d 0065 003a 0800  .o. .n.o.m.e.:..
+00001e50: 0000 0006 0000 0009 4e65 7720 6e61 6d65  ........New name
+00001e60: 3a07 0000 0011 6170 706c 6963 6174 696f  :.....applicatio
+00001e70: 6e57 696e 646f 7701 0300 0000 2200 4e00  nWindow.....".N.
+00001e80: 6500 7300 7300 7500 6e00 6100 2000 7300  e.s.s.u.n.a. .s.
+00001e90: 6500 6c00 6500 7a00 6900 6f00 6e00 6508  e.l.e.z.i.o.n.e.
+00001ea0: 0000 0000 0600 0000 0c4e 6f20 5365 6c65  .........No Sele
+00001eb0: 6374 696f 6e07 0000 0011 6170 706c 6963  ction.....applic
+00001ec0: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
+00001ed0: 2200 4e00 6500 7300 7300 7500 6e00 6100  ".N.e.s.s.u.n.a.
+00001ee0: 2000 5300 6500 6c00 6500 7a00 6900 6f00   .S.e.l.e.z.i.o.
+00001ef0: 6e00 6508 0000 0000 0600 0000 374e 6f20  n.e.........7No 
+00001f00: 5365 6c65 6374 696f 6e20 2020 2020 2020  Selection       
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f30: 2020 2020 0700 0000 1161 7070 6c69 6361      .....applica
+00001f40: 7469 6f6e 5769 6e64 6f77 0103 0000 000c  tionWindow......
+00001f50: 0052 0075 006d 006f 0072 0065 0800 0000  .R.u.m.o.r.e....
+00001f60: 0006 0000 0005 4e6f 6973 6507 0000 0011  ......Noise.....
+00001f70: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+00001f80: 7701 0300 0000 0e00 4e00 6500 7300 7300  w.......N.e.s.s.
+00001f90: 7500 6e00 6f08 0000 0000 0600 0000 044e  u.n.o..........N
+00001fa0: 6f6e 6507 0000 0011 6170 706c 6963 6174  one.....applicat
+00001fb0: 696f 6e57 696e 646f 7701 0300 0000 2400  ionWindow.....$.
+00001fc0: 4400 6900 7300 7000 6100 7200 6900 2000  D.i.s.p.a.r.i. .
+00001fd0: 6100 2000 7300 6900 6e00 6900 7300 7400  a. .s.i.n.i.s.t.
+00001fe0: 7200 6108 0000 0000 0600 0000 084f 6464  r.a..........Odd
+00001ff0: 204c 6566 7407 0000 0011 6170 706c 6963   Left.....applic
+00002000: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
+00002010: 2000 4400 6900 7300 7000 6100 7200 6900   .D.i.s.p.a.r.i.
+00002020: 2000 6100 2000 6400 6500 7300 7400 7200   .a. .d.e.s.t.r.
+00002030: 6108 0000 0000 0600 0000 094f 6464 2052  a..........Odd R
+00002040: 6967 6874 0700 0000 1161 7070 6c69 6361  ight.....applica
+00002050: 7469 6f6e 5769 6e64 6f77 0103 0000 0050  tionWindow.....P
+00002060: 0053 0069 0020 0070 0075 00f2 0020 0073  .S.i. .p.u... .s
+00002070: 0070 006f 0073 0074 0061 0072 0065 0020  .p.o.s.t.a.r.e. 
+00002080: 0073 006f 006c 006f 0020 0075 006e 0020  .s.o.l.o. .u.n. 
+00002090: 0073 0075 006f 006e 006f 0020 0061 006c  .s.u.o.n.o. .a.l
+000020a0: 006c 0061 0020 0076 006f 006c 0074 0061  .l.a. .v.o.l.t.a
+000020b0: 0800 0000 0006 0000 0025 4f6e 6c79 206f  .........%Only o
+000020c0: 6e65 2073 6f75 6e64 2063 616e 2062 6520  ne sound can be 
+000020d0: 6d6f 7665 6420 6174 2061 2074 696d 6507  moved at a time.
+000020e0: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
+000020f0: 696e 646f 7701 0300 0000 6600 5300 6900  indow.....f.S.i.
+00002100: 2000 7000 7500 f200 2000 6300 6100 6d00   .p.u... .c.a.m.
+00002110: 6200 6900 6100 7200 6500 2000 7300 6f00  b.i.a.r.e. .s.o.
+00002120: 6c00 6f00 2000 6900 6c00 2000 6e00 6f00  l.o. .i.l. .n.o.
+00002130: 6d00 6500 2000 6400 6900 2000 7500 6e00  m.e. .d.i. .u.n.
+00002140: 2000 7300 7500 6f00 6e00 6f00 2000 6100   .s.u.o.n.o. .a.
+00002150: 6c00 6c00 6100 2000 7600 6f00 6c00 7400  l.l.a. .v.o.l.t.
+00002160: 6108 0000 0000 0600 0000 274f 6e6c 7920  a.........'Only 
+00002170: 6f6e 6520 736f 756e 6420 6361 6e20 6265  one sound can be
+00002180: 2072 656e 616d 6564 2061 7420 6120 7469   renamed at a ti
+00002190: 6d65 0700 0000 1161 7070 6c69 6361 7469  me.....applicati
+000021a0: 6f6e 5769 6e64 6f77 0103 0000 0050 0053  onWindow.....P.S
+000021b0: 0069 0020 0070 0075 00f2 0020 0063 0061  .i. .p.u... .c.a
+000021c0: 006d 0062 0069 0061 0072 0065 0020 0073  .m.b.i.a.r.e. .s
+000021d0: 006f 006c 006f 0020 0075 006e 0020 0073  .o.l.o. .u.n. .s
+000021e0: 0075 006f 006e 006f 0020 0061 006c 006c  .u.o.n.o. .a.l.l
+000021f0: 0061 0020 0076 006f 006c 0074 0061 0800  .a. .v.o.l.t.a..
+00002200: 0000 0006 0000 0023 4f6e 6c79 2073 6f75  .......#Only sou
+00002210: 6e64 2063 616e 2062 6520 6368 616e 6765  nd can be change
+00002220: 6420 6174 2061 2074 696d 6507 0000 0011  d at a time.....
+00002230: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+00002240: 7701 0300 0000 6400 5300 6f00 6c00 6f00  w.....d.S.o.l.o.
+00002250: 2000 6400 7500 6500 2000 7300 7500 6f00   .d.u.e. .s.u.o.
+00002260: 6e00 6900 2000 6100 6c00 6c00 6100 2000  n.i. .a.l.l.a. .
+00002270: 7600 6f00 6c00 7400 6100 2000 7000 6f00  v.o.l.t.a. .p.o.
+00002280: 7300 7300 6f00 6e00 6f00 2000 6500 7300  s.s.o.n.o. .e.s.
+00002290: 7300 6500 7200 6500 2000 6300 6f00 6d00  s.e.r.e. .c.o.m.
+000022a0: 7000 6100 7200 6100 7400 6908 0000 0000  p.a.r.a.t.i.....
+000022b0: 0600 0000 294f 6e6c 7920 7477 6f20 736f  ....)Only two so
+000022c0: 756e 6473 2063 616e 2062 6520 636f 6d70  unds can be comp
+000022d0: 6172 6564 2061 7420 6120 7469 6d65 0700  ared at a time..
+000022e0: 0000 1161 7070 6c69 6361 7469 6f6e 5769  ...applicationWi
+000022f0: 6e64 6f77 0103 0000 0068 0053 006f 006c  ndow.....h.S.o.l
+00002300: 006f 0020 0064 0075 0065 0020 0073 0075  .o. .d.u.e. .s.u
+00002310: 006f 006e 0069 0020 0061 006c 006c 0061  .o.n.i. .a.l.l.a
+00002320: 0020 0076 006f 006c 0074 0061 0020 0070  . .v.o.l.t.a. .p
+00002330: 006f 0073 0073 006f 006e 006f 0020 0065  .o.s.s.o.n.o. .e
+00002340: 0073 0073 0065 0072 0065 0020 0063 006f  .s.s.e.r.e. .c.o
+00002350: 006e 0063 0061 0074 0065 006e 0061 0074  .n.c.a.t.e.n.a.t
+00002360: 0069 0800 0000 0006 0000 002d 4f6e 6c79  .i.........-Only
+00002370: 2074 776f 2073 6f75 6e64 7320 6361 6e20   two sounds can 
+00002380: 6265 2063 6f6e 6361 7465 6e61 7465 6420  be concatenated 
+00002390: 6174 2061 2074 696d 6507 0000 0011 6170  at a time.....ap
+000023a0: 706c 6963 6174 696f 6e57 696e 646f 7701  plicationWindow.
+000023b0: 0300 0000 0800 5200 6f00 7300 6108 0000  ......R.o.s.a...
+000023c0: 0000 0600 0000 0450 696e 6b07 0000 0011  .......Pink.....
+000023d0: 6170 706c 6963 6174 696f 6e57 696e 646f  applicationWindo
+000023e0: 7701 0300 0000 1200 5200 6900 7000 7200  w.......R.i.p.r.
+000023f0: 6f00 6400 7500 6300 6908 0000 0000 0600  o.d.u.c.i.......
+00002400: 0000 0450 6c61 7907 0000 0011 6170 706c  ...Play.....appl
+00002410: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
+00002420: 0000 2600 4700 7200 6100 6600 6900 6300  ..&.G.r.a.f.i.c.
+00002430: 6f00 2000 6f00 6e00 6400 6100 2000 7300  o. .o.n.d.a. .s.
+00002440: 6f00 6e00 6f00 7200 6108 0000 0000 0600  o.n.o.r.a.......
+00002450: 0000 0d50 6c6f 7420 5761 7665 666f 726d  ...Plot Waveform
+00002460: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
+00002470: 5769 6e64 6f77 0103 0000 0014 0050 0072  Window.......P.r
+00002480: 0065 0066 0065 0072 0065 006e 007a 0065  .e.f.e.r.e.n.z.e
+00002490: 0800 0000 0006 0000 000b 5072 6566 6572  ..........Prefer
+000024a0: 656e 6365 7307 0000 0011 6170 706c 6963  ences.....applic
+000024b0: 6174 696f 6e57 696e 646f 7701 03ff ffff  ationWindow.....
+000024c0: ff08 0000 0000 0600 0000 1550 7974 686f  ...........Pytho
+000024d0: 6e20 536f 756e 6420 416e 616c 7973 6572  n Sound Analyser
+000024e0: 0700 0000 1161 7070 6c69 6361 7469 6f6e  .....application
+000024f0: 5769 6e64 6f77 0103 0000 000a 0052 006f  Window.......R.o
+00002500: 0073 0073 006f 0800 0000 0006 0000 0003  .s.s.o..........
+00002510: 5265 6407 0000 0011 6170 706c 6963 6174  Red.....applicat
+00002520: 696f 6e57 696e 646f 7701 0300 0000 0e00  ionWindow.......
+00002530: 5200 6900 6d00 7500 6f00 7600 6908 0000  R.i.m.u.o.v.i...
+00002540: 0000 0600 0000 0652 656d 6f76 6507 0000  .......Remove...
+00002550: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
+00002560: 646f 7701 0300 0000 1a00 5200 6900 6d00  dow.......R.i.m.
+00002570: 7500 6f00 7600 6900 2000 7400 7500 7400  u.o.v.i. .t.u.t.
+00002580: 7400 6908 0000 0000 0600 0000 0a52 656d  t.i..........Rem
+00002590: 6f76 6520 416c 6c07 0000 0011 6170 706c  ove All.....appl
+000025a0: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
+000025b0: 0000 1000 5200 6900 6e00 6f00 6d00 6900  ....R.i.n.o.m.i.
+000025c0: 6e00 6108 0000 0000 0600 0000 0652 656e  n.a..........Ren
+000025d0: 616d 6507 0000 0011 6170 706c 6963 6174  ame.....applicat
+000025e0: 696f 6e57 696e 646f 7701 0300 0000 3400  ionWindow.....4.
+000025f0: 4300 6100 6d00 6200 6900 6100 2000 4600  C.a.m.b.i.a. .F.
+00002600: 7200 6500 7100 2e00 2000 4300 6100 6d00  r.e.q... .C.a.m.
+00002610: 7000 6900 6f00 6e00 6100 6d00 6500 6e00  p.i.o.n.a.m.e.n.
+00002620: 7400 6f08 0000 0000 0600 0000 0852 6573  t.o..........Res
+00002630: 616d 706c 6507 0000 0011 6170 706c 6963  ample.....applic
+00002640: 6174 696f 6e57 696e 646f 7701 0300 0000  ationWindow.....
+00002650: 0c00 4400 6500 7300 7400 7200 6f08 0000  ..D.e.s.t.r.o...
+00002660: 0000 0600 0000 0552 6967 6874 0700 0000  .......Right....
+00002670: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
+00002680: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
+00002690: 0010 526f 6f74 204d 6561 6e20 5371 7561  ..Root Mean Squa
+000026a0: 7265 0700 0000 1161 7070 6c69 6361 7469  re.....applicati
+000026b0: 6f6e 5769 6e64 6f77 0103 0000 0014 0053  onWindow.......S
+000026c0: 0061 006c 0076 0061 0020 0063 006f 006d  .a.l.v.a. .c.o.m
+000026d0: 0065 0800 0000 0006 0000 0007 5361 7665  .e..........Save
+000026e0: 2041 7307 0000 0011 6170 706c 6963 6174   As.....applicat
+000026f0: 696f 6e57 696e 646f 7701 0300 0000 0e00  ionWindow.......
+00002700: 5300 6300 6100 6c00 6100 7200 6508 0000  S.c.a.l.a.r.e...
+00002710: 0000 0600 0000 0553 6361 6c65 0700 0000  .......Scale....
+00002720: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
+00002730: 6f77 0103 0000 0024 0053 0063 0061 006c  ow.....$.S.c.a.l
+00002740: 0061 0072 0065 0020 0069 006c 0020 006c  .a.r.e. .i.l. .l
+00002750: 0069 0076 0065 006c 006c 006f 0800 0000  .i.v.e.l.l.o....
+00002760: 0006 0000 000b 5363 616c 6520 4c65 7665  ......Scale Leve
+00002770: 6c07 0000 0011 6170 706c 6963 6174 696f  l.....applicatio
+00002780: 6e57 696e 646f 7701 0300 0000 1e00 5300  nWindow.......S.
+00002790: 6500 6c00 6500 7a00 6900 6f00 6e00 6100  e.l.e.z.i.o.n.a.
+000027a0: 2000 7400 7500 7400 7400 6908 0000 0000   .t.u.t.t.i.....
+000027b0: 0600 0000 0a53 656c 6563 7420 416c 6c07  .....Select All.
+000027c0: 0000 0011 6170 706c 6963 6174 696f 6e57  ....applicationW
+000027d0: 696e 646f 7701 0300 0000 1000 5300 6900  indow.......S.i.
+000027e0: 6c00 6500 6e00 7a00 6900 6f08 0000 0000  l.e.n.z.i.o.....
+000027f0: 0600 0000 0753 696c 656e 6365 0700 0000  .....Silence....
+00002800: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
+00002810: 6f77 0103 0000 0012 0053 0069 006e 0075  ow.......S.i.n.u
+00002820: 0073 006f 0069 0064 0065 0800 0000 0006  .s.o.i.d.e......
+00002830: 0000 0008 5369 6e75 736f 6964 0700 0000  ....Sinusoid....
+00002840: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
+00002850: 6f77 0103 0000 001a 0053 0070 0065 0074  ow.......S.p.e.t
+00002860: 0074 0072 006f 0067 0072 0061 006d 006d  .t.r.o.g.r.a.m.m
+00002870: 0061 0800 0000 0006 0000 000b 5370 6563  .a..........Spec
+00002880: 7472 6f67 7261 6d07 0000 0011 6170 706c  trogram.....appl
+00002890: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
+000028a0: 0000 0e00 5300 7000 6500 7400 7400 7200  ....S.p.e.t.t.r.
+000028b0: 6f08 0000 0000 0600 0000 0853 7065 6374  o..........Spect
+000028c0: 7275 6d07 0000 0011 6170 706c 6963 6174  rum.....applicat
+000028d0: 696f 6e57 696e 646f 7701 03ff ffff ff08  ionWindow.......
+000028e0: 0000 0000 0600 0000 2c53 7570 706f 7274  ........,Support
+000028f0: 6564 2053 6f75 6e64 2046 696c 6573 2028  ed Sound Files (
+00002900: 2a2e 7761 7629 3b3b 416c 6c20 4669 6c65  *.wav);;All File
+00002910: 7320 282a 2907 0000 0011 6170 706c 6963  s (*).....applic
+00002920: 6174 696f 6e57 696e 646f 7701 03ff ffff  ationWindow.....
+00002930: ff08 0000 0000 0600 0000 1356 616c 7565  ...........Value
+00002940: 7320 6f75 7420 6f66 2072 616e 6765 0700  s out of range..
+00002950: 0000 1161 7070 6c69 6361 7469 6f6e 5769  ...applicationWi
+00002960: 6e64 6f77 0103 0000 000a 0056 0069 006f  ndow.......V.i.o
+00002970: 006c 0061 0800 0000 0006 0000 0006 5669  .l.a..........Vi
+00002980: 6f6c 6574 0700 0000 1161 7070 6c69 6361  olet.....applica
+00002990: 7469 6f6e 5769 6e64 6f77 0103 0000 000c  tionWindow......
+000029a0: 0041 0076 0076 0069 0073 006f 0800 0000  .A.v.v.i.s.o....
+000029b0: 0006 0000 0007 5761 726e 696e 6707 0000  ......Warning...
+000029c0: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
+000029d0: 646f 7701 0300 0000 1600 4f00 6e00 6400  dow.......O.n.d.
+000029e0: 6100 2000 7300 6f00 6e00 6f00 7200 6108  a. .s.o.n.o.r.a.
+000029f0: 0000 0000 0600 0000 0857 6176 6566 6f72  .........Wavefor
+00002a00: 6d07 0000 0011 6170 706c 6963 6174 696f  m.....applicatio
+00002a10: 6e57 696e 646f 7701 0300 0000 0c00 4200  nWindow.......B.
+00002a20: 6900 6100 6e00 6300 6f08 0000 0000 0600  i.a.n.c.o.......
+00002a30: 0000 0557 6869 7465 0700 0000 1161 7070  ...White.....app
+00002a40: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
+00002a50: 0000 0014 0070 0061 0073 0073 0061 0062  .....p.a.s.s.a.b
+00002a60: 0061 006e 0064 0061 0800 0000 0006 0000  .a.n.d.a........
+00002a70: 0008 6261 6e64 7061 7373 0700 0000 1161  ..bandpass.....a
+00002a80: 7070 6c69 6361 7469 6f6e 5769 6e64 6f77  pplicationWindow
+00002a90: 0103 0000 0014 0066 0065 0072 006d 0061  .......f.e.r.m.a
+00002aa0: 0062 0061 006e 0064 0061 0800 0000 0006  .b.a.n.d.a......
+00002ab0: 0000 0008 6261 6e64 7374 6f70 0700 0000  ....bandstop....
+00002ac0: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
+00002ad0: 6f77 0103 0000 0012 0070 0061 0073 0073  ow.......p.a.s.s
+00002ae0: 0061 0061 006c 0074 006f 0800 0000 0006  .a.a.l.t.o......
+00002af0: 0000 0008 6869 6768 7061 7373 0700 0000  ....highpass....
+00002b00: 1161 7070 6c69 6361 7469 6f6e 5769 6e64  .applicationWind
+00002b10: 6f77 0103 0000 0014 0070 0061 0073 0073  ow.......p.a.s.s
+00002b20: 0061 0062 0061 0073 0073 006f 0800 0000  .a.b.a.s.s.o....
+00002b30: 0006 0000 0007 6c6f 7770 6173 7307 0000  ......lowpass...
+00002b40: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
+00002b50: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
+00002b60: 0000 046e 6f6e 6507 0000 0011 6170 706c  ...none.....appl
+00002b70: 6963 6174 696f 6e57 696e 646f 7701 0300  icationWindow...
+00002b80: 0000 5200 7000 7900 7300 6f00 7500 6e00  ..R.p.y.s.o.u.n.
+00002b90: 6400 6100 6e00 6100 6c00 7900 7300 6500  d.a.n.a.l.y.s.e.
+00002ba0: 7200 2000 2d00 2000 5300 6300 6500 6700  r. .-. .S.c.e.g.
+00002bb0: 6c00 6900 2000 6600 6900 6c00 6500 2000  l.i. .f.i.l.e. .
+00002bc0: 6400 6100 2000 6300 6100 7200 6900 6300  d.a. .c.a.r.i.c.
+00002bd0: 6100 7200 6508 0000 0000 0600 0000 2570  a.r.e.........%p
+00002be0: 7973 6f75 6e64 616e 616c 7973 6572 202d  ysoundanalyser -
+00002bf0: 2043 686f 6f73 6520 6669 6c65 2074 6f20   Choose file to 
+00002c00: 6c6f 6164 0700 0000 1161 7070 6c69 6361  load.....applica
+00002c10: 7469 6f6e 5769 6e64 6f77 0103 ffff ffff  tionWindow......
+00002c20: 0800 0000 0006 0000 001e 7b30 7d20 6973  ..........{0} is
+00002c30: 200a 207b 317d 207b 327d 2064 4220 7468   . {1} {2} dB th
+00002c40: 616e 200a 207b 337d 0700 0000 1161 7070  an . {3}.....app
+00002c50: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
+00002c60: ffff ffff 0800 0000 0006 0000 001a 7b30  ..............{0
+00002c70: 7d20 6973 207b 317d 207b 327d 2064 4220  } is {1} {2} dB 
+00002c80: 7468 616e 207b 337d 0700 0000 1161 7070  than {3}.....app
+00002c90: 6c69 6361 7469 6f6e 5769 6e64 6f77 0103  licationWindow..
+00002ca0: ffff ffff 0800 0000 0006 0000 000f 7b30  ..............{0
+00002cb0: 7d20 7b31 7d20 3a20 7b32 7d20 0a07 0000  } {1} : {2} ....
+00002cc0: 0011 6170 706c 6963 6174 696f 6e57 696e  ..applicationWin
+00002cd0: 646f 7701 0300 0000 2800 4100 7000 7000  dow.....(.A.p.p.
+00002ce0: 6c00 6900 6300 6100 2000 6c00 6500 2000  l.i.c.a. .l.e. .
+00002cf0: 6d00 6f00 6400 6900 6600 6900 6300 6800  m.o.d.i.f.i.c.h.
+00002d00: 6508 0000 0000 0600 0000 0d41 7070 6c79  e..........Apply
+00002d10: 2043 6861 6e67 6573 0700 0000 0c61 7070   Changes.....app
+00002d20: 6c79 4368 616e 6765 7301 0300 0000 6c00  lyChanges.....l.
+00002d30: 4300 6900 2000 7300 6f00 6e00 6f00 2000  C.i. .s.o.n.o. .
+00002d40: 6d00 6f00 6400 6900 6600 6900 6300 6800  m.o.d.i.f.i.c.h.
+00002d50: 6500 2000 6e00 6f00 6e00 2000 7300 6100  e. .n.o.n. .s.a.
+00002d60: 6c00 7600 6100 7400 6500 2e00 2000 4100  l.v.a.t.e... .A.
+00002d70: 7000 7000 6c00 6900 6300 6100 7200 6500  p.p.l.i.c.a.r.e.
+00002d80: 2000 6c00 6500 2000 6d00 6f00 6400 6900   .l.e. .m.o.d.i.
+00002d90: 6600 6900 6300 6800 6500 3f08 0000 0000  f.i.c.h.e.?.....
+00002da0: 0600 0000 2954 6865 7265 2061 7265 2075  ....)There are u
+00002db0: 6e73 6176 6564 2063 6861 6e67 6573 2e20  nsaved changes. 
+00002dc0: 4170 706c 7920 4368 616e 6765 733f 0700  Apply Changes?..
+00002dd0: 0000 0c61 7070 6c79 4368 616e 6765 7301  ...applyChanges.
+00002de0: 0300 0000 1c00 4100 7000 7000 6c00 6900  ......A.p.p.l.i.
+00002df0: 6300 6100 2000 4600 6900 6c00 7400 7200  c.a. .F.i.l.t.r.
+00002e00: 6f08 0000 0000 0600 0000 0c41 7070 6c79  o..........Apply
+00002e10: 2046 696c 7465 7207 0000 0016 6170 706c   Filter.....appl
+00002e20: 7946 4952 3250 7265 7365 7473 4469 616c  yFIR2PresetsDial
+00002e30: 6f67 0103 0000 000e 0043 0075 0074 006f  og.......C.u.t.o
+00002e40: 0066 0066 003a 0800 0000 0006 0000 0008  .f.f.:..........
+00002e50: 4375 746f 6666 3a20 0700 0000 1661 7070  Cutoff: .....app
+00002e60: 6c79 4649 5232 5072 6573 6574 7344 6961  lyFIR2PresetsDia
+00002e70: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00002e80: 0000 1e45 6e64 2054 7261 6e73 6974 696f  ...End Transitio
+00002e90: 6e20 4261 6e64 203d 2043 7574 6f66 6620  n Band = Cutoff 
+00002ea0: 2a07 0000 0016 6170 706c 7946 4952 3250  *.....applyFIR2P
+00002eb0: 7265 7365 7473 4469 616c 6f67 0103 0000  resetsDialog....
+00002ec0: 001c 004f 0072 0064 0069 006e 0065 0020  ...O.r.d.i.n.e. 
+00002ed0: 0066 0069 006c 0074 0072 006f 003a 0800  .f.i.l.t.r.o.:..
+00002ee0: 0000 0006 0000 000e 4669 6c74 6572 204f  ........Filter O
+00002ef0: 7264 6572 3a20 0700 0000 1661 7070 6c79  rder: .....apply
+00002f00: 4649 5232 5072 6573 6574 7344 6961 6c6f  FIR2PresetsDialo
+00002f10: 6701 0300 0000 1e00 5400 6900 7000 6f00  g.......T.i.p.o.
+00002f20: 2000 6400 6900 2000 6600 6900 6c00 7400   .d.i. .f.i.l.t.
+00002f30: 7200 6f00 3a08 0000 0000 0600 0000 0d46  r.o.:..........F
+00002f40: 696c 7465 7220 5479 7065 3a20 0700 0000  ilter Type: ....
+00002f50: 1661 7070 6c79 4649 5232 5072 6573 6574  .applyFIR2Preset
+00002f60: 7344 6961 6c6f 6701 0300 0000 2200 4300  sDialog.....".C.
+00002f70: 7500 7400 6f00 6600 6600 2000 7300 7500  u.t.o.f.f. .s.u.
+00002f80: 7000 6500 7200 6900 6f00 7200 6500 3a08  p.e.r.i.o.r.e.:.
+00002f90: 0000 0000 0600 0000 0f48 6967 6865 7220  .........Higher 
+00002fa0: 4375 746f 6666 3a20 0700 0000 1661 7070  Cutoff: .....app
+00002fb0: 6c79 4649 5232 5072 6573 6574 7344 6961  lyFIR2PresetsDia
+00002fc0: 6c6f 6701 0300 0000 2200 4300 7500 7400  log.....".C.u.t.
+00002fd0: 6f00 6600 6600 2000 6900 6e00 6600 6500  o.f.f. .i.n.f.e.
+00002fe0: 7200 6900 6f00 7200 6500 3a08 0000 0000  r.i.o.r.e.:.....
+00002ff0: 0600 0000 0e4c 6f77 6572 2043 7574 6f66  .....Lower Cutof
+00003000: 663a 2007 0000 0016 6170 706c 7946 4952  f: .....applyFIR
+00003010: 3250 7265 7365 7473 4469 616c 6f67 0103  2PresetsDialog..
+00003020: 0000 004a 0049 006e 0069 007a 0069 006f  ...J.I.n.i.z.i.o
+00003030: 0020 0062 0061 006e 0064 0061 0020 0064  . .b.a.n.d.a. .d
+00003040: 0069 0020 0074 0072 0061 006e 0073 0069  .i. .t.r.a.n.s.i
+00003050: 007a 0069 006f 006e 0065 0020 003d 0020  .z.i.o.n.e. .=. 
+00003060: 0043 0075 0074 006f 0066 0066 002a 0800  .C.u.t.o.f.f.*..
+00003070: 0000 0006 0000 0020 5374 6172 7420 5472  ....... Start Tr
+00003080: 616e 7369 7469 6f6e 2042 616e 6420 3d20  ansition Band = 
+00003090: 4375 746f 6666 202a 0700 0000 1661 7070  Cutoff *.....app
+000030a0: 6c79 4649 5232 5072 6573 6574 7344 6961  lyFIR2PresetsDia
+000030b0: 6c6f 6701 0300 0000 1400 7000 6100 7300  log.......p.a.s.
+000030c0: 7300 6100 6200 6100 6e00 6400 6108 0000  s.a.b.a.n.d.a...
+000030d0: 0000 0600 0000 0862 616e 6470 6173 7307  .......bandpass.
+000030e0: 0000 0016 6170 706c 7946 4952 3250 7265  ....applyFIR2Pre
+000030f0: 7365 7473 4469 616c 6f67 0103 0000 0014  setsDialog......
+00003100: 0066 0065 0072 006d 0061 0062 0061 006e  .f.e.r.m.a.b.a.n
+00003110: 0064 0061 0800 0000 0006 0000 0008 6261  .d.a..........ba
+00003120: 6e64 7374 6f70 0700 0000 1661 7070 6c79  ndstop.....apply
+00003130: 4649 5232 5072 6573 6574 7344 6961 6c6f  FIR2PresetsDialo
+00003140: 6701 0300 0000 1200 7000 6100 7300 7300  g.......p.a.s.s.
+00003150: 6100 6100 6c00 7400 6f08 0000 0000 0600  a.a.l.t.o.......
+00003160: 0000 0868 6967 6870 6173 7307 0000 0016  ...highpass.....
+00003170: 6170 706c 7946 4952 3250 7265 7365 7473  applyFIR2Presets
+00003180: 4469 616c 6f67 0103 0000 0014 0070 0061  Dialog.......p.a
+00003190: 0073 0073 0061 0062 0061 0073 0073 006f  .s.s.a.b.a.s.s.o
+000031a0: 0800 0000 0006 0000 0007 6c6f 7770 6173  ..........lowpas
+000031b0: 7307 0000 0016 6170 706c 7946 4952 3250  s.....applyFIR2P
+000031c0: 7265 7365 7473 4469 616c 6f67 0103 0000  resetsDialog....
+000031d0: 001a 004d 0061 0070 0070 0061 0020 0063  ...M.a.p.p.a. .c
+000031e0: 006f 006c 006f 0072 0069 003a 0800 0000  .o.l.o.r.i.:....
+000031f0: 0006 0000 000a 436f 6c6f 7220 4d61 703a  ......Color Map:
+00003200: 0700 0000 1361 7574 6f63 6f72 7265 6c6f  .....autocorrelo
+00003210: 6772 616d 506c 6f74 0103 0000 0026 0053  gramPlot.....&.S
+00003220: 006f 0076 0072 0061 0070 0070 006f 0073  .o.v.r.a.p.p.o.s
+00003230: 0069 007a 0069 006f 006e 0065 0020 0028  .i.z.i.o.n.e. .(
+00003240: 0025 0029 0800 0000 0006 0000 000b 4f76  .%.)..........Ov
+00003250: 6572 6c61 7020 2825 2907 0000 0013 6175  erlap (%).....au
+00003260: 746f 636f 7272 656c 6f67 7261 6d50 6c6f  tocorrelogramPlo
+00003270: 7401 0300 0000 2600 4400 7500 7200 6100  t.....&.D.u.r.a.
+00003280: 7400 6100 2000 4600 6900 6e00 6500 7300  t.a. .F.i.n.e.s.
+00003290: 7400 7200 6100 2000 2800 7300 2908 0000  t.r.a. .(.s.)...
+000032a0: 0000 0600 0000 1157 696e 646f 7720 4c65  .......Window Le
+000032b0: 6e67 7468 2028 7329 0700 0000 1361 7574  ngth (s).....aut
+000032c0: 6f63 6f72 7265 6c6f 6772 616d 506c 6f74  ocorrelogramPlot
+000032d0: 0103 0000 0012 0046 0069 006e 0065 0073  .......F.i.n.e.s
+000032e0: 0074 0072 0061 003a 0800 0000 0006 0000  .t.r.a.:........
+000032f0: 0007 5769 6e64 6f77 3a07 0000 0013 6175  ..Window:.....au
+00003300: 746f 636f 7272 656c 6f67 7261 6d50 6c6f  tocorrelogramPlo
+00003310: 7401 0300 0000 1a00 4300 6100 6d00 6200  t.......C.a.m.b.
+00003320: 6900 6100 2000 6300 6100 6e00 6100 6c00  i.a. .c.a.n.a.l.
+00003330: 6508 0000 0000 0600 0000 0e43 6861 6e67  e..........Chang
+00003340: 6520 4368 616e 6e65 6c07 0000 0013 6368  e Channel.....ch
+00003350: 616e 6765 4368 616e 6e65 6c44 6961 6c6f  angeChannelDialo
+00003360: 6701 0300 0000 0e00 4300 6100 6e00 6100  g.......C.a.n.a.
+00003370: 6c00 6500 3a08 0000 0000 0600 0000 0943  l.e.:..........C
+00003380: 6861 6e6e 656c 3a20 0700 0000 1363 6861  hannel: .....cha
+00003390: 6e67 6543 6861 6e6e 656c 4469 616c 6f67  ngeChannelDialog
+000033a0: 0103 0000 0010 0053 0069 006e 0069 0073  .......S.i.n.i.s
+000033b0: 0074 0072 006f 0800 0000 0006 0000 0004  .t.r.o..........
+000033c0: 4c65 6674 0700 0000 1363 6861 6e67 6543  Left.....changeC
+000033d0: 6861 6e6e 656c 4469 616c 6f67 0103 0000  hannelDialog....
+000033e0: 000c 0044 0065 0073 0074 0072 006f 0800  ...D.e.s.t.r.o..
+000033f0: 0000 0006 0000 0005 5269 6768 7407 0000  ........Right...
+00003400: 0013 6368 616e 6765 4368 616e 6e65 6c44  ..changeChannelD
+00003410: 6961 6c6f 6701 0300 0000 1200 4300 6f00  ialog.......C.o.
+00003420: 6e00 6300 6100 7400 6500 6e00 6108 0000  n.c.a.t.e.n.a...
+00003430: 0000 0600 0000 0b43 6f6e 6361 7465 6e61  .......Concatena
+00003440: 7465 0700 0000 1163 6f6e 6361 7465 6e61  te.....concatena
+00003450: 7465 4469 616c 6f67 0103 0000 0020 0049  teDialog..... .I
+00003460: 006e 0074 0065 0072 0076 0061 006c 006c  .n.t.e.r.v.a.l.l
+00003470: 006f 0020 0028 006d 0073 0029 003a 0800  .o. .(.m.s.).:..
+00003480: 0000 0006 0000 000c 4465 6c61 7920 286d  ........Delay (m
+00003490: 7329 3a20 0700 0000 1163 6f6e 6361 7465  s): .....concate
+000034a0: 6e61 7465 4469 616c 6f67 0103 0000 0026  nateDialog.....&
+000034b0: 0054 0069 0070 006f 0020 0064 0069 0020  .T.i.p.o. .d.i. 
+000034c0: 0069 006e 0074 0065 0072 0076 0061 006c  .i.n.t.e.r.v.a.l
+000034d0: 006c 006f 003a 0800 0000 0006 0000 000c  .l.o.:..........
+000034e0: 4465 6c61 7920 5479 7065 3a20 0700 0000  Delay Type: ....
+000034f0: 1163 6f6e 6361 7465 6e61 7465 4469 616c  .concatenateDial
+00003500: 6f67 0103 0000 0010 0053 0069 006e 0069  og.......S.i.n.i
+00003510: 0073 0074 0072 006f 0800 0000 0006 0000  .s.t.r.o........
+00003520: 0004 4c65 6674 0700 0000 1163 6f6e 6361  ..Left.....conca
+00003530: 7465 6e61 7465 4469 616c 6f67 0103 0000  tenateDialog....
+00003540: 001c 0043 0061 006e 0061 006c 0065 0020  ...C.a.n.a.l.e. 
+00003550: 006f 0075 0074 0070 0075 0074 003a 0800  .o.u.t.p.u.t.:..
+00003560: 0000 0006 0000 0010 4f75 7470 7574 2043  ........Output C
+00003570: 6861 6e6e 656c 3a20 0700 0000 1163 6f6e  hannel: .....con
+00003580: 6361 7465 6e61 7465 4469 616c 6f67 0103  catenateDialog..
+00003590: 0000 000c 0044 0065 0073 0074 0072 006f  .....D.e.s.t.r.o
+000035a0: 0800 0000 0006 0000 0005 5269 6768 7407  ..........Right.
+000035b0: 0000 0011 636f 6e63 6174 656e 6174 6544  ....concatenateD
+000035c0: 6961 6c6f 6701 0300 0000 1000 5300 7500  ialog.......S.u.
+000035d0: 6f00 6e00 6f00 2000 3100 3a08 0000 0000  o.n.o. .1.:.....
+000035e0: 0600 0000 0953 6f75 6e64 2031 3a20 0700  .....Sound 1: ..
+000035f0: 0000 1163 6f6e 6361 7465 6e61 7465 4469  ...concatenateDi
+00003600: 616c 6f67 0103 0000 0010 0053 0075 006f  alog.......S.u.o
+00003610: 006e 006f 0020 0032 003a 0800 0000 0006  .n.o. .2.:......
+00003620: 0000 0009 536f 756e 6420 323a 2007 0000  ....Sound 2: ...
+00003630: 0011 636f 6e63 6174 656e 6174 6544 6961  ..concatenateDia
+00003640: 6c6f 6701 0300 0000 1600 4e00 6f00 6d00  log.......N.o.m.
+00003650: 6500 2000 5300 7500 6f00 6e00 6f00 3a08  e. .S.u.o.n.o.:.
+00003660: 0000 0000 0600 0000 0d53 6f75 6e64 204c  .........Sound L
+00003670: 6162 656c 3a20 0700 0000 1163 6f6e 6361  abel: .....conca
+00003680: 7465 6e61 7465 4469 616c 6f67 0103 0000  tenateDialog....
+00003690: 001e 0053 0063 0061 006d 0062 0069 0061  ...S.c.a.m.b.i.a
+000036a0: 0020 0069 0020 0073 0075 006f 006e 0069  . .i. .s.u.o.n.i
+000036b0: 0800 0000 0006 0000 000b 5377 6170 2053  ..........Swap S
+000036c0: 6f75 6e64 7307 0000 0011 636f 6e63 6174  ounds.....concat
+000036d0: 656e 6174 6544 6961 6c6f 6701 0300 0000  enateDialog.....
+000036e0: 0600 4200 6c00 7508 0000 0000 0600 0000  ..B.l.u.........
+000036f0: 0442 6c75 6507 0000 0013 6765 6e65 7261  .Blue.....genera
+00003700: 7465 4e6f 6973 6544 6961 6c6f 6701 0300  teNoiseDialog...
+00003710: 0000 1000 4500 6e00 7400 7200 6100 6d00  ....E.n.t.r.a.m.
+00003720: 6200 6508 0000 0000 0600 0000 0442 6f74  b.e..........Bot
+00003730: 6807 0000 0013 6765 6e65 7261 7465 4e6f  h.....generateNo
+00003740: 6973 6544 6961 6c6f 6701 0300 0000 1800  iseDialog.......
+00003750: 4400 7500 7200 6100 7400 6100 2000 2800  D.u.r.a.t.a. .(.
+00003760: 6d00 7300 2900 3a08 0000 0000 0600 0000  m.s.).:.........
+00003770: 0e44 7572 6174 696f 6e20 286d 7329 3a07  .Duration (ms):.
+00003780: 0000 0013 6765 6e65 7261 7465 4e6f 6973  ....generateNois
+00003790: 6544 6961 6c6f 6701 0300 0000 1200 4f00  eDialog.......O.
+000037a0: 7200 6500 6300 6300 6800 6900 6f00 3a08  r.e.c.c.h.i.o.:.
+000037b0: 0000 0000 0600 0000 0545 6172 3a20 0700  .........Ear: ..
+000037c0: 0000 1367 656e 6572 6174 654e 6f69 7365  ...generateNoise
+000037d0: 4469 616c 6f67 0103 0000 001a 0047 0065  Dialog.......G.e
+000037e0: 006e 0065 0072 0061 0020 0072 0075 006d  .n.e.r.a. .r.u.m
+000037f0: 006f 0072 0065 0800 0000 0006 0000 000e  .o.r.e..........
+00003800: 4765 6e65 7261 7465 204e 6f69 7365 0700  Generate Noise..
+00003810: 0000 1367 656e 6572 6174 654e 6f69 7365  ...generateNoise
+00003820: 4469 616c 6f67 0103 0000 0010 0053 0069  Dialog.......S.i
+00003830: 006e 0069 0073 0074 0072 006f 0800 0000  .n.i.s.t.r.o....
+00003840: 0006 0000 0004 4c65 6674 0700 0000 1367  ......Left.....g
+00003850: 656e 6572 6174 654e 6f69 7365 4469 616c  enerateNoiseDial
+00003860: 6f67 0103 0000 000c 0052 0075 006d 006f  og.......R.u.m.o
+00003870: 0072 0065 0800 0000 0006 0000 0005 4e6f  .r.e..........No
+00003880: 6973 6507 0000 0013 6765 6e65 7261 7465  ise.....generate
+00003890: 4e6f 6973 6544 6961 6c6f 6701 0300 0000  NoiseDialog.....
+000038a0: 1e00 5400 6900 7000 6f00 2000 6400 6900  ..T.i.p.o. .d.i.
+000038b0: 2000 7200 7500 6d00 6f00 7200 6500 3a08   .r.u.m.o.r.e.:.
+000038c0: 0000 0000 0600 0000 0c4e 6f69 7365 2054  .........Noise T
+000038d0: 7970 653a 2007 0000 0013 6765 6e65 7261  ype: .....genera
+000038e0: 7465 4e6f 6973 6544 6961 6c6f 6701 0300  teNoiseDialog...
+000038f0: 0000 0800 5200 6f00 7300 6108 0000 0000  ....R.o.s.a.....
+00003900: 0600 0000 0450 696e 6b07 0000 0013 6765  .....Pink.....ge
+00003910: 6e65 7261 7465 4e6f 6973 6544 6961 6c6f  nerateNoiseDialo
+00003920: 6701 0300 0000 1600 5200 6100 6d00 7000  g.......R.a.m.p.
+00003930: 6500 2000 2800 6d00 7300 2900 3a08 0000  e. .(.m.s.).:...
+00003940: 0000 0600 0000 0b52 616d 7073 2028 6d73  .......Ramps (ms
+00003950: 293a 0700 0000 1367 656e 6572 6174 654e  ):.....generateN
+00003960: 6f69 7365 4469 616c 6f67 0103 0000 000a  oiseDialog......
+00003970: 0052 006f 0073 0073 006f 0800 0000 0006  .R.o.s.s.o......
+00003980: 0000 0003 5265 6407 0000 0013 6765 6e65  ....Red.....gene
+00003990: 7261 7465 4e6f 6973 6544 6961 6c6f 6701  rateNoiseDialog.
+000039a0: 0300 0000 0c00 4400 6500 7300 7400 7200  ......D.e.s.t.r.
+000039b0: 6f08 0000 0000 0600 0000 0552 6967 6874  o..........Right
+000039c0: 0700 0000 1367 656e 6572 6174 654e 6f69  .....generateNoi
+000039d0: 7365 4469 616c 6f67 0103 0000 0034 0046  seDialog.....4.F
+000039e0: 0072 0065 0071 0075 0065 006e 007a 0061  .r.e.q.u.e.n.z.a
+000039f0: 0020 0064 0069 0020 0063 0061 006d 0070  . .d.i. .c.a.m.p
+00003a00: 0069 006f 006e 0061 006d 0065 006e 0074  .i.o.n.a.m.e.n.t
+00003a10: 006f 0800 0000 0006 0000 000d 5361 6d70  .o..........Samp
+00003a20: 6c69 6e67 2052 6174 6507 0000 0013 6765  ling Rate.....ge
+00003a30: 6e65 7261 7465 4e6f 6973 6544 6961 6c6f  nerateNoiseDialo
+00003a40: 6701 0300 0000 1600 4e00 6f00 6d00 6500  g.......N.o.m.e.
+00003a50: 2000 5300 7500 6f00 6e00 6f00 3a08 0000   .S.u.o.n.o.:...
+00003a60: 0000 0600 0000 0d53 6f75 6e64 204c 6162  .......Sound Lab
+00003a70: 656c 3a20 0700 0000 1367 656e 6572 6174  el: .....generat
+00003a80: 654e 6f69 7365 4469 616c 6f67 0103 0000  eNoiseDialog....
+00003a90: 002e 004c 0069 0076 0065 006c 006c 006f  ...L.i.v.e.l.l.o
+00003aa0: 0020 0073 0070 0065 0074 0074 0072 0061  . .s.p.e.t.t.r.a
+00003ab0: 006c 0065 0020 0028 0064 0042 0029 003a  .l.e. .(.d.B.).:
+00003ac0: 0800 0000 0006 0000 0014 5370 6563 7472  ..........Spectr
+00003ad0: 756d 204c 6576 656c 2028 6442 293a 0700  um Level (dB):..
+00003ae0: 0000 1367 656e 6572 6174 654e 6f69 7365  ...generateNoise
+00003af0: 4469 616c 6f67 0103 0000 000a 0056 0069  Dialog.......V.i
+00003b00: 006f 006c 0061 0800 0000 0006 0000 0006  .o.l.a..........
+00003b10: 5669 6f6c 6574 0700 0000 1367 656e 6572  Violet.....gener
+00003b20: 6174 654e 6f69 7365 4469 616c 6f67 0103  ateNoiseDialog..
+00003b30: 0000 000c 0042 0069 0061 006e 0063 006f  .....B.i.a.n.c.o
+00003b40: 0800 0000 0006 0000 0005 5768 6974 6507  ..........White.
+00003b50: 0000 0013 6765 6e65 7261 7465 4e6f 6973  ....generateNois
+00003b60: 6544 6961 6c6f 6701 0300 0000 1200 7200  eDialog.......r.
+00003b70: 6500 2e00 2000 2800 4800 7a00 2900 3a08  e... .(.H.z.).:.
+00003b80: 0000 0000 0600 0000 0a72 652e 2028 487a  .........re. (Hz
+00003b90: 293a 2007 0000 0013 6765 6e65 7261 7465  ): .....generate
+00003ba0: 4e6f 6973 6544 6961 6c6f 6701 0300 0000  NoiseDialog.....
+00003bb0: 1000 4500 6e00 7400 7200 6100 6d00 6200  ..E.n.t.r.a.m.b.
+00003bc0: 6508 0000 0000 0600 0000 0442 6f74 6807  e..........Both.
+00003bd0: 0000 0016 6765 6e65 7261 7465 5369 6e75  ....generateSinu
+00003be0: 736f 6964 4469 616c 6f67 0103 0000 0018  soidDialog......
+00003bf0: 0044 0075 0072 0061 0074 0061 0020 0028  .D.u.r.a.t.a. .(
+00003c00: 006d 0073 0029 003a 0800 0000 0006 0000  .m.s.).:........
+00003c10: 000e 4475 7261 7469 6f6e 2028 6d73 293a  ..Duration (ms):
+00003c20: 0700 0000 1667 656e 6572 6174 6553 696e  .....generateSin
+00003c30: 7573 6f69 6444 6961 6c6f 6701 0300 0000  usoidDialog.....
+00003c40: 1200 4f00 7200 6500 6300 6300 6800 6900  ..O.r.e.c.c.h.i.
+00003c50: 6f00 3a08 0000 0000 0600 0000 0545 6172  o.:..........Ear
+00003c60: 3a20 0700 0000 1667 656e 6572 6174 6553  : .....generateS
+00003c70: 696e 7573 6f69 6444 6961 6c6f 6701 0300  inusoidDialog...
+00003c80: 0000 1e00 4600 7200 6500 7100 7500 6500  ....F.r.e.q.u.e.
+00003c90: 6e00 7a00 6100 2000 2800 4800 7a00 2900  n.z.a. .(.H.z.).
+00003ca0: 3a08 0000 0000 0600 0000 0f46 7265 7175  :..........Frequ
+00003cb0: 656e 6379 2028 487a 293a 0700 0000 1667  ency (Hz):.....g
+00003cc0: 656e 6572 6174 6553 696e 7573 6f69 6444  enerateSinusoidD
+00003cd0: 6961 6c6f 6701 0300 0000 2000 4700 6500  ialog..... .G.e.
+00003ce0: 6e00 6500 7200 6100 2000 7300 6900 6e00  n.e.r.a. .s.i.n.
+00003cf0: 7500 7300 6f00 6900 6400 6508 0000 0000  u.s.o.i.d.e.....
+00003d00: 0600 0000 1147 656e 6572 6174 6520 5369  .....Generate Si
+00003d10: 6e75 736f 6964 0700 0000 1667 656e 6572  nusoid.....gener
+00003d20: 6174 6553 696e 7573 6f69 6444 6961 6c6f  ateSinusoidDialo
+00003d30: 6701 0300 0000 1000 4900 4c00 4400 2000  g.......I.L.D. .
+00003d40: 2800 6400 4200 2908 0000 0000 0600 0000  (.d.B.).........
+00003d50: 0849 4c44 2028 6442 2907 0000 0016 6765  .ILD (dB).....ge
+00003d60: 6e65 7261 7465 5369 6e75 736f 6964 4469  nerateSinusoidDi
+00003d70: 616c 6f67 0103 0000 0010 0049 0054 0044  alog.......I.T.D
+00003d80: 0020 0028 0075 0073 0029 0800 0000 0006  . .(.u.s.)......
+00003d90: 0000 0008 4954 4420 2875 7329 0700 0000  ....ITD (us)....
+00003da0: 1667 656e 6572 6174 6553 696e 7573 6f69  .generateSinusoi
+00003db0: 6444 6961 6c6f 6701 0300 0000 1000 5300  dDialog.......S.
+00003dc0: 6900 6e00 6900 7300 7400 7200 6f08 0000  i.n.i.s.t.r.o...
+00003dd0: 0000 0600 0000 044c 6566 7407 0000 0016  .......Left.....
+00003de0: 6765 6e65 7261 7465 5369 6e75 736f 6964  generateSinusoid
+00003df0: 4469 616c 6f67 0103 0000 0018 004c 0069  Dialog.......L.i
+00003e00: 0076 0065 006c 006c 006f 0020 0028 0064  .v.e.l.l.o. .(.d
+00003e10: 0042 0029 0800 0000 0006 0000 000b 4c65  .B.)..........Le
+00003e20: 7665 6c20 2864 4229 3a07 0000 0016 6765  vel (dB):.....ge
+00003e30: 6e65 7261 7465 5369 6e75 736f 6964 4469  nerateSinusoidDi
+00003e40: 616c 6f67 0103 0000 0020 0046 0061 0073  alog..... .F.a.s
+00003e50: 0065 0020 0028 0072 0061 0064 0069 0061  .e. .(.r.a.d.i.a
+00003e60: 006e 0074 0069 0029 003a 0800 0000 0006  .n.t.i.).:......
+00003e70: 0000 0010 5068 6173 6520 2872 6164 6961  ....Phase (radia
+00003e80: 6e73 293a 0700 0000 1667 656e 6572 6174  ns):.....generat
+00003e90: 6553 696e 7573 6f69 6444 6961 6c6f 6701  eSinusoidDialog.
+00003ea0: 0300 0000 1600 5200 6100 6d00 7000 6500  ......R.a.m.p.e.
+00003eb0: 2000 2800 6d00 7300 2900 3a08 0000 0000   .(.m.s.).:.....
+00003ec0: 0600 0000 0b52 616d 7073 2028 6d73 293a  .....Ramps (ms):
+00003ed0: 0700 0000 1667 656e 6572 6174 6553 696e  .....generateSin
+00003ee0: 7573 6f69 6444 6961 6c6f 6701 0300 0000  usoidDialog.....
+00003ef0: 1200 5200 6500 6600 6500 7200 6500 6e00  ..R.e.f.e.r.e.n.
+00003f00: 7a00 6108 0000 0000 0600 0000 0952 6566  z.a..........Ref
+00003f10: 6572 656e 6365 0700 0000 1667 656e 6572  erence.....gener
+00003f20: 6174 6553 696e 7573 6f69 6444 6961 6c6f  ateSinusoidDialo
+00003f30: 6701 0300 0000 0c00 4400 6500 7300 7400  g.......D.e.s.t.
+00003f40: 7200 6f08 0000 0000 0600 0000 0552 6967  r.o..........Rig
+00003f50: 6874 0700 0000 1667 656e 6572 6174 6553  ht.....generateS
+00003f60: 696e 7573 6f69 6444 6961 6c6f 6701 0300  inusoidDialog...
+00003f70: 0000 3400 4600 7200 6500 7100 7500 6500  ..4.F.r.e.q.u.e.
+00003f80: 6e00 7a00 6100 2000 6400 6900 2000 6300  n.z.a. .d.i. .c.
+00003f90: 6100 6d00 7000 6900 6f00 6e00 6100 6d00  a.m.p.i.o.n.a.m.
+00003fa0: 6500 6e00 7400 6f08 0000 0000 0600 0000  e.n.t.o.........
+00003fb0: 0d53 616d 706c 696e 6720 5261 7465 0700  .Sampling Rate..
+00003fc0: 0000 1667 656e 6572 6174 6553 696e 7573  ...generateSinus
+00003fd0: 6f69 6444 6961 6c6f 6701 0300 0000 1200  oidDialog.......
+00003fe0: 5300 6900 6e00 7500 7300 6f00 6900 6400  S.i.n.u.s.o.i.d.
+00003ff0: 6508 0000 0000 0600 0000 0853 696e 7573  e..........Sinus
+00004000: 6f69 6407 0000 0016 6765 6e65 7261 7465  oid.....generate
+00004010: 5369 6e75 736f 6964 4469 616c 6f67 0103  SinusoidDialog..
+00004020: 0000 0016 004e 006f 006d 0065 0020 0053  .....N.o.m.e. .S
+00004030: 0075 006f 006e 006f 003a 0800 0000 0006  .u.o.n.o.:......
+00004040: 0000 000d 536f 756e 6420 4c61 6265 6c3a  ....Sound Label:
+00004050: 2007 0000 0016 6765 6e65 7261 7465 5369   .....generateSi
+00004060: 6e75 736f 6964 4469 616c 6f67 0103 0000  nusoidDialog....
+00004070: 001e 0053 006f 006d 006d 0061 0020 006f  ...S.o.m.m.a. .o
+00004080: 0072 0069 0067 0069 006e 0061 006c 0065  .r.i.g.i.n.a.l.e
+00004090: 0800 0000 0006 0000 000c 4164 6420 4f72  ..........Add Or
+000040a0: 6967 696e 616c 0700 0000 1367 656e 6572  iginal.....gener
+000040b0: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+000040c0: 0000 0018 0053 006f 006d 006d 0061 0020  .....S.o.m.m.a. 
+000040d0: 0075 0067 0075 0061 006c 0065 0800 0000  .u.g.u.a.l.e....
+000040e0: 0006 0000 0008 4164 6420 5361 6d65 0700  ......Add Same..
+000040f0: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
+00004100: 4469 616c 6f67 0103 0000 0012 0041 006c  Dialog.......A.l
+00004110: 0074 0065 0072 006e 0061 0074 0061 0800  .t.e.r.n.a.t.a..
+00004120: 0000 0006 0000 000b 416c 7465 726e 6174  ........Alternat
+00004130: 696e 6707 0000 0013 6765 6e65 7261 7465  ing.....generate
+00004140: 536f 756e 6444 6961 6c6f 6701 0300 0000  SoundDialog.....
+00004150: 3c00 4c00 6100 7200 6700 6800 6500 7a00  <.L.a.r.g.h.e.z.
+00004160: 7a00 6100 2000 6400 6900 2000 6200 6100  z.a. .d.i. .b.a.
+00004170: 6e00 6400 6100 2000 2800 6300 6500 6e00  n.d.a. .(.c.e.n.
+00004180: 7400 6500 7300 6900 6d00 6900 2908 0000  t.e.s.i.m.i.)...
+00004190: 0000 0600 0000 1142 616e 6477 6964 7468  .......Bandwidth
+000041a0: 2028 4365 6e74 7329 0700 0000 1367 656e   (Cents).....gen
+000041b0: 6572 6174 6553 6f75 6e64 4469 616c 6f67  erateSoundDialog
+000041c0: 0103 0000 002e 004c 0061 0072 0067 0068  .......L.a.r.g.h
+000041d0: 0065 007a 007a 0061 0020 0064 0069 0020  .e.z.z.a. .d.i. 
+000041e0: 0062 0061 006e 0064 0061 0020 0028 0048  .b.a.n.d.a. .(.H
+000041f0: 007a 0029 0800 0000 0006 0000 000e 4261  .z.)..........Ba
+00004200: 6e64 7769 6474 6820 2848 7a29 0700 0000  ndwidth (Hz)....
+00004210: 1367 656e 6572 6174 6553 6f75 6e64 4469  .generateSoundDi
+00004220: 616c 6f67 0103 0000 0010 0045 006e 0074  alog.......E.n.t
+00004230: 0072 0061 006d 0062 0065 0800 0000 0006  .r.a.m.b.e......
+00004240: 0000 0004 426f 7468 0700 0000 1367 656e  ....Both.....gen
+00004250: 6572 6174 6553 6f75 6e64 4469 616c 6f67  erateSoundDialog
+00004260: 0103 0000 0036 004c 0069 0076 0065 006c  .....6.L.i.v.e.l
+00004270: 006c 006f 0020 0063 006f 006d 0070 006f  .l.o. .c.o.m.p.o
+00004280: 006e 0065 006e 0074 0065 0020 0028 0064  .n.e.n.t.e. .(.d
+00004290: 0042 0020 0053 0050 004c 0029 0800 0000  .B. .S.P.L.)....
+000042a0: 0006 0000 0018 436f 6d70 6f6e 656e 7420  ......Component 
+000042b0: 4c65 7665 6c20 2864 4220 5350 4c29 0700  Level (dB SPL)..
+000042c0: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
+000042d0: 4469 616c 6f67 0103 0000 0006 0043 006f  Dialog.......C.o
+000042e0: 0073 0800 0000 0006 0000 0006 436f 7369  .s..........Cosi
+000042f0: 6e65 0700 0000 1367 656e 6572 6174 6553  ne.....generateS
+00004300: 6f75 6e64 4469 616c 6f67 0103 0000 0028  oundDialog.....(
+00004310: 0044 0069 0066 0066 0065 0072 0065 006e  .D.i.f.f.e.r.e.n
+00004320: 007a 0061 0020 0064 0069 0063 006f 0074  .z.a. .d.i.c.o.t
+00004330: 0069 0063 0061 003a 0800 0000 0006 0000  .i.c.a.:........
+00004340: 0014 4469 6368 6f74 6963 2044 6966 6665  ..Dichotic Diffe
+00004350: 7265 6e63 653a 0700 0000 1367 656e 6572  rence:.....gener
+00004360: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+00004370: 0000 0016 0044 0075 0072 0061 0074 0061  .....D.u.r.a.t.a
+00004380: 0020 0028 006d 0073 0029 0800 0000 0006  . .(.m.s.)......
+00004390: 0000 000d 4475 7261 7469 6f6e 2028 6d73  ....Duration (ms
+000043a0: 2907 0000 0013 6765 6e65 7261 7465 536f  ).....generateSo
+000043b0: 756e 6444 6961 6c6f 6701 0300 0000 1200  undDialog.......
+000043c0: 4f00 7200 6500 6300 6300 6800 6900 6f00  O.r.e.c.c.h.i.o.
+000043d0: 3a08 0000 0000 0600 0000 0445 6172 3a07  :..........Ear:.
+000043e0: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
+000043f0: 6444 6961 6c6f 6701 0300 0000 0e00 4600  dDialog.......F.
+00004400: 3000 2000 2800 4800 7a00 2908 0000 0000  0. .(.H.z.).....
+00004410: 0600 0000 0746 3020 2848 7a29 0700 0000  .....F0 (Hz)....
+00004420: 1367 656e 6572 6174 6553 6f75 6e64 4469  .generateSoundDi
+00004430: 616c 6f67 0103 0000 001c 0046 0072 0065  alog.......F.r.e
+00004440: 0071 0075 0065 006e 007a 0061 0020 0028  .q.u.e.n.z.a. .(
+00004450: 0048 007a 0029 0800 0000 0006 0000 000e  .H.z.)..........
+00004460: 4672 6571 7565 6e63 7920 2848 7a29 0700  Frequency (Hz)..
+00004470: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
+00004480: 4469 616c 6f67 0103 0000 0008 0047 0061  Dialog.......G.a
+00004490: 0069 006e 0800 0000 0006 0000 0004 4761  .i.n..........Ga
+000044a0: 696e 0700 0000 1367 656e 6572 6174 6553  in.....generateS
+000044b0: 6f75 6e64 4469 616c 6f67 0103 0000 0018  oundDialog......
+000044c0: 0047 0065 006e 0065 0072 0061 0020 0073  .G.e.n.e.r.a. .s
+000044d0: 0075 006f 006e 006f 0800 0000 0006 0000  .u.o.n.o........
+000044e0: 000e 4765 6e65 7261 7465 2053 6f75 6e64  ..Generate Sound
+000044f0: 0700 0000 1367 656e 6572 6174 6553 6f75  .....generateSou
+00004500: 6e64 4469 616c 6f67 0103 0000 0012 0041  ndDialog.......A
+00004510: 0072 006d 006f 006e 0069 0063 006f 003a  .r.m.o.n.i.c.o.:
+00004520: 0800 0000 0006 0000 0008 4861 726d 6f6e  ..........Harmon
+00004530: 6963 0700 0000 1367 656e 6572 6174 6553  ic.....generateS
+00004540: 6f75 6e64 4469 616c 6f67 0103 0000 0032  oundDialog.....2
+00004550: 004c 0069 0076 0065 006c 006c 006f 0020  .L.i.v.e.l.l.o. 
+00004560: 0061 0072 006d 006f 006e 0069 0063 006f  .a.r.m.o.n.i.c.o
+00004570: 0020 0028 0064 0042 0020 0053 0050 004c  . .(.d.B. .S.P.L
+00004580: 0029 0800 0000 0006 0000 0017 4861 726d  .)..........Harm
+00004590: 6f6e 6963 204c 6576 656c 2028 6442 2053  onic Level (dB S
+000045a0: 504c 2907 0000 0013 6765 6e65 7261 7465  PL).....generate
+000045b0: 536f 756e 6444 6961 6c6f 6701 0300 0000  SoundDialog.....
+000045c0: 3e00 4900 6e00 7400 6500 7200 7600 6100  >.I.n.t.e.r.v.a.
+000045d0: 6c00 6c00 6f00 2000 6100 7200 6d00 6f00  l.l.o. .a.r.m.o.
+000045e0: 6e00 6900 6300 6f00 2000 2800 6300 6500  n.i.c.o. .(.c.e.
+000045f0: 6e00 7400 6500 7300 6900 6d00 6900 2908  n.t.e.s.i.m.i.).
+00004600: 0000 0000 0600 0000 1848 6172 6d6f 6e69  .........Harmoni
+00004610: 6320 5370 6163 696e 6720 2843 656e 7473  c Spacing (Cents
+00004620: 2907 0000 0013 6765 6e65 7261 7465 536f  ).....generateSo
+00004630: 756e 6444 6961 6c6f 6701 0300 0000 2400  undDialog.....$.
+00004640: 4100 7200 6d00 6f00 6e00 6900 6300 6f00  A.r.m.o.n.i.c.o.
+00004650: 2000 6100 6c00 6c00 7500 6e00 6700 6100   .a.l.l.u.n.g.a.
+00004660: 7400 6f08 0000 0000 0600 0000 1248 6172  t.o..........Har
+00004670: 6d6f 6e69 6320 5374 7265 7463 6865 6407  monic Stretched.
+00004680: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
+00004690: 6444 6961 6c6f 6701 0300 0000 1600 4100  dDialog.......A.
+000046a0: 7200 6d00 6f00 6e00 6900 6300 6900 7400  r.m.o.n.i.c.i.t.
+000046b0: e000 3a08 0000 0000 0600 0000 0c48 6172  ..:..........Har
+000046c0: 6d6f 6e69 6369 7479 3a07 0000 0013 6765  monicity:.....ge
+000046d0: 6e65 7261 7465 536f 756e 6444 6961 6c6f  nerateSoundDialo
+000046e0: 6701 0300 0000 3000 4600 7200 6500 7100  g.....0.F.r.e.q.
+000046f0: 7500 6500 6e00 7a00 6100 2000 7300 7500  u.e.n.z.a. .s.u.
+00004700: 7000 6500 7200 6900 6f00 7200 6500 2000  p.e.r.i.o.r.e. .
+00004710: 2800 4800 7a00 2908 0000 0000 0600 0000  (.H.z.).........
+00004720: 0f48 6967 6820 4672 6571 2e20 2848 7a29  .High Freq. (Hz)
+00004730: 0700 0000 1367 656e 6572 6174 6553 6f75  .....generateSou
+00004740: 6e64 4469 616c 6f67 0103 0000 0024 0041  ndDialog.....$.A
+00004750: 0072 006d 006f 006e 0069 0063 0061 0020  .r.m.o.n.i.c.a. 
+00004760: 0073 0075 0070 0065 0072 0069 006f 0072  .s.u.p.e.r.i.o.r
+00004770: 0065 0800 0000 0006 0000 000d 4869 6768  .e..........High
+00004780: 2048 6172 6d6f 6e69 6307 0000 0013 6765   Harmonic.....ge
+00004790: 6e65 7261 7465 536f 756e 6444 6961 6c6f  nerateSoundDialo
+000047a0: 6701 0300 0000 1c00 5300 7400 6f00 7000  g.......S.t.o.p.
+000047b0: 2000 7300 7500 7000 6500 7200 6900 6f00   .s.u.p.e.r.i.o.
+000047c0: 7200 6508 0000 0000 0600 0000 0948 6967  r.e..........Hig
+000047d0: 6820 5374 6f70 0700 0000 1367 656e 6572  h Stop.....gener
+000047e0: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+000047f0: 0000 0020 0050 0069 0074 0063 0068 0020  ... .P.i.t.c.h. 
+00004800: 0064 0069 0020 0048 0075 0067 0067 0069  .d.i. .H.u.g.g.i
+00004810: 006e 0073 0800 0000 0006 0000 000d 4875  .n.s..........Hu
+00004820: 6767 696e 7320 5069 7463 6807 0000 0013  ggins Pitch.....
+00004830: 6765 6e65 7261 7465 536f 756e 6444 6961  generateSoundDia
+00004840: 6c6f 6701 0300 0000 1c00 4900 5000 4400  log.......I.P.D.
+00004850: 2000 2800 7200 6100 6400 6900 6100 6e00   .(.r.a.d.i.a.n.
+00004860: 7400 6900 2908 0000 0000 0600 0000 0d49  t.i.)..........I
+00004870: 5044 2028 7261 6469 616e 7329 0700 0000  PD (radians)....
+00004880: 1367 656e 6572 6174 6553 6f75 6e64 4469  .generateSoundDi
+00004890: 616c 6f67 0103 0000 0016 0049 0050 0044  alog.......I.P.D
+000048a0: 0020 004c 0069 006e 0065 0061 0072 0065  . .L.i.n.e.a.r.e
+000048b0: 0800 0000 0006 0000 000a 4950 4420 4c69  ..........IPD Li
+000048c0: 6e65 6172 0700 0000 1367 656e 6572 6174  near.....generat
+000048d0: 6553 6f75 6e64 4469 616c 6f67 0103 0000  eSoundDialog....
+000048e0: 001a 0049 0050 0044 0020 0061 0020 0073  ...I.P.D. .a. .s
+000048f0: 0063 0061 006c 0069 006e 006f 0800 0000  .c.a.l.i.n.o....
+00004900: 0006 0000 000b 4950 4420 5374 6570 7065  ......IPD Steppe
+00004910: 6407 0000 0013 6765 6e65 7261 7465 536f  d.....generateSo
+00004920: 756e 6444 6961 6c6f 6701 0300 0000 0600  undDialog.......
+00004930: 4900 5200 4e08 0000 0000 0600 0000 0349  I.R.N..........I
+00004940: 524e 0700 0000 1367 656e 6572 6174 6553  RN.....generateS
+00004950: 6f75 6e64 4469 616c 6f67 0103 0000 0012  oundDialog......
+00004960: 0054 0069 0070 006f 0020 0049 0052 004e  .T.i.p.o. .I.R.N
+00004970: 003a 0800 0000 0006 0000 0009 4952 4e20  .:..........IRN 
+00004980: 5479 7065 3a07 0000 0013 6765 6e65 7261  Type:.....genera
+00004990: 7465 536f 756e 6444 6961 6c6f 6701 0300  teSoundDialog...
+000049a0: 0000 0600 4900 5400 4408 0000 0000 0600  ....I.T.D.......
+000049b0: 0000 0349 5444 0700 0000 1367 656e 6572  ...ITD.....gener
+000049c0: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+000049d0: 0000 001a 0049 0054 0044 0020 0028 006d  .....I.T.D. .(.m
+000049e0: 0069 0063 0072 006f 0020 0073 0029 0800  .i.c.r.o. .s.)..
+000049f0: 0000 0006 0000 000d 4954 4420 286d 6963  ........ITD (mic
+00004a00: 726f 2073 2907 0000 0013 6765 6e65 7261  ro s).....genera
+00004a10: 7465 536f 756e 6444 6961 6c6f 6701 0300  teSoundDialog...
+00004a20: 0000 1400 4900 7400 6500 7200 6100 7a00  ....I.t.e.r.a.z.
+00004a30: 6900 6f00 6e00 6908 0000 0000 0600 0000  i.o.n.i.........
+00004a40: 0a49 7465 7261 7469 6f6e 7307 0000 0013  .Iterations.....
+00004a50: 6765 6e65 7261 7465 536f 756e 6444 6961  generateSoundDia
+00004a60: 6c6f 6701 0300 0000 1000 5300 6900 6e00  log.......S.i.n.
+00004a70: 6900 7300 7400 7200 6f08 0000 0000 0600  i.s.t.r.o.......
+00004a80: 0000 044c 6566 7407 0000 0013 6765 6e65  ...Left.....gene
+00004a90: 7261 7465 536f 756e 6444 6961 6c6f 6701  rateSoundDialog.
+00004aa0: 0300 0000 3000 4600 7200 6500 7100 7500  ....0.F.r.e.q.u.
+00004ab0: 6500 6e00 7a00 6100 2000 6900 6e00 6600  e.n.z.a. .i.n.f.
+00004ac0: 6500 7200 6900 6f00 7200 6500 2000 2800  e.r.i.o.r.e. .(.
+00004ad0: 4800 7a00 2908 0000 0000 0600 0000 0e4c  H.z.)..........L
+00004ae0: 6f77 2046 7265 712e 2028 487a 2907 0000  ow Freq. (Hz)...
+00004af0: 0013 6765 6e65 7261 7465 536f 756e 6444  ..generateSoundD
+00004b00: 6961 6c6f 6701 0300 0000 2400 4100 7200  ialog.....$.A.r.
+00004b10: 6d00 6f00 6e00 6900 6300 6100 2000 6900  m.o.n.i.c.a. .i.
+00004b20: 6e00 6600 6500 7200 6900 6f00 7200 6508  n.f.e.r.i.o.r.e.
+00004b30: 0000 0000 0600 0000 0c4c 6f77 2048 6172  .........Low Har
+00004b40: 6d6f 6e69 6307 0000 0013 6765 6e65 7261  monic.....genera
+00004b50: 7465 536f 756e 6444 6961 6c6f 6701 0300  teSoundDialog...
+00004b60: 0000 1c00 5300 7400 6f00 7000 2000 6900  ....S.t.o.p. .i.
+00004b70: 6e00 6600 6500 7200 6900 6f00 7200 6508  n.f.e.r.i.o.r.e.
+00004b80: 0000 0000 0600 0000 084c 6f77 2053 746f  .........Low Sto
+00004b90: 7007 0000 0013 6765 6e65 7261 7465 536f  p.....generateSo
+00004ba0: 756e 6444 6961 6c6f 6701 0300 0000 5200  undDialog.....R.
+00004bb0: 4c00 6900 7600 6500 6c00 6c00 6f00 2000  L.i.v.e.l.l.o. .
+00004bc0: 6300 6f00 6d00 7000 6f00 6e00 6500 6e00  c.o.m.p.o.n.e.n.
+00004bd0: 7400 6900 2000 6200 6100 6e00 6400 6100  t.i. .b.a.n.d.a.
+00004be0: 2000 7300 7400 7200 6500 7400 7400 6100   .s.t.r.e.t.t.a.
+00004bf0: 2000 2800 6400 4200 2000 5300 5000 4c00   .(.d.B. .S.P.L.
+00004c00: 2908 0000 0000 0600 0000 244e 6172 726f  ).........$Narro
+00004c10: 7720 4261 6e64 2043 6f6d 706f 6e65 6e74  w Band Component
+00004c20: 204c 6576 656c 2028 6442 2053 504c 2907   Level (dB SPL).
+00004c30: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
+00004c40: 6444 6961 6c6f 6701 0300 0000 2c00 5200  dDialog.....,.R.
+00004c50: 7500 6d00 6f00 7200 6500 2000 6100 2000  u.m.o.r.e. .a. .
+00004c60: 6200 6100 6e00 6400 6100 2000 7300 7400  b.a.n.d.a. .s.t.
+00004c70: 7200 6500 7400 7400 6108 0000 0000 0600  r.e.t.t.a.......
+00004c80: 0000 104e 6172 726f 7762 616e 6420 4e6f  ...Narrowband No
+00004c90: 6973 6507 0000 0013 6765 6e65 7261 7465  ise.....generate
+00004ca0: 536f 756e 6444 6961 6c6f 6701 0300 0000  SoundDialog.....
+00004cb0: 4200 5200 7500 6d00 6f00 7200 6500 2000  B.R.u.m.o.r.e. .
+00004cc0: 3100 2000 6600 7200 6500 7100 7500 6500  1. .f.r.e.q.u.e.
+00004cd0: 6e00 7a00 6100 2000 7300 7500 7000 6500  n.z.a. .s.u.p.e.
+00004ce0: 7200 6900 6f00 7200 6500 2000 2800 4800  r.i.o.r.e. .(.H.
+00004cf0: 7a00 2908 0000 0000 0600 0000 154e 6f2e  z.)..........No.
+00004d00: 2031 2048 6967 6820 4672 6571 2e20 2848   1 High Freq. (H
+00004d10: 7a29 0700 0000 1367 656e 6572 6174 6553  z).....generateS
+00004d20: 6f75 6e64 4469 616c 6f67 0103 0000 0042  oundDialog.....B
+00004d30: 0052 0075 006d 006f 0072 0065 0020 0031  .R.u.m.o.r.e. .1
+00004d40: 0020 0066 0072 0065 0071 0075 0065 006e  . .f.r.e.q.u.e.n
+00004d50: 007a 0061 0020 0069 006e 0066 0065 0072  .z.a. .i.n.f.e.r
+00004d60: 0069 006f 0072 0065 0020 0028 0048 007a  .i.o.r.e. .(.H.z
+00004d70: 0029 0800 0000 0006 0000 0014 4e6f 2e20  .)..........No. 
+00004d80: 3120 4c6f 7720 4672 6571 2e20 2848 7a29  1 Low Freq. (Hz)
+00004d90: 0700 0000 1367 656e 6572 6174 6553 6f75  .....generateSou
+00004da0: 6e64 4469 616c 6f67 0103 0000 0032 004c  ndDialog.....2.L
+00004db0: 0069 0076 0065 006c 006c 006f 0020 0072  .i.v.e.l.l.o. .r
+00004dc0: 0075 006d 006f 0072 0065 0020 0031 0020  .u.m.o.r.e. .1. 
+00004dd0: 0028 0064 0042 0020 0053 0050 004c 0029  .(.d.B. .S.P.L.)
+00004de0: 0800 0000 0006 0000 0017 4e6f 2e20 3120  ..........No. 1 
+00004df0: 532e 204c 6576 656c 2028 6442 2053 504c  S. Level (dB SPL
+00004e00: 2907 0000 0013 6765 6e65 7261 7465 536f  ).....generateSo
+00004e10: 756e 6444 6961 6c6f 6701 0300 0000 4200  undDialog.....B.
+00004e20: 5200 7500 6d00 6f00 7200 6500 2000 3100  R.u.m.o.r.e. .1.
+00004e30: 2000 6600 7200 6500 7100 7500 6500 6e00   .f.r.e.q.u.e.n.
+00004e40: 7a00 6100 2000 7300 7500 7000 6500 7200  z.a. .s.u.p.e.r.
+00004e50: 6900 6f00 7200 6500 2000 2800 4800 7a00  i.o.r.e. .(.H.z.
+00004e60: 2908 0000 0000 0600 0000 154e 6f2e 2032  )..........No. 2
+00004e70: 2048 6967 6820 4672 6571 2e20 2848 7a29   High Freq. (Hz)
+00004e80: 0700 0000 1367 656e 6572 6174 6553 6f75  .....generateSou
+00004e90: 6e64 4469 616c 6f67 0103 0000 0042 0052  ndDialog.....B.R
+00004ea0: 0075 006d 006f 0072 0065 0020 0032 0020  .u.m.o.r.e. .2. 
+00004eb0: 0066 0072 0065 0071 0075 0065 006e 007a  .f.r.e.q.u.e.n.z
+00004ec0: 0061 0020 0069 006e 0066 0065 0072 0069  .a. .i.n.f.e.r.i
+00004ed0: 006f 0072 0065 0020 0028 0048 007a 0029  .o.r.e. .(.H.z.)
+00004ee0: 0800 0000 0006 0000 0014 4e6f 2e20 3220  ..........No. 2 
+00004ef0: 4c6f 7720 4672 6571 2e20 2848 7a29 0700  Low Freq. (Hz)..
+00004f00: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
+00004f10: 4469 616c 6f67 0103 0000 0032 004c 0069  Dialog.....2.L.i
+00004f20: 0076 0065 006c 006c 006f 0020 0072 0075  .v.e.l.l.o. .r.u
+00004f30: 006d 006f 0072 0065 0020 0032 0020 0028  .m.o.r.e. .2. .(
+00004f40: 0064 0042 0020 0053 0050 004c 0029 0800  .d.B. .S.P.L.)..
+00004f50: 0000 0006 0000 0017 4e6f 2e20 3220 532e  ........No. 2 S.
+00004f60: 204c 6576 656c 2028 6442 2053 504c 2907   Level (dB SPL).
+00004f70: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
+00004f80: 6444 6961 6c6f 6701 0300 0000 0a00 4e00  dDialog.......N.
+00004f90: 6f00 5300 7000 6908 0000 0000 0600 0000  o.S.p.i.........
+00004fa0: 054e 6f53 7069 0700 0000 1367 656e 6572  .NoSpi.....gener
+00004fb0: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+00004fc0: 0000 0018 0054 0069 0070 006f 0020 0072  .....T.i.p.o. .r
+00004fd0: 0075 006d 006f 0072 0065 003a 0800 0000  .u.m.o.r.e.:....
+00004fe0: 0006 0000 000b 4e6f 6973 6520 5479 7065  ......Noise Type
+00004ff0: 3a07 0000 0013 6765 6e65 7261 7465 536f  :.....generateSo
+00005000: 756e 6444 6961 6c6f 6701 0300 0000 0e00  undDialog.......
+00005010: 4e00 6500 7300 7300 7500 6e00 6f08 0000  N.e.s.s.u.n.o...
+00005020: 0000 0600 0000 044e 6f6e 6507 0000 0013  .......None.....
+00005030: 6765 6e65 7261 7465 536f 756e 6444 6961  generateSoundDia
+00005040: 6c6f 6701 0300 0000 0a00 4e00 7000 6900  log.......N.p.i.
+00005050: 5300 6f08 0000 0000 0600 0000 054e 7069  S.o..........Npi
+00005060: 536f 0700 0000 1367 656e 6572 6174 6553  So.....generateS
+00005070: 6f75 6e64 4469 616c 6f67 0103 0000 0024  oundDialog.....$
+00005080: 0044 0069 0073 0070 0061 0072 0069 0020  .D.i.s.p.a.r.i. 
+00005090: 0061 0020 0073 0069 006e 0069 0073 0074  .a. .s.i.n.i.s.t
+000050a0: 0072 0061 0800 0000 0006 0000 0008 4f64  .r.a..........Od
+000050b0: 6420 4c65 6674 0700 0000 1367 656e 6572  d Left.....gener
+000050c0: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+000050d0: 0000 0020 0044 0069 0073 0070 0061 0072  ... .D.i.s.p.a.r
+000050e0: 0069 0020 0061 0020 0064 0065 0073 0074  .i. .a. .d.e.s.t
+000050f0: 0072 0061 0800 0000 0006 0000 0009 4f64  .r.a..........Od
+00005100: 6420 5269 6768 7407 0000 0013 6765 6e65  d Right.....gene
+00005110: 7261 7465 536f 756e 6444 6961 6c6f 6701  rateSoundDialog.
+00005120: 0300 0000 2400 5200 6500 6c00 6100 7a00  ....$.R.e.l.a.z.
+00005130: 6900 6f00 6e00 6500 2000 6400 6900 2000  i.o.n.e. .d.i. .
+00005140: 6600 6100 7300 6500 3a08 0000 0000 0600  f.a.s.e.:.......
+00005150: 0000 1350 6861 7365 2072 656c 6174 696f  ...Phase relatio
+00005160: 6e73 6869 703a 0700 0000 1367 656e 6572  nship:.....gener
+00005170: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+00005180: 0000 000a 0046 0061 0073 0065 003a 0800  .....F.a.s.e.:..
+00005190: 0000 0006 0000 0006 5068 6173 653a 0700  ........Phase:..
+000051a0: 0000 1367 656e 6572 6174 6553 6f75 6e64  ...generateSound
+000051b0: 4469 616c 6f67 0103 0000 0008 0052 006f  Dialog.......R.o
+000051c0: 0073 0061 0800 0000 0006 0000 0004 5069  .s.a..........Pi
+000051d0: 6e6b 0700 0000 1367 656e 6572 6174 6553  nk.....generateS
+000051e0: 6f75 6e64 4469 616c 6f67 0103 0000 0014  oundDialog......
+000051f0: 0052 0061 006d 0070 0061 0020 0028 0073  .R.a.m.p.a. .(.s
+00005200: 006d 0029 0800 0000 0006 0000 0009 5261  .m.)..........Ra
+00005210: 6d70 2028 6d73 2907 0000 0013 6765 6e65  mp (ms).....gene
+00005220: 7261 7465 536f 756e 6444 6961 6c6f 6701  rateSoundDialog.
+00005230: 0300 0000 1800 5200 6100 6e00 6400 6f00  ......R.a.n.d.o.
+00005240: 6d00 6900 7a00 7a00 6100 7400 6108 0000  m.i.z.z.a.t.a...
+00005250: 0000 0600 0000 0652 616e 646f 6d07 0000  .......Random...
+00005260: 0013 6765 6e65 7261 7465 536f 756e 6444  ..generateSoundD
+00005270: 6961 6c6f 6701 0300 0000 0c00 4400 6500  ialog.......D.e.
+00005280: 7300 7400 7200 6f08 0000 0000 0600 0000  s.t.r.o.........
+00005290: 0552 6967 6874 0700 0000 1367 656e 6572  .Right.....gener
+000052a0: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+000052b0: 0000 0034 0046 0072 0065 0071 0075 0065  ...4.F.r.e.q.u.e
+000052c0: 006e 007a 0061 0020 0064 0069 0020 0063  .n.z.a. .d.i. .c
+000052d0: 0061 006d 0070 0069 006f 006e 0061 006d  .a.m.p.i.o.n.a.m
+000052e0: 0065 006e 0074 006f 0800 0000 0006 0000  .e.n.t.o........
+000052f0: 000d 5361 6d70 6c69 6e67 2052 6174 6507  ..Sampling Rate.
+00005300: 0000 0013 6765 6e65 7261 7465 536f 756e  ....generateSoun
+00005310: 6444 6961 6c6f 6701 0300 0000 1200 5300  dDialog.......S.
+00005320: 6300 6800 7200 6f00 6500 6400 6500 7208  c.h.r.o.e.d.e.r.
+00005330: 0000 0000 0600 0000 0953 6368 726f 6564  .........Schroed
+00005340: 6572 0700 0000 1367 656e 6572 6174 6553  er.....generateS
+00005350: 6f75 6e64 4469 616c 6f67 0103 0000 0006  oundDialog......
+00005360: 0053 0069 006e 0800 0000 0006 0000 0004  .S.i.n..........
+00005370: 5369 6e65 0700 0000 1367 656e 6572 6174  Sine.....generat
+00005380: 6553 6f75 6e64 4469 616c 6f67 0103 0000  eSoundDialog....
+00005390: 0012 0053 0069 006e 0075 0073 006f 0069  ...S.i.n.u.s.o.i
+000053a0: 0064 0065 0800 0000 0006 0000 0008 5369  .d.e..........Si
+000053b0: 6e75 736f 6964 0700 0000 1367 656e 6572  nusoid.....gener
+000053c0: 6174 6553 6f75 6e64 4469 616c 6f67 0103  ateSoundDialog..
+000053d0: 0000 0016 004e 006f 006d 0065 0020 0053  .....N.o.m.e. .S
+000053e0: 0075 006f 006e 006f 003a 0800 0000 0006  .u.o.n.o.:......
+000053f0: 0000 000d 536f 756e 6420 4c61 6265 6c3a  ....Sound Label:
+00005400: 2007 0000 0013 6765 6e65 7261 7465 536f   .....generateSo
+00005410: 756e 6444 6961 6c6f 6701 0300 0000 2c00  undDialog.....,.
+00005420: 4900 6e00 7400 6500 7200 7600 6100 6c00  I.n.t.e.r.v.a.l.
+00005430: 6c00 6f00 2000 2800 6300 6500 6e00 7400  l.o. .(.c.e.n.t.
+00005440: 6500 7300 6900 6d00 6900 2908 0000 0000  e.s.i.m.i.).....
+00005450: 0600 0000 0f53 7061 6369 6e67 2028 4365  .....Spacing (Ce
+00005460: 6e74 7329 0700 0000 1367 656e 6572 6174  nts).....generat
+00005470: 6553 6f75 6e64 4469 616c 6f67 0103 0000  eSoundDialog....
+00005480: 0034 004c 0069 0076 0065 006c 006c 006f  .4.L.i.v.e.l.l.o
+00005490: 0020 0073 0070 0065 0074 0074 0072 0061  . .s.p.e.t.t.r.a
+000054a0: 006c 0065 0020 0028 0064 0042 0020 0053  .l.e. .(.d.B. .S
+000054b0: 0050 004c 0029 0800 0000 0006 0000 0017  .P.L.)..........
+000054c0: 5370 6563 7472 756d 204c 6576 656c 2028  Spectrum Level (
+000054d0: 6442 2053 504c 2907 0000 0013 6765 6e65  dB SPL).....gene
+000054e0: 7261 7465 536f 756e 6444 6961 6c6f 6701  rateSoundDialog.
+000054f0: 0300 0000 2000 4100 6c00 6c00 7500 6e00  .... .A.l.l.u.n.
+00005500: 6700 6100 6d00 6500 6e00 7400 6f00 2000  g.a.m.e.n.t.o. .
+00005510: 2800 2500 2908 0000 0000 0600 0000 0b53  (.%.)..........S
+00005520: 7472 6574 6368 2028 2529 0700 0000 1367  tretch (%).....g
+00005530: 656e 6572 6174 6553 6f75 6e64 4469 616c  enerateSoundDial
+00005540: 6f67 0103 0000 000a 0054 0069 0070 006f  og.......T.i.p.o
+00005550: 003a 0800 0000 0006 0000 0005 5479 7065  .:..........Type
+00005560: 3a07 0000 0013 6765 6e65 7261 7465 536f  :.....generateSo
+00005570: 756e 6444 6961 6c6f 6701 0300 0000 0c00  undDialog.......
+00005580: 4200 6900 6100 6e00 6300 6f08 0000 0000  B.i.a.n.c.o.....
+00005590: 0600 0000 0557 6869 7465 0700 0000 1367  .....White.....g
+000055a0: 656e 6572 6174 6553 6f75 6e64 4469 616c  enerateSoundDial
+000055b0: 6f67 0103 0000 001a 0043 006f 006c 006f  og.......C.o.l.o
+000055c0: 0072 0065 0020 0073 0066 006f 006e 0064  .r.e. .s.f.o.n.d
+000055d0: 006f 0800 0000 0006 0000 0010 4261 636b  .o..........Back
+000055e0: 6772 6f75 6e64 2043 6f6c 6f72 0700 0000  ground Color....
+000055f0: 1170 7265 6665 7265 6e63 6573 4469 616c  .preferencesDial
+00005600: 6f67 0103 0000 0022 0043 006f 006c 006f  og.....".C.o.l.o
+00005610: 0072 0065 0020 0063 0061 006e 006f 0076  .r.e. .c.a.n.o.v
+00005620: 0061 0063 0063 0069 006f 0800 0000 0006  .a.c.c.i.o......
+00005630: 0000 000c 4361 6e76 6173 2043 6f6c 6f72  ....Canvas Color
+00005640: 0700 0000 1170 7265 6665 7265 6e63 6573  .....preferences
+00005650: 4469 616c 6f67 0103 0000 001a 004d 0061  Dialog.......M.a
+00005660: 0070 0070 0061 0020 0063 006f 006c 006f  .p.p.a. .c.o.l.o
+00005670: 0072 0065 003a 0800 0000 0006 0000 000a  .r.e.:..........
+00005680: 436f 6c6f 7220 4d61 703a 0700 0000 1170  Color Map:.....p
+00005690: 7265 6665 7265 6e63 6573 4469 616c 6f67  referencesDialog
+000056a0: 0103 0000 0010 0043 006f 006d 0061 006e  .......C.o.m.a.n
+000056b0: 0064 006f 003a 0800 0000 0006 0000 0008  .d.o.:..........
+000056c0: 436f 6d6d 616e 643a 0700 0000 1170 7265  Command:.....pre
+000056d0: 6665 7265 6e63 6573 4469 616c 6f67 0103  ferencesDialog..
+000056e0: 0000 0038 004e 0061 007a 0069 006f 006e  ...8.N.a.z.i.o.n
+000056f0: 0065 0020 0028 006e 0065 0063 0065 0073  .e. .(.n.e.c.e.s
+00005700: 0073 0069 0074 0061 0020 0072 0069 0061  .s.i.t.a. .r.i.a
+00005710: 0076 0076 0069 006f 0029 003a 0800 0000  .v.v.i.o.).:....
+00005720: 0006 0000 001b 436f 756e 7472 7920 2872  ......Country (r
+00005730: 6571 7569 7265 7320 7265 7374 6172 7429  equires restart)
+00005740: 3a07 0000 0011 7072 6566 6572 656e 6365  :.....preference
+00005750: 7344 6961 6c6f 6701 0300 0000 2400 4400  sDialog.....$.D.
+00005760: 5000 4900 2000 2d00 2000 7200 6900 7300  P.I. .-. .r.i.s.
+00005770: 6f00 6c00 7500 7a00 6900 6f00 6e00 6500  o.l.u.z.i.o.n.e.
+00005780: 3a08 0000 0000 0600 0000 1144 5049 202d  :..........DPI -
+00005790: 2052 6573 6f6c 7574 696f 6e3a 0700 0000   Resolution:....
+000057a0: 1170 7265 6665 7265 6e63 6573 4469 616c  .preferencesDial
+000057b0: 6f67 0103 0000 000e 0047 0072 0069 0067  og.......G.r.i.g
+000057c0: 006c 0069 0061 0800 0000 0006 0000 0004  .l.i.a..........
+000057d0: 4772 6964 0700 0000 1170 7265 6665 7265  Grid.....prefere
+000057e0: 6e63 6573 4469 616c 6f67 0103 0000 0036  ncesDialog.....6
+000057f0: 004c 0069 006e 0067 0075 0061 0020 0028  .L.i.n.g.u.a. .(
+00005800: 006e 0065 0063 0065 0073 0073 0069 0074  .n.e.c.e.s.s.i.t
+00005810: 0061 0020 0072 0069 0061 0076 0076 0069  .a. .r.i.a.v.v.i
+00005820: 006f 0029 003a 0800 0000 0006 0000 001c  .o.).:..........
+00005830: 4c61 6e67 7561 6765 2028 7265 7175 6972  Language (requir
+00005840: 6573 2072 6573 7461 7274 293a 0700 0000  es restart):....
+00005850: 1170 7265 6665 7265 6e63 6573 4469 616c  .preferencesDial
+00005860: 6f67 0103 0000 0018 0043 006f 006c 006f  og.......C.o.l.o
+00005870: 0072 0065 0020 006c 0069 006e 0065 0061  .r.e. .l.i.n.e.a
+00005880: 0800 0000 0006 0000 000a 4c69 6e65 2043  ..........Line C
+00005890: 6f6c 6f72 0700 0000 1170 7265 6665 7265  olor.....prefere
+000058a0: 6e63 6573 4469 616c 6f67 0103 0000 0018  ncesDialog......
+000058b0: 004c 0069 0076 0065 006c 006c 006f 0020  .L.i.v.e.l.l.o. 
+000058c0: 004d 0061 0078 003a 0800 0000 0006 0000  .M.a.x.:........
+000058d0: 000a 4d61 7820 4c65 7665 6c3a 0700 0000  ..Max Level:....
+000058e0: 1170 7265 6665 7265 6e63 6573 4469 616c  .preferencesDial
+000058f0: 6f67 0103 0000 002a 0043 006f 006d 0061  og.....*.C.o.m.a
+00005900: 006e 0064 006f 0020 0072 0069 0070 0072  .n.d.o. .r.i.p.r
+00005910: 006f 0064 0075 007a 0069 006f 006e 0065  .o.d.u.z.i.o.n.e
+00005920: 003a 0800 0000 0006 0000 000d 506c 6179  .:..........Play
+00005930: 2043 6f6d 6d61 6e64 3a07 0000 0011 7072   Command:.....pr
+00005940: 6566 6572 656e 6365 7344 6961 6c6f 6701  eferencesDialog.
+00005950: 0300 0000 1000 4700 7200 6100 6600 6900  ......G.r.a.f.i.
+00005960: 6300 2600 6908 0000 0000 0600 0000 0650  c.&.i..........P
+00005970: 6c6f 7426 7307 0000 0011 7072 6566 6572  lot&s.....prefer
+00005980: 656e 6365 7344 6961 6c6f 6701 0300 0000  encesDialog.....
+00005990: 1000 5300 6500 6700 6e00 6100 6c00 2600  ..S.e.g.n.a.l.&.
+000059a0: 6508 0000 0000 0600 0000 0753 6967 6e61  e..........Signa
+000059b0: 266c 0700 0000 1170 7265 6665 7265 6e63  &l.....preferenc
+000059c0: 6573 4469 616c 6f67 0103 0000 000c 0053  esDialog.......S
+000059d0: 0075 006f 006e 0026 006f 0800 0000 0006  .u.o.n.&.o......
+000059e0: 0000 0006 536f 756e 2664 0700 0000 1170  ....Soun&d.....p
+000059f0: 7265 6665 7265 6e63 6573 4469 616c 6f67  referencesDialog
+00005a00: 0103 0000 000c 0041 0076 0076 0069 0073  .......A.v.v.i.s
+00005a10: 006f 0800 0000 0006 0000 0007 5761 726e  .o..........Warn
+00005a20: 696e 6707 0000 0011 7072 6566 6572 656e  ing.....preferen
+00005a30: 6365 7344 6961 6c6f 6701 0300 0000 3e00  cesDialog.....>.
+00005a40: 5700 6100 7600 2000 4d00 6100 6e00 6100  W.a.v. .M.a.n.a.
+00005a50: 6700 6500 7200 2000 2800 7200 6900 6300  g.e.r. .(.r.i.c.
+00005a60: 6800 6900 6500 6400 6500 2000 7200 6900  h.i.e.d.e. .r.i.
+00005a70: 6100 7600 7600 6900 6f00 2900 3a08 0000  a.v.v.i.o.).:...
+00005a80: 0000 0600 0000 0c57 6176 204d 616e 6167  .......Wav Manag
+00005a90: 6572 3a07 0000 0011 7072 6566 6572 656e  er:.....preferen
+00005aa0: 6365 7344 6961 6c6f 6701 0300 0000 1200  cesDialog.......
+00005ab0: 4600 6900 6e00 6500 7300 7400 7200 6100  F.i.n.e.s.t.r.a.
+00005ac0: 3a08 0000 0000 0600 0000 0757 696e 646f  :..........Windo
+00005ad0: 773a 0700 0000 1170 7265 6665 7265 6e63  w:.....preferenc
+00005ae0: 6573 4469 616c 6f67 0103 0000 001c 0070  esDialog.......p
+00005af0: 0065 0072 0073 006f 006e 0061 006c 0069  .e.r.s.o.n.a.l.i
+00005b00: 007a 007a 0061 0074 006f 0800 0000 0006  .z.z.a.t.o......
+00005b10: 0000 0006 6375 7374 6f6d 0700 0000 1170  ....custom.....p
+00005b20: 7265 6665 7265 6e63 6573 4469 616c 6f67  referencesDialog
+00005b30: 0103 0000 002a 0076 0061 006c 006f 0072  .....*.v.a.l.o.r
+00005b40: 0065 0020 0064 0070 0069 0020 006e 006f  .e. .d.p.i. .n.o
+00005b50: 006e 0020 0076 0061 006c 0069 0064 006f  .n. .v.a.l.i.d.o
+00005b60: 0800 0000 0006 0000 0013 6470 6920 7661  ..........dpi va
+00005b70: 6c75 6520 6e6f 7420 7661 6c69 6407 0000  lue not valid...
+00005b80: 0011 7072 6566 6572 656e 6365 7344 6961  ..preferencesDia
+00005b90: 6c6f 6701 0300 0000 3200 7600 6100 6c00  log.....2.v.a.l.
+00005ba0: 6f00 7200 6500 2000 6400 7000 6900 2000  o.r.e. .d.p.i. .
+00005bb0: 7400 7200 6f00 7000 7000 6f00 2000 7000  t.r.o.p.p.o. .p.
+00005bc0: 6900 6300 6300 6f00 6c00 6f08 0000 0000  i.c.c.o.l.o.....
+00005bd0: 0600 0000 1364 7069 2076 616c 7565 2074  .....dpi value t
+00005be0: 6f6f 2073 6d61 6c6c 0700 0000 1170 7265  oo small.....pre
+00005bf0: 6665 7265 6e63 6573 4469 616c 6f67 0103  ferencesDialog..
+00005c00: 0000 003c 004e 0075 006f 0076 0061 0020  ...<.N.u.o.v.a. 
+00005c10: 0066 0072 0065 0071 0075 0065 006e 007a  .f.r.e.q.u.e.n.z
+00005c20: 0061 0020 0063 0061 006d 0070 0069 006f  .a. .c.a.m.p.i.o
+00005c30: 006e 0061 006d 0065 006e 0074 006f 003a  .n.a.m.e.n.t.o.:
+00005c40: 0800 0000 0006 0000 0013 4e65 7720 5361  ..........New Sa
+00005c50: 6d70 6c69 6e67 2052 6174 653a 2007 0000  mpling Rate: ...
+00005c60: 000e 7265 7361 6d70 6c65 4469 616c 6f67  ..resampleDialog
+00005c70: 0103 0000 0050 0046 0072 0065 0071 0075  .....P.F.r.e.q.u
+00005c80: 0065 006e 007a 0061 0020 0064 0069 0020  .e.n.z.a. .d.i. 
+00005c90: 0063 0061 006d 0070 0069 006f 006e 0061  .c.a.m.p.i.o.n.a
+00005ca0: 006d 0065 006e 0074 006f 0020 0063 006f  .m.e.n.t.o. .c.o
+00005cb0: 0072 0072 0065 006e 0074 0065 003a 0020  .r.r.e.n.t.e.:. 
+00005cc0: 0025 004c 0031 0800 0000 0006 0000 001b  .%.L.1..........
+00005cd0: 4e65 7720 7361 6d70 6c69 6e67 2072 6174  New sampling rat
+00005ce0: 6520 746f 6f20 736d 616c 6c07 0000 000e  e too small.....
+00005cf0: 7265 7361 6d70 6c65 4469 616c 6f67 0103  resampleDialog..
+00005d00: 0000 0014 0052 0069 0063 0061 006d 0070  .....R.i.c.a.m.p
+00005d10: 0069 006f 006e 0061 0800 0000 0006 0000  .i.o.n.a........
+00005d20: 0008 5265 7361 6d70 6c65 0700 0000 0e72  ..Resample.....r
+00005d30: 6573 616d 706c 6544 6961 6c6f 6701 0300  esampleDialog...
+00005d40: 0000 3a00 4100 6c00 6700 6f00 7200 6900  ..:.A.l.g.o.r.i.
+00005d50: 7400 6d00 6f00 2000 6400 6900 2000 7200  t.m.o. .d.i. .r.
+00005d60: 6900 6300 6100 6d00 7000 6900 6f00 6e00  i.c.a.m.p.i.o.n.
+00005d70: 6100 6d00 6500 6e00 7400 6f00 3a08 0000  a.m.e.n.t.o.:...
+00005d80: 0000 0600 0000 1652 6573 616d 706c 696e  .......Resamplin
+00005d90: 6720 416c 676f 7269 7468 6d3a 2007 0000  g Algorithm: ...
+00005da0: 000e 7265 7361 6d70 6c65 4469 616c 6f67  ..resampleDialog
+00005db0: 0103 0000 000c 0041 0076 0076 0069 0073  .......A.v.v.i.s
+00005dc0: 006f 0800 0000 0006 0000 0007 5761 726e  .o..........Warn
+00005dd0: 696e 6707 0000 000e 7265 7361 6d70 6c65  ing.....resample
+00005de0: 4469 616c 6f67 0103 0000 0024 0054 0069  Dialog.....$.T.i
+00005df0: 0070 006f 0020 0064 0069 0020 0066 0069  .p.o. .d.i. .f.i
+00005e00: 006e 0073 0065 0073 0074 0072 0061 003a  .n.s.e.s.t.r.a.:
+00005e10: 0800 0000 0006 0000 000d 5769 6e64 6f77  ..........Window
+00005e20: 2054 7970 653a 2007 0000 000e 7265 7361   Type: .....resa
+00005e30: 6d70 6c65 4469 616c 6f67 0103 ffff ffff  mpleDialog......
+00005e40: 0800 0000 0006 0000 0006 4269 7473 3a20  ..........Bits: 
+00005e50: 0700 0000 0f73 6176 6553 6f75 6e64 4469  .....saveSoundDi
+00005e60: 616c 6f67 0103 0000 000e 0043 0061 006e  alog.......C.a.n
+00005e70: 0061 006c 0065 003a 0800 0000 0006 0000  .a.l.e.:........
+00005e80: 0009 4368 616e 6e65 6c3a 2007 0000 000f  ..Channel: .....
+00005e90: 7361 7665 536f 756e 6444 6961 6c6f 6701  saveSoundDialog.
+00005ea0: 0300 0000 1a00 4600 6f00 7200 6d00 6100  ......F.o.r.m.a.
+00005eb0: 7400 6f00 2000 6600 6900 6c00 6500 3a08  t.o. .f.i.l.e.:.
+00005ec0: 0000 0000 0600 0000 0d46 696c 6520 466f  .........File Fo
+00005ed0: 726d 6174 3a20 0700 0000 0f73 6176 6553  rmat: .....saveS
+00005ee0: 6f75 6e64 4469 616c 6f67 0103 ffff ffff  oundDialog......
+00005ef0: 0800 0000 0006 0000 0004 4d6f 6e6f 0700  ..........Mono..
+00005f00: 0000 0f73 6176 6553 6f75 6e64 4469 616c  ...saveSoundDial
+00005f10: 6f67 0103 0000 003a 004f 0070 007a 0069  og.....:.O.p.z.i
+00005f20: 006f 006e 0069 0020 0073 0061 006c 0076  .o.n.i. .s.a.l.v
+00005f30: 0061 0074 0061 0067 0067 0069 006f 0020  .a.t.a.g.g.i.o. 
+00005f40: 0064 0065 006c 0020 0073 0075 006f 006e  .d.e.l. .s.u.o.n
+00005f50: 006f 0800 0000 0006 0000 0012 5361 7665  .o..........Save
+00005f60: 2053 6f75 6e64 204f 7074 696f 6e73 0700   Sound Options..
+00005f70: 0000 0f73 6176 6553 6f75 6e64 4469 616c  ...saveSoundDial
+00005f80: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00005f90: 0006 5374 6572 656f 0700 0000 0f73 6176  ..Stereo.....sav
+00005fa0: 6553 6f75 6e64 4469 616c 6f67 0103 0000  eSoundDialog....
+00005fb0: 001a 004d 0061 0070 0070 0061 0020 0063  ...M.a.p.p.a. .c
+00005fc0: 006f 006c 006f 0072 0069 003a 0800 0000  .o.l.o.r.i.:....
+00005fd0: 0006 0000 000a 436f 6c6f 7220 4d61 703a  ......Color Map:
+00005fe0: 0700 0000 0f73 7065 6374 726f 6772 616d  .....spectrogram
+00005ff0: 506c 6f74 0103 0000 0012 0054 0065 006d  Plot.......T.e.m
+00006000: 0070 006f 0020 0028 0073 0029 0800 0000  .p.o. .(.s.)....
+00006010: 0006 0000 0008 4c6f 6720 6178 6973 0700  ......Log axis..
+00006020: 0000 0f73 7065 6374 726f 6772 616d 506c  ...spectrogramPl
+00006030: 6f74 0103 0000 0026 0053 006f 0076 0072  ot.....&.S.o.v.r
+00006040: 0061 0070 0070 006f 0073 0069 007a 0069  .a.p.p.o.s.i.z.i
+00006050: 006f 006e 0065 0020 0028 0025 0029 0800  .o.n.e. .(.%.)..
+00006060: 0000 0006 0000 000b 4f76 6572 6c61 7020  ........Overlap 
+00006070: 2825 2907 0000 000f 7370 6563 7472 6f67  (%).....spectrog
+00006080: 7261 6d50 6c6f 7401 0300 0000 1800 5000  ramPlot.......P.
+00006090: 6f00 7400 6500 6e00 7a00 6100 2000 6400  o.t.e.n.z.a. .d.
+000060a0: 6900 2000 3208 0000 0000 0600 0000 0a50  i. .2..........P
+000060b0: 6f77 6572 206f 6620 3207 0000 000f 7370  ower of 2.....sp
+000060c0: 6563 7472 6f67 7261 6d50 6c6f 7401 0300  ectrogramPlot...
+000060d0: 0000 2600 4400 7500 7200 6100 7400 6100  ..&.D.u.r.a.t.a.
+000060e0: 2000 4600 6900 6e00 6500 7300 7400 7200   .F.i.n.e.s.t.r.
+000060f0: 6100 2000 2800 7300 2908 0000 0000 0600  a. .(.s.).......
+00006100: 0000 1157 696e 646f 7720 4c65 6e67 7468  ...Window Length
+00006110: 2028 7329 0700 0000 0f73 7065 6374 726f   (s).....spectro
+00006120: 6772 616d 506c 6f74 0103 0000 0012 0046  gramPlot.......F
+00006130: 0069 006e 0065 0073 0074 0072 0061 003a  .i.n.e.s.t.r.a.:
+00006140: 0800 0000 0006 0000 0007 5769 6e64 6f77  ..........Window
+00006150: 3a07 0000 000f 7370 6563 7472 6f67 7261  :.....spectrogra
+00006160: 6d50 6c6f 7401 0300 0000 2000 4400 6900  mPlot..... .D.i.
+00006170: 6100 6c00 6f00 6700 6f00 2000 6400 6900  a.l.o.g.o. .d.i.
+00006180: 2000 6900 6e00 7000 7500 7408 0000 0000   .i.n.p.u.t.....
+00006190: 0600 0000 0c49 6e70 7574 2044 6961 6c6f  .....Input Dialo
+000061a0: 6707 0000 000c 7370 6563 7472 756d 506c  g.....spectrumPl
+000061b0: 6f74 0103 0000 0018 0043 006f 006c 006f  ot.......C.o.l.o
+000061c0: 0072 0065 0020 006c 0069 006e 0065 0061  .r.e. .l.i.n.e.a
+000061d0: 0800 0000 0006 0000 000a 4c69 6e65 2043  ..........Line C
+000061e0: 6f6c 6f72 0700 0000 0c73 7065 6374 7275  olor.....spectru
+000061f0: 6d50 6c6f 7401 0300 0000 1c00 5300 7000  mPlot.......S.p.
+00006200: 6500 7300 7300 6f00 7200 6500 2000 4c00  e.s.s.o.r.e. .L.
+00006210: 6900 6e00 6500 6108 0000 0000 0600 0000  i.n.e.a.........
+00006220: 0a4c 696e 6520 5769 6474 6807 0000 000c  .Line Width.....
+00006230: 7370 6563 7472 756d 506c 6f74 0103 0000  spectrumPlot....
+00006240: 001e 0053 0070 0065 0073 0073 006f 0072  ...S.p.e.s.s.o.r
+00006250: 0065 0020 004c 0069 006e 0065 0061 003a  .e. .L.i.n.e.a.:
+00006260: 0800 0000 0006 0000 000b 4c69 6e65 2057  ..........Line W
+00006270: 6964 7468 3a07 0000 000c 7370 6563 7472  idth:.....spectr
+00006280: 756d 506c 6f74 0103 0000 0010 004c 006f  umPlot.......L.o
+00006290: 0067 0020 0061 0073 0073 0065 0800 0000  .g. .a.s.s.e....
+000062a0: 0006 0000 0008 4c6f 6720 6178 6973 0700  ......Log axis..
+000062b0: 0000 0c73 7065 6374 7275 6d50 6c6f 7401  ...spectrumPlot.
+000062c0: 0300 0000 1800 5000 6f00 7400 6500 6e00  ......P.o.t.e.n.
+000062d0: 7a00 6100 2000 6400 6900 2000 3208 0000  z.a. .d.i. .2...
+000062e0: 0000 0600 0000 0a50 6f77 6572 206f 6620  .......Power of 
+000062f0: 3207 0000 000c 7370 6563 7472 756d 506c  2.....spectrumPl
+00006300: 6f74 0103 0000 0012 0046 0069 006e 0065  ot.......F.i.n.e
+00006310: 0073 0074 0072 0061 003a 0800 0000 0006  .s.t.r.a.:......
+00006320: 0000 0007 5769 6e64 6f77 3a07 0000 000c  ....Window:.....
+00006330: 7370 6563 7472 756d 506c 6f74 0103 0000  spectrumPlot....
+00006340: 0020 0044 0069 0061 006c 006f 0067 006f  . .D.i.a.l.o.g.o
+00006350: 0020 0064 0069 0020 0069 006e 0070 0075  . .d.i. .i.n.p.u
+00006360: 0074 0800 0000 0006 0000 000c 496e 7075  .t..........Inpu
+00006370: 7420 4469 616c 6f67 0700 0000 0c77 6176  t Dialog.....wav
+00006380: 6566 6f72 6d50 6c6f 7401 0300 0000 1800  eformPlot.......
+00006390: 4300 6f00 6c00 6f00 7200 6500 2000 6c00  C.o.l.o.r.e. .l.
+000063a0: 6900 6e00 6500 6108 0000 0000 0600 0000  i.n.e.a.........
+000063b0: 0a4c 696e 6520 436f 6c6f 7207 0000 000c  .Line Color.....
+000063c0: 7761 7665 666f 726d 506c 6f74 0103 0000  waveformPlot....
+000063d0: 001c 0053 0070 0065 0073 0073 006f 0072  ...S.p.e.s.s.o.r
+000063e0: 0065 0020 004c 0069 006e 0065 0061 0800  .e. .L.i.n.e.a..
+000063f0: 0000 0006 0000 000a 4c69 6e65 2057 6964  ........Line Wid
+00006400: 7468 0700 0000 0c77 6176 6566 6f72 6d50  th.....waveformP
+00006410: 6c6f 7401 0300 0000 1e00 5300 7000 6500  lot.......S.p.e.
+00006420: 7300 7300 6f00 7200 6500 2000 4c00 6900  s.s.o.r.e. .L.i.
+00006430: 6e00 6500 6100 3a08 0000 0000 0600 0000  n.e.a.:.........
+00006440: 0b4c 696e 6520 5769 6474 683a 0700 0000  .Line Width:....
+00006450: 0c77 6176 6566 6f72 6d50 6c6f 7401 8800  .waveformPlot...
+00006460: 0000 0201 01                             .....
```

### Comparing `pysoundanalyser-0.3.4/translations/pysoundanalyser_it_IT.qm` & `pysoundanalyser-0.3.7/translations/pysoundanalyser_it_IT.qm`

 * *Files identical despite different names*

