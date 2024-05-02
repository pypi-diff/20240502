# Comparing `tmp/statsplotly-0.1.5.tar.gz` & `tmp/statsplotly-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsplotly-0.1.5.tar", max compression
+gzip compressed data, was "statsplotly-0.2.0.tar", max compression
```

## Comparing `statsplotly-0.1.5.tar` & `statsplotly-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,38 @@
--rw-r--r--   0        0        0     1519 2023-11-25 00:43:29.155385 statsplotly-0.1.5/LICENSE
--rw-r--r--   0        0        0     2623 2023-11-25 00:43:29.155385 statsplotly-0.1.5/README.md
--rw-r--r--   0        0        0     2532 2023-11-25 00:44:06.335779 statsplotly-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      225 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/__init__.py
--rw-r--r--   0        0        0     3680 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/constants.py
--rw-r--r--   0        0        0      714 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/exceptions.py
--rw-r--r--   0        0        0      111 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/plot_objects/__init__.py
--rw-r--r--   0        0        0     8496 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/plot_objects/layout_objects.py
--rw-r--r--   0        0        0    26692 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/plot_objects/trace_objects.py
--rw-r--r--   0        0        0       92 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/plot_specifiers/__init__.py
--rw-r--r--   0        0        0     5508 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/plot_specifiers/color.py
--rw-r--r--   0        0        0    23433 2023-11-25 00:43:29.255386 statsplotly-0.1.5/statsplotly/plot_specifiers/data.py
--rw-r--r--   0        0        0     8239 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/plot_specifiers/layout.py
--rw-r--r--   0        0        0    12108 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/plot_specifiers/trace.py
--rw-r--r--   0        0        0        0 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/plotting/__init__.py
--rw-r--r--   0        0        0     5860 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/plotting/helpers.py
--rw-r--r--   0        0        0    58360 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/plotting/main.py
--rw-r--r--   0        0        0        0 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/utils/__init__.py
--rw-r--r--   0        0        0     7819 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/utils/color_utils.py
--rw-r--r--   0        0        0     6285 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/utils/figure_utils.py
--rw-r--r--   0        0        0     5451 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/utils/layout_utils.py
--rw-r--r--   0        0        0     4825 2023-11-25 00:43:29.259386 statsplotly-0.1.5/statsplotly/utils/stats_utils.py
--rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 statsplotly-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1519 2024-05-02 08:47:42.198993 statsplotly-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6330 2024-05-02 08:47:42.198993 statsplotly-0.2.0/README.md
+-rw-r--r--   0        0        0     2885 2024-05-02 08:48:11.478899 statsplotly-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      345 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_base.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/__init__.py
+-rw-r--r--   0        0        0     8240 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_barplot.py
+-rw-r--r--   0        0        0     8126 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_catplot.py
+-rw-r--r--   0        0        0    11056 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_distplot.py
+-rw-r--r--   0        0        0     7247 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_heatmap.py
+-rw-r--r--   0        0        0    20026 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_jointplot.py
+-rw-r--r--   0        0        0    11514 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_plot.py
+-rw-r--r--   0        0        0     6959 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/helpers.py
+-rw-r--r--   0        0        0     4001 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/constants.py
+-rw-r--r--   0        0        0      289 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/exceptions.py
+-rw-r--r--   0        0        0      111 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/__init__.py
+-rw-r--r--   0        0        0      484 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/layout/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/layout/_axis.py
+-rw-r--r--   0        0        0     8458 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/layout/_layout.py
+-rw-r--r--   0        0        0    31230 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/trace.py
+-rw-r--r--   0        0        0      162 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/color/__init__.py
+-rw-r--r--   0        0        0     9518 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/color/_core.py
+-rw-r--r--   0        0        0     7454 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/color/_utils.py
+-rw-r--r--   0        0        0     1730 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/common.py
+-rw-r--r--   0        0        0      862 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/data/__init__.py
+-rw-r--r--   0        0        0    25557 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/data/_core.py
+-rw-r--r--   0        0        0      448 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/data/_utils.py
+-rw-r--r--   0        0        0     4829 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/data/statistics.py
+-rw-r--r--   0        0        0      286 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/figure/__init__.py
+-rw-r--r--   0        0        0     8166 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/figure/_core.py
+-rw-r--r--   0        0        0    23625 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/figure/_utils.py
+-rw-r--r--   0        0        0      595 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/layout/__init__.py
+-rw-r--r--   0        0        0     8221 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/layout/_core.py
+-rw-r--r--   0        0        0     5489 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/layout/_utils.py
+-rw-r--r--   0        0        0    14743 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/trace.py
+-rw-r--r--   0        0        0      111 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/utils.py
+-rw-r--r--   0        0        0     7220 1970-01-01 00:00:00.000000 statsplotly-0.2.0/PKG-INFO
```

### Comparing `statsplotly-0.1.5/LICENSE` & `statsplotly-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statsplotly-0.1.5/pyproject.toml` & `statsplotly-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 [tool.poetry]
 name = "statsplotly"
-version = "0.1.5"
+version = "0.2.0"
 description = "Tidy API for statistical visualization with Plotly"
 authors = ["Benjamin Roland <benjamin.roland@hotmail.fr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/parici75/statsplotly"
 documentation = "https://parici75.github.io/statsplotly/"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.13"
-pydantic = "^2.4"
-seaborn = "^0.12.2"
+pydantic = "^2.6.2"
+seaborn = "^0.13.2"
 scipy = "^1.11.1"
-plotly = "^5.15.0"
 ipykernel = "^6.24.0"
 jupyter = "^1.0.0"
+plotly = "^5.19.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
-mypy = "^1.7.1"
-ruff = "^0.1.6"
-black = "^23.11.0"
-isort = "^5.12.0"
-pyupgrade = "^3.8.0"
-pre-commit = "^3.3.3"
+pytest = "^8.0.2"
+mypy = "^1.8.0"
+ruff = "^0.3.5"
+black = "^24.2.0"
+isort = "^5.13.2"
+pyupgrade = "^3.15.1"
+pre-commit = "^3.6.2"
 pyclean = "^2.7.3"
+coverage = "^7.4.4"
 
 [tool.poetry.group.docs]
 [tool.poetry.group.docs.dependencies]
-m2r2 = "^0.3.3"
+sphinx = "^7.2.6"
 furo = "^2023.5.20"
+myst = "^1.0.4"
+myst-nb = "^1.1.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 pattern  = "^(?P<base>\\d+\\.\\d+\\.\\d+)(-?((?P<stage>[a-zA-Z]+)\\.?(?P<revision>\\d+)?))?"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 ## Tools
 [tool.black]
 target-version = ['py311']
-line_length = 100
+line-length = 100
 preview = true
 
 [tool.ruff]
 line-length = 100
 target-version = "py311"
+exclude = ["tests"]
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "UP", # pyupgrade
     "C",  # flake8-comprehensions
@@ -62,45 +67,58 @@
     "S", # flake8-bandit
     "A", # flake8-builtins
     "INP", # flake8-no-pep420
     "PIE", # flake8-pie
     "PL", # pylint
 ]
 ignore = [
-    "UP015", # Unnecessary open mode parameters
-    "PLC1901", # compare-to-empty-string
+    "E501",
     "PLR0913", # Too many arguments to function call
 ]
-[tool.ruff.per-file-ignores]
-"main.py" = ["C901", "PLR0912", "PLR0915", "E501"]
+[tool.ruff.lint.per-file-ignores]
+"statsplotly/_plotting/**.py" = ["C901", "PLR0912", "PLR0915"]
 
 [tool.isort]
 profile = "black"
 sections = "FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 
 [tool.mypy]
-python_version = 3.11
+python_version = "3.11"
 exclude = ["tests"]
 plugins = [
   "pydantic.mypy", "numpy.typing.mypy_plugin"
 ]
-follow_imports = "silent"
+cache_dir = ".mypy_cache/strict"
+show_error_codes = true
+show_column_numbers = true
+
+follow_imports = "normal"
+warn_no_return = true
+warn_return_any = false
+disallow_any_unimported = false
+disallow_any_generics = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
+disallow_untyped_decorators = true
 warn_redundant_casts = true
 warn_unused_ignores = true
-disallow_untyped_defs = true
-disallow_any_generics = true
-no_implicit_reexport = true
+implicit_reexport = false
+strict_equality = true
+
+# mypy per-module options
+[[tool.mypy.overrides]]
+module = ["dateutil.*", "numpy.*", "scipy.*", "pandas.*", "seaborn.*", "plotly.*", "pymodules.*"]
+ignore_missing_imports = true
+
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = false
 warn_required_dynamic_aliases = true
 
-# mypy per-module options
-[[tool.mypy.overrides]]
-module = ["dateutil.*", "numpy.*", "scipy.*", "pandas.*", "seaborn.*", "plotly.*", "pymodules.*"]
-ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = 10
 testpaths = ["tests"]
```

### Comparing `statsplotly-0.1.5/statsplotly/constants.py` & `statsplotly-0.2.0/statsplotly/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import plotly
 
 # Template
-DEFAULT_TEMPLATE = "none"
+DEFAULT_TEMPLATE = "statsplotly_template"
 
 # Colorscale
 N_COLORSCALE_COLORS = 256
 DEFAULT_COLOR_PALETTE = "viridis"
 SEABORN_DEFAULT_CONTINUOUS_COLOR_PALETTE = "rocket"
 DEFAULT_KDE_COLOR_PALETTE = "magma"
 SHADED_ERROR_ALPHA = 0.2
