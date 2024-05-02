# Comparing `tmp/gflabel-0.1.0.tar.gz` & `tmp/gflabel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gflabel-0.1.0.tar", max compression
+gzip compressed data, was "gflabel-0.1.1.tar", max compression
```

## Comparing `gflabel-0.1.0.tar` & `gflabel-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1456 2024-04-20 08:14:56.041235 gflabel-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     9288 2024-05-01 21:51:31.955586 gflabel-0.1.0/README.md
--rw-r--r--   0        0        0      813 2024-05-01 21:40:46.468572 gflabel-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-21 22:42:35.484373 gflabel-0.1.0/src/gflabel/__init__.py
--rw-r--r--   0        0        0      220 2024-04-22 22:00:53.788778 gflabel-0.1.0/src/gflabel/bases/__init__.py
--rw-r--r--   0        0        0     1369 2024-04-27 16:00:00.308412 gflabel-0.1.0/src/gflabel/bases/plain.py
--rw-r--r--   0        0        0     3265 2024-04-26 22:29:12.537814 gflabel-0.1.0/src/gflabel/bases/pred.py
--rw-r--r--   0        0        0     1409 2024-04-28 22:29:28.240393 gflabel-0.1.0/src/gflabel/bases/webb.py
--rwxr-xr-x   0        0        0     9375 2024-05-01 20:09:53.146528 gflabel-0.1.0/src/gflabel/cli.py
--rw-r--r--   0        0        0    31515 2024-05-01 20:45:20.620929 gflabel-0.1.0/src/gflabel/fragments.py
--rw-r--r--   0        0        0     7517 2024-05-01 20:03:07.620110 gflabel-0.1.0/src/gflabel/label.py
--rw-r--r--   0        0        0     1381 2024-04-27 17:06:38.364896 gflabel-0.1.0/src/gflabel/options.py
--rw-r--r--   0        0        0     9835 1970-01-01 00:00:00.000000 gflabel-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-05-02 21:24:36.673408 gflabel-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     9925 2024-05-02 21:24:36.673408 gflabel-0.1.1/README.md
+-rw-r--r--   0        0        0      813 2024-05-02 21:24:36.677408 gflabel-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/bases/__init__.py
+-rw-r--r--   0        0        0     1369 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/bases/plain.py
+-rw-r--r--   0        0        0     3265 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/bases/pred.py
+-rw-r--r--   0        0        0     1409 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/bases/webb.py
+-rwxr-xr-x   0        0        0     9625 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/cli.py
+-rw-r--r--   0        0        0    30310 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/fragments.py
+-rw-r--r--   0        0        0     8880 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/label.py
+-rw-r--r--   0        0        0     1637 2024-05-02 21:24:36.677408 gflabel-0.1.1/src/gflabel/options.py
+-rw-r--r--   0        0        0    10472 1970-01-01 00:00:00.000000 gflabel-0.1.1/PKG-INFO
```

### Comparing `gflabel-0.1.0/LICENSE.txt` & `gflabel-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.0/README.md` & `gflabel-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [build123d]: https://github.com/gumyr/build123d
 
 ## State
 
 This is an early version of a hobby project. Thus:
 
 - It has a lot of rough edges, not the least that the output is messy and
-  not very useful.
+  not very useful. But functionality not used much might not work well.
 - It sometimes needs manual encouragement to make labels looking good or
   consistent.
 - A habit of sometimes crashing OCP when geometry is a little bit odd.
 
 
 ## Usage
 
@@ -27,21 +27,33 @@
 You should be able to install into your favorite python-virtual-environment
 manager by just using pip:
 
 ```
 pip install gflabel
 ```
 
