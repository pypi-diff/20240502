# Comparing `tmp/pysideprocessing-0.0.5.tar.gz` & `tmp/pysideprocessing-0.0.6.tar.gz`

## Comparing `pysideprocessing-0.0.5.tar` & `pysideprocessing-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/__init__.py
--rw-r--r--   0        0        0     7607 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/color.py
--rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/papplet.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/pconstants.py
--rw-r--r--   0        0        0    16518 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/pgraphics.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/pimage.py
--rw-r--r--   0        0        0    14511 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/pwidget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/src/pysideprocessing/py.typed
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/LICENSE
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/README.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pysideprocessing-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/src/pysideprocessing/__about__.py
+-rw-r--r--   0        0        0     7607 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/src/pysideprocessing/color.py
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/src/pysideprocessing/papplet.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/src/pysideprocessing/pconstants.py
+-rw-r--r--   0        0        0    18318 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/src/pysideprocessing/pgraphics.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/src/pysideprocessing/pimage.py
+-rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/src/pysideprocessing/pwidget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/src/pysideprocessing/py.typed
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/LICENSE
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/README.md
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 pysideprocessing-0.0.6/PKG-INFO
```

### Comparing `pysideprocessing-0.0.5/src/pysideprocessing/color.py` & `pysideprocessing-0.0.6/src/pysideprocessing/color.py`

 * *Files identical despite different names*

### Comparing `pysideprocessing-0.0.5/src/pysideprocessing/pconstants.py` & `pysideprocessing-0.0.6/src/pysideprocessing/pconstants.py`

 * *Files identical despite different names*

### Comparing `pysideprocessing-0.0.5/src/pysideprocessing/pgraphics.py` & `pysideprocessing-0.0.6/src/pysideprocessing/pgraphics.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 __version__ = "0.0.3" # 2023.11
 __author__ = "S. Gebert <nomisge @ live . de>"
 __all__ = ['PGraphics', 'Graphics', 'Paintable']
 
 import pysideprocessing.pconstants as pc
 from pysideprocessing.color import color
 
-from PySide6.QtGui import QPainter, QPixmap, QImage, QPen, QBrush, QPolygon, QColor
+from PySide6.QtGui import QPainter, QPixmap, QImage, QPen, QBrush, QPolygon, QColor, QFont
 from PySide6.QtCore import Qt, QPoint
 from abc import ABC, abstractmethod
 from functools import wraps, singledispatchmethod
 
 def shape_painter(method):
     @wraps(method)
     def _impl(self,*method_args, **method_kwargs):
         #TODO: !Speedup maybe by calling begin / end less often?
-        self._painter.begin(self._paint_device.get_paint_device())
-        self._painter.setPen(self._pen if self._stroke else Qt.NoPen) # type: ignore[attr-defined]
-        self._painter.setBrush(self._brush if self._fill else Qt.NoBrush) # type: ignore[attr-defined]
+        self._painter.begin(self._paint_device.get_paint_device()) # pylint: disable=protected-access
+        self._painter.setPen(self._pen if self._stroke else Qt.NoPen) # pylint: disable=protected-access # type: ignore[attr-defined]
+        self._painter.setBrush(self._brush if self._fill else Qt.NoBrush) # pylint: disable=protected-access # type: ignore[attr-defined]
+        self._text_font.setPointSize(self._text_size) # pylint: disable=protected-access
+        self._painter.setFont(self._text_font) # pylint: disable=protected-access
         method(self,*method_args, **method_kwargs)
-        self._painter.end()
+        self._painter.end() # pylint: disable=protected-access
     return _impl
 
+
 class Paintable(ABC):
     @abstractmethod
     def get_paint_device(self) -> QPixmap|QImage:
         raise NotImplementedError
 
 class Graphics(ABC):
 # -- MODE Settings --
