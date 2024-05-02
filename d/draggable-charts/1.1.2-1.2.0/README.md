# Comparing `tmp/draggable-charts-1.1.2.tar.gz` & `tmp/draggable-charts-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draggable-charts-1.1.2.tar", last modified: Mon Apr 29 22:15:36 2024, max compression
+gzip compressed data, was "draggable-charts-1.2.0.tar", last modified: Thu May  2 20:32:31 2024, max compression
```

## Comparing `draggable-charts-1.1.2.tar` & `draggable-charts-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.644344 draggable-charts-1.1.2/
--rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.1.2/LICENSE
--rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6106 2024-04-29 22:15:36.642326 draggable-charts-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.560516 draggable-charts-1.1.2/draggable_charts/
--rw-rw-rw-   0        0        0       41 2024-04-29 22:11:20.000000 draggable-charts-1.1.2/draggable_charts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.542557 draggable-charts-1.1.2/draggable_charts/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.589071 draggable-charts-1.1.2/draggable_charts/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.544553 draggable-charts-1.1.2/draggable_charts/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.602829 draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/
--rw-rw-rw-   0        0        0   605045 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js
--rw-rw-rw-   0        0        0     1831 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2585172 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js.map
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.619783 draggable-charts-1.1.2/draggable_charts/utils/
--rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.1.2/draggable_charts/utils/__init__.py
--rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.1.2/draggable_charts/utils/callback.py
--rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.1.2/draggable_charts/utils/component_func.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.637951 draggable-charts-1.1.2/draggable_charts/widgets/
--rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.1.2/draggable_charts/widgets/__init__.py
--rw-rw-rw-   0        0        0     4984 2024-04-26 17:59:06.000000 draggable-charts-1.1.2/draggable_charts/widgets/bezierchart.py
--rw-rw-rw-   0        0        0     6458 2024-04-29 15:36:39.000000 draggable-charts-1.1.2/draggable_charts/widgets/cubicbezierchart.py
--rw-rw-rw-   0        0        0     4502 2024-04-26 00:23:06.000000 draggable-charts-1.1.2/draggable_charts/widgets/linechart.py
--rw-rw-rw-   0        0        0     2495 2024-04-26 00:23:32.000000 draggable-charts-1.1.2/draggable_charts/widgets/scatterchart.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.578873 draggable-charts-1.1.2/draggable_charts.egg-info/
--rw-rw-rw-   0        0        0     6106 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      916 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 22:15:36.645272 draggable-charts-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1115 2024-04-29 22:15:28.000000 draggable-charts-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.567503 draggable-charts-1.2.0/
+-rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6106 2024-05-02 20:32:31.564608 draggable-charts-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.419854 draggable-charts-1.2.0/draggable_charts/
+-rw-rw-rw-   0        0        0       41 2024-05-02 20:31:31.000000 draggable-charts-1.2.0/draggable_charts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.390388 draggable-charts-1.2.0/draggable_charts/frontend/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.466528 draggable-charts-1.2.0/draggable_charts/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.393325 draggable-charts-1.2.0/draggable_charts/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.492314 draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   605045 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js
+-rw-rw-rw-   0        0        0     1831 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2585172 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js.map
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.527673 draggable-charts-1.2.0/draggable_charts/utils/
+-rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.2.0/draggable_charts/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.2.0/draggable_charts/utils/callback.py
+-rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.2.0/draggable_charts/utils/component_func.py
+-rw-rw-rw-   0        0        0     1816 2024-05-02 20:23:06.000000 draggable-charts-1.2.0/draggable_charts/utils/options.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.557595 draggable-charts-1.2.0/draggable_charts/widgets/
+-rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.2.0/draggable_charts/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3757 2024-05-02 19:52:35.000000 draggable-charts-1.2.0/draggable_charts/widgets/bezierchart.py
+-rw-rw-rw-   0        0        0     5258 2024-05-02 19:52:32.000000 draggable-charts-1.2.0/draggable_charts/widgets/cubicbezierchart.py
+-rw-rw-rw-   0        0        0     4459 2024-05-02 16:56:46.000000 draggable-charts-1.2.0/draggable_charts/widgets/linechart.py
+-rw-rw-rw-   0        0        0     2324 2024-05-02 19:52:11.000000 draggable-charts-1.2.0/draggable_charts/widgets/scatterchart.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.445246 draggable-charts-1.2.0/draggable_charts.egg-info/
+-rw-rw-rw-   0        0        0     6106 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:32:31.568499 draggable-charts-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2024-05-02 20:31:42.000000 draggable-charts-1.2.0/setup.py
```

### Comparing `draggable-charts-1.1.2/LICENSE` & `draggable-charts-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.2/PKG-INFO` & `draggable-charts-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.1.2/README.md` & `draggable-charts-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.2/draggable_charts/frontend/build/bootstrap.min.css` & `draggable-charts-1.2.0/draggable_charts/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js` & `draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt` & `draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js.map` & `draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js.map`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.2/draggable_charts/utils/callback.py` & `draggable-charts-1.2.0/draggable_charts/utils/callback.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.2/draggable_charts/utils/component_func.py` & `draggable-charts-1.2.0/draggable_charts/utils/component_func.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.2/draggable_charts/widgets/bezierchart.py` & `draggable-charts-1.2.0/draggable_charts/widgets/cubicbezierchart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,30 @@
 from typing import Any, Callable, Literal
 
 import numpy as np
 
 from ..utils import component, get_func_name, register
+from ..utils.options import set_options, include_colors
 
-DEFAULT_OPTIONS = {
-    "x_grid": True,
-    "y_grid": True,
-    "tension": 0.3,
-    "line": False,
-    "fixed_lines": [],
-    "colors": [
-        "#3366CC", "#DC3912", "#FF9900", "#109618", "#990099", "#3B3EAC", "#0099C6",
-        "#DD4477", "#66AA00", "#B82E2E", "#316395", "#994499", "#22AA99", "#AAAA11",
-        "#6633CC", "#E67300", "#8B0707", "#329262", "#5574A6", "#651067"
-    ]
-}
 
-
-def bezier_chart(
+def cubic_bezier_chart(
     data: dict,
-    t: float = 0.5,
     options: dict = None,
     on_change: Callable = None,
     args: tuple[Any, ...] = None,
     kwargs: dict[str, Any] = None,
     key: str = None
 ) -> dict:
     register(key, on_change, args, kwargs)
-    options = _set_options(data, options)
     _validate_scatter_data(data, options)
-    data = add_control_points(data, options, t)
-    data = _include_colors(data, options)
+    data = add_control_points(data, options)
+    data, options = set_options(data, options)
     default_data = {k: v for k, v in data.items() if k not in options["fixed_lines"]}
     return component(id=get_func_name(), kw=locals(), default=default_data, key=key)
 
-def _include_colors(data: dict, options: dict) -> dict:
-    for i, (trace_name, trace_data) in enumerate(data.items()):
-        trace_data['color'] = options['colors'][i % len(options['colors'])]
-    return data
-
-
-def _set_options(data: dict, options: dict) -> dict:
-    if not options:
-        options = DEFAULT_OPTIONS.copy()
-    options['x_type'] = _get_scale_type(data, 'x')
-    options['y_type'] = _get_scale_type(data, 'y')
-    options['colors'] = options.get('colors', DEFAULT_OPTIONS['colors'])
-    return options
-
-def _get_scale_type(data: dict, axis: Literal['x', 'y']) -> Literal['linear', 'category']:
-    for trace_data in data.values():
-        if not all(isinstance(val, (int, float, np.number)) for val in trace_data[axis]):
-            return 'category'
-    return 'linear'
-
 
 def _validate_scatter_data(data: dict, options: dict) -> None:
     # Check if data is a dictionary
     if not isinstance(data, dict):
         raise ValueError("Data must be a dictionary.")
 
     # If x is categorical, check if labels are specified
@@ -69,65 +35,96 @@
     # If y is categorical, check if labels are specified
     if options.get('y_type') == 'category' and not options.get('y_labels'):
         raise ValueError(
             "For categorical data in Y, you must specify the labels in the options.")
 
     # Check if each trace is a dictionary with 'x' and 'y' keys
     for trace_name, trace_data in data.items():
+        if trace_name not in options["fixed_lines"] and len(trace_data['x']) < 2:
+            raise ValueError(
+                f"Each interactive trace must have at least two points. Got: {trace_data}")
+            
         if not isinstance(trace_data, dict) or 'x' not in trace_data or 'y' not in trace_data:
             raise ValueError(
                 f"Each trace must be a dictionary with 'x' and 'y' keys. Got: {trace_data}")
 
         if not isinstance(trace_data['x'], list) or not isinstance(trace_data['y'], list):
             raise ValueError(
                 f"Both 'x' and 'y' must be lists. Got: x: {type(trace_data['x'])} y: {type(trace_data['y'])}")
 
         if len(trace_data['x']) != len(trace_data['y']):
             raise ValueError(
                 f"'x' and 'y' must be lists of the same length. Got: x={trace_data['x']}, y={trace_data['y']}")
 
 
-def add_control_points(data: dict, options: dict, t: float = 0.5) -> dict:
+def add_control_points(data: dict, options: dict) -> dict:
     for trace_name, trace_data in data.items():
-        if len(trace_data['x']) < 2 or trace_name in options["fixed_lines"]:
+        if trace_name in options["fixed_lines"]:
             continue
-        control_points = calculate_control_points(trace_data, t)
-        # Add control points into data:
-        for i, (x_c, y_c) in enumerate(control_points):
-            trace_data['x'].insert(2 * i + 1, x_c)
-            trace_data['y'].insert(2 * i + 1, y_c)
+        
+        new_trace_data = {'x': [], 'y': []}
+        if len(trace_data['x']) == 2:
+            # If there are only two points, add two intermediate points
+            x1, x2 = trace_data['x']
+            y1, y2 = trace_data['y']
+            new_trace_data['x'] = [x1, x1 + (x2 - x1) / 3, x1 + 2 * (x2 - x1) / 3, x2]
+            new_trace_data['y'] = [y1, y1 + (y2 - y1) / 3, y1 + 2 * (y2 - y1) / 3, y2]
+        
+        else:
+            P1, P2 = calculate_control_points(trace_data)
+            for i in range(len(trace_data['x']) - 1):
+                new_trace_data['x'].append(trace_data['x'][i])
+                new_trace_data['x'].append(P1[i][0])
+                new_trace_data['x'].append(P2[i][0])
+                
+                new_trace_data['y'].append(trace_data['y'][i])
+                new_trace_data['y'].append(P1[i][1])
+                new_trace_data['y'].append(P2[i][1])
+            new_trace_data['x'].append(trace_data['x'][-1])
+            new_trace_data['y'].append(trace_data['y'][-1])
+        data[trace_name] = new_trace_data
     return data
 
 
-def calculate_control_points(trace_data: dict, t: float) -> list:
-    control_points = []
-    for i in range(len(trace_data['x']) - 1):
-        x_0, y_0 = trace_data['x'][i], trace_data['y'][i]
-        x_1, y_1 = trace_data['x'][i + 1], trace_data['y'][i + 1]
-        if i == 0:
-            x_c, y_c = calculate_first_control_point(x_0, y_0, x_1, y_1, t)
-        else:
-            x_c, y_c = calculate_next_control_point(x_c, y_c, x_0, y_0, x_1)
-        control_points.append((x_c, y_c))
-    return control_points
-
-
-def calculate_first_control_point(
-    x_0: float, y_0: float,
-    x_1: float, y_1: float,
-    t: float
-) -> tuple[float, float]:
-    x_c = x_0 + (x_1 - x_0) / 2
-    y_c = y_0 + t * (y_1 - y_0)
-    return x_c, y_c
-
-
-def calculate_next_control_point(
-    x_c: float, y_c: float,
-    x_0: float, y_0: float,
-    x_1: float
-) -> tuple[float, float]:
-    m = (y_0 - y_c) / (x_0 - x_c)
-    b = y_0 - m * x_0
-    x_cn = x_0 + (x_1 - x_0) / 2
-    y_cn = m * x_cn + b
-    return x_cn, y_cn
+def calculate_control_points(trace_data: dict) -> list:
+    """See:
+    https://www.particleincell.com/2012/bezier-splines/
+    Second last eq has a typo, it's P2_i = 2*K_(i+1) - P1_(i+1)
+    """
+    n = len(trace_data['x']) - 1 # N. of segments
+
+    # Create matrix A (Ax + b = 0)
+    A = create_tri_diagonal_matrix(n)
+
+    # Create vector b (each component contains bx and by)
+    K = np.array(list(zip(trace_data['x'], trace_data['y'])))
+
+    b = np.array(
+        [(K[0][0] + 2 * K[1][0], K[0][1] + 2 * K[1][1])]
+        + [(4 * K[i][0] + 2 * K[i+1][0], 4 * K[i][1] + 2 * K[i+1][1]) for i in range(1, n - 1)]
+        + [(8 * K[n-1][0] + K[n][0], 8 * K[n-1][1] + K[n][1])]
+    )
+    
+    # Solve the system:
+    P1 = np.linalg.solve(A, b)
+    
+    # Compute P2:
+    # P2_i = ( 2*K_(i+1) - P1_(i+1) ),  for i = 0, ..., n-1
+    # P2_(n-1) = (1/2) * (K_(n-1) + P1_(n-1) )
+    P2 = 2 * K[1:-1] - P1[1:]
+    P2 = np.concatenate( (P2, [(1/2)*(K[-1] + P1[-1])] ))
+    return P1, P2
+    
+
+def create_tri_diagonal_matrix(n):
+    """This function creates the A matrix to find the control points of the cubic bezier curve.
+    See "The Matrix" Section in:
+    https://exploringswift.com/blog/Drawing-Smooth-Cubic-Bezier-Curve-through-prescribed-points-using-Swift
+    """
+    A = np.zeros((n, n))
+    # Main diagonal
+    A += np.diag([2] + [4]*(n-2) + [7], k=0)
+    # Upper diagonal
+    A += np.diag([1]*(n-1), k=1)
+    # Lower diagonal
+    A += np.diag([1]*(n-2) + [2], k=-1)
+    return A
```

