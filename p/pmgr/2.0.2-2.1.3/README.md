# Comparing `tmp/pmgr-2.0.2.tar.gz` & `tmp/pmgr-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmgr-2.0.2.tar", last modified: Wed Jul 14 21:27:26 2021, max compression
+gzip compressed data, was "pmgr-2.1.3.tar", last modified: Thu May  2 21:32:11 2024, max compression
```

## Comparing `pmgr-2.0.2.tar` & `pmgr-2.1.3.tar`

### file list

```diff
@@ -1,46 +1,70 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-07-14 21:27:26.933626 pmgr-2.0.2/
--rw-r--r--   0 klauer   (1318172782) 1704612529       74 2020-03-17 18:21:50.000000 pmgr-2.0.2/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529      244 2021-07-14 21:27:26.933846 pmgr-2.0.2/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      161 2021-07-14 21:26:57.000000 pmgr-2.0.2/README.md
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-07-14 21:27:26.935284 pmgr-2.0.2/pmgr/
--rw-r--r--   0 klauer   (1318172782) 1704612529    35057 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/CfgModel.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    20552 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/FreezeTableView.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4085 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/MyDelegate.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    44777 2021-07-14 21:27:11.000000 pmgr-2.0.2/pmgr/ObjModel.py
--rw-r--r--   0 klauer   (1318172782) 1704612529       92 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2021-07-14 21:27:26.935424 pmgr-2.0.2/pmgr/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1984 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/auth_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1661 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/cfgdialog_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1812 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/chown_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2005 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/colchoose_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3837 2021-06-01 17:29:30.000000 pmgr-2.0.2/pmgr/colmgr.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1580 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/colsave_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1576 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/coluse_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1645 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/confirmdialog_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5167 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/db.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2203 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/deriveddialog_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3631 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/dialogs.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    19784 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/docopt.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1425 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/errordialog_ui.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529    26657 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/harvester.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-07-14 21:27:26.933157 pmgr-2.0.2/pmgr/migrate/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/migrate/__init__.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     5471 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/migrate/fixup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    32543 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/migrate/pmgrobj.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2439 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/param.py
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     8922 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/pmgr.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9374 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/pmgrAPI.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1018 2020-03-17 18:21:50.000000 pmgr-2.0.2/pmgr/pmgrUtils.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529     8137 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/pmgrUtils.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11114 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/pmgr_ui.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    33940 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/pmgrobj.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8143 2021-07-14 21:26:57.000000 pmgr-2.0.2/pmgr/utils.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2021-07-14 21:27:26.931872 pmgr-2.0.2/pmgr.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529      244 2021-07-14 21:27:26.000000 pmgr-2.0.2/pmgr.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      765 2021-07-14 21:27:26.000000 pmgr-2.0.2/pmgr.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2021-07-14 21:27:26.000000 pmgr-2.0.2/pmgr.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       87 2021-07-14 21:27:26.000000 pmgr-2.0.2/pmgr.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        5 2021-07-14 21:27:26.000000 pmgr-2.0.2/pmgr.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      167 2021-07-14 21:27:26.934728 pmgr-2.0.2/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529      538 2021-07-14 21:26:57.000000 pmgr-2.0.2/setup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    68611 2020-03-17 18:21:50.000000 pmgr-2.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.785254 pmgr-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 21:31:47.000000 pmgr-2.1.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-02 21:31:47.000000 pmgr-2.1.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-02 21:31:47.000000 pmgr-2.1.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 21:31:47.000000 pmgr-2.1.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.773254 pmgr-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.777254 pmgr-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-02 21:31:47.000000 pmgr-2.1.3/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-02 21:31:47.000000 pmgr-2.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 21:31:47.000000 pmgr-2.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-02 21:31:47.000000 pmgr-2.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-02 21:31:47.000000 pmgr-2.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 21:31:47.000000 pmgr-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-02 21:32:11.785254 pmgr-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-02 21:31:47.000000 pmgr-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.777254 pmgr-2.1.3/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-02 21:31:47.000000 pmgr-2.1.3/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 21:31:47.000000 pmgr-2.1.3/dev-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      736 2024-05-02 21:31:47.000000 pmgr-2.1.3/do_release
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.781254 pmgr-2.1.3/pmgr/
+-rw-r--r--   0 runner    (1001) docker     (127)    35724 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/CfgModel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.785254 pmgr-2.1.3/pmgr/DB/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/DB/ims_motor.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/DB/ims_motor_cfg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/DB/ims_motor_cfg_log.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/DB/ims_motor_log.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/DB/ims_motor_name_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/DB/ims_motor_update.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/DB/procs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    20709 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/FreezeTableView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/MyDelegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46670 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/ObjModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 21:32:11.000000 pmgr-2.1.3/pmgr/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/auth.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/cfgdialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/chown.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/colchoose.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/colmgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/colsave.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/coluse.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/confirmdialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/deriveddialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19716 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/docopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/errordialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/param.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9249 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/pmgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/pmgr.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/pmgrAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/pmgrUtils.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/pmgrUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38196 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/pmgrobj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.785254 pmgr-2.1.3/pmgr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/tests/test_pmgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-02 21:31:47.000000 pmgr-2.1.3/pmgr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.785254 pmgr-2.1.3/pmgr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-02 21:32:11.000000 pmgr-2.1.3/pmgr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-02 21:32:11.000000 pmgr-2.1.3/pmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:32:11.000000 pmgr-2.1.3/pmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 21:32:11.000000 pmgr-2.1.3/pmgr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 21:32:11.000000 pmgr-2.1.3/pmgr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 21:32:11.000000 pmgr-2.1.3/pmgr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-02 21:31:47.000000 pmgr-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 21:31:47.000000 pmgr-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:32:11.785254 pmgr-2.1.3/setup.cfg
```

### Comparing `pmgr-2.0.2/pmgr/CfgModel.py` & `pmgr-2.1.3/pmgr/CfgModel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 import datetime
-import sys
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
-from . import colmgr
-from . import param
-from . import utils
+from . import colmgr, param, utils
 
 
-try:
-    QString = unicode
-except NameError:
-    # Python 3
-    QString = str
-
 class CfgModel(QtGui.QStandardItemModel):
     """
     This is the Model (from the Model-View-Controller paradigm) supporting
     the configuration table.  This is a 2D table: rows are configurations,
     and columns are configuration values.
 
     The heart of this is two routines:
         data(index, role) takes a QModelIndex and a Qt.DisplayRole and returns
         the value corresponding to that location in the table.
 
         setData(index, value, role) takes a QModelIndex and a new value, and
         stores that value into the table for the specified role.
     """
-    newname = QtCore.pyqtSignal(int, 'QString')
-    cfgChanged = QtCore.pyqtSignal(int, 'QString')
-    
+
+    newname = QtCore.pyqtSignal(int, "QString")
+    cfgChanged = QtCore.pyqtSignal(int, "QString")
+
     layoutAboutToBeChanged = QtCore.pyqtSignal()
     layoutChanged = QtCore.pyqtSignal()
-    cname   = ["Status", "Name", "Parent"]
-    cfld    = ["status", "name", "cfgname"]
-    ctips   = ["D = Deleted\nM = Modified\nN = New", "Configuration Name", "Parent Configuration"]
-    coff    = len(cname)
+    cname = ["Status", "Name", "Parent"]
+    cfld = ["status", "name", "cfgname"]
+    ctips = [
+        "D = Deleted\nM = Modified\nN = New",
+        "Configuration Name",
+        "Parent Configuration",
+    ]
+    coff = len(cname)
     statcol = 0
     namecol = 1
-    cfgcol  = 2
-    mutable = 2   # The first non-frozen column
+    cfgcol = 2
+    mutable = 2  # The first non-frozen column
     fixflds = ["status", "cfgname"]
-    
+
     def __init__(self):
         QtGui.QStandardItemModel.__init__(self)
         self.curidx = 0
         self.path = []
         self.edits = {}
         self.cfgs = {}
         self.status = {}
@@ -59,140 +55,139 @@
         font = QtGui.QFont()
         font.setBold(True)
         for c in range(self.colcnt):
             if c < self.coff:
                 i = QtGui.QStandardItem(self.cname[c])
                 i.setToolTip(self.ctips[c])
             else:
-                i = QtGui.QStandardItem(param.params.pobj.cfgflds[c-self.coff]['alias'])
-                desc = param.params.pobj.cfgflds[c-self.coff]['tooltip']
+                i = QtGui.QStandardItem(
+                    param.params.pobj.cfgflds[c - self.coff]["alias"]
+                )
+                desc = param.params.pobj.cfgflds[c - self.coff]["tooltip"]
                 if desc != "":
                     i.setToolTip(desc)
             self.setHorizontalHeaderItem(c, i)
         self.is_expanded = {}
         self.createStatus()
         self.hutchid = -1
         self.buildtree()
-        param.params.ui.treeWidget.expandItem(self.tree[0]['item']) # Expand DEFAULT.
+        param.params.ui.treeWidget.expandItem(self.tree[0]["item"])  # Expand DEFAULT.
         try:
-            param.params.ui.treeWidget.setCurrentItem(self.tree[self.hutchid]['item'])
+            param.params.ui.treeWidget.setCurrentItem(self.tree[self.hutchid]["item"])
             self.curidx = self.hutchid
-        except:
+        except Exception:
             self.setCurIdx(0)
         if self.curidx != 0:
-            param.params.ui.treeWidget.expandItem(self.tree[self.curidx]['item'])
+            param.params.ui.treeWidget.expandItem(self.tree[self.curidx]["item"])
         s = ""
         for f in param.params.pobj.mutex_flds:
-            s += chr(param.params.pobj.fldmap[f]['colorder']+0x40)
+            s += chr(param.params.pobj.fldmap[f]["colorder"] + 0x40)
         self.mutex_flds = s
 
     def createStatus(self):
         for d in param.params.pobj.cfgs.values():
-            try:
-                v = self.status[d['id']]
-            except:
-                self.status[d['id']] = ""
+            self.status.setdefault(d["id"], "")
 
     def cfgchange(self):
         self.createStatus()
         self.buildtree()
         try:
-            param.params.ui.treeWidget.setCurrentItem(self.tree[self.curidx]['item'])
-        except:
+            param.params.ui.treeWidget.setCurrentItem(self.tree[self.curidx]["item"])
+        except Exception:
             self.setCurIdx(0)
 
     def setModifiedStatus(self, index, idx, d):
         if idx < 0:
             return
         try:
-            v = self.status[idx].index("M")
+            self.status[idx].index("M")
             wasmod = True
-        except:
+        except Exception:
             wasmod = False
         mod = False
         try:
             if self.edits[idx] != {}:
                 mod = True
-        except:
+        except Exception:
             pass
         if mod != wasmod:
             if mod:
                 self.status[idx] = "".join(sorted("M" + self.status[idx]))
             else:
                 self.status[idx] = self.status[idx].replace("M", "")
             statidx = self.index(index.row(), self.statcol)
             self.dataChanged.emit(statidx, statidx)
-    
+
     def haveNewName(self, idx, name):
         name = str(name)
         utils.fixName(param.params.pobj.cfgs.values(), idx, name)
         utils.fixName(self.cfgs.values(), idx, name)
         utils.fixName(self.edits.values(), idx, name)
         for r in range(len(self.path)):
             i = self.path[r]
             try:
-                if self.edits[i]['config'] == idx:
+                if self.edits[i]["config"] == idx:
                     index = self.index(r, self.cfgcol)
                     self.dataChanged.emit(index, index)
-            except:
+            except Exception:
                 if i >= 0:
                     d = param.params.pobj.cfgs[i]
                 else:
                     d = self.cfgs[i]
-                if d['config'] == idx:
+                if d["config"] == idx:
                     index = self.index(r, self.cfgcol)
                     self.dataChanged.emit(index, index)
-        for (id, d) in self.tree.items():
+        for id, d in self.tree.items():
             if id == idx:
-                d['name'] = name
-                d['item'].setText(0, name)
+                d["name"] = name
+                d["item"].setText(0, name)
 
     def buildtree(self):
         t = {}
         for d in param.params.pobj.cfgs.values():
-            idx = d['id']
-            t[idx] = {'name': d['name'], 'link': d['config'], 'children' : []}
+            idx = d["id"]
+            t[idx] = {"name": d["name"], "link": d["config"], "children": []}
             try:
-                t[idx]['link'] = self.edits[idx]['config']
-            except:
+                t[idx]["link"] = self.edits[idx]["config"]
+            except Exception:
                 pass
         for d in self.cfgs.values():
-            idx = d['id']
-            t[idx] = {'name': d['name'], 'link': d['config'], 'children' : []}
+            idx = d["id"]
+            t[idx] = {"name": d["name"], "link": d["config"], "children": []}
         r = []
-        for (k, v) in t.items():
-            l = v['link']
-            if l == None:
+        for k, v in t.items():
+            l = v["link"]
+            if l is None:
                 r.append(k)
             else:
-                t[l]['children'].append(k)
+                t[l]["children"].append(k)
         #
         # Sigh.  Since other users can be changing configs out from under us,
         # we might inadvertently end up with loops.  We'll take care of this
         # before we commit, but for now, we need to make sure everything is
         # reachable.
         #
         d = list(r)
-        for id in d:                         # This loop builds all of the rooted trees.
-            d[len(d):] = t[id]['children']
-        for (k, v) in t.items():
+        for id in d:  # This loop builds all of the rooted trees.
+            d[len(d) :] = t[id]["children"]
+        for k, v in t.items():
             if k in d:
                 continue
-            r.append(k)                      # If this isn't in a rooted tree, it must be in a loop!
+            r.append(k)  # If this isn't in a rooted tree, it must be in a loop!
             d.append(k)
-            l = v['link']
+            l = v["link"]
             while l != k:
                 d.append(l)
-                l = t[l]['link']
-        r.sort(key=lambda v: t[v]['name'])
+                l = t[l]["link"]
+        r.sort(key=lambda v: t[v]["name"])
         for d in t.values():
-            d['children'].sort(key=lambda v: t[v]['name'])
+            d["children"].sort(key=lambda v: t[v]["name"])
         self.root = r
         self.tree = t
-        self.setupTree(param.params.ui.treeWidget, 'item')
+        self.setupTree(param.params.ui.treeWidget, "item")
 
     def setupTree(self, tree, fld):
         tree.clear()
         r = list(self.root)  # Make a copy!
         t = self.tree
         d = []
         hutch = param.params.pobj.hutch.upper()
@@ -201,99 +196,107 @@
                 continue
             d.append(id)
             if id in self.root:
                 item = QtWidgets.QTreeWidgetItem(tree)
                 parent = None
             else:
                 item = QtWidgets.QTreeWidgetItem()
-                parent = t[id]['link']
+                parent = t[id]["link"]
             item.id = id
-            item.setText(0, t[id]['name'])
-            if t[id]['name'] == hutch:
+            item.setText(0, t[id]["name"])
+            if t[id]["name"] == hutch:
                 self.hutchid = id
             t[id][fld] = item
-            if parent != None:
+            if parent is not None:
                 t[parent][fld].addChild(item)
             try:
                 # Everything defaults to collapsed!
                 if self.is_expanded[id]:
                     tree.expandItem(item)
-            except:
+            except Exception:
                 self.is_expanded[id] = False
-            r[len(r):] = t[id]['children']
+            r[len(r) :] = t[id]["children"]
         return t
 
     def index2db(self, index):
         r = index.row()
         c = index.column()
         idx = self.path[r]
         if c < self.coff:
             f = self.cfld[c]
         else:
-            f = param.params.pobj.cfgflds[c-self.coff]['fld']
+            f = param.params.pobj.cfgflds[c - self.coff]["fld"]
         return (idx, f)
 
     def db2index(self, idx, f):
         try:
-            c = param.params.pobj.fldmap[f]['cfgidx'] + self.coff
+            c = param.params.pobj.fldmap[f]["cfgidx"] + self.coff
             r = self.path.index(idx)
             return self.index(r, c)
-        except:
+        except Exception:
             return None
 
     def getCfg(self, idx):
         """
         Get the configuration dictionary for this index.
 
-        Negative indices have not been committed yet and are locally 
+        Negative indices have not been committed yet and are locally
         stored in self.cfgs.  Positive indices are in the database and
         are kept in the pmgrobj.
 
         This routine also creates a "_color" dictionary that gives the
         modification status of each field.
         """
-        if idx == None:
+        if idx is None:
             return {}
         if idx >= 0:
             d = param.params.pobj.cfgs[idx]
         else:
             d = self.cfgs[idx]
         try:
             e = self.edits[idx].keys()
-        except:
+        except Exception:
             e = []
-        if not '_color' in d.keys():
+        if "_color" not in d.keys():
             color = {}
             try:
-                v = self.edits[idx]['mutex']
-            except:
-                v = d['mutex']
-            d['curmutex'] = v
-            for (k, v) in d.items():
-                if k[:3] != 'PV_' and k[:4] != 'FLD_' and not k in self.cfld:
+                v = self.edits[idx]["mutex"]
+            except Exception:
+                v = d["mutex"]
+            d["curmutex"] = v
+            for k, v in d.items():
+                if k[:3] != "PV_" and k[:4] != "FLD_" and k not in self.cfld:
                     continue
-                if v == None and chr(param.params.pobj.fldmap[k]['colorder']+0x40) in d['curmutex']:
+                if (
+                    v is None
+                    and chr(param.params.pobj.fldmap[k]["colorder"] + 0x40)
+                    in d["curmutex"]
+                ):
                     color[k] = param.params.almond
                 elif k in e:
                     color[k] = param.params.red
                 else:
                     color[k] = param.params.black
-            d['_color'] = color
+            d["_color"] = color
         return d
 
     def getval(self, idx, f):
         try:
             return self.edits[idx][f]
-        except:
+        except Exception:
             return self.getCfg(idx)[f]
 
-    def data(self, index, role = QtCore.Qt.DisplayRole):
-        if (role != QtCore.Qt.DisplayRole and role != QtCore.Qt.EditRole and
-            role != QtCore.Qt.ForegroundRole and role != QtCore.Qt.BackgroundRole and
-            role != QtCore.Qt.ToolTipRole):
+    def data(self, index, role=QtCore.Qt.DisplayRole):
+        if (
+            role != QtCore.Qt.DisplayRole
+            and role != QtCore.Qt.EditRole
+            and role != QtCore.Qt.ForegroundRole
+            and role != QtCore.Qt.BackgroundRole
+            and role != QtCore.Qt.ToolTipRole
+        ):
             return QtGui.QStandardItemModel.data(self, index, role)
         if not index.isValid():
             return None
         (idx, f) = self.index2db(index)
         if role == QtCore.Qt.ToolTipRole:
             # We'll make this smarter later!
             return QtGui.QStandardItemModel.data(self, index, role)
@@ -302,90 +305,90 @@
                 return param.params.white
             elif role == QtCore.Qt.ForegroundRole:
                 return param.params.black
             else:
                 return self.status[idx]
         d = self.getCfg(idx)
         if role == QtCore.Qt.ForegroundRole:
-            color = d['_color'][f]
+            color = d["_color"][f]
             return color
         elif role == QtCore.Qt.BackgroundRole:
             if f in self.cfld:
                 return param.params.white
-            if chr(param.params.pobj.fldmap[f]['colorder']+0x40) in d['curmutex']:
+            if chr(param.params.pobj.fldmap[f]["colorder"] + 0x40) in d["curmutex"]:
                 return param.params.almond
             else:
                 return param.params.white
         else:
             try:
                 v = self.edits[idx][f]
-            except:
+            except Exception:
                 v = d[f]
             return v
-        
+
     def setData(self, index, v, role=QtCore.Qt.EditRole):
         if role != QtCore.Qt.DisplayRole and role != QtCore.Qt.EditRole:
-            return QtGui.QStandardItemModel.setData(self, index, value, role)
+            return super().setData(index, v, role)
         (idx, f) = self.index2db(index)
         # Get all the edits for this config.
         try:
             e = self.edits[idx]
-        except:
+        except Exception:
             e = {}
         # OK, the config/cfgname thing is slightly weird.  The field name for our index is
         # 'cfgname', but we are passing an int that should go to 'config'.  So we need to
         # change *both*!  More than that, it's possible that the configuration name has been
         # edited!
-        if f == 'cfgname':
+        if f == "cfgname":
             vlink = v
             v = param.params.db.getCfgName(vlink)
         # Remove the old edit of this field, if any.
         try:
             del e[f]
-            if f == 'cfgname':
-                del e['config']
-        except:
+            if f == "cfgname":
+                del e["config"]
+        except Exception:
             pass
         # Get the configured values.
         d = self.getCfg(idx)
         if not param.equal(v, d[f]):
             # If we have a change, set it as an edit.
             chg = True
             e[f] = v
-            if f == 'cfgname':
-                e['config'] = vlink
+            if f == "cfgname":
+                e["config"] = vlink
         else:
             chg = False
             # No change?
         # Save the edits for this id!
         if e != {}:
             if idx < 0:
                 self.cfgs[idx].update(e)
             else:
                 self.edits[idx] = e
         else:
             try:
                 del self.edits[idx]
-            except:
+            except Exception:
                 pass
         self.setModifiedStatus(index, idx, d)
         # Set our color.
         if chg and idx >= 0:
             # Only mark changes to *existing* configurations in red!
-            d['_color'][f] = param.params.red
+            d["_color"][f] = param.params.red
         else:
-            d['_color'][f] = param.params.black
+            d["_color"][f] = param.params.black
         c = index.column()
         try:
-            cm = chr(param.params.pobj.fldmap[f]['colorder']+0x40)
-            if cm in d['curmutex']:
+            cm = chr(param.params.pobj.fldmap[f]["colorder"] + 0x40)
+            if cm in d["curmutex"]:
                 # This was a calculated value!
-                i = d['curmutex'].find(cm)
-                d['curmutex'] = self.promote(idx, f, i, d['curmutex'])
-        except:
+                i = d["curmutex"].find(cm)
+                d["curmutex"] = self.promote(idx, f, i, d["curmutex"])
+        except Exception:
             pass
         self.dataChanged.emit(index, index)
         if c == self.namecol:
             param.params.db.setCfgName(idx, v)
             self.newname.emit(idx, v)
         else:
             self.cfgChanged.emit(idx, f)
@@ -405,193 +408,205 @@
             else:
                 derived = mlist[0]
         else:
             d = param.params.deriveddialog
             d.reset()
             for fld in mlist:
                 if fld != f:
-                    d.addValue(param.params.pobj.fldmap[fld]['alias'], fld)
+                    d.addValue(param.params.pobj.fldmap[fld]["alias"], fld)
             d.exec_()
             # The user *must* give a value.  I'll take whatever is checked even if the
             # window was just closed!!
             derived = d.getValue()
         for fld in mlist:
             if fld == derived:
                 # The derived value must be None!
-                if cfg[fld] == None:
+                if cfg[fld] is None:
                     try:
                         del self.edits[idx][fld]
                         if self.edits[idx] == {}:
                             del self.edits[idx]
-                    except:
+                    except Exception:
                         pass
                 else:
                     try:
                         self.edits[idx][fld] = None
-                    except:
+                    except Exception:
                         self.edits[idx] = {fld: None}
-        cm = chr(param.params.pobj.fldmap[derived]['colorder']+0x40)
-        curmutex = curmutex[:setidx] + cm + curmutex[setidx+1:]
+        cm = chr(param.params.pobj.fldmap[derived]["colorder"] + 0x40)
+        curmutex = curmutex[:setidx] + cm + curmutex[setidx + 1 :]
         try:
-            e = self.edits[idx]['mutex']
-        except:
-            e = cfg['mutex']
-        e = e[:setidx] + cm + e[setidx+1:]
-        try:
-            self.edits[idx]['mutex'] = e
-        except:
-            self.edits[idx] = {'mutex': e}
+            e = self.edits[idx]["mutex"]
+        except Exception:
+            e = cfg["mutex"]
+        e = e[:setidx] + cm + e[setidx + 1 :]
+        try:
+            self.edits[idx]["mutex"] = e
+        except Exception:
+            self.edits[idx] = {"mutex": e}
         return curmutex
-        
+
     def setCurIdx(self, id):
         self.curidx = id
         self.layoutAboutToBeChanged.emit()
         idx = id
-        path = [idx];
-        while self.tree[idx]['link'] != None:
-            idx = self.tree[idx]['link']
+        path = [idx]
+        while self.tree[idx]["link"] is not None:
+            idx = self.tree[idx]["link"]
             if idx == self.curidx:
                 break
             path[:0] = [idx]
-        for c in self.tree[id]['children']:
-            if not c in path:
+        for c in self.tree[id]["children"]:
+            if c not in path:
                 path.append(c)
         self.path = path
         self.setRowCount(len(path))
         self.layoutChanged.emit()
 
     def selectConfig(self, cfg):
-        param.params.ui.treeWidget.setCurrentItem(self.tree[cfg]['item'])
-        
+        param.params.ui.treeWidget.setCurrentItem(self.tree[cfg]["item"])
+
     def treeNavigation(self, cur, prev):
-        if cur != None:
+        if cur is not None:
             self.setCurIdx(cur.id)
 
     def treeCollapse(self, item):
-        if item != None:
+        if item is not None:
             self.is_expanded[item.id] = False
 
     def treeExpand(self, item):
-        if item != None:
+        if item is not None:
             self.is_expanded[item.id] = True
 
     def checkStatus(self, index, vals):
         (idx, f) = self.index2db(index)
         s = self.status[idx]
         for v in vals:
             if v in s:
                 return True
         return False
 
     def setupContextMenus(self, table):
         menu = utils.MyContextMenu()
         menu.addAction("Create new child", self.createnew)
         menu.addAction("Clone existing", self.clone)
-        menu.addAction("Change parent", self.chparent,
-                       lambda t, i: i.column() == self.cfgcol)
-        menu.addAction("Delete config", self.deletecfg,
-                       lambda t, i: not self.checkStatus(i, 'D'))
-        menu.addAction("Undelete config", self.undeletecfg,
-                       lambda t, i: self.checkStatus(i, 'D'))
-        menu.addAction("Commit this config", self.commitone,
-                       lambda t, i: self.checkStatus(i, 'DMN'))
-        menu.addAction("Revert this config", self.revertone,
-                       lambda t, i: self.checkStatus(i, 'M'))
+        menu.addAction(
+            "Change parent", self.chparent, lambda t, i: i.column() == self.cfgcol
+        )
+        menu.addAction(
+            "Delete config", self.deletecfg, lambda t, i: not self.checkStatus(i, "D")
+        )
+        menu.addAction(
+            "Undelete config", self.undeletecfg, lambda t, i: self.checkStatus(i, "D")
+        )
+        menu.addAction(
+            "Commit this config",
+            self.commitone,
+            lambda t, i: self.checkStatus(i, "DMN"),
+        )
+        menu.addAction(
+            "Revert this config", self.revertone, lambda t, i: self.checkStatus(i, "M")
+        )
         table.addContextMenu(menu)
         colmgr.addColumnManagerMenu(table)
 
     #
     # How is this called?
     #     - Parent is the parent configuration idx.
     #     - Sibling is the sibling configuration dictionary.
     #     - diff is True if we are actually using an object dictionary.
     # So three ways to use this:
     #     - Create configuration from object
     #     - Create new child
     #     - Clone existing
     #
     def create_child(self, parent, sibling, diff=False):
-        id = self.nextid;
+        id = self.nextid
         self.nextid -= 1
         now = datetime.datetime.now()
-        d = {'name': "NewConfig%d" % id, 'config': parent,
-             'cfgname': param.params.db.getCfgName(parent), 'id': id, 
-             'dt_created': now, 'dt_updated': now}
+        d = {
+            "name": "NewConfig%d" % id,
+            "config": parent,
+            "cfgname": param.params.db.getCfgName(parent),
+            "id": id,
+            "dt_created": now,
+            "dt_updated": now,
+        }
         self.status[id] = "N"
-        param.params.db.setCfgName(id, d['name'])
+        param.params.db.setCfgName(id, d["name"])
         color = {}
         for f in param.params.pobj.cfgflds:
-            fld = f['fld']
+            fld = f["fld"]
             d[fld] = sibling[fld]
             color[fld] = param.params.black
         for fld in self.cfld:
             color[fld] = param.params.black
-        d['_color'] = color
+        d["_color"] = color
         if diff:
             # Sigh.  The sibling is from the object model, which means that the
             # the mutex field has the 'wrong' values set.  What we *really* want
             # is the mutex field of the object's config!
-            d['curmutex'] = self.getCfg(sibling['config'])['curmutex']
-            d['mutex'] = d['curmutex']
+            d["curmutex"] = self.getCfg(sibling["config"])["curmutex"]
+            d["mutex"] = d["curmutex"]
         else:
-            d['curmutex'] = sibling['curmutex']
-            d['mutex'] = sibling['mutex']
+            d["curmutex"] = sibling["curmutex"]
+            d["mutex"] = sibling["mutex"]
         # Make sure this respects the mutex! MCB
-        for c in d['curmutex']:
+        for c in d["curmutex"]:
             v = ord(c) - 0x40
             if v > 0:
-                d[param.params.pobj.objflds[v-1]['fld']] = None
+                d[param.params.pobj.objflds[v - 1]["fld"]] = None
         self.cfgs[id] = d
         self.buildtree()
         try:
-            param.params.ui.treeWidget.setCurrentItem(self.tree[id]['item'])
-        except:
+            param.params.ui.treeWidget.setCurrentItem(self.tree[id]["item"])
+        except Exception:
             pass
         return id
 
     def createnew(self, table, index):
         (idx, f) = self.index2db(index)