-DEFAULT_HISTOGRAM_OPACITY = 0.75
+DEFAULT_HISTOGRAM_OPACITY = 0.8
+DEFAULT_OVERLAID_HISTOGRAM_OPACITY = 0.5
 BUILTIN_COLORSCALES = plotly.colors.named_colorscales()
 CSS_COLORS = [
     "aliceblue",
     "antiquewhite",
     "aqua",
     "aquamarine",
     "azure",
@@ -167,32 +168,40 @@
 MAX_MARKER_SIZE = 24
 DEFAULT_MARKER_LINE_COLOR = "grey"
 DEFAULT_MARKER_LINE_WIDTH = 2
 DEFAULT_TRANSPARENCE_OPACITY = 0.8
 DEFAULT_REGRESSION_LINE_OPACITY = 1
 DEFAULT_REGRESSION_LINE_DASH = "dash"
 DEFAULT_HOVERMODE = "closest"
+DEFAULT_STRIPPLOT_JITTER = 1
 
 DEFAULT_ID_LINE_DASH = "longdash"
 DEFAULT_ID_LINE_COLOR = "grey"
 DEFAULT_ID_LINE_WIDTH = 2
 
 # Statistics
 N_GRID_POINTS = 100
 N_CONTOUR_LINES = 20
 CI_ALPHA = 0.05
 IQR = [0.25, 0.75]
 DEFAULT_HISTOGRAM_BIN_COMPUTATION_METHOD = "scott"
 DEFAULT_KDE_BANDWIDTH = 0.2
 
 # Axis parameters
+FIGURE_TITLEFONT = {"family": "Arial", "size": 20}
 AXIS_TITLEFONT = {"family": "Arial", "size": 20}
 TICKFONT = {"family": "Arial", "size": 18}
+SCENE_TICKFONT = {"family": "Arial", "size": 16}
 AXES_HEIGHT = 600
 AXES_WIDTH = 600
 MIN_CAPITALIZE_LENGTH = 3
+RANGE_PADDING_FACTOR = 0.1
 
 # Layout parameters
 LAYOUT_UPDATE_MENUS_TYPE = "dropdown"
 LAYOUT_UPDATE_MENUS_DIRECTION = "down"
 
-DEFAULT_FIGURE_NAME = "plotly_figure"
+# Subplot parameters
+COLORBAR_THICKNESS_SCALING_FACTOR = 30
+COLORBAR_XOFFSET = 1.2
+COLORBAR_REDUCTION_FACTOR = 0.5
+COLORBAR_BOTTOM_POSITION = -0.5
```

### Comparing `statsplotly-0.1.5/statsplotly/plot_objects/layout_objects.py` & `statsplotly-0.2.0/statsplotly/plot_objects/layout/_layout.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,258 +1,264 @@
-import datetime
+from __future__ import annotations
+
 import logging
 from typing import Any
 
-from pydantic import ValidationInfo, field_validator, model_validator
+from pydantic import field_validator
 from pydantic.v1.utils import deep_update
 
-from statsplotly.constants import AXIS_TITLEFONT, DEFAULT_HOVERMODE, TICKFONT
-from statsplotly.exceptions import StatsPlotInvalidArgumentError
-from statsplotly.plot_specifiers.data import BaseModel
-from statsplotly.plot_specifiers.layout import AxesSpecifier, BarMode
+from statsplotly import constants
+from statsplotly._base import BaseModel
+from statsplotly.constants import DEFAULT_HOVERMODE
+from statsplotly.plot_objects.layout._axis import BaseAxis, ColorAxis, XYAxis
+from statsplotly.plot_specifiers.data import DataDimension
+from statsplotly.plot_specifiers.layout import (
+    AxesSpecifier,
+    BarMode,
+    HistogramBarMode,
+    PlotAxis,
+)
 
 logger = logging.getLogger(__name__)
 
-axis_coordinates_type = float | datetime.datetime | str
-
-
-class ColorAxis(BaseModel):
-    cmin: float | None = None
-    cmax: float | None = None
-    colorbar: dict[str, Any] | None = None
-    colorscale: str | list[list[float | str]] | None = None
-    showscale: bool | None = None
-
-
-class BaseAxisLayout(BaseModel):
-    """Compatible properties with 2D and 3D (Scene) Layout."""
 
-    title: str | None = None
-    titlefont: dict[str, Any] = AXIS_TITLEFONT
-    tickfont: dict[str, Any] = TICKFONT
-    range: list[axis_coordinates_type] | None = None  # noqa: A003
-    type: str | None = None  # noqa: A003
-    autorange: bool | str | None = None
-    showgrid: bool | None = None
-    tickmode: str | None = None
-    tickvals: list[axis_coordinates_type] | None = None
-    ticktext: list[str] | None = None
-    zeroline: bool | None = None
-
-    @field_validator("autorange")
-    def validate_autorange(
-        cls, value: bool | str | None, info: ValidationInfo
-    ) -> bool | str | None:
-        if info.data.get("range") is not None:
-            return False
-        return value
-
-    @model_validator(mode="after")  # type: ignore
-    def validate_axis_consistency(cls, model: "BaseAxisLayout") -> "BaseAxisLayout":
-        if model.range is not None and model.tickvals is not None:
-            model.tickvals = model.range
-            if model.ticktext is not None:
-                try:
-                    model.ticktext = [
-                        model.ticktext[int(idx)] for idx in model.tickvals  # type: ignore
-                    ]
-                except TypeError:
-                    logger.error("Can not adjust tick text labels to tick values")
-
-        return model
-
-
-class AxisLayout(BaseAxisLayout):
-    automargin: bool = True
-    scaleanchor: str | None = None
-    scaleratio: float | None = None
+DATA_TO_AXIS_MAP = {DataDimension.X: PlotAxis.XAXIS, DataDimension.Y: PlotAxis.YAXIS}
 
 
-class BaseLayout(BaseModel):
+class _BaseLayout(BaseModel):
     autosize: bool | None = None
     hovermode: str = DEFAULT_HOVERMODE
     title: str | None = None
     height: int | None = None
     width: int | None = None
     showlegend: bool | None = None
 
 
-class XYLayout(BaseLayout):
-    xaxis: AxisLayout
-    yaxis: AxisLayout
+class _XYLayout(_BaseLayout):
+    xaxis: XYAxis
+    yaxis: XYAxis
 
     @classmethod
-    def build_xy_layout(cls, axes_specifier: AxesSpecifier) -> "XYLayout":
-        xaxis_layout = AxisLayout(
+    def build_xy_layout(cls, axes_specifier: AxesSpecifier) -> _XYLayout:
+        xaxis_layout = XYAxis(
             title=axes_specifier.legend.xaxis_title,
             range=axes_specifier.xaxis_range,
         )
-        yaxis_layout = AxisLayout(
+        yaxis_layout = XYAxis(
             title=axes_specifier.legend.yaxis_title,
             range=axes_specifier.yaxis_range,
             scaleanchor=axes_specifier.scaleanchor,
             scaleratio=axes_specifier.scaleratio,
         )
         return cls(
             title=axes_specifier.legend.figure_title,
             xaxis=xaxis_layout,
             yaxis=yaxis_layout,
             height=axes_specifier.height,
             width=axes_specifier.width,
         )
 
 
-class SceneLayout(BaseLayout):
+class _XYColorAxisLayout(_XYLayout):
+    coloraxis: ColorAxis
+
+    @classmethod
+    def build_coloraxis_layout(
+        cls, axes_specifier: AxesSpecifier, coloraxis: ColorAxis
+    ) -> _XYColorAxisLayout:
+        if coloraxis.colorbar is not None:
+            coloraxis.colorbar.update(
+                {
+                    "x": constants.COLORBAR_XOFFSET,
+                    "len": coloraxis.colorbar.get("len", 1) * constants.COLORBAR_REDUCTION_FACTOR,
+                }
+            )
+            if coloraxis.colorbar.get("y") is None:
+                coloraxis.colorbar.update({"y": 0, "yanchor": "bottom"})
+
+        return cls(
+            **_XYLayout.build_xy_layout(axes_specifier=axes_specifier).model_dump(),
+            coloraxis=coloraxis,
+        )
+
+
+class SceneLayout(_BaseLayout):
     scene: dict[str, Any]
     coloraxis: ColorAxis
 
     @classmethod
-    def build_layout(cls, axes_specifier: AxesSpecifier, coloraxis: ColorAxis) -> "SceneLayout":
+    def build_layout(cls, axes_specifier: AxesSpecifier, coloraxis: ColorAxis) -> SceneLayout:
         scene = {
-            "xaxis": BaseAxisLayout(
+            "xaxis": BaseAxis(
                 title=axes_specifier.legend.xaxis_title,
                 range=axes_specifier.xaxis_range,
             ),
-            "yaxis": BaseAxisLayout(
+            "yaxis": BaseAxis(
                 title=axes_specifier.legend.yaxis_title,
                 range=axes_specifier.yaxis_range,
             ),
-            "zaxis": BaseAxisLayout(
+            "zaxis": BaseAxis(
                 title=axes_specifier.legend.zaxis_title,
                 range=axes_specifier.zaxis_range,
             ),
         }
+        if coloraxis.colorbar is not None:
+            coloraxis.colorbar.update(
+                {
+                    "x": constants.COLORBAR_XOFFSET,
+                    "len": coloraxis.colorbar.get("len", 1) * constants.COLORBAR_REDUCTION_FACTOR,
+                }
+            )
+            if coloraxis.colorbar.get("y") is None:
+                coloraxis.colorbar.update({"y": 0, "yanchor": "bottom"})
 
         return cls(
             title=axes_specifier.legend.figure_title,
             scene=scene,
             height=axes_specifier.height,
             width=axes_specifier.width,
             coloraxis=coloraxis,
         )
 
 
-class HeatmapLayout(XYLayout):
+class HeatmapLayout(_XYLayout):
     coloraxis: ColorAxis
 
     @classmethod
-    def update_axis_layout(cls, axis_layout: AxisLayout) -> AxisLayout:
+    def update_axis_layout(cls, axis_layout: XYAxis) -> XYAxis:
         axis_layout_dict = axis_layout.model_dump()
         update_keys: dict[str, Any] = {
             "showgrid": False,
             "zeroline": False,
+            "constrain": "domain",
         }
         axis_layout_dict.update(update_keys)
 
-        return AxisLayout.model_validate(axis_layout_dict)
+        return XYAxis.model_validate(axis_layout_dict)
 
     @classmethod
-    def update_yaxis_layout(cls, yaxis_layout: AxisLayout) -> AxisLayout:
+    def update_yaxis_layout(cls, yaxis_layout: XYAxis) -> XYAxis:
         yaxis_layout_dict = cls.update_axis_layout(yaxis_layout).model_dump()
 
         update_keys: dict[str, Any] = {
             "autorange": "reversed",
             "range": (
                 yaxis_layout_dict.get("range")[::-1]  # type: ignore
                 if yaxis_layout_dict.get("range") is not None
                 else None
             ),
+            "constrain": "domain",
         }
         yaxis_layout_dict.update(update_keys)
 
-        return AxisLayout.model_validate(yaxis_layout_dict)
+        return XYAxis.model_validate(yaxis_layout_dict)
 
     @classmethod
-    def build_layout(cls, axes_specifier: AxesSpecifier, coloraxis: ColorAxis) -> "HeatmapLayout":
-        base_layout = XYLayout.build_xy_layout(axes_specifier=axes_specifier)
+    def build_layout(cls, axes_specifier: AxesSpecifier, coloraxis: ColorAxis) -> HeatmapLayout:
+        base_layout = _XYLayout.build_xy_layout(axes_specifier=axes_specifier)
 
         heatmap_layout = deep_update(
             base_layout.model_dump(),
             {
                 "xaxis": cls.update_axis_layout(
                     base_layout.xaxis,
                 ).model_dump(),
                 "yaxis": cls.update_yaxis_layout(
                     base_layout.yaxis,
                 ).model_dump(),
             },
         )
+        if coloraxis.colorbar is not None:
+            coloraxis.colorbar.update({"title": axes_specifier.legend.zaxis_title})
         heatmap_layout.update({"coloraxis": coloraxis})
 
         return cls.model_validate(heatmap_layout)
 
 
-class CategoricalLayout(XYLayout):
+class CategoricalLayout(_XYColorAxisLayout):
     boxmode: str = "group"
     violinmode: str = "group"
 
     @classmethod
     def set_array_tick_mode(
-        cls, axis_layout: AxisLayout, x_values_map: dict[str, Any]
-    ) -> AxisLayout:
+        cls, axis_layout: XYAxis, categorical_values_map: dict[str, Any]
+    ) -> XYAxis:
         updated_dict = dict.fromkeys(["tickmode", "tickvals", "ticktext"], None)
         updated_dict["tickmode"] = "array"
-        updated_dict["tickvals"] = [k + 1 for k in range(len(x_values_map))]
-        updated_dict["ticktext"] = list(x_values_map.keys())
+        updated_dict["tickvals"] = [k + 1 for k in range(len(categorical_values_map))]
+        updated_dict["ticktext"] = list(categorical_values_map.keys())
 
-        return AxisLayout.model_validate(deep_update(axis_layout.model_dump(), updated_dict))
+        return XYAxis.model_validate(deep_update(axis_layout.model_dump(), updated_dict))
 
     @classmethod
     def build_layout(
-        cls, axes_specifier: AxesSpecifier, x_values_map: dict[str, Any] | None
-    ) -> "CategoricalLayout":
-        base_layout = XYLayout.build_xy_layout(axes_specifier=axes_specifier)
-
-        if x_values_map is not None:
-            xaxis_layout = cls.set_array_tick_mode(
-                axis_layout=base_layout.xaxis, x_values_map=x_values_map
-            )
-            return cls.model_validate(
-                deep_update(base_layout.model_dump(), {"xaxis": xaxis_layout.model_dump()})
-            )
+        cls,
+        axes_specifier: AxesSpecifier,
+        categorical_values_map: dict[DataDimension, dict[str, Any]] | None,
+        coloraxis: ColorAxis,
+    ) -> CategoricalLayout:
+        base_layout = _XYColorAxisLayout.build_coloraxis_layout(
+            axes_specifier=axes_specifier, coloraxis=coloraxis
+        )
 
+        if categorical_values_map is not None:
+            for dimension, values_map in categorical_values_map.items():
+                axis_ref = DATA_TO_AXIS_MAP[dimension]
+                axis_layout = cls.set_array_tick_mode(
+                    axis_layout=getattr(base_layout, axis_ref),
+                    categorical_values_map=values_map,
+                )
+                return cls.model_validate(
+                    deep_update(base_layout.model_dump(), {axis_ref: axis_layout.model_dump()})
+                )
         return cls.model_validate(base_layout.model_dump())
 
 
-class ScatterLayout(XYLayout):
-    coloraxis: ColorAxis
+class ScatterLayout(_XYColorAxisLayout):
 
     @classmethod
     def build_layout(
         cls,
         axes_specifier: AxesSpecifier,
         coloraxis: ColorAxis,
-    ) -> "ScatterLayout":
-        base_layout = XYLayout.build_xy_layout(axes_specifier=axes_specifier)
-        return cls(**base_layout.model_dump(), coloraxis=coloraxis)
+    ) -> ScatterLayout:
 
+        return cls.model_validate(
+            super().build_coloraxis_layout(axes_specifier=axes_specifier, coloraxis=coloraxis)
+        )
 
-class BarLayout(XYLayout):
-    barmode: BarMode | None = None
-    coloraxis: ColorAxis
 
-    @field_validator("barmode", mode="before")
-    def check_barmode(cls, value: str | None) -> BarMode | None:
-        try:
-            return BarMode(value) if value is not None else None
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, BarMode) from exc  # type: ignore
+class BarLayout(_XYColorAxisLayout):
+    barmode: BarMode | None = None
 
     @classmethod
     def build_layout(
         cls,
         axes_specifier: AxesSpecifier,
         coloraxis: ColorAxis,
         barmode: str | None,
-    ) -> "BarLayout":
-        scatter_layout = XYLayout.build_xy_layout(axes_specifier=axes_specifier)
-        return cls(**scatter_layout.model_dump(), coloraxis=coloraxis, barmode=barmode)
+    ) -> BarLayout:
 
+        return cls(
+            **_XYColorAxisLayout.build_coloraxis_layout(
+                axes_specifier=axes_specifier, coloraxis=coloraxis
+            ).model_dump(),
+            barmode=barmode,
+        )
 
-class HistogramLayout(XYLayout):
-    barmode: BarMode | None = None
+
+class HistogramLayout(_XYLayout):
+    barmode: HistogramBarMode
+
+    @field_validator("barmode", mode="before")
+    def validate_histogram_barmode(cls, value: str | None) -> HistogramBarMode:
+        if value is None:
+            return HistogramBarMode.OVERLAY
+
+        return HistogramBarMode(value)
 
     @classmethod
-    def build_layout(cls, axes_specifier: AxesSpecifier, barmode: str | None) -> "HistogramLayout":
-        base_layout = XYLayout.build_xy_layout(axes_specifier=axes_specifier)
+    def build_layout(cls, axes_specifier: AxesSpecifier, barmode: str | None) -> HistogramLayout:
 
-        return cls(**base_layout.model_dump(), barmode=barmode)
+        return cls(
+            **_XYLayout.build_xy_layout(axes_specifier=axes_specifier).model_dump(), barmode=barmode
+        )
```

### Comparing `statsplotly-0.1.5/statsplotly/plot_objects/trace_objects.py` & `statsplotly-0.2.0/statsplotly/plot_objects/trace.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,61 @@
+from __future__ import annotations
+
 import logging
 from abc import ABCMeta, abstractmethod
+from collections.abc import Callable
 from typing import Any
 
 import numpy as np
 import pandas as pd
+import plotly
+import plotly.graph_objects as go
 from numpy.typing import NDArray
 from pydantic.v1.utils import deep_update
 
 from statsplotly import constants
-from statsplotly.plot_specifiers.color import ColorSpecifier
+from statsplotly._base import BaseModel
+from statsplotly.plot_specifiers.color import ColorSpecifier, set_rgb_alpha
 from statsplotly.plot_specifiers.data import (
     TRACE_DIMENSION_MAP,
     AggregationTraceData,
-    BaseModel,
     DataDimension,
     HistogramNormType,
     RegressionType,
     TraceData,
 )
-from statsplotly.plot_specifiers.trace import (
-    HistogramSpecifier,
-    JointplotSpecifier,
-    JointplotType,
-    TraceMode,
-)
-from statsplotly.utils.color_utils import set_rgb_alpha
-from statsplotly.utils.stats_utils import (
+from statsplotly.plot_specifiers.data.statistics import (
     affine_func,
     exponential_regress,
     inverse_func,
     kde_1d,
     kde_2d,
     regress,
 )
+from statsplotly.plot_specifiers.trace import (
+    CategoricalPlotSpecifier,
+    HistogramSpecifier,
+    JointplotSpecifier,
+    JointplotType,
+    OrientedPlotSpecifier,
+    PlotOrientation,
+    TraceMode,
+)
 
 logger = logging.getLogger(__name__)
 
 
-class BaseTrace(BaseModel):
+class _BasePlotlyTrace(BaseModel):
+    _PLOTLY_GRAPH_FCT: Callable[[Any], Any]
+
+    def to_plotly_trace(self) -> plotly.basedatatypes.BaseTraceType:
+        return self._PLOTLY_GRAPH_FCT(self.model_dump())
+
+
+class BaseTrace(BaseModel, metaclass=ABCMeta):
     x: pd.Series | NDArray[Any] | None = None
     y: pd.Series | NDArray[Any] | None = None
     name: str
     opacity: float | None = None
     legendgroup: str | None = None
     showlegend: bool | None = None
 
@@ -73,14 +87,19 @@
                 ],
                 strict=True,
             )
         ]
 
         return error_parameters
 
+    @abstractmethod
+    def build_trace(cls, *args: Any, **kwargs: Any) -> BaseTrace:
+        """This method implements the logic to generate the Trace object."""
+        ...
+
 
 class _ScatterBaseTrace(BaseTrace):
     marker: dict[str, Any] | None = None
     mode: TraceMode | None = None
     error_x: dict[str, Any] | None = None
     error_y: dict[str, Any] | None = None
     text: str | pd.Series | None = None
@@ -88,18 +107,18 @@
     hoverinfo: str = "x+y+name+text"
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
         mode: TraceMode | None,
-    ) -> "_ScatterBaseTrace":
+    ) -> _ScatterBaseTrace:
         error_x_data, error_y_data, _ = cls.get_error_bars(trace_data)
 
         return cls(
             x=trace_data.x_values,
             y=trace_data.y_values,
             name=trace_name,
             opacity=color_specifier.opacity,
@@ -112,42 +131,47 @@
                 "color": (
                     color_specifier.format_color_data(trace_data.color_data)
                     if trace_data.color_data is not None
                     else trace_color
                 ),
                 "opacity": trace_data.opacity_data,
                 "symbol": trace_data.marker_data,
-                "coloraxis": color_specifier.coloraxis_reference,
+                "coloraxis": (
+                    color_specifier.coloraxis_reference
+                    if trace_data.color_data is not None
+                    else None
+                ),
             },
             legendgroup=trace_name,
         )
 
 
-class _DensityTrace(BaseTrace, metaclass=ABCMeta):
+class _DensityTrace(BaseTrace):
     z: pd.Series | NDArray[Any]
     coloraxis: str | None = None
     zmin: float | None = None
     zmax: float | None = None
     text: str | pd.Series | None = None
 
 
-class HeatmapTrace(_DensityTrace):
+class HeatmapTrace(_DensityTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Heatmap
+
     hoverinfo: str = "x+y+z+text"
     colorbar: dict[str, Any] | None = None
     colorscale: str | list[list[str | float]] | None = None
-    text: str | pd.Series | None = None
 
     @classmethod
     def build_histmap_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
         color_specifier: ColorSpecifier,
         jointplot_specifier: JointplotSpecifier,
-    ) -> "HeatmapTrace":
+    ) -> HeatmapTrace:
         anchor_values, hist, bin_centers = jointplot_specifier.compute_histmap(trace_data)
 
         return cls(
             x=(
                 anchor_values
                 if jointplot_specifier.plot_type is JointplotType.X_HISTMAP
                 else bin_centers
@@ -170,37 +194,39 @@
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
         color_specifier: ColorSpecifier,
-    ) -> "HeatmapTrace":
+    ) -> HeatmapTrace:
         return cls(
             x=trace_data.x_values,
             y=trace_data.y_values,
-            z=trace_data.z_values,
+            z=color_specifier.format_color_data(trace_data.z_values),
             zmin=color_specifier.zmin,
             zmax=color_specifier.zmax,
             coloraxis=color_specifier.coloraxis_reference,
             name=trace_name,
             opacity=color_specifier.opacity,
             text=trace_data.text_data,
             legendgroup=trace_name,
         )
 
 
