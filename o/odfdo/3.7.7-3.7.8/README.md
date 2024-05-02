# Comparing `tmp/odfdo-3.7.7.tar.gz` & `tmp/odfdo-3.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odfdo-3.7.7.tar", max compression
+gzip compressed data, was "odfdo-3.7.8.tar", max compression
```

## Comparing `odfdo-3.7.7.tar` & `odfdo-3.7.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11357 2022-08-19 23:34:42.000000 odfdo-3.7.7/LICENSE
--rw-r--r--   0        0        0      433 2022-08-19 23:34:42.000000 odfdo-3.7.7/NOTICE.txt
--rw-r--r--   0        0        0     3308 2024-04-01 16:01:23.803500 odfdo-3.7.7/README.md
--rw-r--r--   0        0        0     5254 2024-04-01 10:08:15.947787 odfdo-3.7.7/odfdo/__init__.py
--rw-r--r--   0        0        0     2361 2024-04-01 10:08:15.948752 odfdo-3.7.7/odfdo/bookmark.py
--rw-r--r--   0        0        0    13076 2024-04-01 10:08:15.949530 odfdo-3.7.7/odfdo/cell.py
--rw-r--r--   0        0        0    21620 2024-04-01 10:08:15.951225 odfdo-3.7.7/odfdo/const.py
--rw-r--r--   0        0        0    16027 2024-04-01 10:08:15.952036 odfdo-3.7.7/odfdo/container.py
--rw-r--r--   0        0        0     3463 2024-04-01 10:08:15.952350 odfdo-3.7.7/odfdo/content.py
--rw-r--r--   0        0        0     6668 2024-04-01 10:08:15.952639 odfdo-3.7.7/odfdo/datatype.py
--rw-r--r--   0        0        0    41960 2024-04-01 10:08:15.953310 odfdo-3.7.7/odfdo/document.py
--rw-r--r--   0        0        0     4192 2024-04-01 10:08:15.953626 odfdo-3.7.7/odfdo/draw_page.py
--rw-r--r--   0        0        0   107411 2024-04-01 10:08:15.954747 odfdo-3.7.7/odfdo/element.py
--rw-r--r--   0        0        0     7976 2024-04-01 10:08:15.955617 odfdo-3.7.7/odfdo/element_typed.py
--rw-r--r--   0        0        0    15586 2024-04-01 10:08:15.956248 odfdo-3.7.7/odfdo/frame.py
--rw-r--r--   0        0        0     3665 2024-04-01 10:08:15.956563 odfdo-3.7.7/odfdo/header.py
--rw-r--r--   0        0        0     1270 2024-04-01 10:08:15.957382 odfdo-3.7.7/odfdo/header_rows.py
--rw-r--r--   0        0        0     3524 2024-04-01 10:08:15.957701 odfdo-3.7.7/odfdo/image.py
--rw-r--r--   0        0        0     3206 2024-04-01 10:08:15.957997 odfdo-3.7.7/odfdo/link.py
--rw-r--r--   0        0        0     7129 2024-04-01 10:08:15.958225 odfdo-3.7.7/odfdo/list.py
--rw-r--r--   0        0        0     3812 2024-04-01 10:08:15.958534 odfdo-3.7.7/odfdo/manifest.py
--rw-r--r--   0        0        0    18936 2024-04-01 10:08:15.958713 odfdo-3.7.7/odfdo/meta.py
--rw-r--r--   0        0        0    11191 2024-04-01 10:08:15.958954 odfdo-3.7.7/odfdo/note.py
--rw-r--r--   0        0        0    28204 2024-04-01 10:08:15.959276 odfdo-3.7.7/odfdo/paragraph.py
--rw-r--r--   0        0        0     9443 2024-04-01 10:08:15.960044 odfdo-3.7.7/odfdo/paragraph_base.py
--rw-r--r--   0        0        0    14661 2024-04-01 10:08:15.960585 odfdo-3.7.7/odfdo/reference.py
--rw-r--r--   0        0        0    25859 2024-04-01 10:08:15.961041 odfdo-3.7.7/odfdo/row.py
--rw-r--r--   0        0        0        1 2024-04-01 10:08:15.961512 odfdo-3.7.7/odfdo/scripts/__init__.py
--rwxr-xr-x   0        0        0     3280 2024-04-01 10:08:15.962026 odfdo-3.7.7/odfdo/scripts/diff.py
--rwxr-xr-x   0        0        0     2186 2024-04-01 10:08:15.962447 odfdo-3.7.7/odfdo/scripts/folder.py
--rwxr-xr-x   0        0        0     3803 2024-04-01 10:08:15.963301 odfdo-3.7.7/odfdo/scripts/headers.py
--rwxr-xr-x   0        0        0     5832 2024-04-01 10:08:15.963611 odfdo-3.7.7/odfdo/scripts/highlight.py
--rwxr-xr-x   0        0        0     3603 2024-04-01 10:08:15.963998 odfdo-3.7.7/odfdo/scripts/replace.py
--rwxr-xr-x   0        0        0     5752 2024-04-01 10:08:15.964706 odfdo-3.7.7/odfdo/scripts/show.py
--rwxr-xr-x   0        0        0     7576 2024-04-01 10:08:15.965411 odfdo-3.7.7/odfdo/scripts/styles.py
--rwxr-xr-x   0        0        0     3442 2024-04-01 10:08:15.966077 odfdo-3.7.7/odfdo/scripts/table_shrink.py
--rw-r--r--   0        0        0     1936 2024-04-01 10:08:15.967048 odfdo-3.7.7/odfdo/scriptutils.py
--rw-r--r--   0        0        0     1939 2024-04-01 10:08:15.967336 odfdo-3.7.7/odfdo/section.py
--rw-r--r--   0        0        0    11548 2024-04-01 10:08:15.967836 odfdo-3.7.7/odfdo/shapes.py
--rw-r--r--   0        0        0     4691 2024-04-01 10:08:15.968192 odfdo-3.7.7/odfdo/smil.py
--rw-r--r--   0        0        0    38072 2024-04-01 10:08:15.968702 odfdo-3.7.7/odfdo/style.py
--rw-r--r--   0        0        0     5244 2024-04-01 10:08:15.969088 odfdo-3.7.7/odfdo/styles.py
--rw-r--r--   0        0        0   104120 2024-04-01 10:08:15.969691 odfdo-3.7.7/odfdo/table.py
--rw-r--r--   0        0        0        1 2024-04-01 10:08:15.970133 odfdo-3.7.7/odfdo/templates/__init__.py
--rw-r--r--   0        0        0     8291 2024-04-01 10:08:15.970835 odfdo-3.7.7/odfdo/templates/drawing.otg
--rw-r--r--   0        0        0    11017 2024-04-01 10:08:15.971235 odfdo-3.7.7/odfdo/templates/lpod_styles.odt
--rw-r--r--   0        0        0    16065 2024-04-01 10:08:15.971582 odfdo-3.7.7/odfdo/templates/presentation.otp
--rw-r--r--   0        0        0     7432 2024-04-01 10:08:15.972020 odfdo-3.7.7/odfdo/templates/spreadsheet.ots
--rw-r--r--   0        0        0     9620 2024-04-01 10:08:15.972500 odfdo-3.7.7/odfdo/templates/text.ott
--rw-r--r--   0        0        0    17070 2024-04-01 10:08:15.973345 odfdo-3.7.7/odfdo/toc.py
--rw-r--r--   0        0        0    24638 2024-04-01 10:08:15.973733 odfdo-3.7.7/odfdo/tracked_changes.py
--rw-r--r--   0        0        0     1318 2024-04-01 10:08:15.973907 odfdo-3.7.7/odfdo/utils/__init__.py
--rw-r--r--   0        0        0     9339 2024-04-01 10:08:15.974689 odfdo-3.7.7/odfdo/utils/cache_map.py
--rw-r--r--   0        0        0      926 2024-04-01 10:08:15.975005 odfdo-3.7.7/odfdo/utils/cached_element.py
--rw-r--r--   0        0        0     3035 2024-04-01 10:08:15.975436 odfdo-3.7.7/odfdo/utils/color.py
--rw-r--r--   0        0        0     4533 2024-04-01 10:08:15.975823 odfdo-3.7.7/odfdo/utils/coordinates.py
--rw-r--r--   0        0        0     1476 2024-04-01 10:08:15.976142 odfdo-3.7.7/odfdo/utils/formula.py
--rw-r--r--   0        0        0     1314 2024-04-01 10:08:15.976364 odfdo-3.7.7/odfdo/utils/isiterable.py
--rw-r--r--   0        0        0     1429 2024-04-01 10:08:15.976629 odfdo-3.7.7/odfdo/utils/str_convert.py
--rw-r--r--   0        0        0     2503 2024-04-01 10:08:15.976906 odfdo-3.7.7/odfdo/utils/style_constants.py
--rw-r--r--   0        0        0     4272 2024-04-01 10:08:15.977335 odfdo-3.7.7/odfdo/utils/xpath_query.py
--rw-r--r--   0        0        0    14844 2024-04-01 10:08:15.977547 odfdo-3.7.7/odfdo/variable.py
--rw-r--r--   0        0        0     1165 2024-04-01 10:08:15.977698 odfdo-3.7.7/odfdo/version.py
--rw-r--r--   0        0        0     3688 2024-04-01 10:08:15.978014 odfdo-3.7.7/odfdo/xmlpart.py
--rw-r--r--   0        0        0     3844 2024-04-01 16:01:23.830660 odfdo-3.7.7/pyproject.toml
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 odfdo-3.7.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-08-19 23:34:42.000000 odfdo-3.7.8/LICENSE
+-rw-r--r--   0        0        0      433 2022-08-19 23:34:42.000000 odfdo-3.7.8/NOTICE.txt
+-rw-r--r--   0        0        0     3308 2024-04-01 16:01:23.803500 odfdo-3.7.8/README.md
+-rw-r--r--   0        0        0     5220 2024-05-02 07:44:54.443931 odfdo-3.7.8/odfdo/__init__.py
+-rw-r--r--   0        0        0     2361 2024-04-01 10:08:15.948752 odfdo-3.7.8/odfdo/bookmark.py
+-rw-r--r--   0        0        0    13076 2024-04-01 10:08:15.949530 odfdo-3.7.8/odfdo/cell.py
+-rw-r--r--   0        0        0    24252 2024-05-02 07:44:54.444099 odfdo-3.7.8/odfdo/const.py
+-rw-r--r--   0        0        0    18030 2024-05-02 07:44:54.444263 odfdo-3.7.8/odfdo/container.py
+-rw-r--r--   0        0        0     3243 2024-05-02 07:44:54.444402 odfdo-3.7.8/odfdo/content.py
+-rw-r--r--   0        0        0     6668 2024-04-01 10:08:15.952639 odfdo-3.7.8/odfdo/datatype.py
+-rw-r--r--   0        0        0    42015 2024-05-02 07:44:54.444601 odfdo-3.7.8/odfdo/document.py
+-rw-r--r--   0        0        0     4192 2024-04-01 10:08:15.953626 odfdo-3.7.8/odfdo/draw_page.py
+-rw-r--r--   0        0        0   104963 2024-05-02 07:44:54.444908 odfdo-3.7.8/odfdo/element.py
+-rw-r--r--   0        0        0     8034 2024-05-02 07:44:54.445090 odfdo-3.7.8/odfdo/element_typed.py
+-rw-r--r--   0        0        0    15586 2024-04-01 10:08:15.956248 odfdo-3.7.8/odfdo/frame.py
+-rw-r--r--   0        0        0     3665 2024-04-01 10:08:15.956563 odfdo-3.7.8/odfdo/header.py
+-rw-r--r--   0        0        0     1270 2024-04-01 10:08:15.957382 odfdo-3.7.8/odfdo/header_rows.py
+-rw-r--r--   0        0        0     3524 2024-04-01 10:08:15.957701 odfdo-3.7.8/odfdo/image.py
+-rw-r--r--   0        0        0     3206 2024-04-01 10:08:15.957997 odfdo-3.7.8/odfdo/link.py
+-rw-r--r--   0        0        0     7129 2024-04-01 10:08:15.958225 odfdo-3.7.8/odfdo/list.py
+-rw-r--r--   0        0        0     3812 2024-04-01 10:08:15.958534 odfdo-3.7.8/odfdo/manifest.py
+-rw-r--r--   0        0        0    19538 2024-05-02 07:44:54.445255 odfdo-3.7.8/odfdo/meta.py
+-rw-r--r--   0        0        0    11191 2024-04-01 10:08:15.958954 odfdo-3.7.8/odfdo/note.py
+-rw-r--r--   0        0        0    28204 2024-04-01 10:08:15.959276 odfdo-3.7.8/odfdo/paragraph.py
+-rw-r--r--   0        0        0     9443 2024-04-01 10:08:15.960044 odfdo-3.7.8/odfdo/paragraph_base.py
+-rw-r--r--   0        0        0    14661 2024-04-01 10:08:15.960585 odfdo-3.7.8/odfdo/reference.py
+-rw-r--r--   0        0        0    25859 2024-04-01 10:08:15.961041 odfdo-3.7.8/odfdo/row.py
+-rw-r--r--   0        0        0        1 2024-04-01 10:08:15.961512 odfdo-3.7.8/odfdo/scripts/__init__.py
+-rwxr-xr-x   0        0        0     3280 2024-04-01 10:08:15.962026 odfdo-3.7.8/odfdo/scripts/diff.py
+-rwxr-xr-x   0        0        0     2178 2024-05-02 07:44:54.445397 odfdo-3.7.8/odfdo/scripts/folder.py
+-rwxr-xr-x   0        0        0     3803 2024-04-01 10:08:15.963301 odfdo-3.7.8/odfdo/scripts/headers.py
+-rwxr-xr-x   0        0        0     5832 2024-04-01 10:08:15.963611 odfdo-3.7.8/odfdo/scripts/highlight.py
+-rwxr-xr-x   0        0        0     3603 2024-04-01 10:08:15.963998 odfdo-3.7.8/odfdo/scripts/replace.py
+-rwxr-xr-x   0        0        0     5752 2024-04-01 10:08:15.964706 odfdo-3.7.8/odfdo/scripts/show.py
+-rwxr-xr-x   0        0        0     7576 2024-04-01 10:08:15.965411 odfdo-3.7.8/odfdo/scripts/styles.py
+-rwxr-xr-x   0        0        0     3442 2024-04-01 10:08:15.966077 odfdo-3.7.8/odfdo/scripts/table_shrink.py
+-rw-r--r--   0        0        0     1936 2024-04-01 10:08:15.967048 odfdo-3.7.8/odfdo/scriptutils.py
+-rw-r--r--   0        0        0     1939 2024-04-01 10:08:15.967336 odfdo-3.7.8/odfdo/section.py
+-rw-r--r--   0        0        0    11548 2024-04-01 10:08:15.967836 odfdo-3.7.8/odfdo/shapes.py
+-rw-r--r--   0        0        0     4691 2024-04-01 10:08:15.968192 odfdo-3.7.8/odfdo/smil.py
+-rw-r--r--   0        0        0    38072 2024-05-02 07:44:54.445588 odfdo-3.7.8/odfdo/style.py
+-rw-r--r--   0        0        0     5244 2024-04-01 10:08:15.969088 odfdo-3.7.8/odfdo/styles.py
+-rw-r--r--   0        0        0   104460 2024-05-02 07:44:54.445878 odfdo-3.7.8/odfdo/table.py
+-rw-r--r--   0        0        0        1 2024-04-01 10:08:15.970133 odfdo-3.7.8/odfdo/templates/__init__.py
+-rw-r--r--   0        0        0     8291 2024-04-01 10:08:15.970835 odfdo-3.7.8/odfdo/templates/drawing.otg
+-rw-r--r--   0        0        0    11017 2024-04-01 10:08:15.971235 odfdo-3.7.8/odfdo/templates/lpod_styles.odt
+-rw-r--r--   0        0        0    16065 2024-04-01 10:08:15.971582 odfdo-3.7.8/odfdo/templates/presentation.otp
+-rw-r--r--   0        0        0     7432 2024-04-01 10:08:15.972020 odfdo-3.7.8/odfdo/templates/spreadsheet.ots
+-rw-r--r--   0        0        0     9620 2024-04-01 10:08:15.972500 odfdo-3.7.8/odfdo/templates/text.ott
+-rw-r--r--   0        0        0    17070 2024-04-01 10:08:15.973345 odfdo-3.7.8/odfdo/toc.py
+-rw-r--r--   0        0        0    24638 2024-04-01 10:08:15.973733 odfdo-3.7.8/odfdo/tracked_changes.py
+-rw-r--r--   0        0        0     1318 2024-04-01 10:08:15.973907 odfdo-3.7.8/odfdo/utils/__init__.py
+-rw-r--r--   0        0        0     9339 2024-04-01 10:08:15.974689 odfdo-3.7.8/odfdo/utils/cache_map.py
+-rw-r--r--   0        0        0      926 2024-04-01 10:08:15.975005 odfdo-3.7.8/odfdo/utils/cached_element.py
+-rw-r--r--   0        0        0     3035 2024-04-01 10:08:15.975436 odfdo-3.7.8/odfdo/utils/color.py
+-rw-r--r--   0        0        0     4533 2024-04-01 10:08:15.975823 odfdo-3.7.8/odfdo/utils/coordinates.py
+-rw-r--r--   0        0        0     1476 2024-04-01 10:08:15.976142 odfdo-3.7.8/odfdo/utils/formula.py
+-rw-r--r--   0        0        0     1314 2024-04-01 10:08:15.976364 odfdo-3.7.8/odfdo/utils/isiterable.py
+-rw-r--r--   0        0        0     1429 2024-04-01 10:08:15.976629 odfdo-3.7.8/odfdo/utils/str_convert.py
+-rw-r--r--   0        0        0     2503 2024-04-01 10:08:15.976906 odfdo-3.7.8/odfdo/utils/style_constants.py
+-rw-r--r--   0        0        0     4272 2024-04-01 10:08:15.977335 odfdo-3.7.8/odfdo/utils/xpath_query.py
+-rw-r--r--   0        0        0    14844 2024-05-02 07:44:54.446064 odfdo-3.7.8/odfdo/variable.py
+-rw-r--r--   0        0        0     1165 2024-04-01 10:08:15.977698 odfdo-3.7.8/odfdo/version.py
+-rw-r--r--   0        0        0     3899 2024-05-02 07:44:54.446210 odfdo-3.7.8/odfdo/xmlpart.py
+-rw-r--r--   0        0        0     3844 2024-05-02 07:44:54.446935 odfdo-3.7.8/pyproject.toml
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 odfdo-3.7.8/PKG-INFO
```

### Comparing `odfdo-3.7.7/LICENSE` & `odfdo-3.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/README.md` & `odfdo-3.7.8/README.md`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/__init__.py` & `odfdo-3.7.8/odfdo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 #
 # Authors (odfdo project): jerome.dumonteil@gmail.com
 # The odfdo project is a derivative work of the lpod-python project:
 # https://github.com/lpod/lpod-python
 # Authors: David Versmisse <david.versmisse@itaapy.com>
 #          Hervé Cauwelier <herve@itaapy.com>
 #          Romain Gauthier <romain@itaapy.com>
-"""
-.. include:: ../README.md
-"""
 
 __all__ = [
     "AnimPar",
     "AnimSeq",
     "AnimTransFilter",
     "Annotation",
     "AnnotationEnd",
```