-        id = self.create_child(idx, self.getCfg(idx))
+        self.create_child(idx, self.getCfg(idx))
 
     def clone(self, table, index):
         (idx, f) = self.index2db(index)
-        parent = self.getCfg(idx)['config']
-        id = self.create_child(parent, self.getCfg(idx))
+        parent = self.getCfg(idx)["config"]
+        self.create_child(parent, self.getCfg(idx))
 
     def hasChildren(self, idx, checked=[]):
-        for c in self.tree[idx]['children']:
-            if not 'D' in self.status[c]:
+        for c in self.tree[idx]["children"]:
+            if "D" not in self.status[c]:
                 return True
         # Sigh.  We might have a circular dependency.
         newchecked = list(checked)
-        newchecked[:0] = self.tree[idx]['children']
-        for c in self.tree[idx]['children']:
-            if not c in checked:
+        newchecked[:0] = self.tree[idx]["children"]
+        for c in self.tree[idx]["children"]:
+            if c not in checked:
                 if self.hasChildren(c, newchecked):
                     return True
         return False
 
     def checkSetMutex(self, d, e):
         for s in param.params.pobj.setflds:
             f = param.params.pobj.fldmap[s[0]]
-            if not f['setmutex'] or f['obj']:
+            if not f["setmutex"] or f["obj"]:
                 continue
             try:
-                z = f['enum'][0]
-            except:
+                z = f["enum"][0]
+            except Exception:
                 z = 0
             vlist = []
             for f in s:
                 try:
                     v = e[f]
-                except:
+                except Exception:
                     v = d[f]
-                if v != None and not param.equal(v, z):
+                if v is not None and not param.equal(v, z):
                     if v in vlist:
-                        return [param.params.pobj.fldmap[f]['alias'] for f in s]
+                        return [param.params.pobj.fldmap[f]["alias"] for f in s]
                     else:
                         vlist.append(v)
         return []
 
     #
     # Try to commit a change.  We assume we are in a transaction already.
     #
@@ -599,131 +614,151 @@
     # else first.
     #
     # If mustdo is True, cause an error if we can't do it.
     #
     def commit(self, idx, mustdo):
         d = self.getCfg(idx)
         try:
-            name = self.edits[idx]['name']
-        except:
-            name = d['name']
+            name = self.edits[idx]["name"]
+        except Exception:
+            name = d["name"]
         if not utils.permission():
             param.params.pobj.transaction_error("Not Authorized to Change %s!" % name)
             return True
         if name[0:10] == "NewConfig-":
             param.params.pobj.transaction_error("Object cannot be named %s!" % name)
             return True
-        if 'D' in self.status[idx]:
+        if "D" in self.status[idx]:
             # We can process the delete only if *no one* is using this!
             if mustdo:
-                if self.tree[idx]['children'] != []:
-                    param.params.pobj.transaction_error("Configuration to be deleted has children!")
+                if self.tree[idx]["children"] != []:
+                    param.params.pobj.transaction_error(
+                        "Configuration to be deleted has children!"
+                    )
                 elif param.params.objmodel.configInUse(idx):
-                    param.params.pobj.transaction_error("Object still using configuration to be deleted!")
+                    param.params.pobj.transaction_error(
+                        "Object still using configuration to be deleted!"
+                    )
                 else:
                     param.params.pobj.configDelete(idx)
             else:
                 if self.hasChildren(idx):
-                    param.params.pobj.transaction_error("Configuration to be deleted has children!")
+                    param.params.pobj.transaction_error(
+                        "Configuration to be deleted has children!"
+                    )
                 elif param.params.objmodel.configInUse(idx):
-                    param.params.pobj.transaction_error("Object still using configuration to be deleted!")
+                    param.params.pobj.transaction_error(
+                        "Object still using configuration to be deleted!"
+                    )
                 else:
                     param.params.pobj.configDelete(idx)
             return True
         else:
             # When is it OK to commit this?  If:
             #    - All the parents already exist.
             #    - We don't make a circular loop.
             #    - Any setmutex sets are OK. (All inherited or all different.)
             #    - Every nullok field, is non-null.
             #    - Every unique field has a value (we'll let mysql actually deal with uniqueness!)
             try:
                 e = self.edits[idx]
-            except:
+            except Exception:
                 e = {}
             s = self.checkSetMutex(d, e)
             if s != []:
-                param.params.pobj.transaction_error("Config %s does not have unique values for %s!" %
-                                                  (name, str(s)))
+                param.params.pobj.transaction_error(
+                    "Config %s does not have unique values for %s!" % (name, str(s))
+                )
                 return True
             for f in param.params.pobj.cfgflds:
-                if not f['nullok'] and d[f['fld']] == "":
-                    param.params.pobj.transaction_error("Field %s cannot be NULL!" % f['fld'])
+                if not f["nullok"] and d[f["fld"]] == "":
+                    param.params.pobj.transaction_error(
+                        "Field %s cannot be NULL!" % f["fld"]
+                    )
                     return True
             try:
-                p = self.edits[idx]['config']
-            except:
-                p = d['config']
-            while p != None:
+                p = self.edits[idx]["config"]
+            except Exception:
+                p = d["config"]
+            while p is not None:
                 if not param.params.db.cfgIsValid(p):
                     if mustdo:
-                        param.params.pobj.transaction_error("Config %s has new uncommitted ancestors!" %
-                                                          param.params.db.getCfgName(idx))
+                        param.params.pobj.transaction_error(
+                            "Config %s has new uncommitted ancestors!"
+                            % param.params.db.getCfgName(idx)
+                        )
                         return True
                     else:
                         return False
                 # If we are only committing one, we need to check the actual parents,
                 # otherwise, we check the edited parents!
                 if mustdo:
-                    p = self.getCfg(p)['config']
+                    p = self.getCfg(p)["config"]
                 else:
                     try:
-                        p = self.edits[p]['config']
-                    except:
-                        p = self.getCfg(p)['config']
+                        p = self.edits[p]["config"]
+                    except Exception:
+                        p = self.getCfg(p)["config"]
                 if p == idx:
-                    return param.params.pobj.transaction_error("Config change for %s creates a dependency loop!" %
-                                                             param.params.db.getCfgName(idx))
+                    return param.params.pobj.transaction_error(
+                        "Config change for %s creates a dependency loop!"
+                        % param.params.db.getCfgName(idx)
+                    )
                     return True
-            if 'N' in self.status[idx]:
+            if "N" in self.status[idx]:
                 newid = param.params.pobj.configInsert(param.params.db.doMap(d))
-                if newid != None:
+                if newid is not None:
                     param.params.db.addCfgmap(idx, newid)
             else:
                 ee = {}
-                for fld in ['name', 'config', 'mutex']:
+                for fld in ["name", "config", "mutex"]:
                     try:
                         ee[fld] = e[fld]
-                    except:
+                    except Exception:
                         pass
                 for f in param.params.pobj.cfgflds:
-                    fld = f['fld']
+                    fld = f["fld"]
                     try:
-                        ee[fld] = e[fld]           # We have a new value!
-                    except:
+                        ee[fld] = e[fld]  # We have a new value!
+                    except Exception:
                         try:
                             if not self.editval[idx][fld]:  # We want to inherit now!
                                 ee[fld] = None
-                            else:                  # The new value is what we are already inheriting!
+                            else:  # The new value is what we are already inheriting!
                                 ee[fld] = d[fld]
-                        except:
-                            pass                   # No change!
+                        except Exception:
+                            pass  # No change!
                 param.params.pobj.configChange(idx, param.params.db.doMap(ee))
             return True
 
     # Commit all of the changes.  Again, we assume we're in a transaction
     # already.
     def commitall(self, verify=True):
         try:
-            todo = todo.union(set(self.edits.keys()))
-        except:
-            todo = set([])
+            todo = set(self.edits.keys())
+        except Exception:
+            todo = set()
+
         # We only need to confirm the changes.  We forbid the deletion of a used config!
         if verify and not self.confirmCommit(list(todo)):
             return
         todo = todo.union(set(self.cfgs.keys()))
-        todo = todo.union(set([idx for idx in self.status.keys() if 'D' in self.status[idx]]))
-        while todo != set([]):
-            done = set([])
+        todo = todo.union(
+            {idx for idx in self.status.keys() if "D" in self.status[idx]}
+        )
+        while todo != set():
+            done = set()
             for idx in todo:
                 if self.commit(idx, False):
-                    done = done.union(set([idx]))
+                    done = done.union({idx})
             todo = todo.difference(done)
-            if done == set([]):
-                param.params.pobj.transaction_error("Configuration commit is not making progress!")
+            if done == set():
+                param.params.pobj.transaction_error(
+                    "Configuration commit is not making progress!"
+                )
                 return
 
     def commitone(self, table, index):
         (idx, f) = self.index2db(index)
         if not self.confirmCommit([idx]):
             return
         param.params.db.start_transaction()
@@ -732,110 +767,128 @@
             self.cfgChangeDone(idx)
 
     def revertall(self):
         self.layoutAboutToBeChanged.emit()
         for idx in self.edits.keys():
             self.revertone(None, idx, True)
         self.layoutChanged.emit()
-        
+
     def revertone(self, table, index, doall=False):
         if doall:
             idx = index
         else:
             (idx, f) = self.index2db(index)
         try:
-            newparent = self.edits[idx]['config']
-        except:
+            newparent = self.edits[idx]["config"]
+        except Exception:
             newparent = None
         try:
             del self.edits[idx]
-        except:
+        except Exception:
             pass
         c = self.getCfg(idx)
-        del c['_color']
+        del c["_color"]
         c = self.getCfg(idx)
         self.status[idx] = self.status[idx].replace("M", "")
-        if newparent != None:
+        if newparent is not None:
             self.buildtree()
             self.setCurIdx(self.curidx)
         elif not doall:
             r = index.row()
             self.dataChanged.emit(self.index(r, 0), self.index(r, self.colcnt - 1))
-        
+
     def cfgChangeDone(self, idx=None):
-        if idx != None:
+        if idx is not None:
             try:
                 del self.edits[idx]
-            except:
+            except Exception:
                 pass
             self.status[idx] = ""
             if idx < 0:
                 del self.cfgs[idx]
         else:
             self.edits = {}
             self.cfgs = {}
             snew = {}
             for k in self.status.keys():
                 if k >= 0:
                     snew[k] = ""
             self.status = snew
         self.buildtree()
         try:
-            param.params.ui.treeWidget.setCurrentItem(self.tree[self.curidx]['item'])
-        except:
-            param.params.ui.treeWidget.setCurrentItem(self.tree[0]['item'])
+            param.params.ui.treeWidget.setCurrentItem(self.tree[self.curidx]["item"])
+        except Exception:
+            param.params.ui.treeWidget.setCurrentItem(self.tree[0]["item"])
 
     def deletecfg(self, table, index):
         (idx, f) = self.index2db(index)
         if idx >= 0:
             d = self.getCfg(idx)
-            if d['config'] != None:
+            if d["config"] is not None:
                 self.status[idx] = "".join(sorted("D" + self.status[idx]))
                 statidx = self.index(index.row(), self.statcol)
                 self.dataChanged.emit(statidx, statidx)
             else:
-                QtWidgets.QMessageBox.critical(None, "Error",
-                                           "Cannot delete root configuration!",
-                                           QtWidgets.QMessageBox.Ok)
+                QtWidgets.QMessageBox.critical(
+                    None,
+                    "Error",
+                    "Cannot delete root configuration!",
+                    QtWidgets.QMessageBox.Ok,
+                )
         elif param.params.objmodel.configInUse(idx):
-            QtWidgets.QMessageBox.critical(None, "Error",
-                                           "Cannot delete configuration still in use!",
-                                           QtWidgets.QMessageBox.Ok)
+            QtWidgets.QMessageBox.critical(
+                None,
+                "Error",
+                "Cannot delete configuration still in use!",
+                QtWidgets.QMessageBox.Ok,
+            )
         else:
             del self.cfgs[idx]
             del self.status[idx]
             self.buildtree()
             try:
-                param.params.ui.treeWidget.setCurrentItem(self.tree[self.curidx]['item'])
-            except:
-                param.params.ui.treeWidget.setCurrentItem(self.tree[0]['item'])
+                param.params.ui.treeWidget.setCurrentItem(
+                    self.tree[self.curidx]["item"]
+                )
+            except Exception:
+                param.params.ui.treeWidget.setCurrentItem(self.tree[0]["item"])
 
     def undeletecfg(self, table, index):
         (idx, f) = self.index2db(index)
-        d = self.getCfg(idx)
+        self.getCfg(idx)
         self.status[idx] = self.status[idx].replace("D", "")
         statidx = self.index(index.row(), self.statcol)
         self.dataChanged.emit(statidx, statidx)
 
     def chparent(self, table, index):
         (idx, f) = self.index2db(index)
         d = self.getCfg(idx)
-        if d['config'] == None:
-            QtWidgets.QMessageBox.critical(None, "Error",
-                                       "Cannot change parent of root class!",
-                                       QtWidgets.QMessageBox.Ok)
+        if d["config"] is None:
+            QtWidgets.QMessageBox.critical(
+                None,
+                "Error",
+                "Cannot change parent of root class!",
+                QtWidgets.QMessageBox.Ok,
+            )
             return
-        if (param.params.cfgdialog.exec_("Select new parent for %s" % d['name'], d['config']) ==
-            QtWidgets.QDialog.Accepted):
+        if (
+            param.params.cfgdialog.exec_(
+                "Select new parent for %s" % d["name"], d["config"]
+            )
+            == QtWidgets.QDialog.Accepted
+        ):
             (idx, f) = self.index2db(index)
             p = param.params.cfgdialog.result
-            if p == d['id']:
-                QtWidgets.QMessageBox.critical(None, "Error",
-                                           "Cannot change parent to self!",
-                                           QtWidgets.QMessageBox.Ok)
+            if p == d["id"]:
+                QtWidgets.QMessageBox.critical(
+                    None,
+                    "Error",
+                    "Cannot change parent to self!",
+                    QtWidgets.QMessageBox.Ok,
+                )
                 return
             self.setData(index, param.params.cfgdialog.result)
             self.buildtree()
             self.setCurIdx(idx)
 
     # Enabled:
     #     Everything.
@@ -845,22 +898,20 @@
     #     QtCore.Qt.ItemIsEditable
     # Drag/Drop:
     #     QtCore.Qt.ItemIsDragEnabled | QtCore.Qt.ItemIsDropEnabled
     #
     def flags(self, index):
         flags = QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsSelectable
         if index.isValid():
-            row = index.row()
             col = index.column()
-            idx = self.path[row]
             try:
-                if (col != self.cfgcol and col != self.statcol):
+                if col != self.cfgcol and col != self.statcol:
                     flags = flags | QtCore.Qt.ItemIsEditable
-            except:
-                pass # We seem to get here too fast sometimes after a delete, so just forget it.
+            except Exception:
+                pass  # We seem to get here too fast sometimes after a delete, so just forget it.
         return flags
 
     #
     # Return the set of changed configurations.
     #
     # idx is the config we are currently looking at.
     # e is a list of values that have edits in this configuration.
@@ -873,85 +924,88 @@
     def findChange(self, idx, e, s, l):
         if idx in s:
             return s
         s.add(idx)
         return s
 
     def confirmCommit(self, l=None):
-        if l == None:
+        if l is None:
             try:
-                todo = todo.union(set(self.edits.keys()))
-            except:
-                todo = ([])
-            l = list(todo)
+                l = list(set(self.edits.keys()))
+            except Exception:
+                l = []
+
         chg = {}
-        chgall = set([])
+        chgall = set()
         for idx in l:
             try:
                 e = self.edits[idx].keys()
-                chg[idx] = self.findChange(idx, e, set([]), l)
-            except:
+                chg[idx] = self.findChange(idx, e, set(), l)
+            except Exception:
                 # No changed values --> no child changes!
-                chg[idx] = set([idx])
+                chg[idx] = {idx}
             chgall = chgall.union(chg[idx])
         nc = len(chgall)
         no = param.params.pobj.countInstance(chgall)
         d = param.params.confirmdialog
         if nc == 0 and no == 0:
             return True
-        d.ui.label.setText("This commit will affect %d configurations and %d motors." %
-                           (nc, no))
+        d.ui.label.setText(
+            "This commit will affect %d configurations and %d motors." % (nc, no)
+        )
         return d.exec_() == QtWidgets.QDialog.Accepted
 
     def editorInfo(self, index):
         c = index.column()
         if c < self.coff:
             return str
         try:
-            return param.params.pobj.cfgflds[c - self.coff]['enum']
-        except:
-            return param.params.pobj.cfgflds[c - self.coff]['type']
+            return param.params.pobj.cfgflds[c - self.coff]["enum"]
+        except Exception:
+            return param.params.pobj.cfgflds[c - self.coff]["type"]
 
     def cfgrenumber(self, old, new):
         for d in self.edits.values():
             try:
-                if d['config'] == old:
-                    d['config'] = new
-            except:
+                if d["config"] == old:
+                    d["config"] = new
+            except Exception:
                 pass
         for d in self.cfgs.values():
-            if d['config'] == old:
-                d['config'] = new
+            if d["config"] == old:
+                d["config"] = new
         if old in self.tree.keys():
             self.tree[new] = self.tree[old]
             del self.tree[old]
         for d in self.tree.values():
-            if d['link'] == old:
-                d['link'] = new
+            if d["link"] == old:
+                d["link"] = new
             try:
-                d['children'][d['children'].index(old)] = new
-            except:
+                d["children"][d["children"].index(old)] = new
+            except Exception:
                 pass
+
         try:
-            self.root[index(self.root, old)] = new
-        except:
+            self.root[self.root.index(old)] = new
+        except Exception:
             pass
+
         if old == self.curidx:
             self.setCurIdx(new)
 
     def modifycfgfromobj(self, obj):
-        idx = obj['config']
+        idx = obj["config"]
         cfg = self.getCfg(idx)
-        if obj['config'] not in self.path:
+        if obj["config"] not in self.path:
             self.setCurIdx(idx)
         r = self.path.index(idx)
         for c in range(self.coff, self.colcnt):
-            f = param.params.pobj.cfgflds[c-self.coff]['fld']
-            o = param.params.pobj.cfgflds[c-self.coff]['colorder']
-            cc = chr(o+0x40)
-            if cc in self.mutex_flds and cc not in cfg['curmutex']:
+            f = param.params.pobj.cfgflds[c - self.coff]["fld"]
+            o = param.params.pobj.cfgflds[c - self.coff]["colorder"]
+            cc = chr(o + 0x40)
+            if cc in self.mutex_flds and cc not in cfg["curmutex"]:
                 continue
             try:
                 if obj[f] != cfg[f]:
                     self.setData(self.index(r, c), obj[f])
-            except:
+            except Exception:
                 pass
```

### Comparing `pmgr-2.0.2/pmgr/FreezeTableView.py` & `pmgr-2.1.3/pmgr/FreezeTableView.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt5 import QtCore, QtWidgets
 
 ######################################################################
 
+
 class FreezeHeaderView(QtWidgets.QHeaderView):
     def __init__(self, orientation, parent=None):
         QtWidgets.QHeaderView.__init__(self, orientation, parent)
         self.__hdr = None
         self.__parent = parent
         self.__orientation = orientation
         self.sortindicator = (None, None)
         self.sectionResized.connect(self.updateSectionWidth)
         self.sortIndicatorChanged.connect(self.selfSortChanged)
-        #MCB self.setClickable(True)  # Sigh.  Why isn't this done when we ask it to be sortable?!?
+        # MCB self.setClickable(True)  # Sigh.  Why isn't this done when we ask it to be sortable?!?
 
     def setShadowHeader(self, hdr):
         self.__hdr = hdr
         self.__hdr.sortIndicatorChanged.connect(self.parentSortChanged)
 
     def sectionSizeFromContents(self, logidx):
-        if self.__hdr == None:
+        if self.__hdr is None:
             return QtWidgets.QHeaderView.sectionSizeFromContents(self, logidx)
         elif self.__orientation == QtCore.Qt.Horizontal:
             return QtCore.QSize(self.__hdr.sectionSize(logidx), self.__hdr.height())
         else:
             return QtCore.QSize(self.__hdr.width(), self.__hdr.sectionSize(logidx))
 
     def updateSectionWidth(self, logidx, oldsize, newsize):
@@ -35,16 +36,18 @@
             self.__hdr.setSortIndicator(logidx, order)
 
     def parentSortChanged(self, logidx, order):
         if (logidx, order) != self.sortindicator:
             self.sortindicator = (logidx, order)
             self.setSortIndicator(logidx, order)
 
+
 ######################################################################
 
+
 class DropTableView(QtWidgets.QTableView):
     def __init__(self, parent, rows, cols, name):
         QtWidgets.QTableView.__init__(self, parent)
         self.hiderows = rows
         self.hidecols = cols
         self.debugname = name
         self.menus = []
@@ -55,17 +58,19 @@
         self.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
         self.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.horizontalHeader().setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         # MCB - This doesn't work.  Probably because we aren't actually
         # tracking the selection, just clearing it when it isn't visible.
         # So just turn it off.
         self.horizontalHeader().setHighlightSections(False)
-        
+
         self.customContextMenuRequested.connect(self.showContextMenu)
-        self.horizontalHeader().customContextMenuRequested.connect(self.showHeaderContextMenu)
+        self.horizontalHeader().customContextMenuRequested.connect(
+            self.showHeaderContextMenu
+        )
 
     #
     # We're cheating here.  We are making a distinction between a drag (which
     # becomes a CopyAction) and a shift-drag (which becomes a MoveAction).
     # However, we don't really want to ever move, since that automatically
     # deletes the source data in the model.  Therefore, in our dropEvent,
     # we remember what we wanted, but force everything to be CopyAction.
@@ -76,48 +81,48 @@
             event.setDropAction(QtCore.Qt.CopyAction)
         QtWidgets.QTableView.dropEvent(self, event)
 
     def setModel(self, model):
         QtWidgets.QTableView.setModel(self, model)
         model.columnsInserted.connect(self.insertColumns)
         model.rowsInserted.connect(self.insertRows)
-        
+
     def insertColumns(self, parent, start, finish):
         if self.hidecols != -1:
             if self.model().columnCount() != self.horizontalHeader().count():
                 # Sigh.  We have a race condition.  Just reschedule for later.
-                QtCore.QTimer.singleShot(0, lambda : self.hideAllColumns(start))
+                QtCore.QTimer.singleShot(0, lambda: self.hideAllColumns(start))
             else:
-                for col in range(start, finish+1):
+                for col in range(start, finish + 1):
                     if col >= self.hidecols:
                         self.setColumnHidden(col, True)
-    
+
     def insertRows(self, parent, start, finish):
         if self.hiderows != -1:
             if self.model().rowCount() != self.verticalHeader().count():
                 # Sigh.  We have a race condition.  Just reschedule for later.
-                QtCore.QTimer.singleShot(0, lambda : self.hideAllRows(start))
+                QtCore.QTimer.singleShot(0, lambda: self.hideAllRows(start))
             else:
-                for row in range(start, finish+1):
+                for row in range(start, finish + 1):
                     if row >= self.hiderows:
                         self.setRowHidden(row, True)
 
     def hideAllColumns(self, start):
         if self.model().columnCount() != self.horizontalHeader().count():
             # Still racing!
-            QtCore.QTimer.singleShot(0, lambda : self.hideAllColumns(start))
+            QtCore.QTimer.singleShot(0, lambda: self.hideAllColumns(start))
         else:
             for col in range(start, self.model().columnCount()):
                 if col >= self.hidecols:
                     self.setColumnHidden(col, True)
 
     def hideAllRows(self, start):
         if self.model().rowCount() != self.verticalHeader().count():
             # Still racing!
-            QtCore.QTimer.singleShot(0, lambda : self.hideAllRows(start))
+            QtCore.QTimer.singleShot(0, lambda: self.hideAllRows(start))
         else:
             for row in range(start, self.model().rowCount()):
                 if row >= self.hiderows:
                     self.setRowHidden(row, True)
 
     def addContextMenu(self, menu):
         self.menus.append(menu)
@@ -139,16 +144,18 @@
     def showHeaderContextMenu(self, pos):
         index = self.horizontalHeader().logicalIndexAt(pos)
         for m in self.hmenus:
             if m.isActive(self, index):
                 m.doMenu(self, pos, index)
                 return
 
+
 ######################################################################
-    
+
+
 class FreezeTableView(DropTableView):
     def __init__(self, parent=None):
         DropTableView.__init__(self, parent, -1, -1, "main")
         self.didinit = False
 
     def init(self, model, rows=0, cols=0):
         self.setModel(model)
@@ -162,26 +169,26 @@
         self.fTV = fTV
         fTV.setModel(self.model())
         fTV.setHorizontalHeader(FreezeHeaderView(QtCore.Qt.Horizontal, self))
         fTV.horizontalHeader().setShadowHeader(self.horizontalHeader())
         fTV.setVerticalHeader(FreezeHeaderView(QtCore.Qt.Vertical, self))
         fTV.verticalHeader().setShadowHeader(self.verticalHeader())
         fTV.setStyleSheet("QTableView { border: none; }")
-        #fTV.setStyleSheet("QTableView { border: none; background-color: #FF0000  }")
-        #fTV.horizontalHeader().setStyleSheet("QHeaderView { background-color: #FF0000  }")
+        # fTV.setStyleSheet("QTableView { border: none; background-color: #FF0000  }")
+        # fTV.horizontalHeader().setStyleSheet("QHeaderView { background-color: #FF0000  }")
 
         for col in range(self.model().columnCount()):
             if col >= self.fcols:
                 fTV.setColumnHidden(col, True)
         for row in range(self.model().rowCount()):
             if row >= self.frows:
                 fTV.setRowHidden(row, True)
         fTV.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
         fTV.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
-    
+
         cTV = DropTableView(self, -1, self.fcols, "cTV")
         self.cTV = cTV
         cTV.setModel(self.model())
         cTV.verticalHeader().hide()
         cTV.horizontalHeader().hide()
         cTV.setStyleSheet("QTableView { border: none; }")
         for col in range(self.model().columnCount()):
@@ -243,23 +250,27 @@
         self.setFrozenRowHeight()
 
         # Share a delegate!
         delegate = self.itemDelegate()
         self.fTV.setItemDelegate(delegate)
         self.cTV.setItemDelegate(delegate)
         self.rTV.setItemDelegate(delegate)
-        
+
         self.horizontalHeader().sectionResized.connect(self.updateSectionWidth)
         self.verticalHeader().sectionResized.connect(self.updateSectionHeight)
-        
+
         cTV.verticalScrollBar().valueChanged.connect(self.verticalScrollBar().setValue)
         self.verticalScrollBar().valueChanged.connect(cTV.verticalScrollBar().setValue)
-        
-        rTV.horizontalScrollBar().valueChanged.connect(self.horizontalScrollBar().setValue)
-        self.horizontalScrollBar().valueChanged.connect(rTV.horizontalScrollBar().setValue)
+
+        rTV.horizontalScrollBar().valueChanged.connect(
+            self.horizontalScrollBar().setValue
+        )
+        self.horizontalScrollBar().valueChanged.connect(
+            rTV.horizontalScrollBar().setValue
+        )
 
         self.selectionModel().selectionChanged.connect(self.parentSelectionChanged)
         cTV.selectionModel().selectionChanged.connect(self.colSelectionChanged)
         rTV.selectionModel().selectionChanged.connect(self.rowSelectionChanged)
         fTV.selectionModel().selectionChanged.connect(self.frozenSelectionChanged)
 
         self.horizontalHeader().sectionMoved.connect(self.fixColumnMove)
@@ -313,15 +324,15 @@
             self.rTV.setRowHidden(row, hide)
 
     def setSortingEnabled(self, value):
         DropTableView.setSortingEnabled(self, value)
         self.cTV.setSortingEnabled(value)
         self.rTV.setSortingEnabled(value)
         self.fTV.setSortingEnabled(value)
-        
+
     def addHorizontalSectionWidget(self, logidx, w):
         self.itemDelegate().addSectionWidget(logidx, w, self)
 
     def setFrozenColWidth(self):
         total = 0
         for i in range(self.fcols):
             total += self.columnWidth(i)
@@ -352,65 +363,91 @@
     def resizeEvent(self, event):
         DropTableView.resizeEvent(self, event)
         if self.didinit:
             self.updateFTGeometry()
 
     def moveCursor(self, ca, mods):
         cur = DropTableView.moveCursor(self, ca, mods)
-        if (ca == QtWidgets.QAbstractItemView.MoveLeft and cur.column() > 0 and
-            self.visualRect(cur).topLeft().x() < self.fcolwidth):
-            nv = (self.horizontalScrollBar().value() + self.visualRect(cur).topLeft().x() -
-                  self.fcolwidth)
+        if (
+            ca == QtWidgets.QAbstractItemView.MoveLeft
+            and cur.column() > 0
+            and self.visualRect(cur).topLeft().x() < self.fcolwidth
+        ):
+            nv = (
+                self.horizontalScrollBar().value()
+                + self.visualRect(cur).topLeft().x()
+                - self.fcolwidth
+            )
             self.horizontalScrollBar().setValue(nv)
-        if (ca == QtWidgets.QAbstractItemView.MoveUp and cur.row() > 0 and
-            self.visualRect(cur).topLeft().y() < self.frowheight):
-            nv = (self.verticalScrollBar().value() + self.visualRect(cur).topLeft().y() -
-                  self.frowheight)
+        if (
+            ca == QtWidgets.QAbstractItemView.MoveUp
+            and cur.row() > 0
+            and self.visualRect(cur).topLeft().y() < self.frowheight
+        ):
+            nv = (
+                self.verticalScrollBar().value()
+                + self.visualRect(cur).topLeft().y()
+                - self.frowheight
+            )
             self.verticalScrollBar().setValue(nv)
         return cur
 
     def scrollTo(self, index, hint):
         if index.column() > 0:
             DropTableView.scrollTo(self, index, hint)
 
     def updateFTGeometry(self):
