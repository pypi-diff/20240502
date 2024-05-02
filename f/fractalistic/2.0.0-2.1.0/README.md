# Comparing `tmp/fractalistic-2.0.0.tar.gz` & `tmp/fractalistic-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractalistic-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractalistic-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractalistic-2.0.0.tar` & `fractalistic-2.1.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0       30 2023-11-27 19:49:07.456040 fractalistic-2.0.0/.flake8
--rw-r--r--   0        0        0       84 2023-11-27 19:49:07.456040 fractalistic-2.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1706 2023-11-27 19:49:07.456040 fractalistic-2.0.0/.github/ISSUE_TEMPLATE/BUG_REPORT.yml
--rw-r--r--   0        0        0      667 2023-11-27 19:49:07.456040 fractalistic-2.0.0/.github/ISSUE_TEMPLATE/EMPTY_ISSUE.yml
--rw-r--r--   0        0        0     1100 2023-11-27 19:49:07.456040 fractalistic-2.0.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.yml
--rw-r--r--   0        0        0       28 2023-11-27 19:49:07.456040 fractalistic-2.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      558 2023-11-27 19:49:07.456040 fractalistic-2.0.0/.github/workflows/greeting.yml
--rw-r--r--   0        0        0     3077 2023-11-27 19:49:07.456040 fractalistic-2.0.0/.gitignore
--rw-r--r--   0        0        0     2154 2023-11-27 19:50:49.722967 fractalistic-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1114 2023-11-27 19:49:07.456040 fractalistic-2.0.0/LICENSE
--rw-r--r--   0        0        0     5640 2023-11-27 19:50:49.722967 fractalistic-2.0.0/README.md
--rw-r--r--   0        0        0    92810 2023-11-27 19:49:07.460040 fractalistic-2.0.0/assets/banner.png
--rw-r--r--   0        0        0    19694 2023-11-27 19:49:07.460040 fractalistic-2.0.0/assets/logo.png
--rw-r--r--   0        0        0   734491 2023-11-27 19:49:07.460040 fractalistic-2.0.0/assets/screenshot0.png
--rw-r--r--   0        0        0    63598 2023-11-27 19:49:07.460040 fractalistic-2.0.0/assets/screenshot1.png
--rw-r--r--   0        0        0   316839 2023-11-27 19:49:07.464040 fractalistic-2.0.0/assets/screenshot10.png
--rw-r--r--   0        0        0    86013 2023-11-27 19:49:07.464040 fractalistic-2.0.0/assets/screenshot11.png
--rw-r--r--   0        0        0   518438 2023-11-27 19:49:07.468040 fractalistic-2.0.0/assets/screenshot12.png
--rw-r--r--   0        0        0  1299126 2023-11-27 19:49:07.468040 fractalistic-2.0.0/assets/screenshot13.png
--rw-r--r--   0        0        0   669984 2023-11-27 19:50:49.730966 fractalistic-2.0.0/assets/screenshot14.png
--rw-r--r--   0        0        0   747290 2023-11-27 19:50:49.730966 fractalistic-2.0.0/assets/screenshot15.png
--rw-r--r--   0        0        0    83013 2023-11-27 19:49:07.468040 fractalistic-2.0.0/assets/screenshot2.png
--rw-r--r--   0        0        0   138349 2023-11-27 19:49:07.472040 fractalistic-2.0.0/assets/screenshot3.png
--rw-r--r--   0        0        0   208848 2023-11-27 19:49:07.472040 fractalistic-2.0.0/assets/screenshot4.png
--rw-r--r--   0        0        0   715333 2023-11-27 19:49:07.472040 fractalistic-2.0.0/assets/screenshot5.png
--rw-r--r--   0        0        0   128194 2023-11-27 19:49:07.476040 fractalistic-2.0.0/assets/screenshot6.png
--rw-r--r--   0        0        0   225118 2023-11-27 19:49:07.476040 fractalistic-2.0.0/assets/screenshot7.png
--rw-r--r--   0        0        0   268108 2023-11-27 19:49:07.480040 fractalistic-2.0.0/assets/screenshot8.png
--rw-r--r--   0        0        0   205556 2023-11-27 19:49:07.480040 fractalistic-2.0.0/assets/screenshot9.png
--rw-r--r--   0        0        0      310 2023-11-27 19:50:49.730966 fractalistic-2.0.0/cool_locations/1.fc
--rw-r--r--   0        0        0      158 2023-11-27 19:49:07.480040 fractalistic-2.0.0/cool_locations/info.txt
--rw-r--r--   0        0        0      109 2023-11-27 19:50:49.730966 fractalistic-2.0.0/fractalistic/__init__.py
--rw-r--r--   0        0        0     3572 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/__main__.py
--rw-r--r--   0        0        0    40711 2023-11-27 19:50:49.730966 fractalistic-2.0.0/fractalistic/app.py
--rw-r--r--   0        0        0      381 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/app.tcss
--rw-r--r--   0        0        0      585 2023-11-27 19:50:49.730966 fractalistic-2.0.0/fractalistic/click_modes.py
--rw-r--r--   0        0        0     1577 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/colors.py
--rw-r--r--   0        0        0     3065 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/command.py
--rw-r--r--   0        0        0      784 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/fractal_canv.py
--rw-r--r--   0        0        0      147 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/fractals/__init__.py
--rw-r--r--   0        0        0      602 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/fractals/burning_ship.py
--rw-r--r--   0        0        0      406 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/fractals/fractal_base.py
--rw-r--r--   0        0        0      629 2023-11-27 19:50:49.730966 fractalistic-2.0.0/fractalistic/fractals/julia.py
--rw-r--r--   0        0        0      595 2023-11-27 19:50:49.730966 fractalistic-2.0.0/fractalistic/fractals/mandelbrot.py
--rw-r--r--   0        0        0      163 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/line_divergence_result.py
--rw-r--r--   0        0        0     2731 2023-11-27 19:50:49.730966 fractalistic-2.0.0/fractalistic/settings.py
--rw-r--r--   0        0        0     1691 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/utils.py
--rw-r--r--   0        0        0      205 2023-11-27 19:49:07.480040 fractalistic-2.0.0/fractalistic/vec.py
--rw-r--r--   0        0        0      705 2023-11-27 19:50:49.730966 fractalistic-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6271 1970-01-01 00:00:00.000000 fractalistic-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-11-24 18:26:27.627140 fractalistic-2.1.0/.flake8
+-rw-r--r--   0        0        0       84 2023-10-26 09:56:27.314127 fractalistic-2.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1706 2023-10-26 09:47:19.247350 fractalistic-2.1.0/.github/ISSUE_TEMPLATE/BUG_REPORT.yml
+-rw-r--r--   0        0        0      667 2023-10-26 09:47:19.247350 fractalistic-2.1.0/.github/ISSUE_TEMPLATE/EMPTY_ISSUE.yml
+-rw-r--r--   0        0        0     1100 2023-10-26 09:47:19.247350 fractalistic-2.1.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.yml
+-rw-r--r--   0        0        0       28 2023-10-26 09:47:19.247350 fractalistic-2.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      558 2023-11-25 08:46:54.076459 fractalistic-2.1.0/.github/workflows/greeting.yml
+-rw-r--r--   0        0        0     3077 2023-10-26 09:47:19.247350 fractalistic-2.1.0/.gitignore
+-rw-r--r--   0        0        0     2385 2024-05-02 09:07:04.857987 fractalistic-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1114 2023-10-26 09:47:19.247350 fractalistic-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5595 2024-05-02 07:30:42.086420 fractalistic-2.1.0/README.md
+-rw-r--r--   0        0        0    92810 2023-11-24 18:26:27.631140 fractalistic-2.1.0/assets/banner.png
+-rw-r--r--   0        0        0    19694 2023-11-24 18:26:27.631140 fractalistic-2.1.0/assets/logo.png
+-rw-r--r--   0        0        0   734491 2023-11-24 20:24:45.117208 fractalistic-2.1.0/assets/screenshot0.png
+-rw-r--r--   0        0        0    63598 2023-11-24 18:26:27.635140 fractalistic-2.1.0/assets/screenshot1.png
+-rw-r--r--   0        0        0   316839 2023-11-24 18:26:27.635140 fractalistic-2.1.0/assets/screenshot10.png
+-rw-r--r--   0        0        0    86013 2023-11-24 18:26:27.635140 fractalistic-2.1.0/assets/screenshot11.png
+-rw-r--r--   0        0        0   518438 2023-11-24 20:24:45.121208 fractalistic-2.1.0/assets/screenshot12.png
+-rw-r--r--   0        0        0  1299126 2023-11-24 20:24:45.121208 fractalistic-2.1.0/assets/screenshot13.png
+-rw-r--r--   0        0        0   236954 2024-05-02 07:30:42.090420 fractalistic-2.1.0/assets/screenshot14.png
+-rw-r--r--   0        0        0   461061 2024-05-02 07:30:42.090420 fractalistic-2.1.0/assets/screenshot15.png
+-rw-r--r--   0        0        0   455395 2024-05-02 07:30:42.094420 fractalistic-2.1.0/assets/screenshot16.png
+-rw-r--r--   0        0        0    83013 2023-11-24 18:26:27.643140 fractalistic-2.1.0/assets/screenshot2.png
+-rw-r--r--   0        0        0   138349 2023-11-24 18:26:27.643140 fractalistic-2.1.0/assets/screenshot3.png
+-rw-r--r--   0        0        0   208848 2023-11-24 18:26:27.643140 fractalistic-2.1.0/assets/screenshot4.png
+-rw-r--r--   0        0        0   715333 2023-11-24 18:26:27.643140 fractalistic-2.1.0/assets/screenshot5.png
+-rw-r--r--   0        0        0   128194 2023-11-24 18:26:27.643140 fractalistic-2.1.0/assets/screenshot6.png
+-rw-r--r--   0        0        0   225118 2023-11-24 18:26:27.647140 fractalistic-2.1.0/assets/screenshot7.png
+-rw-r--r--   0        0        0   268108 2023-11-24 18:26:27.647140 fractalistic-2.1.0/assets/screenshot8.png
+-rw-r--r--   0        0        0   205556 2023-11-24 18:26:27.647140 fractalistic-2.1.0/assets/screenshot9.png
+-rw-r--r--   0        0        0      310 2024-05-02 07:30:42.094420 fractalistic-2.1.0/cool_locations/1.fc
+-rw-r--r--   0        0        0      158 2023-11-24 18:26:27.647140 fractalistic-2.1.0/cool_locations/info.txt
+-rw-r--r--   0        0        0      109 2024-05-02 09:07:04.857987 fractalistic-2.1.0/fractalistic/__init__.py
+-rw-r--r--   0        0        0     3572 2023-11-24 18:26:27.647140 fractalistic-2.1.0/fractalistic/__main__.py
+-rw-r--r--   0        0        0    47568 2024-05-02 09:07:04.857987 fractalistic-2.1.0/fractalistic/app.py
+-rw-r--r--   0        0        0      381 2023-10-29 19:38:33.317747 fractalistic-2.1.0/fractalistic/app.tcss
+-rw-r--r--   0        0        0      675 2024-05-02 07:30:42.094420 fractalistic-2.1.0/fractalistic/click_modes.py
+-rw-r--r--   0        0        0     1577 2023-11-24 18:26:27.647140 fractalistic-2.1.0/fractalistic/colors.py
+-rw-r--r--   0        0        0     2984 2024-05-02 09:07:04.857987 fractalistic-2.1.0/fractalistic/command.py
+-rw-r--r--   0        0        0      784 2023-11-24 20:24:45.121208 fractalistic-2.1.0/fractalistic/fractal_canv.py
+-rw-r--r--   0        0        0      208 2024-05-02 07:30:42.094420 fractalistic-2.1.0/fractalistic/fractals/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-02 07:30:42.094420 fractalistic-2.1.0/fractalistic/fractals/burning_ship.py
+-rw-r--r--   0        0        0      406 2023-11-24 18:26:27.647140 fractalistic-2.1.0/fractalistic/fractals/fractal_base.py
+-rw-r--r--   0        0        0      698 2024-05-02 07:30:42.094420 fractalistic-2.1.0/fractalistic/fractals/inv_mandel.py
+-rw-r--r--   0        0        0      629 2024-05-02 07:30:42.094420 fractalistic-2.1.0/fractalistic/fractals/julia.py
+-rw-r--r--   0        0        0      595 2024-05-02 07:30:42.094420 fractalistic-2.1.0/fractalistic/fractals/mandelbrot.py
+-rw-r--r--   0        0        0      163 2023-11-24 21:13:57.087481 fractalistic-2.1.0/fractalistic/line_divergence_result.py
+-rw-r--r--   0        0        0     2997 2024-05-02 07:30:42.094420 fractalistic-2.1.0/fractalistic/settings.py
+-rw-r--r--   0        0        0     1831 2024-05-02 07:30:42.094420 fractalistic-2.1.0/fractalistic/utils.py
+-rw-r--r--   0        0        0      205 2023-11-24 18:26:27.647140 fractalistic-2.1.0/fractalistic/vec.py
+-rw-r--r--   0        0        0      705 2024-05-02 07:30:42.094420 fractalistic-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6226 1970-01-01 00:00:00.000000 fractalistic-2.1.0/PKG-INFO
```

### Comparing `fractalistic-2.0.0/.github/ISSUE_TEMPLATE/BUG_REPORT.yml` & `fractalistic-2.1.0/.github/ISSUE_TEMPLATE/BUG_REPORT.yml`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/.github/ISSUE_TEMPLATE/EMPTY_ISSUE.yml` & `fractalistic-2.1.0/.github/ISSUE_TEMPLATE/EMPTY_ISSUE.yml`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.yml` & `fractalistic-2.1.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.yml`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/.github/workflows/greeting.yml` & `fractalistic-2.1.0/.github/workflows/greeting.yml`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/.gitignore` & `fractalistic-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/CHANGELOG.md` & `fractalistic-2.1.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# 2.1.0 - 2024-05-02
+
+### Added
+- Inverse mandelbrot set
+- `fractal` command
+- `color` command
+- Custom burning ship exponent
+
+### Improved
+- Beautiful log messages
+
+### Fixed
+- Bug with custom exponents
+- Errors in help messages
+
 # 2.0.0 - 2023-11-27
 
 ### Added
 - New render parameters
 - Julia/Mandelbrot custom exponents
 - Custom Mandelbrot start point
