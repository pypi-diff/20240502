# Comparing `tmp/wlr_layout_ui-1.6.3.tar.gz` & `tmp/wlr_layout_ui-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.6.3.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.6.4.tar", max compression
```

## Comparing `wlr_layout_ui-1.6.3.tar` & `wlr_layout_ui-1.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.3/LICENSE
--rw-r--r--   0        0        0      888 2024-04-29 21:35:54.187715 wlr_layout_ui-1.6.3/README.md
--rw-r--r--   0        0        0      652 2024-05-01 18:59:46.162788 wlr_layout_ui-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     2927 2024-05-01 18:55:10.622445 wlr_layout_ui-1.6.3/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4249 2024-04-29 20:48:36.973600 wlr_layout_ui-1.6.3/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.3/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    24936 2024-05-01 18:57:19.785730 wlr_layout_ui-1.6.3/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.3/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5508 2024-04-29 20:53:16.599453 wlr_layout_ui-1.6.3/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.3/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.3/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4529 2024-05-01 17:21:39.484459 wlr_layout_ui-1.6.3/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12998 2024-05-01 18:51:08.232951 wlr_layout_ui-1.6.3/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.4/LICENSE
+-rw-r--r--   0        0        0      888 2024-04-29 21:35:54.187715 wlr_layout_ui-1.6.4/README.md
+-rw-r--r--   0        0        0      652 2024-05-02 18:21:50.648077 wlr_layout_ui-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     2934 2024-05-02 18:21:25.240782 wlr_layout_ui-1.6.4/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4249 2024-04-29 20:48:36.973600 wlr_layout_ui-1.6.4/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.4/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    25016 2024-05-01 21:28:43.369353 wlr_layout_ui-1.6.4/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.4/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5508 2024-04-29 20:53:16.599453 wlr_layout_ui-1.6.4/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.4/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.4/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4529 2024-05-01 17:21:39.484459 wlr_layout_ui-1.6.4/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12998 2024-05-01 18:51:08.232951 wlr_layout_ui-1.6.4/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.4/PKG-INFO
```

### Comparing `wlr_layout_ui-1.6.3/LICENSE` & `wlr_layout_ui-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.3/README.md` & `wlr_layout_ui-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.3/pyproject.toml` & `wlr_layout_ui-1.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.6.3"
+version = "1.6.4"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
 license = "MIT"
```

### Comparing `wlr_layout_ui-1.6.3/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.6.4/src/wlr_layout_ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 print("No such profile: %s" % sys.argv[1])
                 raise SystemExit(1)
             load()
             p_by_id = {p["uid"]: p for p in profile}
             rects = [
                 (
                     Rect(-i["x"], i["y"], i["height"], i["width"])
-                    if i["transform"] in (1, 3, 5, 7)
+                    if i.get("transform", 0) in (1, 3, 5, 7)
                     else Rect(-i["x"], i["y"], i["width"], i["height"])
                 )
                 for i in profile
             ]
 
             for i, di in enumerate(displayInfo):
                 di.active = p_by_id[di.uid]["active"]
```

### Comparing `wlr_layout_ui-1.6.3/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.6.4/src/wlr_layout_ui/displaywidget.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.3/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.6.4/src/wlr_layout_ui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         but_w = 120
         but_h = 28
 
         # make profiles widgets {{{
         ref_rect = Rect(0, 0, but_w, but_h)
         s_but_style = Style(color=(213, 139, 139))
         act_but_style = Style(color=(139, 233, 202))
+        main_but_style = Style(color=(255, 185, 50))
         p_new_but = Button(
             ref_rect.copy(),
             label="Save new",
             style=s_but_style,
             action=lambda: self.set_text_input(self.action_save_new_profile),
         )
         p_save_but = Button(
@@ -93,26 +94,26 @@
 
         self.sidepanel = VBox(
             widgets=[
                 Button(
                     ref_rect.copy(),
                     label="Apply",
                     action=self.action_save_layout,
-                    style=act_but_style,
+                    style=main_but_style,
                 ),
                 Button(
                     ref_rect.copy(),
                     label="Reload",
                     action=self.action_reload,
-                    style=act_but_style,
+                    style=main_but_style,
                 ),
                 Spacer(
                     ref_rect.copy(),
                     label="Profiles:",
-                    style=act_but_style,
+                    style=Style(text_color=(255, 255, 255, 200)),
                 ),
                 p_new_but,
                 p_save_but,
                 p_load_but,
                 self.profile_list,
             ]
         )
```

### Comparing `wlr_layout_ui-1.6.3/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.6.4/src/wlr_layout_ui/screens.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.3/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.6.4/src/wlr_layout_ui/shapes.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.3/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.6.4/src/wlr_layout_ui/utils.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.3/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.6.4/src/wlr_layout_ui/widgets.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.3/PKG-INFO` & `wlr_layout_ui-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.6.3
+Version: 1.6.4
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