### Comparing `draggable-charts-1.1.2/draggable_charts/widgets/linechart.py` & `draggable-charts-1.2.0/draggable_charts/widgets/linechart.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from typing import Any, Callable, Dict, Union
 
 import numpy as np
 import pandas as pd
 
 from ..utils import component, get_func_name, register
-
-DEFAULT_OPTIONS = {
-    "x_grid": True,
-    "y_grid": True,
-    "tension": 0.3
-}
+from ..utils.options import DEFAULT_OPTIONS
 
 
 def line_chart(
     data: Union[pd.DataFrame, pd.Series],
     options: Dict[str, Any] = {},
     on_change: Callable = None,
     args: tuple[Any, ...] = None,
```

### Comparing `draggable-charts-1.1.2/draggable_charts/widgets/scatterchart.py` & `draggable-charts-1.2.0/draggable_charts/widgets/scatterchart.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from typing import Any, Callable, Literal
 
 import numpy as np
 
 from ..utils import component, get_func_name, register
-
-DEFAULT_OPTIONS = {
-    "x_grid": True,
-    "y_grid": True,
-    "tension": 0.3,
-    "line": False,
-}
+from ..utils.options import set_options, include_colors
 
 
 def _get_scale_type(data: dict, axis: Literal['x', 'y']) -> Literal['linear', 'category']:
     for trace_data in data.values():
         if not all(isinstance(val, (int, float, np.number)) for val in trace_data[axis]):
             return 'category'
     return 'linear'
@@ -52,13 +46,10 @@
     options: dict = None,
     on_change: Callable = None,
     args: tuple[Any, ...] = None,
     kwargs: dict[str, Any] = None,
     key: str = None
 ) -> dict:
     register(key, on_change, args, kwargs)