-class ScatterTrace(_ScatterBaseTrace):
+class ScatterTrace(_ScatterBaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Scatter
+
     hoverinfo: str = "x+y+name+text"
     line: dict[str, Any] | None = None
     fill: str | None = None
     fillcolor: str | None = None
 
     @classmethod
-    def build_id_line(cls, x_values: pd.Series, y_values: pd.Series) -> "ScatterTrace":
+    def build_id_line(cls, x_values: pd.Series, y_values: pd.Series) -> ScatterTrace:
         line_data = pd.Series(
             (
                 min(x_values.min(), y_values.min()),
                 max(x_values.max(), y_values.max()),
             )
         )
         return cls(
@@ -213,57 +239,65 @@
                 "width": constants.DEFAULT_ID_LINE_WIDTH,
                 "dash": constants.DEFAULT_ID_LINE_DASH,
             },
         )
 
     @classmethod
     def build_lower_error_trace(
-        cls, trace_data: TraceData, trace_name: str, trace_color: str
-    ) -> "ScatterTrace":
+        cls, trace_data: TraceData, trace_name: str, trace_color: str | None
+    ) -> ScatterTrace:
         if trace_data.shaded_error is None:
             raise ValueError("`trace_data.shaded_error` can not be `None`")
 
         return cls(
             x=trace_data.x_values,
             y=trace_data.shaded_error.apply(lambda x: x[0]),
             name=f"{trace_name} {trace_data.shaded_error.name} lower bound",
             mode=TraceMode.LINES,
             line={"width": 0},
             fill="tonexty",
-            fillcolor=set_rgb_alpha(trace_color, constants.SHADED_ERROR_ALPHA),
+            fillcolor=(
+                set_rgb_alpha(trace_color, constants.SHADED_ERROR_ALPHA)
+                if trace_color is not None
+                else None
+            ),
             legendgroup=trace_name,
             showlegend=False,
         )
 
     @classmethod
     def build_upper_error_trace(
-        cls, trace_data: TraceData, trace_name: str, trace_color: str
-    ) -> "ScatterTrace":
+        cls, trace_data: TraceData, trace_name: str, trace_color: str | None
+    ) -> ScatterTrace:
         if trace_data.shaded_error is None:
             raise ValueError("`trace_data.shaded_error` can not be `None`")
         return cls(
             x=trace_data.x_values,
             y=trace_data.shaded_error.apply(lambda x: x[1]),
             name=f"{trace_name} {trace_data.shaded_error.name} upper bound",
             mode=TraceMode.LINES,
             marker={"size": trace_data.size_data, "color": trace_color},
             line={"width": 0},
-            fillcolor=set_rgb_alpha(trace_color, constants.SHADED_ERROR_ALPHA),
+            fillcolor=(
+                set_rgb_alpha(trace_color, constants.SHADED_ERROR_ALPHA)
+                if trace_color is not None
+                else None
+            ),
             legendgroup=trace_name,
             showlegend=False,
         )
 
     @classmethod
     def build_regression_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
         trace_color: str,
         regression_type: RegressionType,
-    ) -> "ScatterTrace":
+    ) -> ScatterTrace:
         if trace_data.x_values is None or trace_data.y_values is None:
             raise ValueError("`trace_data.x_values` and `trace_data.x_values` can not be `None`")
 
         if regression_type is RegressionType.LINEAR:
             p, r2, (x_grid, y_fit) = regress(trace_data.x_values, trace_data.y_values, affine_func)
             regression_legend = f"alpha={p[0]:.2f}, r={np.sqrt(r2):.2f}"
         elif regression_type is RegressionType.EXPONENTIAL:
@@ -286,45 +320,47 @@
         )
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
         mode: TraceMode | None,
-    ) -> "ScatterTrace":
+    ) -> ScatterTrace:
         return cls(
             **super()
             .build_trace(
                 trace_data=trace_data,
                 trace_name=trace_name,
                 trace_color=trace_color,
                 color_specifier=color_specifier,
                 mode=mode,
             )
             .model_dump()
         )
 
 
-class Scatter3DTrace(_ScatterBaseTrace):
+class Scatter3DTrace(_ScatterBaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Scatter3d
+
     hoverinfo: str = "x+y+z+name+text"
     z: pd.Series | NDArray[Any]
     error_z: dict[str, Any] | None = None
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
         mode: TraceMode | None,
-    ) -> "Scatter3DTrace":
+    ) -> Scatter3DTrace:
         scatter_trace = _ScatterBaseTrace.build_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             trace_color=trace_color,
             color_specifier=color_specifier,
             mode=mode,
         )
@@ -345,206 +381,267 @@
                 },
             },
         )
 
         return cls.model_validate(scatter3d_trace)
 
 
-class _CategoricalTrace(BaseTrace, metaclass=ABCMeta):
-    hoverinfo: str = "x+y+name+text"
+class _CategoricalTrace(BaseTrace):
+    hoverinfo: str
     marker: dict[str, Any] | None = None
     text: str | pd.Series | None = None
 
     @classmethod
-    @abstractmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
-    ) -> "_CategoricalTrace":
+        categorical_plot_specifier: CategoricalPlotSpecifier,
+    ) -> _CategoricalTrace:
+        hover_info = "name+text"
+        if categorical_plot_specifier.orientation is PlotOrientation.VERTICAL:
+            hover_info += "+y"
+        else:
+            hover_info += "+x"
+
         return cls(
             x=trace_data.x_values,
             y=trace_data.y_values,
+            hoverinfo=hover_info,
             name=trace_name,
             text=trace_data.text_data,
+            legendgroup=trace_name,
             opacity=color_specifier.opacity,
             marker={
                 "size": trace_data.size_data,
                 "color": (
                     color_specifier.format_color_data(trace_data.color_data)
                     if trace_data.color_data is not None
                     else trace_color
                 ),
                 "opacity": trace_data.opacity_data,
                 "symbol": trace_data.marker_data,
             },
         )
 
 
-class StripTrace(_CategoricalTrace):
+class StripTrace(_CategoricalTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Scatter
+
     mode: str = TraceMode.MARKERS
 
-    @staticmethod
-    def get_x_strip_map(x_values: pd.Series) -> dict[str, Any]:
-        def _cast_strip_coordinates(x_coord: Any) -> Any:
-            if np.issubdtype(type(x_coord), np.datetime64):
-                return pd.Timestamp(x_coord)
-            return x_coord
-
-        x_dict: dict[str, Any] = {}
-        for i, x_level in enumerate(np.sort(x_values.dropna().unique()), 1):
-            x_dict[_cast_strip_coordinates(x_level)] = i
+    @classmethod
+    def build_trace(
+        cls,
+        trace_data: TraceData,
+        trace_name: str,
+        trace_color: str | None,
+        color_specifier: ColorSpecifier,
+        categorical_plot_specifier: CategoricalPlotSpecifier,
+    ) -> StripTrace:
+
+        categorical_trace = _CategoricalTrace.build_trace(
+            trace_data, trace_name, trace_color, color_specifier, categorical_plot_specifier
+        )
+
+        strip_trace = deep_update(
+            categorical_trace.model_dump(),
+            {
+                "marker": {
+                    "coloraxis": color_specifier.coloraxis_reference,
+                },
+            },
+        )
+
+        return cls.model_validate(strip_trace)
 
-        return x_dict
+
+class _OrientedTrace(_CategoricalTrace):
+    orientation: str
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
-    ) -> "StripTrace":
+        categorical_plot_specifier: CategoricalPlotSpecifier,
+    ) -> _OrientedTrace:
+
+        categorical_trace = _CategoricalTrace.build_trace(
+            trace_data, trace_name, trace_color, color_specifier, categorical_plot_specifier
+        )
+
         return cls(
-            **super().build_trace(trace_data, trace_name, trace_color, color_specifier).model_dump()
+            **categorical_trace.model_dump(),
+            orientation=(
+                "h" if categorical_plot_specifier.orientation is PlotOrientation.HORIZONTAL else "v"
+            ),
         )
 
 
-class BoxTrace(_CategoricalTrace):
+class BoxTrace(_OrientedTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Box
+
     boxmean: bool = True
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
-    ) -> "BoxTrace":
-        return cls(
-            **super().build_trace(trace_data, trace_name, trace_color, color_specifier).model_dump()
+        categorical_plot_specifier: CategoricalPlotSpecifier,
+    ) -> BoxTrace:
+        return cls.model_validate(
+            super().build_trace(
+                trace_data, trace_name, trace_color, color_specifier, categorical_plot_specifier
+            )
         )
 
 
-class ViolinTrace(_CategoricalTrace):
+class ViolinTrace(_OrientedTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Violin
+
     meanline_visible: bool = True
     scalemode: str = "width"
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
-    ) -> "ViolinTrace":
-        return cls(
-            **super().build_trace(trace_data, trace_name, trace_color, color_specifier).model_dump()
+        categorical_plot_specifier: CategoricalPlotSpecifier,
+    ) -> ViolinTrace:
+        return cls.model_validate(
+            super().build_trace(
+                trace_data, trace_name, trace_color, color_specifier, categorical_plot_specifier
+            )
         )
 
 
-class BarTrace(BaseTrace):
+class BarTrace(BaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Bar
+
     hoverinfo: str = "x+y+name+text"
     marker: dict[str, Any] | None = None
+    error_x: dict[str, Any] | None = None
     error_y: dict[str, Any] | None = None
     text: str | pd.Series | None = None
     textposition: str | None = None
+    orientation: str
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData | AggregationTraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
-    ) -> "BarTrace":
-        _, error_y_data, _ = cls.get_error_bars(trace_data)
+        bar_plot_specifier: OrientedPlotSpecifier,
+    ) -> BarTrace:
+        error_x_data, error_y_data, _ = cls.get_error_bars(trace_data)
+        bar_annotation = trace_name if trace_data.color_data is not None else None
 
         return cls(
             x=trace_data.x_values,
             y=trace_data.y_values,
+            orientation=(
+                "h" if bar_plot_specifier.orientation is PlotOrientation.HORIZONTAL else "v"
+            ),
             name=trace_name,
             opacity=color_specifier.opacity,
-            text=trace_data.text_data,
+            text=trace_data.text_data if trace_data.text_data is not None else bar_annotation,
+            error_x=error_x_data,
             error_y=error_y_data,
             marker={
                 "color": (
                     color_specifier.format_color_data(trace_data.color_data)
                     if trace_data.color_data is not None
                     else trace_color
                 ),
                 "opacity": trace_data.opacity_data,
                 "coloraxis": color_specifier.coloraxis_reference,
             },
             legendgroup=trace_name,
         )
 
 
-class StepHistogramTrace(BaseTrace):
+class StepHistogramTrace(BaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Scatter
+
     line: dict[str, Any]
     hoverinfo: str = "all"
     mode: TraceMode = TraceMode.LINES
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
         histogram_specifier: HistogramSpecifier,
-    ) -> "StepHistogramTrace":
+    ) -> StepHistogramTrace:
         histogram_data = getattr(trace_data, TRACE_DIMENSION_MAP[histogram_specifier.dimension])
-        hist, bin_edges, binsize = histogram_specifier.histogram(histogram_data)
-        bin_centers = (bin_edges[1:] + bin_edges[:-1]) / 2
+        hist, bin_edges, binsize = histogram_specifier.compute_histogram(histogram_data)
+        bin_centers = np.concatenate(
+            ([bin_edges[0]], (bin_edges[1:] + bin_edges[:-1]) / 2, [bin_edges[-1]])
+        )
+        padded_hist = np.pad(hist, 1, constant_values=0)
 
         return cls(
-            x=bin_centers if histogram_specifier.dimension is DataDimension.X else hist,
-            y=hist if histogram_specifier.dimension is DataDimension.X else bin_centers,
+            x=bin_centers if histogram_specifier.dimension is DataDimension.X else padded_hist,
+            y=padded_hist if histogram_specifier.dimension is DataDimension.X else bin_centers,
             name=f"{trace_name} {histogram_data.name}",
             line={
-                "color": (
-                    trace_data.color_data if trace_data.color_data is not None else trace_color
-                ),
+                "color": trace_color,
                 "shape": "hvh" if histogram_specifier.dimension is DataDimension.X else "vhv",
             },
             opacity=color_specifier.opacity,
             legendgroup=trace_name,
         )
 
 
-class RugTrace(BaseTrace):
+class RugTrace(BaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Scatter
+
     hoverinfo: str
     line: dict[str, Any] | None = None
     mode: TraceMode = TraceMode.LINES
     showlegend: bool = False
     text: str | pd.Series | None = None
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
         histogram_specifier: HistogramSpecifier,
-    ) -> "RugTrace":
+    ) -> RugTrace:
         rug_data = getattr(trace_data, TRACE_DIMENSION_MAP[histogram_specifier.dimension])
 
         rug_coord = np.tile(rug_data, (2, 1)).transpose()
         rug_coord_grid = np.concatenate(
             (rug_coord, np.tile(None, (len(rug_coord), 1))),  # type:ignore
             axis=1,
         ).ravel()
 
-        hist, _, _ = histogram_specifier.histogram(data=rug_data)
-
-        rug_length_coord = np.tile(np.array([0, 0.1 * max(hist)]), (len(rug_coord), 1))
+        rug_length_coord = np.tile(
+            np.array([0, -0.1 * histogram_specifier.get_distribution_max_value(rug_data)]),
+            (len(rug_coord), 1),
+        )
         rug_length_grid = np.concatenate(
             (
                 rug_length_coord,
                 np.tile(None, (len(rug_length_coord), 1)),  # type:ignore
             ),
             axis=1,
         ).ravel()
@@ -559,75 +656,112 @@
                 rug_length_grid
                 if histogram_specifier.dimension is DataDimension.X
                 else rug_coord_grid
             ),
             name=f"{trace_name} {rug_data.name} raw observations",
             hoverinfo="x+text" if histogram_specifier.dimension is DataDimension.X else "y+text",
             line={
-                "color": (
-                    trace_data.color_data if trace_data.color_data is not None else trace_color
-                ),
+                "color": trace_color,
                 "width": 1,
             },
             legendgroup=trace_name,
         )
 
 
-class HistogramTrace(BaseTrace):
+class HistogramTrace(BaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Histogram
+
     marker: dict[str, Any] | None = None
     cumulative: dict[str, Any] | None = None
     xbins: dict[str, Any] | None = None
     histnorm: HistogramNormType | None = None
     hoverinfo: str = "all"
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
         histogram_specifier: HistogramSpecifier,
-    ) -> "HistogramTrace":
+    ) -> HistogramTrace:
         histogram_data = getattr(trace_data, TRACE_DIMENSION_MAP[histogram_specifier.dimension])
-        bin_edges, bin_size = histogram_specifier.histogram_bin_edges(histogram_data)
+        bin_edges, bin_size = histogram_specifier.get_histogram_bin_edges(histogram_data)
 
         return cls(
             x=histogram_data if histogram_specifier.dimension is DataDimension.X else None,
             y=histogram_data if histogram_specifier.dimension is DataDimension.Y else None,
-            name=f"{trace_name} distribution",
+            name=(
+                f"{trace_name} cumulative distribution"
+                if histogram_specifier.cumulative
+                else f"{trace_name} distribution"
+            ),
             opacity=color_specifier.opacity,
             legendgroup=trace_name,
-            marker={
-                "color": trace_data.color_data if trace_data.color_data is not None else trace_color
-            },
+            marker={"color": trace_color},
             cumulative={"enabled": histogram_specifier.cumulative},
             xbins={"start": bin_edges[0], "end": bin_edges[-1], "size": bin_size},
             histnorm=histogram_specifier.histnorm,
         )
 
 
-class Histogram2dTrace(BaseTrace):
+class EcdfTrace(BaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Scatter
+
+    line: dict[str, Any]
+    hoverinfo: str = "all"
+    mode: TraceMode = TraceMode.LINES
+
+    @classmethod
+    def build_trace(
+        cls,
+        trace_data: TraceData,
+        trace_name: str,
+        trace_color: str | None,
+        color_specifier: ColorSpecifier,
+        histogram_specifier: HistogramSpecifier,
+    ) -> EcdfTrace:
+        rank_counts, ranks = histogram_specifier.compute_ecdf(
+            getattr(trace_data, TRACE_DIMENSION_MAP[histogram_specifier.dimension])
+        )
+
+        return cls(
+            x=ranks if histogram_specifier.dimension is DataDimension.X else rank_counts,
+            y=rank_counts if histogram_specifier.dimension is DataDimension.X else ranks,
+            name=f"{trace_name} ecdf",
+            opacity=color_specifier.opacity,
+            legendgroup=trace_name,
+            line={
+                "color": trace_color,
+                "shape": "hv" if histogram_specifier.dimension is DataDimension.X else "vh",
+            },
+        )
+
+
+class Histogram2dTrace(BaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Histogram2d
+
     marker: dict[str, Any] | None = None
     xbins: dict[str, Any] | None = None
     ybins: dict[str, Any] | None = None
     colorbar: dict[str, Any] | None = None
     colorscale: str | list[list[str | float]] | None = None
     histnorm: HistogramNormType | None = None
     hoverinfo: str = "all"
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
         jointplot_specifier: JointplotSpecifier,
-    ) -> "Histogram2dTrace":
+    ) -> Histogram2dTrace:
         (
             hist,
             (xbin_edges, ybin_edges),
             (xbin_size, ybin_size),
         ) = jointplot_specifier.histogram2d(
             data=pd.concat([trace_data.x_values, trace_data.y_values], axis=1)
         )
