# Comparing `tmp/rdeditor-0.1.3.9.tar.gz` & `tmp/rdeditor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdeditor-0.1.3.9.tar", last modified: Thu Apr 25 08:03:59 2024, max compression
+gzip compressed data, was "rdeditor-0.2.0.tar", last modified: Thu May  2 12:56:19 2024, max compression
```

## Comparing `rdeditor-0.1.3.9.tar` & `rdeditor-0.2.0.tar`

### file list

```diff
@@ -1,146 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.347580 rdeditor-0.1.3.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.351580 rdeditor-0.1.3.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/.github/workflows/actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/DEVELOPER.md
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.351580 rdeditor-0.1.3.9/Screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)    52961 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/Screenshots/Main_window.png
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/Screenshots/Side_bar.png
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/Screenshots/Top_Menu.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.351580 rdeditor-0.1.3.9/rdeditor/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/Mendelev_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.347580 rdeditor-0.1.3.9/rdeditor/icon_themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.355580 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.363580 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_E_Z.png
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_E_Z.svg
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_R_S.png
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/about.png
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/appicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/calc.png
--rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/exit.png
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/grid.png
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Broom.png
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Bulleted List.png
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Cancel.png
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Carbon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Cursor.png
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Decrease Font.png
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Delete.png
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Double.png
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Edit.png
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Exit.png
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Hydrogen.png
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Increase Font.png
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Info.png
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Left.png
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Line.png
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Minus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Molecule.png
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Open.png
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Oxygen.png
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Physics.png
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Pinch.png
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Redo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Replace Atom.png
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Reset.png
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Right.png
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Save as.png
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Save.png
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Scatter Plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Shutdown.png
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Single.png
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Trash.png
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Triple.png
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Undo.png
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-copy-96.png
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-paste-100.png
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/molblock.png
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/next.png
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/open.png
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/prev.png
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/ptable.png
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/ptable.svg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/index.theme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.363580 rdeditor-0.1.3.9/rdeditor/icon_themes/light/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_E_Z.png
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_E_Z.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16252 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_R_S.png
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/about.png
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon copy.png
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon.svg.png
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/calc.png
--rw-r--r--   0 runner    (1001) docker     (127)    20176 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/exit.png
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/grid.png
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Broom.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Bulleted List.png
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Cancel.png
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Carbon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Cursor.png
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Decrease Font.png
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Delete.png
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Double.png
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Edit.png
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Exit.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Hydrogen.png
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Increase Font.png
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Info.png
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Left.png
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Line.png
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Minus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Molecule.png
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Open.png
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Oxygen.png
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Physics.png
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Pinch.png
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Redo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Replace Atom.png
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Reset.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Right.png
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Save as.png
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Save.png
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Scatter Plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Shutdown.png
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Single.png
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Trash.png
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Triple.png
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Undo.png
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-copy-96.png
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-paste-100.png
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/molblock.png
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/next.png
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/open.png
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/prev.png
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/ptable.png
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/ptable.svg
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/index.theme
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/molEditWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/molViewWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/ptable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/ptable_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    28148 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/rdEditor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/rdeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.385522 rdeditor-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.361523 rdeditor-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.365522 rdeditor-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-02 12:56:12.000000 rdeditor-0.2.0/.github/workflows/actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 12:56:12.000000 rdeditor-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-02 12:56:12.000000 rdeditor-0.2.0/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-02 12:56:12.000000 rdeditor-0.2.0/DEVELOPER.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-02 12:56:12.000000 rdeditor-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 12:56:12.000000 rdeditor-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-02 12:56:19.385522 rdeditor-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-02 12:56:12.000000 rdeditor-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.365522 rdeditor-0.2.0/Screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)    52961 2024-05-02 12:56:12.000000 rdeditor-0.2.0/Screenshots/Main_window.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-02 12:56:12.000000 rdeditor-0.2.0/Screenshots/Side_bar.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-02 12:56:12.000000 rdeditor-0.2.0/Screenshots/Top_Menu.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.365522 rdeditor-0.2.0/rdeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/Mendelev_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 12:56:19.000000 rdeditor-0.2.0/rdeditor/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.361523 rdeditor-0.2.0/rdeditor/icon_themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.369522 rdeditor-0.2.0/rdeditor/icon_themes/dark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.377523 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/Change_E_Z.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/Change_E_Z.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/Change_R_S.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/appicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/benzene.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/calc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/cyclohexane.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/exit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/grid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Broom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Bulleted List.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Cancel.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Carbon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Cursor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Decrease Font.png
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Double.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Exit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Hydrogen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Increase Font.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Info.png
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Line.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Molecule.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Oxygen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Physics.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Pinch.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Redo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Replace Atom.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Reset.png
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Save as.png
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Save.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Scatter Plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Shutdown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Single.png
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Trash.png
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Triple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Undo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-copy-96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-paste-100.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/molblock.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/next.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/prev.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/ptable.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/application/ptable.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/dark/index.theme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.377523 rdeditor-0.2.0/rdeditor/icon_themes/light/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.385522 rdeditor-0.2.0/rdeditor/icon_themes/light/application/
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/Change_E_Z.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/Change_E_Z.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16252 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/Change_R_S.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/appicon copy.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/appicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/appicon.svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/benzene.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/benzene.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/calc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/cyclohexane.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/cyclohexane.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20176 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/exit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/grid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Broom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Bulleted List.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Cancel.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Carbon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Cursor.png
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Decrease Font.png
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Double.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Exit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Hydrogen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Increase Font.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Info.png
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Line.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Molecule.png
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Oxygen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Physics.png
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Pinch.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Redo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Replace Atom.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Reset.png
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Save as.png
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Save.png
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Scatter Plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Shutdown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Single.png
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Trash.png
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Triple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Undo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-copy-96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-paste-100.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/molblock.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/next.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/open.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/prev.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/ptable.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/application/ptable.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/icon_themes/light/index.theme
+-rw-r--r--   0 runner    (1001) docker     (127)    24743 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/molEditWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/molViewWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/ptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/ptable_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29853 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/rdEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-02 12:56:12.000000 rdeditor-0.2.0/rdeditor/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:56:19.385522 rdeditor-0.2.0/rdeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-02 12:56:19.000000 rdeditor-0.2.0/rdeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-02 12:56:19.000000 rdeditor-0.2.0/rdeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:56:19.000000 rdeditor-0.2.0/rdeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 12:56:19.000000 rdeditor-0.2.0/rdeditor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:56:19.000000 rdeditor-0.2.0/rdeditor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 12:56:19.000000 rdeditor-0.2.0/rdeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 12:56:19.000000 rdeditor-0.2.0/rdeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 12:56:12.000000 rdeditor-0.2.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:56:19.385522 rdeditor-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-02 12:56:12.000000 rdeditor-0.2.0/setup.py
```

### Comparing `rdeditor-0.1.3.9/.github/workflows/actions.yml` & `rdeditor-0.2.0/.github/workflows/actions.yml`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/.gitignore` & `rdeditor-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/CITATION.bib` & `rdeditor-0.2.0/CITATION.bib`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/DEVELOPER.md` & `rdeditor-0.2.0/DEVELOPER.md`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/LICENSE` & `rdeditor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/PKG-INFO` & `rdeditor-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdeditor
-Version: 0.1.3.9
+Version: 0.2.0
 Summary: An RDKit based molecule editor using PySide
 Home-page: http://github.com/ebjerrum/rdeditor
 Author: Esben Jannik Bjerrum
 Author-email: esbenjannik@rocketmail.com
 License: LGPL
 Keywords: RDKit molecule editor pyside
 Requires-Python: >=3.8
```