```

### Comparing `fractalistic-2.0.0/LICENSE` & `fractalistic-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/README.md` & `fractalistic-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 - 📌 Click to show coordinates and divergence
 - 🏃 Multithreaded rendering
 
 # Roadmap
 
 Possible features to add later:
 - [ ] Splash screen
-- [ ] app.log_error(), etc utility functions
 - [ ] New mandelbrot variants
 
 Commands:
 - [ ] Command to show current pos, zoom, etc
 
 # How to migrate your state files to >= 2.0.0
```

### Comparing `fractalistic-2.0.0/assets/banner.png` & `fractalistic-2.1.0/assets/banner.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/logo.png` & `fractalistic-2.1.0/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot0.png` & `fractalistic-2.1.0/assets/screenshot0.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot1.png` & `fractalistic-2.1.0/assets/screenshot1.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot10.png` & `fractalistic-2.1.0/assets/screenshot10.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot11.png` & `fractalistic-2.1.0/assets/screenshot11.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot12.png` & `fractalistic-2.1.0/assets/screenshot12.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot13.png` & `fractalistic-2.1.0/assets/screenshot13.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot2.png` & `fractalistic-2.1.0/assets/screenshot2.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot3.png` & `fractalistic-2.1.0/assets/screenshot3.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot4.png` & `fractalistic-2.1.0/assets/screenshot4.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot5.png` & `fractalistic-2.1.0/assets/screenshot5.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot6.png` & `fractalistic-2.1.0/assets/screenshot6.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot7.png` & `fractalistic-2.1.0/assets/screenshot7.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot8.png` & `fractalistic-2.1.0/assets/screenshot8.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/assets/screenshot9.png` & `fractalistic-2.1.0/assets/screenshot9.png`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/fractalistic/__main__.py` & `fractalistic-2.1.0/fractalistic/__main__.py`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/fractalistic/app.py` & `fractalistic-2.1.0/fractalistic/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from textual.events import Click
 from textual.color import Color
 from textual import on
 from textual import log
 # ---------- Local imports
 from . import fractals, colors, __version__
 from .utils import (
-    SRC_DIR, get_divergence_matrix, set_precision, pos_to_c)
+    SRC_DIR, get_divergence_matrix, set_precision, pos_to_c,
+    get_fractal_index_from_name, get_color_index_from_name)
 from .fractals.fractal_base import FractalBase
 from .vec import Vec
 from .click_modes import CLICK_MODES
 from .settings import Settings, RenderSettings, StateInfo
 from .command import Command, CommandIncrement, CommandIncrementArgParseResult
 from .fractal_canv import FractalCanv
 from .line_divergence_result import LineDivergenceResult