### Comparing `odfdo-3.7.7/odfdo/bookmark.py` & `odfdo-3.7.8/odfdo/bookmark.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/cell.py` & `odfdo-3.7.8/odfdo/cell.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/const.py` & `odfdo-3.7.8/odfdo/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,20 +104,67 @@
 
 # Paths of standard parts
 ODF_CONTENT = "content.xml"
 ODF_META = "meta.xml"
 ODF_SETTINGS = "settings.xml"
 ODF_STYLES = "styles.xml"
 ODF_MANIFEST = "META-INF/manifest.xml"
+ODF_MANIFEST_NAME = "manifest.xml"
 
+OFFICE_VERSION = "1.1"
+
+OFFICE_PREFIX = b"""<?xml version="1.0" encoding="UTF-8"?>
+<office:document
+  xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
+  xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0"
+  xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0"
+  xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0"
+  xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0"
+  xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0"
+  xmlns:xlink="http://www.w3.org/1999/xlink"
+  xmlns:dc="http://purl.org/dc/elements/1.1/"
+  xmlns:meta="urn:oasis:names:tc:opendocument:xmlns:meta:1.0"
+  xmlns:number="urn:oasis:names:tc:opendocument:xmlns:datastyle:1.0"
+  xmlns:presentation="urn:oasis:names:tc:opendocument:xmlns:presentation:1.0"
+  xmlns:svg="urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0"
+  xmlns:chart="urn:oasis:names:tc:opendocument:xmlns:chart:1.0"
+  xmlns:dr3d="urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0"
+  xmlns:math="http://www.w3.org/1998/Math/MathML"
+  xmlns:form="urn:oasis:names:tc:opendocument:xmlns:form:1.0"
+  xmlns:script="urn:oasis:names:tc:opendocument:xmlns:script:1.0"
+  xmlns:ooo="http://openoffice.org/2004/office"
+  xmlns:oooc="http://openoffice.org/2004/calc"
+  xmlns:ooow="http://openoffice.org/2004/writer"
+  xmlns:xforms="http://www.w3.org/2002/xforms"
+  xmlns:xsd="http://www.w3.org/2001/XMLSchema"
+  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
+  xmlns:smil="urn:oasis:names:tc:opendocument:xmlns:smil-compatible:1.0"
+  xmlns:anim="urn:oasis:names:tc:opendocument:xmlns:animation:1.0"
+  xmlns:rpt="http://openoffice.org/2005/report"
+  xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
+  xmlns:xhtml="http://www.w3.org/1999/xhtml"
+  xmlns:grddl="http://www.w3.org/2003/g/data-view#"
+  xmlns:officeooo="http://openoffice.org/2009/office"
+  xmlns:tableooo="http://openoffice.org/2009/table"
+  xmlns:drawooo="http://openoffice.org/2010/draw"
+  xmlns:calcext="urn:org:documentfoundation:names:experimental:calc:xmlns:calcext:1.0"
+  xmlns:loext="urn:org:documentfoundation:names:experimental:office:xmlns:loext:1.0"
+  xmlns:field="urn:openoffice:names:experimental:ooo-ms-interop:xmlns:field:1.0"
+  xmlns:formx="urn:openoffice:names:experimental:ooxml-odf-interop:xmlns:form:1.0"
+  xmlns:css3t="http://www.w3.org/TR/css3-text/"
+  xmlns:config="urn:oasis:names:tc:opendocument:xmlns:config:1.0"
+  xmlns:dom="http://www.w3.org/2001/xml-events"
+  xmlns:manifest="urn:oasis:names:tc:opendocument:xmlns:manifest:1.0"
+  xmlns:rdfa="http://docs.oasis-open.org/opendocument/meta/rdfa#"
+"""
 # packaging
 FOLDER = "folder"