@@ -97,14 +100,24 @@
         """       
 
     @abstractmethod
     def no_fill(self):
         """Legt fest, dass die Formen nicht gefüllt werden sollen.
         """
 
+    @abstractmethod
+    def text_font(self, font: str):
+        """Legt die Schriftart fest, in der Text gedruckt wird.
+        """
+ 
+    @abstractmethod
+    def text_size(self, size: int):
+        """Legt die Schriftgröße fest, in der Text gedruckt wird.
+        """
+        
 # -- Background operations
     @abstractmethod
     def background(self, backgroundcolor: color):
         """Sets the color used for the background of the Processing window.
             
         The default background is light gray. This function is
         typically used within **draw()** to clear the display window at the
@@ -286,28 +299,48 @@
         y2 : int
             meist die y-Koordinate des 2. Punkts.
         x3 : int
             meist die x-Koordinate des 3. Punkts.
         y3 : int
             meist die y-Koordinate des 3. Punkts.
         """
+        
+    @abstractmethod        
+    def text(self, s:str, x:int, y:int):        
+        """Gibt einen Text an den gegebenen Koordinaten aus
+        
+        Zur Ausgabe des Textes wird der ausgewaehlte Font verwendet. Dieser muss vorher mit {@link #textFont(Font) textFont() } festgelegt.
+        
+        Parameters
+        ----------
+        s : str
+            Text, der angezeigt werden soll
+        x : int
+            x-Koordinate des Textanfangs
+        y : int
+            y-Koordinate der Grundlinie des Textes.
+        """
 
 class PGraphics(Graphics):
     _painter: QPainter
     _paint_device: Paintable
     
     _rect_mode: int
     _ellipse_mode: int
     
     _background: int
     
     _stroke: bool
     _pen: QPen
     _fill: bool
     _brush: QBrush
+     
+    _text_font: QFont
+    _text_size: int
+    _text_align: int
     
     def __init__(self, paint_device: Paintable):
 #         super().__init__()
         self._painter = QPainter()
         self._paint_device = paint_device
         
         self._background = 0xffd3d3d3
@@ -317,14 +350,19 @@
         self._pen = QPen()
         self._pen.setWidth(4)
         self._pen.setColor(QColor.fromRgba(int(color("black"))))
         
         self._fill = True
         self._brush = QBrush(Qt.SolidPattern) # type: ignore[attr-defined]
         self._brush.setColor(QColor.fromRgba(int(color("white"))))
+
+        self._text_font = QFont()
+        self._text_font.setFamily('Times')
+        self._text_font.setBold(False)
+        self._text_size =12
         
         self._rect_mode = pc.CORNER
         self._ellipse_mode = pc.CENTER
                 
     @property
     def painter(self) -> QPainter:
         return self._painter
@@ -357,14 +395,24 @@
         self._fill = True
         self._brush.setColor(QColor.fromRgba(int(fillcolor)))
 
     def no_fill(self):
 #         self._brush = 
         self._fill = False
 
+    def text_font(self, font: str):
+        new_font = QFont()
+        new_font.setFamily('Times')
+        new_font.setBold(False)
+        self._text_font = new_font
+        #TODO: create font by string or some class?
+
+    def text_size(self, size: int):
+        self._text_size = size
+
 # -- Background operations
     
     def clear(self):
         self._paint_device.get_paint_device().fill(QColor.fromRgba(self._background))
     
     @singledispatchmethod
     def background(self, backgroundcolor: color): # type: ignore[override]
@@ -406,8 +454,13 @@
         self._painter.drawRect(x,y,extend,extend)
     
     @shape_painter
     def triangle(self, x1:int, y1:int,x2:int,y2:int, x3:int, y3:int):
         p = QPolygon.fromList([QPoint(x1,y1), QPoint(x2,y2), QPoint(x3,y3)])
 #         p = p << QPoint(x1,y1) << QPoint(x2,y2) << QPoint(x3,y3)
         self._painter.drawPolygon(p)
-        
+
+    @shape_painter
+    def text(self, s:str, x:int, y:int):
+        self._painter.drawText(x,y, s)
+        #TODO: handle different inputs, e.g. with more parameters...
+
```

### Comparing `pysideprocessing-0.0.5/src/pysideprocessing/pimage.py` & `pysideprocessing-0.0.6/src/pysideprocessing/pimage.py`

 * *Files identical despite different names*

### Comparing `pysideprocessing-0.0.5/src/pysideprocessing/pwidget.py` & `pysideprocessing-0.0.6/src/pysideprocessing/pwidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -317,45 +317,18 @@
     @image_modification
     def square(self, x:int, y:int, extend:int):
         self._graphics.square(x,y,extend)       
  
     @image_modification
     def triangle(self, x1:int, y1:int,x2:int,y2:int, x3:int, y3:int):
         self._graphics.triangle(x1,y1,x2,y2,x3,y3)
-       
-# --- Schriftdarstellung ---
-    @image_modification
-    def draw_text(self, s:str, x:int, y:int):
-        """Gibt einen Text an den gegebenen Koordinaten aus
-        
-        Zur Ausgabe des Textes wird der ausgewaehlte Font verwendet. Dieser muss vorher mit {@link #textFont(Font) textFont() } festgelegt.
-        
-        Parameters
-        ----------
-        s : str
-            Text, der angezeigt werden soll
-        x : int
-            x-Koordinate des Textanfangs
-        y : int
-            y-Koordinate der Grundlinie des Textes.
-     """
-        print(f"TEXT PRINTING: {s}, {x}, {y}")
-        raise NotImplementedError()
-    
-    def text_font(self, font): #TODO font type?
-        """Legt die Schriftart fuer Textausgaben fest.
         
-        Jeder uebliche Java-Font kann verwendet werden. Er kann mit z.B. Font f = new Font( "Arial", Font.PLAIN, 14 ); definiert werden. 
-     
-        Parameters
-        ----------
-        font :
-            ein Font-Objekt 
-        """
-        raise NotImplementedError()
+    @image_modification
+    def text(self, s:str, x:int, y:int):
+        self._graphics.text(s,x,y)
 
 # --- Farbfestlegungen ---
     def get(self, x: int, y: int) -> color:
         """Der Farbwert an der Position x,y de"""
         raise NotImplementedError()
  
     def stroke(self, pencolor: color):
@@ -375,14 +348,20 @@
         """
         self._graphics.no_fill()
            
     @image_modification
     def background(self, argb: color):
         self._graphics.background(argb)
         
+    def text_font(self, font: str):
+        self._graphics.text_font(font)
+        
+    def text_size(self, size: int):
+        self._graphics.text_size(size)
+        
 # --- Dateioperationen ---
     def image_mode(self):
         raise NotImplementedError
     
     def create_image(self):
         raise NotImplementedError
 
@@ -445,8 +424,8 @@
         
         self.setCentralWidget(canvas)
         canvas.setup()
         self.draw_loop_timer = QTimer()
         self.draw_loop_timer.setInterval(int(1000/60))
         self.draw_loop_timer.timeout.connect(canvas.draw) # type: ignore[attr-defined]
         self.draw_loop_timer.start()  
-    
+
```

### Comparing `pysideprocessing-0.0.5/.gitignore` & `pysideprocessing-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pysideprocessing-0.0.5/LICENSE` & `pysideprocessing-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysideprocessing-0.0.5/pyproject.toml` & `pysideprocessing-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Natural Language :: English",
     "Topic :: Education",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 dependencies = [
-  "pyside6",
+  "pyside6<=6.6.3.1",
   "numpy",
   "numba",
   "makefun",
 ]
 
 [tool.hatch.version]
 path = "src/pysideprocessing/__about__.py"
```

### Comparing `pysideprocessing-0.0.5/PKG-INFO` & `pysideprocessing-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysideprocessing
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python implementation of processing using pyside6
 Project-URL: Home, https://codeberg.org/nomisge/pysideprocessing
 Project-URL: PyPI-Site, https://pypi.org/project/pysideprocessing/
 Author-email: nomisge <nomisge@live.de>
 License-File: LICENSE
 Keywords: processing,pyside6,qt
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: makefun
 Requires-Dist: numba
 Requires-Dist: numpy
-Requires-Dist: pyside6
+Requires-Dist: pyside6<=6.6.3.1
 Description-Content-Type: text/markdown
 
 # pysideprocessing
 
 Pysideprocessing implements processing.org in the python language with pyside6 as gui component.
 
 Processing.org is a wonderful tool, but it's python version builds upon jython, which lacks a lot of features introduced since python 3 release.
```