-    if not options:
-        options = DEFAULT_OPTIONS.copy()
-    options['x_type'] = _get_scale_type(data, 'x')
-    options['y_type'] = _get_scale_type(data, 'y')
+    data, options = set_options(data, options)
     _validate_scatter_data(data, options)
     return component(id=get_func_name(), kw=locals(), default=data, key=key)
```

### Comparing `draggable-charts-1.1.2/draggable_charts.egg-info/PKG-INFO` & `draggable-charts-1.2.0/draggable_charts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.1.2/draggable_charts.egg-info/SOURCES.txt` & `draggable-charts-1.2.0/draggable_charts.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 draggable_charts/frontend/build/index.html
 draggable_charts/frontend/build/static/js/main.96151505.js
 draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt
 draggable_charts/frontend/build/static/js/main.96151505.js.map
 draggable_charts/utils/__init__.py
 draggable_charts/utils/callback.py
 draggable_charts/utils/component_func.py
+draggable_charts/utils/options.py
 draggable_charts/widgets/__init__.py
 draggable_charts/widgets/bezierchart.py
 draggable_charts/widgets/cubicbezierchart.py
 draggable_charts/widgets/linechart.py
 draggable_charts/widgets/scatterchart.py
```

### Comparing `draggable-charts-1.1.2/setup.py` & `draggable-charts-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="draggable-charts",
-    version="1.1.2",
+    version="1.2.0",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/balexandermunoz/draggable-charts",
     packages=setuptools.find_packages(),
```