@@ -91,129 +92,76 @@
     # ---------- COMMANDS
 
     # ========== increment type commands
 
     def command_max_iter(self, value: int) -> None:
         self.render_settings.max_iter = value
 
-        self.log_write(f"max_iter set to [blue]{self.render_settings.max_iter}")
+        self.log_success(f"max_iter set to [blue]{self.render_settings.max_iter}")
         self.update_canv()
 
-    def command_zoom_lvl(self, value: int) -> None:
-        self.settings.zoom_intensity = value
-        self.log_write(f"Zoom level set to [blue]{self.settings.zoom_intensity}%")
-
     def command_move_dist(self, value: int) -> None:
         self.settings.move_distance = value
-        self.log_write(f"Move distance set to [blue]{self.settings.move_distance}")
+        self.log_success(f"Move distance set to [blue]{self.settings.move_distance}")
 
     def command_precision(self, value: int) -> None:
         self.precision = value
 
-        self.log_write(f"Numeric precision set to [blue]{value}")
+        self.log_success(f"Numeric precision set to [blue]{value}")
         self.update_canv()
 
-    def command_threads(self, value: int) -> None:
-        self.settings.threads = value
-        self.log_write(f"Rendering thread count set to [blue]{self.settings.threads}")
-
     def command_screenshot_threads(self, value: int) -> None:
         self.settings.screenshot_threads = value
-        self.log_write(f"Screenshot thread count set to [blue]{self.settings.screenshot_threads}")
-
-    # ========== other commands
-
-    def command_help(self, args, argc: int) -> None:
-        if argc == 0:
-            command_desc = [
-                f"- [blue]{name}[/blue]: {self.command_list[name].help}"
-                for name in self.command_list
-            ]
+        self.log_success(f"Screenshot thread count set to [blue]{self.settings.screenshot_threads}")
 
-            self.log_write([
-                "[on blue]Available commands",
-                *command_desc,
-                "[green]Use 'help command_name' to get more info about a command"
-            ])
-
-        elif argc == 1:
-            command = self.get_command(args[0])
-            if command is None:
-                return
-
-            self.log_write([
-                f"[on blue]{args[0]} command",
-                command.help,
-                command.extra_help
-            ])
-
-    def command_clear(self, args, argc: int) -> None:
-        self.rich_log.clear()
-        self.print_log_bar = False
-
-    def command_quit(self, args, argc: int) -> None:
-        self.log_write("Quitting...")
-        self.exit()
+    def command_threads(self, value: int) -> None:
+        self.settings.threads = value
+        self.log_success(f"Rendering thread count set to [blue]{self.settings.threads}")
 
-    def command_version(self, args, argc: int) -> None:
-        self.log_write(f"Fractalistic version: [on blue]{__version__}")
+    def command_zoom_lvl(self, value: int) -> None:
+        self.settings.zoom_intensity = value
+        self.log_success(f"Zoom level set to [blue]{self.settings.zoom_intensity}%")
 
+    # ========== other commands
     def command_capture(self, args, argc: int) -> None:
         if argc == 0:
             self.action_screenshot()
         elif argc == 2:
             try:
                 width = int(args[0])
                 height = int(args[1])
             except ValueError:
-                self.log_write("Width and height must be integers")
+                self.log_error("Width and height must be integers")
                 return
 
             if width <= 0 or height <= 0:
-                self.log_write("Width and height must be positive")
+                self.log_error("Width and height must be positive")
                 return
 
             self.action_screenshot(Vec(width, height))
 
     def command_capture_fit(self, args, argc: int) -> None:
         if argc == 0:
             self.action_screenshot(self.get_screenshot_size_fit())
         elif argc == 1:
             try:
                 quality = int(args[0])
             except ValueError:
-                self.log_write("Quality must be an integer")
+                self.log_error("Quality must be an integer")
                 return
 
             if quality <= 0:
-                self.log_write("Quality must be positive")
+                self.log_error("Quality must be positive")
                 return
 
             self.action_screenshot(self.get_screenshot_size_fit(quality))
 
-    def command_pos(self, args, argc: int) -> None:
-        # If no args are provided, just show the current position
-        if argc == 0:
-            self.log_write(f"Current position: [blue]{self.render_settings.screen_pos_on_plane}")
-            return
-
-        # If args are provided, go to the given x and y position
-        real = None
-        imag = None
-        try:
-            real = mpfr(args[0])
-            imag = mpfr(args[1])
-        except ValueError:
-            self.log_write("Real and imaginary parts must be valid integers or floats")
-            return
-
-        self.render_settings.screen_pos_on_plane = mpc(real, imag)
-
-        # Update canvas since we just moved
-        self.update_canv()
+    def command_clear(self, args, argc: int) -> None:
+        self.rich_log.clear()
+        self.print_log_bar = False
 
     def command_click_mode(self, args: list[str], argc: int) -> None:
         # If no args are provided, print the current modes
         # and the available modes.
         if argc == 0:
             self.log_write([
                 "[purple]Available modes:[/purple]"
@@ -221,126 +169,249 @@
                 f"\nCurrent left click mode: [blue]{self.settings.left_click_mode_name}[/blue]",
                 f"Current right click mode: [blue]{self.settings.right_click_mode_name}[/blue]",
             ])
             return
 
         # If two args were provided
         if args[0] not in ["left", "right"]:
-            self.log_write("[red]First argument must be 'left' or 'right'")
+            self.log_error("[red]First argument must be 'left' or 'right'")
             return
 
         if args[1] not in CLICK_MODES:
-            self.log_write(f"[red]Second argument must be one of: {', '.join([mode for mode in CLICK_MODES])}")
+            self.log_error(f"[red]Second argument must be one of: {', '.join([mode for mode in CLICK_MODES])}")
             return
 
         if args[0] == "left":
             self.settings.left_click_mode_name = args[1]
         else:
             self.settings.right_click_mode_name = args[1]
 
-        self.log_write(f"{args[0].capitalize()} click mode set to [blue]{args[1]}")
+        self.log_success(f"{args[0].capitalize()} click mode set to [blue]{args[1]}")
 
-    def command_save_state(self, args, argc: int) -> None:
+    def command_color(self, args, argc: int) -> None:
         if argc == 0:
-            filename = f"{self.selected_fractal.__name__}_state_{int(time())}.fc"
-        else:
-            filename = args[0]
-
-        try:
-            with open(filename, "wb") as f:
-                state_info = StateInfo()
-                state_info.render_settings = self.render_settings
-                pickle.dump(state_info, f)
-        except OSError as e:
-            self.log_write(f"Cannot write to file '{filename}'. [red]Errno {e.errno}: {e.strerror}.")
+            self.log_write([
+                f"Current color: [blue]{self.selected_color.__name__}[/blue]",
+                "Available colors: "
+                f"{', '.join([f'[violet]{color.__name__}[/violet]' for color in colors.color_renderers])}"
+            ])
             return
 
-        self.log_write(f"State saved to [blue]{filename}")
+        color_name = args[0]
+        color_index = get_color_index_from_name(color_name)
 
-    def command_load_state(self, args, argc: int) -> None:
-        self.load_state(args[0])
+        if color_index is None:
+            self.log_error(f"Cannot find color [white on red]{color_name}")
+            return
+
+        self.render_settings.color_renderer_index = color_index
+        self.log_success(f"Current color set to [blue]{self.selected_color.__name__}")
         self.update_canv()
 
     def command_exp_type(self, args, argc: int) -> None:
         if argc == 0:
             self.log_write([
                 f"Julia exponent type: [blue]{type(self.render_settings.julia_exponent).__name__}[/blue]",
-                f"Mandelbrot exponent type: [blue]{type(self.render_settings.mandelbrot_exponent).__name__}"
+                f"Mandelbrot exponent type: [blue]{type(self.render_settings.mandelbrot_exponent).__name__}",
+                f"Burning ship exponent type: [blue]{type(self.render_settings.burning_ship_exponent).__name__}"
             ])
             return
 
-        if args[0] not in ["julia", "mandel"]:
-            self.log_write("[red]First argument must be 'julia' or 'mandel'")
+        fract = args[0]
+        wanted_type = args[1]
+
+        if fract not in ["julia", "mandel", "burning_ship"]:
+            self.log_error("[red]First argument must be 'julia', 'mandel' or 'burning_ship'")
             return
 
-        if args[1] not in ["int", "float", "mpc"]:
-            self.log_write("[red]Second argument must be 'int', 'float' or 'mpc'")
+        if wanted_type not in ["int", "float", "mpc"]:
+            self.log_error("[red]Second argument must be 'int', 'float' or 'mpc'")
             return
 
         new_value = eval(args[1])(int(2))
 
-        if args[0] == "julia":
-            self.render_settings.julia_exponent = new_value
-        else:
-            self.render_settings.mandelbrot_exponent = new_value
+        match fract:
+            case "julia":
+                self.render_settings.julia_exponent = new_value
+            case "mandel":
+                self.render_settings.mandelbrot_exponent = new_value
+            case "burning_ship":
+                self.render_settings.burning_ship_exponent = new_value
 
-        self.log_write(
-            f"{args[0].capitalize()} exponent type set to [purple]{args[1]}[/purple], "
-            "resetting the starting value to 2")
+        self.log_info(
+            f"{fract.capitalize()} exponent type set to [purple]{args[1]}[/purple] and reset to 2.")
 
         self.update_canv()
 