-        self.fTV.setGeometry((self.frameWidth() +
-                              (self.verticalHeader().width() if self.frowheight == 0 else 0)),
-                             (self.frameWidth() +
-                              (self.horizontalHeader().height() if self.fcolwidth == 0 else 0)),
-                             (self.fcolwidth + (self.verticalHeader().width()
-                                               if self.frowheight != 0 else 0)),
-                             (self.frowheight + (self.horizontalHeader().height()
-                                                 if self.fcolwidth != 0 else 0)))
-        self.cTV.setGeometry(self.verticalHeader().width() + self.frameWidth(),
-                             self.horizontalHeader().height() + self.frameWidth() + self.frowheight,
-                             self.fcolwidth,
-                             self.viewport().height() - self.frowheight)
-        self.rTV.setGeometry(self.verticalHeader().width() + self.frameWidth() + self.fcolwidth,
-                             self.horizontalHeader().height() + self.frameWidth(),
-                             self.viewport().width() - self.fcolwidth,
-                             self.frowheight)
+        self.fTV.setGeometry(
+            (
+                self.frameWidth()
+                + (self.verticalHeader().width() if self.frowheight == 0 else 0)
+            ),
+            (
+                self.frameWidth()
+                + (self.horizontalHeader().height() if self.fcolwidth == 0 else 0)
+            ),
+            (
+                self.fcolwidth
+                + (self.verticalHeader().width() if self.frowheight != 0 else 0)
+            ),
+            (
+                self.frowheight
+                + (self.horizontalHeader().height() if self.fcolwidth != 0 else 0)
+            ),
+        )
+        self.cTV.setGeometry(
+            self.verticalHeader().width() + self.frameWidth(),
+            self.horizontalHeader().height() + self.frameWidth() + self.frowheight,
+            self.fcolwidth,
+            self.viewport().height() - self.frowheight,
+        )
+        self.rTV.setGeometry(
+            self.verticalHeader().width() + self.frameWidth() + self.fcolwidth,
+            self.horizontalHeader().height() + self.frameWidth(),
+            self.viewport().width() - self.fcolwidth,
+            self.frowheight,
+        )
 
     def setHorizontalHeader(self, header):
         DropTableView.setHorizontalHeader(self, header)
         self.fTV.horizontalHeader().setShadowHeader(self.horizontalHeader())
         self.horizontalHeader().sectionResized.connect(self.updateSectionWidth)
-        
+
     def setItemDelegateForRow(self, row, delegate):
         DropTableView.setItemDelegateForRow(self, row, delegate)
         self.fTV.setItemDelegateForRow(row, delegate)
         self.cTV.setItemDelegateForRow(row, delegate)
         self.rTV.setItemDelegateForRow(row, delegate)
-        
+
     def setItemDelegateForColumn(self, column, delegate):
         DropTableView.setItemDelegateForColumn(self, column, delegate)
         self.fTV.setItemDelegateForColumn(column, delegate)
         self.cTV.setItemDelegateForColumn(column, delegate)
         self.rTV.setItemDelegateForColumn(column, delegate)
-        
+
     def setItemDelegate(self, delegate):
         DropTableView.setItemDelegate(self, delegate)
         self.fTV.setItemDelegate(delegate)
         self.cTV.setItemDelegate(delegate)
         self.rTV.setItemDelegate(delegate)
 
     def openPersistentEditor(self, index):
@@ -446,16 +483,24 @@
     def setRowHeight(self, row, size):
         DropTableView.setRowHeight(self, row, size)
         self.fTV.setRowHeight(row, size)
         self.cTV.setRowHeight(row, size)
         self.rTV.setRowHeight(row, size)
 
     def printSize(self, n):
-        print("%d: main=%d, fTV=%d, rTV=%d, cTV=%d" % (n, self.rowHeight(n), self.fTV.rowHeight(n),
-                                                       self.rTV.rowHeight(n), self.cTV.rowHeight(n)))
+        print(
+            "%d: main=%d, fTV=%d, rTV=%d, cTV=%d"
+            % (
+                n,
+                self.rowHeight(n),
+                self.fTV.rowHeight(n),
+                self.rTV.rowHeight(n),
+                self.cTV.rowHeight(n),
+            )
+        )
 
     def addContextMenu(self, menu):
         DropTableView.addContextMenu(self, menu)
         self.cTV.addContextMenu(menu)
         self.rTV.addContextMenu(menu)
         self.fTV.addContextMenu(menu)
```

### Comparing `pmgr-2.0.2/pmgr/MyDelegate.py` & `pmgr-2.1.3/pmgr/MyDelegate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-from PyQt5.QtGui import *
-from PyQt5.QtWidgets import *
-from PyQt5.QtCore import *
 import re
-import numpy as np
 
-from . import param
+import numpy as np
+from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt5.QtCore import Qt
 
 #########################################################################
 #
 # Code shamelessly stolen from http://jdreaver.com/posts/2014-07-28-scientific-notation-spin-box-pyside.html.
 #
 
-_float_re = re.compile(r'(([+-]?\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?)')
+_float_re = re.compile(r"(([+-]?\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?)")
+
 
 def valid_float_string(string):
     match = _float_re.search(string)
     return match.groups()[0] == string if match else False
 
-class FloatValidator(QValidator):
+
+class FloatValidator(QtGui.QValidator):
     def validate(self, string, position):
         if valid_float_string(string):
-            return (QValidator.Acceptable, string, position)
+            return (self.State.Acceptable, string, position)
         s = str(string)
-        if s == "" or s[position-1] in 'e.-+':
-            return (QValidator.Intermediate, string, position)
-        return (QValidator.Invalid, string, position)
+        if s == "" or s[position - 1] in "e.-+":
+            return (self.State.Intermediate, string, position)
+        return (self.State.Invalid, string, position)
 
     def fixup(self, text):
         match = _float_re.search(str(text))
         return match.groups()[0] if match else ""
 
-class ScientificDoubleSpinBox(QDoubleSpinBox):
+
+class ScientificDoubleSpinBox(QtWidgets.QDoubleSpinBox):
     def __init__(self, parent=None):
-        QDoubleSpinBox.__init__(self, parent)
+        super().__init__(parent)
         self.setMinimum(-np.inf)
         self.setMaximum(np.inf)
         self.validator = FloatValidator()
         self.setDecimals(1000)
 
     def validate(self, text, position):
         return self.validator.validate(text, position)
@@ -51,70 +52,71 @@
         return format_float(value)
 
     def stepBy(self, steps):
         text = self.cleanText()
         groups = _float_re.search(text).groups()
         decimal = float(groups[1])
         decimal += steps
-        new_string = "{:g}".format(decimal) + (groups[3] if groups[3] else "")
+        new_string = f"{decimal:g}" + (groups[3] if groups[3] else "")
         self.lineEdit().setText(new_string)
 
+
 def format_float(value):
     """Modified form of the 'g' format specifier."""
-    string = "{:g}".format(value).replace("e+", "e")
-    string = re.sub("e(-?)0*(\d+)", r"e\1\2", string)
+    string = f"{value:g}".replace("e+", "e")
+    string = re.sub(r"e(-?)0*(\d+)", r"e\1\2", string)
     return string
 
+
 #########################################################################
 
-class MyDelegate(QStyledItemDelegate):
-    def __init__(self, parent):
-        QStyledItemDelegate.__init__(self, parent)
 
+class MyDelegate(QtWidgets.QStyledItemDelegate):
     def createEditor(self, parent, option, index):
         e = index.model().editorInfo(index)
         if e == str:
-            editor = QItemEditorFactory.defaultFactory().createEditor(QVariant.String, parent)
+            editor = QtWidgets.QItemEditorFactory.defaultFactory().createEditor(
+                QtCore.QVariant.String, parent
+            )
             editor.mydelegate = False
         elif e == int:
-            editor = QItemEditorFactory.defaultFactory().createEditor(QVariant.Int, parent)
+            editor = QtWidgets.QItemEditorFactory.defaultFactory().createEditor(
+                QtCore.QVariant.Int, parent
+            )
             editor.mydelegate = False
         elif e == float:
             editor = ScientificDoubleSpinBox(parent)
             editor.mydelegate = False
         else:
             # Must be an enum list!
-            editor = QComboBox(parent)
+            editor = QtWidgets.QComboBox(parent)
             editor.enum = e
             editor.setAutoFillBackground(True)
             for item in e:
                 editor.addItem(item)
             editor.mydelegate = True
         return editor
 
     def setEditorData(self, editor, index):
         if editor.mydelegate:
             value = index.model().data(index, Qt.EditRole)
             try:
                 idx = editor.enum.index(value)
                 editor.setCurrentIndex(idx)
-            except:
+            except Exception:
                 # What was dumb is now smart?!?
                 editor.setCurrentIndex(0)
         else:
-            QStyledItemDelegate.setEditorData(self, editor, index)
+            super().setEditorData(editor, index)
 
     def setModelData(self, editor, model, index):
         if editor.mydelegate:
-            if editor.enum == None:
+            if editor.enum is None:
                 v = editor.checkState()
                 if v == Qt.Checked:
                     model.setData(index, 1)
                 else:
                     model.setData(index, 0)
             else:
                 model.setData(index, editor.currentText())
         else:
-            QStyledItemDelegate.setModelData(self, editor, model, index)
-
-    def sizeHint(self, option, index):
-        return QStyledItemDelegate.sizeHint(self, option, index)
+            super().setModelData(editor, model, index)
```

### Comparing `pmgr-2.0.2/pmgr/ObjModel.py` & `pmgr-2.1.3/pmgr/ObjModel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-from functools import reduce
 import datetime
+from functools import reduce
 
-from PyQt5 import QtCore, QtGui, QtWidgets
 import pyca
+from PyQt5 import QtCore, QtGui, QtWidgets
 
-from . import colmgr
-from . import param
-from . import utils
-
+from . import colmgr, param, utils
 
-try:
-    QString = unicode
-except NameError:
-    # Python 3
-    QString = str
 
 class ObjModel(QtGui.QStandardItemModel):
     """
     This is the Model (from the Model-View-Controller paradigm) supporting
     the object table.  This is a 2D table: rows are configurations, and
     columns are object values.
 
     The heart of this is two routines:
         data(index, role) takes a QModelIndex and a Qt.DisplayRole and returns
         the value corresponding to that location in the table.
 
         setData(index, value, role) takes a QModelIndex and a new value, and
         stores that value into the table for the specified role.
     """
+
     layoutAboutToBeChanged = QtCore.pyqtSignal()
     layoutChanged = QtCore.pyqtSignal()
-    cname   = ["Status", "PV Base", "Config", "Owner", "Config Mode", "Comment"]
-    cfld    = ["status", "rec_base", "cfgname", "owner", "category", "comment"]
-    ctips   = ["C = All PVs Connected\nD = Deleted\nM = Modified\nN = New\nX = Inconsistent",
-               "PV Base Name", "Configuration Name", "Owner", None, None]
-    coff    = len(cname)
+    cname = ["Status", "PV Base", "Config", "Owner", "Config Mode", "Comment"]
+    cfld = ["status", "rec_base", "cfgname", "owner", "category", "comment"]
+    ctips = [
+        "C = All PVs Connected\nD = Deleted\nM = Modified\nN = New\nX = Inconsistent",
+        "PV Base Name",
+        "Configuration Name",
+        "Owner",
+        None,
+        None,
+    ]
+    coff = len(cname)
     statcol = 0
-    pvcol   = 1
-    cfgcol  = 2
-    owncol  = 3
-    catcol  = 4
-    comcol  = 5
+    pvcol = 1
+    cfgcol = 2
+    owncol = 3
+    catcol = 4
+    comcol = 5
     mutable = 3  # The first non-frozen column
     fixflds = ["status", "cfgname", "owner"]
-    
+
     def __init__(self):
         QtGui.QStandardItemModel.__init__(self)
         self.pvdict = {}
         self.edits = {}
         self.objs = {}
         self.status = {}
         self.istatus = {}
@@ -61,52 +60,51 @@
         self.setRowCount(len(param.params.pobj.objs))
         self.rowmap = list(param.params.pobj.objs.keys())
         font = QtGui.QFont()
         font.setBold(True)
         for c in range(self.colcnt):
             if c < self.coff:
                 i = QtGui.QStandardItem(self.cname[c])
-                if self.ctips[c] != None:
+                if self.ctips[c] is not None:
                     i.setToolTip(self.ctips[c])
             else:
-                i = QtGui.QStandardItem(param.params.pobj.objflds[c-self.coff]['alias'])
-                desc = param.params.pobj.objflds[c-self.coff]['tooltip']
+                i = QtGui.QStandardItem(
+                    param.params.pobj.objflds[c - self.coff]["alias"]
+                )
+                desc = param.params.pobj.objflds[c - self.coff]["tooltip"]
                 if desc != "":
                     i.setToolTip(desc)
             self.setHorizontalHeaderItem(c, i)
         self.createStatus()
         self.connectAllPVs()
 
         self.layoutAboutToBeChanged.connect(self.doShowAll)
         self.layoutChanged.connect(self.doShow)
 
     def createStatus(self):
         for d in param.params.pobj.objs.values():
-            try:
-                v = self.status[d['id']]
-            except:
-                self.status[d['id']] = ""
-            try:
-                v = self.istatus[d['id']]
-            except:
-                self.istatus[d['id']] = set([])
+            self.status.setdefault(d["id"], "")
+            self.istatus.setdefault(d["id"], set())
 
     def getStatus(self, idx):
         v = self.status[idx]
-        if self.istatus[idx] != set([]):
+        if self.istatus[idx] != set():
             return "".join(sorted("X" + v))
         else:
             return v
 
     def index2db(self, index):
         c = index.column()
         if c < self.coff:
             return (self.rowmap[index.row()], self.cfld[c])
         else:
-            return (self.rowmap[index.row()], param.params.pobj.objflds[c-self.coff]['fld'])
+            return (
+                self.rowmap[index.row()],
+                param.params.pobj.objflds[c - self.coff]["fld"],
+            )
 
     def getObj(self, idx):
         """
         Get the object dictionary for this index.  Negative indices
         aren't committed and found in self.objs, otherwise we look in
         the real database.
 
@@ -122,28 +120,28 @@
         """
         if idx >= 0:
             return param.params.pobj.objs[idx]
         else:
             return self.objs[idx]
 
     #
-    # getCfg(idx, field, GetEdit=True) - 
+    # getCfg(idx, field, GetEdit=True) -
     #     This retrieves both configuration fields and object fields.  If it's a configuration
     #     field, we always return the most recent edited value of the *edited* config field
     #     for this object.  If it's an object field, we return an edit if GetEdit is true,
     #     otherwise the configured value.
     #
     def getCfg(self, idx, f, GetEdit=True):
         """
         Get the value of the field for a particular index.
 
         Object fields and configuration fields are handled slightly
         differently.
 
-        If it's a configuration field, return the most recent edit if 
+        If it's a configuration field, return the most recent edit if
         one exists, otherwise return the configured value.
 
         If it's an object field, return the most recent edit if GetEdit
         is True, otherwise return the configured value.
 
         Parameters
         ----------
@@ -160,214 +158,225 @@
         -------
         value : any
             The field value.
         """
         if GetEdit:
             try:
                 return self.edits[idx][f]
-            except:
+            except Exception:
                 pass
-        if f in self.cfld or f == 'mutex' or f == 'config':
+        if f in self.cfld or f == "mutex" or f == "config":
             return self.getObj(idx)[f]
-        elif param.params.pobj.fldmap[f]['obj']:
-            return self.getObj(idx)['_cfg'][f]
+        elif param.params.pobj.fldmap[f]["obj"]:
+            return self.getObj(idx)["_cfg"][f]
         else:
             try:
-                cfg = self.edits[idx]['config']
-            except:
-                cfg = self.getObj(idx)['config']
+                cfg = self.edits[idx]["config"]
+            except Exception:
+                cfg = self.getObj(idx)["config"]
             try:
                 return param.params.cfgmodel.edits[cfg][f]
-            except:
+            except Exception:
                 return param.params.cfgmodel.getCfg(cfg)[f]
-        
-    def data(self, index, role = QtCore.Qt.DisplayRole):
-        if (role != QtCore.Qt.DisplayRole and role != QtCore.Qt.EditRole and
-            role != QtCore.Qt.ForegroundRole and role != QtCore.Qt.BackgroundRole and
-            role != QtCore.Qt.ToolTipRole):
+
+    def data(self, index, role=QtCore.Qt.DisplayRole):
+        if (
+            role != QtCore.Qt.DisplayRole
+            and role != QtCore.Qt.EditRole
+            and role != QtCore.Qt.ForegroundRole
+            and role != QtCore.Qt.BackgroundRole
+            and role != QtCore.Qt.ToolTipRole
+        ):
             return QtGui.QStandardItemModel.data(self, index, role)
         if not index.isValid():
             return None
         (idx, f) = self.index2db(index)
         if role == QtCore.Qt.ToolTipRole:
-            if f == 'status':
+            if f == "status":
                 return QtGui.QStandardItemModel.data(self, index, role)
             try:
-                if param.params.pobj.fldmap[f]['readonly']:
+                if param.params.pobj.fldmap[f]["readonly"]:
                     return QtGui.QStandardItemModel.data(self, index, role)
-            except:
+            except Exception:
                 pass
             try:
-                ve = self.edits[idx][f]     # Edited value
-                if ve == None:
+                ve = self.edits[idx][f]  # Edited value
+                if ve is None:
                     ve = "None"
-            except:
+            except Exception:
                 ve = None
             try:
-                va = self.getObj(idx)[f]    # Actual value
-            except:
+                va = self.getObj(idx)[f]  # Actual value
+            except Exception:
                 va = None
-            vc = self.getCfg(idx, f, False) # Configured value
-            if ve == None and (vc == None or param.equal(va, vc)):
+            vc = self.getCfg(idx, f, False)  # Configured value
+            if ve is None and (vc is None or param.equal(va, vc)):
                 return QtGui.QStandardItemModel.data(self, index, role)
             v = "Configured Value: %s" % str(vc)
             v += "\nActual Value: %s" % str(va)
-            if ve != None:
+            if ve is not None:
                 v += "\nEdited Value: %s" % str(ve)
             return v
         if f == "status":
             if role == QtCore.Qt.ForegroundRole:
                 return param.params.black
             elif role == QtCore.Qt.BackgroundRole:
                 return param.params.white
             else:
                 return self.getStatus(idx)
         try:
             v = self.getObj(idx)[f]  # Actual value
-        except:
+        except Exception:
             v = None
-        v2 = self.getCfg(idx, f) # Configured value
-        if f[:4] == 'FLD_' or f[:3] == 'PV_':
-            if (v == None or v2 == None or param.equal(v, v2) or 
-                param.params.pobj.fldmap[f]['readonly']):
+        v2 = self.getCfg(idx, f)  # Configured value
+        if f[:4] == "FLD_" or f[:3] == "PV_":
+            if (
+                v is None
+                or v2 is None
+                or param.equal(v, v2)
+                or param.params.pobj.fldmap[f]["readonly"]
+            ):
                 try:
-                    self.istatus[idx].remove(f) # If we don't have a value (either
-                                                # the PV isn't connected, or is is a
-                                                # derived value in the configuration),
-                                                # or the PV is equal to the configuration,
-                                                # we're not inconsistent.  (Readonly PVs
-                                                # are never inconsistent!)
-                except:
+                    self.istatus[idx].remove(f)  # If we don't have a value (either
+                    # the PV isn't connected, or is is a
+                    # derived value in the configuration),
+                    # or the PV is equal to the configuration,
+                    # we're not inconsistent.  (Readonly PVs
+                    # are never inconsistent!)
+                except Exception:
                     pass
             else:
-                self.istatus[idx].add(f)        # Otherwise, we are!
+                self.istatus[idx].add(f)  # Otherwise, we are!
         if role == QtCore.Qt.BackgroundRole:
             # If the actual value is None, the PV is not connected.
             # If the configuration value is None, the PV is derived.
-            if f in self.cfld or param.params.pobj.fldmap[f]['obj']:
+            if f in self.cfld or param.params.pobj.fldmap[f]["obj"]:
                 # An object value!  Let "derived" win!
-                if v2 == None:
-                    return param.params.almond    # A derived value.
-                elif v == None:
-                    return param.params.gray      # Not connected.
+                if v2 is None:
+                    return param.params.almond  # A derived value.
+                elif v is None:
+                    return param.params.gray  # Not connected.
                 elif v == "" and v2 != "":
-                    return param.params.ltblue    # Actually empty, but there is a configured value.
+                    return (
+                        param.params.ltblue
+                    )  # Actually empty, but there is a configured value.
                 else:
-                    return param.params.white     # An ordinary cell.
+                    return param.params.white  # An ordinary cell.
             else:
                 # A configuration value!  Let "not connected" win!
-                if v == None:
-                    return param.params.gray      # Not connected.
+                if v is None:
+                    return param.params.gray  # Not connected.
                 elif v == "" and v2 != "":
-                    return param.params.ltblue    # Actually empty, but there is a configured value.
-                elif v2 == None:
-                    return param.params.almond    # A derived value.
+                    return (
+                        param.params.ltblue
+                    )  # Actually empty, but there is a configured value.
+                elif v2 is None:
+                    return param.params.almond  # A derived value.
                 else:
-                    return param.params.ltgray    # An ordinary cell.
+                    return param.params.ltgray  # An ordinary cell.
         elif role == QtCore.Qt.ForegroundRole:
             try:
                 v = self.edits[idx][f]
                 return param.params.red
-            except:
+            except Exception:
                 pass
             try:
-                if param.params.pobj.fldmap[f]['readonly']:
+                if param.params.pobj.fldmap[f]["readonly"]:
                     return param.params.black
-            except:
+            except Exception:
                 pass
-            if v2 == None or param.equal(v, v2):
+            if v2 is None or param.equal(v, v2):
                 return param.params.black
             else:
                 return param.params.blue
             return None
         elif role == QtCore.Qt.DisplayRole:
             try:
                 v = self.edits[idx][f]
-            except:
+            except Exception:
                 pass
-        else:   # QtCore.Qt.EditRole
+        else:  # QtCore.Qt.EditRole
             try:
                 v = self.edits[idx][f]
-            except:
-                if v2 != None:
+            except Exception:
+                if v2 is not None:
                     v = v2
         # DisplayRole or EditRole fall through... v has our value!
-        if f == 'category':
+        if f == "category":
             v = param.params.catenum2[param.params.catenum.index(v)]
         return v
 
     def setValue(self, idx, f, v):
         try:
             d = self.edits[idx]
-        except:
+        except Exception:
             d = {}
-        hadedit = (d != {})
+        hadedit = d != {}
         # OK, the config/cfgname thing is slightly weird.  The field name for our index is
         # 'cfgname', but we are passing an int that should go to 'config'.  So we need to
         # change *both*!
-        if f == 'cfgname':
+        if f == "cfgname":
             vlink = v
             v = param.params.db.getCfgName(vlink)
         # Remove f from the current set of edits.
         try:
             del d[f]
-            if f == 'cfgname':
-                del d['config']
-        except:
+            if f == "cfgname":
+                del d["config"]
+        except Exception:
             pass
-        if f == 'category':
+        if f == "category":
             v = param.params.catenum[param.params.catenum2.index(v)]
         # Get the currently configured value of the field.
         v2 = self.getCfg(idx, f)
         if not param.equal(v, v2):
             # If we have a change, add it to the edits and change the status if necessary.
             d[f] = v
-            if f == 'cfgname':
-                d['config'] = vlink
+            if f == "cfgname":
+                d["config"] = vlink
             if not hadedit and idx >= 0:
                 self.status[idx] = "".join(sorted("M" + self.status[idx]))
                 self.statchange(idx)
         else:
             # If we just undid our last change, we're no longer modified.
             if hadedit and d == {} and idx >= 0:
                 self.status[idx] = self.status[idx].replace("M", "")
                 self.statchange(idx)
-        if d != {}:       # If we still have edits.
-            if idx < 0:   # If this is a new object, make the change directly.
-
+        if d != {}:  # If we still have edits.
+            if idx < 0:  # If this is a new object, make the change directly.
                 self.objs[idx].update(d)
-                self.objs[idx]['_cfg'].update(d)
-            else:         # Otherwise, save the change in edits.
+                self.objs[idx]["_cfg"].update(d)
+            else:  # Otherwise, save the change in edits.
                 self.edits[idx] = d
-        else:             # If we've deleted our last change.
-            try:          # Try to fixup the status.
+        else:  # If we've deleted our last change.
+            try:  # Try to fixup the status.
                 del self.edits[idx]
                 self.status[idx] = self.status[idx].replace("M", "")
                 self.statchange(idx)
-            except:
+            except Exception:
                 pass
-        mutex = self.getCfg(idx, 'mutex')
+        mutex = self.getCfg(idx, "mutex")
         try:
             # If we are assigning a value to a derived field, make something else
             # derived!
-            cm = chr(param.params.pobj.fldmap[f]['colorder']+0x40)
+            cm = chr(param.params.pobj.fldmap[f]["colorder"] + 0x40)
             if cm in mutex:
                 i = mutex.find(cm)
                 self.promote(idx, f, i, mutex)
-        except:
+        except Exception:
             pass
 
     def setData(self, index, v, role=QtCore.Qt.EditRole):
         if role != QtCore.Qt.DisplayRole and role != QtCore.Qt.EditRole:
-            return QtGui.QStandardItemModel.setData(self, index, value, role)
+            return super().setData(index, v, role)
         (idx, f) = self.index2db(index)
-        
+
         self.setValue(idx, f, v)
-        
-        if f == 'rec_base':
+
+        if f == "rec_base":
             self.connectPVs(idx)
             r = index.row()
             self.dataChanged.emit(self.index(r, 0), self.index(r, self.colcnt - 1))
         else:
             self.dataChanged.emit(index, index)
         return True
 
@@ -380,67 +389,71 @@
             else:
                 derived = mlist[0]
         else:
             d = param.params.deriveddialog
             d.reset()
             for fld in mlist:
                 if fld != f:
-                    d.addValue(param.params.pobj.fldmap[fld]['alias'], fld)
+                    d.addValue(param.params.pobj.fldmap[fld]["alias"], fld)
             d.exec_()
             # The user *must* give a value.  I'll take whatever is checked even if the
             # window was just closed!!
             derived = d.getValue()
         for fld in mlist:
             if fld == derived:
                 # The config value of the derived field must be None!
-                if self.getObj(idx)['_cfg'][fld] == None:
-                    try: # If it was configured to be None, get rid of any edit.
+                if self.getObj(idx)["_cfg"][fld] is None:
+                    try:  # If it was configured to be None, get rid of any edit.
                         del self.edits[idx][fld]
                         if self.edits[idx] == {}:
                             del self.edits[idx]
                             self.status[idx] = self.status[idx].replace("M", "")
                             self.statchange(idx)
-                    except:
+                    except Exception:
                         pass
-                else:   # If it had a value, edit it to None.
+                else:  # If it had a value, edit it to None.
                     try:
                         self.edits[idx][fld] = None
-                    except:
+                    except Exception:
                         self.edits[idx] = {fld: None}
-        cm = chr(param.params.pobj.fldmap[derived]['colorder']+0x40)
-        curmutex = curmutex[:setidx] + cm + curmutex[setidx+1:]
-        if self.getObj(idx)['mutex'] == curmutex:
+        cm = chr(param.params.pobj.fldmap[derived]["colorder"] + 0x40)
+        curmutex = curmutex[:setidx] + cm + curmutex[setidx + 1 :]
+        if self.getObj(idx)["mutex"] == curmutex:
             try:
-                del self.edits[idx]['mutex']
+                del self.edits[idx]["mutex"]
                 if self.edits[idx] == {}:
                     del self.edits[idx]
                     self.status[idx] = self.status[idx].replace("M", "")
                     self.statchange(idx)
-            except:
+            except Exception:
                 pass
         else:
             try:
-                self.edits[idx]['mutex'] = curmutex
-            except:
-                self.edits[idx] = {'mutex': curmutex}
+                self.edits[idx]["mutex"] = curmutex
+            except Exception:
+                self.edits[idx] = {"mutex": curmutex}
         return curmutex
-        
+
     def sortkey(self, idx, c):
         if c == self.statcol:
             return self.getStatus(idx)
         if c < self.coff:
             f = self.cfld[c]
         else:
-            f = param.params.pobj.objflds[c-self.coff]['fld']
+            f = param.params.pobj.objflds[c - self.coff]["fld"]
         try:
             return self.edits[idx][f]
-        except:
+        except Exception:
             try:
-                return self.getObj(idx)[f]
-            except:
+                x = self.getObj(idx)[f]
+                if x is None:
+                    return ""
+                else:
+                    return x
+            except Exception:
                 return ""
 
     def sort(self, Ncol, order):
         if (Ncol, order) != self.lastsort:
             self.lastsort = (Ncol, order)
             self.layoutAboutToBeChanged.emit()
             self.rowmap = sorted(self.rowmap, key=lambda idx: self.sortkey(idx, Ncol))
@@ -458,139 +471,141 @@
         self.layoutAboutToBeChanged.emit()
         self.layoutChanged.emit()
 
     def statchange(self, id):
         try:
             idx = self.index(self.rowmap.index(id), self.statcol)
             self.dataChanged.emit(idx, idx)
