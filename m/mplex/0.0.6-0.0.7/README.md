# Comparing `tmp/mplex-0.0.6.tar.gz` & `tmp/mplex-0.0.7.tar.gz`

## Comparing `mplex-0.0.6.tar` & `mplex-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mplex-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mplex-0.0.6/MANIFEST.in
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mplex-0.0.6/requirements.txt
--rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 mplex-0.0.6/examples/test.ipynb
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 mplex-0.0.6/examples/figures/non_uniform.svg
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 mplex-0.0.6/examples/figures/uniform.svg
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/__init__.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/annotate.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/artist.py
--rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/axes.py
--rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/axes_collection.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/cm.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/colors.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/core.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/figure.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/grid.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/style.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/text.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/transforms.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/utils.py
--rw-r--r--   0        0        0    40374 2020-02-02 00:00:00.000000 mplex-0.0.6/mplex/stylesheets/default.mplstyle
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mplex-0.0.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mplex-0.0.6/LICENSE
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mplex-0.0.6/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mplex-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 mplex-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 mplex-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mplex-0.0.7/MANIFEST.in
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mplex-0.0.7/requirements.txt
+-rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 mplex-0.0.7/examples/test.ipynb
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 mplex-0.0.7/examples/figures/non_uniform.svg
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 mplex-0.0.7/examples/figures/uniform.svg
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/__init__.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/annotate.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/artist.py
+-rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/axes.py
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/axes_collection.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/cm.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/colors.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/core.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/figure.py
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/grid.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/plot.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/style.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/text.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/transforms.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/utils.py
+-rw-r--r--   0        0        0    40474 2020-02-02 00:00:00.000000 mplex-0.0.7/mplex/stylesheets/default.mplstyle
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mplex-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mplex-0.0.7/LICENSE
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mplex-0.0.7/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mplex-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 mplex-0.0.7/PKG-INFO
```

### Comparing `mplex-0.0.6/examples/test.ipynb` & `mplex-0.0.7/examples/test.ipynb`

 * *Files identical despite different names*

### Comparing `mplex-0.0.6/examples/figures/non_uniform.svg` & `mplex-0.0.7/examples/figures/non_uniform.svg`

 * *Files identical despite different names*

### Comparing `mplex-0.0.6/examples/figures/uniform.svg` & `mplex-0.0.7/examples/figures/uniform.svg`

 * *Files identical despite different names*

### Comparing `mplex-0.0.6/mplex/annotate.py` & `mplex-0.0.7/mplex/annotate.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     if transform == "axes":
         kw["xycoords"] = ax.transAxes
         line_kw["transform"] = ax.transAxes
 
     kwx = dict(rotation=0, va="top", size=size_x, **kw)
     kwy = dict(rotation=90, va="baseline", size=size_y, **kw)
     kwx_, kwy_ = safe_unpack(text_kw)
-
     if kwx_ is not None:
         kwx.update(**kwx_)
     if kwy_ is not None:
         kwy.update(**kwy_)
 
     kwx["size"] = size_x
     kwy["size"] = size_y
```

### Comparing `mplex-0.0.6/mplex/axes.py` & `mplex-0.0.7/mplex/axes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Axes(plt.Axes):
     def add_text(
         self,
         x,
         y,
         s,
         pad=0,
-        transform="axes",
+        transform="data",
         pad_unit="offset points",
         ha="l",
         va="b",
         **kwargs,
     ):
         from mplex.text import add_text
```

### Comparing `mplex-0.0.6/mplex/axes_collection.py` & `mplex-0.0.7/mplex/axes_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     def __getattr__(self, name: str):
         a = np.array([getattr(ax, name) for ax in self._axs.ravel()], object).reshape(
             (*self._axs.shape, -1)
         )
 
         if all(map(callable, a.ravel())):
             return lambda *args, **kwargs: np.array(
-                [i(*args, **kwargs) for i in a.ravel()]
+                [i(*args, **kwargs) for i in a.ravel()],
+                object,
             ).reshape((*self._axs.shape, -1))
 
         return a
 
     @property
     def axs(self):
         return self._axs