+    def command_fractal(self, args, argc: int) -> None:
+        if argc == 0:
+            self.log_write([
+                f"Current fractal: [blue]{self.selected_fractal.__name__}[/blue]",
+                "Available fractals: "
+                f"{', '.join([f'[violet]{fractal.__name__}[/violet]' for fractal in fractals.fractal_list])}"
+            ])
+            return
+
+        fractal_name = args[0]
+
+        fractal_index = get_fractal_index_from_name(fractal_name)
+
+        if fractal_index is None:
+            self.log_error(f"Cannot find fractal [white on red]{fractal_name}")
+            return
+
+        self.render_settings.fractal_index = fractal_index
+        self.log_success(f"Current fractal set to [blue]{self.selected_fractal.__name__}")
+        self.update_canv()
+
+    def command_help(self, args, argc: int) -> None:
+        if argc == 1:
+            if args[0] == "+":
+                command_desc = [
+                    f"- [blue]{name}[/blue]: {self.command_list[name].help}"
+                    for name in self.command_list
+                ]
+
+                self.log_write([
+                    "[on blue]Available commands",
+                    *command_desc,
+                    "[green]Use 'help command_name' to get more info about a command"
+                ])
+                return
+
+            command = self.get_command(args[0])
+            if command is None:
+                return
+
+            self.log_write([
+                f"[on blue]{args[0]} command",
+                command.help,
+                command.extra_help
+            ])
+            return
+
+        # If no args were passed
+        self.log_write([
+            "[on blue]Available commands",
+            ", ".join([f"[blue]{name}[/blue]" for name in self.command_list]),
+            "[green]Use [bold]'help +'[/bold] to get a list of all commands and a basic description. "
+            "[green]Use [bold]'help command_name'[/bold] to get more info about a command"
+        ])
+
+    def command_load_state(self, args, argc: int) -> None:
+        self.load_state(args[0])
+        self.update_canv()
+
+    def command_pos(self, args, argc: int) -> None:
+        # If no args are provided, just show the current position
+        if argc == 0:
+            self.log_info(f"Current position: [blue]{self.render_settings.screen_pos_on_plane}")
+            return
+
+        # If args are provided, go to the given x and y position
+        real = None
+        imag = None
+        try:
+            real = mpfr(args[0])
+            imag = mpfr(args[1])
+        except ValueError:
+            self.log_error("Real and imaginary parts must be valid integers or floats")
+            return
+
+        self.render_settings.screen_pos_on_plane = mpc(real, imag)
+
+        # Update canvas since we just moved
+        self.update_canv()
+
+    def command_quit(self, args, argc: int) -> None:
+        self.log_info("Quitting...")
+        self.exit()
+
+    def command_save_state(self, args, argc: int) -> None:
+        if argc == 0:
+            filename = f"{self.selected_fractal.__name__}_state_{int(time())}.fc"
+        else:
+            filename = args[0]
+
+        try:
+            with open(filename, "wb") as f:
+                state_info = StateInfo()
+                state_info.render_settings = self.render_settings
+                pickle.dump(state_info, f)
+        except OSError as e:
+            self.log_error(f"Cannot write to file '{filename}'. [red]Errno {e.errno}: {e.strerror}.")
+            return
+
+        self.log_success(f"State saved to [blue]{filename}")
+
     def command_set_exp(self, args, argc: int) -> None:
         if argc == 0:
             self.log_write([
                 f"Julia exponent: [blue]{type(self.render_settings.julia_exponent).__name__}"
                 f"({self.render_settings.julia_exponent})",
                 f"Mandelbrot exponent: [blue]{type(self.render_settings.mandelbrot_exponent).__name__}"
-                f"({self.render_settings.mandelbrot_exponent})"
+                f"({self.render_settings.mandelbrot_exponent})",
+                f"Burning ship exponent: [blue]{type(self.render_settings.burning_ship_exponent).__name__}"
+                f"({self.render_settings.burning_ship_exponent})"
             ])
             return
 
         fract = args[0]
         real = args[1]
         imag = None if argc == 2 else args[2]
 
-        if fract not in ["julia", "mandel"]:
-            self.log_write("[red]First argument must be 'julia' or 'mandel'")
+        if fract not in ["julia", "mandel", "burning_ship"]:
+            self.log_error("[red]First argument must be 'julia', 'mandel' or 'burning_ship")
             return
 
-        exp_type = type(self.render_settings.__getattribute__(
-                    "julia_exponent" if fract == "julia" else "mandelbrot_exponent"))
+        match fract:
+            case "julia":
+                exp_type = type(self.render_settings.julia_exponent)
+            case "mandel":
+                exp_type = type(self.render_settings.mandelbrot_exponent)
+            case "burning_ship":
+                exp_type = type(self.render_settings.burning_ship_exponent)
 
         try:
-            real_parsed = exp_type(real)
+            real_parsed = mpfr(real)
         except ValueError:
-            self.log_write(f"Real part must be a valid {type(self.render_settings.julia_exponent).__name__}")
+            self.log_error(f"Real part must be a valid {exp_type.__name__}")
             return
 
         # If an imag part was provided
         if exp_type is mpc:
             if imag is None:
                 self.log_write(
                     "Imaginary part is required because the exponent type is mpc. "
                     "If you don't want to use complex numbers, "
                     "change the exponent type to int or float with the [blue]exp_type[/blue] command.")
                 return
-            imag_parsed = mpc(imag)
-            self.render_settings.__setattr__(
-                "julia_exponent" if fract == "julia" else "mandelbrot_exponent",
-                mpc(real_parsed, imag_parsed))
+            imag_parsed = mpfr(imag)
+            match fract:
+                case "julia":
+                    self.render_settings.julia_exponent = mpc(real_parsed, imag_parsed)
+                case "mandel":
+                    self.render_settings.mandelbrot_exponent = mpc(real_parsed, imag_parsed)
+                case "burning_ship":
+                    self.render_settings.burning_ship_exponent = mpc(real_parsed, imag_parsed)
         else:
             if imag is not None:
-                self.log_write("Imaginary part ignored because the exponent type is not mpc")
-            # TODO: improve this sht
-            self.render_settings.__setattr__(
-                "julia_exponent" if fract == "julia" else "mandelbrot_exponent",
-                real_parsed)
+                self.log_warning("Imaginary part ignored because the exponent type is not mpc")
+            match fract:
+                case "julia":
+                    self.render_settings.julia_exponent = exp_type(real_parsed)
+                case "mandel":
+                    self.render_settings.mandelbrot_exponent = exp_type(real_parsed)
+                case "burning_ship":
+                    self.render_settings.burning_ship_exponent = exp_type(real_parsed)
         self.update_canv()
 