-ZIP = "ZIP"
-XML = "XML"
-PACKAGING = {FOLDER, ZIP, FOLDER}
+ZIP = "zip"
+XML = "xml"
+PACKAGING = {FOLDER, XML, ZIP}
 
 # Presentation classes (for layout)
 ODF_CLASSES = (
     "title",
     "outline",
     "subtitle",
     "text",
```

### Comparing `odfdo-3.7.7/odfdo/container.py` & `odfdo-3.7.8/odfdo/container.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,22 +28,30 @@
 import os
 import shutil
 import time
 from copy import deepcopy
 from pathlib import Path, PurePath
 from zipfile import ZIP_DEFLATED, ZIP_STORED, BadZipfile, ZipFile, is_zipfile
 
+from lxml.etree import fromstring, tostring
+
 from .const import (
+    FOLDER,
     ODF_CONTENT,
     ODF_EXTENSIONS,
     ODF_MANIFEST,
     ODF_META,
     ODF_MIMETYPES,
     ODF_SETTINGS,
     ODF_STYLES,
+    OFFICE_PREFIX,
+    OFFICE_VERSION,
+    PACKAGING,
+    XML,
+    ZIP,
 )
 from .scriptutils import printwarn
 from .utils import bytes_to_str, str_to_bytes
 
 
 def normalize_path(path: str) -> str:
     if path.endswith("/"):  # folder
@@ -54,15 +62,15 @@
 class Container:
     """Representation of the ODF file."""
 
     def __init__(self, path: Path | str | io.BytesIO | None = None) -> None:
         self.__parts: dict[str, bytes | None] = {}
         self.__parts_ts: dict[str, int] = {}
         self.__path_like: Path | str | io.BytesIO | None = None
-        self.__packaging: str = "zip"
+        self.__packaging: str = ZIP
         self.path: Path | None = None  # or Path
         if path:
             self.open(path)
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} type={self.mimetype} path={self.path}>"
 