-        except:
+        except Exception:
             pass
 
     #
     # Connect all of the PVs, and build a pv dictionary.  The dictionary
     # has two mappings: field to PV and pv name to PV.  We use the second
     # to find PVs we are already connected to, and we use the first to
     # find the PV when we apply.
     #
     def connectPVs(self, idx):
         """
         Connect all of the PVs for the given index, and build a pv
         dictionary.  The dictionary has two mappings: field to PV and
-        pv name to PV.  We use the second to find PVs we are already 
+        pv name to PV.  We use the second to find PVs we are already
         connected to, and we use the first to find the PV when we apply.
 
         Parameters
         ----------
         idx : int
             An object identifier.
 
         Returns
         -------
         Nothing.
         """
         try:
             oldpvdict = self.pvdict[idx]
-        except:
+        except Exception:
             oldpvdict = {}
         d = self.getObj(idx)
         try:
-            base = self.edits[idx]['rec_base']
-        except:
-            base = d['rec_base']
+            base = self.edits[idx]["rec_base"]
+        except Exception:
+            base = d["rec_base"]
         newpvdict = {}
-        d['connstat'] = len(param.params.pobj.objflds)*[False]
+        d["connstat"] = len(param.params.pobj.objflds) * [False]
         self.status[idx] = self.status[idx].replace("C", "")
         if base != "":
             for ofld in param.params.pobj.objflds:
-                n = base + ofld['pv']
-                f = ofld['fld']
+                n = base + ofld["pv"]
+                f = ofld["fld"]
                 try:
-                    del oldpvdict[f]   # Get rid of the field mapping
-                                       # so we don't disconnect the PV below!
-                except:
+                    del oldpvdict[f]  # Get rid of the field mapping
+                    # so we don't disconnect the PV below!
+                except Exception:
                     pass
                 try:
                     pv = oldpvdict[n]
                     d[f] = pv.value
-                    d['connstat'][ofld['objidx']] = True
+                    d["connstat"][ofld["objidx"]] = True
                     del oldpvdict[n]
-                except:
+                except Exception:
                     d[f] = None
                     pv = utils.monitorPv(n, self.pv_handler)
-                    if ofld['type'] == str:
+                    if ofld["type"] == str:
                         pv.set_string_enum(True)
                 newpvdict[n] = pv
                 newpvdict[f] = pv
                 pv.obj = d
                 pv.fld = f
-        if reduce(lambda a,b: a and b, d['connstat']):
-            del d['connstat']
+        if reduce(lambda a, b: a and b, d["connstat"]):
+            del d["connstat"]
             self.status[idx] = "".join(sorted("C" + self.status[idx]))
             self.statchange(idx)
         self.pvdict[idx] = newpvdict
         for pv in oldpvdict.values():
             try:
                 pv.disconnect()
-            except:
+            except Exception:
                 pass
 
     def connectAllPVs(self):
         for idx in self.rowmap:
             try:
                 self.connectPVs(idx)
-            except:
+            except Exception:
                 pass
 
     def pv_handler(self, pv, e):
         if e is None:
             pv.obj[pv.fld] = pv.value
             change = False
-            v2 = self.getCfg(pv.obj['id'], pv.fld) # Configured value
-            if v2 == None or param.equal(pv.value, v2):
-                if pv.fld in self.istatus[pv.obj['id']]:
-                    self.istatus[pv.obj['id']].remove(pv.fld)
+            v2 = self.getCfg(pv.obj["id"], pv.fld)  # Configured value
+            if v2 is None or param.equal(pv.value, v2):
+                if pv.fld in self.istatus[pv.obj["id"]]:
+                    self.istatus[pv.obj["id"]].remove(pv.fld)
                     change = True
             else:
-                if pv.fld not in self.istatus[pv.obj['id']]:
-                    self.istatus[pv.obj['id']].add(pv.fld)
+                if pv.fld not in self.istatus[pv.obj["id"]]:
+                    self.istatus[pv.obj["id"]].add(pv.fld)
                     change = True
             try:
-                idx = param.params.pobj.fldmap[pv.fld]['objidx']
-                pv.obj['connstat'][idx] = True
-                if reduce(lambda a,b: a and b, pv.obj['connstat']):
-                    del pv.obj['connstat']
-                    self.status[pv.obj['id']] = "".join(sorted("C" + self.status[pv.obj['id']]))
+                idx = param.params.pobj.fldmap[pv.fld]["objidx"]
+                pv.obj["connstat"][idx] = True
+                if reduce(lambda a, b: a and b, pv.obj["connstat"]):
+                    del pv.obj["connstat"]
+                    self.status[pv.obj["id"]] = "".join(
+                        sorted("C" + self.status[pv.obj["id"]])
+                    )
                     change = True
-            except:
+            except Exception:
                 pass
             if change:
-                self.statchange(pv.obj['id'])
+                self.statchange(pv.obj["id"])
             try:
-                index = self.index(self.rowmap.index(pv.obj['id']), idx + self.coff)
-                v = self.data(index) # Just to force a status change!
+                index = self.index(self.rowmap.index(pv.obj["id"]), idx + self.coff)
+                self.data(index)  # Just to force a status change!
                 self.dataChanged.emit(index, index)
-            except:
+            except Exception:
                 pass
 
     def haveNewName(self, idx, name):
         name = str(name)
         utils.fixName(param.params.pobj.objs.values(), idx, name)
         utils.fixName(self.objs.values(), idx, name)
         utils.fixName(self.edits.values(), idx, name)
         for i in range(len(self.rowmap)):
             ii = self.rowmap[i]
             try:
-                if self.edits[ii]['config'] == idx:
-                    self.edits[ii]['cfgname'] = str(name)
+                if self.edits[ii]["config"] == idx:
+                    self.edits[ii]["cfgname"] = str(name)
                     index = self.index(i, self.cfgcol)
                     self.dataChanged.emit(index, index)
-            except:
+            except Exception:
                 d = self.getObj(ii)
-                if d['config'] == idx:
-                    d['cfgname'] = str(name)
+                if d["config"] == idx:
+                    d["cfgname"] = str(name)
                     index = self.index(i, self.cfgcol)
                     self.dataChanged.emit(index, index)
 
     def checkStatus(self, index, vals):
         (idx, f) = self.index2db(index)
         s = self.getStatus(idx)
         for v in vals:
@@ -603,123 +618,181 @@
         return idx >= 0
 
     def haveObjPVDiff(self, index):
         db = param.params.pobj
         try:
             (idx, f) = self.index2db(index)
             flist = [f]
-        except:
+        except Exception:
             idx = self.rowmap[index]
-            flist = [d['fld'] for d in param.params.pobj.objflds if d['obj'] == True]
+            flist = [d["fld"] for d in param.params.pobj.objflds if d["obj"] is True]
         for f in flist:
             if idx < 0:
                 try:
-                    vc = self.objs[idx]['_cfg'][f]
-                except:
+                    vc = self.objs[idx]["_cfg"][f]
+                except Exception:
                     pass
                 try:
                     va = self.objs[idx][f]
-                except:
+                except Exception:
                     pass
             else:
                 try:
                     vc = self.edits[idx][f]
-                except:
+                except Exception:
                     try:
-                        vc = db.objs[idx]['_cfg'][f]
-                    except:
+                        vc = db.objs[idx]["_cfg"][f]
+                    except Exception:
                         return False
                 try:
                     va = db.objs[idx][f]
-                except:
+                except Exception:
                     return False
             try:
-                if db.fldmap[f]['obj'] and not param.equal(va, vc) and vc != None:
+                if db.fldmap[f]["obj"] and not param.equal(va, vc) and vc is not None:
                     return True
-            except:
+            except Exception:
                 pass
         return False
 
     def setupContextMenus(self, table):
         menu = utils.MyContextMenu()
         menu.addAction("Create new object", self.create)
-        menu.addAction("Delete this object", self.delete,
-                       lambda table, index: index.row() >= 0 and self.rowmap[index.row()] != 0 and
-                       not self.checkStatus(index, 'D'))
-        menu.addAction("Undelete this object", self.undelete,
-                       lambda table, index: index.row() >= 0 and self.rowmap[index.row()] != 0 and
-                       self.checkStatus(index, 'D'))
-        menu.addAction("Change configuration", self.chparent,
-                       lambda table, index: self.rowmap[index.row()] != 0 and index.column() == self.cfgcol)
-        menu.addAction("Set field from PV", self.setFromPV,
-                       lambda table, index: index.row() >= 0 and
-                       self.rowmap[index.row()] != 0 and self.haveObjPVDiff(index))
-        menu.addAction("Set object fields from PV", self.setAllFromPV,
-                       lambda table, index: index.row() >= 0 and
-                       self.rowmap[index.row()] != 0 and self.haveObjPVDiff(index.row()))
-        menu.addAction("Create configuration from object", self.createcfg,
-                       lambda table, index: index.row() >= 0 and self.rowmap[index.row()] != 0)
-        menu.addAction("Set configuration from PV", self.modifycfg,
-                       lambda table, index: index.row() >= 0 and self.rowmap[index.row()] != 0)
-        menu.addAction("Set configuration and object fields from PV", self.modifycfgobj,
-                       lambda table, index: index.row() >= 0 and
-                       self.rowmap[index.row()] != 0 and self.savedObj(index) and
-                       self.haveObjPVDiff(index.row()))
-        menu.addAction("Commit this object", self.commitone,
-                       lambda table, index: index.row() >= 0 and self.rowmap[index.row()] != 0 and
-                       self.checkStatus(index, 'DMN'))
-        menu.addAction("Apply to this object", self.applyone,
-                       lambda table, index: index.row() >= 0 and self.rowmap[index.row()] != 0 and
-                       self.checkStatus(index, 'DMNX'))
-        menu.addAction("Revert this object", self.revertone,
-                       lambda table, index: self.checkStatus(index, 'M'))
+        menu.addAction(
+            "Delete this object",
+            self.delete,
+            lambda table, index: index.row() >= 0
+            and self.rowmap[index.row()] != 0
+            and not self.checkStatus(index, "D"),
+        )
+        menu.addAction(
+            "Undelete this object",
+            self.undelete,
+            lambda table, index: index.row() >= 0
+            and self.rowmap[index.row()] != 0
+            and self.checkStatus(index, "D"),
+        )
+        menu.addAction(
+            "Change configuration",
+            self.chparent,
+            lambda table, index: self.rowmap[index.row()] != 0
+            and index.column() == self.cfgcol,
+        )
+        menu.addAction(
+            "Set field from PV",
+            self.setFromPV,
+            lambda table, index: index.row() >= 0
+            and self.rowmap[index.row()] != 0
+            and self.haveObjPVDiff(index),
+        )
+        menu.addAction(
+            "Set object fields from PV",
+            self.setAllFromPV,
+            lambda table, index: index.row() >= 0
+            and self.rowmap[index.row()] != 0
+            and self.haveObjPVDiff(index.row()),
+        )
+        menu.addAction(
+            "Create configuration from object",
+            self.createcfg,
+            lambda table, index: index.row() >= 0 and self.rowmap[index.row()] != 0,
+        )
+        menu.addAction(
+            "Set configuration from PV",
+            self.modifycfg,
+            lambda table, index: index.row() >= 0 and self.rowmap[index.row()] != 0,
+        )
+        menu.addAction(
+            "Set configuration and object fields from PV",
+            self.modifycfgobj,
+            lambda table, index: index.row() >= 0
+            and self.rowmap[index.row()] != 0
+            and self.savedObj(index)
+            and self.haveObjPVDiff(index.row()),
+        )
+        menu.addAction(
+            "Commit this object",
+            self.commitone,
+            lambda table, index: index.row() >= 0
+            and self.rowmap[index.row()] != 0
+            and self.checkStatus(index, "DMN"),
+        )
+        menu.addAction(
+            "Apply to this object",
+            self.applyone,
+            lambda table, index: index.row() >= 0
+            and self.rowmap[index.row()] != 0
+            and self.checkStatus(index, "DMNX"),
+        )
+        menu.addAction(
+            "Revert this object",
+            self.revertone,
+            lambda table, index: self.checkStatus(index, "M"),
+        )
         table.addContextMenu(menu)
         colmgr.addColumnManagerMenu(table)
-    
+
     def setFromPV(self, table, index):
         (idx, f) = self.index2db(index)
         if idx >= 0:
             self.setData(index, param.params.pobj.objs[idx][f])
         else:
             self.setData(index, self.objs[idx][f])
 
     def setAllFromPV(self, table, index):
         db = param.params.pobj
         (idx, f) = self.index2db(index)
-        flist = [(d['fld'], self.coff + d['objidx']) for d in param.params.pobj.objflds if d['obj'] == True]
-        for (f, c) in flist:
+        flist = [
+            (d["fld"], self.coff + d["objidx"])
+            for d in param.params.pobj.objflds
+            if d["obj"] is True
+        ]
+        for f, c in flist:
             if idx >= 0:
                 va = param.params.pobj.objs[idx][f]
                 try:
                     vc = self.edits[idx][f]
-                except:
-                    vc = db.objs[idx]['_cfg'][f]
+                except Exception:
+                    vc = db.objs[idx]["_cfg"][f]
             else:
                 va = self.objs[idx][f]
-                vc = self.objs[idx]['_cfg'][f]
-            if vc != None:
+                vc = self.objs[idx]["_cfg"][f]
+            if vc is not None:
                 self.setData(self.index(index.row(), c), va)
-        
+
     def create(self, table, index):
-        idx = self.nextid;
+        idx = self.nextid
         self.nextid -= 1
         now = datetime.datetime.now()
         d = dict(param.params.pobj.objs[0])
-        del d['_cfg']
-        del d['connstat']
-        dd = {'id': idx, 'config': 0, 'owner': param.params.hutch, 
-              'rec_base': "DUMMY:"+str(-idx), 'dt_created': now, 'dt_updated': now, 'category': 'Manual',
-              'cfgname': param.params.db.getCfgName(0) }
+        del d["_cfg"]
+        del d["connstat"]
+        dd = {
+            "id": idx,
+            "config": 0,
+            "owner": param.params.hutch,
+            "rec_base": "DUMMY:" + str(-idx),
+            "dt_created": now,
+            "dt_updated": now,
+            "category": "Manual",
+            "cfgname": param.params.db.getCfgName(0),
+        }
         d.update(dd)
         self.status[idx] = "N"
-        self.istatus[idx] = set([])
-        d['_cfg'] = dict(d)
+        self.istatus[idx] = set()
+        d["_cfg"] = dict(d)
         self.objs[idx] = d
         self.rowmap.append(idx)
         self.adjustSize()
+        ni = self.rowmap.index(idx)
+        # Sigh. 0 doesn't work because of a decision in FreezeTableView.
+        newidx = self.index(ni, 1)
+        param.params.ui.objectTable.setCurrentIndex(newidx)
+        param.params.ui.objectTable.scrollTo(newidx,
+                                             QtWidgets.QAbstractItemView.EnsureVisible)
 
     def adjustSize(self):
         self.setRowCount(len(self.rowmap))
         lastsort = self.lastsort
         self.lastsort = (None, None)
         self.sort(lastsort[0], lastsort[1])
 
@@ -731,17 +804,25 @@
     # do modifycfg and setFromPV!
     def modifycfgobj(self, table, index):
         self.setAllFromPV(table, index)
         self.modifycfg(table, index)
 
     def createcfg(self, table, index):
         (idx, f) = self.index2db(index)
-        if (param.params.cfgdialog.exec_("Select parent configuration for configuration of %s" % self.getObjName(idx), 0)
-            == QtWidgets.QDialog.Accepted):
-            v = param.params.cfgmodel.create_child(param.params.cfgdialog.result, self.getObj(idx), True)
+        if (
+            param.params.cfgdialog.exec_(
+                "Select parent configuration for configuration of %s"
+                % self.getObjName(idx),
+                0,
+            )
+            == QtWidgets.QDialog.Accepted
+        ):
+            v = param.params.cfgmodel.create_child(
+                param.params.cfgdialog.result, self.getObj(idx), True
+            )
             self.setCfg(idx, v)
 
     def delete(self, table, index):
         (idx, f) = self.index2db(index)
         if idx >= 0:
             self.status[idx] = "".join(sorted("D" + self.status[idx]))
             self.statchange(idx)
@@ -756,29 +837,29 @@
         (idx, f) = self.index2db(index)
         self.status[idx] = self.status[idx].replace("D", "")
         self.statchange(idx)
 
     def checkSetMutex(self, d, e):
         for s in param.params.pobj.setflds:
             f = param.params.pobj.fldmap[s[0]]
-            if not f['setmutex'] or not f['obj']:
+            if not f["setmutex"] or not f["obj"]:
                 continue
             try:
-                z = f['enum'][0]
-            except:
+                z = f["enum"][0]
+            except Exception:
                 z = 0
             vlist = []
             for f in s:
                 try:
                     v = e[f]
-                except:
+                except Exception:
                     v = d[f]
-                if v != None and not param.equal(v, z):
+                if v is not None and not param.equal(v, z):
                     if v in vlist:
-                        return [param.params.pobj.fldmap[f]['alias'] for f in s]
+                        return [param.params.pobj.fldmap[f]["alias"] for f in s]
                     else:
                         vlist.append(v)
         return []
 
     def commit(self, idx):
         """
         Try to commit a change.  We assume we are in a transaction already.
@@ -790,51 +871,59 @@
 
         Returns
         -------
         Nothing.
         """
         d = self.getObj(idx)
         try:
-            name = self.edits[idx]['rec_base']
-        except:
-            name = d['rec_base']
+            name = self.edits[idx]["rec_base"]
+        except Exception:
+            name = d["rec_base"]
         if not utils.permission():
             param.params.pobj.transaction_error("Not Authorized to Change %s!" % name)
             return
         if name[0:10] == "":
             param.params.pobj.transaction_error("PV Base cannot be null!")
             return
-        if 'D' in self.status[idx]:
+        if "D" in self.status[idx]:
             param.params.pobj.objectDelete(idx)
         else:
             try:
                 e = self.edits[idx]
-            except:
+            except Exception:
                 e = {}
             try:
-                if e['config'] < 0:
+                if e["config"] < 0:
                     try:
-                        if param.params.db.cfgmap[e['config']] < 0:
+                        if param.params.db.cfgmap[e["config"]] < 0:
                             raise Exception
-                    except:
-                        param.params.pobj.transaction_error("New configuration must be committed before committing %s!" % name)
+                    except Exception:
+                        param.params.pobj.transaction_error(
+                            "New configuration must be committed before committing %s!"
+                            % name
+                        )
                         return
-            except:
+            except Exception:
                 pass
             s = self.checkSetMutex(d, e)
             if s != []:
-                param.params.pobj.transaction_error("Object %s does not have unique values for %s!" % 
-                                                    (name, str(s)))
+                param.params.pobj.transaction_error(
+                    "Object %s does not have unique values for %s!" % (name, str(s))
+                )
                 return
-            if 'N' in self.status[idx]:
-                newidx = param.params.pobj.objectInsert(param.params.db.doMap(self.getObj(idx)['_cfg']))
-                if newidx != None:
+            if "N" in self.status[idx]:
+                newidx = param.params.pobj.objectInsert(
+                    param.params.db.doMap(self.getObj(idx)["_cfg"])
+                )
+                if newidx is not None:
                     param.params.db.addObjmap(idx, newidx)
-            elif 'M' in self.status[idx]:
-                param.params.pobj.objectChange(idx, param.params.db.doMap(self.edits[idx]))
+            elif "M" in self.status[idx]:
+                param.params.pobj.objectChange(
+                    idx, param.params.db.doMap(self.edits[idx])
+                )
 
     #
     # Note: this calls commit (and checks permissions!) even if no change!
     #
     def commitone(self, table, index):
         param.params.db.start_transaction()
         (idx, f) = self.index2db(index)
@@ -848,20 +937,22 @@
     #
     # Note: this only calls commit for changes!
     #
     def commitall(self):
         if not param.params.cfgmodel.confirmCommit():
             return False
         param.params.db.start_transaction()
-        for (idx, s) in self.status.items():
-            if 'D' in s:
+        for idx, s in self.status.items():
+            if "D" in s:
                 self.commit(idx)
         param.params.cfgmodel.commitall(False)
-        for (idx, s) in self.status.items():
-            if ('N' in s or 'M' in s) and not 'D' in s:  # Paranoia.  We should never have DM or DN.
+        for idx, s in self.status.items():
+            if (
+                "N" in s or "M" in s
+            ) and "D" not in s:  # Paranoia.  We should never have DM or DN.
                 self.commit(idx)
         if param.params.db.end_transaction():
             param.params.cfgmodel.cfgChangeDone()
             self.objChangeDone()
             return True
         else:
             return False
@@ -876,202 +967,211 @@
 
     def apply(self, idx):
         d = self.getObj(idx)
         pvd = self.pvdict[idx]
         for s in param.params.pobj.setflds:
             for f in s:
                 fm = param.params.pobj.fldmap[f]
-                if fm['readonly']:
+                if fm["readonly"]:
                     continue
-                if fm['writezero']:
+                if fm["writezero"]:
                     try:
-                        v = d[f]             # PV value
-                    except:
+                        v = d[f]  # PV value
+                    except Exception:
                         continue
-                    v2 = self.getCfg(idx, f) # Configured value
+                    v2 = self.getCfg(idx, f)  # Configured value
                     #
                     # Write a value if:
                     #     1. It's not derived (the value isn't None), and either
                     #     2a. It's a change, or
                     #     2b. It's a "must write" value.
                     #
-                    if v2 != None and (not param.equal(v, v2) or fm['mustwrite']):
+                    if v2 is not None and (not param.equal(v, v2) or fm["mustwrite"]):
                         try:
-                            z = fm['enum'][0]
-                        except:
+                            z = fm["enum"][0]
+                        except Exception:
                             z = 0
                         try:
                             pv = pvd[f]
                             if param.params.debug:
-                                print("Put %s to %s" % (str(z), pv.name))
+                                print("Put {} to {}".format(str(z), pv.name))
                             else:
                                 pv.put(z, timeout=-1.0)
-                        except:
+                        except Exception:
                             pass
             pyca.flush_io()
             for f in s:
                 fm = param.params.pobj.fldmap[f]
-                if fm['readonly']:
+                if fm["readonly"]:
                     continue
                 try:
-                    v = d[f]             # PV value
-                except:
+                    v = d[f]  # PV value
+                except Exception:
                     continue
-                v2 = self.getCfg(idx, f) # Configured value
-                if v2 != None and (not param.equal(v, v2) or fm['mustwrite']):
+                v2 = self.getCfg(idx, f)  # Configured value
+                if v2 is not None and (not param.equal(v, v2) or fm["mustwrite"]):
                     try:
                         pv = pvd[f]
                         if param.params.debug:
-                            print("Put %s to %s" % (str(v2), pv.name))
+                            print("Put {} to {}".format(str(v2), pv.name))
                         else:
                             pv.put(v2, timeout=-1.0)
-                    except:
+                    except Exception:
                         pass
             pyca.flush_io()
 
     #
     # Note: commitone always calls commit, and that does the permission check!
     #
     def applyone(self, table, index):
         if self.commitone(table, index):
             (idx, f) = self.index2db(index)
             self.apply(idx)
 
     def applyVerify(self, changes):
-        d = QtWidgets.QDialog();
+        d = QtWidgets.QDialog()
         d.setWindowTitle("Apply Confirmation")
         d.layout = QtWidgets.QVBoxLayout(d)
         d.mlabel = QtWidgets.QLabel(d)
         d.mlabel.setText("Apply will modify settings on the following motors:")
         d.layout.addWidget(d.mlabel)
         d.checks = []
         for idx in changes:
             check = QtWidgets.QCheckBox(d)
             check.setChecked(True)
             check.setText(self.getObjName(idx))
             d.layout.addWidget(check)
             d.checks.append(check)
         d.buttonBox = QtWidgets.QDialogButtonBox(d)
         d.buttonBox.setOrientation(QtCore.Qt.Horizontal)
-        d.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Ok)
+        d.buttonBox.setStandardButtons(
+            QtWidgets.QDialogButtonBox.Cancel | QtWidgets.QDialogButtonBox.Ok
+        )
         d.layout.addWidget(d.buttonBox)
         d.buttonBox.accepted.connect(d.accept)
         d.buttonBox.rejected.connect(d.reject)
         if d.exec_() == QtWidgets.QDialog.Accepted:
-            checks =  [c.isChecked() for c in d.checks]
+            checks = [c.isChecked() for c in d.checks]
             return [changes[i] for i in range(len(changes)) if checks[i]]
         else:
             return []
 
-
     #
     # If there are no changes, commitall does not do a permission check, so we need
     # to do one.
     #
     def applyall(self):
         if not self.commitall():
             return
         if not utils.permission():
-            QtWidgets.QMessageBox.critical(None, "Error", "Not authorized to apply changes!",
-                                       QtWidgets.QMessageBox.Ok)
+            QtWidgets.QMessageBox.critical(
+                None,
+                "Error",
+                "Not authorized to apply changes!",
+                QtWidgets.QMessageBox.Ok,
+            )
             return
         changes = [idx for idx in self.rowmap if "X" in self.getStatus(idx)]
         changes = self.applyVerify(changes)
         for idx in changes:
             self.apply(idx)
 
     def revertone(self, table, index):
         (idx, f) = self.index2db(index)
         try:
-            if 'config' in self.edits[idx].keys():
-                self.setCfg(idx, self.getObj(idx)['config'])
+            if "config" in self.edits[idx].keys():
+                self.setCfg(idx, self.getObj(idx)["config"])
             del self.edits[idx]
-        except:
+        except Exception:
             pass
         self.status[idx] = self.status[idx].replace("M", "")
         row = self.rowmap.index(idx)
         self.dataChanged.emit(self.index(row, 0), self.index(row, self.colcnt - 1))
 
     def objChangeDone(self, idx=None):
-        if idx != None:
+        if idx is not None:
             try:
                 del self.edits[idx]
-            except:
+            except Exception:
                 pass
             if idx < 0:
                 del self.objs[idx]
                 del self.status[idx]
                 del self.istatus[idx]
             else:
-                if 'C' in self.status[idx]:
+                if "C" in self.status[idx]:
                     self.status[idx] = "C"
                 else:
                     self.status[idx] = ""
                 self.statchange(idx)
             self.rowmap = list(param.params.pobj.objs.keys())
             self.rowmap[:0] = self.objs.keys()
         else:
             self.edits = {}
             self.objs = {}
             snew = {}
             for k in self.status.keys():
                 if k < 0:
                     del self.istatus[k]
                 else:
-                    if 'C' in self.status[k]:
+                    if "C" in self.status[k]:
                         snew[k] = "C"
                     else:
                         snew[k] = ""
                     self.statchange(k)
             self.status = snew
             self.rowmap = list(param.params.pobj.objs.keys())
         self.adjustSize()
 
     def setCfg(self, idx, cfg):
-        self.setValue(idx, 'cfgname', cfg)
+        self.setValue(idx, "cfgname", cfg)
         acts = self.getObj(idx)
-        flist = [d['fld'] for d in param.params.pobj.objflds]
+        flist = [d["fld"] for d in param.params.pobj.objflds]
         for f in flist:
             v = acts[f]
-            v2 = self.getCfg(idx, f) # Configured value
-            if v == None or v2 == None or param.equal(v, v2):
+            v2 = self.getCfg(idx, f)  # Configured value
+            if v is None or v2 is None or param.equal(v, v2):
                 try:
                     self.istatus[idx].remove(f)
-                except:
+                except Exception:
                     pass
             else:
                 self.istatus[idx].add(f)
         r = self.rowmap.index(idx)
         self.dataChanged.emit(self.index(r, 0), self.index(r, self.colcnt - 1))
 
     def chparent(self, table, index):
         (idx, f) = self.index2db(index)
         d = self.getObj(idx)
-        if (param.params.cfgdialog.exec_("Select new configuration for %s" % d['rec_base'], d['config']) ==
-            QtWidgets.QDialog.Accepted):
+        if (
+            param.params.cfgdialog.exec_(
+                "Select new configuration for %s" % d["rec_base"], d["config"]
+            )
+            == QtWidgets.QDialog.Accepted
+        ):
             self.setCfg(idx, param.params.cfgdialog.result)
 
     def cfgEdit(self, idx, f):
         f = str(f)
-        if f == 'cfgname':
+        if f == "cfgname":
             c1 = 0
             c2 = self.colcnt - 1
         else:
             try:
-                c1 = self.coff + param.params.pobj.fldmap[f]['objidx']
+                c1 = self.coff + param.params.pobj.fldmap[f]["objidx"]
                 c2 = c1
-            except:
+            except Exception:
                 # We shouldn't be here.
                 return
         for i in range(len(self.rowmap)):
             id = self.rowmap[i]
             try:
-                cfg = self.edits[id]['config']
-            except:
-                cfg = self.getObj(id)['config']
+                cfg = self.edits[id]["config"]
+            except Exception:
+                cfg = self.getObj(id)["config"]
             if cfg == idx:
                 self.dataChanged.emit(self.index(i, c1), self.index(i, c2))
 
     # Enabled:
     #     Everything.
     # Selectable:
     #     QtCore.Qt.ItemIsSelectable
@@ -1082,127 +1182,140 @@
     #
     def flags(self, index):
         flags = QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsSelectable
         if index.isValid():
             (idx, f) = self.index2db(index)
             col = index.column()
             if col < self.coff:
-                if idx != 0 and not f in self.fixflds:
+                if idx != 0 and f not in self.fixflds:
                     flags = flags | QtCore.Qt.ItemIsEditable
             else:
-                if (idx != 0 and param.params.pobj.objflds[col-self.coff]['obj'] and
-                    not param.params.pobj.objflds[col-self.coff]['readonly']):
+                if (
+                    idx != 0
+                    and param.params.pobj.objflds[col - self.coff]["obj"]
+                    and not param.params.pobj.objflds[col - self.coff]["readonly"]
+                ):
                     flags = flags | QtCore.Qt.ItemIsEditable
         return flags
 
     def editorInfo(self, index):
         c = index.column()
         if c == self.catcol:
             return param.params.catenum2
         if c < self.coff:
             return str
         try:
-            return param.params.pobj.objflds[c - self.coff]['enum']
-        except:
-            return param.params.pobj.objflds[c - self.coff]['type']
+            return param.params.pobj.objflds[c - self.coff]["enum"]
+        except Exception:
+            return param.params.pobj.objflds[c - self.coff]["type"]
 
     def doShow(self):
         ui = param.params.ui
         v = []
         if ui.actionManual.isChecked():
             v.append("Manual")
         if ui.actionProtected.isChecked():
             v.append("Protected")
         for i in range(len(self.rowmap)):
             # Sometimes, we get a little ahead of ourselves after a deletion and this fails.
             # However, we'll get the *real* update soon enough, so just stop the error.
             try:
-                if self.rowmap[i] == 0 or self.getCfg(self.rowmap[i], 'category', True) in v:
+                if (
+                    self.rowmap[i] == 0
+                    or self.getCfg(self.rowmap[i], "category", True) in v
+                ):
                     param.params.ui.objectTable.setRowHidden(i, False)
                 else:
                     param.params.ui.objectTable.setRowHidden(i, True)
-            except:
+            except Exception:
                 pass
 
     def doShowAll(self):
         for i in range(len(self.rowmap)):
             param.params.ui.objectTable.setRowHidden(i, False)
 
     def doTrack(self):
         self.track = param.params.ui.actionTrack.isChecked()
         if self.track and self.selrow >= 0:
-            param.params.cfgmodel.selectConfig(self.getCfg(self.rowmap[self.selrow], 'config', True))
+            param.params.cfgmodel.selectConfig(
+                self.getCfg(self.rowmap[self.selrow], "config", True)
+            )
 
     def selectionChanged(self, selected, deselected):
         if not selected.isEmpty():
-            i = selected.indexes()[0];
+            i = selected.indexes()[0]
             self.selrow = i.row()
         else:
             self.selrow = -1
         if self.track and self.selrow >= 0:
-            param.params.cfgmodel.selectConfig(self.getCfg(self.rowmap[self.selrow], 'config', True))
+            param.params.cfgmodel.selectConfig(
+                self.getCfg(self.rowmap[self.selrow], "config", True)
+            )
 
     def getObjSel(self):
         ui = param.params.ui
         d = {True: "1", False: "0"}
         v = ""
-        v += "0"             # actionAuto is deprecated, but still takes space!
+        v += "0"  # actionAuto is deprecated, but still takes space!
         v += d[ui.actionProtected.isChecked()]
         v += d[ui.actionManual.isChecked()]
         v += d[ui.actionTrack.isChecked()]
         return v
 
     def setObjSel(self, v):
-        if v != "" and v != None:
+        if v != "" and v is not None:
             ui = param.params.ui
-            d = {"1" : True, "0": False}
+            d = {"1": True, "0": False}
             ui.actionProtected.setChecked(d[v[1]])
             ui.actionManual.setChecked(d[v[2]])
             ui.actionTrack.setChecked(d[v[3]])
             self.doShow()
             self.doTrack()
 
     def getObjName(self, idx):
         try:
-            return self.edits[idx]['rec_base']
-        except:
-            return self.getObj(idx)['rec_base']
+            return self.edits[idx]["rec_base"]
+        except Exception:
+            return self.getObj(idx)["rec_base"]
 
     def getObjList(self, types=None):
-        if types == None:
+        if types is None:
             types = param.params.catenum
-        return [self.getObjName(idx) for idx in self.rowmap
-                if self.getCfg(idx, 'category', True) in types]
+        return [
+            self.getObjName(idx)
+            for idx in self.rowmap
+            if self.getCfg(idx, "category", True) in types
+        ]
 
     def getObjId(self, name):
         for i in self.rowmap:
             if self.getObjName(i) == name:
                 return i
         return 0
 
     def cfgrenumber(self, old, new):
         for d in self.edits.values():
             try:
-                if d['config'] == old:
-                    d['config'] = new
-            except:
+                if d["config"] == old:
+                    d["config"] = new
+            except Exception:
                 pass
         for d in self.objs.values():
-            if d['config'] == old:
-                d['config'] = new
+            if d["config"] == old:
+                d["config"] = new
 
     #
     # Check if the configuration idx is in use: either as an edit or as a database value.
-    #    
+    #
     def configInUse(self, idx):
-        for (k, v) in param.params.pobj.objs.items():
+        for k, v in param.params.pobj.objs.items():
             try:
-                if self.edits[k]['config'] == idx:
+                if self.edits[k]["config"] == idx:
                     return True
-            except:
+            except Exception:
                 pass
-            if v['config'] == idx:
+            if v["config"] == idx:
                 return True
-        for (k, v) in self.objs.items():
-            if v['config'] == idx:
+        for k, v in self.objs.items():
+            if v["config"] == idx:
                 return True
         return False
```

### Comparing `pmgr-2.0.2/pmgr/colmgr.py` & `pmgr-2.1.3/pmgr/colmgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,111 +1,119 @@
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt5 import QtCore, QtWidgets
 
-from . import utils
-from . import param
-from . import colchoose_ui
+from . import param, utils
+from .dialogs import load_ui_file
 
 #
 # This is an attempt at a general purpose column manager for QTableViews.
 # We have added a save/restoreHeaderState function to our FreezeTableView,
 # because our headers are special.  In general though, we could just
 # access the header's restoreState function directly here.
 #
 # We assume that the QTableView has an additional property, colmgr,
 # that points to the group in which the settings should be saved/restored
 # in our QSettings.  The QSettings parameters are in param.params.settings.
 #
 
-def addColumnManagerMenu(table, extra = [], hideOK=True, cfgOK=True):
+
+def addColumnManagerMenu(table, extra=[], hideOK=True, cfgOK=True):
     menu = utils.MyContextMenu()
     if hideOK:
-        menu.addAction("Hide column",        hidecol)
-        menu.addAction("Reset columns",      resetcol)
+        menu.addAction("Hide column", hidecol)
+        menu.addAction("Reset columns", resetcol)
         menu.addAction("Run column chooser", choosecol)
-    menu.addAction("Autosize columns",   sizecol)
+    menu.addAction("Autosize columns", sizecol)
     if cfgOK:
         menu.addAction("Save column config", savecol)
-        menu.addAction("Use column config",  restorecol)
-    for (t, f) in extra:
+        menu.addAction("Use column config", restorecol)
+    for t, f in extra:
         menu.addAction(t, f)
     table.addHeaderContextMenu(menu)
 
+
 def hidecol(table, index):
     table.horizontalHeader().hideSection(index)
-    
+
+
 def resetcol(table, index):
     for i in range(table.model().columnCount()):
         if table.isColumnHidden(i):
             table.showColumn(i)
     h = table.horizontalHeader()
     for i in range(table.model().columnCount()):
         if h.visualIndex(i) != i:
             h.moveSection(h.visualIndex(i), i)
 
+
 def sizecol(table, index):
     table.resizeColumnsToContents()
 
+
 def choosecol(table, index):
     m = table.model()
     h = table.horizontalHeader()
     try:
         d = m.colchoosedialog
-    except:
+    except Exception:
         d = QtWidgets.QDialog()
-        d.ui = colchoose_ui.Ui_Dialog()
+        d.ui = load_ui_file("colchoose.ui")()
         d.ui.setupUi(d)
         c = []
         for i in range(m.mutable):
             c.append(None)
         for i in range(m.mutable, m.columnCount()):
             cb = QtWidgets.QCheckBox(d)
             cb.setText(m.horizontalHeaderItem(i).text())
             c.append(cb)
             d.ui.gridLayout.addWidget(cb, (i - m.mutable) / 5, (i - m.mutable) % 5)
-        d.ui.allButton.clicked.connect(lambda : doAllButton(d))
-        d.ui.noneButton.clicked.connect(lambda : doNoneButton(d))
+        d.ui.allButton.clicked.connect(lambda: doAllButton(d))
+        d.ui.noneButton.clicked.connect(lambda: doNoneButton(d))
         d.cols = c
-        d.resize(0,0)
+        d.resize(0, 0)
         m.colchoosedialog = d
     c = d.cols
     for i in range(m.mutable, m.columnCount()):
         c[i].setChecked(not h.isSectionHidden(i))
     if d.exec_() == QtWidgets.QDialog.Accepted:
         for i in range(m.mutable, m.columnCount()):
             if c[i].isChecked():
                 h.showSection(i)
             else:
                 h.hideSection(i)
 
+
 def doAllButton(d):
     for c in d.cols:
-        if c != None:
+        if c is not None:
             c.setChecked(True)
 
+
 def doNoneButton(d):
     for c in d.cols:
-        if c != None:
+        if c is not None:
             c.setChecked(False)
 
+
 def savecol(table, index):
     d = param.params.colsavedialog
     d.ui.lineEdit.setText("")
     if d.exec_() == QtWidgets.QDialog.Accepted:
         cfg = str(d.ui.lineEdit.text())
         if cfg == "":
             # Complain!
             return
         settings = QtCore.QSettings(param.params.settings[0], param.params.settings[1])
         settings.beginGroup(table.colmgr)
         settings.setValue(cfg, table.saveHeaderState())
-    
+
+
 def restorecol(table, index):
     settings = QtCore.QSettings(param.params.settings[0], param.params.settings[1])
     settings.beginGroup(table.colmgr)
-    d = param.params.colusedialog;
+    d = param.params.colusedialog
     d.ui.comboBox.clear()
     for x in list(settings.childKeys()):
         d.ui.comboBox.addItem(x)
     if d.exec_() == QtWidgets.QDialog.Accepted:
         cfg = str(d.ui.comboBox.currentText())
         v = settings.value(cfg)
         if v is not None:
```

### Comparing `pmgr-2.0.2/pmgr/db.py` & `pmgr-2.1.3/pmgr/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import threading
 import time
-import sys
 
 from PyQt5 import QtCore
 
+from . import dialogs, param
 from .pmgrobj import pmgrobj
-from . import dialogs
-from . import param
 
 
 class dbPoll(threading.Thread):
-    
     def __init__(self, sig, interval):
-        super(dbPoll, self).__init__()
+        super().__init__()
         self.sig = sig
         self.interval = interval
         self.daemon = True
         self.armed = True
 
     def run(self):
         last = 0
@@ -29,79 +26,83 @@
             else:
                 last = now
             v = param.params.pobj.checkForUpdate()
             if v != 0 and self.armed:
                 self.armed = False
                 self.sig.emit(v)
 
+
 class db(QtCore.QObject):
-    cfgchange     = QtCore.pyqtSignal()
-    objchange     = QtCore.pyqtSignal()
-    readsig       = QtCore.pyqtSignal(int)
+    cfgchange = QtCore.pyqtSignal()
+    objchange = QtCore.pyqtSignal()
+    readsig = QtCore.pyqtSignal(int)
 
     def __init__(self):
-        super(db, self).__init__()
+        super().__init__()
         self.nameedits = {}
         self.errordialog = dialogs.errordialog()
-        param.params.pobj = pmgrobj(param.params.table, param.params.hutch, 
-                                    debug=param.params.debug, 
-                                    prod=param.params.prod)
+        param.params.pobj = pmgrobj(
+            param.params.table,
+            param.params.hutch,
+            debug=param.params.debug,
+            prod=param.params.prod,
+        )
         self.poll = None
         self.readTables()
         self.readsig.connect(self.readTables)
         self.poll = dbPoll(self.readsig, 5)
         self.poll.start()
         self.cfgmap = {}
         self.objmap = {}
 
     def setCfgName(self, id, name):
         try:
-            if param.params.pobj.cfgs[id]['name'] == name:
-                del self.nameedits[id]['name']
+            if param.params.pobj.cfgs[id]["name"] == name:
+                del self.nameedits[id]["name"]
             else:
                 self.nameedits[id] = name
-        except:
+        except Exception:
             self.nameedits[id] = name
 
     def getCfgName(self, id):
         try:
             return self.nameedits[id]
-        except:
-            return param.params.pobj.cfgs[id]['name']
+        except Exception:
+            return param.params.pobj.cfgs[id]["name"]
 
     def getCfgId(self, name):
         for k, v in self.nameedits.items():
             if v == name:
                 return k
         for k, v in param.params.pobj.cfgs.items():
-            if v['name'] == name:
-                return v['id']
+            if v["name"] == name:
+                return v["id"]
         return None
 
     def setCfgNames(self, l):
         for o in l:
-            c = o['config']
-            if c == None:
-                o['cfgname'] = ""
+            c = o["config"]
+            if c is None:
+                o["cfgname"] = ""
             else:
-                o['cfgname'] = self.getCfgName(c)
+                o["cfgname"] = self.getCfgName(c)
 
     def readTables(self, mask=None, nosig=False):
-        if mask == None:
-            mask=param.params.pobj.DB_ALL
+        if mask is None:
+            mask = param.params.pobj.DB_ALL
         mask = param.params.pobj.updateTables(mask)
         if mask == 0:
             return
         if (mask & param.params.pobj.DB_CONFIG) != 0:
             self.setCfgNames(param.params.pobj.cfgs.values())
         if (mask & param.params.pobj.DB_OBJECT) != 0:
             # ObjModel keeps actual (PV) values in this dictionary, so
             # we keep the configured values in a subdictionary.
             for o in param.params.pobj.objs.values():
-                o['_cfg'] = dict(o)
+                o["_cfg"] = dict(o)
             self.setCfgNames(param.params.pobj.objs.values())
         if not nosig:
             if (mask & param.params.pobj.DB_CONFIG) != 0:
                 self.cfgchange.emit()
             if (mask & param.params.pobj.DB_OBJECT) != 0:
                 self.objchange.emit()
         if self.poll is not None:
@@ -134,44 +135,43 @@
         self.cfgmap[old] = new
 
     def addObjmap(self, old, new):
         self.objmap[old] = new
 
     def doMap(self, d):
         try:
-            oldcfg = d['config']
+            oldcfg = d["config"]
             newcfg = self.cfgmap[oldcfg]
             dd = {}
             dd.update(d)
-            dd['config'] = newcfg
+            dd["config"] = newcfg
             d = dd
-        except:
+        except Exception:
             pass
         try:
-            oldport = d['port']
+            oldport = d["port"]
             newport = self.objmap[oldport]
             dd = {}
             dd.update(d)
-            dd['port'] = newport
+            dd["port"] = newport
             d = dd
-        except:
+        except Exception:
             pass
         return d
 
     def applyCfgMap(self, obj):
-        for (old, new) in self.cfgmap.items():
+        for old, new in self.cfgmap.items():
             obj.cfgrenumber(old, new)
 
     def applyObjMap(self, obj):
-        for (old, new) in self.objmap.items():
+        for old, new in self.objmap.items():
             obj.objrenumber(old, new)
 
     def applyMaps(self):
         self.applyCfgMap(param.params.cfgmodel)
         self.applyCfgMap(param.params.objmodel)
 
     def cfgIsValid(self, id):
         return id >= 0 or id in self.cfgmap.keys()
 
     def objIsValid(self, id):
         return id >= 0 or id in self.objmap.keys()
-
```

### Comparing `pmgr-2.0.2/pmgr/docopt.py` & `pmgr-2.1.3/pmgr/docopt.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,57 +2,55 @@
 
  * http://docopt.org
  * Repository and issue-tracker: https://github.com/docopt/docopt
  * Licensed under terms of MIT license (see LICENSE-MIT)
  * Copyright (c) 2013 Vladimir Keleshev, vladimir@keleshev.com
 
 """
-import sys
 import re
+import sys
 
-
-__all__ = ['docopt']
-__version__ = '0.6.2'
+__all__ = ["docopt"]
+__version__ = "0.6.2"
 
 
 class DocoptLanguageError(Exception):
 
     """Error in construction of usage-message by developer."""
 
 
 class DocoptExit(SystemExit):
 
     """Exit in case user invoked program with incorrect arguments."""
 
-    usage = ''
+    usage = ""
 
-    def __init__(self, message=''):
-        SystemExit.__init__(self, (message + '\n' + self.usage).strip())
+    def __init__(self, message=""):
+        SystemExit.__init__(self, (message + "\n" + self.usage).strip())
 
 
-class Pattern(object):
-
+class Pattern:
     def __eq__(self, other):
         return repr(self) == repr(other)
 
     def __hash__(self):
         return hash(repr(self))
 
     def fix(self):
         self.fix_identities()
         self.fix_repeating_arguments()
         return self
 
     def fix_identities(self, uniq=None):
         """Make pattern-tree tips point to same object if they are equal."""
-        if not hasattr(self, 'children'):
+        if not hasattr(self, "children"):
             return self
         uniq = list(set(self.flat())) if uniq is None else uniq
         for i, child in enumerate(self.children):
-            if not hasattr(child, 'children'):
+            if not hasattr(child, "children"):
                 assert child in uniq
                 self.children[i] = uniq[uniq.index(child)]
             else:
                 child.fix_identities(uniq)
 
     def fix_repeating_arguments(self):
         """Fix elements that should accumulate/increment values."""
@@ -100,32 +98,31 @@
 
     """Leaf/terminal node of a pattern tree."""
 
     def __init__(self, name, value=None):
         self.name, self.value = name, value
 
     def __repr__(self):
-        return '%s(%r, %r)' % (self.__class__.__name__, self.name, self.value)
+        return "{}({!r}, {!r})".format(self.__class__.__name__, self.name, self.value)
 
     def flat(self, *types):
         return [self] if not types or type(self) in types else []
 
     def match(self, left, collected=None):
         collected = [] if collected is None else collected
         pos, match = self.single_match(left)
         if match is None:
             return False, left, collected
-        left_ = left[:pos] + left[pos + 1:]
+        left_ = left[:pos] + left[pos + 1 :]
         same_name = [a for a in collected if a.name == self.name]
         if type(self.value) in (int, list):
             if type(self.value) is int:
                 increment = 1
             else:
-                increment = ([match.value] if type(match.value) is str
-                             else match.value)
+                increment = [match.value] if type(match.value) is str else match.value
             if not same_name:
                 match.value = increment
                 return True, left_, collected + [match]
             same_name[0].value += increment
             return True, left_, collected
         return True, left_, collected + [match]
 
@@ -134,121 +131,117 @@
 
     """Branch/inner node of a pattern tree."""
 
     def __init__(self, *children):
         self.children = list(children)
 
     def __repr__(self):
-        return '%s(%s)' % (self.__class__.__name__,
-                           ', '.join(repr(a) for a in self.children))
+        return "{}({})".format(
+            self.__class__.__name__, ", ".join(repr(a) for a in self.children)
+        )
 
     def flat(self, *types):
         if type(self) in types:
             return [self]
         return sum([child.flat(*types) for child in self.children], [])
 
 
 class Argument(LeafPattern):
-
     def single_match(self, left):
         for n, pattern in enumerate(left):
             if type(pattern) is Argument:
                 return n, Argument(self.name, pattern.value)
         return None, None
 
     @classmethod
     def parse(class_, source):
-        name = re.findall('(<\S*?>)', source)[0]
-        value = re.findall('\[default: (.*)\]', source, flags=re.I)
+        name = re.findall(r"(<\S*?>)", source)[0]
+        value = re.findall(r"\[default: (.*)\]", source, flags=re.I)
         return class_(name, value[0] if value else None)
 
 
 class Command(Argument):
-
     def __init__(self, name, value=False):
         self.name, self.value = name, value
 
     def single_match(self, left):
         for n, pattern in enumerate(left):
             if type(pattern) is Argument:
                 if pattern.value == self.name:
                     return n, Command(self.name, True)
                 else:
                     break
         return None, None
 
 
 class Option(LeafPattern):
-
     def __init__(self, short=None, long=None, argcount=0, value=False):
         assert argcount in (0, 1)
         self.short, self.long, self.argcount = short, long, argcount
         self.value = None if value is False and argcount else value
 
     @classmethod
     def parse(class_, option_description):
         short, long, argcount, value = None, None, 0, False
-        options, _, description = option_description.strip().partition('  ')
-        options = options.replace(',', ' ').replace('=', ' ')
+        options, _, description = option_description.strip().partition("  ")
+        options = options.replace(",", " ").replace("=", " ")
         for s in options.split():
-            if s.startswith('--'):
+            if s.startswith("--"):
                 long = s
-            elif s.startswith('-'):
+            elif s.startswith("-"):
                 short = s
             else:
                 argcount = 1
         if argcount:
-            matched = re.findall('\[default: (.*)\]', description, flags=re.I)
+            matched = re.findall(r"\[default: (.*)\]", description, flags=re.I)
             value = matched[0] if matched else None
         return class_(short, long, argcount, value)
 
     def single_match(self, left):
         for n, pattern in enumerate(left):
             if self.name == pattern.name:
                 return n, pattern
         return None, None
 
     @property
     def name(self):
         return self.long or self.short
 
     def __repr__(self):
-        return 'Option(%r, %r, %r, %r)' % (self.short, self.long,
-                                           self.argcount, self.value)
+        return "Option({!r}, {!r}, {!r}, {!r})".format(
+            self.short, self.long, self.argcount, self.value
+        )
 
 
 class Required(BranchPattern):
-
     def match(self, left, collected=None):
         collected = [] if collected is None else collected
         l = left
         c = collected
         for pattern in self.children:
             matched, l, c = pattern.match(l, c)
             if not matched:
                 return False, left, collected
         return True, l, c
 
 
 class Optional(BranchPattern):
-
     def match(self, left, collected=None):
         collected = [] if collected is None else collected
         for pattern in self.children:
             m, left, collected = pattern.match(left, collected)
         return True, left, collected
 
 
 class OptionsShortcut(Optional):
 
     """Marker/placeholder for [options] shortcut."""
 
 
 class OneOrMore(BranchPattern):
-
     def match(self, left, collected=None):
         assert len(self.children) == 1
         collected = [] if collected is None else collected
         l = left
         c = collected
         l_ = None
         matched = True
@@ -262,168 +255,169 @@
             l_ = l
         if times >= 1:
             return True, l, c
         return False, left, collected
 
 
 class Either(BranchPattern):
-
     def match(self, left, collected=None):
         collected = [] if collected is None else collected
         outcomes = []
         for pattern in self.children:
             matched, _, _ = outcome = pattern.match(left, collected)
             if matched:
                 outcomes.append(outcome)
         if outcomes:
             return min(outcomes, key=lambda outcome: len(outcome[1]))
         return False, left, collected
 
 
 class Tokens(list):
-
     def __init__(self, source, error=DocoptExit):
-        self += source.split() if hasattr(source, 'split') else source
+        self += source.split() if hasattr(source, "split") else source
         self.error = error
 
     @staticmethod
     def from_pattern(source):
-        source = re.sub(r'([\[\]\(\)\|]|\.\.\.)', r' \1 ', source)
-        source = [s for s in re.split('\s+|(\S*<.*?>)', source) if s]
+        source = re.sub(r"([\[\]\(\)\|]|\.\.\.)", r" \1 ", source)
+        source = [s for s in re.split(r"\s+|(\S*<.*?>)", source) if s]
         return Tokens(source, error=DocoptLanguageError)
 
     def move(self):
         return self.pop(0) if len(self) else None
 
     def current(self):
         return self[0] if len(self) else None
 
 
 def parse_long(tokens, options):
     """long ::= '--' chars [ ( ' ' | '=' ) chars ] ;"""
-    long, eq, value = tokens.move().partition('=')
-    assert long.startswith('--')
-    value = None if eq == value == '' else value
+    long, eq, value = tokens.move().partition("=")
+    assert long.startswith("--")
+    value = None if eq == value == "" else value
     similar = [o for o in options if o.long == long]
     if tokens.error is DocoptExit and similar == []:  # if no exact match
         similar = [o for o in options if o.long and o.long.startswith(long)]
     if len(similar) > 1:  # might be simply specified ambiguously 2+ times?
-        raise tokens.error('%s is not a unique prefix: %s?' %
-                           (long, ', '.join(o.long for o in similar)))
+        raise tokens.error(
+            "%s is not a unique prefix: %s?"
+            % (long, ", ".join(o.long for o in similar))
+        )
     elif len(similar) < 1:
-        argcount = 1 if eq == '=' else 0
+        argcount = 1 if eq == "=" else 0
         o = Option(None, long, argcount)
         options.append(o)
         if tokens.error is DocoptExit:
             o = Option(None, long, argcount, value if argcount else True)
     else:
-        o = Option(similar[0].short, similar[0].long,
-                   similar[0].argcount, similar[0].value)
+        o = Option(
+            similar[0].short, similar[0].long, similar[0].argcount, similar[0].value
+        )
         if o.argcount == 0:
             if value is not None:
-                raise tokens.error('%s must not have an argument' % o.long)
+                raise tokens.error("%s must not have an argument" % o.long)
         else:
             if value is None:
-                if tokens.current() in [None, '--']:
-                    raise tokens.error('%s requires argument' % o.long)
+                if tokens.current() in [None, "--"]:
+                    raise tokens.error("%s requires argument" % o.long)
                 value = tokens.move()
         if tokens.error is DocoptExit:
             o.value = value if value is not None else True
     return [o]
 
 
 def parse_shorts(tokens, options):
     """shorts ::= '-' ( chars )* [ [ ' ' ] chars ] ;"""
     token = tokens.move()
-    assert token.startswith('-') and not token.startswith('--')
-    left = token.lstrip('-')
+    assert token.startswith("-") and not token.startswith("--")
+    left = token.lstrip("-")
     parsed = []
-    while left != '':
-        short, left = '-' + left[0], left[1:]
+    while left != "":
+        short, left = "-" + left[0], left[1:]
         similar = [o for o in options if o.short == short]
         if len(similar) > 1:
-            raise tokens.error('%s is specified ambiguously %d times' %
-                               (short, len(similar)))
+            raise tokens.error(
+                "%s is specified ambiguously %d times" % (short, len(similar))
+            )
         elif len(similar) < 1:
             o = Option(short, None, 0)
             options.append(o)
             if tokens.error is DocoptExit:
                 o = Option(short, None, 0, True)
         else:  # why copying is necessary here?
-            o = Option(short, similar[0].long,
-                       similar[0].argcount, similar[0].value)
+            o = Option(short, similar[0].long, similar[0].argcount, similar[0].value)
             value = None
             if o.argcount != 0:
-                if left == '':
-                    if tokens.current() in [None, '--']:
-                        raise tokens.error('%s requires argument' % short)
+                if left == "":
+                    if tokens.current() in [None, "--"]:
+                        raise tokens.error("%s requires argument" % short)
                     value = tokens.move()
                 else:
                     value = left
-                    left = ''
+                    left = ""
             if tokens.error is DocoptExit:
                 o.value = value if value is not None else True
         parsed.append(o)
     return parsed
 
 
 def parse_pattern(source, options):
     tokens = Tokens.from_pattern(source)
     result = parse_expr(tokens, options)
     if tokens.current() is not None:
-        raise tokens.error('unexpected ending: %r' % ' '.join(tokens))
+        raise tokens.error("unexpected ending: %r" % " ".join(tokens))
     return Required(*result)
 
 
 def parse_expr(tokens, options):
     """expr ::= seq ( '|' seq )* ;"""
     seq = parse_seq(tokens, options)
-    if tokens.current() != '|':
+    if tokens.current() != "|":
         return seq
     result = [Required(*seq)] if len(seq) > 1 else seq
-    while tokens.current() == '|':
+    while tokens.current() == "|":
         tokens.move()
         seq = parse_seq(tokens, options)
         result += [Required(*seq)] if len(seq) > 1 else seq
     return [Either(*result)] if len(result) > 1 else result
 
 
 def parse_seq(tokens, options):
     """seq ::= ( atom [ '...' ] )* ;"""
     result = []
-    while tokens.current() not in [None, ']', ')', '|']:
+    while tokens.current() not in [None, "]", ")", "|"]:
         atom = parse_atom(tokens, options)
-        if tokens.current() == '...':
+        if tokens.current() == "...":
             atom = [OneOrMore(*atom)]
             tokens.move()
         result += atom
     return result
 
 
 def parse_atom(tokens, options):
     """atom ::= '(' expr ')' | '[' expr ']' | 'options'
-             | long | shorts | argument | command ;
+    | long | shorts | argument | command ;
     """
     token = tokens.current()
     result = []
-    if token in '([':
+    if token in "([":
         tokens.move()
-        matching, pattern = {'(': [')', Required], '[': [']', Optional]}[token]
+        matching, pattern = {"(": [")", Required], "[": ["]", Optional]}[token]
         result = pattern(*parse_expr(tokens, options))
         if tokens.move() != matching:
             raise tokens.error("unmatched '%s'" % token)
         return [result]
-    elif token == 'options':
+    elif token == "options":
         tokens.move()
         return [OptionsShortcut()]
-    elif token.startswith('--') and token != '--':
+    elif token.startswith("--") and token != "--":
         return parse_long(tokens, options)
-    elif token.startswith('-') and token not in ('-', '--'):
+    elif token.startswith("-") and token not in ("-", "--"):
         return parse_shorts(tokens, options)
-    elif token.startswith('<') and token.endswith('>') or token.isupper():
+    elif token.startswith("<") and token.endswith(">") or token.isupper():
         return [Argument(tokens.move())]
     else:
         return [Command(tokens.move())]
 
 
 def parse_argv(tokens, options, options_first=False):
     """Parse command-line argument vector.
