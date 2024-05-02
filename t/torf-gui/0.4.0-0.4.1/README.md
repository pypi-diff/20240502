# Comparing `tmp/torf-gui-0.4.0.tar.gz` & `tmp/torf-gui-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torf-gui-0.4.0.tar", last modified: Wed May  1 23:42:42 2024, max compression
+gzip compressed data, was "torf-gui-0.4.1.tar", last modified: Thu May  2 00:31:21 2024, max compression
```

## Comparing `torf-gui-0.4.0.tar` & `torf-gui-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:42:42.468367 torf-gui-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-01 23:42:24.000000 torf-gui-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-01 23:42:42.468367 torf-gui-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-01 23:42:24.000000 torf-gui-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-01 23:42:24.000000 torf-gui-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:42:42.468367 torf-gui-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-01 23:42:24.000000 torf-gui-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:42:42.468367 torf-gui-0.4.0/torf_gui/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-01 23:42:24.000000 torf-gui-0.4.0/torf_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-01 23:42:24.000000 torf-gui-0.4.0/torf_gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-01 23:42:24.000000 torf-gui-0.4.0/torf_gui/ui_about.py
--rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-05-01 23:42:24.000000 torf-gui-0.4.0/torf_gui/ui_mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 23:42:24.000000 torf-gui-0.4.0/torf_gui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:42:42.468367 torf-gui-0.4.0/torf_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-01 23:42:42.000000 torf-gui-0.4.0/torf_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 23:42:42.000000 torf-gui-0.4.0/torf_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:42:42.000000 torf-gui-0.4.0/torf_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 23:42:42.000000 torf-gui-0.4.0/torf_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 23:42:42.000000 torf-gui-0.4.0/torf_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 23:42:42.000000 torf-gui-0.4.0/torf_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:31:21.768348 torf-gui-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-02 00:30:59.000000 torf-gui-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-02 00:31:21.768348 torf-gui-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-02 00:30:59.000000 torf-gui-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 00:30:59.000000 torf-gui-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:31:21.768348 torf-gui-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-02 00:30:59.000000 torf-gui-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:31:21.768348 torf-gui-0.4.1/torf_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 00:30:59.000000 torf-gui-0.4.1/torf_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25386 2024-05-02 00:30:59.000000 torf-gui-0.4.1/torf_gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-02 00:30:59.000000 torf-gui-0.4.1/torf_gui/ui_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-05-02 00:30:59.000000 torf-gui-0.4.1/torf_gui/ui_mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 00:30:59.000000 torf-gui-0.4.1/torf_gui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:31:21.768348 torf-gui-0.4.1/torf_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-02 00:31:21.000000 torf-gui-0.4.1/torf_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-02 00:31:21.000000 torf-gui-0.4.1/torf_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:31:21.000000 torf-gui-0.4.1/torf_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 00:31:21.000000 torf-gui-0.4.1/torf_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 00:31:21.000000 torf-gui-0.4.1/torf_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 00:31:21.000000 torf-gui-0.4.1/torf_gui.egg-info/top_level.txt
```

### Comparing `torf-gui-0.4.0/LICENSE` & `torf-gui-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torf-gui-0.4.0/PKG-INFO` & `torf-gui-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torf-gui
-Version: 0.4.0
+Version: 0.4.1
 Summary: An advanced GUI torrent file creator with batch functionality, powered by PyQt and torf.
 Home-page: https://github.com/SavageCore/torf-gui
 Author: Oliver Sayers
 Author-email: talk@savagecore.uk
 Keywords: bittorrent torrent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `torf-gui-0.4.0/README.md` & `torf-gui-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `torf-gui-0.4.0/setup.py` & `torf-gui-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `torf-gui-0.4.0/torf_gui/gui.py` & `torf-gui-0.4.1/torf_gui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,19 +386,16 @@
         ptail = os.path.split(self.torrent.path)[1]
         if self.inputMode == "file":
             self._statusBarMsg(
                 f"{ptail}: {humanfriendly.format_size(t_info[0], binary=True)}"
             )
         else:
             self._statusBarMsg(
-                "{}: {} files, {}".format(
-                    ptail,
-                    t_info[1],
-                    humanfriendly.format_size(t_info[0], binary=True),
-                )
+                f"{ptail}: {t_info[1]} files, "
+                f"{humanfriendly.format_size(t_info[0], binary=True)}"
             )
         self.pieceSizeComboBox.setCurrentIndex(0)
         self.updatePieceCountLabel(t_info[3], t_info[2])
         self.pieceCountLabel.show()
         self.createButton.setEnabled(True)
 
     def commentEdited(self, comment):
```

### Comparing `torf-gui-0.4.0/torf_gui/ui_about.py` & `torf-gui-0.4.1/torf_gui/ui_about.py`

 * *Files identical despite different names*

### Comparing `torf-gui-0.4.0/torf_gui/ui_mainwindow.py` & `torf-gui-0.4.1/torf_gui/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `torf-gui-0.4.0/torf_gui.egg-info/PKG-INFO` & `torf-gui-0.4.1/torf_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torf-gui
-Version: 0.4.0
+Version: 0.4.1
 Summary: An advanced GUI torrent file creator with batch functionality, powered by PyQt and torf.
 Home-page: https://github.com/SavageCore/torf-gui
 Author: Oliver Sayers
 Author-email: talk@savagecore.uk
 Keywords: bittorrent torrent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