@@ -73,22 +81,22 @@
             self.path = Path(path_or_file).expanduser()
             if not self.path.exists():
                 raise FileNotFoundError(str(self.path))
             self.__path_like = self.path
         if (self.path or isinstance(self.__path_like, io.BytesIO)) and is_zipfile(
             self.__path_like  # type: ignore
         ):
-            self.__packaging = "zip"
+            self.__packaging = ZIP
             return self._read_zip()
         if self.path:
             is_folder = False
             with contextlib.suppress(OSError):
                 is_folder = self.path.is_dir()
             if is_folder:
-                self.__packaging = "folder"
+                self.__packaging = FOLDER
                 return self._read_folder()
         raise TypeError(f"Document format not managed by odfdo: {type(path_or_file)}.")
 
     def _read_zip(self) -> None:
         if isinstance(self.__path_like, io.BytesIO):
             self.__path_like.seek(0)
         with ZipFile(self.__path_like) as zf:  # type: ignore
@@ -250,51 +258,81 @@
 
         for part_path, data in self.__parts.items():
             if data is None:
                 # Deleted
                 continue
             dump(part_path, data)
 
+    def _xml_content(self) -> bytes:
+        mimetype = self.__parts["mimetype"].decode("utf8")
+        doc_xml = (
+            OFFICE_PREFIX.decode("utf8")
+            + f'office:version="{OFFICE_VERSION}"\n'
+            + f'office:mimetype="{mimetype}">'
+            + "</office:document>"
+        )
+        root = fromstring(doc_xml.encode("utf8"))
+        for path in ODF_META, ODF_SETTINGS, ODF_STYLES, ODF_CONTENT:
+            if path not in self.__parts:
+                printwarn(f"Missing '{path}'")
+                continue
+            part = self.__parts[path]
+            if part is None:
+                continue
+            if isinstance(part, bytes):
+                xpart = fromstring(part)
+            else:
+                xpart = part
+            print(xpart, part.__class__.__name__)
+            for child in xpart:
+                root.append(child)
+        return tostring(root, encoding="UTF-8", xml_declaration=True)
+
+    def _save_xml(self, target: Path | str) -> None:
+        """Save a XML flat ODF format from the available parts."""
+        target = Path(target).with_suffix(".xml")
+        target.write_bytes(self._xml_content())
+
     # Public API
 
     def get_parts(self) -> list[str]:
         """Get the list of members."""
         if not self.path:
             # maybe a file like zip archive
             return list(self.__parts.keys())
-        if self.__packaging == "zip":
+        if self.__packaging == ZIP:
             parts = []
             with ZipFile(self.path) as zf:
                 for name in zf.namelist():
                     upath = normalize_path(name)
                     parts.append(upath)
             return parts