@@ -653,84 +787,94 @@
             ),
             histnorm=jointplot_specifier.histogram_specifier[  # type: ignore
                 DataDimension.X
             ].histnorm,
         )
 
 
-class KdeTrace(BaseTrace):
-    hoverinfo: str = "none"
+class KdeTrace(BaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Scatter
+
+    hoverinfo: str = "x+y"
     line: dict[str, Any]
     mode: TraceMode = TraceMode.LINES
     showlegend: bool = False
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         color_specifier: ColorSpecifier,
         histogram_specifier: HistogramSpecifier,
-    ) -> "KdeTrace":
+    ) -> KdeTrace:
         histogram_data = getattr(trace_data, TRACE_DIMENSION_MAP[histogram_specifier.dimension])
-        bin_edges, bin_size = histogram_specifier.histogram_bin_edges(histogram_data)
+        bin_edges, bin_size = histogram_specifier.get_histogram_bin_edges(histogram_data)
 
         grid = np.linspace(
             np.floor(bin_edges.min()),
             np.ceil(bin_edges.max()),
             constants.N_GRID_POINTS,
         )
         kde = kde_1d(histogram_data, grid)
-        color = trace_data.color_data if trace_data.color_data is not None else trace_color
-
+        line_color = (
+            set_rgb_alpha(trace_color, color_specifier.opacity or 1)
+            if trace_color is not None
+            else None
+        )
         return cls(
             x=grid if histogram_specifier.dimension is DataDimension.X else kde,
             y=kde if histogram_specifier.dimension is DataDimension.X else grid,
             name=f"{trace_name} pdf",
-            line={"color": set_rgb_alpha(color, color_specifier.opacity or 1)},
+            line={"color": line_color},
             legendgroup=trace_name,
         )
 
 
-class HistogramLineTrace(BaseTrace):
+class HistogramLineTrace(BaseTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Scatter
+
     hoverinfo: str
     line: dict[str, Any]
     mode: TraceMode = TraceMode.LINES
     showlegend: bool = True
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
-        trace_color: str,
+        trace_color: str | None,
         histogram_specifier: HistogramSpecifier,
         hline_coordinates: tuple[str, float] | None = None,
         vline_coordinates: tuple[str, float] | None = None,
-    ) -> "HistogramLineTrace":
+    ) -> HistogramLineTrace:
         if vline_coordinates is not None:
             vline_name, vline_data = vline_coordinates
             x_data = np.repeat(vline_data, 2)
             if trace_data.x_values is not None:
-                hist, _, _ = histogram_specifier.histogram(trace_data.x_values)
-                y_data = np.array([0, max(hist)])
+                y_data = np.array(
+                    [0, histogram_specifier.get_distribution_max_value(trace_data.x_values)]
+                )
             else:
                 if trace_data.y_values is None:
                     raise ValueError("`trace_data.y_values` can not be `None`")
                 y_data = np.sort(trace_data.y_values)[[0, -1]]
             name = f"{trace_name} {vline_name}={vline_data:.2f}"
             hoverinfo = "x+name"
 
         elif hline_coordinates is not None:
             hline_name, hline_data = hline_coordinates
             y_data = np.repeat(hline_data, 2)
             if trace_data.y_values is not None:
-                hist, _, _ = histogram_specifier.histogram(trace_data.y_values)
-                x_data = np.array([0, max(hist)])
+                hist, _, _ = histogram_specifier.compute_histogram(trace_data.y_values)
+                x_data = np.array(
+                    [0, histogram_specifier.get_distribution_max_value(trace_data.y_values)]
+                )
             else:
                 if trace_data.x_values is None:
                     raise ValueError("`trace_data.x_values` can not be `None`")
                 x_data = np.sort(trace_data.x_values)[[0, -1]]
             name = f"{trace_name} {hline_name}={hline_data:.2f}"
             hoverinfo = "y+name"
         else:
@@ -747,45 +891,47 @@
                 "dash": "dot",
             },
             hoverinfo=hoverinfo,
             legendgroup=trace_name,
         )
 
 
-class ContourTrace(_DensityTrace):
+class ContourTrace(_DensityTrace, _BasePlotlyTrace):
+    _PLOTLY_GRAPH_FCT = go.Contour
+
     colorscale: str | list[list[str | float]] | None = None
     hoverinfo: str = "all"
     ncontours: int
     reversescale: bool = True
     showscale: bool = False
 
     @classmethod
     def build_trace(
         cls,
         trace_data: TraceData,
         trace_name: str,
         color_specifier: ColorSpecifier,
         jointplot_specifier: JointplotSpecifier,
-    ) -> "ContourTrace":
+    ) -> ContourTrace:
         if trace_data.x_values is None or trace_data.y_values is None:
             raise ValueError("`trace_data.x_values` and `trace_data.x_values` can not be `None`")
         # X grid
         bin_edges, binsize = jointplot_specifier.histogram_specifier[  # type: ignore
             DataDimension.X
-        ].histogram_bin_edges(trace_data.x_values)
+        ].get_histogram_bin_edges(trace_data.x_values)
         x_grid = np.linspace(
             np.floor(bin_edges.min()),
             np.ceil(bin_edges.max()),
             constants.N_GRID_POINTS,
         )
 
         # Y grid
         bin_edges, binsize = jointplot_specifier.histogram_specifier[  # type: ignore
             DataDimension.Y
-        ].histogram_bin_edges(trace_data.y_values)
+        ].get_histogram_bin_edges(trace_data.y_values)
         y_grid = np.linspace(
             np.floor(bin_edges.min()),
             np.ceil(bin_edges.max()),
             constants.N_GRID_POINTS,
         )
 
         z_data = kde_2d(trace_data.x_values, trace_data.y_values, x_grid, y_grid)
```

### Comparing `statsplotly-0.1.5/statsplotly/plot_specifiers/data.py` & `statsplotly-0.2.0/statsplotly/plot_specifiers/data/_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+from __future__ import annotations
+
 import logging
 from collections.abc import Callable, Generator
 from enum import Enum
 from functools import wraps
 from typing import Any, TypeVar
 
 import numpy as np
 import pandas as pd
 import scipy as sc
 from numpy.typing import NDArray
-from pandas.api.types import is_numeric_dtype
-from pydantic import BaseModel as PydanticBaseModel
-from pydantic import ConfigDict, ValidationInfo, field_validator, model_validator
+from pydantic import ValidationInfo, field_validator, model_validator
 
 from statsplotly import constants
+from statsplotly._base import BaseModel
 from statsplotly.exceptions import (
-    StatsPlotInvalidArgumentError,
     StatsPlotMissingImplementationError,
     StatsPlotSpecificationError,
 )
-from statsplotly.utils.color_utils import rand_jitter
-from statsplotly.utils.stats_utils import range_normalize, sem
+
+from ._utils import rand_jitter
+from .statistics import range_normalize, sem
 
 logger = logging.getLogger(__name__)
 
 
-class BaseModel(PydanticBaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True)
+class DataDimension(str, Enum):
+    X = "x"
+    Y = "y"
+    Z = "z"
 
 
 class SliceTraceType(str, Enum):
     ALL_DATA = "all data"
+    SLICE = "slice"
 
 
 class NormalizationType(str, Enum):
     CENTER = "center"
     MIN_MAX = "minmax"
     ZSCORE = "zscore"
 
@@ -42,14 +46,15 @@
     LINEAR = "linear"
     EXPONENTIAL = "exponential"
     INVERSE = "inverse"
 
 
 class AggregationType(str, Enum):
     MEAN = "mean"
+    GEO_MEAN = "geo_mean"
     COUNT = "count"
     MEDIAN = "median"
     PERCENT = "percent"
     PROBABILITY = "probability"
     SUM = "sum"
 
 
@@ -58,14 +63,15 @@
     MEDIAN = "median"
 
 
 class ErrorBarType(str, Enum):
     SEM = "sem"
     IQR = "iqr"
     STD = "std"
+    GEO_STD = "geo_std"
     BOOTSTRAP = "bootstrap"
 
 
 class HistogramNormType(str, Enum):
     COUNT = ""
     PERCENT = "percent"
     PROBABILITY = "probability"
@@ -74,41 +80,44 @@
 
 AGG_TO_ERROR_MAPPING: dict[CentralTendencyType, ErrorBarType] = {
     CentralTendencyType.MEAN: ErrorBarType.STD,
     CentralTendencyType.MEDIAN: ErrorBarType.IQR,
 }
 
 
-class DataTypes(BaseModel):
-    x: np.dtype[Any] | None = None
-    y: np.dtype[Any] | None = None
-    z: np.dtype[Any] | None = None
-    color: np.dtype[Any] | None = None
-    marker: np.dtype[Any] | None = None
-    size: np.dtype[Any] | None = None
-    text: np.dtype[Any] | None = None
-
-
-class DataDimension(str, Enum):
-    X = "x"
-    Y = "y"
-    Z = "z"
-
-
 TRACE_DIMENSION_MAP = dict(
     zip(
         DataDimension,
         ["_".join((dimension.value, "values")) for dimension in DataDimension],
         strict=True,
     )
 )
 
+AGG_DIMENSION_TO_ERROR_DIMENSION = dict(
+    zip(
+        DataDimension,
+        ["_".join(("error", dimension.value)) for dimension in DataDimension],
+        strict=True,
+    )
+)
+
+
 F = TypeVar("F", bound=Callable[..., Any])
 
 
+class DataTypes(BaseModel):
+    x: np.dtype[Any] | None = None
+    y: np.dtype[Any] | None = None
+    z: np.dtype[Any] | None = None
+    color: np.dtype[Any] | None = None
+    marker: np.dtype[Any] | None = None
+    size: np.dtype[Any] | None = None
+    text: np.dtype[Any] | None = None
+
+
 class DataPointer(BaseModel):
     x: str | None = None
     y: str | None = None
     z: str | None = None
     slicer: str | None = None
     shaded_error: str | None = None
     error_x: str | None = None
@@ -116,47 +125,42 @@
     error_z: str | None = None
     color: str | None = None
     marker: str | None = None
     opacity: str | float | None = None
     size: str | float | None = None
     text: str | None = None
 
-    @model_validator(mode="after")  # type: ignore
-    def check_missing_dimension(cls, model: "DataPointer") -> "DataPointer":
-        if model.x is None and model.y is None:
-            raise ValueError("Both x and y dimensions can not be None")
-        return model
+    @model_validator(mode="after")
+    def check_missing_dimension(self) -> DataPointer:
+        if self.x is None and self.y is None:
+            raise ValueError("Both `x` and `y` dimensions can not be None")
+        return self
 
     @property
     def text_identifiers(self) -> list[str] | None:
         if self.text is not None:
             return self.text.split("+")
         return None
 
 
 class DataHandler(BaseModel):
     data: pd.DataFrame
     data_pointer: DataPointer
     slice_order: list[Any] | None = None
     slice_logical_indices: dict[str, Any] | None = None
 
-    @model_validator(mode="before")
-    def check_pointers_in_data(cls, values: dict[str, Any]) -> dict[str, Any]:
-        data_pointer = values.get("data_pointer")
-        data = values.get("data")
-        if not isinstance(data, pd.DataFrame):
-            raise ValueError(f"`data` must be a `DataFrame`, got {type(data)}")
-
+    @model_validator(mode="after")
+    def check_pointers_in_data(self) -> DataHandler:
         for dimension in DataDimension:
             if (
-                pointer := getattr(data_pointer, dimension)
-            ) is not None and pointer not in data.columns:
-                raise ValueError(f"{pointer} is not present in {data.columns}")
-        values.update({"data": data})
-        return values
+                pointer := getattr(self.data_pointer, dimension)
+            ) is not None and pointer not in self.data.columns:
+                raise ValueError(f"{pointer} is not present in {self.data.columns}")
+
+        return self
 
     @field_validator("data")
     def check_dataframe_format(cls, value: pd.DataFrame) -> pd.DataFrame:
         if len(value.columns.names) > 1:
             raise ValueError(
                 "Multi-indexed columns are not supported, flatten the header before calling"
                 " statsplotly"
@@ -190,43 +194,43 @@
         for pointer, variable in self.data_pointer.model_dump().items():
             if variable in self.data.columns:
                 data_types[pointer] = dtypes.loc[variable]
 
         return DataTypes.model_validate(data_types)
 
     @property
-    def slicer_groupby_data(self) -> pd.DataFrame | pd.Grouper:
+    def _slicer_groupby_data(self) -> pd.DataFrame | pd.Grouper:
         if self.data_pointer.slicer is not None:
-            return self.data.groupby(self.data_pointer.slicer)
+            return self.data.groupby(self.data_pointer.slicer, sort=False)
         return self.data
 
     @staticmethod
     def _get_data_slice_indices(
         slice_ids: pd.Series, slice_order: list[str] | None
     ) -> dict[str, NDArray[Any]]:
         if slice_order is not None:
             if len(excluded_slices := set(slice_ids.unique()).difference(set(slice_order))) > 0:
                 logger.info(
                     f"{list(excluded_slices)} slices are not present in slices {slice_order} and"
                     " will not be plotted"
                 )
             slices = []
             for slice_id in slice_order:
-                if slice_id not in slice_ids.values:
+                if slice_id not in slice_ids.to_numpy():
                     raise ValueError(
                         f"Invalid slice identifier: '{slice_id}' could not be found in"
                         f" '{slice_ids.name}'"
                     )
                 slices.append(str(slice_id))
         else:
             slices = slice_ids.dropna().unique().astype(str)
 
         logical_indices: dict[str, NDArray[Any]] = {}
         for slice_id in slices:
-            logical_indices[slice_id] = (slice_ids.astype(str) == slice_id).values
+            logical_indices[slice_id] = (slice_ids.astype(str) == slice_id).to_numpy()
 
         return logical_indices
 
     @staticmethod
     def to_dataframe(function: F) -> pd.DataFrame:
         @wraps(function)
         def wrapper(*args: Any, **kwargs: Any) -> pd.DataFrame:
@@ -239,15 +243,15 @@
 
     @classmethod
     def build_handler(
         cls,
         data: pd.DataFrame,
         data_pointer: DataPointer,
         slice_order: list[str] | None = None,
-    ) -> "DataHandler":
+    ) -> DataHandler:
         slice_logical_indices = None
 
         data = data.reset_index()
         if data_pointer.slicer is not None:
             data = data.dropna(subset=data_pointer.slicer)
             slice_logical_indices = cls._get_data_slice_indices(
                 slice_ids=data[data_pointer.slicer], slice_order=slice_order
@@ -260,94 +264,96 @@
         )
 
     @to_dataframe
     def get_mean(self, dimension: str) -> pd.DataFrame:
         def std(x: pd.Series) -> list[float]:
             return [x.mean() - x.std(), x.mean() + x.std()]
 
-        return self.slicer_groupby_data[getattr(self.data_pointer, dimension)].agg([np.mean, std])
+        return self._slicer_groupby_data[getattr(self.data_pointer, dimension)].agg([np.mean, std])
 
     @to_dataframe
     def get_median(self, dimension: str) -> pd.DataFrame:
         def iqr(x: pd.Series) -> list[float]:
             return np.quantile(x, constants.IQR, axis=0).tolist()
 
-        return self.slicer_groupby_data[getattr(self.data_pointer, dimension)].agg([np.median, iqr])
+        return self._slicer_groupby_data[getattr(self.data_pointer, dimension)].agg(
+            [np.median, iqr]
+        )
 
     def get_data(self, dimension: str) -> pd.Series | None:
         if (dimension_pointer := getattr(self.data_pointer, dimension)) is None:
             return None
         if dimension_pointer not in self.data.columns:
             return None
         return self.data[dimension_pointer]
 