-This should work on most platforms, but for specifically macOS arm64, the
-underlying cadquery-ocp library is not available as a wheel through pypi.
-In this case, you will have to set up the build123d environment manually.
-build123d has [some notes][install_build123d] on resolving this conflict.
+This should work on most modern platforms, but with the following caveats:
+
+- Linux wheels for the dependency cadquery-ocp are only available on
+  resonably modern (e.g. Ubuntu 22.4+) linux distributions, so you may have to
+  go to conda to install on an older machine.
+- For specifically macOS arm64, the underlying cadquery-ocp library is not
+  available as a wheel through pypi. In this case, you will have to set up the
+  build123d environment manually. build123d has [some notes][install_build123d]
+  on resolving this conflict.
 
 [install_build123d]: https://build123d.readthedocs.io/en/latest/installation.html#special-notes-on-apple-silicon-installs
 
+Otherwise, you can check out this repository and `pip install` it directly, or
+install directly from the github repo:
+
+```
+pip install git+https://github.com/ndevenish/gflabel.git
+```
+
 ### Basic Examples
 
 By default, labels are written to an output file "`label.step`". You can change
 this with `-o FILENAME`. `.step`, `.stl` and `.svg` are recognised
 
 A simple, single label generation on a pred-style base:
 
@@ -73,19 +85,26 @@
 specified as  20mm):
 ```
 gflabel "{head(hex)} {bolt(20)}\nM2×20"
 ```
 ![](images/example_boltbin.png)
 
 Some symbols can also take many modifiers for e.g. drive or head type:
+
 ```
 gflabel "{head(+)} {bolt(50,slotted,round)}\nM3×50"
 ```
 ![](images/example_bolt_broken.png)
 
+And multiple label styles/symbol styles/fonts can be selected:
+```
+gflabel --base=webb --font=Arial "M3×20{...}{webbolt(+)}"
+```
+![](images/example_webb.png)
+
 ## Command Parameters
 
 Core command parameters (call `gflabel --help` for the full list):
 
 ```
 usage: gflabel [options] LABEL [LABEL ...]
 
@@ -151,15 +170,15 @@
 | Names             | Description                                                       |
 |-------------------|-------------------------------------------------------------------|
 | ...               | Blank area that always expands to fill available space.<br><br>If specified multiple times, the areas will be balanced between<br>entries. This can be used to justify/align text. |
 | &lt;number&gt;    | A gap of specific width, in mm.                                   |
 | bolt              | Variable length bolt, in the style of Printables pred-box labels.<br><br>If the requested bolt is longer than the available space, then the<br>bolt will be as large as possible with a broken thread. |
 | box               | Arbitrary width, height centered box. If height is not specified, will expand to row height. |
 | head              | Screw head with specifiable head-shape.                           |
-| hexhead           | Circular screw head with a hexagonal drive. Same as 'head(hex)'.  |
+| hexhead           | Hexagonal screw head. Will accept drives, but not compulsory.     |
 | hexnut, nut       | Hexagonal outer profile nut with circular cutout.                 |
 | threaded_insert   | Representation of a threaded insert.                              |
 | variable_resistor | Electrical symbol of a variable resistor.                         |
 | washer            | Circular washer with a circular hole.                             |
 | webbolt           | Alternate bolt representation incorporating screw drive, with fixed length. |
 
 A basic set of examples showing the usage of some of these:
```

### Comparing `gflabel-0.1.0/pyproject.toml` & `gflabel-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gflabel"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Nicholas Devenish <ndevenish@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -24,15 +24,15 @@
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpversion]
-current_version = "0.1.0"
+current_version = "0.1.1"
 tag = true
 tag_name = "v{new_version}"
 commit = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
```

### Comparing `gflabel-0.1.0/src/gflabel/bases/plain.py` & `gflabel-0.1.1/src/gflabel/bases/plain.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.0/src/gflabel/bases/pred.py` & `gflabel-0.1.1/src/gflabel/bases/pred.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.0/src/gflabel/bases/webb.py` & `gflabel-0.1.1/src/gflabel/bases/webb.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.0/src/gflabel/cli.py` & `gflabel-0.1.1/src/gflabel/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,19 @@
     parser.add_argument(
         "--depth",
         help="How high (or deep) the label extrusion is.",
         metavar="DEPTH_MM",
         default=0.4,
         type=float,
     )