-        elif self.__packaging == "folder":
+        elif self.__packaging == FOLDER:
             return self._get_folder_parts()
         else:
             raise ValueError("Unable to provide parts of the document")
 
     def get_part(self, path: str) -> str | bytes | None:
         """Get the bytes of a part of the ODF."""
         path = str(path)
         if path in self.__parts:
             part = self.__parts[path]
             if part is None:
                 raise ValueError(f'Part "{path}" is deleted')
-            if self.__packaging == "folder":
+            if self.__packaging == FOLDER:
                 cache_ts = self.__parts_ts.get(path, -1)
                 current_ts = self._get_folder_part_timestamp(path)
                 if current_ts != cache_ts:
                     part, timestamp = self._get_folder_part(path)
                     self.__parts[path] = part
                     self.__parts_ts[path] = timestamp
             return part
-        if self.__packaging == "zip":
+        if self.__packaging == ZIP:
             return self._get_zip_part(path)
-        if self.__packaging == "folder":
+        if self.__packaging == FOLDER:
             part, timestamp = self._get_folder_part(path)
             self.__parts[path] = part
             self.__parts_ts[path] = timestamp
             return part
         return None
 
     @property
@@ -323,20 +361,26 @@
     def del_part(self, path: str) -> None:
         """Mark a part for deletion."""
         self.__parts[path] = None
 
     @property
     def clone(self) -> Container:
         """Make a copy of this container with no path."""
-        if self.path and self.__packaging == "zip":
+        if self.path and self.__packaging == ZIP:
             self._get_all_zip_part()
         clone = deepcopy(self)
         clone.path = None
         return clone
 
+    def _backup_or_unlink(self, backup: bool, target: str | Path) -> None:
+        if backup:
+            self._do_backup(target)
+        else:
+            self._do_unlink(target)
+
     @staticmethod
     def _do_backup(target: str | Path) -> None:
         path = Path(target)
         if not path.exists():
             return
         back_file = Path(path.stem + ".backup" + path.suffix)
         if back_file.is_dir():
@@ -345,24 +389,35 @@
             except OSError as e:
                 printwarn(str(e))
         try:
             shutil.move(target, back_file)
         except OSError as e:
             printwarn(str(e))
 
-    def _save_packaging(self, packaging: str | None) -> str:
+    @staticmethod
+    def _do_unlink(target: str | Path) -> None:
+        path = Path(target)
+        if path.exists():
+            try:
+                shutil.rmtree(path)
+            except OSError as e:
+                printwarn(str(e))
+
+    def _clean_save_packaging(self, packaging: str | None) -> str:
         if not packaging:
-            packaging = self.__packaging if self.__packaging else "zip"
+            packaging = self.__packaging if self.__packaging else ZIP
         packaging = packaging.strip().lower()
-        # if packaging not in ('zip', 'flat', 'folder'):
-        if packaging not in ("zip", "folder"):
+        if packaging not in PACKAGING:
             raise ValueError(f'Packaging of type "{packaging}" is not supported')
         return packaging
 
-    def _save_target(self, target: str | Path | io.BytesIO | None) -> str | io.BytesIO:
+    def _clean_save_target(
+        self,
+        target: str | Path | io.BytesIO | None,
+    ) -> str | io.BytesIO:
         if target is None:
             target = self.path
         if isinstance(target, Path):
             target = str(target)
         if isinstance(target, str):
             while target.endswith(os.sep):
                 target = target[:-1]
@@ -378,25 +433,28 @@
     def _save_as_folder(self, target: str | Path, backup: bool) -> None:
         if not isinstance(target, (str, Path)):
             raise TypeError(
                 f"Saving in folder format requires a folder name, not '{target!r}'"
             )
         if not str(target).endswith(".folder"):
             target = str(target) + ".folder"
-        if backup:
-            self._do_backup(target)
-        else:
-            path = Path(target)
-            if path.exists():
-                try:
-                    shutil.rmtree(path)
-                except OSError as e:
-                    printwarn(str(e))
+        self._backup_or_unlink(backup, target)
         self._save_folder(target)
 
+    def _save_as_xml(self, target: str | Path | io.BytesIO, backup: bool) -> None:
+        if not isinstance(target, (str, Path)):
+            raise TypeError(
+                f"Saving in XML format requires a folder name, not '{target!r}'"
+            )
+        if not str(target).endswith(".xml"):
+            target = str(target) + ".xml"
+        if isinstance(target, (str, Path)) and backup:
+            self._do_backup(target)
+        self._save_xml(target)
+
     def save(
         self,
         target: str | Path | io.BytesIO | None,
         packaging: str | None = None,
         backup: bool = False,
     ) -> None:
         """Save the container to the given target, a path or a file-like
@@ -405,27 +463,29 @@
         Package the output document in the same format than current document,
         unless "packaging" is different.
 
         Arguments:
 
             target -- str or file-like or Path
 
-            packaging -- 'zip', or for debugging purpose 'folder'
+            packaging -- 'zip', or for debugging purpose 'xml' or 'folder'
 
             backup -- boolean
         """
         parts = self.__parts
-        packaging = self._save_packaging(packaging)
+        packaging = self._clean_save_packaging(packaging)
         # Load parts else they will be considered deleted
         for path in self.get_parts():
             if path not in parts:
                 self.get_part(path)
-        target = self._save_target(target)
-        if packaging == "folder":
+        target = self._clean_save_target(target)
+        if packaging == FOLDER:
             if isinstance(target, io.BytesIO):
                 raise TypeError(
                     "Impossible to save on io.BytesIO with 'folder' packaging"
                 )
             self._save_as_folder(target, backup)
+        elif packaging == XML:
+            self._save_as_xml(target, backup)
         else:
             # default:
             self._save_as_zip(target, backup)
```

### Comparing `odfdo-3.7.7/odfdo/content.py` & `odfdo-3.7.8/odfdo/content.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,21 +27,14 @@
 from odfdo.element import Element
 
 from .style import Style
 from .xmlpart import XmlPart
 
 
 class Content(XmlPart):
-    @property
-    def body(self) -> Element:
-        body = self.root.document_body
-        if not isinstance(body, Element):
-            raise ValueError("No body found in document")  # noqa:TRY004
-        return body
-
     # The following two seem useless but they match styles API
 
     def _get_style_contexts(self, family: str | None) -> tuple:
         if family == "font-face":
             return (self.get_element("//office:font-face-decls"),)
         return (
             self.get_element("//office:font-face-decls"),
```

### Comparing `odfdo-3.7.7/odfdo/datatype.py` & `odfdo-3.7.8/odfdo/datatype.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/document.py` & `odfdo-3.7.8/odfdo/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from typing import Any
 from uuid import uuid4
 
 from .cell import Cell  # noqa: F401
 from .const import (
     ODF_CONTENT,
     ODF_MANIFEST,
+    ODF_MANIFEST_NAME,
     ODF_META,
     ODF_SETTINGS,
     ODF_STYLES,
     ODF_TEMPLATES,
     ZIP,
 )
 from .container import Container
@@ -116,21 +117,22 @@
         "manifest": ODF_MANIFEST,
     }.get(path, path)
 
 
 def _get_part_class(
     path: str,
 ) -> type[XmlPart] | None:
+    name = Path(path).name
     return {
         ODF_CONTENT: Content,
         ODF_META: Meta,
         ODF_SETTINGS: XmlPart,
         ODF_STYLES: Styles,
-        ODF_MANIFEST: Manifest,
-    }.get(path)
+        ODF_MANIFEST_NAME: Manifest,
+    }.get(name)
 
 
 def container_from_template(template: str | Path | io.BytesIO) -> Container:
     """Return a Container instance based on template argument.
 
     Internal use only."""
     template_container = Container()
```

### Comparing `odfdo-3.7.7/odfdo/draw_page.py` & `odfdo-3.7.8/odfdo/draw_page.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/element.py` & `odfdo-3.7.8/odfdo/element.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from lxml.etree import (
     XPath,
     _Element,
     fromstring,
     tostring,
 )
 
-from .const import ODF_COLOR_PROPERTY
+from .const import ODF_COLOR_PROPERTY, OFFICE_PREFIX, OFFICE_VERSION
 from .datatype import Boolean, DateTime
 from .utils import (
     FAMILY_MAPPING,
     FAMILY_ODF_STD,
     CachedElement,
     hexa_color,
     make_xpath_query,
@@ -100,60 +100,21 @@
 }
 FIRST_CHILD = 0
 LAST_CHILD = 1
 NEXT_SIBLING = 2
 PREV_SIBLING = 3
 STOPMARKER = 5
 
+"office:version="
 # An empty XML document with all namespaces declared
-NAMESPACES_XML = b"""<?xml version="1.0" encoding="UTF-8"?>
-<office:document
-  xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
-  xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0"
-  xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0"
-  xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0"
-  xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0"
-  xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0"
-  xmlns:xlink="http://www.w3.org/1999/xlink"
-  xmlns:dc="http://purl.org/dc/elements/1.1/"
-  xmlns:meta="urn:oasis:names:tc:opendocument:xmlns:meta:1.0"
-  xmlns:number="urn:oasis:names:tc:opendocument:xmlns:datastyle:1.0"
-  xmlns:presentation="urn:oasis:names:tc:opendocument:xmlns:presentation:1.0"
-  xmlns:svg="urn:oasis:names:tc:opendocument:xmlns:svg-compatible:1.0"
-  xmlns:chart="urn:oasis:names:tc:opendocument:xmlns:chart:1.0"
-  xmlns:dr3d="urn:oasis:names:tc:opendocument:xmlns:dr3d:1.0"
-  xmlns:math="http://www.w3.org/1998/Math/MathML"
-  xmlns:form="urn:oasis:names:tc:opendocument:xmlns:form:1.0"
-  xmlns:script="urn:oasis:names:tc:opendocument:xmlns:script:1.0"
-  xmlns:ooo="http://openoffice.org/2004/office"
-  xmlns:oooc="http://openoffice.org/2004/calc"
-  xmlns:ooow="http://openoffice.org/2004/writer"
-  xmlns:xforms="http://www.w3.org/2002/xforms"
-  xmlns:xsd="http://www.w3.org/2001/XMLSchema"
-  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
-  xmlns:smil="urn:oasis:names:tc:opendocument:xmlns:smil-compatible:1.0"
-  xmlns:anim="urn:oasis:names:tc:opendocument:xmlns:animation:1.0"
-  xmlns:rpt="http://openoffice.org/2005/report"
-  xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
-  xmlns:xhtml="http://www.w3.org/1999/xhtml"
-  xmlns:grddl="http://www.w3.org/2003/g/data-view#"
-  xmlns:officeooo="http://openoffice.org/2009/office"
-  xmlns:tableooo="http://openoffice.org/2009/table"
-  xmlns:drawooo="http://openoffice.org/2010/draw"
-  xmlns:calcext="urn:org:documentfoundation:names:experimental:calc:xmlns:calcext:1.0"
-  xmlns:loext="urn:org:documentfoundation:names:experimental:office:xmlns:loext:1.0"
-  xmlns:field="urn:openoffice:names:experimental:ooo-ms-interop:xmlns:field:1.0"
-  xmlns:formx="urn:openoffice:names:experimental:ooxml-odf-interop:xmlns:form:1.0"
-  xmlns:css3t="http://www.w3.org/TR/css3-text/"
-  xmlns:config="urn:oasis:names:tc:opendocument:xmlns:config:1.0"
-  xmlns:dom="http://www.w3.org/2001/xml-events"
-  xmlns:manifest="urn:oasis:names:tc:opendocument:xmlns:manifest:1.0"
-  xmlns:rdfa="http://docs.oasis-open.org/opendocument/meta/rdfa#"
-  office:version="1.1">%s</office:document>
-"""
+NAMESPACES_XML = (
+    OFFICE_PREFIX
+    + f'office:version="{OFFICE_VERSION}">'.encode()
+    + b"%s</office:document>"
+)
 
 
 class PropDef(NamedTuple):
     name: str
     attr: str
     family: str = ""
 
@@ -1291,15 +1252,15 @@
                 "text:change",
                 "text:change-start",
                 "text:change-end",
                 "text:reference-mark",
                 "text:reference-mark-start",
                 "text:reference-mark-end",
             )
-            request_self = " | ".join(["self::%s" % c for c in clean_tags])
+            request_self = " | ".join([f"self::{tag}" for tag in clean_tags])
             inner = [e for e in inner if not e.xpath(request_self)]
             request = " | ".join([f"descendant::{tag}" for tag in clean_tags])
             for element in inner:
                 to_del = element.xpath(request)
                 for elem in to_del:
                     if isinstance(elem, Element):
                         element.delete(elem)
```

### Comparing `odfdo-3.7.7/odfdo/element_typed.py` & `odfdo-3.7.8/odfdo/element_typed.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,17 @@
             return (value, value_type)
         if value_type in {"float", "percentage", "currency"}:
             read_number = self.get_attribute("office:value")
             if not isinstance(read_number, (Decimal, str)):
                 raise TypeError(f'Wrong type for "office:value": {type(read_number)}')
             value = Decimal(read_number)
             # Return 3 instead of 3.0 if possible
-            if int(value) == value:
-                return (int(value), value_type)
+            with contextlib.suppress(ValueError):
+                if int(value) == value:
+                    return (int(value), value_type)
             return (value, value_type)
         if value_type == "date":
             read_attribute = self.get_attribute("office:date-value")
             if not isinstance(read_attribute, str):
                 raise TypeError(
                     f'Wrong type for "office:date-value": {type(read_attribute)}'
                 )
