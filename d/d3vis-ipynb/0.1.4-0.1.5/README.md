# Comparing `tmp/d3vis_ipynb-0.1.4.tar.gz` & `tmp/d3vis_ipynb-0.1.5.tar.gz`

## Comparing `d3vis_ipynb-0.1.4.tar` & `d3vis_ipynb-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/D3vis_ipynb.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/RELEASE.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/install.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/setup.cfg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/setup.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/_version.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/embedding.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/web.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/widgets.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/package.json
--rw-r--r--   0        0        0    27995 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/363.eafafc6b255bbd58c086.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js
--rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/remoteEntry.d538e52840abf118c637.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/style.js
--rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    93817 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/d3vis_ipynb/nbextension/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/amd-public-path.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/package.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/webpack.config.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/webpack.exports.config.js
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/css/widget.css
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/extension.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/index.js
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/labplugin.js
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/web-dev.js
--rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/widgets.js
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/barplot.js
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/histogramplot.js
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/linearhistplot.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/rangeslider.js
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/graphs/scatterplot.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/tools/lasso.js
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/js/lib/wrappers/embedding.wrapper.js
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/README.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/D3vis_ipynb.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/RELEASE.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/install.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/setup.cfg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/setup.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/_version.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/embedding.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/web.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/widgets.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/package.json
+-rw-r--r--   0        0        0    27996 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/363.d9832b540bc5aa86432a.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js
+-rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/remoteEntry.0a6c310552f16e38d4c2.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/style.js
+-rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    93818 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/d3vis_ipynb/nbextension/index.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/amd-public-path.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/package.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/webpack.config.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/webpack.exports.config.js
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/css/widget.css
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/extension.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/index.js
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/labplugin.js
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/web-dev.js
+-rw-r--r--   0        0        0    12874 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/widgets.js
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/barplot.js
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/histogramplot.js
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/linearhistplot.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/rangeslider.js
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/graphs/scatterplot.js
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/tools/lasso.js
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/js/lib/wrappers/embedding.wrapper.js
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/README.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.5/PKG-INFO
```

### Comparing `d3vis_ipynb-0.1.4/RELEASE.md` & `d3vis_ipynb-0.1.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/setup.cfg` & `d3vis_ipynb-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/__init__.py` & `d3vis_ipynb-0.1.5/d3vis_ipynb/__init__.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/embedding.py` & `d3vis_ipynb-0.1.5/d3vis_ipynb/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,20 +120,21 @@
         self._all_widgets.append(widget)
         if self._is_displayed:
             widget.elementId = self.positions_hashs[position]
             display(widget)
         else:
             self._widgets_to_display[position] = widget
 
-    def _repr_html_(self):
+    def _ipython_display_(self):
         self._is_displayed = True
         for key in self._widgets_to_display.keys():
             widget = self._widgets_to_display[key]
             widget.elementId = self.positions_hashs[key]
             display(widget)
+        super()._ipython_display_()
 
     def export(self):
         absolute_path = os.path.dirname(__file__)
         relative_js_path = "../js/lib/"
         js_path = os.path.abspath(os.path.join(absolute_path, relative_js_path))
         relative_data_path = "wrappers/data.json"
         data_path = os.path.join(js_path, relative_data_path)
