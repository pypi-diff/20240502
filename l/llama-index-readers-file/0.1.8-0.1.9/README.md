# Comparing `tmp/llama_index_readers_file-0.1.8.tar.gz` & `tmp/llama_index_readers_file-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_file-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_readers_file-0.1.9.tar", max compression
```

## Comparing `llama_index_readers_file-0.1.8.tar` & `llama_index_readers_file-0.1.9.tar`

### file list

```diff
@@ -1,48 +1,51 @@
--rw-r--r--   0        0        0       39 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/README.md
--rw-r--r--   0        0        0     1570 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/__init__.py
--rw-r--r--   0        0        0      132 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/docs/__init__.py
--rw-r--r--   0        0        0     6554 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/docs/base.py
--rw-r--r--   0        0        0       84 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/epub/__init__.py
--rw-r--r--   0        0        0     1646 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/epub/base.py
--rw-r--r--   0        0        0       84 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/flat/__init__.py
--rw-r--r--   0        0        0      905 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/flat/base.py
--rw-r--r--   0        0        0       90 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/html/__init__.py
--rw-r--r--   0        0        0     2160 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/html/base.py
--rw-r--r--   0        0        0       87 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/image/__init__.py
--rw-r--r--   0        0        0     4110 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/image/base.py
--rw-r--r--   0        0        0      109 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/image_caption/__init__.py
--rw-r--r--   0        0        0     3029 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/image_caption/base.py
--rw-r--r--   0        0        0      459 2024-03-06 03:53:33.011489 llama_index_readers_file-0.1.8/llama_index/readers/file/image_deplot/README.md
--rw-r--r--   0        0        0      127 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/image_deplot/__init__.py
--rw-r--r--   0        0        0     3132 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/image_deplot/base.py
--rw-r--r--   0        0        0       40 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/image_deplot/requirements.txt
--rw-r--r--   0        0        0      116 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/image_vision_llm/__init__.py
--rw-r--r--   0        0        0     3030 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/image_vision_llm/base.py
--rw-r--r--   0        0        0       87 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/ipynb/__init__.py
--rw-r--r--   0        0        0     1552 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/ipynb/base.py
--rw-r--r--   0        0        0       96 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/markdown/__init__.py
--rw-r--r--   0        0        0     3929 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/markdown/base.py
--rw-r--r--   0        0        0       84 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/mbox/__init__.py
--rw-r--r--   0        0        0     3822 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/mbox/base.py
--rw-r--r--   0        0        0      958 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/paged_csv/README.md
--rw-r--r--   0        0        0      106 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/paged_csv/__init__.py
--rw-r--r--   0        0        0     1418 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/paged_csv/base.py
--rw-r--r--   0        0        0     1099 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/pymu_pdf/README.md
--rw-r--r--   0        0        0      121 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/pymu_pdf/__init__.py
--rw-r--r--   0        0        0     2813 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/pymu_pdf/base.py
--rw-r--r--   0        0        0        8 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/pymu_pdf/requirements.txt
--rw-r--r--   0        0        0       86 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/slides/__init__.py
--rw-r--r--   0        0        0     3782 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/slides/base.py
--rw-r--r--   0        0        0      121 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/tabular/__init__.py
--rw-r--r--   0        0        0     3932 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/tabular/base.py
--rw-r--r--   0        0        0     2560 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/unstructured/README.md
--rw-r--r--   0        0        0      135 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/unstructured/__init__.py
--rw-r--r--   0        0        0     3762 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/unstructured/base.py
--rw-r--r--   0        0        0       18 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/unstructured/requirements.txt
--rw-r--r--   0        0        0      103 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/video_audio/__init__.py
--rw-r--r--   0        0        0     2158 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/video_audio/base.py
--rw-r--r--   0        0        0      666 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/xml/README.md
--rw-r--r--   0        0        0      108 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/xml/__init__.py
--rw-r--r--   0        0        0     2822 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/llama_index/readers/file/xml/base.py
--rw-r--r--   0        0        0     2489 2024-03-06 03:53:33.015489 llama_index_readers_file-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llama_index_readers_file-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/README.md
+-rw-r--r--   0        0        0     1638 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/__init__.py
+-rw-r--r--   0        0        0      132 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/docs/__init__.py
+-rw-r--r--   0        0        0     6554 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/docs/base.py
+-rw-r--r--   0        0        0       84 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/epub/__init__.py
+-rw-r--r--   0        0        0     1646 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/epub/base.py
+-rw-r--r--   0        0        0       84 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/flat/__init__.py
+-rw-r--r--   0        0        0      905 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/flat/base.py
+-rw-r--r--   0        0        0       90 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/html/__init__.py
+-rw-r--r--   0        0        0     2160 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/html/base.py
+-rw-r--r--   0        0        0       87 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image/__init__.py
+-rw-r--r--   0        0        0     4110 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image/base.py
+-rw-r--r--   0        0        0      109 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image_caption/__init__.py
+-rw-r--r--   0        0        0     3029 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image_caption/base.py
+-rw-r--r--   0        0        0      459 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image_deplot/README.md
+-rw-r--r--   0        0        0      127 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image_deplot/__init__.py
+-rw-r--r--   0        0        0     3132 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image_deplot/base.py
+-rw-r--r--   0        0        0       40 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image_deplot/requirements.txt
+-rw-r--r--   0        0        0      116 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image_vision_llm/__init__.py
+-rw-r--r--   0        0        0     3030 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/image_vision_llm/base.py
+-rw-r--r--   0        0        0       87 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/ipynb/__init__.py
+-rw-r--r--   0        0        0     1552 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/ipynb/base.py
+-rw-r--r--   0        0        0       96 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/markdown/__init__.py
+-rw-r--r--   0        0        0     3929 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/markdown/base.py
+-rw-r--r--   0        0        0       84 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/mbox/__init__.py
+-rw-r--r--   0        0        0     3822 2024-03-09 12:21:25.492312 llama_index_readers_file-0.1.9/llama_index/readers/file/mbox/base.py
+-rw-r--r--   0        0        0      958 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/paged_csv/README.md
+-rw-r--r--   0        0        0      106 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/paged_csv/__init__.py
+-rw-r--r--   0        0        0     1418 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/paged_csv/base.py
+-rw-r--r--   0        0        0     1099 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/pymu_pdf/README.md
+-rw-r--r--   0        0        0      121 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/pymu_pdf/__init__.py
+-rw-r--r--   0        0        0     2813 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/pymu_pdf/base.py
+-rw-r--r--   0        0        0        8 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/pymu_pdf/requirements.txt
+-rw-r--r--   0        0        0      726 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/rtf/README.md
+-rw-r--r--   0        0        0       81 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/rtf/__init__.py
+-rw-r--r--   0        0        0     1026 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/rtf/base.py
+-rw-r--r--   0        0        0       86 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/slides/__init__.py
+-rw-r--r--   0        0        0     3782 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/slides/base.py
+-rw-r--r--   0        0        0      121 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/tabular/__init__.py
+-rw-r--r--   0        0        0     3932 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/tabular/base.py
+-rw-r--r--   0        0        0     2560 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/unstructured/README.md
+-rw-r--r--   0        0        0      135 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/unstructured/__init__.py
+-rw-r--r--   0        0        0     3762 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/unstructured/base.py
+-rw-r--r--   0        0        0       18 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/unstructured/requirements.txt
+-rw-r--r--   0        0        0      103 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/video_audio/__init__.py
+-rw-r--r--   0        0        0     2158 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/video_audio/base.py
+-rw-r--r--   0        0        0      666 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/xml/README.md
+-rw-r--r--   0        0        0      108 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/xml/__init__.py
+-rw-r--r--   0        0        0     2822 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/llama_index/readers/file/xml/base.py
+-rw-r--r--   0        0        0     2532 2024-03-09 12:21:25.496312 llama_index_readers_file-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 llama_index_readers_file-0.1.9/PKG-INFO
```

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/__init__.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from llama_index.readers.file.paged_csv import PagedCSVReader
 from llama_index.readers.file.pymu_pdf import PyMuPDFReader
 from llama_index.readers.file.slides import PptxReader
 from llama_index.readers.file.tabular import PandasCSVReader, CSVReader
 from llama_index.readers.file.unstructured import UnstructuredReader
 from llama_index.readers.file.video_audio import VideoAudioReader
 from llama_index.readers.file.xml import XMLReader
+from llama_index.readers.file.rtf import RTFReader
 
 __all__ = [
     "DocxReader",
     "HWPReader",
     "PDFReader",
     "EpubReader",
     "FlatReader",
@@ -35,8 +36,9 @@
     "VideoAudioReader",
     "UnstructuredReader",
     "PyMuPDFReader",
     "ImageTabularChartReader",
     "XMLReader",
     "PagedCSVReader",
     "CSVReader",
+    "RTFReader",
 ]
```

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/docs/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/docs/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/epub/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/epub/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/flat/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/flat/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/html/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/html/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/image/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/image/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/image_caption/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/image_caption/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/image_deplot/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/image_deplot/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/image_vision_llm/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/image_vision_llm/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/ipynb/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/ipynb/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/markdown/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/markdown/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/mbox/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/mbox/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/paged_csv/README.md` & `llama_index_readers_file-0.1.9/llama_index/readers/file/paged_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/paged_csv/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/paged_csv/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/pymu_pdf/README.md` & `llama_index_readers_file-0.1.9/llama_index/readers/file/pymu_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/pymu_pdf/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/pymu_pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/slides/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/slides/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/tabular/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/tabular/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/unstructured/README.md` & `llama_index_readers_file-0.1.9/llama_index/readers/file/unstructured/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/unstructured/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/video_audio/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/video_audio/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/xml/README.md` & `llama_index_readers_file-0.1.9/llama_index/readers/file/xml/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/llama_index/readers/file/xml/base.py` & `llama_index_readers_file-0.1.9/llama_index/readers/file/xml/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_file-0.1.8/pyproject.toml` & `llama_index_readers_file-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 MarkdownReader = "hursh-desai"
 MboxReader = "llama-index"
 PDFReader = "ravi03071991"
 PagedCSVReader = "thejessezhang"
 PandasCSVReader = "ephe-meral"
 PptxReader = "thejessezhang"
 PyMuPDFReader = "iamarunbrahma"