@@ -432,63 +426,65 @@
         argv ::= [ long | shorts ]* [ argument ]* [ '--' [ argument ]* ] ;
     else:
         argv ::= [ long | shorts | argument ]* [ '--' [ argument ]* ] ;
 
     """
     parsed = []
     while tokens.current() is not None:
-        if tokens.current() == '--':
+        if tokens.current() == "--":
             return parsed + [Argument(None, v) for v in tokens]
-        elif tokens.current().startswith('--'):
+        elif tokens.current().startswith("--"):
             parsed += parse_long(tokens, options)
-        elif tokens.current().startswith('-') and tokens.current() != '-':
+        elif tokens.current().startswith("-") and tokens.current() != "-":
             parsed += parse_shorts(tokens, options)
         elif options_first:
             return parsed + [Argument(None, v) for v in tokens]
         else:
             parsed.append(Argument(None, tokens.move()))
     return parsed
 
 
 def parse_defaults(doc):
     defaults = []
-    for s in parse_section('options:', doc):
+    for s in parse_section("options:", doc):
         # FIXME corner case "bla: options: --foo"
-        _, _, s = s.partition(':')  # get rid of "options:"
-        split = re.split('\n[ \t]*(-\S+?)', '\n' + s)[1:]
+        _, _, s = s.partition(":")  # get rid of "options:"
+        split = re.split("\n[ \t]*(-\\S+?)", "\n" + s)[1:]
         split = [s1 + s2 for s1, s2 in zip(split[::2], split[1::2])]
-        options = [Option.parse(s) for s in split if s.startswith('-')]
+        options = [Option.parse(s) for s in split if s.startswith("-")]
         defaults += options
     return defaults
 
 
 def parse_section(name, source):
-    pattern = re.compile('^([^\n]*' + name + '[^\n]*\n?(?:[ \t].*?(?:\n|$))*)',
-                         re.IGNORECASE | re.MULTILINE)
+    pattern = re.compile(
+        "^([^\n]*" + name + "[^\n]*\n?(?:[ \t].*?(?:\n|$))*)",
+        re.IGNORECASE | re.MULTILINE,
+    )
     return [s.strip() for s in pattern.findall(source)]
 
 
 def formal_usage(section):
-    _, _, section = section.partition(':')  # drop "usage:"
+    _, _, section = section.partition(":")  # drop "usage:"
     pu = section.split()
-    return '( ' + ' '.join(') | (' if s == pu[0] else s for s in pu[1:]) + ' )'
+    return "( " + " ".join(") | (" if s == pu[0] else s for s in pu[1:]) + " )"
 
 
 def extras(help, version, options, doc):
-    if help and any((o.name in ('-h', '--help')) and o.value for o in options):
+    if help and any((o.name in ("-h", "--help")) and o.value for o in options):
         print(doc.strip("\n"))
         sys.exit()
-    if version and any(o.name == '--version' and o.value for o in options):
+    if version and any(o.name == "--version" and o.value for o in options):
         print(version)
         sys.exit()
 
 
 class Dict(dict):
     def __repr__(self):
-        return '{%s}' % ',\n '.join('%r: %r' % i for i in sorted(self.items()))
+        return "{%s}" % ",\n ".join("%r: %r" % i for i in sorted(self.items()))
 
 
 def docopt(doc, argv=None, help=True, version=None, options_first=False):
     """Parse `argv` based on command-line interface described in `doc`.
 
     `docopt` creates your command-line interface based on its
     description that you pass as `doc`. Such description can contain