+    def command_version(self, args, argc: int) -> None:
+        self.log_info(f"Fractalistic version: [on blue]{__version__}")
+
     # We cant directly set command_list because we couldn't reference command methods correctly
     # Please order the commands alphabetically
     def set_command_list(self) -> None:
         self.command_list = {
             "capture": Command(
                 funct=self.command_capture,
                 help="Take a high quality screenshot",
@@ -360,29 +431,45 @@
                 help="Clear the log panel",
                 accepted_arg_counts=[0]),
             "click_mode": Command(
                 funct=self.command_click_mode,
                 help="Set the action to take when left or right clicking on the canvas.",
                 accepted_arg_counts=[0, 2],
                 extra_help=(
-                    "[green]Usage : [left/right] [mode]\nUsage : no args[/green]\n"
+                    "[green]Usage : \\[left/right] \\[mode]\nUsage : no args[/green]\n"
                     "If no argument is given, print out the current click modes and the available modes. "
                     "Else, set the left/right click action to \\[mode].")),
+            "color": Command(
+                funct=self.command_color,
+                help="List all the available color schemes or select the specified one.",
+                accepted_arg_counts=[0, 1],
+                extra_help=(
+                    "[green]Usage : \\[color]\nUsage : no args[/green]\n"
+                    "If no argument is given, print out the current color and all the available colors. "
+                    "Else, select the specified color.")),
             "exp_type": Command(
                 funct=self.command_exp_type,
                 help="Set the data type used for Julia and Mandelbrot exponents.",
                 accepted_arg_counts=[0, 2],
                 extra_help=(
-                    "[green]Usage : \\[mandel/julia] \\[int/float/mpc]\nUsage : no args[/green]\n"
+                    "[green]Usage : \\[mandel/julia/burning_ship] \\[int/float/mpc]\nUsage : no args[/green]\n"
                     "If no argument is given, print out the current types. "
                     "Else, set the mandel/julia exponent type to \\[type].\n"
                     "- It is important to use the simplest type possible because it has a huge impact on performance.\n"
                     "- \\[mpc] is the complex type from the gmpy2 library.\n"
                     "- If you change the type, the exponent value will be reset to 2.\n"
                     "- [red]Be aware that using float or mpc types will make renders much slower.")),
+            "fractal": Command(
+                funct=self.command_fractal,
+                help="List all the available fractals or select the specified one.",
+                accepted_arg_counts=[0, 1],
+                extra_help=(
+                    "[green]Usage : \\[fract name]\nUsage : no args[/green]\n"
+                    "If no argument is given, print out the available fractals. "
+                    "Else, select the specified one. The fractal name is case insensitive.")),
             "help": Command(
                 funct=self.command_help,
                 help="Show the help message",
                 accepted_arg_counts=[0, 1]),
             "load_state": Command(
                 funct=self.command_load_state,
                 help="Load a state from a file.",
@@ -428,17 +515,17 @@
                     "[green]Usage : \\[filename]\nUsage : no args[/green]\n"
                     "If no filename is specified, one will be generated automatically.")),
             "set_exp": Command(
                 funct=self.command_set_exp,
                 help="Set the julia/mandel exponent value.",
                 accepted_arg_counts=[0, 2, 3],
                 extra_help=(
-                    "[green]Usage : \\[mandel/julia] \\[real] \\[?imag]\nUsage : no args[/green]\n"
+                    "[green]Usage : \\[frac_name] \\[real] \\[?imag]\nUsage : no args[/green]\n"
                     "If no argument is given, print out the current exponent values. "
-                    "Else, set the mandel/julia exponent value to \\[real] + \\[imag]j.\n"
+                    "Else, set the exponent value to \\[real] + \\[imag]j.\n"
                     "Providing the imaginary part is only required if the exponent type is \\[mpc].")),
             "threads": CommandIncrement(
                 funct=self.command_threads,
                 help="Change the number of threads used for rendering",
                 app_attribute="settings.threads",
                 min_value=1),
             "version": Command(
@@ -452,15 +539,15 @@
                 min_value=1,
                 max_value=100),
         }
 
     # ---------- ACTIONS
     def action_cancel_screenshot(self) -> None:
         self.cancel_screenshot = True
-        self.log_write("Screenshot cancelled")
+        self.log_info("Screenshot cancelled")
 
     def action_go(self, x, y) -> None:
         if not self.ready:
             return
 
         # Remove the marker when moving
         self.remove_marker()
@@ -490,31 +577,29 @@
         if not self.ready:
             return
 
         self.render_settings.color_renderer_index = (
             (self.render_settings.color_renderer_index + 1) % len(colors.color_renderers))
 
         self.update_canv()
-        self.log_write(f"Now using the [purple]{self.selected_color.__name__}[/purple] color scheme")
+        self.log_info(f"Now using the [purple]{self.selected_color.__name__}[/purple] color scheme")
 
     def action_next_fractal(self) -> None:
         if not self.ready:
             return
 
         # Remove the marker when changing fractal
         self.remove_marker()
 
         self.render_settings.fractal_index = (self.render_settings.fractal_index + 1) % len(fractals.fractal_list)
         self.update_canv()
 
-        to_write = [f"Now viewing the [purple]{self.selected_fractal.__name__}[/purple] fractal."]
+        self.log_info(f"Now viewing the [purple]{self.selected_fractal.__name__}[/purple] fractal.")
         if self.selected_fractal.message is not None:
-            to_write.append(self.selected_fractal.message)
-
-        self.log_write(to_write)
+            self.log_info(self.selected_fractal.message)
 
     def action_screenshot(self, screenshot_size: Vec | None = None) -> None:
         if not self.ready:
             return
 
         # I dont know why this is working
         # Execute action_screenshot_2 in a non-blocking way
@@ -564,15 +649,15 @@
         # If the screenshot wasn't cancelled, save the screenshot to a file,
         # put a message in the log panel and wait one second to
         # allow the user to see that the operation is finished successfully.
         if not self.cancel_screenshot:
             save_to = f"{self.selected_fractal.__name__}_screenshot_{int(time())}.png"
             image.save(save_to)
             self.call_after_refresh(
-                self.log_write,
+                self.log_success,
                 f"Screenshot [{screenshot_width}x{screenshot_height}] saved to [on violet]{save_to}")
 
             # Wait one second to allow the user to see that the operation is finished successfully
             sleep(1)
 
         self.progress_bar.add_class("hidden")
         self.container.remove_class("hidden")
@@ -608,17 +693,19 @@
             return
 
         self.reset_position()
         self.update_canv()
 
     @on(Input.Submitted, "Input")
     def command_input_on_submitted(self, event: Input.Submitted) -> None:
+        # Get the command from the input and clear it
         command = event.value.strip()
         self.command_input.value = ""
 
+        # Ignore empty commands
         if len(command) == 0:
             return
 
         self.parse_command(command)
 
     # ---------- TEXTUAL APP VARS
 
@@ -626,14 +713,34 @@
         Binding("ctrl+c", "quit_", "Quit", priority=True)
     ]
 
     CSS_PATH = os.path.join(SRC_DIR, "app.tcss")
 
     # ---------- UTILS
 
+    def log_error(self, message: str, subject: str | None = None) -> None:
+        self.log_write([
+            f"[on red] Error{f': {subject}' if subject is not None else ''} ",
+            f"[red]{message}"])
+
+    def log_info(self, message: str, subject: str | None = None) -> None:
+        self.log_write([
+            f"[on blue] Info{f': {subject}' if subject is not None else ''} ",
+            f"[blue]{message}"])
+
+    def log_success(self, message: str, subject: str | None = None) -> None:
+        self.log_write([
+            f"[black on green] Success{f': {subject}' if subject is not None else ''} ",
+            f"[green]{message}"])
+
+    def log_warning(self, message: str, subject: str | None = None) -> None:
+        self.log_write([
+            f"[black on yellow] Warning{f': {subject}' if subject is not None else ''} ",
+            f"[yellow]{message}"])
+
     def set_marker(self, pos):
         if self.settings.marker_pos is not None:
             c_num = self.pos_to_c(self.settings.marker_pos)
             divergence = self.get_divergence(c_num)
             color = Color.parse("black") if divergence == -1 else self.selected_color(divergence)
             self.canv.set_pixel(self.settings.marker_pos.x, self.settings.marker_pos.y, color)
 
