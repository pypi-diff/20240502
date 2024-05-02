# Comparing `tmp/gunshotmatch_reports-0.5.0.tar.gz` & `tmp/gunshotmatch_reports-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunshotmatch_reports-0.5.0.tar", last modified: Tue Apr 30 14:35:11 2024, max compression
+gzip compressed data, was "gunshotmatch_reports-0.6.0.tar", last modified: Thu May  2 09:48:43 2024, max compression
```

## Comparing `gunshotmatch_reports-0.5.0.tar` & `gunshotmatch_reports-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 14:35:11.768609 gunshotmatch_reports-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-30 14:35:11.772609 gunshotmatch_reports-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-30 14:35:11.772609 gunshotmatch_reports-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-30 14:35:11.772609 gunshotmatch_reports-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 14:35:11.772609 gunshotmatch_reports-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 09:48:43.093726 gunshotmatch_reports-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-02 09:48:43.097726 gunshotmatch_reports-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-02 09:48:43.097726 gunshotmatch_reports-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-02 09:48:43.097726 gunshotmatch_reports-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 09:48:43.097726 gunshotmatch_reports-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-02 09:48:20.581642 gunshotmatch_reports-0.6.0/gunshotmatch_reports/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-02 09:48:20.581642 gunshotmatch_reports-0.6.0/gunshotmatch_reports/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-02 09:48:20.581642 gunshotmatch_reports-0.6.0/gunshotmatch_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:48:20.581642 gunshotmatch_reports-0.6.0/gunshotmatch_reports/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-02 09:48:20.581642 gunshotmatch_reports-0.6.0/gunshotmatch_reports/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-05-02 09:48:20.581642 gunshotmatch_reports-0.6.0/gunshotmatch_reports/peaks.py
```

### Comparing `gunshotmatch_reports-0.5.0/LICENSE` & `gunshotmatch_reports-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.5.0/README.rst` & `gunshotmatch_reports-0.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-reports
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.5.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.6.0
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_reports-0.5.0/PKG-INFO` & `gunshotmatch_reports-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.2
 Name: gunshotmatch-reports
-Version: 0.5.0
+Version: 0.6.0
 Summary: PDF Report Generation for GunShotMatch.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Home-page: https://github.com/GunShotMatch/gunshotmatch-reports
 Project-URL: Issue Tracker, https://github.com/GunShotMatch/gunshotmatch-reports/issues
 Project-URL: Source Code, https://github.com/GunShotMatch/gunshotmatch-reports
 Project-URL: Documentation, https://gunshotmatch-reports.readthedocs.io/en/latest
@@ -117,15 +117,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-reports
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.5.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.6.0
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_reports-0.5.0/pyproject.toml` & `gunshotmatch_reports-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "gunshotmatch-reports"
-version = "0.5.0"
+version = "0.6.0"
 description = "PDF Report Generation for GunShotMatch."
 readme = "README.rst"
 keywords = []
 dynamic = []
 dependencies = [
     "domdf-python-tools>=3.8.0.post2",
     "libgunshotmatch>=0.5.0",
```

### Comparing `gunshotmatch_reports-0.5.0/gunshotmatch_reports/chromatogram.py` & `gunshotmatch_reports-0.6.0/gunshotmatch_reports/chromatogram.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
 # 3rd party
 from domdf_python_tools.paths import PathLike
 from libgunshotmatch.project import Project
 from libgunshotmatch_mpl.chromatogram import draw_chromatograms
 from matplotlib import pyplot as plt  # type: ignore[import]
 
+# this package
+from gunshotmatch_reports.utils import save_pdf
+
 __all__ = ["build_chromatogram_report"]
 
 
 def build_chromatogram_report(project: Project, pdf_filename: Optional[PathLike] = None) -> str:
 	"""
 	Construct a chromatogram report for the given project and write to the chosen file.
 
@@ -52,10 +55,10 @@
 		pdf_filename = project.name + "_chromatogram.pdf"
 	else:
 		pdf_filename = os.fspath(pdf_filename)
 
 	fig = plt.figure(layout="constrained", figsize=(11.7, 8.3))
 	axes = fig.subplots(len(project.datafile_data), 1, sharex=True)
 	draw_chromatograms(project, fig, axes)
-	fig.savefig(pdf_filename)
+	save_pdf(fig, pdf_filename)
 
 	return pdf_filename
```

### Comparing `gunshotmatch_reports-0.5.0/gunshotmatch_reports/utils.py` & `gunshotmatch_reports-0.6.0/gunshotmatch_reports/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
-from io import BytesIO
+from io import BytesIO, StringIO
 from typing import List, Tuple, TypeVar
 
 # 3rd party
-from matplotlib import pyplot as plt  # type: ignore[import]
+import matplotlib  # type: ignore[import]
+from domdf_python_tools.paths import PathPlus
+from domdf_python_tools.typing import PathLike
+from matplotlib import pyplot as plt
 from matplotlib.figure import Figure  # type: ignore[import]
 from reportlab.graphics.shapes import Drawing  # type: ignore[import]
 from svglib.svglib import svg2rlg  # type: ignore[import]
 
-__all__ = ["extend_list", "figure_to_drawing", "scale"]
+__all__ = ["extend_list", "figure_to_drawing", "scale", "save_pdf", "save_svg"]
 
 
 def scale(drawing: Drawing, scale: float) -> Drawing:
 	"""
 	Scale reportlab.graphics.shapes.Drawing() object while maintaining aspect ratio.
 
 	:param drawing:
@@ -85,7 +88,43 @@
 	fillsize = length - len(l)
 	for _ in range(fillsize):
 		l.append(fillvalue)
 
 	assert len(l) == length
 
 	return l
+
+
+def save_pdf(fig: Figure, filename: PathLike) -> None:
+	"""
+	Save a PDF without a creation date.
+
+	:param fig:
+	:param filename:
+
+	.. versionadded:: 0.6.0
+	"""
+
+	fig.savefig(filename, format="pdf", metadata={"CreationDate": None})
+
+
+def save_svg(fig: Figure, filename: PathLike) -> None:
+	"""
+	Save an SVG with fixed hashsalt and without a creation date.
+
+	:param fig:
+	:param filename:
+
+	.. versionadded:: 0.6.0
+	"""
+
+	filename_p = PathPlus(filename)
+
+	current_hashsalt = matplotlib.rcParams.get("svg.hashsalt")
+
+	try:
+		matplotlib.rcParams["svg.hashsalt"] = filename_p.name
+		s = StringIO()
+		fig.savefig(s, format="svg", metadata={"Date": None})
+		filename_p.write_clean(s.getvalue())
+	finally:
+		matplotlib.rcParams["svg.hashsalt"] = current_hashsalt
```

### Comparing `gunshotmatch_reports-0.5.0/gunshotmatch_reports/__init__.py` & `gunshotmatch_reports-0.6.0/gunshotmatch_reports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2024 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.5.0"
+__version__: str = "0.6.0"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `gunshotmatch_reports-0.5.0/gunshotmatch_reports/alignment.py` & `gunshotmatch_reports-0.6.0/gunshotmatch_reports/alignment.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.5.0/gunshotmatch_reports/peaks.py` & `gunshotmatch_reports-0.6.0/gunshotmatch_reports/peaks.py`

 * *Files identical despite different names*