### Comparing `rdeditor-0.1.3.9/README.md` & `rdeditor-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/Screenshots/Main_window.png` & `rdeditor-0.2.0/Screenshots/Main_window.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/Screenshots/Side_bar.png` & `rdeditor-0.2.0/Screenshots/Side_bar.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/Screenshots/Top_Menu.png` & `rdeditor-0.2.0/Screenshots/Top_Menu.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_E_Z.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/Change_E_Z.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_E_Z.svg` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/Change_E_Z.svg`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_R_S.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/Change_R_S.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/about.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/about.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/appicon.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/appicon.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/calc.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/calc.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/exit.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/exit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/grid.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/grid.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Broom.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Broom.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Bulleted List.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Bulleted List.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Cancel.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Cancel.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Carbon.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Carbon.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Cursor.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Cursor.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Decrease Font.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Decrease Font.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Delete.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Delete.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Double.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Double.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Edit.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Edit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Exit.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Exit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Hydrogen.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Hydrogen.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Increase Font.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Increase Font.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Info.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Info.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Left.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Left.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Line.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Line.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Minus.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Minus.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Molecule.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Molecule.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Open.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Open.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Oxygen.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Oxygen.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Physics.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Physics.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Pinch.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Pinch.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Plus.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Plus.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Redo.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Redo.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Replace Atom.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Replace Atom.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Reset.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Reset.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Right.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Right.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Save as.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Save as.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Save.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Save.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Scatter Plot.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Scatter Plot.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Shutdown.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Shutdown.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Single.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Single.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Trash.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Trash.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Triple.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Triple.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Undo.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-Undo.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-copy-96.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-copy-96.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-paste-100.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/icons8-paste-100.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/molblock.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/molblock.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/next.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/next.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/open.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/open.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/plot.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/plot.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/prev.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/prev.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/ptable.png` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/ptable.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/ptable.svg` & `rdeditor-0.2.0/rdeditor/icon_themes/dark/application/ptable.svg`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_E_Z.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/Change_E_Z.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_E_Z.svg` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/Change_E_Z.svg`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_R_S.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/Change_R_S.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/about.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/about.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon copy.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/appicon copy.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/appicon.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon.svg.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/appicon.svg.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/calc.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/calc.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/exit.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/exit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/grid.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/grid.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Broom.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Broom.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Bulleted List.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Bulleted List.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Cancel.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Cancel.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Carbon.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Carbon.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Cursor.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Cursor.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Decrease Font.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Decrease Font.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Delete.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Delete.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Edit.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Edit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Exit.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Exit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Hydrogen.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Hydrogen.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Increase Font.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Increase Font.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Info.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Info.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Left.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Left.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Minus.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Minus.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Molecule.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Molecule.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Open.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Open.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Oxygen.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Oxygen.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Physics.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Physics.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Pinch.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Pinch.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Plus.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Plus.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Redo.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Redo.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Replace Atom.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Replace Atom.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Reset.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Reset.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Right.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Right.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Save as.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Save as.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Save.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Save.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Scatter Plot.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Scatter Plot.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Shutdown.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Shutdown.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Trash.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Trash.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Triple.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Triple.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Undo.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-Undo.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-copy-96.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-copy-96.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-paste-100.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/icons8-paste-100.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/molblock.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/molblock.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/next.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/next.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/open.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/open.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/plot.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/plot.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/prev.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/prev.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/ptable.png` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/ptable.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/ptable.svg` & `rdeditor-0.2.0/rdeditor/icon_themes/light/application/ptable.svg`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/molEditWidget.py` & `rdeditor-0.2.0/rdeditor/molEditWidget.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/python
 # Import required modules
 from __future__ import print_function
 from PySide2 import QtCore, QtGui, QtSvg, QtWidgets
 import sys
 import logging
+from warnings import warn
+
 
 import numpy as np
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from rdkit.Chem import Draw
 from rdkit.Chem import rdDepictor
 from rdkit.Chem.Draw import rdMolDraw2D
@@ -32,23 +34,24 @@
         # This sets the window to delete itself when its closed, so it doesn't keep querying the model
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose)
 
         # Properties
         self._prevmol = None  # For undo
         self.coordlist = None  # SVG coords of the current mols atoms
 
-        # Standard atom types
+        # Standard atom, bond and ring types
         self.symboltoint = symboltoint
-
         self.bondtypes = Chem.rdchem.BondType.names  # A dictionary with all available rdkit bondtypes
+        self.available_rings = ["ALI6", "ARO6"]
 
         # Default actions
         self._action = "Add"
-        self._bondtype = self.bondtypes["SINGLE"]
-        self._atomtype = 6
+        # self._chemEntityType = "bond"
+        # self._chemEntitySubType = self.bondtypes["SINGLE"]
+        self.chemEntity = self.bondtypes["SINGLE"]
 
         # Points to calculate the SVG to coord scaling
         self.points = [Point2D(0, 0), Point2D(1, 1)]
 
         # Bind signals to slots
         self.finishedDrawing.connect(self.update_coordlist)  # When drawing finished, update coordlist of SVG atoms.
 
@@ -68,57 +71,143 @@
         if actionname != self.action:
             self._action = actionname
             self.actionChanged.emit()
 
     def setAction(self, actionname):
         self.action = actionname
 
