# Comparing `tmp/ragdaemon-0.4.1.tar.gz` & `tmp/ragdaemon-0.4.2.tar.gz`

## Comparing `ragdaemon-0.4.1.tar` & `ragdaemon-0.4.2.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/app.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/context.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/graph.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/llm.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/utils.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/app.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/context.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/graph.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/llm.py
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/utils.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.2/PKG-INFO
```

### Comparing `ragdaemon-0.4.1/tutorial.ipynb` & `ragdaemon-0.4.2/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/.github/workflows/run-tests.yml` & `ragdaemon-0.4.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/app.py` & `ragdaemon-0.4.2/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/context.py` & `ragdaemon-0.4.2/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/daemon.py` & `ragdaemon-0.4.2/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/get_paths.py` & `ragdaemon-0.4.2/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/graph.py` & `ragdaemon-0.4.2/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/utils.py` & `ragdaemon-0.4.2/ragdaemon/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import hashlib
 import os
 import re
 import subprocess
+from base64 import b64encode
 from pathlib import Path
 
 from spice import Spice
 from spice.models import UnknownModel
 from spice.spice import get_model_from_name
 
 from ragdaemon.errors import RagdaemonError
@@ -14,14 +15,19 @@
 
 
 def hash_str(string: str) -> str:
     """Return the MD5 hash of the input string."""
     return hashlib.md5(string.encode()).hexdigest()
 
 
+def basic_auth(username: str, password: str):
+    token = b64encode(f"{username}:{password}".encode("utf-8")).decode("ascii")
+    return f"Basic {token}"
+
+
 def get_git_diff(diff_args: str, cwd: str) -> str:
     args = ["git", "diff", "-U1"]
     if diff_args and diff_args != "DEFAULT":
         args += diff_args.split(" ")
     diff = subprocess.check_output(args, cwd=cwd, text=True)
     return diff
```

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/__init__.py` & `ragdaemon-0.4.2/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.4.2/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/chunker.py` & `ragdaemon-0.4.2/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.4.2/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.4.2/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/diff.py` & `ragdaemon-0.4.2/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.4.2/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.4.2/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.4.2/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/database/__init__.py` & `ragdaemon-0.4.2/ragdaemon/database/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         try:
             db = ChromaDB(
                 cwd=cwd,
                 db_path=db_path,
                 spice_client=spice_client,
                 embedding_model=embedding_model,
                 embedding_provider=embedding_provider,
+                verbose=verbose,
             )
             # In case the api key is wrong, try to embed something to trigger an error.
             _ = db.add(ids="test", documents="test doc")
             db.delete(ids="test")
             return db
         except Exception as e:
             if verbose:
```

### Comparing `ragdaemon-0.4.1/ragdaemon/database/chroma_database.py` & `ragdaemon-0.4.2/ragdaemon/database/chroma_database.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import os
 from pathlib import Path
-from typing import Any, TYPE_CHECKING, Optional, cast
+from typing import TYPE_CHECKING, Any, Optional, cast
 
+import dotenv
+from chromadb.config import Settings
 from spice import Spice
 
+from ragdaemon import __version__
 from ragdaemon.database.database import Database
 from ragdaemon.errors import RagdaemonError
-from ragdaemon import __version__
+from ragdaemon.utils import basic_auth
 
 MAX_INPUTS_PER_CALL = 2048
 
 if TYPE_CHECKING:
     from chromadb.api.types import (
         GetResult,
         Metadata,
@@ -34,14 +38,15 @@
     def __init__(
         self,
         cwd: Path,
         db_path: Path,
         spice_client: Spice,
         embedding_model: str,
         embedding_provider: Optional[str] = None,
+        verbose: bool = False,
     ) -> None:
         self.cwd = cwd
         self.db_path = db_path
         self.embedding_model = embedding_model
 
         import chromadb  # Imports are slow so do it lazily
         from chromadb.api.types import (
@@ -67,15 +72,35 @@
                         provider=embedding_provider,
                     ).embeddings
                     output.extend(embeddings)
                 return output
 
         embedding_function = SpiceEmbeddingFunction()
 
-        _client = chromadb.PersistentClient(path=str(db_path))
+        dotenv.load_dotenv()
+
+        try:
+            host = os.environ["CHROMA_SERVER_HOST"]
+            port = int(os.environ.get("CHROMA_SERVER_HTTP_PORT", 443))
+            username = os.environ["CHROMA_SERVER_USERNAME"]
+            password = os.environ["CHROMA_SERVER_PASSWORD"]
+            _client = chromadb.HttpClient(
+                host=host,
+                port=port,
+                ssl=port == 443,
+                headers={"Authorization": basic_auth(username, password)},
+                settings=Settings(allow_reset=True, anonymized_telemetry=False),
+            )
+        except KeyError:
+            if verbose:
+                print(
+                    "No Chroma HTTP client environment variables found. Defaulting to PersistentClient."
+                )
+            _client = chromadb.PersistentClient(path=str(db_path))
+
         minor_version = ".".join(__version__.split(".")[:2])
         name = f"ragdaemon-{minor_version}-{self.embedding_model}"
         self._collection = _client.get_or_create_collection(
             name=name,
             embedding_function=embedding_function,
         )
```

### Comparing `ragdaemon-0.4.1/ragdaemon/database/database.py` & `ragdaemon-0.4.2/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/database/lite_database.py` & `ragdaemon-0.4.2/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.4.2/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/static/favicon.ico` & `ragdaemon-0.4.2/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.4.2/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/static/js/main.js` & `ragdaemon-0.4.2/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.4.2/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/static/js/three/node.js` & `ragdaemon-0.4.2/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.4.2/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/ragdaemon/templates/index.html` & `ragdaemon-0.4.2/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/conftest.py` & `ragdaemon-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/test_comments.py` & `ragdaemon-0.4.2/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/test_context.py` & `ragdaemon-0.4.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/test_daemon.py` & `ragdaemon-0.4.2/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/test_get_paths.py` & `ragdaemon-0.4.2/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/test_sample.py` & `ragdaemon-0.4.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/annotators/test_chunker.py` & `ragdaemon-0.4.2/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.4.2/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/annotators/test_diff.py` & `ragdaemon-0.4.2/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/annotators/test_hierarchy.py` & `ragdaemon-0.4.2/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.4.2/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/annotators/test_summarizer.py` & `ragdaemon-0.4.2/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/data/chunker_graph.json` & `ragdaemon-0.4.2/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/data/context_message.txt` & `ragdaemon-0.4.2/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/data/diff_graph.json` & `ragdaemon-0.4.2/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/data/hard_to_chunk.txt` & `ragdaemon-0.4.2/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/data/hierarchy_graph.json` & `ragdaemon-0.4.2/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.4.2/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/tests/sample/src/interface.py` & `ragdaemon-0.4.2/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/LICENSE` & `ragdaemon-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/README.md` & `ragdaemon-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.1/pyproject.toml` & `ragdaemon-0.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.4.1"
+version = "0.4.2"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.4.1/PKG-INFO` & `ragdaemon-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