```

### Comparing `odfdo-3.7.7/odfdo/frame.py` & `odfdo-3.7.8/odfdo/frame.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/header.py` & `odfdo-3.7.8/odfdo/header.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/header_rows.py` & `odfdo-3.7.8/odfdo/header_rows.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/image.py` & `odfdo-3.7.8/odfdo/image.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/link.py` & `odfdo-3.7.8/odfdo/link.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/list.py` & `odfdo-3.7.8/odfdo/list.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/manifest.py` & `odfdo-3.7.8/odfdo/manifest.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/meta.py` & `odfdo-3.7.8/odfdo/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,57 +372,80 @@
             raise ValueError("cycles must be a positive int")
         element = self.get_element("//meta:editing-cycles")
         if element is None:
             element = Element.from_tag("meta:editing-cycles")
             self.get_meta_body().append(element)
         element.text = str(cycles)
 
-    def get_generator(self) -> str | None:
-        """Get the signature of the software that generated this document.
+    @property
+    def generator(self) -> str | None:
+        """Get or set the signature of the software that generated this
+        document.
 
         Return: str (or None if inexistant)
 
         Example::
 
-            >>> document.meta.get_generator()
+            >>> document.meta.generator
             KOffice/2.0.0
+            >>> document.meta.generator = "Odfdo experiment"
         """
         element = self.get_element("//meta:generator")
         if element is None:
             return None
         return element.text
 
+    @generator.setter
+    def generator(self, generator: str) -> None:
+        element = self.get_element("//meta:generator")
+        if element is None:
+            element = Element.from_tag("meta:generator")
+            self.get_meta_body().append(element)
+        element.text = generator
+        self._generator_modified = True
+
+    def get_generator(self) -> str | None:
+        """Get the signature of the software that generated this document.
+
+        (Also available as "self.generator" getter/setter.)
+
+        Return: str (or None if inexistant)
+
+        Example::
+
+            >>> document.meta.get_generator()
+            KOffice/2.0.0
+        """
+        return self.generator
+
     def set_generator(self, generator: str) -> None:
         """Set the signature of the software that generated this document.
 
+        (Also available as "self.generator" getter/setter.)
+
         Arguments:
 
             generator -- str
 
         Example::
 
             >>> document.meta.set_generator("Odfdo experiment")
         """
-        element = self.get_element("//meta:generator")
-        if element is None:
-            element = Element.from_tag("meta:generator")
-            self.get_meta_body().append(element)
-        element.text = generator
-        self._generator_modified = True
+        self.generator = generator
 
     def set_generator_default(self) -> None:
         """Set the signature of the software that generated this document
         to ourself.
 
         Example::
 
             >>> document.meta.set_generator_default()
         """
         if not self._generator_modified:
-            self.set_generator(GENERATOR)
+            self.generator = GENERATOR
 
     def get_statistic(self) -> dict[str, int] | None:
         """Get the statistic from the software that generated this document.
 
         Return: dict (or None if inexistant)
 
         Example::
@@ -532,15 +555,15 @@
             value = str(DateTime.encode(value))
         elif isinstance(value, str):
             value_type = "string"
         elif isinstance(value, timedelta):
             value_type = "time"
             value = str(Duration.encode(value))
         else:
-            raise TypeError('unexpected type "%s" for value' % type(value))
+            raise TypeError(f'unexpected type "{type(value)}" for value')
         # Already the same element ?
         for metadata in self.get_elements("//meta:user-defined"):
             if not isinstance(metadata, Element):
                 continue
             if metadata.get_attribute("meta:name") == name:
                 break
         else:
```

### Comparing `odfdo-3.7.7/odfdo/note.py` & `odfdo-3.7.8/odfdo/note.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/paragraph.py` & `odfdo-3.7.8/odfdo/paragraph.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/paragraph_base.py` & `odfdo-3.7.8/odfdo/paragraph_base.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/reference.py` & `odfdo-3.7.8/odfdo/reference.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/row.py` & `odfdo-3.7.8/odfdo/row.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/scripts/diff.py` & `odfdo-3.7.8/odfdo/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/scripts/folder.py` & `odfdo-3.7.8/odfdo/scripts/folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # Authors: Jerome Dumonteil <jerome.dumonteil@itaapy.com>
 from __future__ import annotations
 
 from argparse import ArgumentParser
 from pathlib import Path
 
 from odfdo import Document, __version__
+from odfdo.const import FOLDER, ZIP
 
 PROG = "odfdo-folder"
 
 
 def configure_parser() -> ArgumentParser:
     description = "Convert standard ODF file to folder, and reverse."
     parser = ArgumentParser(prog=PROG, description=description)
@@ -56,19 +57,18 @@
         print(f"Error: {e}")
         raise SystemExit(1) from None
 
 
 def convert_folder(path_str: str) -> None:
     path = Path(path_str)
     if path.is_file():
-        out_packaging = "folder"
+        out_packaging = FOLDER
     elif path.is_dir():
-        out_packaging = "zip"
+        out_packaging = ZIP
     else:
         raise ValueError(f"Not a file or folder: {path}")
     document = Document(path)
-    pretty = out_packaging == "folder"
-    document.save(packaging=out_packaging, pretty=pretty)
+    document.save(packaging=out_packaging, pretty=False)
 
 
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `odfdo-3.7.7/odfdo/scripts/headers.py` & `odfdo-3.7.8/odfdo/scripts/headers.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/scripts/highlight.py` & `odfdo-3.7.8/odfdo/scripts/highlight.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/scripts/replace.py` & `odfdo-3.7.8/odfdo/scripts/replace.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/scripts/show.py` & `odfdo-3.7.8/odfdo/scripts/show.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/scripts/styles.py` & `odfdo-3.7.8/odfdo/scripts/styles.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/scripts/table_shrink.py` & `odfdo-3.7.8/odfdo/scripts/table_shrink.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/scriptutils.py` & `odfdo-3.7.8/odfdo/scriptutils.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/section.py` & `odfdo-3.7.8/odfdo/section.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/shapes.py` & `odfdo-3.7.8/odfdo/shapes.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/smil.py` & `odfdo-3.7.8/odfdo/smil.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/style.py` & `odfdo-3.7.8/odfdo/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
             break_after -- 'page', 'column' or 'auto'
         """
         self._family: str | None = None
         tag_or_elem = kwargs.get("tag_or_elem", None)
         if tag_or_elem is None:
             family = to_str(family)
             if family not in FAMILY_MAPPING:
-                raise ValueError("Unknown family value: %s" % family)
+                raise ValueError(f"Unknown family value: '{family}'")
             kwargs["tag"] = FAMILY_MAPPING[family]
         super().__init__(**kwargs)
         if self._do_init and family not in SUBCLASSED_STYLES:
             kwargs.pop("tag", None)
             kwargs.pop("tag_or_elem", None)
             self.family = family  # relevant test made by property
             # Common attributes
```

### Comparing `odfdo-3.7.7/odfdo/styles.py` & `odfdo-3.7.8/odfdo/styles.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/table.py` & `odfdo-3.7.8/odfdo/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,26 @@
     insert_map_once,
     isiterable,
     make_cache_map,
     set_item_in_vault,
     translate_from_any,
 )
 
