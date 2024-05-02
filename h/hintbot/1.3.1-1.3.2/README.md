# Comparing `tmp/hintbot-1.3.1.tar.gz` & `tmp/hintbot-1.3.2.tar.gz`

## Comparing `hintbot-1.3.1.tar` & `hintbot-1.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hintbot-1.3.1/.copier-answers.yml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hintbot-1.3.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.3.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hintbot-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 hintbot-1.3.1/RELEASE.md
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 hintbot-1.3.1/install.json
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.3.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hintbot-1.3.1/setup.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hintbot-1.3.1/tsconfig.json
--rw-r--r--   0        0        0   220911 2020-02-02 00:00:00.000000 hintbot-1.3.1/yarn.lock
--rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 hintbot-1.3.1/example/assignment1.ipynb
--rw-r--r--   0        0        0    10402 2020-02-02 00:00:00.000000 hintbot-1.3.1/example/assignment2.ipynb
--rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 hintbot-1.3.1/example/assignment3.ipynb
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 hintbot-1.3.1/example/assignment4.ipynb
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/_version.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/application.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/handlers.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/labextension/package.json
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/labextension/schemas/hintbot/package.json.orig
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/labextension/schemas/hintbot/plugin.json
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/labextension/static/496.48e8a8a41e7a4f0b36b7.js
--rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/labextension/static/747.ded73249030e62fecded.js
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/labextension/static/remoteEntry.197002f29a2522c7697c.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hintbot-1.3.1/hintbot/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hintbot-1.3.1/jupyter-config/server-config/hintbot.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.3.1/schema/plugin.json
--rw-r--r--   0        0        0     8212 2020-02-02 00:00:00.000000 hintbot-1.3.1/src/createHintBanner.ts
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hintbot-1.3.1/src/handler.ts
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 hintbot-1.3.1/src/index.ts
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 hintbot-1.3.1/src/requestHint.ts
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hintbot-1.3.1/src/showHintTypeDialog.tsx
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hintbot-1.3.1/src/showReflectionDialog.tsx
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 hintbot-1.3.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.3.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hintbot-1.3.1/style/index.js
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 hintbot-1.3.1/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 hintbot-1.3.1/LICENSE
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 hintbot-1.3.1/README.md
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hintbot-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 hintbot-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hintbot-1.3.2/.copier-answers.yml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hintbot-1.3.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.3.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hintbot-1.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 hintbot-1.3.2/RELEASE.md
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 hintbot-1.3.2/install.json
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.3.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hintbot-1.3.2/setup.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hintbot-1.3.2/tsconfig.json
+-rw-r--r--   0        0        0   220911 2020-02-02 00:00:00.000000 hintbot-1.3.2/yarn.lock
+-rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 hintbot-1.3.2/example/assignment1.ipynb
+-rw-r--r--   0        0        0    10402 2020-02-02 00:00:00.000000 hintbot-1.3.2/example/assignment2.ipynb
+-rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 hintbot-1.3.2/example/assignment3.ipynb
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 hintbot-1.3.2/example/assignment4.ipynb
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/_version.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/application.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/handlers.py
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/labextension/package.json
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/labextension/schemas/hintbot/package.json.orig
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/labextension/schemas/hintbot/plugin.json
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/labextension/static/496.48e8a8a41e7a4f0b36b7.js
+-rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/labextension/static/747.ded73249030e62fecded.js
+-rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/labextension/static/remoteEntry.4d3e85a4dc5d1b6dfe21.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hintbot-1.3.2/hintbot/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hintbot-1.3.2/jupyter-config/server-config/hintbot.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.3.2/schema/plugin.json
+-rw-r--r--   0        0        0     8212 2020-02-02 00:00:00.000000 hintbot-1.3.2/src/createHintBanner.ts
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hintbot-1.3.2/src/handler.ts
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 hintbot-1.3.2/src/index.ts
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 hintbot-1.3.2/src/requestHint.ts
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hintbot-1.3.2/src/showHintTypeDialog.tsx
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hintbot-1.3.2/src/showReflectionDialog.tsx
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 hintbot-1.3.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.3.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hintbot-1.3.2/style/index.js
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 hintbot-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 hintbot-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 hintbot-1.3.2/README.md
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hintbot-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 hintbot-1.3.2/PKG-INFO
```

### Comparing `hintbot-1.3.1/RELEASE.md` & `hintbot-1.3.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/package.json` & `hintbot-1.3.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.3.2'"}*