```

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/web.py` & `d3vis_ipynb-0.1.5/d3vis_ipynb/web.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/widgets.py` & `d3vis_ipynb-0.1.5/d3vis_ipynb/widgets.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/package.json` & `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603365384615384%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.0a6c310552f16e38d4c2.js'}}",*

 * * "'version'": "'0.1.5'"}*

```diff
@@ -16,15 +16,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d538e52840abf118c637.js"
+            "load": "static/remoteEntry.0a6c310552f16e38d4c2.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -54,9 +54,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/363.eafafc6b255bbd58c086.js` & `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/363.d9832b540bc5aa86432a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -560,15 +560,15 @@
                 value_changed() {
                     const e = this.model.get("matrix"),
                         t = this.model.get("grid_areas"),
                         n = this.model.get("grid_template_areas");
                     let a = this.model.get("style");
                     a || (a = "basic");
                     const i = document.createElement("div");
-                    i.classList.add(a), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + e.length + ", 20vh)", i.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", i.style.width = "100%", t.forEach((e => {
+                    i.classList.add(a), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + e.length + ", 180px)", i.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", i.style.width = "100%", t.forEach((e => {
                         const t = document.createElement("div");
                         t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), i.appendChild(t)
                     })), this.el.appendChild(i), console.log("Embedding:"), console.log(i)
                 }
             }
             class I extends a.DOMWidgetModel {
                 defaults() {
@@ -829,11 +829,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.4","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.5","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js` & `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js` & `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/remoteEntry.d538e52840abf118c637.js` & `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/remoteEntry.0a6c310552f16e38d4c2.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, s, d, l, f, p, c, h, v, g, b, m, y, w = {
+    var e, r, t, n, o, i, a, u, d, s, l, f, c, p, h, v, g, b, m, y, w = {
             772: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(363).then((() => () => t(363))),
                         "./extension": () => Promise.all([t.e(363), t.e(493)]).then((() => () => t(493)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -42,47 +42,47 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        363: "eafafc6b255bbd58c086",
+        363: "d9832b540bc5aa86432a",
         493: "053b071a46f0bcccaab9",
         693: "c8409ce8329f6703470f"
     } [e] + ".js?v=" + {
-        363: "eafafc6b255bbd58c086",
+        363: "d9832b540bc5aa86432a",
         493: "053b071a46f0bcccaab9",
         693: "c8409ce8329f6703470f"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
             var a, u;
             if (void 0 !== o)
-                for (var s = document.getElementsByTagName("script"), d = 0; d < s.length; d++) {
-                    var l = s[d];
+                for (var d = document.getElementsByTagName("script"), s = 0; s < d.length; s++) {
+                    var l = d[s];
                     if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + o) {
                         a = l;
                         break
                     }
                 }
             a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var f = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+                    a.onerror = a.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), u && document.head.appendChild(a)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -107,16 +107,16 @@
                             u = o[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
-                    s = [];
-                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.1.4", (() => E.e(363).then((() => () => E(363)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
+                    d = [];
+                return "default" === t && (u("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), u("d3vis_ipynb", "0.1.5", (() => E.e(363).then((() => () => E(363)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -152,77 +152,77 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var a = [];
         for (i = 1; i < e.length; i++) {
             var u = e[i];
-            a.push(0 === u ? "not(" + s() + ")" : 1 === u ? "(" + s() + " || " + s() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
+            a.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
         }
-        return s();
+        return d();
 
-        function s() {
+        function d() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, u = 1, s = !0;; u++, a++) {
-                var d, l, f = u < e.length ? (typeof e[u])[0] : "";
-                if (a >= r.length || "o" == (l = (typeof(d = r[a]))[0])) return !s || ("u" == f ? u > n && !o : "" == f != o);
+            for (var a = 0, u = 1, d = !0;; u++, a++) {
+                var s, l, f = u < e.length ? (typeof e[u])[0] : "";
+                if (a >= r.length || "o" == (l = (typeof(s = r[a]))[0])) return !d || ("u" == f ? u > n && !o : "" == f != o);
                 if ("u" == l) {
-                    if (!s || "u" != f) return !1
-                } else if (s)
+                    if (!d || "u" != f) return !1
+                } else if (d)
                     if (f == l)
                         if (u <= n) {
-                            if (d != e[u]) return !1
+                            if (s != e[u]) return !1
                         } else {
-                            if (o ? d > e[u] : d < e[u]) return !1;
-                            d != e[u] && (s = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (d = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
-                    s = !1, u--
+                    d = !1, u--
                 } else {
                     if (u <= n || l < f != o) return !1;
-                    s = !1
-                } else "s" != f && "n" != f && (s = !1, u--)
+                    d = !1
+                } else "s" != f && "n" != f && (d = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, a = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
+    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return i(n, o) || f(s(e, t, o, n)), p(e[t][o])
+        return i(n, o) || f(d(e, t, o, n)), c(e[t][o])
     }, l = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
         var i = E.I(r);
         return i && i.then ? i.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), d(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
         var i = r && E.o(r, t) && l(r, t, n);
-        return i ? p(i) : o()
+        return i ? c(i) : o()
     })), g = {}, b = {
         801: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
@@ -272,20 +272,20 @@
                             a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [i, a, u] = t,
-                    s = 0;
+                    d = 0;
                 if (i.some((r => 0 !== e[r]))) {
                     for (n in a) E.o(a, n) && (E.m[n] = a[n]);
                     u && u(E)
                 }
-                for (r && r(t); s < i.length; s++) o = i[s], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); d < i.length; d++) o = i[d], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var P = E(772);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).d3vis_ipynb = P
 })();
```

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/labextension/static/third-party-licenses.json` & `d3vis_ipynb-0.1.5/d3vis_ipynb/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/d3vis_ipynb/nbextension/index.js` & `d3vis_ipynb-0.1.5/d3vis_ipynb/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -179,15 +179,15 @@
             55: t => {
                 t.exports = e
             },
             308: e => {
                 e.exports = t
             },
             330: t => {
-                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.4","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.5","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
@@ -3949,15 +3949,15 @@
             value_changed() {
                 const t = this.model.get("matrix"),
                     e = this.model.get("grid_areas"),
                     n = this.model.get("grid_template_areas");
                 let r = this.model.get("style");
                 r || (r = "basic");
                 const i = document.createElement("div");
-                i.classList.add(r), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + t.length + ", 20vh)", i.style.gridTemplateColumns = "repeat(" + t[0].length + ", 1fr)", i.style.width = "100%", e.forEach((t => {
+                i.classList.add(r), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + t.length + ", 180px)", i.style.gridTemplateColumns = "repeat(" + t[0].length + ", 1fr)", i.style.width = "100%", e.forEach((t => {
                     const e = document.createElement("div");
                     e.setAttribute("id", t), e.style.gridArea = t, e.classList.add("dashboard-div"), i.appendChild(e)
                 })), this.el.appendChild(i), console.log("Embedding:"), console.log(i)
             }
         }
         class zi extends t.DOMWidgetModel {
             defaults() {
```

### Comparing `d3vis_ipynb-0.1.4/js/amd-public-path.js` & `d3vis_ipynb-0.1.5/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/package.json` & `d3vis_ipynb-0.1.5/js/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.5'"}*

```diff
@@ -50,9 +50,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `d3vis_ipynb-0.1.4/js/webpack.config.js` & `d3vis_ipynb-0.1.5/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/webpack.exports.config.js` & `d3vis_ipynb-0.1.5/js/webpack.exports.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/css/widget.css` & `d3vis_ipynb-0.1.5/js/css/widget.css`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/labplugin.js` & `d3vis_ipynb-0.1.5/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/web-dev.js` & `d3vis_ipynb-0.1.5/js/lib/web-dev.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/widgets.js` & `d3vis_ipynb-0.1.5/js/lib/widgets.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -365,15 +365,15 @@
         }
 
         const node = document.createElement("div");
 
         node.classList.add(style);
         node.style.display = "grid";
         node.style.gridTemplateAreas = grid_template_areas;
-        node.style.gridTemplateRows = "repeat(" + matrix.length + ", 20vh)";
+        node.style.gridTemplateRows = "repeat(" + matrix.length + ", 180px)";
         node.style.gridTemplateColumns = "repeat(" + matrix[0].length + ", 1fr)";
         node.style.width = "100%";
 
         grid_areas.forEach((area) => {
             const grid_area = document.createElement("div");
             grid_area.setAttribute("id", area);
             grid_area.style.gridArea = area;
```

### Comparing `d3vis_ipynb-0.1.4/js/lib/graphs/barplot.js` & `d3vis_ipynb-0.1.5/js/lib/graphs/barplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/graphs/histogramplot.js` & `d3vis_ipynb-0.1.5/js/lib/graphs/histogramplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/graphs/linearhistplot.js` & `d3vis_ipynb-0.1.5/js/lib/graphs/linearhistplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/graphs/rangeslider.js` & `d3vis_ipynb-0.1.5/js/lib/graphs/rangeslider.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/graphs/scatterplot.js` & `d3vis_ipynb-0.1.5/js/lib/graphs/scatterplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/tools/lasso.js` & `d3vis_ipynb-0.1.5/js/lib/tools/lasso.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/js/lib/wrappers/embedding.wrapper.js` & `d3vis_ipynb-0.1.5/js/lib/wrappers/embedding.wrapper.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/LICENSE.txt` & `d3vis_ipynb-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/README.md` & `d3vis_ipynb-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.4/pyproject.toml` & `d3vis_ipynb-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "ipywidgets>=7.7.1",
+    "ipywidgets==7.7.1",
     "simplejson >=3.19.0",
     "anywidget >= 0.9.6"
 ]
-version = "0.1.4"
+version = "0.1.5"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
```

### Comparing `d3vis_ipynb-0.1.4/PKG-INFO` & `d3vis_ipynb-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: d3vis_ipynb
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Custom Jupyter Widget Library with visualizations created with D3.js.
 Project-URL: Homepage, https://github.com/H-IAAC/d3vis_ipynb
 Author-email: Daniel Adam Miranda <daniel.miranda@eldorado.org.br>
 License: Copyright (c) 2024 Daniel Adam Miranda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -43,15 +43,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Requires-Dist: anywidget>=0.9.6
-Requires-Dist: ipywidgets>=7.7.1
+Requires-Dist: ipywidgets==7.7.1
 Requires-Dist: simplejson>=3.19.0
 Provides-Extra: docs
 Requires-Dist: jupyter-sphinx; extra == 'docs'
 Requires-Dist: nbsphinx; extra == 'docs'
 Requires-Dist: nbsphinx-link; extra == 'docs'
 Requires-Dist: pypandoc; extra == 'docs'
 Requires-Dist: pytest-check-links; extra == 'docs'
```