-    bondTypeChanged = QtCore.Signal(name="bondTypeChanged")
+    # bondTypeChanged = QtCore.Signal(name="bondTypeChanged")
+
+    # chemEntityTypeChanged = QtCore.Signal(name="chemEntityTypeChanged")
+
+    @property
+    def chemEntity(self):
+        return self._chementity
+
+    @chemEntity.setter
+    def chemEntity(self, chementity):
+        if isinstance(chementity, Chem.rdchem.BondType):  # Bondtypes are also ints, but ints are not BondTypes
+            self.setBond(chementity)
+        elif isinstance(chementity, int):
+            self.setAtom(chementity)
+        elif isinstance(chementity, str):
+            if chementity in self.bondtypes:
+                self.setBond(chementity)
+            elif chementity in self.available_rings:
+                self.setRing(chementity)
+            elif chementity in symboltoint.keys():
+                self.setAtom(chementity)
+            else:
+                self.logger.error(f"Unknown string entity type with value {chementity}")
+                return
+        else:
+            self.logger.error(f"Unknown type {type(chementity)}")
+            return
+        # self.logger.debug(f"ChemEntity set for {chementity} of type {type(chementity)}")
+
+    def setChemEntity(self, chementity):
+        self.chemEntity = chementity
+
+    # Readonly, inferred from chemEntity
+    @property
+    def chemEntityType(self):
+        return self._chementitytype
 
     @property
     def bondtype(self):