@@ -548,34 +544,34 @@
     * For video introduction see http://docopt.org
     * Full documentation is available in README.rst as well as online
       at https://github.com/docopt/docopt#readme
 
     """
     argv = sys.argv[1:] if argv is None else argv
 
-    usage_sections = parse_section('usage:', doc)
+    usage_sections = parse_section("usage:", doc)
     if len(usage_sections) == 0:
         raise DocoptLanguageError('"usage:" (case-insensitive) not found.')
     if len(usage_sections) > 1:
         raise DocoptLanguageError('More than one "usage:" (case-insensitive).')
     DocoptExit.usage = usage_sections[0]
 
     options = parse_defaults(doc)
     pattern = parse_pattern(formal_usage(DocoptExit.usage), options)
     # [default] syntax for argument is disabled
-    #for a in pattern.flat(Argument):
+    # for a in pattern.flat(Argument):
     #    same_name = [d for d in arguments if d.name == a.name]
     #    if same_name:
     #        a.value = same_name[0].value
     argv = parse_argv(Tokens(argv), list(options), options_first)
     pattern_options = set(pattern.flat(Option))
     for options_shortcut in pattern.flat(OptionsShortcut):
         doc_options = parse_defaults(doc)
         options_shortcut.children = list(set(doc_options) - pattern_options)
-        #if any_options:
+        # if any_options:
         #    options_shortcut.children += [Option(o.short, o.long, o.argcount)
         #                    for o in argv if type(o) is Option]
     extras(help, version, argv, doc)
     matched, left, collected = pattern.fix().match(argv)
     if matched and left == []:  # better error message if left?
         return Dict((a.name, a.value) for a in (pattern.flat() + collected))
     raise DocoptExit()
```

### Comparing `pmgr-2.0.2/pmgr/migrate/pmgrobj.py` & `pmgr-2.1.3/pmgr/pmgrobj.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,103 @@
-import time
+import configparser
 import datetime
 import re
 
 import MySQLdb as mdb
+
 try:
     import _mysql_exceptions
 except ImportError:
     import MySQLdb._exceptions as _mysql_exceptions
-import pyca
+
+from . import utils
+
+CREDENTIALS = "/cds/group/pcds/admin/pmgr/pmgr.ini"
 
 ####################
 #
 # Utility Functions
 #
 ####################
 
-# Map MySQL types to python types in a quick and dirty manner.
+
 def m2pType(name):
-    if name[:7] == 'varchar' or name[:8] == 'datetime':
+    """
+    Map MySQL types to python types.
+
+    Parameters
+    ----------
+    name : str
+        A MySQL type name.
+
+    Returns
+    -------
+    kind : type
+        A python type corresponding to name, or None if a corresponding
+        type cannot be determined.
+    """
+    if name[:7] == "varchar" or name[:8] == "datetime":
         return str
-    if name[:3] == 'int' or name[:8] == 'smallint' or name[:7] == 'tinyint':
+    if name[:3] == "int" or name[:8] == "smallint" or name[:7] == "tinyint":
         return int
-    if name[:6] == 'double':
+    if name[:6] == "double":
         return float
     print("Unknown type %s" % name)
     return None
 
-# Map MySQL field names to PV extensions.
+
 def fixName(name):
+    """
+    Map MySQL field names to PV suffixes.
+
+    Parameters
+    ----------
+    name : str
+        A MySQL field.  It is assumed that this is begins either "FLD_"
+        (if this should be a field of the base PV) or "PV_" (if this is
+        an extension of the base PV).
+
+    Returns
+    -------
+    suffix : str
+        A suffix to be appended to the base PV name.  "FLD_" will be replaced
+        with ".", and "PV_" will be replaced with ":".  Single "_" in the name
+        will become ":" and double "_" will become single "_".
+    """
     name = re.sub("::", "_", re.sub("_", ":", name))
     if name[:3] == "PV:":
         return name[2:]
     else:
-        c = name.rindex(':')
-        return name[3:c] + '.' + name[c+1:]
+        c = name.rindex(":")
+        return name[3:c] + "." + name[c + 1 :]
+
 
-# Map MySQL field names to the descriptive part of the name.
 def createAlias(name):
+    """
+    Map MySQL field names to the descriptive part of the name.
+
+    name : str
+        A MySQL field.  It is assumed that this is begins either "FLD_"
+        (if this should be a field of the base PV) or "PV_" (if this is
+        an extension of the base PV).
+
+    Returns
+    -------
+    desc : str
+        Remove the prefix "FLD_" or "PV_" from name and replace "__" with "_".
+    """
     name = re.sub("__", "_", name)
     if name[:3] == "PV_":
         return name[3:]
     if name[:4] == "FLD_":
         return name[4:]
     else:
         return name
 
+
 ####################
 #
 # pmgrobj - The Parameter Manager Object class.
 #
 ####################
 #
 # pmgrobj(table, hutch, debug=False)
@@ -78,28 +127,23 @@
 #     fldmap
 #         - A dictionary mapping field names to information dictionaries.
 #     setflds
 #         - A list containing lists of field names, each list having the
 #           same setorder, with the entire list sorted by setorder.
 #     cfgs
 #         - A configuration ID to configuration dictionary mapping.
-#           The keys are a few boilerplate keys (id, config, owner, etc.)
+#           The keys are a few boilerplate keys (id, config, etc.)
 #           and the configuration fields.  Note that due to inheritance
 #           and mutual exclusion, many of these fields could be "None".
+#     cfgmap
+#         - A configuration name to ID dictionary mapping.
 #     objs
-#         - An object ID to object dictionary mapping.  The keys are a 
-#           few boilerplate keys (id, config, owner, etc.) and the
-#           object-only fields (the objflds with the 'obj' key value True).
-#     groupids
-#         - A list of group IDs.
-#     groups
-#         - A group ID to group information dictionary mapping.  The group
-#           information dictionary keys are either integers (which map to
-#           a dictionary giving a config and port for that group element)
-#           or "global" (which maps to a dictionary with keys "name" and "len".)
+#         - An object ID to object dictionary mapping.  The keys are a
+#           few boilerplate keys (id, config, etc.) and the object-only
+#           fields (the objflds with the 'obj' key value True).
 #
 # The field information dictionaries have the following keys:
 #     fld
 #         - The field name.
 #     pv
 #         - The field name translated to a PV base extension.
 #     alias
@@ -131,122 +175,93 @@
 #     unique
 #         - Must this field have a unique value?
 #     tooltip
 #         - The tooltip/hint text for this field.
 #     readonly
 #         - Is this field is readonly?
 #
-# Exported methods:
-#     checkForUpdate()
-#         - Returns a mask of DB_CONFIG, DB_OBJECT, and DB_GROUP indicating
-#           which tables (if any) are out of date.
-#     updateTables(mask=DB_ALL)
-#         - Read in the specified tables.
-#     start_transaction()
-#         - Begin to make DB changes.
-#     transaction_error(msg)
-#         - Generate an error message for the DB change.
-#     end_transaction()
-#         - Commit or rollback the current transaction.  Return a list of
-#           error strings, so an empty list indicates a successful commit.
-#     configDelete(idx, namefunc=None)
-#         - Delete a configuration.  (namefunc is an idx -> name mapping function).
-#     configInsert(d)
-#         - Insert a new configuration.  Returns the new configuration ID or None
-#           if it fails.
-#     configChange(idx, e)
-#         - Change an existing configuration.  e is a field -> value dictionary for
-#           the changes.
-#     objectDelete(idx)
-#         - Delete an existing object.
-#     objectInsert(d)
-#         - Insert a new object.  Returns the new object ID or None if it fails.
-#     objectChange(idx, e)
-#         - Change an existing object.  e is a field -> value dictionary for the
-#           changes.
-#     groupDelete(idx)
-#         - Delete an existing configuration group.
-#     groupInsert(d)
-#         - Insert a new configuration group.  d is a dictionary which maps from
-#           integers (group element indices) to a dictionary with config/port indices.
-#     groupUpdate(idx, d)
-#         - Change an existing configuration group. d is the same as the groupInsert
-#           dictionary.
-#     countInstance(cfglist)
-#         - Return a count of objects that depend on one of the listed configurations.
-#     getAutoCfg(d)
-#         - Given an object dictionary, find and return the most recently used
-#           configuration that has the autoconfig field set to a matching value.
-#           First look in this hutch, then in any hutch.  If none is found, return
-#           an empty dictionary.
-#     getConfig(idx)
-#         - Expand the configuration to deal with parentage.  cfgs[idx] could have
-#           many "None" values which are inherited, and this routine will fill them
-#           out and set the "_haveval" key to a dictionary indicating which fields
-#           have values set by the configuration itself (True) and which are inherited
-#           (False).
-#     applyConfig(idx)
-#         - Given an object ID, apply its current configuration to it.
-#     applyAllConfigs()
-#         - Apply the current configuration to all objects.
 
-class pmgrobj(object):
+
+class pmgrobj:
     DB_CONFIG = 1
     DB_OBJECT = 2
-    DB_GROUP  = 4
-    DB_CFGGRP = 8
-    DB_ALL    = 7
+    DB_ALL = 3
 
-    ORDER_MASK    = 0x0003ff
+    ORDER_MASK = 0x0003FF
     SETMUTEX_MASK = 0x000200
-    MUST_WRITE    = 0x000400
-    WRITE_ZERO    = 0x000800
-    AUTO_CONFIG   = 0x001000
-    READ_ONLY     = 0x002000
-
-    unwanted = ['seq', 'owner', 'id', 'category', 'dt_created',
-                'date', 'dt_updated', 'name', 'action', 'rec_base', 'comment']
+    MUST_WRITE = 0x000400
+    WRITE_ZERO = 0x000800
+    AUTO_CONFIG = 0x001000
+    READ_ONLY = 0x002000
+
+    unwanted = [
+        "seq",
+        "owner",
+        "id",
+        "category",
+        "dt_created",
+        "date",
+        "dt_updated",
+        "name",
+        "action",
+        "rec_base",
+        "comment",
+    ]
 
     def __init__(self, table, hutch, debug=False, prod=True):
         self.table = table
         self.hutch = hutch
         self.debug = debug
         self.cfgs = None
         self.objs = None
-        self.groupids = []
-        self.groups = {}
         self.errorlist = []
         self.autoconfig = None
         self.in_trans = False
-        if prod:
-            print("Using production server.")
-            self.con = mdb.connect('psdb', 'pscontrols', 'pcds', 'pscontrols')
-        else:
-            print("Using development server.")
-            self.con = mdb.connect('psdbdev01', 'mctest', 'mctest', 'pscontrols')
+        self.con = self.connect(prod)
         self.con.autocommit(False)
         self.cur = self.con.cursor(mdb.cursors.DictCursor)
         self.cur.execute("call init_pcds()")
         self.readFormat()
         self.dbgid = 42
-        self.lastcfg = datetime.datetime(1900,1,1,0,0,1)
-        self.lastobj = datetime.datetime(1900,1,1,0,0,1)
-        self.lastgrp = datetime.datetime(1900,1,1,0,0,1)
+        self.lastcfg = datetime.datetime(1900, 1, 1, 0, 0, 1)
+        self.lastobj = datetime.datetime(1900, 1, 1, 0, 0, 1)
         self.hutchlist = self.getHutchList()
         self.checkForUpdate()
         self.updateTables()
 
+    def connect(self, prod):
+        conf = configparser.ConfigParser(defaults={})
+        conf.read(CREDENTIALS)
+        cfg = "production" if prod else "development"
+        print("Using %s server." % cfg)
+        return mdb.connect(conf[cfg]['host'], conf[cfg]['user'], conf[cfg]['password'], conf[cfg]['db'])
+
     def readFormat(self):
+        """
+        Retrieve the table formats from the database.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        Nothing.
+        """
         self.cur.execute("describe %s" % self.table)
-        locfld = [(d['Field'], m2pType(d['Type']), d['Null'], d['Key']) for d in self.cur.fetchall()]
-        locfld = locfld[10:]   # Skip the standard fields!
+        locfld = [
+            (d["Field"], m2pType(d["Type"]), d["Null"], d["Key"])
+            for d in self.cur.fetchall()
+        ]
 
         self.cur.execute("describe %s_cfg" % self.table)
-        fld = [(d['Field'], m2pType(d['Type']), d['Null'], d['Key']) for d in self.cur.fetchall()]
-        fld = fld[7:]         # Skip the standard fields!
+        fld = [
+            (d["Field"], m2pType(d["Type"]), d["Null"], d["Key"])
+            for d in self.cur.fetchall()
+        ]
 
         self.cur.execute("select * from %s_name_map" % self.table)
         result = self.cur.fetchall()
 
         alias = {}
         colorder = {}
         setorder = {}
@@ -255,245 +270,328 @@
         mutex = {}
         nullok = {}
         unique = {}
         mutex_sets = []
         mutex_flds = []
         for i in range(16):
             mutex_sets.append([])
-        for (f, t, nl, k) in locfld:
-            alias[f] = createAlias(f)
-            colorder[f] = 1000
-            setorder[f] = 0
-            mutex[f] = 0
-            tooltip[f] = ''
-            nullok[f] = ((nl == 'YES') or (t != str))
-            unique[f] = k == "UNI"
-        for (f, t, nl, k) in fld:
-            alias[f] = createAlias(f)
-            colorder[f] = 1000
-            setorder[f] = 0
-            mutex[f] = 0
-            tooltip[f] = ''
-            nullok[f] = ((nl == 'YES') or (t != str))
-            unique[f] = k == "UNI"
+        for f, t, nl, k in locfld:
+            if f[0].isupper():
+                alias[f] = createAlias(f)
+                colorder[f] = 1000
+                setorder[f] = 0
+                mutex[f] = 0
+                tooltip[f] = ""
+                nullok[f] = (nl == "YES") or (t != str)
+                unique[f] = k == "UNI"
+        for f, t, nl, k in fld:
+            if f[0].isupper():
+                alias[f] = createAlias(f)
+                colorder[f] = 1000
+                setorder[f] = 0
+                mutex[f] = 0
+                tooltip[f] = ""
+                nullok[f] = (nl == "YES") or (t != str)
+                unique[f] = k == "UNI"
 
         for d in result:
-            f = d['db_field_name']
-            if d['alias'] != "":
-                alias[f] = d['alias']
-            colorder[f] = d['col_order']
-            setorder[f] = d['set_order']
-            tooltip[f] = d['tooltip']
-            v = d['enum']
+            f = d["db_field_name"]
+            if d["alias"] != "":
+                alias[f] = d["alias"]
+            colorder[f] = d["col_order"]
+            setorder[f] = d["set_order"]
+            tooltip[f] = d["tooltip"]
+            v = d["enum"]
             if v != "":
-                enum[f] = v.split('|')
-            v = d['mutex_mask']
+                enum[f] = v.split("|")
+            v = d["mutex_mask"]
             if v != 0:
                 for i in range(16):
                     if v & (1 << i) != 0:
                         mutex_sets[i].append(f)
                 mutex_flds.append(f)
             if setorder[f] & self.AUTO_CONFIG != 0:
                 self.autoconfig = f
         # We're assuming the bits are used from LSB to MSB, no gaps!
         self.mutex_sets = [l for l in mutex_sets if l != []]
         self.mutex_flds = mutex_flds
         for d in result:
-            f = d['db_field_name']
+            f = d["db_field_name"]
             mutex[f] = []
-            v = d['mutex_mask']
+            v = d["mutex_mask"]
             if v != 0:
                 for i in range(16):
                     if v & (1 << i) != 0:
                         mutex[f].append(i)
 
         self.objflds = []
         setflds = {}
-        setset = set([])
-        for (f, t, nl, k) in locfld:
-            n = fixName(f)
-            so = setorder[f] & self.ORDER_MASK
-            setset.add(so)
-            d = {'fld': f, 'pv': n, 'alias' : alias[f], 'type': t, 'nullok': nullok[f],
-                 'colorder': colorder[f], 'setorder': so, 'unique': unique[f],
-                 'mustwrite': (setorder[f] & self.MUST_WRITE) == self.MUST_WRITE,
-                 'writezero': (setorder[f] & self.WRITE_ZERO) == self.WRITE_ZERO,
-                 'setmutex': (setorder[f] & self.SETMUTEX_MASK) == self.SETMUTEX_MASK,
-                 'readonly': (setorder[f] & self.READ_ONLY) == self.READ_ONLY,
-                 'tooltip': tooltip[f], 'mutex' : mutex[f], 'obj': True}
-            try:
-                setflds[so].append(f)
-            except:
-                setflds[so] = [f]
-            try:
-                d['enum'] = enum[f]
-            except:
-                pass 
-            self.objflds.append(d)
-        for (f, t, nl, k) in fld:
-            n = fixName(f)
-            so = setorder[f] & self.ORDER_MASK
-            setset.add(so)
-            d = {'fld': f, 'pv': n, 'alias' : alias[f], 'type': t, 'nullok': nullok[f],
-                 'colorder': colorder[f], 'setorder': so, 'unique': unique[f],
-                 'mustwrite': (setorder[f] & self.MUST_WRITE) == self.MUST_WRITE,
-                 'writezero': (setorder[f] & self.WRITE_ZERO) == self.WRITE_ZERO,
-                 'setmutex': (setorder[f] & self.SETMUTEX_MASK) == self.SETMUTEX_MASK,
-                 'readonly': (setorder[f] & self.READ_ONLY) == self.READ_ONLY,
-                 'tooltip': tooltip[f], 'mutex' : mutex[f], 'obj': False}
-            try:
-                setflds[so].append(f)
-            except:
-                setflds[so] = [f]
-            try:
-                d['enum'] = enum[f]
-            except:
-                pass
-            self.objflds.append(d)
-        self.objflds.sort(key=lambda d: d['colorder'])   # New regime: col_order is manditory and unique!
+        setset = set()
+        for f, t, nl, k in locfld:
+            if f[0].isupper():
+                n = fixName(f)
+                so = setorder[f] & self.ORDER_MASK
+                setset.add(so)
+                d = {
+                    "fld": f,
+                    "pv": n,
+                    "alias": alias[f],
+                    "type": t,
+                    "nullok": nullok[f],
+                    "colorder": colorder[f],
+                    "setorder": so,
+                    "unique": unique[f],
+                    "mustwrite": (setorder[f] & self.MUST_WRITE) == self.MUST_WRITE,
+                    "writezero": (setorder[f] & self.WRITE_ZERO) == self.WRITE_ZERO,
+                    "setmutex": (setorder[f] & self.SETMUTEX_MASK)
+                    == self.SETMUTEX_MASK,
+                    "readonly": (setorder[f] & self.READ_ONLY) == self.READ_ONLY,
+                    "tooltip": tooltip[f],
+                    "mutex": mutex[f],
+                    "obj": True,
+                }
+                try:
+                    setflds[so].append(f)
+                except Exception:
+                    setflds[so] = [f]
+                try:
+                    d["enum"] = enum[f]
+                except Exception:
+                    pass
+                self.objflds.append(d)
+        for f, t, nl, k in fld:
+            if f[0].isupper():
+                n = fixName(f)
+                so = setorder[f] & self.ORDER_MASK
+                setset.add(so)
+                d = {
+                    "fld": f,
+                    "pv": n,
+                    "alias": alias[f],
+                    "type": t,
+                    "nullok": nullok[f],
+                    "colorder": colorder[f],
+                    "setorder": so,
+                    "unique": unique[f],
+                    "mustwrite": (setorder[f] & self.MUST_WRITE) == self.MUST_WRITE,
+                    "writezero": (setorder[f] & self.WRITE_ZERO) == self.WRITE_ZERO,
+                    "setmutex": (setorder[f] & self.SETMUTEX_MASK)
+                    == self.SETMUTEX_MASK,
+                    "readonly": (setorder[f] & self.READ_ONLY) == self.READ_ONLY,
+                    "tooltip": tooltip[f],
+                    "mutex": mutex[f],
+                    "obj": False,
+                }
+                try:
+                    setflds[so].append(f)
+                except Exception:
+                    setflds[so] = [f]
+                try:
+                    d["enum"] = enum[f]
+                except Exception:
+                    pass
+                self.objflds.append(d)
+        self.objflds.sort(
+            key=lambda d: d["colorder"]
+        )  # New regime: col_order is manditory and unique!
         self.fldmap = {}
         for i in range(len(self.objflds)):
             d = self.objflds[i]
-            d['objidx'] = i
-            self.fldmap[d['fld']] = d
-        self.cfgflds = [d for d in self.objflds if d['obj'] == False]
+            d["objidx"] = i
+            self.fldmap[d["fld"]] = d
+        self.cfgflds = [d for d in self.objflds if d["obj"] is False]
         for i in range(len(self.cfgflds)):
-            self.cfgflds[i]['cfgidx'] = i
+            self.cfgflds[i]["cfgidx"] = i
         # Set the type of each mutex_set and make sure it's consistent
         self.mutex_obj = []
         for l in self.mutex_sets:
-            self.mutex_obj.append(self.fldmap[l[0]]['obj'])
+            self.mutex_obj.append(self.fldmap[l[0]]["obj"])
             for m in l:
-                if self.fldmap[m]['obj'] != self.mutex_obj[-1]:
+                if self.fldmap[m]["obj"] != self.mutex_obj[-1]:
                     print("Inconsistent mutex set %s!" % str(l))
                     raise Exception()
         setset = list(setset)
         setset.sort()
         self.setflds = [setflds[i] for i in setset]
         self.con.commit()
 
     def getHutchList(self):
+        """
+        Retieve the current list of supported hutches from the database.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        hlist : list
+            A list of strings, one for each supported hutch.
+        """
         l = []
         try:
             self.cur.execute("select * from %s_update" % (self.table))
             for d in self.cur.fetchall():
-                n = d['tbl_name']
-                if n[-4:] != '_grp' and n != 'config':
+                n = d["tbl_name"]
+                if n != "config":
                     l.append(n)
             self.con.commit()
             l.sort()
-        except:
+        except Exception:
             pass
         return l
 
     def checkForUpdate(self):
+        """
+        Check the database for updates.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        mask : int
+            A bit mask of DB_CONFIG and DB_OBJECT indicating which tables
+            (if any) are out of date.
+        """
         if self.in_trans:
-            return 0      # Not now!
+            return 0  # Not now!
         try:
             v = 0
             if self.hutch is None:
                 self.cur.execute("select * from %s_update" % self.table)
             else:
-                self.cur.execute("select * from %s_update where tbl_name = 'config' or tbl_name = '%s' or tbl_name = '%s'" %
-                                 (self.table, self.hutch, self.hutch + "_grp"))
+                self.cur.execute(
+                    "select * from %s_update where tbl_name = 'config' or tbl_name = '%s'"
+                    % (self.table, self.hutch)
+                )
             for d in self.cur.fetchall():
-                if d['tbl_name'] == 'config':
-                    if d['dt_updated'] > self.lastcfg:
-                        self.lastcfg = d['dt_updated']
+                if d["tbl_name"] == "config":
+                    if d["dt_updated"] > self.lastcfg:
+                        self.lastcfg = d["dt_updated"]
                         v = v | self.DB_CONFIG
-                elif d['tbl_name'][-4:] == "_grp":
-                    if d['dt_updated'] > self.lastgrp:
-                        self.lastgrp = d['dt_updated']
-                        v = v | self.DB_GROUP
                 else:
-                    if d['dt_updated'] > self.lastobj:
-                        self.lastobj = d['dt_updated']
+                    if d["dt_updated"] > self.lastobj:
+                        self.lastobj = d["dt_updated"]
                         v = v | self.DB_OBJECT
             self.con.commit()
-        except:
+        except Exception:
             pass
         return v
 
     def readDB(self, kind):
+        """
+        Read in a complete database table.
+
+        Parameters
+        ----------
+        kind : int
+            Which table to read, either DB_CONFIG or DB_OBJECT.
+
+        Returns
+        -------
+        dlist : list
+            A list of dictionaries containing the entire database.
+        """
         if kind == self.DB_CONFIG:
             ext = "_cfg"
-        elif kind == self.DB_OBJECT:
+        else:  # self.DB_OBJECT
             if self.hutch is None:
                 ext = ""
             else:
                 ext = " where owner = '%s' or id = 0" % self.hutch
-        elif kind == self.DB_GROUP:
-            if self.hutch is None:
-                ext = "_grp"
-            else:
-                ext = "_grp where owner = '%s'" % self.hutch
-        else: # self.DB_CFGGRP
-            ext = "_cfg_grp"
         try:
-            self.cur.execute("select * from %s%s" % (self.table, ext))
+            self.cur.execute("select * from {}{}".format(self.table, ext))
             return list(self.cur.fetchall())
-        except:
+        except Exception:
             return []
 
     def updateTables(self, mask=DB_ALL):
-        if self.in_trans:                    # This shouldn't happen.  But let's be paranoid.
+        """
+        Update the specified tables from the database.
+
+        Parameters
+        ----------
+        mask : int
+            A bit mask of DB_CONFIG and DB_OBJECT indicating which tables
+            should be read.  (Defaults to all tables.)
+        """
+        if self.in_trans:  # This shouldn't happen.  But let's be paranoid.
             return
         if (mask & self.DB_CONFIG) != 0:
             cfgs = self.readDB(self.DB_CONFIG)
             if cfgs == []:
                 mask &= ~self.DB_CONFIG
             else:
-                map = {}
+                cid = {}
+                cname = {}
                 for d in cfgs:
-                    map[d['id']] = d
-                self.cfgs = map
+                    cid[d['id']] = d
+                    cname[d['name']] = d['id']
+                self.cfgs = cid
+                self.cfgmap = cname
         if (mask & self.DB_OBJECT) != 0:
             objs = self.readDB(self.DB_OBJECT)
             if objs == []:
                 mask &= ~self.DB_OBJECT
             else:
                 objmap = {}
                 for o in objs:
-                    objmap[o['id']] = o
+                    objmap[o["id"]] = o
                 self.objs = objmap
-        if (mask & self.DB_GROUP) != 0:
-            grps = self.readDB(self.DB_GROUP)
-            cfggrp = self.readDB(self.DB_CFGGRP)
-            if grps == []:
-                mask &= ~self.DB_GROUP
-            else:
-                self.groupids   = []
-                self.groups     = {}
-                for g in grps:
-                    id = g['id']
-                    self.groupids.append(id)
-                    self.groups[id] = {}
-                    try:
-                        self.groups[id]['global'] = {'len' : 0, 'name' : g['name'], 'active': g['active']}
-                    except:
-                        print(g)
-                        raise
-                for g in cfggrp:
-                    id = g['group_id']
-                    if id in self.groups.keys():
-                        self.groups[id][g['dispseq']] = {'config': g['config_id'],
-                                                         'port': g['port_id']}
-                        sz = self.groups[id]['global']['len'] + 1
-                        self.groups[id]['global']['len'] = sz
         return mask
 
     def start_transaction(self):
+        """
+        Prepare to make changes to the database.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        Nothing
+        """
         self.in_trans = True
         self.errorlist = []
         return True
 
     def transaction_error(self, msg):
+        """
+        Indicate an error during a database transaction.
+
+        Parameters
+        ----------
+        msg : str
+            An error string.
+
+        Returns
+        -------
+        None
+        """
         self.errorlist.append(_mysql_exceptions.Error(0, msg))
 
     def end_transaction(self):
+        """
+        Attempt to commit the transaction, or roll it back if there is
+        an issue.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        elist : list
+            A list of strings containing the error messages accumulated
+            during the transaction.  If the transaction succeeded, this is
+            an empty list.
+        """
         didcommit = False
         if self.errorlist == []:
             try:
                 self.con.commit()
                 if self.debug:
                     print("COMMIT!")
                 didcommit = True
@@ -502,60 +600,103 @@
         if not didcommit:
             self.con.rollback()
             if self.debug:
                 print("ROLLBACK!")
         self.in_trans = False
         el = []
         for e in self.errorlist:
-            (n, m) = e.args
+            if len(e.args) == 1:
+                n = e.args[0]
+                m = ""
+            else:
+                (n, m) = e.args
             if n != 0:
                 el.append("Error %d: %s\n" % (n, m))
             else:
                 el.append("Error: %s\n" % (m))
         return el
 
-####################
-#
-# Actual database manipulation routines!
-#
-####################
+    ####################
+    #
+    # Actual database manipulation routines!
+    #
+    ####################
 
     @staticmethod
     def defaultNamefunc(idx):
         return "#" + str(idx)
 
     def configDelete(self, idx, namefunc=defaultNamefunc):
-        try:
-            if self.cur.execute("select id from %s where config = %%s" % self.table, (idx,)) != 0:
+        """
+        Delete a configuration from the database.  Assumes inside a
+        transaction, but does not commit the change.
+
+        Parameters
+        ----------
+        idx : int
+            A database ID for the configuration to be deleted.
+
+        namefunc : int -> str
+            A function to provide human-readable names for the database ID.
+            (A useful function is not really defined here.)
+
+        Returns
+        -------
+        Nothing
+
+        If the deletion fails, errors are appended to the transaction
+        errorlist.
+        """
+        try:
+            if (
+                self.cur.execute(
+                    "select id from %s where config = %%s" % self.table, (idx,)
+                )
+                != 0
+            ):
                 self.errorlist.append(
-                    _mysql_exceptions.Error(0,
-                                            "Can't delete configuration %s, still in use." % namefunc(idx)))
+                    _mysql_exceptions.Error(
+                        0,
+                        "Can't delete configuration %s, still in use." % namefunc(idx),
+                    )
+                )
                 return
             self.cur.execute("delete from %s_cfg where id = %%s" % self.table, (idx,))
         except _mysql_exceptions.Error as e:
             self.errorlist.append(e)
- 
+
     def configInsert(self, d):
-        cmd = "insert %s_cfg (name, config, owner, mutex, dt_updated" % self.table
-        vals = d['_val']
+        """
+        Insert a new configuration into the database, assuming inside
+        a transaction.
+
+        Parameters
+        ----------
+        d : dict
+            A dictionary containing values for database fields.
+
+        Returns
+        -------
+        id : int
+            A new configuration ID, or None if this fails. Adds to
+            transaction errorlist on failure.
+        """
+        cmd = "insert %s_cfg (name, config, mutex, dt_updated" % self.table
         for f in self.cfgflds:
-            fld = f['fld']
-            if vals[fld]:
-                cmd += ", " + fld
-        cmd += ") values (%s, %s, %s, %s, now()"
-        vlist = [d['name']]
-        vlist.append(d['config'])
-        vlist.append(self.hutch)
-        vlist.append(d['mutex'])
+            fld = f["fld"]
+            cmd += ", " + fld
+        cmd += ") values (%s, %s, %s, now()"
+        vlist = [d["name"]]
+        vlist.append(d["config"])
+        vlist.append(d["mutex"])
         for f in self.cfgflds:
-            fld = f['fld']
-            if vals[fld]:
-                cmd += ", %s"
-                vlist.append(d[fld])
-        cmd += ')'
+            fld = f["fld"]
+            cmd += ", %s"
+            vlist.append(d[fld])
+        cmd += ")"
         if self.debug:
             print(cmd % tuple(vlist))
             id = self.dbgid
             self.dbgid += 1
             return id
         try:
             self.cur.execute(cmd, tuple(vlist))
@@ -564,98 +705,196 @@
             return None
         try:
             self.cur.execute("select last_insert_id()")
             return list(self.cur.fetchone().values())[0]
         except _mysql_exceptions.Error as e:
             self.errorlist.append(e)
             return None
-            
+
     def configChange(self, idx, e, update=True):
+        """
+        Modify a configuration in the database.
+
+        Parameters
+        ----------
+        idx : int
+            An id for a configuration entry in the database.
+
+        e : dict
+            A dictionary containing updated values for some of the
+            database fields.
+
+        update : boolean
+            If True, update the timestamp on the entry.  (Defaults to
+            True.)
+
+        Returns
+        -------
+        Nothing.  Adds to transaction errorlist on failure.
+        """
         cmd = "update %s_cfg set " % self.table
         if update:
             cmd += "dt_updated = now()"
             sep = ", "
         else:
             sep = ""
         vlist = []
         try:
-            v = e['name']
+            v = e["name"]
             cmd += "%sname = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
+        except Exception:
             pass
         try:
-            v = e['config']
+            v = e["config"]
             cmd += "%sconfig = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
+        except Exception:
             pass
         try:
-            v = e['mutex']
+            v = e["mutex"]
             cmd += "%smutex = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
-            pass
-        try:
-            v = e['owner']
-            cmd += "%sowner = %%s" % sep
-            sep = ", "
-            vlist.append(v)
-        except:
+        except Exception:
             pass
         for f in self.cfgflds:
-            fld = f['fld']
+            fld = f["fld"]
             try:
-                v = e[fld]           # We have a new value!
-                cmd += "%s%s = %%s" % (sep, fld)
+                v = e[fld]  # We have a new value!
+                cmd += "{}{} = %s".format(sep, fld)
                 sep = ", "
                 vlist.append(v)
-            except:
-                pass                 # No change to this field!
-        cmd += ' where id = %s'
+            except Exception:
+                pass  # No change to this field!
+        cmd += " where id = %s"
         vlist.append(idx)
         if self.debug:
             print(cmd % tuple(vlist))
             return
         try:
             self.cur.execute(cmd, tuple(vlist))
         except _mysql_exceptions.Error as err:
             self.errorlist.append(err)
 
+    def _cleanHistory(self, cur, prev, diff):
+        """
+        Clean up the history a little for user display.
+
+        Get rid of internal fields, and generate a diff if
+        requested.
+        """
+        d = {'action': cur['action'], 'date': cur['dt_updated'], 'name': cur['name']}
+        if cur['action'] == 'delete':
+            return d
+        if cur['action'] == 'insert' or prev is None or not diff:
+            for fi in self.cfgflds:
+                f = fi['fld']
+                d[f] = cur[f]
+            return d
+        else:
+            # Generate a diff!
+            for fi in self.cfgflds:
+                f = fi['fld']
+                if prev[f] != cur[f]:
+                    d[f] = cur[f]
+            return d
+
+    def configHistory(self, idx, start=None, finish=None, diff=True):
+        """
+        Retrieve the history of the specified configuration between 
+        the specified dates.
+
+        start and finish are assumed to be datetime objects.  If
+        either or both is None, there is no time limit on that end.
+
+        If diff is true, only list how values have changed between
+        successive entries, otherwise give all field values.
+        """
+        try:
+            cmd = "select * from %s_cfg_log where id = %d" % (self.table, idx)
+            if start is not None:
+                if finish is not None:
+                    cmd = cmd + " and dt_updated between '%s' and '%s'" % (start, finish)
+                else:
+                    cmd = cmd + " and dt_updated >= '%s'" % start
+            elif finish is not None:
+                    cmd = cmd + " and dt_updated <= '%s'" % finish
+            self.cur.execute(cmd)
+            l = []
+            p = None
+            for r in self.cur.fetchall():
+                l.append(self._cleanHistory(r, p, diff))
+                p = r
+            return l
+        except Exception:
+            return []
+
     def objectDelete(self, idx):
+        """
+        Delete an object from the database.  Assumes inside a
+        transaction, but does not commit the change.
+
+        Parameters
+        ----------
+        idx : int
+            A database ID for the object to be deleted.
+
+        Returns
+        -------
+        Nothing
+
+        If the deletion fails, errors are appended to the transaction
+        errorlist.
+        """
         try:
             self.cur.execute("delete from %s where id = %%s" % self.table, (idx,))
         except _mysql_exceptions.Error as e:
             self.errorlist.append(e)
 
     def objectInsert(self, d):
-        cmd = "insert %s (name, config, owner, rec_base, category, mutex, dt_created, dt_updated, comment" % self.table
+        """
+        Insert a new object into the database, assuming inside a transaction.
+
+        Parameters
+        ----------
+        d : dict
+            A dictionary containing values for database fields.
+
+        Returns
+        -------
+        id : int
+            A new object ID, or None if this fails. Adds to transaction
+            errorlist on failure.
+        """
+        cmd = (
+            "insert %s (config, owner, rec_base, category, mutex, dt_created, dt_updated, comment"
+            % self.table
+        )
         for f in self.objflds:
-            if f['obj'] == False:
+            if f["obj"] is False:
                 continue
-            fld = f['fld']
+            fld = f["fld"]
             cmd += ", " + fld
-        cmd += ") values (%s, %s, %s, %s, %s, %s, now(), now(), %s"
-        vlist = [d['name']]
-        vlist.append(d['config'])
+        cmd += ") values (%s, %s, %s, %s, %s, now(), now(), %s"
+        vlist = [d["config"]]
         vlist.append(self.hutch)
-        vlist.append(d['rec_base'])
-        vlist.append(d['category'])
-        vlist.append(d['mutex'])
-        vlist.append(d['comment'])
+        vlist.append(d["rec_base"])
+        vlist.append(d["category"])
+        vlist.append(d["mutex"])
+        vlist.append(d["comment"])
         for f in self.objflds:
-            if f['obj'] == False:
+            if f["obj"] is False:
                 continue
-            fld = f['fld']
+            fld = f["fld"]
             cmd += ", %s"
             vlist.append(d[fld])
-        cmd += ')'
+        cmd += ")"
         if self.debug:
             print(cmd % tuple(vlist))
             id = self.dbgid
             self.dbgid += 1
             return id
         try:
             self.cur.execute(cmd, tuple(vlist))
@@ -665,248 +904,342 @@
             self.cur.execute("select last_insert_id()")
             return list(self.cur.fetchone().values())[0]
         except _mysql_exceptions.Error as e:
             self.errorlist.append(e)
             return None
 
     def objectChange(self, idx, e, update=True):
+        """
+        Modify an object in the database.
+
+        Parameters
+        ----------
+        idx : int
+            An id for a configuration entry in the database.
+
+        e : dict
+            A dictionary containing updated values for some of the
+            database fields.
+
+        update : boolean
+            If True, update the timestamp on the entry.  (Defaults to
+            True.)
+
+        Returns
+        -------
+        Nothing.  Adds to transaction errorlist on failure.
+        """
         cmd = "update %s set " % self.table
         if update:
             cmd += "dt_updated = now()"
             sep = ", "
         else:
             sep = ""
         vlist = []
         try:
-            v = e['name']
+            v = e["name"]
             cmd += "%sname = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
+        except Exception:
             pass
         try:
-            v = e['config']
+            v = e["config"]
             cmd += "%sconfig = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
+        except Exception:
             pass
         try:
-            v = e['rec_base']
+            v = e["rec_base"]
             cmd += "%srec_base = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
+        except Exception:
             pass
         try:
-            v = e['category']
+            v = e["category"]
             cmd += "%scategory = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
+        except Exception:
             pass
         try:
-            v = e['mutex']
+            v = e["mutex"]
             cmd += "%smutex = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
+        except Exception:
             pass
         try:
-            v = e['comment']
+            v = e["comment"]
             cmd += "%scomment = %%s" % sep
             sep = ", "
             vlist.append(v)
-        except:
+        except Exception:
             pass
         for f in self.objflds:
-            if f['obj'] == False:
+            if f["obj"] is False:
                 continue
-            fld = f['fld']
+            fld = f["fld"]
             try:
-                v = e[fld]           # We have a new value!
-            except:
+                v = e[fld]  # We have a new value!
+            except Exception:
                 continue
-            cmd += "%s%s = %%s" % (sep, fld)
+            cmd += "{}{} = %s".format(sep, fld)
             sep = ", "
             vlist.append(v)
-        cmd += ' where id = %s'
+        cmd += " where id = %s"
         vlist.append(idx)
         if self.debug:
             print(cmd % tuple(vlist))
             return
         try:
             self.cur.execute(cmd, tuple(vlist))
         except _mysql_exceptions.Error as err:
             self.errorlist.append(err)
 
-    def groupClear(self, id):
-        if self.debug:
-            print("delete from %s_cfg_grp where group_id = %d" % (self.table, id))
-            return True
-        try:
-            self.cur.execute("delete from %s_cfg_grp where group_id = %%s" % self.table, (id, ))
-            return True
-        except _mysql_exceptions.Error as e:
-            self.errorlist.append(e)
-            return False
-
-    def groupDelete(self, id):
-        if not self.groupClear(id):
-            return False
-        if self.debug:
-            print("delete from %s_grp where id = %d" % (self.table, id))
-            return True
-        try:
-            self.cur.execute("delete from %s_grp where id = %%s" % self.table, (id, ))
-            return True
-        except _mysql_exceptions.Error as e:
-            self.errorlist.append(e)
-            return False
-
-    def groupInsert(self, g):
-        if self.debug:
-            print("insert %s_grp (name, owner, active, dt_created, dt_updated) values (%s, %s, 0, now(), now())" % \
-                  (self.table, g['global']['name'], self.hutch))
-            print("select last_insert_id()")
-            id = self.dbgid
-            self.dbgid += 1
-        else:
-            try:
-                self.cur.execute("insert %s_grp (name, owner, active, dt_created, dt_updated) values (%%s, %%s, 0, now(), now())" \
-                                 % self.table, (g['global']['name'], self.hutch))
-                self.cur.execute("select last_insert_id()")
-                id = list(self.cur.fetchone().values())[0]
-            except _mysql_exceptions.Error as e:
-                self.errorlist.append(e)
-                return False
-        self.groupUpdate(id, g)
-
-    def groupUpdate(self, id, g):
-        if not self.groupClear(id):
-            return False
-        keys = g.keys()
-        keys.remove('global')
-        keys.sort()
-        seq = 0
-        for k in keys:
-            if g[k]['config'] != 0:
-                try:
-                    cmd = "insert %s_cfg_grp (group_id, config_id, port_id, dispseq)" % self.table
-                    cmd += "values (%s, %s, %s, %s)"
-                    try:
-                        port = str(g[k]['port'])
-                    except:
-                        port = "0"
-                    if self.debug:
-                        print(cmd % (str(id), str(g[k]['config']), port, str(seq)))
-                    else:
-                        self.cur.execute(cmd, (id, g[k]['config'], port, seq))
-                    seq += 1
-                except _mysql_exceptions.Error as e:
-                    self.errorlist.append(e)
-                    return False
-        try:
-            cmd = "update %s_grp set active = %%s, name = %%s, dt_updated = now() where id = %%s" % self.table
-            if self.debug:
-                print(cmd % (g['global']['active'], id))
-            else:
-                self.cur.execute(cmd, (g['global']['active'], g['global']['name'], id))
-            return True
-        except _mysql_exceptions.Error as e:
-            self.errorlist.append(e)
-            return False
-
-    def countInstance(self, chg):
-        if len(chg) == 0:
+    def countInstance(self, clist):
+        """
+        Count the number of objects that use one of the listed configurations.
+
+        Parameters
+        ----------
+        clist : list
+            A list of configuration IDs.
+
+        Returns
+        -------
+        cnt : int
+            The number of objects in the database using one of the listed
+            configurations.
+        """
+        if len(clist) == 0:
             return 0
         cmd = "select count(*) from %s where " % self.table
         p = ""
-        for v in chg:
+        for v in clist:
             cmd += "%sconfig = %d" % (p, v)
             p = " or "
         try:
             self.cur.execute(cmd)
             return list(self.cur.fetchone().values())[0]
         except _mysql_exceptions.Error as err:
             self.errorlist.append(err)
 
-    def getAutoCfg(self, d):
-        f = self.autoconfig
-        v = d[f]
-        cmd = "select max(seq) from %s_log where %s = %%s and owner = %%s and action != 'delete' group by id" % \
-              (self.table, f)
-        if self.debug:
-            print(cmd % (v, self.hutch))
-        try:
-            if self.cur.execute(cmd, (v, self.hutch)) != 1:
-                # Couldn't find it in our hutch, look in any!
-                cmd = "select max(seq) from %s_log where %s = %%s and action != 'delete' group by id" % \
-                      (self.table, f)
-                if self.debug:
-                    print(cmd % (v))
-                self.cur.execute(cmd, (v))
-            seq = list(self.cur.fetchone().values())[0]
-            cmd = "select * from %s_log where seq = %%s" % (self.table)
-            if self.debug:
-                print("debug?")
-                print(cmd % seq)
-            self.cur.execute(cmd, seq)
-            r = self.cur.fetchone()
-            try:
-                del r[f]
-            except:
-                pass
-            for f in self.unwanted:
+    def applyConfig(self, idx, cfg=None):
+        """
+        Apply the configuration of the specified object.
+
+        Parameters
+        ----------
+        idx : int / str
+            An object id or base PV name.
+
+        cfg : int
+            A configuration id, if idx is just a base PV name.
+
+        Returns
+        -------
+        Nothing.
+        """
+        vals = {}
+        if type(idx) == int:
+            vals.update(self.objs[idx])
+            vals.update(self.cfgs[vals["config"]])
+        else:
+            vals["rec_base"] = idx
+            vals.update(self.cfgs[cfg])
+        base = vals["rec_base"]
+        for s in self.setflds:
+            #
+            # Write zeros.
+            #
+            for f in s:
+                if self.fldmap[f]["readonly"] or vals[f] is None:
+                    continue
+                if self.fldmap[f]["writezero"]:
+                    try:
+                        z = self.fldmap[f]["enum"][0]
+                        haveenum = True
+                    except Exception:
+                        z = 0
+                        haveenum = False
+                    try:
+                        utils.caput(base + self.fldmap[f]["pv"], z, enum=haveenum)
+                    except Exception:
+                        pass
+            #
+            # Write values.
+            #
+            for f in s:
+                try:
+                    if vals[f] is None or self.fldmap[f]["readonly"]:
+                        continue
+                except Exception:
+                    continue  # If we just passed in a base PV, we might not have every field!
                 try:
-                    del r[f]
-                except:
+                    z = self.fldmap[f]["enum"][0]
+                    haveenum = True
+                except Exception:
+                    z = 0
+                    haveenum = False
+                try:
+                    utils.caput(base + self.fldmap[f]["pv"], vals[f], enum=haveenum)
+                except Exception:
                     pass
-            try:
-                # See the comment in ObjModel.setValue.  This is just bizarreness.
-                r['cfgname'] = r['config']
-                del r['config']
-            except:
-                pass
-            return r
-        except _mysql_exceptions.Error as err:
-            print(err)
-            return {}
 
-    def getConfig(self, idx, loop=[]):
-        if idx == None or idx in loop:
-            return {}
+    def applyAllConfigs(self):
+        """
+        Apply the current configuration to all objects in the database.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        Nothing.
+        """
+        for i in self.objs.keys():
+            self.applyConfig(i)
+
+    def diffConfig(self, idx, cfgidx=None):
+        """
+        Return the difference between the actual values of an object
+        and configured values.
+
+        Parameters
+        ----------
+        idx : int
+            An object id to find the differences for.
+
+        cfgidx : int
+            A configuration id to compare to.  If this is None, default
+            to the current configuration of the object.
+
+        Returns
+        -------
+        diff : dict
+            A dictionary mapping field names (str) to (actual,
+            configuration) tuples for each difference.
+        """
+        vals = {}
+        vals.update(self.objs[idx])
+        if cfgidx is None:
+            cfgidx = vals["config"]
+        vals.update(self.cfgs[cfgidx])
+        base = vals["rec_base"]
         d = {}
-        d.update(self.cfgs[idx])
-        haveval = {}
-        v = d['mutex']
-        if d['config'] != None:
-            lp = list(loop)
-            lp.append(idx)
-            vals = self.getConfig(d['config'], lp)   # Get the parent configuration
-            pmutex = vals['curmutex']
-            mutex = ""                               # Build the mutex from the set and inherited values.
-            for i in range(len(self.mutex_sets)):
-                if self.mutex_obj[i]:
-                    mutex += ' '
-                elif v[i] != ' ':
-                    mutex += v[i]
-                else:
-                    mutex += pmutex[i]
-            d['curmutex'] = mutex
-        else:
-            d['curmutex'] = v
-        for (k, v) in d.items():
-            if k[:3] != 'PV_' and k[:4] != 'FLD_':
-                continue
-            if v == None:
-                # This key might have a value because it is the unset element of a mutex set!
-                haveval[k] = chr(self.fldmap[k]['colorder']+0x40) in d['curmutex']
-            else:
-                haveval[k] = True
-            if not haveval[k]:
+        for s in self.setflds:
+            for f in s:
+                if vals[f] is None or self.fldmap[f]["readonly"]:
+                    continue
+                n = base + self.fldmap[f]["pv"]
                 try:
-                    d[k] = vals[k]     # Try to get the parent value.
-                except:
-                    d[k] = None
-        d['_haveval'] = haveval
+                    self.fldmap[f]["enum"][0]
+                    haveenum = True
+                except Exception:
+                    haveenum = False
+                v = utils.caget(n, enum=haveenum)
+                if type(v) == float:
+                    if v == 0.0:
+                        if abs(v - vals[f]) > 0.00000001:
+                            d[f] = (v, vals[f])
+                    else:
+                        if abs((v - vals[f]) / v) > 0.00000001:
+                            d[f] = (v, vals[f])
+                else:
+                    if v != vals[f]:
+                        d[f] = (v, vals[f])
         return d
+
+    def getActualConfig(self, idx):
+        """
+        Get the actual values of all of the configuration parameters of an object.
+
+        Parameters
+        ----------
+        idx : int
+            An object id.
+
+        Returns
+        -------
+        cdict : dict
+            A dictionary mapping field names (str) to values.
+        """
+        base = self.objs[idx]["rec_base"]
+        d = {}
+        for f in self.cfgflds:
+            n = base + f["pv"]
+            try:
+                f["enum"][0]
+                haveenum = True
+            except Exception:
+                haveenum = False
+            v = utils.caget(n, enum=haveenum)
+            d[f["fld"]] = v
+        return d
+
+    def matchConfigs(self, pattern, substr=True, ci=True, parent=None):
+        """
+        Search for configuration names in the database.
+
+        Parameters
+        ----------
+        pattern : str
+            The pattern to search for.  "." matches any character, "*" matches any string.
+            These special characters can be quoted using "\".
+
+        substr : boolean
+            If True, the pattern should match a substring of the
+            configuration name.  Otherwise, the pattern must match the
+            entire configuration name.  (Defaults to True.)
+
+        ci : boolean
+            If True, the match is case insensitive, otherwise it is case
+            sensitive.  (Defaults to True.)
+
+        parent : str
+            The name of a parent configuration.  Only match children of
+            this configuration.
+
+        Returns
+        -------
+        clist : list
+            A list of configuration names matching the pattern.
+        """
+        p = pattern.replace(r"\.", r"\DOT").replace(r"\*", r"\SPLAT")
+        p = p.replace("_", r"\_").replace("%", r"\%")
+        p = p.replace("*", "%").replace(".", "_")
+        p = p.replace(r"\DOT", ".").replace(r"\SPLAT", "*")
+        if substr:
+            p = "%"+p+"%"
+        if parent is not None:
+            pid = self.cfgmap[parent]
+            self.cur.execute("select name from %s_cfg where name %slike '%s' and config = %d" %
+                             (self.table, "collate latin1_general_ci " if ci else "",
+                              p, pid))
+        else:
+            self.cur.execute("select name from %s_cfg where name %slike '%s'" %
+                             (self.table, "collate latin1_general_ci " if ci else "",
+                              p))
+        return [d['name'] for d in self.cur.fetchall()]
+
+    def hutchInsert(self, hutchname):
+        """
+        Add a new hutch.
+
+        Parameters
+        ----------
+        hutchname : str
+            The new hutchname.  The owner will be all lowercase, the
+            base config will be all uppercase.
+        """
+        newowner = hutchname.lower()
+        newconfig = hutchname.upper()
+        d = self.cfgs[0].copy()
+        d['name'] = newconfig
+        d['config'] = 0
+        id = self.configInsert(d)
+        if id is not None:
+            self.cur.execute('insert %s_update (tbl_name, dt_updated) values ("%s", now());' % (self.table, newowner))
```

### Comparing `pmgr-2.0.2/pmgr/param.py` & `pmgr-2.1.3/pmgr/param.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,80 @@
+import os
+import pwd
+
 from PyQt5 import QtCore, QtGui
-import pwd, os
 
 AUTH_FILE = "/reg/g/pcds/pyps/config/%s/pmgr.auth"
 params = None
 
+
 def equal(v1, v2):
     try:
         if type(v1) == float:
             # I hate floating point.  OK, we need to be "close", but if we are *at* zero
             # the "close" test fails!
             return v1 == v2 or abs(v1 - v2) < (abs(v1) + abs(v2)) * 1e-12
         else:
             return v1 == v2
-    except:
+    except Exception:
         return False
 
-class param_structure(object):
+
+class param_structure:
     def __init__(self):
         self.myuid = pwd.getpwuid(os.getuid())[0]
         self.user = None
-        self.almond = QtGui.QColor(255,235,205)
+        self.almond = QtGui.QColor(255, 235, 205)
         self.almond.name = "almond"
-        self.white  = QtGui.QColor(255,255,255)
+        self.white = QtGui.QColor(255, 255, 255)
         self.white.name = "white"
-        self.gray   = QtGui.QColor(160,160,160)
+        self.gray = QtGui.QColor(160, 160, 160)
         self.gray.name = "gray"
-        self.ltgray = QtGui.QColor(224,224,224)
+        self.ltgray = QtGui.QColor(224, 224, 224)
         self.ltgray.name = "ltgray"
-        self.ltblue = QtGui.QColor(0,  255,255)
+        self.ltblue = QtGui.QColor(0, 255, 255)
         self.ltblue.name = "ltblue"
-        self.blue   = QtGui.QColor(QtCore.Qt.blue)
+        self.blue = QtGui.QColor(QtCore.Qt.blue)
         self.blue.name = "blue"
-        self.red    = QtGui.QColor(QtCore.Qt.red)
+        self.red = QtGui.QColor(QtCore.Qt.red)
         self.red.name = "red"
-        self.black  = QtGui.QColor(QtCore.Qt.black)
+        self.black = QtGui.QColor(QtCore.Qt.black)
         self.black.name = "black"
         self.purple = QtGui.QColor(204, 0, 102)
         self.purple.name = "purple"
-        self.cfgdialog       = None
-        self.colusedialog    = None
-        self.colsavedialog   = None
-        self.deriveddialog   = None
-        self.confirmdialog   = None
+        self.cfgdialog = None
+        self.colusedialog = None
+        self.colsavedialog = None
+        self.deriveddialog = None
+        self.confirmdialog = None
         self.settings = ("SLAC", "ParamMgr")
-        self.debug  = False
-        self.applyOK  = False
+        self.debug = False
+        self.applyOK = False
 
         self.ui = None
         self.objmodel = None
         self.cfgmodel = None
         self.db = None
         self.pobj = None
 
         self.hutch = None
         self.table = None
 
         self.PROTECTED = 0
-        self.MANUAL    = 1
-        self.AUTO      = 2
-        self.catenum   = ["Protected", "Manual", "Auto"]    # Database names.
-        self.setCatEnum(["Protected", "Manual"])    # Displayed names.
+        self.MANUAL = 1
+        self.AUTO = 2
+        self.catenum = ["Protected", "Manual", "Auto"]  # Database names.
+        self.setCatEnum(["Protected", "Manual"])  # Displayed names.
 
     def setCatEnum(self, l):
         self.catenum2 = l
-        if self.ui != None:
+        if self.ui is not None:
             self.ui.actionProtected.setText("Show " + l[0])
             self.ui.actionManual.setText("Show " + l[1])
 
     def setTable(self, v):
         self.table = v
-            
+
     def setHutch(self, v):
         self.hutch = v
         lines = open(AUTH_FILE % v).readlines()
         self.auth_users = [l.strip() for l in lines]
```

### Comparing `pmgr-2.0.2/pmgr/pmgr.py` & `pmgr-2.1.3/pmgr/pmgr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 #!/usr/bin/env python
 import sys
-import threading
+import os
+import grp
 
-from PyQt5 import QtCore, QtGui, QtWidgets
 from psp.options import Options
+from PyQt5 import QtCore, QtWidgets
 
-from .pmgr_ui import Ui_MainWindow
-from .ObjModel import ObjModel
+from . import dialogs, param, utils
 from .CfgModel import CfgModel
 from .db import db
+from .dialogs import load_ui_file
 from .MyDelegate import MyDelegate
-from . import dialogs
-from . import param
-from . import auth_ui
-from . import utils
+from .ObjModel import ObjModel
+
+AUTHGROUP = None
 
 ######################################################################
 
+
 class authdialog(QtWidgets.QDialog):
     def __init__(self, parent=None):
-      QtWidgets.QWidget.__init__(self, parent)
-      self.ui = auth_ui.Ui_Dialog()
-      self.ui.setupUi(self)
+        QtWidgets.QWidget.__init__(self, parent)
+        self.ui = load_ui_file("auth.ui")()
+        self.ui.setupUi(self)
+
 
 ######################################################################
 
-class GraphicUserInterface(QtWidgets.QMainWindow):
 
+class GraphicUserInterface(QtWidgets.QMainWindow):
     def __init__(self):
         QtWidgets.QMainWindow.__init__(self)
 
         self.authdialog = authdialog(self)
         self.utimer = QtCore.QTimer()
-        
-        param.params.ui = Ui_MainWindow()
+
+        param.params.ui = load_ui_file("pmgr.ui")()
         ui = param.params.ui
 
         ui.setupUi(self)
 
         # Not sure how to do this in designer, so we put it randomly and move it now.
         ui.statusbar.addWidget(ui.userLabel)
         self.setUser(param.params.myuid)
-        
-        self.setWindowTitle("Parameter Manager for %s (%s)" % (param.params.hutch.upper(), param.params.table))
+
+        self.setWindowTitle(
+            "Parameter Manager for {} ({})".format(
+                param.params.hutch.upper(), param.params.table
+            )
+        )
 
         ui.objectTable.verticalHeader().hide()
         ui.objectTable.setCornerButtonEnabled(False)
         ui.objectTable.horizontalHeader().setSectionsMovable(True)
 
         ui.configTable.verticalHeader().hide()
         ui.configTable.setCornerButtonEnabled(False)
         ui.configTable.horizontalHeader().setSectionsMovable(True)
 
         param.params.db = db()
-        
+
         ui.menuView.addAction(ui.configWidget.toggleViewAction())
         ui.configWidget.setWindowTitle(param.params.table + " configurations")
         param.params.cfgmodel = CfgModel()
         ui.configTable.init(param.params.cfgmodel, 0, param.params.cfgmodel.mutable)
         ui.configTable.setShowGrid(True)
         ui.configTable.resizeColumnsToContents()
         ui.configTable.setItemDelegate(MyDelegate(self))
@@ -65,26 +71,28 @@
         ui.menuView.addAction(ui.objectWidget.toggleViewAction())
         ui.objectWidget.setWindowTitle(param.params.table + " objects")
         param.params.objmodel = ObjModel()
         ui.objectTable.init(param.params.objmodel, 0, param.params.objmodel.mutable)
         ui.objectTable.setShowGrid(True)
         ui.objectTable.resizeColumnsToContents()
         ui.objectTable.setSortingEnabled(True)
-        ui.objectTable.sortByColumn(param.params.objmodel.pvcol, QtCore.Qt.AscendingOrder)
+        ui.objectTable.sortByColumn(
+            param.params.objmodel.pvcol, QtCore.Qt.AscendingOrder
+        )
         ui.objectTable.setItemDelegate(MyDelegate(self))
 
         param.params.objmodel.setupContextMenus(ui.objectTable)
         param.params.cfgmodel.setupContextMenus(ui.configTable)
 
-        param.params.cfgdialog       = dialogs.cfgdialog(param.params.cfgmodel, self)
-        param.params.colsavedialog   = dialogs.colsavedialog(self)
-        param.params.colusedialog    = dialogs.colusedialog(self)
-        param.params.deriveddialog   = dialogs.deriveddialog(self)
-        param.params.confirmdialog   = dialogs.confirmdialog(self)
-        param.params.chowndialog     = dialogs.chowndialog(self)
+        param.params.cfgdialog = dialogs.cfgdialog(param.params.cfgmodel, self)
+        param.params.colsavedialog = dialogs.colsavedialog(self)
+        param.params.colusedialog = dialogs.colusedialog(self)
+        param.params.deriveddialog = dialogs.deriveddialog(self)
+        param.params.confirmdialog = dialogs.confirmdialog(self)
+        param.params.chowndialog = dialogs.chowndialog(self)
 
         param.params.db.objchange.connect(param.params.objmodel.objchange)
         param.params.db.cfgchange.connect(param.params.objmodel.cfgchange)
         param.params.db.cfgchange.connect(param.params.cfgmodel.cfgchange)
 
         param.params.cfgmodel.newname.connect(param.params.cfgmodel.haveNewName)
         param.params.cfgmodel.newname.connect(param.params.objmodel.haveNewName)
@@ -131,25 +139,33 @@
             ui.applyButton.hide()
         ui.actionProtected.triggered.connect(param.params.objmodel.doShow)
         ui.actionManual.triggered.connect(param.params.objmodel.doShow)
         ui.actionTrack.triggered.connect(param.params.objmodel.doTrack)
         ui.actionAuth.triggered.connect(self.doAuthenticate)
         ui.actionExit.triggered.connect(self.doExit)
         self.utimer.timeout.connect(self.unauthenticate)
-        ui.objectTable.selectionModel().selectionChanged.connect(param.params.objmodel.selectionChanged)
+        ui.objectTable.selectionModel().selectionChanged.connect(
+            param.params.objmodel.selectionChanged
+        )
         # MCB - Sigh. I should just make FreezeTableView actually work.
-        ui.objectTable.cTV.selectionModel().selectionChanged.connect(param.params.objmodel.selectionChanged)
+        ui.objectTable.cTV.selectionModel().selectionChanged.connect(
+            param.params.objmodel.selectionChanged
+        )
 
     def closeEvent(self, event):
         settings = QtCore.QSettings(param.params.settings[0], param.params.settings[1])
         settings.beginGroup(param.params.table)
         settings.setValue("geometry", self.saveGeometry())
         settings.setValue("windowState", self.saveState())
-        settings.setValue("cfgcol/default", param.params.ui.configTable.saveHeaderState())
-        settings.setValue("objcol/default", param.params.ui.objectTable.saveHeaderState())
+        settings.setValue(
+            "cfgcol/default", param.params.ui.configTable.saveHeaderState()
+        )
+        settings.setValue(
+            "objcol/default", param.params.ui.objectTable.saveHeaderState()
+        )
         settings.setValue("objsel", param.params.objmodel.getObjSel())
         QtWidgets.QMainWindow.closeEvent(self, event)
 
     def doExit(self):
         self.close()
 
     def setUser(self, user):
@@ -158,65 +174,68 @@
 
     def authenticate_user(self, user="", password=""):
         if user == "":
             self.setUser(param.params.myuid)
             return True
         if utils.authenticate_user(user, password):
             self.setUser(user)
-            self.utimer.start(10 * 60000) # Ten minutes!
+            self.utimer.start(10 * 60000)  # Ten minutes!
             return True
         else:
-            QtWidgets.QMessageBox.critical(None, "Error", "Invalid Password",
-                                       QtWidgets.QMessageBox.Ok)
+            QtWidgets.QMessageBox.critical(
+                None, "Error", "Invalid Password", QtWidgets.QMessageBox.Ok
+            )
             return False
 
     def doAuthenticate(self):
         result = self.authdialog.exec_()
         user = str(self.authdialog.ui.nameEdit.text())
         password = str(self.authdialog.ui.passEdit.text())
         self.authdialog.ui.passEdit.setText("")
         if result == QtWidgets.QDialog.Accepted:
             if not self.authenticate_user(user, password):
                 self.unauthenticate()
 
     def unauthenticate(self):
         self.utimer.stop()
         self.authenticate_user()
-        
+
 
 def main():
-    #MCB QtWidgets.QApplication.setGraphicsSystem("raster")
+    if AUTHGROUP is not None and grp.getgrnam(AUTHGROUP).gr_gid not in os.getgroups():
+        raise Exception("You are not a member of %s and are not authorized to run the parameter manager!" % AUTHGROUP)
+    # MCB QtWidgets.QApplication.setGraphicsSystem("raster")
     param.params = param.param_structure()
-    app = QtWidgets.QApplication([''])
-  
+    app = QtWidgets.QApplication([""])
+
     # Options( [mandatory list, optional list, switches list] )
-    options = Options(['hutch', 'type'], [], ['debug', 'applyenable', 'dev', 'help'])
+    options = Options(["hutch", "type"], [], ["debug", "applyenable", "dev", "help"])
     try:
         options.parse()
     except Exception as msg:
         options.usage(str(msg))
         sys.exit()
 
     if options.help is not None:
-        options.usage(str(msg))
+        options.usage("")  # TODO: 'msg' was unset here
         sys.exit()
 
     param.params.setHutch(options.hutch.lower())
     param.params.setTable(options.type)
     param.params.debug = False if options.debug is None else True
     param.params.applyOK = False if options.applyenable is None else True
     param.params.prod = True if options.dev is None else False
     gui = GraphicUserInterface()
     param.params.setTable(options.type)  # Sigh, do this again to fix dropdown.
     # MCB - We need a better way of doing this.
     if options.type == "ims_motor":
-        param.params.setCatEnum(["Beamline", "Dumb"]) # Displayed names.
+        param.params.setCatEnum(["Beamline", "Dumb"])  # Displayed names.
     try:
         gui.show()
         retval = app.exec_()
     except KeyboardInterrupt:
         app.exit(1)
     sys.exit(retval)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `pmgr-2.0.2/pmgr/pmgrAPI.py` & `pmgr-2.1.3/pmgr/pmgrAPI.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .pmgrobj import pmgrobj
+from datetime import datetime
 
-class pmgrAPI(object):
+class pmgrAPI:
     """
     An application interface to the parameter manager.
 
     Parameters
     ----------
     table : str
         The type of object being configured.  (Probably "ims_motor".)
 
     hutch : str
         The name of the hutch used to retrieve objects from the database.
     """
+
     def __init__(self, table, hutch):
         self.hutch = hutch.upper()
         self.pm = pmgrobj(table, hutch)
 
     @staticmethod
     def _search(dl, f, v):
         """