```

### Comparing `mplex-0.0.6/mplex/colors.py` & `mplex-0.0.7/mplex/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,7 +31,12 @@
         return r, g, b, a
     elif colors.to_hex(bg) == "#000000":
         c = 1 - np.array(colors.to_rgb(c))
         r, g, b, a = remove_bg(c, "w")
         return 1 - r, 1 - g, 1 - b, a
     else:
         raise NotImplementedError
+
+
+def to_gray(c):
+    r, g, b = colors.to_rgb(c)
+    return r * 0.2126 + g * 0.7152 + b * 0.0722
```

### Comparing `mplex-0.0.6/mplex/core.py` & `mplex-0.0.7/mplex/core.py`

 * *Files identical despite different names*

### Comparing `mplex-0.0.6/mplex/figure.py` & `mplex-0.0.7/mplex/figure.py`

 * *Files identical despite different names*

### Comparing `mplex-0.0.6/mplex/grid.py` & `mplex-0.0.7/mplex/grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 class Grid(Figure):
     def __init__(
         self,
         axsize=(100, 100),
         shape=(None, None),
         space=(0, 0),
+        border=(0, 0, 0, 0),
         figsize=(None, None),
         unit="pt",
         spines="a",
         sharex="a",
         sharey="a",
         tickdir="oo",
         ticks_sides="lb",
@@ -50,20 +51,25 @@
         hspace = to_array(hspace, nrow - 1)
 
         if len(wspace) < ncol - 1:
             wspace = wspace[np.arange(ncol - 1) % len(wspace)]
 
         if len(hspace) < nrow - 1:
             hspace = hspace[np.arange(nrow - 1) % len(hspace)]
+        
+        if not hasattr(border, "__len__"):
+            border = (border, border, border, border)
+        elif len(border) == 2:
+            border = (border[0], border[0], border[1], border[1])
 
         if len(wspace) == ncol - 1:
-            wspace = np.pad(wspace, 1)
+            wspace = np.array((border[0], *wspace, border[1]))
 
         if len(hspace) == nrow - 1:
-            hspace = np.pad(hspace, 1)
+            hspace = np.array((border[2], *hspace, border[3]))
 
         assert len(wspace) == ncol + 1
         assert len(hspace) == nrow + 1
 
         gridw = np.array(sum(zip_longest(wspace, axw), ())[:-1])
         gridh = np.array(sum(zip_longest(hspace, axh), ())[:-1])
 
@@ -152,7 +158,14 @@
     @property
     def gs(self):
         return self._gs
 
     def sca(self, *keys):
         """Set current axes"""
         self._ca = self[keys]
+
+    def to_rgba_array(self):
+        canvas = self.fig.canvas
+        canvas.draw()
+        img = np.frombuffer(canvas.buffer_rgba(), dtype=np.uint8)
+        img = img.reshape(canvas.get_width_height()[::-1] + (4,))
+        return img
```

### Comparing `mplex-0.0.6/mplex/transforms.py` & `mplex-0.0.7/mplex/transforms.py`

 * *Files identical despite different names*

### Comparing `mplex-0.0.6/mplex/utils.py` & `mplex-0.0.7/mplex/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 
 _to_inch = {
     "pt": Fraction(1 / 72),
     "inch": Fraction(1),
     "in": Fraction(1),
     "cm": Fraction(50, 127),
+    "mm": Fraction(5, 127),
 }
 
 
 def convert_unit(x, fro: str, to: str) -> Any:
     if isinstance(x, Real):
         return float(_to_inch[fro] / _to_inch[to] * x)
     else:
@@ -30,14 +31,16 @@
     if is_array(a):
         return np.asarray(a)
 
     return np.array([a] * n)
 
 
 def safe_unpack(a, *, default1=None, default2=None):
+    if isinstance(a, (str, dict)):
+        a = (a, a)
     try:
         a1, a2 = a
     except (TypeError, ValueError):
         if default1 is None:
             if default2 is None:
                 a1 = a2 = a
             else:
```

### Comparing `mplex-0.0.6/mplex/stylesheets/default.mplstyle` & `mplex-0.0.7/mplex/stylesheets/default.mplstyle`

 * *Files 1% similar despite different names*

```diff
@@ -212,23 +212,23 @@
 ##
 ## Note that font.size controls default text sizes.  To configure
 ## special text sizes tick labels, axes, labels, title, etc., see the rc
 ## settings for axes and ticks.  Special text sizes can be defined
 ## relative to font.size, using the following values: xx-small, x-small,
 ## small, medium, large, x-large, xx-large, larger, or smaller
 
-#font.family:  sans-serif
+font.family:  sans-serif
 #font.style:   normal
 #font.variant: normal
 #font.weight:  normal
 #font.stretch: normal
 font.size:    7.0
 
 #font.serif:      DejaVu Serif, Bitstream Vera Serif, Computer Modern Roman, New Century Schoolbook, Century Schoolbook L, Utopia, ITC Bookman, Bookman, Nimbus Roman No9 L, Times New Roman, Times, Palatino, Charter, serif
-font.sans-serif: Arial, Helvetica, DejaVu Sans, Bitstream Vera Sans, Computer Modern Sans Serif, Lucida Grande, Verdana, Geneva, Lucid, Avant Garde, sans-serif
+font.sans-serif: Arial, DejaVu Sans, Bitstream Vera Sans, Computer Modern Sans Serif, Lucida Grande, Verdana, Geneva, Lucid, Avant Garde, sans-serif
 #font.cursive:    Apple Chancery, Textile, Zapf Chancery, Sand, Script MT, Felipa, Comic Neue, Comic Sans MS, cursive
 #font.fantasy:    Chicago, Charcoal, Impact, Western, Humor Sans, xkcd, fantasy
 #font.monospace:  DejaVu Sans Mono, Bitstream Vera Sans Mono, Computer Modern Typewriter, Andale Mono, Nimbus Mono L, Courier New, Courier, Fixed, Terminal, monospace
 
 
 ## ***************************************************************************
 ## * TEXT                                                                    *
@@ -263,21 +263,22 @@
 
 
 ## ***************************************************************************
 ## * LaTeX                                                                   *
 ## ***************************************************************************
 ## For more information on LaTeX properties, see
 ## https://matplotlib.org/stable/users/explain/text/usetex.html
-#text.usetex: False  # use latex for all text handling. The following fonts
+text.usetex: False   # use latex for all text handling. The following fonts
                      # are supported through the usual rc parameter settings:
                      # new century schoolbook, bookman, times, palatino,
                      # zapf chancery, charter, serif, sans-serif, helvetica,
                      # avant garde, courier, monospace, computer modern roman,
                      # computer modern sans serif, computer modern typewriter
-#text.latex.preamble:   # IMPROPER USE OF THIS FEATURE WILL LEAD TO LATEX FAILURES
+text.latex.preamble: \usepackage{amsmath} \usepackage{amssymb} \usepackage{sfmath} \usepackage{sansmath} \sansmath
+                        # IMPROPER USE OF THIS FEATURE WILL LEAD TO LATEX FAILURES
                         # AND IS THEREFORE UNSUPPORTED. PLEASE DO NOT ASK FOR HELP
                         # IF THIS FEATURE DOES NOT DO WHAT YOU EXPECT IT TO.
                         # text.latex.preamble is a single line of LaTeX code that
                         # will be passed on to the LaTeX system. It may contain
                         # any code that is valid for the LaTeX "preamble", i.e.
                         # between the "\documentclass" and "\begin{document}"
                         # statements.
@@ -322,22 +323,22 @@
 axes.facecolor:     none     # axes background color
 #axes.edgecolor:     black   # axes edge color
 axes.linewidth:     0.5      # edge line width
 #axes.grid:          False   # display grid or not
 #axes.grid.axis:     both    # which axis the grid should apply to
 #axes.grid.which:    major   # grid lines at {major, minor, both} ticks
 #axes.titlelocation: center  # alignment of the title: {left, right, center}
-#axes.titlesize:     large   # font size of the axes title
+axes.titlesize:     7.0     # font size of the axes title
 #axes.titleweight:   normal  # font weight of title
 #axes.titlecolor:    auto    # color of the axes title, auto falls back to
                              # text.color as default value
 #axes.titley:        None    # position title (axes relative units).  None implies auto
-#axes.titlepad:      6.0     # pad between axes and title in points
-#axes.labelsize:     medium  # font size of the x and y labels
-#axes.labelpad:      4.0     # space between label and axis
+axes.titlepad:      2.0     # pad between axes and title in points
+axes.labelsize:      6.0    # font size of the x and y labels
+axes.labelpad:      2.0     # space between label and axis
 #axes.labelweight:   normal  # weight of the x and y labels
 #axes.labelcolor:    black
 #axes.axisbelow:     line    # draw axis gridlines and ticks:
                              #     - below patches (True)
                              #     - above patches but below lines ('line')
                              #     - above all (False)
 
@@ -427,45 +428,45 @@
 ## * TICKS                                                                   *
 ## ***************************************************************************
 ## See https://matplotlib.org/stable/api/axis_api.html#matplotlib.axis.Tick
 #xtick.top:           False   # draw ticks on the top side
 #xtick.bottom:        True    # draw ticks on the bottom side
 #xtick.labeltop:      False   # draw label on the top
 #xtick.labelbottom:   True    # draw label on the bottom
-xtick.major.size:    2.0      # major tick size in points
+xtick.major.size:    1.5      # major tick size in points
 xtick.minor.size:    1.0      # minor tick size in points
 xtick.major.width:   0.5      # major tick width in points
 xtick.minor.width:   0.5      # minor tick width in points
-xtick.major.pad:     2.0      # distance to major tick label in points
-xtick.minor.pad:     2.0      # distance to the minor tick label in points
+xtick.major.pad:     1.5      # distance to major tick label in points
+xtick.minor.pad:     1.5      # distance to the minor tick label in points
 #xtick.color:         black   # color of the ticks
 #xtick.labelcolor:    inherit # color of the tick labels or inherit from xtick.color
-xtick.labelsize:     6.0      # font size of the tick labels
+xtick.labelsize:     5.0      # font size of the tick labels
 #xtick.direction:     out     # direction: {in, out, inout}
 #xtick.minor.visible: False   # visibility of minor ticks on x-axis
 #xtick.major.top:     True    # draw x axis top major ticks
 #xtick.major.bottom:  True    # draw x axis bottom major ticks
 #xtick.minor.top:     True    # draw x axis top minor ticks
 #xtick.minor.bottom:  True    # draw x axis bottom minor ticks
 #xtick.minor.ndivs:   auto    # number of minor ticks between the major ticks on x-axis
 #xtick.alignment:     center  # alignment of xticks
 
 #ytick.left:          True    # draw ticks on the left side
 #ytick.right:         False   # draw ticks on the right side
 #ytick.labelleft:     True    # draw tick labels on the left side
 #ytick.labelright:    False   # draw tick labels on the right side
-ytick.major.size:    2.0      # major tick size in points
+ytick.major.size:    1.5      # major tick size in points
 ytick.minor.size:    1.0      # minor tick size in points
 ytick.major.width:   0.5      # major tick width in points
 ytick.minor.width:   0.5      # minor tick width in points
-ytick.major.pad:     2.0      # distance to major tick label in points
-ytick.minor.pad:     2.0      # distance to the minor tick label in points
+ytick.major.pad:     1.5      # distance to major tick label in points
+ytick.minor.pad:     1.5      # distance to the minor tick label in points
 #ytick.color:         black   # color of the ticks
 #ytick.labelcolor:    inherit # color of the tick labels or inherit from ytick.color
-ytick.labelsize:     6.0     # font size of the tick labels
+ytick.labelsize:     5.0     # font size of the tick labels
 #ytick.direction:     out     # direction: {in, out, inout}
 #ytick.minor.visible: False   # visibility of minor ticks on y-axis
 #ytick.major.left:    True    # draw y axis left major ticks
 #ytick.major.right:   True    # draw y axis right major ticks
 #ytick.minor.left:    True    # draw y axis left minor ticks
 #ytick.minor.right:   True    # draw y axis right minor ticks
 #ytick.minor.ndivs:   auto    # number of minor ticks between the major ticks on y-axis
@@ -514,15 +515,15 @@
 ## ***************************************************************************
 ## See https://matplotlib.org/stable/api/figure_api.html#matplotlib.figure.Figure
 figure.titlesize:   7.0        # size of the figure title (``Figure.suptitle()``)
 #figure.titleweight: normal    # weight of the figure title
 figure.labelsize:   6.0        # size of the figure label (``Figure.sup[x|y]label()``)
 #figure.labelweight: normal    # weight of the figure label
 #figure.figsize:     6.4, 4.8  # figure size in inches
-figure.dpi:         144        # figure dots per inch
+figure.dpi:         300        # figure dots per inch
 figure.facecolor:   none       # figure face color
 figure.edgecolor:   none       # figure edge color
 figure.frameon:     False      # enable figure frame
 #figure.max_open_warning: 20   # The maximum number of figures to open through
                                # the pyplot interface before emitting a warning.
                                # If less than one this feature is disabled.
 #figure.raise_window : True    # Raise the GUI window to front when show() is called.
@@ -669,20 +670,20 @@
 #ps.papersize:      letter  # {figure, letter, legal, ledger, A0-A10, B0-B10}
 #ps.useafm:         False   # use AFM fonts, results in small files
 #ps.usedistiller:   False   # {ghostscript, xpdf, None}
                             # Experimental: may produce smaller files.
                             # xpdf intended for production of publication quality files,
                             # but requires ghostscript, xpdf and ps2eps
 #ps.distiller.res:  6000    # dpi
-#ps.fonttype:       3       # Output Type 3 (Type3) or Type 42 (TrueType)
+ps.fonttype:       42       # Output Type 3 (Type3) or Type 42 (TrueType)
 
 ### PDF backend params
 #pdf.compression:    6  # integer from 0 to 9
                         # 0 disables compression (good for debugging)
-#pdf.fonttype:       3  # Output Type 3 (Type3) or Type 42 (TrueType)
+pdf.fonttype:       42  # Output Type 3 (Type3) or Type 42 (TrueType)
 #pdf.use14corefonts: False
 #pdf.inheritcolor:   False
 
 ### SVG backend params
 #svg.image_inline: True  # Write raster image data directly into the SVG file
 #svg.fonttype: path      # How to handle SVG fonts:
                          #     path: Embed characters as paths -- supported
@@ -748,8 +749,8 @@
 ## subprocess.Popen, except that on Windows, we look up an install of
 ## ImageMagick in the registry (as convert is also the name of a system tool).
 #animation.convert_path: convert
 ## Additional arguments to pass to convert.
 #animation.convert_args: -layers, OptimizePlus
 #
 #animation.embed_limit:  20.0     # Limit, in MB, of size of base64 encoded
-                                  # animation in HTML (i.e. IPython notebook)
+                                  # animation in HTML (i.e. IPython notebook)
```

### Comparing `mplex-0.0.6/.gitignore` & `mplex-0.0.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -153,8 +153,10 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-.idea/
+.idea/
+
+.DS_Store
```

### Comparing `mplex-0.0.6/LICENSE` & `mplex-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mplex-0.0.6/README.md` & `mplex-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mplex-0.0.6/PKG-INFO` & `mplex-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mplex
-Version: 0.0.6
+Version: 0.0.7
 Summary: A matplotlib extension
 Project-URL: Homepage, https://github.com/tkclam/mplex
 Author-email: Thomas Ka Chung Lam <thomas.lam@epfl.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