-    def slices_data(
+    def iter_slices(
         self,
     ) -> Generator[tuple[str, pd.DataFrame], None, None]:
         levels: list[str] = self.slice_levels or (
-            [self.data_pointer.y] if self.data_pointer.y is not None else [""]
+            [self.data_pointer.y]
+            if self.data_pointer.y is not None
+            else [self.data_pointer.x or ""]
         )
         for level in levels:
             trace_data = (
                 self.data.loc[self.slice_logical_indices[level]]
                 if self.slice_logical_indices is not None
                 else self.data
             )
             yield level, trace_data
 
 
 class DataProcessor(BaseModel):
-    x_values_mapping: dict[str, Any] | None = None
+    data_values_map: dict[DataDimension, dict[str, Any]] | None = None
     jitter_settings: dict[DataDimension, float] | None = None
     normalizer: dict[DataDimension, NormalizationType] | None = None
 
     @field_validator("normalizer", mode="before")
     def check_normalizer(
         cls, value: dict[DataDimension, Any]
     ) -> dict[DataDimension, NormalizationType]:
         validated_norm: dict[DataDimension, NormalizationType] = {}
         for dimension, normalization in value.items():
             if normalization is not None:
-                try:
-                    validated_norm.update({dimension: NormalizationType(normalization)})
-                except ValueError as exc:
-                    raise StatsPlotInvalidArgumentError(
-                        normalization, NormalizationType  # type: ignore
-                    ) from exc
+                validated_norm.update({dimension: normalization})
 
         return validated_norm
 
     @staticmethod
     def jitter_data(data_series: pd.Series, jitter_amount: float) -> pd.Series:
         if jitter_amount == 0:
             return data_series
-        jittered_data = pd.Series(rand_jitter(data_series, jitter_amount), name=data_series.name)
-        return jittered_data
+
+        return pd.Series(rand_jitter(data_series, jitter_amount), name=data_series.name)
 
     @staticmethod
     def normalize_data(data_series: pd.Series, normalizer: NormalizationType) -> pd.Series:
         match normalizer:
             case NormalizationType.CENTER:
                 return data_series - data_series.mean()
             case NormalizationType.MIN_MAX:
                 return pd.Series(
-                    range_normalize(data_series.values, 0, 1),
+                    range_normalize(data_series.to_numpy(), 0, 1),
                     name=data_series.name,
                 )
             case NormalizationType.ZSCORE:
                 return pd.Series(
-                    sc.stats.zscore(data_series.values, nan_policy="omit"),
+                    sc.stats.zscore(data_series.to_numpy(), nan_policy="omit"),
                     name=data_series.name,
                 )
 
     def process_trace_data(self, trace_data: dict[str, pd.Series]) -> pd.Series:
-        if self.x_values_mapping is not None:
-            trace_data[TRACE_DIMENSION_MAP[DataDimension.X]] = trace_data[
-                TRACE_DIMENSION_MAP[DataDimension.X]
-            ].map(lambda x: self.x_values_mapping[x])
+        if self.data_values_map is not None:
+            for dimension, values_map in self.data_values_map.items():
+                trace_data[TRACE_DIMENSION_MAP[dimension]] = (
+                    trace_data[TRACE_DIMENSION_MAP[dimension]]
+                    .astype(str)
+                    .map(lambda x, values_map=values_map: values_map[x])
+                )
 
         if self.normalizer is not None:
             for dimension, normalizer in self.normalizer.items():
                 if normalizer is None:
                     continue
                 try:
                     trace_data[TRACE_DIMENSION_MAP[dimension]] = self.normalize_data(
@@ -374,70 +380,90 @@
                         f" {trace_data[TRACE_DIMENSION_MAP[dimension]].dtype} can not be jittered"
                     )
 
         return trace_data
 
 
 class AggregationSpecifier(BaseModel):
-    aggregation_func: AggregationType | None = None
-    error_bar: ErrorBarType | None = None
+    aggregation_func: AggregationType | Callable[[Any], float] | None = None
+    aggregated_dimension: DataDimension
+    error_bar: ErrorBarType | Callable[[Any], NDArray[Any]] | None = None
     data_types: DataTypes
     data_pointer: DataPointer
 
-    @field_validator("aggregation_func", mode="before")
-    def check_aggregation_func(cls, value: str | None) -> AggregationType | None:
-        try:
-            return AggregationType(value) if value is not None else None
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, AggregationType) from exc  # type: ignore
-
-    @field_validator("error_bar", mode="before")
-    def check_error_bar(cls, value: str | None, info: ValidationInfo) -> ErrorBarType | None:
+    @field_validator("error_bar")
+    def check_error_bar(
+        cls, value: ErrorBarType | None, info: ValidationInfo
+    ) -> ErrorBarType | None:
         if value is not None and (
             (agg_func := info.data.get("aggregation_func")) is None
             or agg_func is AggregationType.COUNT
         ):
             raise StatsPlotSpecificationError(
-                f"Error bar requires one of "
+                f"Plotting error bar requires one of "
                 f"{[member.value for member in AggregationType if member is not AggregationType.COUNT]} "  # noqa: E501
                 f"aggregation function"
             )
-        try:
-            return ErrorBarType(value) if value is not None else None
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, ErrorBarType) from exc  # type: ignore
-
-    @field_validator("data_pointer")
-    def check_data_pointer(cls, value: DataPointer, info: ValidationInfo) -> DataPointer:
-        # x dimension
-        if value.x is None:
-            value.x = "index"
+        return value
+
+    @model_validator(mode="after")
+    def check_aggregation_specifier(self) -> AggregationSpecifier:
+        if (aggregation_func := self.aggregation_func) is not None:
+            if getattr(self.data_pointer, self.aggregated_dimension) is None:
+                raise StatsPlotSpecificationError(
+                    f"aggregation dimension `{self.aggregated_dimension}` not found in the data"
+                )
 
-        if (aggregation_func := info.data.get("aggregation_func")) is not None:
             # text can not be displayed along aggregation trace
-            if value.text is not None:
+            if self.data_pointer.text is not None:
                 logger.warning("Text data can not be displayed along aggregated data")
-            # y dimension
-            if value.y is None and aggregation_func is not AggregationType.COUNT:
-                raise StatsPlotSpecificationError(f"{aggregation_func} aggregation requires y data")
-            if value.y is not None:
-                if aggregation_func is AggregationType.COUNT:
-                    raise StatsPlotSpecificationError(
-                        f"{aggregation_func.value} aggregation does not apply to y data"
-                    )
 
-                if (dtypes := info.data.get("data_types")) is None:
-                    raise ValueError("`data_type` can not be `None`")
-                if not is_numeric_dtype(y_dtype := dtypes.y):
+            if aggregation_func is AggregationType.COUNT:
+                if (
+                    sum(
+                        [
+                            dimension is not None
+                            for dimension in [self.data_pointer.x, self.data_pointer.y]
+                        ]
+                    )
+                    > 1
+                ):
                     raise StatsPlotSpecificationError(
-                        f"{aggregation_func.value} aggregation requires numeric type y data, got: "
-                        f"`{y_dtype}`"
+                        f"{aggregation_func.value} aggregation only applies to one dimension"
                     )
 
-        return value
+        return self
+
+    @property
+    def reference_dimension(self) -> DataDimension:
+        if self.aggregation_func is AggregationType.COUNT:
+            return self.aggregated_dimension
+        if self.aggregated_dimension is DataDimension.X:
+            return DataDimension.Y
+        return DataDimension.X
+
+    @property
+    def aggregation_plot_dimension(self) -> DataDimension:
+        if self.aggregation_func is AggregationType.COUNT:
+            return (
+                DataDimension.Y if self.aggregated_dimension is DataDimension.X else DataDimension.X
+            )
+        return self.aggregated_dimension
+
+    @property
+    def reference_data(self) -> str | None:
+        if self.aggregation_func is AggregationType.COUNT:
+            return self.aggregated_data
+        if self.reference_dimension is DataDimension.X:
+            return self.data_pointer.x
+        return self.data_pointer.y
+
+    @property
+    def aggregated_data(self) -> str:
+        return getattr(self.data_pointer, self.aggregated_dimension)
 
 
 class _BaseTraceData(BaseModel):
     x_values: pd.Series | None = None
     y_values: pd.Series | None = None
     z_values: pd.Series | None = None
     shaded_error: pd.Series | None = None
@@ -451,15 +477,20 @@
     opacity_data: float | pd.Series | None = None
 
     @field_validator("error_x", "error_y", "error_z")
     def check_error_data(cls, value: pd.Series | None) -> pd.Series | None:
         if value is None:
             return value
 
-        if not all(value.apply(lambda x: np.issubdtype(np.asarray(x).dtype, np.number))):
+        if not all(
+            value.apply(
+                lambda x: np.issubdtype(np.asarray(x).dtype, np.number)
+                or any(xx is None for xx in x)
+            )
+        ):
             raise ValueError(f"{value.name} error data must be numeric")
 
         if not all(value.apply(lambda x: len(x) == 2)):  # noqa: PLR2004
             raise ValueError(
                 f"{value.name} error data must be bidirectional to be plotted relative to the"
                 " underlying data"
             )
@@ -510,51 +541,52 @@
         trace_data["text_data"] = cls.assemble_hover_text(
             data=data, text_pointers=pointer.text_identifiers
         )
         trace_data["color_data"] = (
             data[pointer.color] if pointer.color in data.columns else pointer.color
         )
         trace_data["size_data"] = (
-            data[[pointer.size]]
-            .apply(
-                lambda x: range_normalize(x, constants.MIN_MARKER_SIZE, constants.MAX_MARKER_SIZE)
+            range_normalize(
+                data[pointer.size], constants.MIN_MARKER_SIZE, constants.MAX_MARKER_SIZE
             )
-            .squeeze()
             if pointer.size in data.columns
             else pointer.size
         )
         trace_data["opacity_data"] = (
-            data[pointer.opacity] if pointer.opacity in data.columns else pointer.opacity
+            range_normalize(data[pointer.opacity], 0, 1)
+            if pointer.opacity in data.columns
+            else pointer.opacity
         )
 
         return trace_data
 
 
 class TraceData(_BaseTraceData):
     @classmethod
     def build_trace_data(
         cls,
         data: pd.DataFrame,
         pointer: DataPointer,
         processor: DataProcessor | None = None,
-    ) -> "TraceData":
+    ) -> TraceData:
         trace_data = cls._build_trace_data_from_pointer(data, pointer)
         if processor is not None:
             trace_data = processor.process_trace_data(trace_data)
 
         return cls.model_validate(trace_data)
 
 
 class AggregationTraceData(TraceData):
+
     @classmethod
     def _compute_error_bar(
         cls,
         data_group: pd.Grouper,
         agg_function: F,
-        error_bar: ErrorBarType,
+        error_bar: ErrorBarType | Callable[[Any], NDArray[Any]],
     ) -> pd.Series:
         if error_bar in (ErrorBarType.STD, ErrorBarType.SEM):
             data_agg = data_group.apply(agg_function)
             match error_bar:
                 case ErrorBarType.STD:
                     error_data = data_group.std()
 
@@ -564,14 +596,22 @@
                     )
 
             return pd.Series(
                 zip(data_agg - error_data, data_agg + error_data, strict=True),
                 name=data_agg.name,
             )
 
+        if error_bar is ErrorBarType.GEO_STD:
+            data_agg = data_group.apply(agg_function)
+            error_data = data_group.apply(lambda series: np.exp(np.std(np.log(series))))
+            return pd.Series(
+                zip(data_agg / error_data, data_agg * error_data, strict=True),
+                name=data_agg.name,
+            )
+
         if error_bar is ErrorBarType.IQR:
             return data_group.apply(lambda series: np.quantile(series, constants.IQR))
 
         if error_bar is ErrorBarType.BOOTSTRAP:
             # bootstrap accepts a sequence of data
             return data_group.apply(
                 lambda x: np.array(
@@ -579,68 +619,102 @@
                         (x,),
                         agg_function,
                         confidence_level=1 - constants.CI_ALPHA,
                     ).confidence_interval
                 )
             )
 
+        if isinstance(error_bar, Callable):  # type: ignore
+            return data_group.apply(error_bar)
+
         raise StatsPlotMissingImplementationError(f"Unsupported error bar type: {error_bar}")
 
     @classmethod
     def _build_aggregation_data_from_pointer(
         cls,
         data: pd.DataFrame,
         aggregation_specifier: AggregationSpecifier,
     ) -> dict[str, Any]:
         trace_data: dict[str, Any] = {}
-        if (x := aggregation_specifier.data_pointer.x) is None:
-            raise ValueError("`aggregation_specifier.data_pointer.x` can not be `None`")
-        y = aggregation_specifier.data_pointer.y
 
-        trace_data["x_values"] = pd.Series(np.sort(data[x].unique()), name=x)
+        trace_data[TRACE_DIMENSION_MAP[aggregation_specifier.reference_dimension]] = pd.Series(
+            data[aggregation_specifier.reference_data].unique(),
+            name=aggregation_specifier.reference_data,
+        )
         if (
             aggregation_specifier.aggregation_func is AggregationType.COUNT
             or aggregation_specifier.aggregation_func is AggregationType.PROBABILITY
             or aggregation_specifier.aggregation_func is AggregationType.PERCENT
         ):
-            _y_values: list[NDArray[Any]] = []
-            for x_value in trace_data["x_values"]:
-                y_value = (data[x] == x_value).sum()
+            _aggregated_values: list[NDArray[Any]] = []
+            for reference_value in trace_data[
+                TRACE_DIMENSION_MAP[aggregation_specifier.reference_dimension]
+            ]:
+                aggregated_value = (
+                    data[aggregation_specifier.reference_data] == reference_value
+                ).sum()
                 if aggregation_specifier.aggregation_func is AggregationType.PROBABILITY:
-                    _y_values.append(y_value / data[x].notnull().sum())
+                    _aggregated_values.append(
+                        aggregated_value
+                        / data[aggregation_specifier.reference_data].notnull().sum()
+                    )
                 elif aggregation_specifier.aggregation_func is AggregationType.PERCENT:
-                    _y_values.append(y_value / data[x].notnull().sum() * 100)
+                    _aggregated_values.append(
+                        aggregated_value
+                        / data[aggregation_specifier.reference_data].notnull().sum()
+                        * 100
+                    )
                 else:
-                    _y_values.append(y_value)
-            trace_data["y_values"] = pd.Series(
-                _y_values,
-                name="_".join((x, aggregation_specifier.aggregation_func.value)),
+                    _aggregated_values.append(aggregated_value)
+            trace_data[TRACE_DIMENSION_MAP[aggregation_specifier.aggregation_plot_dimension]] = (
+                pd.Series(
+                    _aggregated_values,
+                    name="_".join(
+                        (
+                            aggregation_specifier.aggregated_dimension,
+                            aggregation_specifier.aggregation_func.value,
+                        )
+                    ),
+                )
             )
 
         else:
-            agg_func: Callable[[Any], Any]
-            match aggregation_specifier.aggregation_func:
-                case AggregationType.MEAN:
-                    agg_func = np.mean
-                case AggregationType.MEDIAN:
-                    agg_func = np.median
-                case AggregationType.SUM:
-                    agg_func = np.sum
-
-            trace_data["y_values"] = data.groupby(x)[y].apply(agg_func)
+            if isinstance(aggregation_specifier.aggregation_func, AggregationType):
+                agg_func: Callable[[Any], Any]
+                match aggregation_specifier.aggregation_func:
+                    case AggregationType.MEAN:
+                        agg_func = np.mean
+                    case AggregationType.GEO_MEAN:
+                        agg_func = sc.stats.mstats.gmean
+                    case AggregationType.MEDIAN:
+                        agg_func = np.median
+                    case AggregationType.SUM:
+                        agg_func = np.sum
+            else:
+                agg_func = aggregation_specifier.aggregation_func  # type: ignore
+
+            trace_data[TRACE_DIMENSION_MAP[aggregation_specifier.aggregated_dimension]] = (
+                data.groupby(aggregation_specifier.reference_data, sort=False)[
+                    aggregation_specifier.aggregated_data
+                ].apply(agg_func)
+            )
 
             if aggregation_specifier.error_bar is not None:
-                trace_data["error_y"] = cls._compute_error_bar(
-                    data.groupby(x)[y],
+                trace_data[
+                    AGG_DIMENSION_TO_ERROR_DIMENSION[aggregation_specifier.aggregated_dimension]
+                ] = cls._compute_error_bar(
+                    data.groupby(aggregation_specifier.reference_data, sort=False)[
+                        aggregation_specifier.aggregated_data
+                    ],
                     agg_func,
                     aggregation_specifier.error_bar,
                 )
 
         return trace_data
 
     @classmethod
     def build_aggregation_trace_data(
         cls, data: pd.DataFrame, aggregation_specifier: AggregationSpecifier
-    ) -> "AggregationTraceData":
+    ) -> AggregationTraceData:
         trace_data = cls._build_aggregation_data_from_pointer(data, aggregation_specifier)
 
         return cls.model_validate(trace_data)
```

### Comparing `statsplotly-0.1.5/statsplotly/plot_specifiers/layout.py` & `statsplotly-0.2.0/statsplotly/plot_specifiers/layout/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,76 @@
+from __future__ import annotations
+
 import logging
 from enum import Enum
 from typing import Any
 
 import numpy as np
 from dateutil.parser import parse as parse_date
-from pydantic import BaseModel, field_validator, model_validator
+from pydantic import BaseModel, field_validator
 
 from statsplotly import constants
-from statsplotly.exceptions import StatsPlotInvalidArgumentError
+from statsplotly.plot_specifiers.common import smart_legend, smart_title
 from statsplotly.plot_specifiers.data import (
     AggregationType,
     DataDimension,
     DataPointer,
     ErrorBarType,
     HistogramNormType,
     TraceData,
 )
-from statsplotly.utils.layout_utils import smart_legend, smart_title
 
 logger = logging.getLogger(__name__)
 
 
+class PlotAxis(str, Enum):
+    XAXIS = "xaxis"
+    YAXIS = "yaxis"
+    COLORAXIS = "coloraxis"
+
+
+class ColoraxisReference(str, Enum):
+    MAIN_COLORAXIS = "coloraxis"
+
+
+class HistogramBarMode(str, Enum):
+    STACK = "stack"
+    OVERLAY = "overlay"
+
+
 class BarMode(str, Enum):
     STACK = "stack"
     GROUP = "group"
     OVERLAY = "overlay"
     RELATIVE = "relative"
 
 
 class AxisFormat(str, Enum):
     SQUARE = "square"
     FIXED_RATIO = "fixed_ratio"
     EQUAL = "equal"
     ID_LINE = "id_line"
 
 
-class ColoraxisReference(str, Enum):
-    MAIN_COLORAXIS = "coloraxis"
+class AxisType(str, Enum):
+    TWO_DIMENSIONAL = "two_dimensional"
+    THREE_DIMENSIONAL = "three_dimensional"
 
 
 class LegendSpecifier(BaseModel):
     data_pointer: DataPointer
     x_transformation: AggregationType | HistogramNormType | None = None
     y_transformation: AggregationType | HistogramNormType | None = None
     title: str | None = None
     x_label: str | None = None
     y_label: str | None = None
     z_label: str | None = None
     error_bar: str | None = None
-
-    @model_validator(mode="before")
-    def check_y_label(cls, values: dict[str, Any]) -> dict[str, Any]:
-        data_pointer, y_transformation, y_label = (
-            values.get("data_pointer"),
-            values.get("y_transformation"),
-            values.get("y_label"),
-        )
-        if data_pointer is None:
-            raise ValueError("`data_pointer` can not be `None`")
-        if data_pointer.y is None and y_transformation is None and y_label is None:
-            raise ValueError(
-                "No y_label provided for the legend, check"
-                f" {LegendSpecifier.__name__} specification"
-            )
-        return values
+    shaded_error: str | None = None
+    axis_type: AxisType | None = None
 
     def _get_axis_title_from_dimension_pointer(self, dimension: DataDimension) -> str:
         pointer_label = getattr(self.data_pointer, dimension) or ""
         if dimension is DataDimension.X:
             return f"{pointer_label} {self.x_transformation_legend or ''}"
         if dimension is DataDimension.Y:
             return f"{pointer_label} {self.y_transformation_legend or ''}"
@@ -91,131 +94,146 @@
             self.x_transformation.value
             if self.x_transformation is not HistogramNormType.COUNT
             else "count"
         )
 
     @property
     def xaxis_title(self) -> str:
-        return smart_legend(
-            self.x_label or self._get_axis_title_from_dimension_pointer(DataDimension.X)
+        return self.x_label or smart_legend(
+            self._get_axis_title_from_dimension_pointer(DataDimension.X)
         )
 
     @property
     def yaxis_title(self) -> str:
-        return smart_legend(
-            self.y_label or self._get_axis_title_from_dimension_pointer(DataDimension.Y)
+        return self.y_label or smart_legend(
+            self._get_axis_title_from_dimension_pointer(DataDimension.Y)
         )
 
     @property
     def zaxis_title(self) -> str | None:
         if self.data_pointer.z is None:
             return None
-        return smart_legend(
-            self.z_label or self._get_axis_title_from_dimension_pointer(DataDimension.Z)
+        return self.z_label or smart_legend(
+            self._get_axis_title_from_dimension_pointer(DataDimension.Z)
         )
 
     @property
-    def figure_title(self) -> str:  # noqa: PLR0912
+    def figure_title(self) -> str:  # noqa: C901, PLR0912
         if self.title is not None:
             return self.title
 
-        if self.y_transformation is not None:
-            if self.data_pointer.y is not None:
-                title = (
-                    f"{self.data_pointer.y} {self.y_transformation_legend} vs {self.data_pointer.x}"
-                )
-            else:
-                title = f"{self.data_pointer.x} {self.y_transformation_legend}"
-        elif self.x_transformation is not None:
-            if self.data_pointer.x is not None:
-                title = (
-                    f"{self.data_pointer.x} {self.x_transformation_legend} vs {self.data_pointer.y}"
-                )
-            else:
-                title = f"{self.data_pointer.y} {self.x_transformation_legend}"
-        else:
-            title = f"{self.data_pointer.y} vs {self.data_pointer.x}"
+        x_bit_title = f"{self.data_pointer.x or ''} {self.x_transformation_legend or ''}"
+        y_bit_title = f"{self.data_pointer.y or ''} {self.y_transformation_legend or ''}"
+        title_bits = [bit.strip() for bit in [y_bit_title, x_bit_title] if bit.strip()]
+        title = " vs ".join(title_bits)
 
         if self.data_pointer.z is not None:
-            title = f"{title} vs {self.data_pointer.z}"
+            if self.axis_type is AxisType.THREE_DIMENSIONAL:
+                title = f"{title} vs {self.data_pointer.z}"
+            else:
+                title = f"{title} {self.data_pointer.z}"
+
         if self.data_pointer.slicer is not None:
             title = f"{title} per {self.data_pointer.slicer}"
         if self.error_bar is not None:
             if self.error_bar in (ErrorBarType.SEM, ErrorBarType.BOOTSTRAP):
                 title = f"{title} ({(1 - constants.CI_ALPHA) * 100}% CI {self.error_bar})"
             else:
                 title = f"{title} ({self.error_bar})"
+        if self.shaded_error is not None:
+            title = f"{title} (± {self.shaded_error})"
 
         return smart_title(title)
 
 
 class AxesSpecifier(BaseModel):
     axis_format: AxisFormat | None = None
     traces: list[TraceData]
     legend: LegendSpecifier
     x_range: list[float | str] | None = None
     y_range: list[float | str] | None = None
     z_range: list[float | str] | None = None
 
-    @field_validator("axis_format", mode="before")
-    def validate_axis_format(cls, value: str | None) -> AxisFormat | None:
-        try:
-            return AxisFormat(value) if value is not None else None
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, AxisFormat) from exc  # type: ignore
-
     @field_validator("x_range", "y_range", "z_range")
     def validate_axis_range_format(
         cls, value: list[float | str] | None
     ) -> list[float | str] | None:
         if value is not None:
             try:
                 [parse_date(limit) for limit in value if isinstance(limit, str)]
             except Exception as exc:
                 raise ValueError("Axis range must be numeric or `datetime`") from exc
         return value
 
+    @staticmethod
+    def pad_axis_range(axis_range: list[Any], padding_factor: float) -> list[Any]:
+        if axis_range[0] < 0:
+            axis_range[0] *= 1 + padding_factor
+        else:
+            axis_range[0] *= 1 - padding_factor
+
+        axis_range[1] *= 1 + padding_factor
+
+        return axis_range
+
     def get_axes_range(self) -> list[Any] | None:
-        values_span = np.concatenate([
-            data
-            for trace in self.traces
-            for data in [trace.x_values, trace.y_values, trace.z_values]
-            if data is not None
-        ])
+        values_span = np.concatenate(
+            [
+                data
+                for trace in self.traces
+                for data in [trace.x_values, trace.y_values, trace.z_values]
+                if data is not None
+            ]
+        )
         axes_span = [
             axis_span
             for axis_span in [self.x_range, self.y_range, self.z_range]
             if axis_span is not None
         ]
         try:
             if len(axes_span) > 0:
-                return [
+                min_value, max_value = (
                     np.max([np.min(values_span), np.min(axes_span)]),
                     np.min([np.max(values_span), np.max(axes_span)]),
-                ]
-            return [np.min(values_span), np.max(values_span)]
+                )
+
+            else:
+                min_value, max_value = np.min(values_span), np.max(values_span)
+
         except TypeError:
-            logger.debug("Can not calculate a common range for axes")
+            logger.debug(
+                f"Can not calculate a common range for values of type = '{values_span.dtype}'"
+            )
             return None
 
+        else:
+            try:
+                return self.pad_axis_range(
+                    [min_value, max_value], padding_factor=constants.RANGE_PADDING_FACTOR
+                )
+
+            except TypeError:
+                logger.debug(
+                    f"Can not pad a common range for values of type = '{values_span.dtype}'"
+                )
+                return [min_value, max_value]
+
     @property
     def height(self) -> int | None:
         if self.axis_format in (
             AxisFormat.SQUARE,
-            AxisFormat.EQUAL,
             AxisFormat.ID_LINE,
         ):
             return constants.AXES_HEIGHT
         return None
 
     @property
     def width(self) -> int | None:
         if self.axis_format in (
             AxisFormat.SQUARE,
-            AxisFormat.EQUAL,
             AxisFormat.ID_LINE,
         ):
             return constants.AXES_WIDTH
         return None
 
     @property
     def xaxis_range(self) -> list[Any] | None:
@@ -236,16 +254,16 @@
         if self.axis_format is AxisFormat.EQUAL:
             return self.get_axes_range()
 
         return self.z_range
 
     @property
     def scaleratio(self) -> float | None:
-        if self.axis_format in (AxisFormat.FIXED_RATIO, AxisFormat.EQUAL):
+        if self.axis_format in (AxisFormat.FIXED_RATIO, AxisFormat.EQUAL, AxisFormat.ID_LINE):
             return 1
         return None
 
     @property
     def scaleanchor(self) -> str | None:
-        if self.axis_format in (AxisFormat.FIXED_RATIO, AxisFormat.EQUAL):
+        if self.axis_format in (AxisFormat.FIXED_RATIO, AxisFormat.EQUAL, AxisFormat.ID_LINE):
             return "x"
         return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `statsplotly-0.1.5/statsplotly/plot_specifiers/trace.py` & `statsplotly-0.2.0/statsplotly/plot_specifiers/trace.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,42 @@
+from __future__ import annotations
+
 import logging
 from collections.abc import Callable
 from enum import Enum
 from functools import wraps
 from typing import Any, TypeVar, cast
 
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
 from pandas.api.types import is_numeric_dtype
-from pydantic import field_validator
-from pydantic_core.core_schema import ValidationInfo
+from pydantic import ValidationInfo, field_validator, model_validator
 
 from statsplotly import constants
-from statsplotly.exceptions import (
-    StatsPlotInvalidArgumentError,
-    StatsPlotSpecificationError,
-)
+from statsplotly._base import BaseModel
+from statsplotly.exceptions import StatsPlotSpecificationError
 from statsplotly.plot_specifiers.data import (
-    BaseModel,
     CentralTendencyType,
     DataDimension,
+    DataHandler,
+    DataTypes,
     HistogramNormType,
     RegressionType,
     TraceData,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class TraceMode(str, Enum):
     MARKERS = "markers"
     LINES = "lines"
     MARKERS_LINES = "markers+lines"
+    LINES_TEXT = "lines+text"
 
 
 class CategoricalPlotType(str, Enum):
     STRIP = "stripplot"
     VIOLIN = "violinplot"
     BOX = "boxplot"
 
@@ -51,51 +52,120 @@
     KDE = "kde"
     SCATTER_KDE = "scatter+kde"
     X_HISTMAP = "x_histmap"
     Y_HISTMAP = "y_histmap"
     HISTOGRAM = "histogram"
 
 
-TS = TypeVar("TS", bound="_TraceSpecifier")
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 class _TraceSpecifier(BaseModel):
     @staticmethod
     def remove_nans(function: F) -> F:
         @wraps(function)
-        def wrapper(self: type[TS], data: pd.Series, *args: Any, **kwargs: Any) -> F:
+        def wrapper(self: _TraceSpecifier, data: pd.Series, *args: Any, **kwargs: Any) -> F:
             return function(self, data.dropna(), *args, **kwargs)
 
         return cast(F, wrapper)
 
 
-class ScatterSpecifier(_TraceSpecifier):
+class _XYTraceValidator(BaseModel):
+    data_types: DataTypes
+
+    @model_validator(mode="after")
+    def validate_model(self) -> _XYTraceValidator:
+        if not (self.data_types.x is not None and self.data_types.y is not None):
+            raise StatsPlotSpecificationError(
+                f"Both `x` and `y`dimensions must be supplied for {self.__class__.__name__}"
+            )
+        return self
+
+
+class PlotOrientation(str, Enum):
+    HORIZONTAL = "horizontal"
+    VERTICAL = "vertical"
+
+
+class OrientedPlotSpecifier(BaseModel):
+    prefered_orientation: PlotOrientation | None = None
+    data_types: DataTypes
+
+    @property
+    def orientation(self) -> PlotOrientation:
+        if self.data_types.x is None:
+            return PlotOrientation.HORIZONTAL
+        if self.data_types.y is None:
+            return PlotOrientation.VERTICAL
+        if self.prefered_orientation is not None:
+            return self.prefered_orientation
+        if is_numeric_dtype(self.data_types.x):
+            return PlotOrientation.HORIZONTAL
+        return PlotOrientation.VERTICAL
+
+    @property
+    def anchor_dimension(self) -> DataDimension:
+        if self.orientation is PlotOrientation.VERTICAL:
+            return DataDimension.X
+        return DataDimension.Y
+
+    @property
+    def anchored_dimension(self) -> DataDimension | None:
+        if self.data_types.x is None or self.data_types.y is None:
+            return None
+        if self.anchor_dimension is DataDimension.X:
+            return DataDimension.Y
+        return DataDimension.X
+
+
+class ScatterSpecifier(_TraceSpecifier, _XYTraceValidator):
     mode: TraceMode | None = None
     regression_type: RegressionType | None = None
 
-    @field_validator("mode", mode="before")
-    def check_mode(cls, value: str | None) -> TraceMode | None:
-        try:
-            return TraceMode(value) if value is not None else None
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, TraceMode) from exc  # type: ignore
-
-    @field_validator("regression_type", mode="before")
-    def check_regression_type(cls, value: str | None) -> RegressionType | None:
-        try:
-            return RegressionType(value) if value is not None else None
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, RegressionType) from exc  # type: ignore
+
+class CategoricalPlotSpecifier(OrientedPlotSpecifier, _TraceSpecifier, _XYTraceValidator):
+    plot_type: CategoricalPlotType
+
+    @field_validator("plot_type", mode="before")
+    def validate_plot_type(cls, value: str | None) -> CategoricalPlotType:
+        if value is None:
+            return CategoricalPlotType.STRIP
+        return CategoricalPlotType(value)
+
+    @model_validator(mode="after")
+    def validate_model(self) -> CategoricalPlotSpecifier:
+        if self.data_types.color is not None and self.plot_type is not CategoricalPlotType.STRIP:
+            raise StatsPlotSpecificationError(
+                f"Only slice-level color data can be specified with `{self.plot_type.value}`, got marker-level argument `color={self.data_types.color}`"
+            )
+        return self
+
+    def get_category_strip_map(
+        self, data_handler: DataHandler
+    ) -> dict[DataDimension, dict[str, Any]] | None:
+        categorical_data = data_handler.get_data(self.anchor_dimension)
+        if categorical_data is None:
+            raise StatsPlotSpecificationError(
+                f"Could not find `{self.anchor_dimension.value}` in data pointer"
+            )
+        if is_numeric_dtype(categorical_data):
+            return None
+
+        categorical_data_dict: dict[str, Any] = {}
+        for i, x_level in enumerate(np.sort(categorical_data.dropna().astype(str).unique()), 1):
+            categorical_data_dict[x_level] = i
+
+        return {self.anchor_dimension: categorical_data_dict}
 
 
 class HistogramSpecifier(_TraceSpecifier):
     hist: bool | None = None
     cumulative: bool | None = None
     step: bool | None = None
+    ecdf: bool | None = None
     kde: bool | None = None
     rug: bool | None = None
     histnorm: HistogramNormType
     bin_edges: NDArray[Any] | None = None
     bins: str | list[float] | int
     central_tendency: CentralTendencyType | None = None
     data_type: np.dtype[Any]
@@ -105,127 +175,145 @@
     def check_cumulative(cls, value: bool | None, info: ValidationInfo) -> bool | None:
         if value and not info.data.get("hist"):
             raise StatsPlotSpecificationError(
                 "Cumulative histogram requires histogram bins plotting"
             )
         return value
 
-    @field_validator("kde")
-    def check_kde(cls, value: bool | None, info: ValidationInfo) -> bool | None:
-        if value and info.data.get("cumulative"):
-            raise StatsPlotSpecificationError(
-                "KDE is incompatible with cumulative histogram plotting"
-            )
-        if value and info.data.get("step"):
-            raise StatsPlotSpecificationError("KDE is incompatible with step histogram plotting")
-        return value
-
-    @field_validator("bins")
+    @field_validator("bins", mode="before")
     def check_bins(cls, value: str | list[float] | int | None) -> str | list[float] | int:
         return value if value is not None else constants.DEFAULT_HISTOGRAM_BIN_COMPUTATION_METHOD
 
     @field_validator("histnorm", mode="before")
-    def check_histnorm(cls, value: str | None, info: ValidationInfo) -> HistogramNormType:
+    def check_histnorm(cls, value: str | None, info: ValidationInfo) -> str | None:
         if info.data.get("kde"):
             if value is None:
                 logger.info(
                     f"Setting histogram norm to {HistogramNormType.PROBABILITY_DENSITY.value} with"
                     " KDE plotting"
                 )
                 return HistogramNormType.PROBABILITY_DENSITY
 
-            if value is not HistogramNormType.PROBABILITY_DENSITY:
-                raise StatsPlotSpecificationError(
-                    "Histogram norm must be set to"
-                    f" {HistogramNormType.PROBABILITY_DENSITY.value} with KDE plotting, got {value}"
-                )
-        try:
-            return HistogramNormType(value) if value is not None else HistogramNormType.COUNT
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, HistogramNormType) from exc  # type: ignore
-
-    @field_validator("central_tendency")
-    def check_central_tendency(cls, value: str | None) -> CentralTendencyType | None:
-        try:
-            return CentralTendencyType(value) if value is not None else None
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, CentralTendencyType) from exc  # type: ignore
+        return value or HistogramNormType.COUNT
 
     @field_validator("dimension")
     def check_dimension(cls, value: DataDimension, info: ValidationInfo) -> DataDimension:
         if not is_numeric_dtype(dtype := info.data.get("data_type")):
             raise StatsPlotSpecificationError(
                 f"Distribution of {value} values of type: `{dtype}` can not be computed"
             )
         return value
 
+    @model_validator(mode="after")
+    def check_parameter_consistency(self: HistogramSpecifier) -> HistogramSpecifier:
+        if self.ecdf and self.histnorm is HistogramNormType.PROBABILITY_DENSITY:
+            raise StatsPlotSpecificationError(
+                "Histogram norm can not be set to"
+                f" {HistogramNormType.PROBABILITY_DENSITY.value} with ECDF plotting"
+            )
+
+        if self.kde:
+            if self.histnorm is not HistogramNormType.PROBABILITY_DENSITY:
+                raise StatsPlotSpecificationError(
+                    "Histogram norm must be set to"
+                    f" {HistogramNormType.PROBABILITY_DENSITY.value} with KDE plotting,"
+                    f" got `{self.histnorm.name}`"
+                )
+
+            if self.cumulative:
+                raise StatsPlotSpecificationError(
+                    "KDE is incompatible with cumulative histogram plotting"
+                )
+
+            if self.step:
+                raise StatsPlotSpecificationError(
+                    "KDE is incompatible with step histogram plotting"
+                )
+
+        return self
+
     @property
     def density(self) -> bool:
         return True if self.histnorm is HistogramNormType.PROBABILITY_DENSITY else False
 
+    def get_distribution_max_value(self, data: pd.Series) -> float:
+        dist_function: Callable[[Any], Any]
+        if self.ecdf:
+            dist_function = self.compute_ecdf
+        else:
+            dist_function = self.compute_histogram
+
+        return dist_function(data)[0].max()
+
     @_TraceSpecifier.remove_nans
-    def histogram_bin_edges(self, data: pd.Series) -> tuple[NDArray[Any], float]:
+    def get_histogram_bin_edges(self, data: pd.Series) -> tuple[NDArray[Any], float]:
         bin_edges = np.histogram_bin_edges(
             data,
             bins=self.bin_edges if self.bin_edges is not None else self.bins,
         )
         bin_size = np.round(
             bin_edges[1] - bin_edges[0], 6
         )  # Round to assure smooth binning by plotly
 
         return bin_edges, bin_size
 
     @_TraceSpecifier.remove_nans
-    def histogram(self, data: pd.Series) -> tuple[pd.Series, NDArray[Any], float]:
-        bin_edges, bin_size = self.histogram_bin_edges(data)
+    def compute_histogram(self, data: pd.Series) -> tuple[pd.Series, NDArray[Any], float]:
+        bin_edges, bin_size = self.get_histogram_bin_edges(data)
         hist, bin_edges = np.histogram(data, bins=bin_edges, density=self.density)
 
         # Normalize if applicable
         if (
             self.histnorm is HistogramNormType.PROBABILITY
             or self.histnorm is HistogramNormType.PERCENT
         ):
             hist = hist / sum(hist)
             if self.histnorm is HistogramNormType.PERCENT:
                 hist = hist * 100
 
+        if self.cumulative:
+            hist = np.cumsum(hist)
+
         return (
             pd.Series(hist, name=self.histnorm if len(self.histnorm) > 0 else "count"),
             bin_edges,
             bin_size,
         )
 
+    @_TraceSpecifier.remove_nans
+    def compute_ecdf(self, data: pd.Series) -> tuple[pd.Series, NDArray[Any]]:
+        unique_values, counts = np.unique(np.sort(data), return_counts=True)
+
+        cdf = np.cumsum(counts)
+
+        if (
+            self.histnorm is HistogramNormType.PROBABILITY
+            or self.histnorm is HistogramNormType.PERCENT
+        ):
+            cdf = cdf / data.size
+            if self.histnorm is HistogramNormType.PERCENT:
+                cdf = cdf * 100
+
+        return (
+            pd.Series(cdf, name=self.histnorm if len(self.histnorm) > 0 else "count"),
+            unique_values,
+        )
+
 
 class JointplotSpecifier(_TraceSpecifier):
     plot_type: JointplotType
     marginal_plot: MarginalPlotDimension | None = None
     histogram_specifier: dict[DataDimension, HistogramSpecifier] | None = None
     scatter_specifier: ScatterSpecifier
 
-    @field_validator("plot_type", mode="before")
-    def check_jointplot_type(cls, value: str) -> JointplotType:
-        try:
-            return JointplotType(value)
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(value, JointplotType) from exc  # type: ignore
-
-    @field_validator("marginal_plot", mode="before")
-    def check_marginal_plot(cls, value: str) -> MarginalPlotDimension | None:
-        try:
-            return MarginalPlotDimension(value) if value is not None else None
-        except ValueError as exc:
-            raise StatsPlotInvalidArgumentError(
-                value, MarginalPlotDimension  # type: ignore
-            ) from exc
-
     @field_validator("scatter_specifier")
     def check_scatter_specifier(
         cls, value: ScatterSpecifier, info: ValidationInfo
     ) -> ScatterSpecifier:
-        if value.regression_type is not None and (plot_type := info.data["plot_type"]) not in (
+        if value.regression_type is not None and (plot_type := info.data.get("plot_type")) not in (
             JointplotType.SCATTER,
             JointplotType.SCATTER_KDE,
         ):
             raise StatsPlotSpecificationError(
                 f"{value.regression_type.value} regression can not be displayed on a"
                 f" {plot_type} plot"
             )
@@ -259,16 +347,16 @@
     @_TraceSpecifier.remove_nans
     def histogram2d(
         self, data: pd.DataFrame
     ) -> tuple[pd.Series, tuple[NDArray[Any], NDArray[Any]], tuple[float, float]]:
         if self.histogram_specifier is None:
             raise ValueError("`histogram_specifier` can not be `None`")
         x, y = data.iloc[:, 0], data.iloc[:, 1]
-        xbin_edges, xbin_size = self.histogram_specifier[DataDimension.X].histogram_bin_edges(x)
-        ybin_edges, ybin_size = self.histogram_specifier[DataDimension.X].histogram_bin_edges(y)
+        xbin_edges, xbin_size = self.histogram_specifier[DataDimension.X].get_histogram_bin_edges(x)
+        ybin_edges, ybin_size = self.histogram_specifier[DataDimension.Y].get_histogram_bin_edges(y)
 
         hist, _, _ = np.histogram2d(
             x,
             y,
             bins=[xbin_edges, ybin_edges],
             density=self.histogram_specifier[DataDimension.X].density,
         )
@@ -305,21 +393,21 @@
             anchor_values, histogram_data = (
                 trace_data.y_values,
                 trace_data.x_values,
             )
             histogram_specifier = self.histogram_specifier[DataDimension.X].model_copy()
 
         # Get and set uniform bin edges along anchor values
-        bin_edges, bin_size = histogram_specifier.histogram_bin_edges(histogram_data)
+        bin_edges, bin_size = histogram_specifier.get_histogram_bin_edges(histogram_data)
         histogram_specifier.bin_edges = bin_edges
 
         # Initialize histogram array
         hist = np.zeros((len(anchor_values.unique()), len(bin_edges) - 1))
         for i, anchor_value in enumerate(anchor_values.unique()):
-            hist[i, :], _, _ = histogram_specifier.histogram(
+            hist[i, :], _, _ = histogram_specifier.compute_histogram(
                 histogram_data[anchor_values == anchor_value]
             )
 
         # Bin centers
         bin_centers = (bin_edges[1:] + bin_edges[:-1]) / 2
 
         return (
```

### Comparing `statsplotly-0.1.5/statsplotly/plotting/helpers.py` & `statsplotly-0.2.0/statsplotly/_plotting/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,176 +1,203 @@
 """Helper modules for plotting routines."""
 
-from plotly import graph_objs as go
+import plotly
 
-from statsplotly.plot_objects.trace_objects import (
-    BaseTrace,
+from statsplotly.plot_objects.trace import (
     ContourTrace,
+    EcdfTrace,
     HeatmapTrace,
     Histogram2dTrace,
     HistogramTrace,
     KdeTrace,
     RugTrace,
     ScatterTrace,
     StepHistogramTrace,
 )
 from statsplotly.plot_specifiers.color import ColorSpecifier
 from statsplotly.plot_specifiers.data import TraceData
+from statsplotly.plot_specifiers.layout import set_horizontal_colorbar
 from statsplotly.plot_specifiers.trace import (
     HistogramSpecifier,
     JointplotSpecifier,
     JointplotType,
     ScatterSpecifier,
 )
 
 
 def plot_jointplot_main_traces(
     trace_data: TraceData,
     trace_name: str,
     trace_color: str,
     color_specifier: ColorSpecifier,
     jointplot_specifier: JointplotSpecifier,
-) -> dict[str, BaseTrace]:
+) -> dict[str, plotly.basedatatypes.BaseTraceType]:
     """Constructs the main traces of a jointplot layout."""
 
-    traces: dict[str, BaseTrace] = {}
+    traces: dict[str, plotly.basedatatypes.BaseTraceType] = {}
     if jointplot_specifier.plot_kde:
         contour_trace = ContourTrace.build_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             color_specifier=color_specifier,
             jointplot_specifier=jointplot_specifier,
         )
-        traces[contour_trace.name] = go.Contour(contour_trace.model_dump())
+        traces[contour_trace.name] = contour_trace.to_plotly_trace()
 
     if jointplot_specifier.plot_type is JointplotType.HISTOGRAM:
         histogram_trace = Histogram2dTrace.build_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             trace_color=trace_color,
             color_specifier=color_specifier,
             jointplot_specifier=jointplot_specifier,
         )