+RTFReader = "FunkyOz"
 UnstructuredReader = "thejessezhang"
 VideoAudioReader = "llama-index"
 XMLReader = "mmaatouk"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
@@ -45,23 +46,24 @@
 description = "llama-index readers file integration"
 exclude = ["**/BUILD"]
 keywords = ["10k", "10q", "chart", "eml", "figure", "html", "hwp", "image", "invoice", "ipynb", "jupyter", "notebook", "pdf", "pymupdf", "receipt", "sec", "spreadsheet", "tabular", "unstructured.io", "yaml", "yml"]
 license = "MIT"
 maintainers = ["FarisHijazi", "Haowjy", "ephe-meral", "hursh-desai", "iamarunbrahma", "jon-chuang", "mmaatouk", "ravi03071991", "sangwongenip", "thejessezhang"]
 name = "llama-index-readers-file"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 pymupdf = "^1.23.21"
 bs4 = "^0.0.2"
 beautifulsoup4 = "^4.12.3"
 pypdf = "^4.0.1"
+striprtf = "^0.0.26"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_readers_file-0.1.8/PKG-INFO` & `llama_index_readers_file-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-file
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index readers file integration
 License: MIT
 Keywords: 10k,10q,chart,eml,figure,html,hwp,image,invoice,ipynb,jupyter,notebook,pdf,pymupdf,receipt,sec,spreadsheet,tabular,unstructured.io,yaml,yml
 Author: Your Name
 Author-email: you@example.com
 Maintainer: FarisHijazi
 Requires-Python: >=3.8.1,<4.0
@@ -14,11 +14,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: pymupdf (>=1.23.21,<2.0.0)
 Requires-Dist: pypdf (>=4.0.1,<5.0.0)
+Requires-Dist: striprtf (>=0.0.26,<0.0.27)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Readers Integration: File
```