+    parser.add_argument(
+        "--no-overheight",
+        help="Disable the 'Overheight' system. This allows some symbols to oversize, meaning that the rest of the line will first shrink before they are shrunk.",
+        action="store_true",
+    )
 
     parser.add_argument(
         "labels", nargs="*" if "--vscode" in sys.argv else "+", metavar="LABEL"
     )
     parser.add_argument(
         "-d",
         "--divisions",
```

### Comparing `gflabel-0.1.0/src/gflabel/fragments.py` & `gflabel-0.1.1/src/gflabel/fragments.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import functools
 import logging
 import re
 import textwrap
 from abc import ABCMeta, abstractmethod
 from collections.abc import Callable
-from math import cos, pi, radians, sin, tan
+from math import cos, radians, sin
 from typing import Any, Iterable, NamedTuple, Type
 
 from build123d import (
     Align,
     Axis,
     BuildLine,
     BuildSketch,
@@ -32,14 +32,15 @@
     Text,
     Triangle,
     Vector,
     add,
     fillet,
     make_face,
     mirror,
+    offset,
 )
 
 from .options import RenderOptions
 
 logger = logging.getLogger(__name__)
 RE_FRAGMENT = re.compile(r"(.+?)(?:\((.*)\))?$")
 
@@ -84,15 +85,15 @@
     args = [x.strip() for x in args.split(",")] if args else []
 
     if name not in FRAGMENTS:
         raise RuntimeError(f"Unknown fragment class: {name}")
     return FRAGMENTS[name](*args)
 
 
-def fragment(*names: str, examples: list[str] = []):
+def fragment(*names: str, examples: list[str] = [], overheight: float | None = None):
     """Register a label fragment generator"""
 
     def _wrapped(
         fn: Type[Fragment] | Callable[[float, float], Sketch],
     ) -> Type[Fragment] | Callable[[float, float], Sketch]:
         if not isinstance(fn, type) and callable(fn):
             logger.debug(f"Wrapping fragment function {fn}")
@@ -100,19 +101,23 @@
             # We can have callable functions
             # class FnWrapper(Fragment):
             #     def render(
             #         self, height: float, maxsize: float, options: Any
             #     ) -> Sketch:
             #         return orig_fn(height, maxsize)
             def fragment(*args):
-                return FunctionalFragment(fn, *args)
+                frag = FunctionalFragment(fn, *args)
+                frag.overheight = overheight
+                frag.examples = examples
+                return frag
 
             # fragment = lambda *args: FunctionalFragment(fn, *args)
             fragment.__doc__ = fn.__doc__
             setattr(fragment, "examples", examples)
+            setattr(fragment, "overheight", overheight)
         else:
             fragment = fn
         # Now assign this in the name dict
         for name in names:
             logger.debug(f"Registering fragment {name}")
             FRAGMENTS[name] = fragment
         return fn
@@ -130,14 +135,20 @@
     # If this fragment is visible. If not visible, rendered sketch will
     # indicate bounding box only, but should never be added.
     visible = True
 
     # An example, or list of examples, demonstrating the fragment.
     examples: list[str] | None = None
 
+    # Fragments are allowed to go overheight, in which case the entire
+    # label is scaled down to fit. If this is set then the working area
+    # will preemptively be scaled to compensate, avoiding a double-round
+    # of resizing.
+    overheight: float | None = None
+
     def __init__(self, *args: list[Any]):
         if args:
             raise ValueError("Not all fragment arguments handled")
 
     # If this fragment is variable, what's the smallest it can go?
     def min_width(self, height: float) -> float:
         """If this fragment is variable, what's the smallest it can go?"""
@@ -257,21 +268,24 @@
 
     def render(self, height: float, maxsize: float, options: RenderOptions) -> Sketch:
         with BuildSketch() as sketch:
             Rectangle(_whitespace_width(self.whitespace, height, options), height)
         return sketch.sketch
 
 
-@fragment("hexhead")
-def _fragment_hexhead(height: float, _maxsize: float) -> Sketch:
-    """Circular screw head with a hexagonal drive. Same as 'head(hex)'."""
+@fragment("hexhead", examples=["{hexhead}"])
+def _fragment_hexhead(height: float, _maxsize: float, *drives: str) -> Sketch:
+    """Hexagonal screw head. Will accept drives, but not compulsory."""
     with BuildSketch(mode=Mode.PRIVATE) as sketch:
-        Circle(height / 2)
-        add(drive_shape("hex").scale(height * 0.6), mode=Mode.SUBTRACT)
-        # RegularPolygon(height / 2 * 0.6, side_count=6, mode=Mode.SUBTRACT)
+        RegularPolygon(height / 2, 6)
+        if drives:
+            add(
+                compound_drive_shape(drives, 0.6 * height / 2, height / 2),
+                mode=Mode.SUBTRACT,
+            )
     return sketch.sketch
 
 
 @fragment("head")
 def _fragment_head(height: float, _maxsize: float, *headshapes: str) -> Sketch:
     """Screw head with specifiable head-shape."""
     with BuildSketch(mode=Mode.PRIVATE) as sketch:
@@ -541,37 +555,18 @@
 
 @fragment("webbolt")
 class WebbBoltFragment(BoltBase):
     """
     Alternate bolt representation incorporating screw drive, with fixed length.
     """
 
-    # def __init__(self, *features: str):
-    #     super().__init__(*features)
-    # alias_mapping = {
-    #     "countersink": "countersunk",
-    #     "tap": "tapping",
-    #     "tapped": "tapping",
-    # }
-    # # Map aliases to canonical names
-    # feats = [x.lower() for x in features]
-    # feats = [alias_mapping[x] if x in alias_mapping else x for x in feats]
-    # # A list of all modifier options that aren't heads
-    # mods = {"tapping", "flip"}
-    # headshapes = {"countersunk", "pan", "round", "socket"}
-
-    # self.drives = set(features) - mods - headshapes
-    # self.features = set(features) & mods
-
-    # headshapes = set(features) & headshapes
-    # if len(headshapes) > 1:
-    #     raise ValueError("Cannot specify multiple head shapes")
-    # self.headshape = next(iter(headshapes), "pan")
+    overheight = 1.6
 
     def render(self, height: float, maxsize: float, options: RenderOptions) -> Sketch:
+        height *= self.overheight
         # 12 mm high for 15 mm wide. Scale to this.
         width = 15 / 12 * height
         # Relative proportion of body:head
         body_w = width / 2
         # How many threads to have on the body
         n_threads = 6
         # How deep each thread profile should be
@@ -682,25 +677,25 @@
 
         if "flip" in self.modifiers:
             return sketch.sketch.scale(-1)
 
         return sketch.sketch
 
 
-@fragment("variable_resistor", examples=["{variable_resistor}"])
+@fragment("variable_resistor", examples=["{variable_resistor}"], overheight=1.5)
 def _fragment_variable_resistor(height: float, maxsize: float) -> Sketch:
     """Electrical symbol of a variable resistor."""
-    # symb = import_svg("symbols/variable_resistor.svg")
-    t = 0.4 / 2
-    w = 6.5
-    h = 2
+    t = 0.4 / 2  # Line half-thickness. Lines are offset by this.
+    w = 6.5  # Width of resistor
+    h = 2  # Height of resistor
+    l_arr = 7  # Arrow length
+    l_head = 1.5  # Arrow head length
+    angle = 30  # Angle of Arrow
+
     with BuildSketch(mode=Mode.PRIVATE) as sketch:
-        # add(symb)
-        # Circle(1)
-        # sweep(symb)
         with BuildLine():
             Polyline(
                 [
                     (-6, 0),
                     (-6, t),
                     (-w / 2 - t, t),
                     (-w / 2 - t, h / 2 + t),
@@ -711,62 +706,32 @@
                 ],
                 close=True,
             )
         make_face()
         mirror(sketch.sketch, Plane.XZ)
         mirror(sketch.sketch, Plane.YZ)
 
-        # with BuildLine():
-        l_arr = 7
-        l_head = 1.5
-        angle = 30
-
         theta = radians(angle)
-        oh = t / tan(theta) + t / sin(theta)
-        sigma = pi / 2 - theta
-        l_short = t / cos(sigma)
-        #     l_arrow = 1.5
-        #     angle = 30
-        #     # Work out the intersect height
-        #     h_i = t / math.sin(math.radians(angle))
-        #     arr_bottom_lost = t / math.tan(math.radians(angle))
-        arrow_parts = [
-            (0, -l_arr / 2),
-            (-t, -l_arr / 2),
-            (-t, l_arr / 2 - oh),
-            (
-                -t - sin(theta) * (l_head - l_short),
-                l_arr / 2 - oh - cos(theta) * (l_head - l_short),
-            ),
-            (-sin(theta) * l_head, l_arr / 2 - cos(theta) * l_head),
-            (0, l_arr / 2),
-            # (0, -l_arr / 2),
-        ]
         with BuildSketch(mode=Mode.PRIVATE) as arrow:
-            with BuildLine() as line:
+            with BuildLine() as _line:
                 Polyline(
-                    arrow_parts,
-                    # close=True,
+                    [
+                        (0, -l_arr / 2),
+                        (0, l_arr / 2),
+                        (-sin(theta) * l_head, l_arr / 2 - cos(theta) * l_head),
+                    ]
                 )
-                mirror(line.line, Plane.YZ)
+                offset(amount=t)
             make_face()
+            mirror(arrow.sketch, Plane.YZ)
         add(arrow.sketch.rotate(Axis.Z, -30))
-        # sketch.sketch.rotate(Axis.Z, 20)
-        # with BuildLine() as line:
-        #     Line([(0, -arr_h / 2), (0, arr_h / 2)])
-        # Arrow(arr_h, line, t * 2, head_at_start=False)
-        # mirror(line.line, Plane.XZ)
-        # mirror(line.line, Plane.YZ)
-        # offset(symb, amount=1)
-        # add(symb)
-    # Scale to fit in our height, unless this would take us over width
+
+    # Scale to fit in our height
     size = sketch.sketch.bounding_box().size
-    scale = height / size.Y
-    # actual_w = min(scale * size.X, maxsize)
-    # scale = actual_w / size.X
+    scale = (height * 1.5) / size.Y
 
     return sketch.sketch.scale(scale)
 
 
 def drive_shape(shape: str, radius: float = 1, outer_radius: float = 1) -> Sketch:
     """
     Returns a shape representing a particular screw head.
```

### Comparing `gflabel-0.1.0/src/gflabel/label.py` & `gflabel-0.1.1/src/gflabel/label.py`

 * *Files 27% similar despite different names*

```diff
@@ -88,15 +88,21 @@
                 render_y = (
                     area.Y / 2
                     - (row_height + self.opts.line_spacing_mm) * n
                     - row_height / 2
                 )
                 print(f"Rendering line {n} ({line}) at {render_y})")
                 with Locations([(0, render_y)]):
-                    add(self._render_single_line(line, Vector(X=area.X, Y=row_height)))
+                    add(
+                        self._render_single_line(
+                            line,
+                            Vector(X=area.X, Y=row_height),
+                            self.opts.allow_overheight,
+                        )
+                    )
 
         scale_to_maxwidth = area.X / sketch.sketch.bounding_box().size.X
         scale_to_maxheight = area.Y / sketch.sketch.bounding_box().size.Y
         if scale_to_maxheight < 1:
             print(
                 f"Vertical scale is too high for area ({scale_to_maxheight}); downscaling"
             )
@@ -130,27 +136,45 @@
             return second_try
         print(
             f'Entry "{spec}" calculated width = {sketch.sketch.bounding_box().size.X:.1f} (max {area.X})'
         )
 
         return sketch.sketch
 
-    def _render_single_line(self, line: str, area: Vector) -> Sketch:
+    def _render_single_line(
+        self, line: str, area: Vector, allow_overheight: bool
+    ) -> Sketch:
         """
         Render a single line of a labelspec.
         """
         # Firstly, split the line into a set of fragment objects
         frags = _spec_to_fragments(line)
 
-        rendered: dict[fragments.Fragment, Sketch]
-        rendered = {
-            f: f.render(area.Y, area.X, self.opts)
-            for f in frags
-            if not f.variable_width
-        }
+        # Overheight fragments: Work out if we have any, so that we can
+        # scale the total height such that they fit.
+        # If this isn't turned on, then we will still allow the fragment
+        # to be overheight but it will be given a smaller vertical area
+        # such that the overheight fits in the line.
+        options = self.opts._replace(allow_overheight=allow_overheight)
+        Y_available = area.Y
+        if allow_overheight:
+            max_overheight = max(x.overheight or 1 for x in frags)
+            if max_overheight > 1:
+                Y_available /= max_overheight
+                print(
+                    f"Scaling Y area to account for overheight from {area.Y:.2f} -> {Y_available:.2f}"
+                )
+
+        rendered: dict[fragments.Fragment, Sketch] = {}
+        for frag in [x for x in frags if not x.variable_width]:
+            # Handle overheight if we have overheight turned off
+            frag_available_y = Y_available / (
+                1 if allow_overheight else (frag.overheight or 1)
+            )
+            rendered[frag] = frag.render(frag_available_y, area.X, self.opts)
 
         # Work out what we have left to give to the variable labels
         remaining_area = area.X - sum(
             x.bounding_box().size.X for x in rendered.values()
         )
         count_variable = len(frags) - len(rendered)
 
@@ -158,18 +182,22 @@
         # For now, very dumb algorithm: Each variable fragment gets w/N.
         # but we recalculate after each render.
         for frag in sorted(
             [x for x in frags if x.variable_width],
             key=lambda x: x.priority,
             reverse=True,
         ):
+            # Handle overheight if we have overheight turned off
+            frag_available_y = Y_available / (
+                1 if allow_overheight else (frag.overheight or 1)
+            )
             render = frag.render(
-                area.Y,
+                frag_available_y,
                 max(remaining_area / count_variable, frag.min_width(area.Y)),
-                self.opts,
+                options,
             )
             rendered[frag] = render
             count_variable -= 1
             remaining_area -= render.bounding_box().size.X
 
         # Calculate the total width
         total_width = sum(x.bounding_box().size.X for x in rendered.values())
```

### Comparing `gflabel-0.1.0/src/gflabel/options.py` & `gflabel-0.1.1/src/gflabel/options.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,21 +31,26 @@
     font_height_mm: float | None = None
 
 
 class RenderOptions(NamedTuple):
     line_spacing_mm: float = 0.1
     margin_mm: float = 0.4
     font: FontOptions = FontOptions()
+    # Overheight fragments cause the entire line to be scaled down in
+    # height so that they can fit. Is this allowed, or will they scale
+    # like everything else?
+    allow_overheight: bool = True
 
     @classmethod
     def from_args(cls, args: argparse.Namespace) -> RenderOptions:
         font_style = [
             x for x in FontStyle if x.name.lower() == args.font_style.lower()
         ][0]
         return cls(
             margin_mm=args.margin,
             font=FontOptions(
                 font=args.font,
                 font_style=font_style,
                 font_height_mm=args.font_size,
             ),
+            allow_overheight=not args.no_overheight,
         )
```

### Comparing `gflabel-0.1.0/PKG-INFO` & `gflabel-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gflabel
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: BSD-3-Clause
 Author: Nicholas Devenish
 Author-email: ndevenish@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 [build123d]: https://github.com/gumyr/build123d
 
 ## State
 
 This is an early version of a hobby project. Thus:
 
 - It has a lot of rough edges, not the least that the output is messy and
-  not very useful.
+  not very useful. But functionality not used much might not work well.
 - It sometimes needs manual encouragement to make labels looking good or
   consistent.
 - A habit of sometimes crashing OCP when geometry is a little bit odd.
 
 
 ## Usage
 
@@ -44,21 +44,33 @@
 You should be able to install into your favorite python-virtual-environment
 manager by just using pip:
 
 ```
 pip install gflabel
 ```
 
-This should work on most platforms, but for specifically macOS arm64, the
-underlying cadquery-ocp library is not available as a wheel through pypi.
-In this case, you will have to set up the build123d environment manually.
-build123d has [some notes][install_build123d] on resolving this conflict.
+This should work on most modern platforms, but with the following caveats:
+
+- Linux wheels for the dependency cadquery-ocp are only available on
+  resonably modern (e.g. Ubuntu 22.4+) linux distributions, so you may have to
+  go to conda to install on an older machine.
+- For specifically macOS arm64, the underlying cadquery-ocp library is not
+  available as a wheel through pypi. In this case, you will have to set up the
+  build123d environment manually. build123d has [some notes][install_build123d]
+  on resolving this conflict.
 
 [install_build123d]: https://build123d.readthedocs.io/en/latest/installation.html#special-notes-on-apple-silicon-installs
 
+Otherwise, you can check out this repository and `pip install` it directly, or
+install directly from the github repo:
+
+```
+pip install git+https://github.com/ndevenish/gflabel.git
+```
+
 ### Basic Examples
 
 By default, labels are written to an output file "`label.step`". You can change
 this with `-o FILENAME`. `.step`, `.stl` and `.svg` are recognised
 
 A simple, single label generation on a pred-style base:
 
@@ -90,19 +102,26 @@
 specified as  20mm):
 ```
 gflabel "{head(hex)} {bolt(20)}\nM2×20"
 ```
 ![](images/example_boltbin.png)
 
 Some symbols can also take many modifiers for e.g. drive or head type:
+
 ```
 gflabel "{head(+)} {bolt(50,slotted,round)}\nM3×50"
 ```
 ![](images/example_bolt_broken.png)
 
+And multiple label styles/symbol styles/fonts can be selected:
+```
+gflabel --base=webb --font=Arial "M3×20{...}{webbolt(+)}"
+```
+![](images/example_webb.png)
+
 ## Command Parameters
 
 Core command parameters (call `gflabel --help` for the full list):
 
 ```
 usage: gflabel [options] LABEL [LABEL ...]
 
@@ -168,15 +187,15 @@
 | Names             | Description                                                       |
 |-------------------|-------------------------------------------------------------------|
 | ...               | Blank area that always expands to fill available space.<br><br>If specified multiple times, the areas will be balanced between<br>entries. This can be used to justify/align text. |
 | &lt;number&gt;    | A gap of specific width, in mm.                                   |
 | bolt              | Variable length bolt, in the style of Printables pred-box labels.<br><br>If the requested bolt is longer than the available space, then the<br>bolt will be as large as possible with a broken thread. |
 | box               | Arbitrary width, height centered box. If height is not specified, will expand to row height. |
 | head              | Screw head with specifiable head-shape.                           |
-| hexhead           | Circular screw head with a hexagonal drive. Same as 'head(hex)'.  |
+| hexhead           | Hexagonal screw head. Will accept drives, but not compulsory.     |
 | hexnut, nut       | Hexagonal outer profile nut with circular cutout.                 |
 | threaded_insert   | Representation of a threaded insert.                              |
 | variable_resistor | Electrical symbol of a variable resistor.                         |
 | washer            | Circular washer with a circular hole.                             |
 | webbolt           | Alternate bolt representation incorporating screw drive, with fixed length. |
 
 A basic set of examples showing the usage of some of these:
```