-        traces[histogram_trace.name] = go.Histogram2d(histogram_trace.model_dump())
+        # Make colorbars horizontal
+        if histogram_trace.colorbar is not None:
+            histogram_trace.colorbar = set_horizontal_colorbar(histogram_trace.colorbar)
+
+        traces[histogram_trace.name] = histogram_trace.to_plotly_trace()
 
     if jointplot_specifier.plot_type in (
         JointplotType.X_HISTMAP,
         JointplotType.Y_HISTMAP,
     ):
         heatmap_trace = HeatmapTrace.build_histmap_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             color_specifier=color_specifier,
             jointplot_specifier=jointplot_specifier,
         )
-        traces[heatmap_trace.name] = go.Heatmap(heatmap_trace.model_dump())
+        # Make colorbars horizontal
+        # TODO: Get read of this one when we use _SubplotGridCommonColoraxisFormatter class for managing coloraxis
+        if heatmap_trace.colorbar is not None:
+            heatmap_trace.colorbar = set_horizontal_colorbar(heatmap_trace.colorbar)
+
+        traces[heatmap_trace.name] = heatmap_trace.to_plotly_trace()
 
     return traces
 
 
 def plot_scatter_traces(
     trace_data: TraceData,
     trace_name: str,
     trace_color: str,
     color_specifier: ColorSpecifier,
     scatter_specifier: ScatterSpecifier,
-) -> dict[str, BaseTrace]:
+) -> dict[str, plotly.basedatatypes.BaseTraceType]:
     """Constructs scatter traces."""
 
-    traces: dict[str, BaseTrace] = {}
-    traces[trace_name] = go.Scatter(
-        **ScatterTrace.build_trace(
-            trace_data=trace_data,
-            trace_name=trace_name,
-            trace_color=trace_color,
-            color_specifier=color_specifier,
-            mode=scatter_specifier.mode,
-        ).model_dump()
-    )
+    traces: dict[str, plotly.basedatatypes.BaseTraceType] = {}
+    traces[trace_name] = ScatterTrace.build_trace(
+        trace_data=trace_data,
+        trace_name=trace_name,
+        trace_color=trace_color,
+        color_specifier=color_specifier,
+        mode=scatter_specifier.mode,
+    ).to_plotly_trace()
 
     if trace_data.shaded_error is not None:
         upper_bound_trace = ScatterTrace.build_upper_error_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             trace_color=trace_color,
         )
-        traces[upper_bound_trace.name] = go.Scatter(**upper_bound_trace.model_dump())
+        traces[upper_bound_trace.name] = upper_bound_trace.to_plotly_trace()
 
         lower_bound_trace = ScatterTrace.build_lower_error_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             trace_color=trace_color,
         )
-        traces[lower_bound_trace.name] = go.Scatter(**lower_bound_trace.model_dump())
+        traces[lower_bound_trace.name] = lower_bound_trace.to_plotly_trace()
 
     if scatter_specifier.regression_type is not None:
         regression_trace = ScatterTrace.build_regression_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             trace_color=trace_color,
             regression_type=scatter_specifier.regression_type,
         )
-        traces[regression_trace.name] = go.Scatter(**regression_trace.model_dump())
+        traces[regression_trace.name] = regression_trace.to_plotly_trace()
 
     return traces
 
 
-def plot_marginal_traces(
+def plot_distplot_traces(
     trace_data: TraceData,
     trace_name: str,
     trace_color: str,
     color_specifier: ColorSpecifier,
     histogram_specifier: HistogramSpecifier,
-) -> dict[str, BaseTrace]:
-    """Constructs traces of marginal distributions."""
+) -> dict[str, plotly.basedatatypes.BaseTraceType]:
+    """Constructs distplot traces."""
 
-    traces: dict[str, BaseTrace] = {}
+    traces: dict[str, plotly.basedatatypes.BaseTraceType] = {}
     if histogram_specifier.dimension is None:
         raise ValueError("`histogram_specifier.dimension` can not be `None`")
 
     if histogram_specifier.hist:
+        hist_trace: StepHistogramTrace | HistogramTrace
         if histogram_specifier.step:
-            traces["_".join((trace_name, histogram_specifier.dimension))] = go.Scatter(
-                StepHistogramTrace.build_trace(
-                    trace_data=trace_data,
-                    trace_name=trace_name,
-                    trace_color=trace_color,
-                    color_specifier=color_specifier,
-                    histogram_specifier=histogram_specifier,
-                ).model_dump()
+            hist_trace = StepHistogramTrace.build_trace(
+                trace_data=trace_data,
+                trace_name=trace_name,
+                trace_color=trace_color,
+                color_specifier=color_specifier,
+                histogram_specifier=histogram_specifier,
             )
+
         else:
-            traces["_".join((trace_name, histogram_specifier.dimension))] = go.Histogram(
-                HistogramTrace.build_trace(
-                    trace_data=trace_data,
-                    trace_name=trace_name,
-                    trace_color=trace_color,
-                    color_specifier=color_specifier,
-                    histogram_specifier=histogram_specifier,
-                ).model_dump()
+            hist_trace = HistogramTrace.build_trace(
+                trace_data=trace_data,
+                trace_name=trace_name,
+                trace_color=trace_color,
+                color_specifier=color_specifier,
+                histogram_specifier=histogram_specifier,
             )
+        traces["_".join((hist_trace.name, histogram_specifier.dimension))] = (
+            hist_trace.to_plotly_trace()
+        )
+
+    if histogram_specifier.ecdf:
+        ecdf_trace = EcdfTrace.build_trace(
+            trace_data=trace_data,
+            trace_name=trace_name,
+            trace_color=trace_color,
+            color_specifier=color_specifier,
+            histogram_specifier=histogram_specifier,
+        )
+        traces["_".join((ecdf_trace.name, histogram_specifier.dimension))] = (
+            ecdf_trace.to_plotly_trace()
+        )
 
     if histogram_specifier.rug:
         rug_trace = RugTrace.build_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             trace_color=trace_color,
             color_specifier=color_specifier,
             histogram_specifier=histogram_specifier,
         )
-        traces["_".join((rug_trace.name, histogram_specifier.dimension))] = go.Scatter(
-            rug_trace.model_dump()
+        traces["_".join((rug_trace.name, histogram_specifier.dimension))] = (
+            rug_trace.to_plotly_trace()
         )
 
     if histogram_specifier.kde:
         kde_trace = KdeTrace.build_trace(
             trace_data=trace_data,
             trace_name=trace_name,
             trace_color=trace_color,
             color_specifier=color_specifier,
             histogram_specifier=histogram_specifier,
         )
-        traces["_".join((kde_trace.name, histogram_specifier.dimension))] = go.Scatter(
-            kde_trace.model_dump()
+        traces["_".join((kde_trace.name, histogram_specifier.dimension))] = (
+            kde_trace.to_plotly_trace()
         )
 
+    # Make sure we show at least one legend item
+    if not any(
+        trace.showlegend if trace.showlegend is not None else True for trace in traces.values()
+    ):
+        list(traces.values())[-1].update(showlegend=True)
+
     return traces
```

### Comparing `statsplotly-0.1.5/statsplotly/utils/color_utils.py` & `statsplotly-0.2.0/statsplotly/plot_specifiers/color/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,14 @@
 
 class ColorSystem(str, Enum):
     LINEAR = "linear"
     LOGARITHMIC = "logarithmic"
     DISCRETE = "discrete"
 
 
-def rand_jitter(arr: NDArray[Any], jitter_amount: float = 1) -> NDArray[Any]:
-    """from https://stackoverflow.com/questions/8671808/matplotlib-avoiding
-    -overlapping-datapoints-in-a-scatter-dot-beeswarm-plot"""
-    spread = 0.01 * (max(arr) - min(arr)) * jitter_amount or 0.05 * jitter_amount
-
-    return arr + np.random.randn(len(arr)) * spread
-
-
 def get_colorarray_from_seaborn(cmap: Cmap_specs | None, n_colors: int) -> NDArray[Any]:
     try:
         return sns.color_palette(cmap, n_colors=n_colors)
     except ValueError as exc:
         if isinstance(cmap, str):
             return sns.color_palette(cmap.lower(), n_colors=n_colors)
         raise exc
@@ -87,31 +79,27 @@
         try:
             # Then matplotlib
             return get_colorarray_from_matplotlib(cmap, n_colors=n_colors)
         except ValueError as exc:
             raise UnsupportedColormapError(f"{cmap} is not a supported colormap") from exc
 
 
-def to_rgb(numeric_array: NDArray[Any]) -> list[str]:
-    """Transforms a list of numeric rgb tuple into a list of rgb strings"""
-    rgb_array = [
-        "rgb" + str(rgb_tuple[:3])
-        for rgb_tuple in [tuple(int(rgb * 256) for rgb in x) for x in numeric_array]
-    ]
-    return rgb_array
+def to_rgb_string(numeric_rgb: tuple[float, float, float]) -> str:
+    """Transforms a numeric rgb tuple into a rgb string"""
+    return "rgb" + str(tuple(int(color * 256) for color in numeric_rgb)[:3])
 
 
 def get_rgb_discrete_array(
     n_colors: int, color_palette: Cmap_specs | matplotlib.colors.Colormap | None
 ) -> list[str]:
     """Color list/Seaborn color_palette wrapper."""
     rgb_array = cmap_to_array(n_colors, color_palette)
 
     # Convert the RGB value array to a RGB plotly_friendly string array
-    return to_rgb(rgb_array)
+    return [to_rgb_string(rgb) for rgb in rgb_array]
 
 
 def compute_colorscale(  # noqa PLR0912 C901
     n_colors: int,
     color_system: ColorSystem,
     logscale: float | None = 10,
     color_palette: Cmap_specs | matplotlib.colors.Colormap | None = None,
@@ -142,15 +130,15 @@
             colors = cmap_to_array(n_colors, color_palette)
         except UnsupportedColormapError as exc:
             raise ValueError(
                 f"{color_palette} is not supported for {color_system.value} color mapping, please "
                 "specify a Matplotlib-supported colormap"
             ) from exc
         else:
-            color_palette = to_rgb(colors)
+            color_palette = [to_rgb_string(color) for color in colors]
 
         nsample = len(color_palette)
         colorscale = []
         for log_scale, color_index in zip(
             np.logspace(-1, 0, nsample, base=logscale),
             [int(x) for x in np.linspace(0, n_colors - 1, nsample)],
             strict=True,
@@ -168,28 +156,28 @@
             colors = cmap_to_array(n_colors, color_palette)
         except UnsupportedColormapError as exc:
             raise ValueError(
                 f"{color_palette} is not supported for {color_system.value} mapping, please "
                 "specify a plotly or matplotlib-supported colorscale"
             ) from exc
         else:
-            color_palette = to_rgb(colors)
+            color_palette = [to_rgb_string(color) for color in colors]
         nsample = len(color_palette)
         colorscale = []
         for lin_scale, color_index in zip(
             np.linspace(0, 1, nsample),
             [int(x) for x in np.linspace(0, n_colors - 1, nsample)],
             strict=True,
         ):
             colorscale.append([lin_scale, color_palette[color_index]])
 
     elif color_system is ColorSystem.DISCRETE:
         try:
             colors = cmap_to_array(n_colors, color_palette)
-            color_palette = to_rgb(colors)
+            color_palette = [to_rgb_string(color) for color in colors]
         except UnsupportedColormapError as exc:
             raise ValueError(
                 f"{color_palette} is not supported for {color_system.value} mapping, please "
                 "specify a matplotlib-supported colorscale"
             ) from exc
         # Initialize colormap
         colorscale = []
@@ -201,17 +189,17 @@
             strict=True,
         ):
             colorscale.append([map_index, color])
 
     return colorscale
 
 
-def set_rgb_alpha(color_string: str, alpha: float | None = 1) -> str:
-    """Transforms a rgb string into a rgba string or adjust alpha value."""
-    if re.search("rgba", color_string) is not None:
-        # Changing alpha value
-        rgba_string = re.sub(r"\d.\d*", str(alpha), color_string)
-    else:
-        # Converting to rgb to rgba string
-        rgba_string = f"{re.sub('rgb', 'rgba', color_string)[:-1]} , {str(alpha)})"
+def set_rgb_alpha(color_ref: str | tuple[float, float, float], alpha: float = 1) -> str:
+    """Return a rgba string from a color reference."""
+    try:
+        rgb_string = to_rgb_string(matplotlib.colors.to_rgb(color_ref))
+    except ValueError:
+        # Already an rgb string
+        rgb_string = color_ref  # type: ignore
 
-    return rgba_string
+    # Convert to rgba string
+    return f"{re.sub('rgb', 'rgba', rgb_string)[:-1]} , {str(alpha)})"
```

### Comparing `statsplotly-0.1.5/statsplotly/utils/layout_utils.py` & `statsplotly-0.2.0/statsplotly/plot_specifiers/layout/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,27 @@
 from plotly import graph_objs as go
 
 from statsplotly import constants
 from statsplotly.plot_specifiers.data import DataHandler, SliceTraceType
 from statsplotly.plot_specifiers.trace import JointplotSpecifier, JointplotType
 
 
-def slice_name_in_trace_name(slice_name: str) -> Callable[[str], re.Match[Any] | None]:
+def set_horizontal_colorbar(colorbar_dict: dict[str, Any]) -> dict[str, Any]:
+    colorbar_dict.update(
+        {
+            "orientation": "h",
+            "y": constants.COLORBAR_BOTTOM_POSITION,
+            "xanchor": "center",
+            "yanchor": "bottom",
+        }
+    )
+    return colorbar_dict
+
+
+def _slice_name_in_trace_name(slice_name: str) -> Callable[[str], re.Match[Any] | None]:
     return re.compile(rf"\b({slice_name})\b").search
 
 
 def adjust_jointplot_legends(
     jointplot_specifier: JointplotSpecifier,
     slices_marginal_traces: dict[str, Any],
 ) -> None:
@@ -39,17 +51,21 @@
                 if (legendgroup := slices_marginal_traces[trace].legendgroup) not in legend_groups:
                     slices_marginal_traces[trace].update({"showlegend": True})
                     legend_groups.append(legendgroup)
 
         # Separate legend groups if we have only one slice
         if len(slices_marginal_traces) == 1:
             for trace in slices_marginal_traces:
-                slices_marginal_traces[trace].update({
-                    "legendgroup": " ".join((slices_marginal_traces[trace].legendgroup, "marginal"))
-                })
+                slices_marginal_traces[trace].update(
+                    {
+                        "legendgroup": " ".join(
+                            (slices_marginal_traces[trace].legendgroup, "marginal")
+                        )
+                    }
+                )
 
 
 def add_update_menu(
     fig: go.Figure,
     data_handler: DataHandler,
     slices_traces: dict[str, Any] | None = None,
     preplotted_traces: dict[str, Any] | None = None,
@@ -57,42 +73,51 @@
     trace_update_rule: dict[str, Any] = {}
     if slices_traces is None:
         slices_traces = {}
     if preplotted_traces is None:
         preplotted_traces = {}
 
     # all data visibility rules
-    trace_update_rule[SliceTraceType.ALL_DATA.value] = {
-        "visibility": [
-            trace.legendgroup == SliceTraceType.ALL_DATA.value
-            or (
-                trace.name
-                in [
-                    slice_trace.name
-                    for slice_trace in {**slices_traces, **preplotted_traces}.values()
-                ]
-            )
-            for trace in fig.data
-        ],
-        "showlegend": [trace.showlegend for trace in fig.data],
-        "legendgroup": [trace.legendgroup for trace in fig.data],
-    }
+    if SliceTraceType.ALL_DATA.value in [trace.legendgroup for trace in fig.data]:
+        trace_update_rule[SliceTraceType.ALL_DATA.value] = {
+            "visibility": [
+                trace.legendgroup == SliceTraceType.ALL_DATA.value
+                or (
+                    trace.name
+                    in [
+                        slice_trace.name
+                        for slice_trace in {**slices_traces, **preplotted_traces}.values()
+                    ]
+                )
+                for trace in fig.data
+            ],
+            "showlegend": [trace.showlegend for trace in fig.data],
+            "legendgroup": [
+                (
+                    trace.legendgroup
+                    if trace.name
+                    not in [slice_trace.name for slice_trace in slices_traces.values()]
+                    else SliceTraceType.SLICE.value
+                )
+                for trace in fig.data
+            ],
+        }
 
     def set_and_update_visibility_status(trace_name: str) -> bool:
         if trace_name in visibility_set:
             return False
         visibility_set.add(trace_name)
         return True
 
     for level in data_handler.slice_levels:
         # slicer visibility rules
         visibility_set: set[str] = set()
         trace_update_rule[level] = {
             "visibility": [
-                slice_name_in_trace_name(level)(trace.name) is not None for trace in fig.data
+                _slice_name_in_trace_name(level)(trace.name) is not None for trace in fig.data
             ],
             "showlegend": [set_and_update_visibility_status(trace.name) for trace in fig.data],
             "legendgroup": [trace.name for trace in fig.data],
         }
 
     # Update layout
     fig.update_layout(
@@ -117,41 +142,17 @@
                     }
                     for level, trace_update in trace_update_rule.items()
                 ],
             }
         ]
     )
 
-    # Adjust initial visibility
-    for trace, visibility in zip(
-        fig.data, fig.layout.updatemenus[0]["buttons"][0]["args"][0]["visible"], strict=True
-    ):
-        trace.update({"visible": visibility})
-
-    return fig
-
-
-def smart_title(title_string: str) -> str:
-    """Split string at _, capitalizes words, and joins with space."""
-    title_string = title_string.strip()
-    if len(title_string) == 0:
-        return title_string
-    return " ".join([
-        (
-            "".join([word[0].upper(), word[1:]])
-            if (len(word) >= constants.MIN_CAPITALIZE_LENGTH)
-            and not (any(letter.isupper() for letter in word))
-            else word
+    # Adjust initial parameters
+    for i, trace in enumerate(fig.data):
+        trace.update(
+            {
+                parameter: fig.layout.updatemenus[0]["buttons"][0]["args"][0][parameter][i]
+                for parameter in ["visible", "showlegend", "legendgroup"]
+            }
         )
-        for word in re.split(" |_", title_string)
-    ])
 
-
-def smart_legend(legend_string: str) -> str:
-    """Cleans and capitalizes axis legends for figure."""
-    legend_string = legend_string.strip()
-    if len(legend_string) == 0:
-        return legend_string
-    return " ".join([
-        "".join([w[0].upper(), w[1:]]) if i == 0 else w
-        for i, w in enumerate(re.split("_", legend_string))
-    ])
+    return fig
```

### Comparing `statsplotly-0.1.5/statsplotly/utils/stats_utils.py` & `statsplotly-0.2.0/statsplotly/plot_specifiers/data/statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Utility statistical functions."""
+"""Utility statistics functions."""
 
 from collections.abc import Callable
 from typing import Any
 
 import numpy as np
 import scipy as sc
 from numpy.typing import NDArray
@@ -103,41 +103,41 @@
 
     x_grid_mesh, y_grid_mesh = np.meshgrid(x_grid, y_grid)
     z = kde.evaluate(np.vstack([x_grid_mesh.ravel(), y_grid_mesh.ravel()]))
 
     return z.reshape(x_grid_mesh.shape)
 
 
-def sem(array: NDArray[Any], confidence_level: float = 0.95) -> float:
+def sem(data: NDArray[Any], confidence_level: float = 0.95) -> float:
     """Returns the margin of error at the given confidence level."""
     confidence_level = confidence_level / 2  # Converts to 2-tail
 
     # Anonymous function based on the Inverse of the complementary error function erfc.
     # see https://www.mathworks.com/help/matlab/ref/erfcinv.html?searchHighlight=erfcinv&s_tid=doc_srchtitle
     def my_norm_inv(confidence_level: float) -> float:
         return -np.sqrt(2) * sc.special.erfcinv(2 * confidence_level)
 
     zscore_ci = abs(
         my_norm_inv(confidence_level)
     )  # This is the same as doing: abs(sc.stats.norm.ppf(ci, 0, 1))
 
-    return np.std(array) / np.sqrt(len(array)) * zscore_ci
+    return np.std(data) / np.sqrt(len(data)) * zscore_ci
 
 
 def get_iqr(x: NDArray[Any]) -> NDArray[Any]:
     """Returns inter-quartile range."""
     iqr = np.subtract(*np.percentile(x, [75, 25]))
     return iqr
 
 
-def range_normalize(arr: NDArray[Any], a: float, b: float) -> NDArray[Any]:
+def range_normalize(data: NDArray[Any], a: float, b: float) -> NDArray[Any]:
     """Normalizes an array between a and b (min and max) values."""
-    if min(arr) == max(arr):
-        return np.clip(arr, a, b)
-    return (b - a) * (arr - min(arr)) / (max(arr) - min(arr)) + a
+    if min(data) == max(data):
+        return np.clip(data, a, b)
+    return (b - a) * (data - min(data)) / (max(data) - min(data)) + a
 
 
 def reject_outliers(data: NDArray[Any], m: float = 2.0) -> NDArray[Any]:
     """Uses distance from the median of a distribution to remove outliers.
     (from https://stackoverflow.com/a/45399188/4696032)
     Returns the masks of non outliers.
     """
```