```diff
@@ -203,9 +203,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.3.1"
+    "version": "1.3.2"
 }
```

### Comparing `hintbot-1.3.1/tsconfig.json` & `hintbot-1.3.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/yarn.lock` & `hintbot-1.3.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/example/assignment1.ipynb` & `hintbot-1.3.2/example/assignment1.ipynb`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/example/assignment2.ipynb` & `hintbot-1.3.2/example/assignment2.ipynb`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/example/assignment3.ipynb` & `hintbot-1.3.2/example/assignment3.ipynb`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/example/assignment4.ipynb` & `hintbot-1.3.2/example/assignment4.ipynb`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/hintbot/__init__.py` & `hintbot-1.3.2/hintbot/__init__.py`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/hintbot/handlers.py` & `hintbot-1.3.2/hintbot/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 import os
 import requests
 import tornado
 from jupyter_server.base.handlers import JupyterHandler
 from jupyter_server.extension.handler import ExtensionHandlerMixin
 
 HOST_URL = os.getenv('HOST_URL')
-print("*****************")
-print(HOST_URL)
-print("*****************")
 
 STATUS = {
     "Loading": 0,
     "Success": 1,
     "Cancelled": 2,
     "Error": 3
 }
```

### Comparing `hintbot-1.3.1/hintbot/labextension/package.json` & `hintbot-1.3.2/hintbot/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788773148148149%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4d3e85a4dc5d1b6dfe21.js'}}",*

 * * "'version'": "'1.3.2'"}*

```diff
@@ -105,15 +105,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/educational-technology-collective/hintbot",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.197002f29a2522c7697c.js",
+            "load": "static/remoteEntry.4d3e85a4dc5d1b6dfe21.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "hintbot"
                 },
@@ -208,9 +208,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.3.1"
+    "version": "1.3.2"
 }
```

### Comparing `hintbot-1.3.1/hintbot/labextension/schemas/hintbot/package.json.orig` & `hintbot-1.3.2/hintbot/labextension/schemas/hintbot/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.3.2'"}*

```diff
@@ -203,9 +203,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.3.1"
+    "version": "1.3.2"
 }
```

### Comparing `hintbot-1.3.1/hintbot/labextension/schemas/hintbot/plugin.json` & `hintbot-1.3.2/hintbot/labextension/schemas/hintbot/plugin.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/hintbot/labextension/static/496.48e8a8a41e7a4f0b36b7.js` & `hintbot-1.3.2/hintbot/labextension/static/496.48e8a8a41e7a4f0b36b7.js`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/hintbot/labextension/static/747.ded73249030e62fecded.js` & `hintbot-1.3.2/hintbot/labextension/static/747.ded73249030e62fecded.js`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/hintbot/labextension/static/remoteEntry.197002f29a2522c7697c.js` & `hintbot-1.3.2/hintbot/labextension/static/remoteEntry.4d3e85a4dc5d1b6dfe21.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => S.e(496).then((() => () => S(496))),
                         from: i,
                         eager: !1
                     })
-                })("hintbot", "1.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("hintbot", "1.3.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `hintbot-1.3.1/hintbot/labextension/static/third-party-licenses.json` & `hintbot-1.3.2/hintbot/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/schema/plugin.json` & `hintbot-1.3.2/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/src/createHintBanner.ts` & `hintbot-1.3.2/src/createHintBanner.ts`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/src/handler.ts` & `hintbot-1.3.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/src/index.ts` & `hintbot-1.3.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/src/requestHint.ts` & `hintbot-1.3.2/src/requestHint.ts`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/src/showHintTypeDialog.tsx` & `hintbot-1.3.2/src/showHintTypeDialog.tsx`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/src/showReflectionDialog.tsx` & `hintbot-1.3.2/src/showReflectionDialog.tsx`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/style/base.css` & `hintbot-1.3.2/style/base.css`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/.gitignore` & `hintbot-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/LICENSE` & `hintbot-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/README.md` & `hintbot-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/pyproject.toml` & `hintbot-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hintbot-1.3.1/PKG-INFO` & `hintbot-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hintbot
-Version: 1.3.1
+Version: 1.3.2
 Dynamic: Keywords
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/educational-technology-collective/hintbot
 Project-URL: Bug Tracker, https://github.com/educational-technology-collective/hintbot/issues
 Project-URL: Repository, https://github.com/educational-technology-collective/hintbot.git
 Author-email: etc <mengyanw@umich.edu>
 License: BSD 3-Clause License
```