@@ -39,48 +41,47 @@
             of the field.  Raises an exception if no match.
         """
         for d in dl.values():
             if d[f] == v:
                 return d
         raise Exception("%s not found!" % v)
 
-    @staticmethod
-    def _fixmutex(d, mutex):
+    def _fixmutex(self, d, mutex):
         """
-        A private method to fix the configuration fields to match the 
+        A private method to fix the configuration fields to match the
         mutex condition.
 
         The "mutex" field is slightly complicated.  The general idea is
         that there can be sets of fields that when you set all but one
-        field in the set, the remaining field is calculated from the 
+        field in the set, the remaining field is calculated from the
         others.  For each such set, the "mutex" string indicates which
         field is the derived one.  (Derived fields should not have values
         assigned in the database.)
 
         Parameters
         ----------
         d : dict
             A configuration dictionary.
 
         mutex: str
-            A string with one character per mutex set.  The character 
+            A string with one character per mutex set.  The character
             is a space if this set is not used.  Otherwise, the character
             encodes a field identified by column order, chr(colorder + 64).
 
         Returns
         -------
         d : dict
             The original configuration dictionary with the derived fields
             removed.
         """
         for c in mutex:
-            if c != ' ':
+            if c != " ":
                 try:
-                    del d[self.pm.objflds[ord[c]-65]['name']]
-                except:
+                    del d[self.pm.objflds[ord(c) - 65]["name"]]
+                except Exception:
                     pass
         return d
 
     def update_db(self):
         """
         Re-read the configuration database, if needed.
 
@@ -107,16 +108,33 @@
         -------
         config : str
             The name of the configuration associated with the PV.
 
         Throws an exception if the PV is not in the database.
         """
         self.update_db()
-        d = self._search(self.pm.objs, 'rec_base', pv)
-        return self.pm.cfgs[d['config']]['name']
+        d = self._search(self.pm.objs, "rec_base", pv)
+        return self.pm.cfgs[d["config"]]["name"]
+
+    def get_config_values(self, cfgname):
+        """
+        Return the values in a configuration.
+
+        Parameters
+        ----------
+        config : str
+            The name of the configuration.
+
+        Returns
+        -------
+        A dictionary mapping field names to configured values.
+        """
+        d = self._search(self.pm.cfgs, 'name', cfgname)
+        d = d.copy()  # Make a copy, since we don't know what the user is going to do with this!
+        return d
 
     def set_config(self, pv, cfgname, o=None):
         """
         Set the configuration for a given PV base.
 
         Parameters
         ----------
@@ -129,21 +147,21 @@
         Returns
         -------
         Nothing.  Raises an exception if the assignment fails for any reason.
         """
         #
         # NOTE: o is a private parameter.  It is an object dictionary for the pv,
         # and is used internally to avoid an extra update and lookup.
-        # 
+        #
         if o is None:
             self.update_db()
-            o = self._search(self.pm.objs, 'rec_base', pv)
-        d = self._search(self.pm.cfgs, 'name', cfgname)
+            o = self._search(self.pm.objs, "rec_base", pv)
+        d = self._search(self.pm.cfgs, "name", cfgname)
         self.pm.start_transaction()
-        self.pm.objectChange(o['id'], {'config': d['id']})
+        self.pm.objectChange(o["id"], {"config": d["id"]})
         el = self.pm.end_transaction()
         if el != []:
             raise Exception("DB Errors", el)
 
     def apply_config(self, pv, cfgname=None):
         """
         Apply the configuration for a given PV base.
@@ -160,25 +178,25 @@
         Returns
         -------
         Nothing.  Raises an exception if the application fails for any reason.
         """
         self.update_db()
         try:
             # See if the object is in the database.
-            o = self._search(self.pm.objs, 'rec_base', pv)
-        except:
+            o = self._search(self.pm.objs, "rec_base", pv)
+        except Exception:
             # It isn't.  So use the alternative form of applyConfig.
-            c = self._search(self.pm.cfgs, 'name', cfgname)
-            self.pm.applyConfig(pv, cfg=c['id'])
+            c = self._search(self.pm.cfgs, "name", cfgname)
+            self.pm.applyConfig(pv, cfg=c["id"])
             return
         # The object is in the database!  Set its config, and apply!
         if cfgname is not None:
             self.set_config(pv, cfgname, o=o)
             self.update_db()
-        self.pm.applyConfig(o['id'])
+        self.pm.applyConfig(o["id"])
 
     def diff_config(self, pv, cfgname=None):
         """
         Find the differences between the actual motor settings and the
         configuration.
 
         Parameters
@@ -195,20 +213,20 @@
         diff : dict
             A dictionary mapping field names to (actual, config) tuples of
             differing values.
 
         Raises an exception if the comparison fails for any reason.
         """
         self.update_db()
-        o = self._search(self.pm.objs, 'rec_base', pv)
+        o = self._search(self.pm.objs, "rec_base", pv)
         if cfgname is None:
             cfgidx = None
         else:
-            cfgidx = self._search(self.pm.cfgs, 'name', cfgname)['id']
-        return self.pm.diffConfig(o['id'], cfgidx)
+            cfgidx = self._search(self.pm.cfgs, "name", cfgname)["id"]
+        return self.pm.diffConfig(o["id"], cfgidx)
 
     def save_config(self, pv, cfgname=None, overwrite=False, parent=None):
         """
         Save the current motor settings into the database.
 
         Parameters
         ----------
@@ -218,66 +236,66 @@
         cfgname : str
             The name of the configuration to save.  If this is None, use
             the default configuration in the database.  If this is not
             None, change the motor entry to use the new configuration
             after it is saved.
 
         overwrite : boolean
-            If cfgname is not None and is an existing configuration, 
+            If cfgname is not None and is an existing configuration,
             overwrite it if this is True, otherwise throw an exception.
 
         parent : str
-            The name of the parent configuration, if this is a new 
+            The name of the parent configuration, if this is a new
             configuration.  If this is None, default to the uppercase
             hutch name.
 
         Returns
         -------
         Nothing.  Raises an exception if the this fails for any reason.
         """
         self.update_db()
-        o = self._search(self.pm.objs, 'rec_base', pv)
+        o = self._search(self.pm.objs, "rec_base", pv)
         if cfgname is None:
             # Default to overwriting the existing configuration.
-            do = self.pm.cfgs[o['config']]
-            cfgname = do['name']
+            do = self.pm.cfgs[o["config"]]
+            cfgname = do["name"]
             overwrite = True
         else:
             try:
-                do = self._search(self.pm.cfgs, 'name', cfgname)
-            except:
+                do = self._search(self.pm.cfgs, "name", cfgname)
+            except Exception:
                 do = None
                 overwrite = False
             if do is not None and not overwrite:
                 raise Exception("Configuration %s already exists!" % cfgname)
-        d = self.pm.getActualConfig(o['id'])
+        d = self.pm.getActualConfig(o["id"])
         if overwrite:
-            d = self._fixmutex(d, do['mutex'])
+            d = self._fixmutex(d, do["mutex"])
             self.pm.start_transaction()
-            self.pm.configChange(o['config'], d)
+            self.pm.configChange(o["config"], d)
             el = self.pm.end_transaction()
             if el != []:
                 raise Exception("DB Errors", el)
         else:
             # Add a new configuration
             if parent is None:
                 parent = self.hutch
-            p = self._search(self.pm.cfgs, 'name', parent)
-            d['mutex'] = p['mutex']
-            d['config'] = p['id']
-            d = self._fixmutex(d, p['mutex'])
-            d['name'] = cfgname
+            p = self._search(self.pm.cfgs, "name", parent)
+            d["mutex"] = p["mutex"]
+            d["config"] = p["id"]
+            d = self._fixmutex(d, p["mutex"])
+            d["name"] = cfgname
             self.pm.start_transaction()
             self.pm.configInsert(d)
             el = self.pm.end_transaction()
             if el != []:
                 raise Exception("DB Errors", el)
             self.set_config(pv, cfgname)
 
-    def match_config(self, pattern, substr=True, ci=True):
+    def match_config(self, pattern, substr=True, ci=True, parent=None):
         """
         Find configurations that match a given pattern.
 
         Parameters
         ----------
         pattern : str
             The pattern to look for.  "." matches any character, and "*"
@@ -287,17 +305,91 @@
             If True, match a substring, otherwise match the entire
             configuration name.  (Default to True.)
 
         ci : boolean
             If True, do a case insensitive match, otherwise be case
             sensitive.  (Default to True.)
 
+        parent : str
+            The name of a parent configuration.  Only match children of
+            this configuration.
+
         Returns
         -------
         clist : list
             A list of configuration names (strings) that match the pattern.
 
         Throws an exception if there is a database problem.
         """
         self.update_db()
-        return self.pm.matchConfigs(pattern, substr, ci)
+        return self.pm.matchConfigs(pattern, substr, ci, parent)
 
+    def add_hutch(self, newhutch):
+        """
+        Add a new hutch.
+
+        Parameters
+        ----------
+        hutch : str
+            The name of the new hutch.  Case doesn't matter: the main
+            configuration will be all uppercase, and the new owner will
+            be all lowercase.
+        """
+        self.pm.start_transaction()
+        self.pm.hutchInsert(newhutch)
+        el = self.pm.end_transaction()
+        if el != []:
+            raise Exception("DB Errors", el)
+
+    @staticmethod
+    def _get_datetime(s):
+        """
+        Try to convert a string into a datetime object.  The following
+        conversions are attempted:
+             ISO format
+             mm/dd/yyyy
+             mm/dd/yyyy hh:mm
+        If all three fail, a ValueError exception is raised.
+        """
+        try:
+            return datetime.fromisoformat(s)
+        except ValueError:
+            pass
+        try:
+            return datetime.strptime(s, "%m/%d/%Y %H:%M")
+        except ValueError:
+            pass
+        try:
+            return datetime.strptime(s, "%m/%d/%Y")
+        except ValueError:
+            pass
+        raise ValueError("Not a valid date: %s" % s)
+
+    def config_history(self, cfgname, start=None, finish=None, diff=False):
+        """
+        Return the history of a configuration.
+
+        Parameters
+        ----------
+        config : str
+            The name of the configuration.
+
+        start, finish: date
+            The date range of interest (None == no limit).  These can be datetime
+            objects, or strings that are interpreted as either isoformat dates,
+            "mm/dd/yyyy" dates, or "mm/dd/yyyy hh:mm".  Formatting is rather
+            strict.
+
+        diff: boolean
+            Should updates be listed in full, or as a difference from the previous?
+
+        Returns
+        -------
+        A list of dictionaries mapping field names to configured values.  The "action"
+        keyword indicates what has been done here: "insert", "update" or "delete"
+        """
+        if type(start) == str:
+            start = self._get_datetime(start)
+        if type(finish) == str:
+            finish = self._get_datetime(start)
+        d = self._search(self.pm.cfgs, 'name', cfgname)
+        return self.pm.configHistory(d['id'], start, finish, diff)
```

### Comparing `pmgr-2.0.2/pmgr/pmgrUtils.cfg` & `pmgr-2.1.3/pmgr/pmgrUtils.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
 # pmgr becomes gets used for more devices. The scripts *should* be able to
 # handle different objtypes so long as they are in the parameter manager. Simply
 # add them to this list for compatibility.
 supportedObjTypes = ims_motor
 # Note: All of the print statements say motor at the moment. If new devices are
 # added, this is something that should be changed though it does not affect the
 # performance of the script.
-
```

### Comparing `pmgr-2.0.2/pmgr/utils.py` & `pmgr-2.1.3/pmgr/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from PyQt5 import QtCore, QtGui, QtWidgets
 import threading
 
 import kerberos
-from psp.Pv import Pv
 import pyca
+from psp.Pv import Pv
+from PyQt5 import QtWidgets
 
 from . import param
 
 ######################################################################
-       
+
+
 #
 # Class to support for context menus in DropTableView.  The API is:
 #     isActive(table, index)
 #         - Return True is this menu should be displayed at this index
 #           in the table.
 #     doMenu(table, pos, index)
 #         - Show/execute the menu at location pos/index in the table.
@@ -38,14 +39,15 @@
             The current location in the view.
 
         Returns
         -------
         active : boolean
             Return True if the menu should be displayed.
     """
+
     def __init__(self, isAct=None):
         QtWidgets.QMenu.__init__(self)
         self.isAct = isAct
         self.actions = []
         self.havecond = False
 
     def addAction(self, name, action, cond=None):
@@ -68,15 +70,15 @@
             index : QModelIndex / int
                 The location in the view being pointed at.
 
             Returns
             -------
             Nothing.
 
-        cond : function 
+        cond : function
             A function that makes this menu item conditional.
 
             Parameters
             ----------
             table : TableView / HeaderView
                 The view being pointed at.
 
@@ -84,15 +86,15 @@
                 The location in the view being pointed at.
 
             Returns
             -------
             active : boolean
                 True if this menu item should be active.
         """
-        if cond != None:
+        if cond is not None:
             self.havecond = True
         self.actions.append((name, action, cond))
         QtWidgets.QMenu.addAction(self, name)
 
     def isActive(self, table, index):
         """
         Determine if this menu should be active, and if so, rebuild it
@@ -108,27 +110,27 @@
 
         Returns
         -------
         active : boolean
             Return True if this menu should be displayed, rebuilding it
             if necessary.
         """
-        if self.isAct == None or self.isAct(table, index):
+        if self.isAct is None or self.isAct(table, index):
             if self.havecond:
                 self.clear()
                 for name, action, cond in self.actions:
-                    if cond == None or cond(table, index):
+                    if cond is None or cond(table, index):
                         QtWidgets.QMenu.addAction(self, name)
             return True
         else:
             return False
 
     def doMenu(self, table, pos, index):
         """
-        Display the menu at the specified position.  If an action is 
+        Display the menu at the specified position.  If an action is
         selected, execute it.
 
         table : TableView / HeaderView
             The current view being pointed at.
 
         pos : QPoint
             The position where a context menu was requested.
@@ -141,154 +143,171 @@
         Nothing
         """
         if type(index) == int:
             gpos = table.horizontalHeader().viewport().mapToGlobal(pos)
         else:
             gpos = table.viewport().mapToGlobal(pos)
         selectedItem = self.exec_(gpos)
-        if selectedItem != None:
+        if selectedItem is not None:
             txt = selectedItem.text()
             for name, action, cond in self.actions:
                 if txt == name:
                     action(table, index)
                     return
 
+
 ######################################################################
 
 #
 # Utility functions to deal with PVs.
 #
 
-def caput(pvname,value,timeout=1.0,**kw):
+
+def caput(pvname, value, timeout=1.0, **kw):
     try:
         pv = Pv(pvname)
         pv.connect(timeout)
         pv.get(ctrl=False, timeout=timeout)
         try:
-            if kw['enum']:
+            if kw["enum"]:
                 pv.set_string_enum(True)
-        except:
+        except Exception:
             pass
         pv.put(value, timeout=timeout)
         pv.disconnect()
     except pyca.pyexc as e:
-        print('pyca exception: %s' %(e))
+        print("pyca exception: %s" % (e))
     except pyca.caexc as e:
-        print('channel access exception: %s' %(e))
+        print("channel access exception: %s" % (e))
+
 
-def caget(pvname,timeout=1.0,**kw):
+def caget(pvname, timeout=1.0, **kw):
     try:
         pv = Pv(pvname)
         pv.connect(timeout)
         try:
-            if kw['enum']:
+            if kw["enum"]:
                 pv.set_string_enum(True)
-        except:
+        except Exception:
             pass
         pv.get(ctrl=False, timeout=timeout)
         v = pv.value
         pv.disconnect()
         return v
     except pyca.pyexc as e:
-        print('pyca exception: %s' %(e))
+        print("pyca exception: %s" % (e))
         return None
     except pyca.caexc as e:
-        print('channel access exception: %s' %(e))
+        print("channel access exception: %s" % (e))
         return None
 
+
 def __get_callback(pv, e):
     if e is None:
         pv.get_done.set()
         pv.disconnect()
         pyca.flush_io()
 
+
 #
 # Do an asynchronous caget, but notify a threading.Event after it
 # completes instead of just waiting.
 #
 def caget_async(pvname):
     try:
         pv = Pv(pvname)
         pv.get_done = threading.Event()
         pv.connect_cb = lambda isconn: __connect_callback(pv, isconn)
         pv.getevt_cb = lambda e=None: __get_callback(pv, e)
         pv.connect(-1)
         return pv
     except pyca.pyexc as e:
-        print('pyca exception: %s' %(e))
+        print("pyca exception: %s" % (e))
         return None
     except pyca.caexc as e:
-        print('channel access exception: %s' %(e))
+        print("channel access exception: %s" % (e))
         return None
 
+
 def connectPv(name, timeout=-1.0):
     try:
         pv = Pv(name)
         if timeout < 0:
             pv.save_connect_cb = pv.connect_cb
             pv.connect_cb = lambda isconn: __connect_callback(pv, isconn)
             pv.connect(timeout)
         else:
             pv.connect(timeout)
             pv.get(ctrl=False, timeout=timeout)
         return pv
-    except:
-      return None
+    except Exception:
+        return None
+
 
 def __connect_callback(pv, isconn):
-    if (isconn):
+    if isconn:
         pv.connect_cb = pv.save_connect_cb
         if pv.connect_cb:
             pv.connect_cb(isconn)
         pv.get(ctrl=False, timeout=-1.0)
 
+
 def __getevt_callback(pv, e=None):
     if pv.handler:
         pv.handler(pv, e)
     if e is None:
         pv._Pv__getevt_handler(e)
         pv.getevt_cb = None
         pv.monitor(pyca.DBE_VALUE)
         pyca.flush_io()
 
+
 def __monitor_callback(pv, e=None):
     pv.handler(pv, e)
-        
-def monitorPv(name,handler):
+
+
+def monitorPv(name, handler):
     try:
         pv = connectPv(name)
         pv.handler = handler
-        pv.getevt_cb = lambda  e=None: __getevt_callback(pv, e)
+        pv.getevt_cb = lambda e=None: __getevt_callback(pv, e)
         pv.monitor_cb = lambda e=None: __monitor_callback(pv, e)
         return pv
-    except:
+    except Exception:
         return None
 
+
 #
 # Go through a list of dictionaries and create a 'cfgname' name for the
 # specified 'config' idx.
 #
 def fixName(l, idx, name):
     for d in l:
         try:
-            if d['config'] == idx:
-                d['cfgname'] = name
-        except:
+            if d["config"] == idx:
+                d["cfgname"] = name
+        except Exception:
             pass
 
+
 #
 # Determine if the current user has the authority to modify a record.
 #
 def permission():
     return param.params.user in param.params.auth_users
 
+
 #
 # Check if the user/password pair is valid.  This is actually not terribly secure (the KDC can
 # be spoofed), but it's really close enough for our purposes.
 #
+# The verify has to be False... otherwise, this is a bit too secure for us!
+#
 def authenticate_user(user, password):
     try:
-        if kerberos.checkPassword(user, password, "krbtgt/SLAC.STANFORD.EDU", "SLAC.STANFORD.EDU"):
+        if kerberos.checkPassword(
+            user, password, "krbtgt/SLAC.STANFORD.EDU", "SLAC.STANFORD.EDU", False
+        ):
             return True
-    except:
+    except Exception:
         pass
     return False
```