+        warn(
+            ".bondtype has been deprecated, in favor of .chemEntityType and setter .chemEntity.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._bondtype
 
+    @property
+    def ringtype(self):
+        warn(
+            ".ringtype has been deprecated, in favor of .chemEntityType and setter .chemEntity.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._ringtype
+
     @bondtype.setter
     def bondtype(self, bondtype):
+        warn(
+            ".bondtype has been deprecated, in favor of .chemEntityType and setter .chemEntity.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         if bondtype != self.bondtype:
             self._bondtype = bondtype
-            self.bondTypeChanged.emit()
+            # self.bondTypeChanged.emit()
+
+    @ringtype.setter
+    def ringtype(self, ringtype):
+        warn(
+            ".ringtype has been deprecated, in favor of .chemEntityType and setter .chemEntity.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        if ringtype != self.ringtype:
+            self._ringtype = ringtype
+
+    def setRing(self, ringtype):
+        if ringtype in self.available_rings:
+            self._chementitytype = "ring"
+            self._chementity = ringtype
+        else:
+            self.logger.error(f"Currently only {self.available_rings} are supported.")
 
-    def setBondType(self, bondtype):
+    def setBond(self, bondtype):
         if type(bondtype) == Chem.rdchem.BondType:
-            self.bondtype = bondtype
+            self._chementitytype = "bond"
+            self._chementity = bondtype
+
         elif isinstance(bondtype, str):
             assert bondtype in self.bondtypes.keys(), "Bondtype %s not known" % bondtype
-            self.bondtype = self.bondtypes[bondtype]
+            self._chementitytype = "bond"
+            self._chementity = self.bondtypes[bondtype]
         else:
             self.logger.error("Bondtype must be string or rdchem.BondType, not %s" % type(bondtype))
 
-    atomTypeChanged = QtCore.Signal(name="atomTypeChanged")
-
     @property
     def atomtype(self):
+        warn(
+            ".atomtype has been deprecated, in favor of .chemEntityType and setter .chemEntity.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._atomtype
 
     @atomtype.setter
     def atomtype(self, atomtype):
+        warn(
+            ".atomtype has been deprecated, in favor of .chemEntityType and setter .chemEntity.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         if atomtype != self.atomtype:
             self._atomtype = atomtype
-            self.atomTypeChanged.emit()
 
-    def setAtomType(self, atomtype):
+    def setAtom(self, atomtype):
         self.logger.debug("Setting atomtype selection to %s" % atomtype)
         if atomtype in self.symboltoint.keys():
             self.logger.debug("Atomtype found in keys")
-            self.atomtype = self.symboltoint[atomtype]
-        elif type(atomtype) == IntType:
-            # Can we assert that its a proper number known by RDKit??
-            self.atomtype = atomtype
+            # self.atomtype = self.symboltoint[atomtype]
+            self._chementitytype = "atom"
+            self._chementity = self.symboltoint[atomtype]
+        elif isinstance(atomtype, int):
+            if atomtype in self.symboltoint.values():
+                self._chementitytype = "atom"
+                self._chementity = atomtype
+            else:
+                self.logger.error(f"Atom number {atomtype} not known.")
         else:
-            self.error("Atomtype must be string or integer, not %s" % type(atomtype))
+            self.logger.error("Atomtype must be string or integer, not %s" % type(atomtype))
 
     # Function to translate from SVG coords to atom coords using scaling calculated from atomcoords (0,0) and (1,1)
     # Returns rdkit Point2D
     def SVG_to_coord(self, x_svg, y_svg):
         if self.drawer is not None:
             scale0 = self.drawer.GetDrawCoords(self.points[0])
             scale1 = self.drawer.GetDrawCoords(self.points[1])
@@ -212,82 +301,188 @@
             elif type(clicked) == Point2D:
                 self.logger.debug("Canvas Click")
                 self.canvas_click(clicked)
 
     # Lookup tables to relate actions to context type with action type #TODO more clean to use Dictionaries??
     def atom_click(self, atom):
         if self.action == "Add":
-            self.add_atom_to(atom)
+            self.add_to_atom(atom)
         elif self.action == "Remove":
             self.remove_atom(atom)
         elif self.action == "Select":
             self.select_atom_add(atom)
         elif self.action == "Replace":
-            self.replace_atom(atom)
+            self.replace_on_atom(atom)
         elif self.action == "Add Bond":
             self.add_bond(atom)
         elif self.action == "Increase Charge":
             self.increase_charge(atom)
         elif self.action == "Decrease Charge":
             self.decrease_charge(atom)
         elif self.action == "RStoggle":
             self.toogleRS(atom)
         else:
             self.logger.warning("The combination of Atom click and Action %s undefined" % self.action)
 
     def bond_click(self, bond):
         if self.action == "Add":
-            self.toggle_bond(bond)
+            self.add_to_bond(bond)
         elif self.action == "Add Bond":
             self.replace_bond(bond)
         elif self.action == "Remove":
             self.remove_bond(bond)
         elif self.action == "Select":
             self.select_bond(bond)
         elif self.action == "Replace":
-            self.replace_bond(bond)
+            self.replace_on_bond(bond)
         elif self.action == "EZtoggle":
             self.toogleEZ(bond)
         else:
             self.logger.warning("The combination of Bond click and Action %s undefined" % self.action)
 
     def canvas_click(self, point):
         if self.action == "Add":
-            self.add_canvas_atom(point)
+            self.add_canvas_entity(point)
+
         elif self.action == "Select":
             # Click on canvas
             # Unselect any selected
             if len(self.selectedAtoms) > 0:
                 self.clearAtomSelection()
         else:
             self.logger.warning("The combination of Canvas click and Action %s undefined" % self.action)
 
-    # Atom Actions
-    def add_atom_to(self, atom):
+    def add_to_atom(self, atom):
+        if self.chemEntityType == "atom":
+            self.add_atom_to_atom(atom)
+        if self.chemEntityType == "ring":
+            self.add_ring_to_atom(atom)
+        if self.chemEntityType == "bond":
+            self.add_bond_to_atom(atom)
+
+    def add_atom_to_atom(self, atom):
         rwmol = Chem.rdchem.RWMol(self.mol)
-        newatom = Chem.rdchem.Atom(self.atomtype)
+        newatom = Chem.rdchem.Atom(self.chemEntity)
         newidx = rwmol.AddAtom(newatom)
-        newbond = rwmol.AddBond(atom.GetIdx(), newidx, order=self.bondtype)
+        newbond = rwmol.AddBond(atom.GetIdx(), newidx, Chem.rdchem.BondType.SINGLE)
         self.mol = rwmol
 
+    def add_bond_to_atom(self, atom):
+        rwmol = Chem.rdchem.RWMol(self.mol)
+        newatom = Chem.rdchem.Atom(6)
+        newidx = rwmol.AddAtom(newatom)
+        newbond = rwmol.AddBond(atom.GetIdx(), newidx, order=self.chemEntity)
+        self.mol = rwmol
+
+    def add_ring_to_atom(self, atom):
+        if self.chemEntity == "ARO6":
+            ring = Chem.MolFromSmiles("c1ccccc1")
+        elif self.chemEntity == "ALI6":
+            ring = Chem.MolFromSmiles("C1CCCCC1")
+        combined = Chem.rdchem.RWMol(Chem.CombineMols(self.mol, ring))
+        _ = combined.AddBond(atom.GetIdx(), self.mol.GetNumAtoms(), Chem.rdchem.BondType.SINGLE)
+        self.mol = combined
+
+    def add_to_bond(self, bond):
+        if self.chemEntityType == "atom":
+            self.toggle_bond(bond)
+        if self.chemEntityType == "ring":
+            self.add_ring_to_bond(bond)
+        if self.chemEntityType == "bond":
+            self.replace_bond(bond)
+
+    def add_ring_to_bond(self, bond):
+        if self.chemEntity == "ARO6":
+            ring = Chem.MolFromSmarts("c:c:c:c")
+            bondType = Chem.rdchem.BondType.AROMATIC
+        if self.chemEntity == "ALI6":
+            ring = Chem.MolFromSmarts("C-C-C-C")
+            bondType = Chem.rdchem.BondType.SINGLE
+        combined = Chem.rdchem.RWMol(Chem.CombineMols(self.mol, ring))
+        combined.AddBond(
+            bond.GetEndAtomIdx(),
+            self.mol.GetNumAtoms() + 3,
+            bondType,
+        )
+
+        combined.AddBond(
+            bond.GetBeginAtomIdx(),
+            self.mol.GetNumAtoms(),
+            bondType,
+        )
+        # if bond to which aromatic ring is added is not aromatic it will be made aromatic
+        if self.chemEntity == "ARO6":
+            combined.GetBondWithIdx(bond.GetIdx()).SetIsAromatic(True)
+        # the extra sanitization is done to make sure that aromaticity is correctly displayed
+        try:
+            Chem.SanitizeMol(combined)
+            self.mol = Chem.MolFromSmiles(Chem.MolToSmiles(combined))
+        except Exception as e:
+            self.mol = combined
+
+    def add_canvas_entity(self, point):
+        if self.chemEntityType == "atom":
+            self.add_canvas_atom(point)
+        if self.chemEntityType == "ring":
+            self.add_canvas_ring(point)
+        if self.chemEntityType == "bond":
+            self.add_canvas_bond(point)
+
     def add_canvas_atom(self, point):
         rwmol = Chem.rdchem.RWMol(self.mol)
         if rwmol.GetNumAtoms() == 0:
             point.x = 0.0
             point.y = 0.0
-        newatom = Chem.rdchem.Atom(self.atomtype)
+        newatom = Chem.rdchem.Atom(self.chemEntity)
         newidx = rwmol.AddAtom(newatom)
         # This should only trigger if we have an empty canvas
         if not rwmol.GetNumConformers():
             rdDepictor.Compute2DCoords(rwmol)
         conf = rwmol.GetConformer(0)
         p3 = Point3D(point.x, point.y, 0)
         conf.SetAtomPosition(newidx, p3)
         self.mol = rwmol
 
+    def add_canvas_bond(self, point):
+        rwmol = Chem.rdchem.RWMol(self.mol)
+        if rwmol.GetNumAtoms() == 0:
+            point.x = 0.0
+            point.y = 0.0
+
+        atom_0 = rwmol.AddAtom(Chem.rdchem.Atom(6))
+        atom_1 = rwmol.AddAtom(Chem.rdchem.Atom(6))
+        print(self.chemEntity)
+        newidx = rwmol.AddBond(atom_0, atom_1, order=self.chemEntity)
+
+        # This should only trigger if we have an empty canvas
+        if not rwmol.GetNumConformers():
+            rdDepictor.Compute2DCoords(rwmol)
+        conf = rwmol.GetConformer(0)
+        p3 = Point3D(point.x, point.y, 0)
+        conf.SetAtomPosition(self.mol.GetNumAtoms(), p3)
+        self.mol = rwmol
+
+    def add_canvas_ring(self, point):
+        if self.chemEntity == "ARO6":
+            ring = Chem.MolFromSmiles("c1ccccc1")
+        elif self.chemEntity == "ALI6":
+            ring = Chem.MolFromSmiles("C1CCCCC1")
+
+        if self.mol.GetNumAtoms() == 0:
+            point.x = 0.0
+            point.y = 0.0
+        combined = Chem.rdchem.RWMol(Chem.CombineMols(self.mol, ring))
+        # This should only trigger if we have an empty canvas
+        if not combined.GetNumConformers():
+            rdDepictor.Compute2DCoords(combined)
+        conf = combined.GetConformer(0)
+        p3 = Point3D(point.x, point.y, 0)
+        conf.SetAtomPosition(self.mol.GetNumAtoms(), p3)
+        self.mol = combined
+
     def remove_atom(self, atom):
         rwmol = Chem.rdchem.RWMol(self.mol)
         rwmol.RemoveAtom(atom.GetIdx())
         self.clearAtomSelection()  # Removing atoms updates Idx'es
         self.mol = rwmol
 
     def select_atom(self, atom):
@@ -297,28 +492,35 @@
     def select_atom_add(self, atom):
         selidx = atom.GetIdx()
         if selidx in self._selectedAtoms:
             self.unselectAtom(selidx)
         else:
             self.selectAtomAdd(selidx)
 
+    def replace_on_atom(self, atom):
+        if self.chemEntityType == "atom":
+            self.replace_atom(atom)
+        else:
+            pass
+
     def replace_atom(self, atom):
         rwmol = Chem.rdchem.RWMol(self.mol)
-        newatom = Chem.rdchem.Atom(self.atomtype)
+        newatom = Chem.rdchem.Atom(self.chemEntity)
         rwmol.ReplaceAtom(atom.GetIdx(), newatom)
         self.mol = rwmol
 
     # Double step action
     def add_bond(self, atom):
         if len(self.selectedAtoms) > 0:
             selected = self.selectedAtoms[-1]
             rwmol = Chem.rdchem.RWMol(self.mol)
             neighborIdx = [atm.GetIdx() for atm in self.mol.GetAtomWithIdx(selected).GetNeighbors()]
             if atom.GetIdx() not in neighborIdx:  # check if bond already exists
-                rwmol.AddBond(selected, atom.GetIdx(), order=self.bondtype)
+                bondType = self.chemEntity if self.chemEntityType == "bond" else Chem.rdchem.BondType.SINGLE
+                rwmol.AddBond(selected, atom.GetIdx(), order=bondType)
             self.mol = rwmol
             self.selectedAtoms = []
         else:
             self.select_atom(atom)
 
     def toogleRS(self, atom):
         self.backupMol()
@@ -365,15 +567,15 @@
         self.assert_stereo_atoms(bond)
         self.logger.debug("Current stereotype of clicked atom %s" % stereotype)
         # TODO: what if molecule already contain STEREOE or STEREOZ
         stereotypes = [
             Chem.rdchem.BondStereo.STEREONONE,
             Chem.rdchem.BondStereo.STEREOCIS,
             Chem.rdchem.BondStereo.STEREOTRANS,
-            #                        Chem.rdchem.BondStereo.STEREOANY, TODO, this should be wiggly, but is not
+            #  Chem.rdchem.BondStereo.STEREOANY, TODO, this should be wiggly, but is not
             Chem.rdchem.BondStereo.STEREONONE,
         ]
         newidx = np.argmax(np.array(stereotypes) == stereotype) + 1
         bond.SetStereo(stereotypes[newidx])
         self.logger.debug("New stereotype set to %s" % bond.GetStereo())
         try:
             self.logger.debug(
@@ -401,19 +603,26 @@
         # Find the next type in the list based on current
         # If current is not in list? Then it selects the first and add 1 => SINGLE
         newidx = np.argmax(np.array(bondtypes) == bondtype) + 1
         newtype = bondtypes[newidx]
         bond.SetBondType(newtype)
         self.molChanged.emit()
 
-    # self.replace_bond(bond)
+    def replace_on_bond(self, bond):
+        if self.chemEntityType == "atom":
+            self.toggle_bond(bond)
+        if self.chemEntityType == "ring":
+            self.toggle_bond(bond)
+        if self.chemEntityType == "bond":
+            self.replace_bond(bond)
+
     def replace_bond(self, bond):
         self.backupMol()
         self.logger.debug("Replacing bond %s" % bond)
-        bond.SetBondType(self.bondtype)
+        bond.SetBondType(self.chemEntity)
         self.molChanged.emit()
 
     # self.remove_bond(bond)
     def remove_bond(self, bond):
         rwmol = Chem.rdchem.RWMol(self.mol)
         rwmol.RemoveBond(bond.GetBeginAtomIdx(), bond.GetEndAtomIdx())
         self.mol = rwmol
```

### Comparing `rdeditor-0.1.3.9/rdeditor/molViewWidget.py` & `rdeditor-0.2.0/rdeditor/molViewWidget.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from rdkit.Chem import Draw
 from rdkit.Chem import rdDepictor
 from rdkit.Chem.Draw import rdMolDraw2D
 from rdkit.Geometry.rdGeometry import Point2D
 
+from rdeditor.utilities import validate_rgb
+
 
 # The Viewer Class
 class MolWidget(QtSvg.QSvgWidget):
     def __init__(self, mol=None, parent=None):
         # Also init the super class
         super(MolWidget, self).__init__(parent)
 
@@ -31,17 +33,24 @@
         # Private Properties
         self._mol = None  # The molecule
         self._drawmol = None  # Molecule for drawing
         self.drawer = None  # drawing object for producing SVG
         self._selectedAtoms = []  # List of selected atoms
         self._darkmode = False
 
+        # Color settings
+        self._unsanitizable_background_colour = None  # (1, 0.75, 0.75)
+        self._last_selected_highlight_colour = (1, 0.2, 0.2)
+        self._selected_highlight_colour = (1, 0.5, 0.5)
+
         # Bind signales to slots for automatic actions
         self.molChanged.connect(self.sanitize_draw)
         self.selectionChanged.connect(self.draw)
+        self.drawSettingsChanged.connect(self.draw)
+        self.sanitizeSignal.connect(self.changeSanitizeStatus)
 
         # Initialize class with the mol passed
         self.mol = mol
 
     ##Properties and their wrappers
     @property
     def loglevel(self):
@@ -113,26 +122,70 @@
             assert all(isinstance(item, int) for item in atomlist), "selectedAtoms should be a list of integers"
             self._selectedAtoms = atomlist
             self.selectionChanged.emit()
 
     def setSelectedAtoms(self, atomlist):
         self.selectedAtoms = atomlist
 
+    drawSettingsChanged = QtCore.Signal(name="drawSettingsChanged")
+
+    @property
+    def unsanitizable_background_colour(self):
+        return self._unsanitizable_background_colour
+
+    @unsanitizable_background_colour.setter
+    def unsanitizable_background_colour(self, colour):
+        if colour != self._unsanitizable_background_colour:
+            if colour is not None:
+                assert validate_rgb(colour)
+            self._unsanitizable_background_colour = colour
+            self.drawSettingsChanged.emit()
+
+    @property
+    def last_selected_highlight_colour(self):
+        return self._last_selected_highlight_colour
+
+    @last_selected_highlight_colour.setter
+    def last_selected_highlight_colour(self, colour):
+        assert validate_rgb(colour)
+        if colour != self._last_selected_highlight_colour:
+            self._last_selected_highlight_colour = colour
+            self.drawSettingsChanged.emit()
+
+    @property
+    def selected_highlight_colour(self):
+        return self._selected_highlight_colour
+
+    @selected_highlight_colour.setter
+    def selected_highlight_colour(self, colour):
+        if colour != self._selected_highlight_colour:
+            assert validate_rgb(colour)
+            self._selected_highlight_colour = colour
+            self.drawSettingsChanged.emit()
+
     # Actions and functions
     @QtCore.Slot()
     def draw(self):
         self.logger.debug("Updating SVG")
         svg = self.getMolSvg()
         self.load(QtCore.QByteArray(svg.encode("utf-8")))
 
     @QtCore.Slot()
     def sanitize_draw(self):
         self.sanitizeMol()
         self.draw()
 
+    @QtCore.Slot()
+    def changeSanitizeStatus(self, value):
+        self.logger.debug(f"changeBorder called with value {value}")
+        if value.upper() == "SANITIZABLE":
+            self.molecule_sanitizable = True
+        else:
+            self.molecule_sanitizable = False
+
     def computeNewCoords(self, ignoreExisting=False, canonOrient=False):
         """Computes new coordinates for the molecule taking into account all
         existing positions (feeding these to the rdkit coordinate generation as
         prev_coords).
         """
         # This code is buggy when you are not using the CoordGen coordinate
         # generation system, so we enable it here
@@ -196,19 +249,24 @@
         # TODO, what if self._drawmol doesn't exist?
         if self._drawmol is not None:
             # Chiral tags on R/S
             chiraltags = Chem.FindMolChiralCenters(self._drawmol)
             opts = self.drawer.drawOptions()
             if self._darkmode:
                 rdMolDraw2D.SetDarkMode(opts)
+            if (not self.molecule_sanitizable) and self.unsanitizable_background_colour:
+                opts.setBackgroundColour(self.unsanitizable_background_colour)
             for tag in chiraltags:
                 idx = tag[0]
                 opts.atomLabels[idx] = self._drawmol.GetAtomWithIdx(idx).GetSymbol() + ":" + tag[1]
             if len(self._selectedAtoms) > 0:
-                colors = {self._selectedAtoms[-1]: (1, 0.2, 0.2)}  # Color lastly selected a different color
+                colors = {atom_idx: self.selected_highlight_colour for atom_idx in self._selectedAtoms}
+                colors[self._selectedAtoms[-1]] = (
+                    self.last_selected_highlight_colour
+                )  # Color lastly selected an optionally different color
                 self.drawer.DrawMolecule(
                     self._drawmol,
                     highlightAtoms=self._selectedAtoms,
                     highlightAtomColors=colors,
                 )
             else:
                 self.drawer.DrawMolecule(self._drawmol)
```

### Comparing `rdeditor-0.1.3.9/rdeditor/ptable.py` & `rdeditor-0.2.0/rdeditor/ptable.py`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.9/rdeditor/ptable_widget.py` & `rdeditor-0.2.0/rdeditor/ptable_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,42 +6,40 @@
 
 from PySide2 import QtGui, QtCore, QtWidgets
 
 from rdeditor.ptable import ptable
 
 
 class PTable(QtWidgets.QWidget):
-    def __init__(self):
+    def __init__(self, actionGroup):
         super(PTable, self).__init__()
         self.ptable = ptable
-        self.initUI()
+        self.initUI(actionGroup)
         # logging
         self.logger = logging.getLogger()
 
-    def initUI(self):
+    def initUI(self, actionGroup):
         grid = QtWidgets.QGridLayout()
         # Create actions dictionary and group dictionary
-        self.atomActionGroup = QtWidgets.QActionGroup(self, exclusive=True)
+        # self.atomActionGroup = QtWidgets.QActionGroup(self, exclusive=True)
         self.atomActions = {}
         # for atomname in self.editor.atomtypes.keys(): Gives unsorted list
         for key in self.ptable.keys():
             atomname = self.ptable[key]["Symbol"]
             action = QtWidgets.QAction(
                 "%s" % atomname,
                 self,
                 statusTip="Set atomtype to %s" % atomname,
                 triggered=self.atomtypePush,
                 objectName=atomname,
                 checkable=True,
             )
-            self.atomActionGroup.addAction(action)
+            # self.atomActionGroup.addAction(action)
+            actionGroup.addAction(action)
             self.atomActions[atomname] = action
-            if action.objectName() == "C":
-                action.setChecked(True)
-
             button = QtWidgets.QToolButton()
             button.setDefaultAction(action)
             button.setFocusPolicy(QtCore.Qt.NoFocus)
             button.setMaximumWidth(40)
 
             if self.ptable[key]["Group"] is not None:
                 grid.addWidget(button, self.ptable[key]["Period"], self.ptable[key]["Group"])
```

### Comparing `rdeditor-0.1.3.9/rdeditor/rdEditor.py` & `rdeditor-0.2.0/rdeditor/rdEditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,33 +18,37 @@
 
 # Import model
 import rdeditor
 from rdeditor.molEditWidget import MolEditWidget
 from rdeditor.ptable_widget import PTable
 
 from rdkit import Chem
+import qdarktheme
 
 
 # The main window class
 class MainWindow(QtWidgets.QMainWindow):
     # Constructor function
     def __init__(self, fileName=None, loglevel="WARNING"):
         super(MainWindow, self).__init__()
         self.pixmappath = os.path.abspath(os.path.dirname(__file__)) + "/pixmaps/"
         QtGui.QIcon.setThemeSearchPaths(
             # QtGui.QIcon.themeSearchPaths() +
             [os.path.abspath(os.path.dirname(__file__)) + "/icon_themes/"]
         )
         self.loglevels = ["Critical", "Error", "Warning", "Info", "Debug", "Notset"]
         self.editor = MolEditWidget()
-        self.ptable = PTable()
+        self.chemEntityActionGroup = QtWidgets.QActionGroup(self, exclusive=True)
+        self.ptable = PTable(self.chemEntityActionGroup)
         self._fileName = None
         self.initGUI(fileName=fileName)
         self.applySettings()
         self.ptable.atomtypeChanged.connect(self.setAtomTypeName)
+        # self.singleBondAction.trigger()
+        self.ptable.atomActions["C"].trigger()
 
     # Properties
     @property
     def fileName(self):
         return self._fileName
 
     @fileName.setter
@@ -55,15 +59,15 @@
 
     def initGUI(self, fileName=None):
         self.setWindowTitle("rdEditor")
         self.setWindowIcon(QIcon.fromTheme("appicon"))
         self.setGeometry(100, 100, 200, 150)
 
         self.center = self.editor
-        self.center.setFixedSize(600, 600)
+        self.center.setFixedSize(650, 650)
         self.setCentralWidget(self.center)
         self.fileName = fileName
 
         self.filters = "MOL Files (*.mol *.mol);;SMILES Files (*.smi *.smi);;Any File (*)"
 
         self.SetupComponents()
 
@@ -104,15 +108,15 @@
 
         return all_actions
 
     def resetActionIcons(self):
         actions_with_icons = list(set(self.getAllIconActions(QApplication)))
         for action in actions_with_icons:
             icon_name = action.icon().name()
-            print(f"reset icon {icon_name}")
+            self.editor.logger.debug(f"reset icon {icon_name}")
             action.setIcon(QIcon.fromTheme(icon_name))
 
     def applySettings(self):
         self.settings = QSettings("Cheminformania.com", "rdEditor")
         theme_name = self.settings.value("theme_name", "Fusion")
 
         self.applyTheme(theme_name)
@@ -213,15 +217,21 @@
         # Debug level sub menu
 
     def populateThemeActions(self, menu: QMenu):
         stylelist = QStyleFactory.keys() + ["Qdt light", "Qdt dark"]
         self.themeActionGroup = QtWidgets.QActionGroup(self, exclusive=True)
         self.themeActions = {}
         for style_name in stylelist:
-            action = QAction(style_name, self, objectName=style_name, triggered=self.setTheme, checkable=True)
+            action = QAction(
+                style_name,
+                self,
+                objectName=style_name,
+                triggered=self.setTheme,
+                checkable=True,
+            )
             self.themeActionGroup.addAction(action)
             self.themeActions[style_name] = action
             menu.addAction(action)
 
     def CreateToolBars(self):
         self.mainToolBar = self.addToolBar("Main")
         # Main action bar
@@ -249,14 +259,17 @@
         # Side Toolbar
         self.sideToolBar = QtWidgets.QToolBar(self)
         self.addToolBar(QtCore.Qt.LeftToolBarArea, self.sideToolBar)
         self.sideToolBar.addAction(self.singleBondAction)
         self.sideToolBar.addAction(self.doubleBondAction)
         self.sideToolBar.addAction(self.tripleBondAction)
         self.sideToolBar.addSeparator()
+        self.sideToolBar.addAction(self.ringAliphatic6Action)
+        self.sideToolBar.addAction(self.ringAromatic6Action)
+        self.sideToolBar.addSeparator()
         for action in self.atomActions:
             self.sideToolBar.addAction(action)
         self.sideToolBar.addAction(self.openPtableAction)
 
     def loadSmilesFile(self, filename):
         self.fileName = filename
         with open(self.fileName, "r") as file:
@@ -348,15 +361,15 @@
         self.exitFile()
         event.ignore()
 
     def exitFile(self):
         response = self.msgApp("Confirmation", "This will quit the application. Do you want to Continue?")
         if response == "Y":
             self.ptable.close()
-            exit(0)  # TODO, how to exit qapplication from within class instance?
+            exit(0)
         else:
             self.editor.logger.debug("Abort closing")
 
     # Function to show Diaglog box with provided Title and Message
     def msgApp(self, title, msg):
         userInfo = QMessageBox.question(self, title, msg)
         if userInfo == QMessageBox.Yes:
@@ -378,35 +391,42 @@
         )
 
     def setAction(self):
         sender = self.sender()
         self.editor.setAction(sender.objectName())
         self.myStatusBar.showMessage("Action %s selected" % sender.objectName())
 
+    # TODO, the various setTypes could be unified, as the editor now understands a single chementity
+    def setRingType(self):
+        sender = self.sender()
+        self.editor.setChemEntity(sender.objectName())
+        self.myStatusBar.showMessage("Ringtype %s selected" % sender.objectName())
+
     def setBondType(self):
         sender = self.sender()
-        self.editor.setBondType(sender.objectName())
+        self.editor.setChemEntity(sender.objectName())
         self.myStatusBar.showMessage("Bondtype %s selected" % sender.objectName())
 
     def setAtomType(self):
         sender = self.sender()
-        self.editor.setAtomType(sender.objectName())
+        self.editor.setChemEntity(sender.objectName())
+        # self.editor.setRingType(None)
         self.myStatusBar.showMessage("Atomtype %s selected" % sender.objectName())
 
     def setAtomTypeName(self, atomname):
-        self.editor.setAtomType(str(atomname))
+        self.editor.setChemEntity(str(atomname))
         self.myStatusBar.showMessage("Atomtype %s selected" % atomname)
 
     def openPtable(self):
         self.ptable.show()
 
     def setLogLevel(self):
         loglevel = self.sender().objectName().split(":")[-1]  # .upper()
         self.editor.logger.setLevel(loglevel.upper())
-        print(f"Sat loglevel to {loglevel}")
+        self.editor.logger.log(self.editor.logger.getEffectiveLevel(), f"loglevel set to {loglevel}")
         self.settings.setValue("loglevel", loglevel)
         self.settings.sync()
 
     def setTheme(self):
         sender = self.sender()
         theme_name = sender.objectName()
         self.myStatusBar.showMessage(f"Setting theme or style to {theme_name}")
@@ -483,15 +503,18 @@
             "A&bout",
             self,
             statusTip="Displays info about text editor",
             triggered=self.aboutHelp,
         )
 
         self.aboutQtAction = QAction(
-            "About &Qt", self, statusTip="Show the Qt library's About box", triggered=QApplication.aboutQt
+            "About &Qt",
+            self,
+            statusTip="Show the Qt library's About box",
+            triggered=QApplication.aboutQt,
         )
 
         self.openPtableAction = QAction(
             QIcon.fromTheme("ptable"),
             "O&pen Periodic Table",
             self,
             shortcut=QKeySequence.Open,
@@ -638,58 +661,85 @@
             self,
             shortcut="Ctrl+1",
             statusTip="Set bondtype to SINGLE",
             triggered=self.setBondType,
             objectName="SINGLE",
             checkable=True,
         )
-        self.bondtypeActionGroup.addAction(self.singleBondAction)
+        self.chemEntityActionGroup.addAction(self.singleBondAction)
 
         self.doubleBondAction = QAction(
             QIcon.fromTheme("icons8-Double"),
             "Double Bond",
             self,
             shortcut="Ctrl+2",
             statusTip="Set bondtype to DOUBLE",
             triggered=self.setBondType,
             objectName="DOUBLE",
             checkable=True,
         )
-        self.bondtypeActionGroup.addAction(self.doubleBondAction)
+        self.chemEntityActionGroup.addAction(self.doubleBondAction)
 
         self.tripleBondAction = QAction(
             QIcon.fromTheme("icons8-Triple"),
             "Triple Bond",
             self,
             shortcut="Ctrl+3",
             statusTip="Set bondtype to TRIPLE",
             triggered=self.setBondType,
             objectName="TRIPLE",
             checkable=True,
         )
-        self.bondtypeActionGroup.addAction(self.tripleBondAction)
-        self.singleBondAction.setChecked(True)
+        self.chemEntityActionGroup.addAction(self.tripleBondAction)
+
+        # self.singleBondAction.setChecked(True)
+
+        self.ringAromatic6Action = QAction(
+            QIcon.fromTheme("benzene"),
+            "Benzene Ring",
+            self,
+            shortcut="Ctrl+4",
+            statusTip="Select Benzene Ring",
+            triggered=self.setRingType,
+            objectName="ARO6",
+            checkable=True,
+        )
+        self.chemEntityActionGroup.addAction(self.ringAromatic6Action)
+        self.ringAliphatic6Action = QAction(
+            QIcon.fromTheme("cyclohexane"),
+            "Aliphatic Six Ring",
+            self,
+            shortcut="Ctrl+5",
+            statusTip="Select Aliphatic Ring",
+            triggered=self.setRingType,
+            objectName="ALI6",
+            checkable=True,
+        )
+        self.chemEntityActionGroup.addAction(self.ringAliphatic6Action)
 
         # Build dictionary of ALL available bondtypes in RDKit
         self.bondActions = {}
         for key in self.editor.bondtypes.keys():
             action = QAction(
                 "%s" % key,
                 self,
                 statusTip="Set bondtype to %s" % key,
                 triggered=self.setBondType,
                 objectName=key,
                 checkable=True,
             )
-            self.bondtypeActionGroup.addAction(action)
+            self.chemEntityActionGroup.addAction(action)
             self.bondActions[key] = action
         # Replace defined actions
+
         self.bondActions["SINGLE"] = self.singleBondAction
         self.bondActions["DOUBLE"] = self.doubleBondAction
         self.bondActions["TRIPLE"] = self.tripleBondAction
+        self.bondActions["ARO6"] = self.ringAromatic6Action
+        self.bondActions["ALI6"] = self.ringAliphatic6Action
 
         # Misc Actions
         self.undoAction = QAction(
             QIcon.fromTheme("prev"),
             "U&ndo",
             self,
             shortcut="Ctrl+Z",
@@ -718,16 +768,14 @@
             objectName="Recalculate Coordinates",
         )
 
         # Atom Actions in actiongroup, reuse from ptable widget
         self.atomActions = []
         for atomname in ["H", "B", "C", "N", "O", "F", "P", "S", "Cl", "Br", "I"]:
             action = self.ptable.atomActions[atomname]
-            if action.objectName() == "C":
-                action.setChecked(True)
             self.atomActions.append(action)
 
         self.loglevelactions = {}
         self.loglevelActionGroup = QtWidgets.QActionGroup(self, exclusive=True)
         for key in self.loglevels:
             self.loglevelactions[key] = QAction(
                 key,
```

### Comparing `rdeditor-0.1.3.9/rdeditor.egg-info/PKG-INFO` & `rdeditor-0.2.0/rdeditor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdeditor
-Version: 0.1.3.9
+Version: 0.2.0
 Summary: An RDKit based molecule editor using PySide
 Home-page: http://github.com/ebjerrum/rdeditor
 Author: Esben Jannik Bjerrum
 Author-email: esbenjannik@rocketmail.com
 License: LGPL
 Keywords: RDKit molecule editor pyside
 Requires-Python: >=3.8
```

### Comparing `rdeditor-0.1.3.9/rdeditor.egg-info/SOURCES.txt` & `rdeditor-0.2.0/rdeditor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,31 @@
 rdeditor/__init__.py
 rdeditor/_version.py
 rdeditor/molEditWidget.py
 rdeditor/molViewWidget.py
 rdeditor/ptable.py
 rdeditor/ptable_widget.py
 rdeditor/rdEditor.py
+rdeditor/utilities.py
 rdeditor.egg-info/PKG-INFO
 rdeditor.egg-info/SOURCES.txt
 rdeditor.egg-info/dependency_links.txt
 rdeditor.egg-info/entry_points.txt
 rdeditor.egg-info/not-zip-safe
 rdeditor.egg-info/requires.txt
 rdeditor.egg-info/top_level.txt
 rdeditor/icon_themes/dark/index.theme
 rdeditor/icon_themes/dark/application/Change_E_Z.png
 rdeditor/icon_themes/dark/application/Change_E_Z.svg
 rdeditor/icon_themes/dark/application/Change_R_S.png
 rdeditor/icon_themes/dark/application/about.png
 rdeditor/icon_themes/dark/application/appicon.png
+rdeditor/icon_themes/dark/application/benzene.png
 rdeditor/icon_themes/dark/application/calc.png
+rdeditor/icon_themes/dark/application/cyclohexane.png
 rdeditor/icon_themes/dark/application/exit.png
 rdeditor/icon_themes/dark/application/grid.png
 rdeditor/icon_themes/dark/application/icons8-Broom.png
 rdeditor/icon_themes/dark/application/icons8-Bulleted List.png
 rdeditor/icon_themes/dark/application/icons8-Cancel.png
 rdeditor/icon_themes/dark/application/icons8-Carbon.png
 rdeditor/icon_themes/dark/application/icons8-Cursor.png
@@ -81,15 +84,19 @@
 rdeditor/icon_themes/light/application/Change_E_Z.png
 rdeditor/icon_themes/light/application/Change_E_Z.svg
 rdeditor/icon_themes/light/application/Change_R_S.png
 rdeditor/icon_themes/light/application/about.png
 rdeditor/icon_themes/light/application/appicon copy.png
 rdeditor/icon_themes/light/application/appicon.png
 rdeditor/icon_themes/light/application/appicon.svg.png
+rdeditor/icon_themes/light/application/benzene.png
+rdeditor/icon_themes/light/application/benzene.svg
 rdeditor/icon_themes/light/application/calc.png
+rdeditor/icon_themes/light/application/cyclohexane.png
+rdeditor/icon_themes/light/application/cyclohexane.svg
 rdeditor/icon_themes/light/application/exit.png
 rdeditor/icon_themes/light/application/grid.png
 rdeditor/icon_themes/light/application/icons8-Broom.png
 rdeditor/icon_themes/light/application/icons8-Bulleted List.png
 rdeditor/icon_themes/light/application/icons8-Cancel.png
 rdeditor/icon_themes/light/application/icons8-Carbon.png
 rdeditor/icon_themes/light/application/icons8-Cursor.png
```

### Comparing `rdeditor-0.1.3.9/setup.py` & `rdeditor-0.2.0/setup.py`

 * *Files identical despite different names*