-_xpath_row = xpath_compile("table:table-row")
-_xpath_row_idx = xpath_compile("(table:table-row)[$idx]")
-_xpath_column = xpath_compile("table:table-column")
-_xpath_column_idx = xpath_compile("(table:table-column)[$idx]")
+_xpath_row = xpath_compile(
+    "table:table-row|table:table-rows/table:table-row|table:table-header-rows/table:table-row"
+)
+_xpath_row_idx = xpath_compile(
+    "(table:table-row|table:table-rows/table:table-row|table:table-header-rows/table:table-row)[$idx]"
+)
+_xpath_column = xpath_compile(
+    "table:table-column|table:table-columns/table:table-column|table:table-header-columns/table:table-column"
+)
+_xpath_column_idx = xpath_compile(
+    "(table:table-column|table:table-columns/table:table-column|table:table-header-columns/table:table-column)[$idx]"
+)
 
 
 def _table_name_check(name: Any) -> str:
     if not isinstance(name, str):
         raise TypeError("String required.")
     name = name.strip()
     if not name:
```

### Comparing `odfdo-3.7.7/odfdo/templates/drawing.otg` & `odfdo-3.7.8/odfdo/templates/drawing.otg`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/templates/lpod_styles.odt` & `odfdo-3.7.8/odfdo/templates/lpod_styles.odt`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/templates/presentation.otp` & `odfdo-3.7.8/odfdo/templates/presentation.otp`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/templates/spreadsheet.ots` & `odfdo-3.7.8/odfdo/templates/spreadsheet.ots`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/templates/text.ott` & `odfdo-3.7.8/odfdo/templates/text.ott`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/toc.py` & `odfdo-3.7.8/odfdo/toc.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/tracked_changes.py` & `odfdo-3.7.8/odfdo/tracked_changes.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/__init__.py` & `odfdo-3.7.8/odfdo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/cache_map.py` & `odfdo-3.7.8/odfdo/utils/cache_map.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/cached_element.py` & `odfdo-3.7.8/odfdo/utils/cached_element.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/color.py` & `odfdo-3.7.8/odfdo/utils/color.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/coordinates.py` & `odfdo-3.7.8/odfdo/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/formula.py` & `odfdo-3.7.8/odfdo/utils/formula.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/isiterable.py` & `odfdo-3.7.8/odfdo/utils/isiterable.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/str_convert.py` & `odfdo-3.7.8/odfdo/utils/str_convert.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/style_constants.py` & `odfdo-3.7.8/odfdo/utils/style_constants.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/utils/xpath_query.py` & `odfdo-3.7.8/odfdo/utils/xpath_query.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/variable.py` & `odfdo-3.7.8/odfdo/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,15 +394,15 @@
     ) -> None:
         """display can be: 'number', 'name', 'number-and-name', 'plain-number' or
         'plain-number-and-name'
         """
         super().__init__(**kwargs)
         if self._do_init:
             if display not in VarChapter.DISPLAY_VALUE_CHOICE:
-                raise ValueError("unknown display value: %s" % display)
+                raise ValueError(f"Unknown display value: '{display}'")
             self.display = display
             if outline_level is not None:
                 self.outline_level = outline_level
 
 
 VarChapter._define_attribut_property()
 
@@ -426,15 +426,15 @@
         fixed: bool = False,
         **kwargs: Any,
     ) -> None:
         """display can be: 'full', 'path', 'name' or 'name-and-extension'"""
         super().__init__(**kwargs)
         if self._do_init:
             if display not in VarFileName.DISPLAY_VALUE_CHOICE:
-                raise ValueError("unknown display value: %s" % display)
+                raise ValueError(f"Unknown display value: '{display}'")
             self.display = display
             if fixed:
                 self.fixed = True
 
 
 VarFileName._define_attribut_property()
```

### Comparing `odfdo-3.7.7/odfdo/version.py` & `odfdo-3.7.8/odfdo/version.py`

 * *Files identical despite different names*

### Comparing `odfdo-3.7.7/odfdo/xmlpart.py` & `odfdo-3.7.8/odfdo/xmlpart.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,21 @@
     @property
     def root(self) -> Element:
         if self.__root is None:
             tree = self._get_tree()
             self.__root = Element.from_tag(tree.getroot())
         return self.__root
 
+    @property
+    def body(self) -> Element:
+        body = self.root.document_body
+        if not isinstance(body, Element):
+            raise ValueError(f"No body found in {self.part_name!r}")  # noqa:TRY004
+        return body
+
     def get_elements(self, xpath_query: str) -> list[Element | Text]:
         root = self.root
         return root.xpath(xpath_query)
 
     def get_element(self, xpath_query: str) -> Any:
         result = self.get_elements(xpath_query)
         if not result:
@@ -97,15 +104,17 @@
                 value = getattr(self, name)
                 value = deepcopy(value)
                 setattr(clone, name, value)
         return clone
 
     def serialize(self, pretty: bool = False) -> bytes:
         tree = self._get_tree()
-        # Lxml declaration is too exotic to me
-        data = [b'<?xml version="1.0" encoding="UTF-8"?>']
-        bytes_tree = tostring(tree, pretty_print=pretty, encoding="utf-8")
+        xml_header = b'<?xml version="1.0" encoding="UTF-8"?>\n'
+        bytes_tree = tostring(
+            tree,
+            pretty_print=pretty,
+            encoding="utf8",
+        )
         # Lxml with pretty_print is adding a empty line
         if pretty:
             bytes_tree = bytes_tree.strip()
-        data.append(bytes_tree)
-        return b"\n".join(data)
+        return xml_header + bytes_tree
```

### Comparing `odfdo-3.7.7/pyproject.toml` & `odfdo-3.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odfdo"
-version = "3.7.7"
+version = "3.7.8"
 description = "Python library for OpenDocument Format"
 license = "Apache-2.0"
 keywords = ["python", "library", "ODF", "OpenDocument"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -34,19 +34,19 @@
     { version = ">=4.9.4,<6", python = ">=3.12" },
 ]
 [tool.poetry.group.docs.dependencies]
 pdoc = ">=14.4.0"
 
 [tool.poetry.group.dev.dependencies]
 poetry = "~1.8"
-pytest = ">=7.0"
+pytest = ">=8.0"
 tox = ">=4"
 Pillow = ">=10.0.0"
 lxml-stubs = "*"
-ruff = ">=0.3.4"
+ruff = ">=0.4.2"
 
 [tool.poetry.scripts]
 odfdo-diff = "odfdo.scripts.diff:main"
 odfdo-folder = 'odfdo.scripts.folder:main'
 odfdo-highlight = 'odfdo.scripts.highlight:main'
 odfdo-show = 'odfdo.scripts.show:main'
 odfdo-styles = 'odfdo.scripts.styles:main'
```

### Comparing `odfdo-3.7.7/PKG-INFO` & `odfdo-3.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odfdo
-Version: 3.7.7
+Version: 3.7.8
 Summary: Python library for OpenDocument Format
 Home-page: https://github.com/jdum/odfdo
 License: Apache-2.0
 Keywords: python,library,ODF,OpenDocument
 Author: Jérôme Dumonteil
 Author-email: jerome.dumonteil@gmail.com
 Requires-Python: >=3.9,<4
```

