# Comparing `tmp/wlr_layout_ui-1.6.2.tar.gz` & `tmp/wlr_layout_ui-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.6.2.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.6.3.tar", max compression
```

## Comparing `wlr_layout_ui-1.6.2.tar` & `wlr_layout_ui-1.6.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.2/LICENSE
--rw-r--r--   0        0        0      888 2024-04-29 21:35:54.187715 wlr_layout_ui-1.6.2/README.md
--rw-r--r--   0        0        0      652 2024-04-29 21:55:15.488535 wlr_layout_ui-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     2435 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.2/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4249 2024-04-29 20:48:36.973600 wlr_layout_ui-1.6.2/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.2/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    24791 2024-04-29 21:55:03.391612 wlr_layout_ui-1.6.2/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.2/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5508 2024-04-29 20:53:16.599453 wlr_layout_ui-1.6.2/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.2/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.2/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4529 2024-04-29 21:19:26.061682 wlr_layout_ui-1.6.2/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12366 2024-04-29 20:52:12.478107 wlr_layout_ui-1.6.2/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.3/LICENSE
+-rw-r--r--   0        0        0      888 2024-04-29 21:35:54.187715 wlr_layout_ui-1.6.3/README.md
+-rw-r--r--   0        0        0      652 2024-05-01 18:59:46.162788 wlr_layout_ui-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2927 2024-05-01 18:55:10.622445 wlr_layout_ui-1.6.3/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4249 2024-04-29 20:48:36.973600 wlr_layout_ui-1.6.3/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.3/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    24936 2024-05-01 18:57:19.785730 wlr_layout_ui-1.6.3/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.3/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5508 2024-04-29 20:53:16.599453 wlr_layout_ui-1.6.3/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.3/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.3/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4529 2024-05-01 17:21:39.484459 wlr_layout_ui-1.6.3/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12998 2024-05-01 18:51:08.232951 wlr_layout_ui-1.6.3/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.3/PKG-INFO
```

### Comparing `wlr_layout_ui-1.6.2/LICENSE` & `wlr_layout_ui-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.2/README.md` & `wlr_layout_ui-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.2/pyproject.toml` & `wlr_layout_ui-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.6.2"
+version = "1.6.3"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
 license = "MIT"
```

### Comparing `wlr_layout_ui-1.6.2/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.6.3/src/wlr_layout_ui/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,30 @@
             try:
                 profile = profiles[sys.argv[1]]
             except KeyError:
                 print("No such profile: %s" % sys.argv[1])
                 raise SystemExit(1)
             load()
             p_by_id = {p["uid"]: p for p in profile}
-            rects = [Rect(i["x"], i["y"], i["width"], i["height"]) for i in profile]
-            for di in displayInfo:
+            rects = [
+                (
+                    Rect(-i["x"], i["y"], i["height"], i["width"])
+                    if i["transform"] in (1, 3, 5, 7)
+                    else Rect(-i["x"], i["y"], i["width"], i["height"])
+                )
+                for i in profile
+            ]
+
+            for i, di in enumerate(displayInfo):
                 di.active = p_by_id[di.uid]["active"]
+                di.transform = p_by_id[di.uid].get("transform", 0)
+                di.scale = p_by_id[di.uid].get("scale", 1.0)
+                if di.transform in (1, 3, 5, 7):
+                    rects[i].width, rects[i].height = rects[i].height, rects[i].width
+
             cmd = make_command(displayInfo, rects, not LEGACY)
             time.sleep(0.5)
             if os.system(cmd):
                 print("Failed applying the layout")
         sys.exit(0)
     load()
     max_width = int(
```

### Comparing `wlr_layout_ui-1.6.2/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.6.3/src/wlr_layout_ui/displaywidget.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.2/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.6.3/src/wlr_layout_ui/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,25 @@
     config,
     find_matching_mode,
     make_command,
     sorted_frequencies,
     sorted_resolutions,
     trim_rects_flip_y,
 )