@@ -705,25 +812,25 @@
     def load_state(self, filename: str) -> None:
         try:
             with open(filename, "rb") as f:
                 try:
                     state_file: StateInfo = pickle.load(f)
                     self.settings.render_settings = state_file.render_settings
                 except Exception as e:
-                    self.log_write(
-                        f"[red]Cannot decode file '{filename}'. "
+                    self.log_error(
+                        f"Cannot decode file '{filename}'. "
                         "After version 2.0.0, the state file format changed.[/red]"
                         f"\nError: {e}")
                     return
 
         except OSError as e:
-            self.log_write(f"Cannot read file '{filename}'. [red]Errno {e.errno}: {e.strerror}.")
+            self.log_error(f"Cannot read file '{filename}'. [red]Errno {e.errno}: {e.strerror}.")
             return
 
-        self.log_write(f"State loaded from [blue]{filename}[/blue]")
+        self.log_success(f"State loaded from [blue]{filename}[/blue]")
 
     def reset_position(self) -> None:
         # remove the marker
         self.remove_marker()
 
         self.render_settings.cell_size = 4 / self.settings.canv_size.x
         self.render_settings.screen_pos_on_plane = mpc(0, 0)
@@ -737,17 +844,17 @@
         return self.settings.render_settings
 
     @precision.setter
     def precision(self, value):
         set_precision(value)
         self.render_settings.wanted_numeric_precision = value
 
-    def get_command(self, name: str) -> Command | None:
+    def get_command(self, name: str) -> Command | CommandIncrement | None:
         if name not in self.command_list:
-            self.log_write(f"[red]Cannot find command: [white on red]{name}")
+            self.log_error(f"[red]Cannot find command: [white on red]{name}")
             return None
 
         return self.command_list[name]
 
     def get_screenshot_size_fit(self, quality: int | None = None) -> Vec:
         """
         Return the size of the screenshot so that it fits the terminal
@@ -767,40 +874,67 @@
 
         return Vec(self.settings.screenshot_size.x, self.settings.screenshot_size.y)
 
     def remove_marker(self) -> None:
         self.settings.marker_pos = None
 
     def parse_command(self, text: str) -> None:
+        """All executed commands are sent directly here."""
+
+        # Extract non-empty arguments, including the command name
         args = list(filter(lambda x: len(x) > 0, text.split(" ")))
 
         command_name = args.pop(0)
+
+        # Returns none if the command is not found
+        # Else, returns Command() or CommandIncrement()
         command = self.get_command(command_name)
 
+        # Error message in case the command is not found
+        # is handled by get_command
         if command is None:
             return
 
+        # Check if the number of arguments is accepted by the command
         if not len(args) in command.accepted_arg_count:
-            self.log_write(
-                f"[red]Command [white on red]{command_name}[/white on red] expects "
-                f"{', or '.join([str(x) for x in command.accepted_arg_count])} arguments, got {len(args)}")
+            self.log_error(
+                f"Command [white on red]{command_name}[/white on red] expects "
+                f"{', or '.join([str(x) for x in command.accepted_arg_count])} arguments, but got {len(args)}")
 
             return
 
+        # CommandIncrement() is a special case
+        # Else we just call the command with the arguments.
         if isinstance(command, CommandIncrement):
+
+            # app_attribute example : "settings.render_settings.max_iter"
+            # means that the command will increment (self).settings.render_settings.max_iter
+            ############################################################
+            # "attributes": ["settings", "render_settings", "max_iter"]
+            # we recursively go through the path to get the wanted attribute's value
             attributes = command.app_attribute.split(".")
             current_attribute_value = self
             for attribute in attributes:
                 current_attribute_value = current_attribute_value.__getattribute__(attribute)
 
+            # If no args are provided, just print the current value here
+            if len(args) == 0:
+                self.log_info(f"The value is currently set to [blue]{current_attribute_value}")
+                return
+
+            # We pass the args and the current attribute value to CommandIncrement().parse_args()
             value: CommandIncrementArgParseResult = command.parse_args(current_attribute_value, args)
             if value.success:
+                # If the new value was successfully parsed, we call the command's funct
+                # which role is to set the new value, notice the user,
+                # and update the canvas according to the new value, if needed.
                 command.funct(value.new_value)
             else:
-                self.log_write(value.error_message)
+                # If the new value was not successfully parsed, we log the error message
+                self.log_error(value.error_message)
                 return
         else:
             command.funct(args, len(args))
 
     @property
     def selected_fractal(self) -> FractalBase:
         return fractals.fractal_list[self.render_settings.fractal_index]
@@ -984,34 +1118,39 @@
                     f"Clicked at (pos): {self.settings.marker_pos}",
                     f"Divergence: {divergence}",
                 ])
             case "julia":
                 # Hide the marker since the fractal has changed
                 self.remove_marker()
                 self.render_settings.julia_click = c_num
-                self.log_write([
-                    "[on red] Current Julia Set ",
-                    f"{self.render_settings.julia_click:.4f}",
-                ])
+                self.log_info(
+                    "Current Julia Set:\n"
+                    f"{self.render_settings.julia_click:.4f}")
                 self.update_canv()
             case "move":
                 self.render_settings.screen_pos_on_plane = c_num
                 self.update_canv()
             case "zoom_in":
                 self.zoom_at_pos(click_pos, "in")
                 self.update_canv()
             case "zoom_out":
                 self.zoom_at_pos(click_pos, "out")
                 self.update_canv()
             case "mb_start":
                 self.render_settings.mandelbrot_starting_value = c_num
-                self.log_write([
-                    "[on red] Current Mandelbrot Set starting value ",
-                    f"{self.render_settings.mandelbrot_starting_value:.4f}",
-                ])
+                self.log_info(
+                    "Current Mandelbrot Set starting value:\n"
+                    f"{self.render_settings.mandelbrot_starting_value:.4f}")
+                self.update_canv()
+            case "inv_mb_num":
+                self.render_settings.inv_mandel_numerator = c_num
+                self.log_info(
+                    "Current Inverse Mandelbrot Set numerator:\n"
+                    f"{self.render_settings.inv_mandel_numerator:.4f}")
+
                 self.update_canv()
 
     def compose(self):
         # Mount the footer and a progress bar
         yield Footer()
         yield self.progress_bar
```

### Comparing `fractalistic-2.0.0/fractalistic/colors.py` & `fractalistic-2.1.0/fractalistic/colors.py`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/fractalistic/command.py` & `fractalistic-2.1.0/fractalistic/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,21 +39,20 @@
             accepted_arg_counts=[0, 1, 2]
         )
         self.max_value = max_value
         self.min_value = min_value
         self.app_attribute = app_attribute
 
     def parse_args(self, current_attrib_value, args) -> CommandIncrementArgParseResult:
-        """Returns the new value if the args are valid, else None"""
+        """Returns the new attribute value if the args are valid, else None"""
         result = CommandIncrementArgParseResult()
-        if len(args) == 0:
-            result.error_message = f"The value is currently set to [blue]{current_attrib_value}"
-            return result
 
-        elif len(args) == 1:
+        # len(args) == 0 is handled by app.py:parse_command
+
+        if len(args) == 1:
             try:
                 result.new_value = int(args[0])
             except ValueError:
                 result.error_message = "[red]The value must be an integer"
                 return result
 
         elif len(args) == 2:
```

### Comparing `fractalistic-2.0.0/fractalistic/fractal_canv.py` & `fractalistic-2.1.0/fractalistic/fractal_canv.py`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/fractalistic/fractals/burning_ship.py` & `fractalistic-2.1.0/fractalistic/fractals/mandelbrot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from .fractal_base import FractalBase
 from gmpy2 import mpc
 from ..settings import RenderSettings
+from .fractal_base import FractalBase
 
 
-class BurningShip(FractalBase):
+class Mandelbrot(FractalBase):
     """
     With U0 = 0 and c being the point in the complex plane,
-    Un+1 = (|Re(Un)| + i|Im(Un)|)² + c
+    Un+1 = Un² + c
     """
-
     message = None
 
     @staticmethod
     def get(point: mpc, settings: RenderSettings) -> int:
         i = 0
-        z = mpc(0, 0)
-        while abs(z) < 5 and i < settings.max_iter:
-            z = mpc(abs(z.real), abs(z.imag))
-            z = z*z - point
+        z = settings.mandelbrot_starting_value
+        while abs(z) < 2 and i < settings.max_iter:
+            z = z.__pow__(settings.mandelbrot_exponent) + point
             i += 1
 
         if i == settings.max_iter:
             return -1
 
         return i
```

### Comparing `fractalistic-2.0.0/fractalistic/fractals/julia.py` & `fractalistic-2.1.0/fractalistic/fractals/julia.py`

 * *Files identical despite different names*

### Comparing `fractalistic-2.0.0/fractalistic/fractals/mandelbrot.py` & `fractalistic-2.1.0/fractalistic/fractals/inv_mandel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from gmpy2 import mpc
 from ..settings import RenderSettings
 from .fractal_base import FractalBase
 
 
-class Mandelbrot(FractalBase):
+class InverseMandelbrot(FractalBase):
     """
     With U0 = 0 and c being the point in the complex plane,
-    Un+1 = Un² + c
+    Un+1 = b/(Un² + c)
     """
-    message = None
+    message = "The inverse mandelbrot uses your configured mandelbrot values."
 
     @staticmethod
     def get(point: mpc, settings: RenderSettings) -> int:
         i = 0
         z = settings.mandelbrot_starting_value
         while abs(z) < 2 and i < settings.max_iter:
-            z = z.__pow__(settings.mandelbrot_exponent) + point
+            z = settings.inv_mandel_numerator/(z.__pow__(settings.mandelbrot_exponent) + point)
             i += 1
 
         if i == settings.max_iter:
             return -1
 
         return i
```

### Comparing `fractalistic-2.0.0/fractalistic/settings.py` & `fractalistic-2.1.0/fractalistic/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,24 @@
     """
 
     mandelbrot_exponent: float | int | mpc = int(2)
     """-> P in the mandelbrot formula:
     Un+1 = (Un)^p + C
     """
 
+    burning_ship_exponent: float | int | mpc = int(2)
+    """-> P in the burning ship formula:
+    Un+1 = (|Re(Un)| + i|Im(Un)|)^p + C
+    """
+
+    inv_mandel_numerator: mpc = mpc(1, 0)
+    """-> b in the inverse mandelbrot formula:
+    Un+1 = b/(Un² + C)
+    """
+
     color_renderer_index: int = 0
     """Index of the current color renderer"""
 
     wanted_numeric_precision: int = 64
     """The wanted numeric precision"""
 
     max_iter: int = 128
```

### Comparing `fractalistic-2.0.0/fractalistic/utils.py` & `fractalistic-2.1.0/fractalistic/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,25 @@
 from gmpy2 import mpc
 import gmpy2
 
 SRC_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_fractal_index_from_name(name: str):
-    return {frac.__name__: i for i, frac in enumerate(fractal_list)}[name]
+    try:
+        return {frac.__name__.lower(): i for i, frac in enumerate(fractal_list)}[name.lower()]
+    except KeyError:
+        return None
 
 
 def get_color_index_from_name(name: str):
-    return {color.__name__: i for i, color in enumerate(color_renderers)}[name]
+    try:
+        return {color.__name__.lower(): i for i, color in enumerate(color_renderers)}[name.lower()]
+    except KeyError:
+        return None
 
 
 def pos_to_c(pos: Vec, cell_size, screen_pos_on_plane, screen_size) -> mpc:
     """Takes a position (x, y) of the canvas and converts it into the corresponding complex number on the plane"""
     result_real = (pos.x - screen_size.x//2) * cell_size
     result_imag = (pos.y - screen_size.y//2) * -cell_size
     result = mpc(result_real, result_imag) + screen_pos_on_plane
```

### Comparing `fractalistic-2.0.0/pyproject.toml` & `fractalistic-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 dynamic = ["version", "description"]
 
 
 dependencies = [
     "textual==0.38.1",
     "click_extra==4.7.1",
     "gmpy2==2.1.5",
-    "pillow==10.0.1",
+    "pillow==10.3.0",
     "asyncio==3.4.3",
     "textual_canvas==0.2.0"
 ]
 
 [project.urls]
 Repository = "https://github.com/SkwalExe/fractalistic"
 Changelog = "https://github.com/SkwalExe/fractalistic/blob/main/CHANGELOG.md"
```

### Comparing `fractalistic-2.0.0/PKG-INFO` & `fractalistic-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fractalistic
-Version: 2.0.0
+Version: 2.1.0
 Summary: Terminal based fractal explorer, including Mandelbrot, Burning Ship, and Julia.
 Author-email: Leopold Koprivnik <skwal@etik.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: textual==0.38.1
 Requires-Dist: click_extra==4.7.1
 Requires-Dist: gmpy2==2.1.5
-Requires-Dist: pillow==10.0.1
+Requires-Dist: pillow==10.3.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: textual_canvas==0.2.0
 Project-URL: Changelog, https://github.com/SkwalExe/fractalistic/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/SkwalExe/fractalistic
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/SkwalExe/fractalistic/main/assets/logo.png">
@@ -74,15 +74,14 @@
 - 📌 Click to show coordinates and divergence
 - 🏃 Multithreaded rendering
 
 # Roadmap
 
 Possible features to add later:
 - [ ] Splash screen
-- [ ] app.log_error(), etc utility functions
 - [ ] New mandelbrot variants
 
 Commands:
 - [ ] Command to show current pos, zoom, etc
 
 # How to migrate your state files to >= 2.0.0
```