-from .widgets import Button, Dropdown, HBox, Style, VBox, Widget
+from .widgets import Button, Dropdown, HBox, Style, VBox, Widget, Spacer
 
 hex_re = re.compile("^[0-9x]+$")
 
 CONFIRM_DELAY = 20
 
 
+def get_closest_match(float_list, value):
+    return min(float_list, key=lambda x: abs(x - value))
+
+
 def get_size(screen, scale=0):
     "Get the size of the window based on the screen size and UI_RATIO"
     if not scale:
         scale = UI_RATIO
     w, h = ((screen.mode.width / scale) / screen.scale), (
         (screen.mode.height / scale) / screen.scale
     )
@@ -84,38 +88,44 @@
             label="Load",
             style=act_but_style,
             action=self.action_load_selected_profile,
         )
         self.profile_list = Dropdown(ref_rect.copy(), label="Profiles", options=[])
 
         self.sidepanel = VBox(
-            widgets=[p_new_but, p_save_but, p_load_but, self.profile_list]
-        )
-        self.sync_profiles()
-
-        # }}}
-
-        # make main buttons {{{
-        ref_rect = Rect(0, 0, but_w, but_h)
-        self.action_box = VBox(
             widgets=[
                 Button(
                     ref_rect.copy(),
                     label="Apply",
                     action=self.action_save_layout,
                     style=act_but_style,
                 ),
                 Button(
                     ref_rect.copy(),
                     label="Reload",
                     action=self.action_reload,
                     style=act_but_style,
                 ),
+                Spacer(
+                    ref_rect.copy(),
+                    label="Profiles:",
+                    style=act_but_style,
+                ),
+                p_new_but,
+                p_save_but,
+                p_load_but,
+                self.profile_list,
             ]
         )
+        self.sync_profiles()
+
+        # }}}
+
+        # make main buttons {{{
+        ref_rect = Rect(0, 0, but_w, but_h)
 
         ref_rect.width = int(ref_rect.width * 1.2)
         self.resolutions = Dropdown(
             ref_rect.copy(),
             label="Resolution",
             options=[],
             onchange=self.action_update_screen_spec,
@@ -168,38 +178,36 @@
             toggled_label="Off",
             action=self.action_toggle_screen_power,
             style=Style(highlight=(200, 100, 150), color=(100, 200, 150)),
             togglable=True,
         )
 
         base_widgets: list[Widget] = [
+            self.on_off_but,
             self.resolutions,
             self.freqs,
         ]
         if config.get("hyprland"):
             base_widgets.append(self.rotation)
             base_widgets.append(self.scale_ratio)
-        base_widgets.append(self.on_off_but)
 
         self.settings_box = HBox(widgets=base_widgets)
         self.require_selected_item.add(self.settings_box)
         # }}}
 
         self._widgets: list[Widget] = [
-            self.action_box,
             self.settings_box,
             self.sidepanel,
         ]
         for w in self._widgets:
             w.margin = WINDOW_MARGIN
 
         # alignment
-        self.action_box.set_alignment("top", "left")
-        self.settings_box.set_alignment("top")
-        self.sidepanel.set_alignment("top", "right")
+        self.settings_box.set_alignment("top", "right")
+        self.sidepanel.set_alignment("top", "left")
 
         self.gui_screens: list[GuiScreen] = []
         self.load_screens()
         # Ensure correct positioning
         self.on_resize(width, height)
         self.set_current_modes_as_ref()
 
@@ -243,37 +251,28 @@
             max_height = max(m.height for m in screen.available)
 
             is_rotated = screen.transform in (1, 3, 5, 7)
 
             if screen.mode:
 
                 w, h = get_size(screen)
-                h = int(
-                    (screen.mode.height if is_rotated else screen.mode.height)
-                    / UI_RATIO
-                    / screen.scale
-                )
-                if is_rotated:
-                    y -= screen.mode.height - screen.mode.width
-
                 rect = Rect(
                     int(x / UI_RATIO),
                     -int(y / UI_RATIO) - h,
                     w,
                     h,
                 )
             else:
                 rect = Rect(
                     int(x / UI_RATIO),
                     int(y / UI_RATIO),
                     int((max_width / UI_RATIO) / screen.scale),
                     int((max_height / UI_RATIO) / screen.scale),
                 )
-            if is_rotated:
-                rect.width, rect.height = rect.height, rect.width
+
             gs = GuiScreen(screen, rect)
             gs.genColor()
             gui_screens.append(gs)
 
         max_x = max(s.rect.right for s in gui_screens)
         min_x = min(s.rect.left for s in gui_screens)
         min_y = min(s.rect.top for s in gui_screens)
@@ -569,14 +568,15 @@
         GuiScreen.cur_color = 0
         self.load_screens()
 
     def action_reload(self):
         reload_pre_commands()
         time.sleep(0.5)
         self.reset_sel()
+        self.center_layout(immediate=True)
 
     def get_profile_data(self):
         screens_rect = [
             screen.target_rect.scaled(UI_RATIO) for screen in self.gui_screens
         ]
         trim_rects_flip_y(screens_rect)
         ret = []
@@ -587,14 +587,15 @@
                     "active": gs.screen.active,
                     "width": gs.screen.mode.width,
                     "height": gs.screen.mode.height,
                     "freq": gs.screen.mode.freq,
                     "x": rect.x,
                     "y": rect.y,
                     "uid": gs.screen.uid,
+                    "scale": gs.screen.scale,
                     "transform": gs.screen.transform,
                 }
             )
         return ret
 
     def action_save_new_profile(self):
         assert self.text_input
@@ -705,14 +706,19 @@
 
         cur_mode = screen.screen.mode
         # Update resolution
         res = sorted_resolutions(screen.screen.available)
         self.resolutions.options = [
             {"name": f"{r[0]} x {r[1]}", "value": r} for r in res
         ]
+        self.rotation.selected_index = screen.screen.transform
+        values = [o["value"] for o in self.scale_ratio.options]
+        self.scale_ratio.selected_index = values.index(
+            get_closest_match(values, screen.screen.scale)
+        )
         i = -1
         for i, r in enumerate(res):
             if r[0] == cur_mode.width and r[1] == cur_mode.height:
                 break
         self.resolutions.selected_index = i
         self.rotation.selected_index = screen.screen.transform
         self.action_update_frequencies(screen)
```

### Comparing `wlr_layout_ui-1.6.2/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.6.3/src/wlr_layout_ui/screens.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.2/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.6.3/src/wlr_layout_ui/shapes.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.2/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.6.3/src/wlr_layout_ui/utils.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.2/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.6.3/src/wlr_layout_ui/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,36 @@
     def get_selected_index(self):
         return self.selected_index
 
 
 # }}}
 
 
+class Spacer(Widget):  # {{{
+    "Represents an empty space in the layout, with an optional label"
+
+    def __init__(self, rect, label="", style=None):
+        super().__init__(rect, style)
+        self.label = label
+
+    def draw(self, cursor):
+        if self.label:
+            makeLabel(
+                self.label,
+                x=self.rect.x + self.rect.width // 2,
+                y=self.rect.y + self.rect.height // 2,
+                anchor_x="center",
+                anchor_y="center",
+                color=self.style.text_color,
+            ).draw()
+
+    def __repr__(self):
+        return f"<Spacer {self.label}>"
+
+
 class Button(Widget):  # {{{
     def __init__(
         self,
         rect,
         label,
         style=None,
         action=lambda: None,
```

### Comparing `wlr_layout_ui-1.6.2/PKG-INFO` & `wlr_layout_ui-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.6.2
+Version: 1.6.3
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

