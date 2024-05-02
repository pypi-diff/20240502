# Comparing `tmp/izihawa_textparser-0.1.98.tar.gz` & `tmp/izihawa_textparser-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_textparser-0.1.98.tar", max compression
+gzip compressed data, was "izihawa_textparser-0.1.99.tar", max compression
```

## Comparing `izihawa_textparser-0.1.98.tar` & `izihawa_textparser-0.1.99.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       21 2023-11-24 08:41:50.733970 izihawa_textparser-0.1.98/README.md
--rw-r--r--   0        0        0      321 2024-02-12 13:56:57.317339 izihawa_textparser-0.1.98/izihawa_textparser/__init__.py
--rw-r--r--   0        0        0     7012 2024-02-12 18:11:12.135839 izihawa_textparser-0.1.98/izihawa_textparser/_document_chunker.py
--rw-r--r--   0        0        0     3673 2024-02-09 12:58:35.182450 izihawa_textparser-0.1.98/izihawa_textparser/_epub.py
--rw-r--r--   0        0        0     9293 2023-12-19 10:37:24.202586 izihawa_textparser-0.1.98/izihawa_textparser/_grobid.py
--rw-r--r--   0        0        0    10779 2024-02-04 14:33:36.024020 izihawa_textparser-0.1.98/izihawa_textparser/_pubmed.py
--rw-r--r--   0        0        0     6626 2024-02-12 13:48:12.799720 izihawa_textparser-0.1.98/izihawa_textparser/_text_splitters.py
--rw-r--r--   0        0        0     2654 2023-12-15 19:39:08.576686 izihawa_textparser-0.1.98/izihawa_textparser/cli.py
--rw-r--r--   0        0        0     7081 2024-02-12 14:36:07.918580 izihawa_textparser-0.1.98/izihawa_textparser/utils.py
--rw-r--r--   0        0        0      744 2024-02-12 18:11:35.388750 izihawa_textparser-0.1.98/pyproject.toml
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 izihawa_textparser-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-11-24 08:41:50.733970 izihawa_textparser-0.1.99/README.md
+-rw-r--r--   0        0        0      321 2024-02-12 13:56:57.317339 izihawa_textparser-0.1.99/izihawa_textparser/__init__.py
+-rw-r--r--   0        0        0     6875 2024-02-12 18:24:44.784258 izihawa_textparser-0.1.99/izihawa_textparser/_document_chunker.py
+-rw-r--r--   0        0        0     3673 2024-02-09 12:58:35.182450 izihawa_textparser-0.1.99/izihawa_textparser/_epub.py
+-rw-r--r--   0        0        0     9293 2023-12-19 10:37:24.202586 izihawa_textparser-0.1.99/izihawa_textparser/_grobid.py
+-rw-r--r--   0        0        0    10779 2024-02-04 14:33:36.024020 izihawa_textparser-0.1.99/izihawa_textparser/_pubmed.py
+-rw-r--r--   0        0        0     6626 2024-02-12 13:48:12.799720 izihawa_textparser-0.1.99/izihawa_textparser/_text_splitters.py
+-rw-r--r--   0        0        0     2654 2023-12-15 19:39:08.576686 izihawa_textparser-0.1.99/izihawa_textparser/cli.py
+-rw-r--r--   0        0        0     7081 2024-02-12 14:36:07.918580 izihawa_textparser-0.1.99/izihawa_textparser/utils.py
+-rw-r--r--   0        0        0      744 2024-02-12 18:31:00.103719 izihawa_textparser-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 izihawa_textparser-0.1.99/PKG-INFO
```

### Comparing `izihawa_textparser-0.1.98/izihawa_textparser/_document_chunker.py` & `izihawa_textparser-0.1.99/izihawa_textparser/_document_chunker.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,19 +60,20 @@
     if a.chunk_id > b.chunk_id:
         t = a
         a = b
         b = t
     assert b.chunk_id == a.chunk_id + 1
     new_chunk = Chunk(**dataclasses.asdict(a))
     new_chunk.length = b.start_index - a.start_index + b.length
+    new_chunk.text = a.text + '\n\n' + b.text
     return new_chunk
 
 
 def _is_table(text: str):
-    return '\\being{tabular}' in text
+    return '\\begin{tabular}' in text
 
 
 def _is_figure_header(text: str):
     return bool(re.search(r'[Tt]ab(le|\.)', text))
 
 
 class DocumentChunker:
@@ -122,17 +123,22 @@
                 remove_markdown(page_content, remove_tables=self._remove_tables),
                 extra_whitespace=True,
                 dashes=True,
                 bullets=True,
                 trailing_punctuation=True,
             )
             title_parts = extract_title_parts(document, split)
-
             parts = [chunk_text]
 
+            if self._add_metadata:
+                parts += f'TITLE: {" ".join(title_parts)}'
+            if self._add_year and 'issued_at' in document and document['issued_at'] != -62135596800:
+                issued_at = datetime.fromtimestamp(document['issued_at'], tz=None)
+                parts += f"YEAR: {issued_at.year}"
+
             chunk = Chunk(
                 document_id=document['id'],
                 field=field,
                 chunk_id=chunk_id,
                 start_index=split.metadata["start_index"],
                 length=len(page_content),
                 issued_at=document.get('issued_at'),
@@ -145,31 +151,20 @@
             if any(
                 [((title_part.lower() in BANNED_SECTIONS)
                   or (bool(BANNED_SECTION_PREFIXES_REGEXP.match(title_part.lower()))))
                  for title_part in title_parts]
             ):
                 continue
 
-            if chunks:
-                print('has_chunks')
-                print(
-                    chunk.text,
-                    _is_table(chunk.text),
-                    _is_figure_header(chunks[-1].text),
-                    _is_figure_header(chunk.text),
-                    _is_table(chunks[-1].text)
-                )
-                if _is_table(chunk.text) and _is_figure_header(chunks[-1].text):
-                    title_parts.append(chunks[-1].text)
-                    chunk = merge_chunks(chunks[-1], chunk)
-                    chunks.pop(len(chunks) - 1)
-                elif _is_figure_header(chunk.text) and _is_table(chunks[-1].text):
-                    chunk = merge_chunks(chunks[-1], chunk)
-                    title_parts.append(chunk.text)
-                    chunks.pop(len(chunks) - 1)
+            if chunks and (
+                (_is_table(chunk.text) and _is_figure_header(chunks[-1].text))
+                or (_is_figure_header(chunk.text) and _is_table(chunks[-1].text))
+            ):
+                chunk = merge_chunks(chunks[-1], chunk)
+                chunks.pop(len(chunks) - 1)
 
             if self._add_metadata:
                 chunk.text += '\n' + f'TITLE: {" ".join(title_parts)}'
             if self._add_year and 'issued_at' in document and document['issued_at'] != -62135596800:
                 issued_at = datetime.fromtimestamp(document['issued_at'], tz=None)
                 chunk.text += '\n' + f"YEAR: {issued_at.year}"
```

### Comparing `izihawa_textparser-0.1.98/izihawa_textparser/_epub.py` & `izihawa_textparser-0.1.99/izihawa_textparser/_epub.py`

 * *Files identical despite different names*

### Comparing `izihawa_textparser-0.1.98/izihawa_textparser/_grobid.py` & `izihawa_textparser-0.1.99/izihawa_textparser/_grobid.py`

 * *Files identical despite different names*

### Comparing `izihawa_textparser-0.1.98/izihawa_textparser/_pubmed.py` & `izihawa_textparser-0.1.99/izihawa_textparser/_pubmed.py`

 * *Files identical despite different names*

### Comparing `izihawa_textparser-0.1.98/izihawa_textparser/_text_splitters.py` & `izihawa_textparser-0.1.99/izihawa_textparser/_text_splitters.py`

 * *Files identical despite different names*

### Comparing `izihawa_textparser-0.1.98/izihawa_textparser/cli.py` & `izihawa_textparser-0.1.99/izihawa_textparser/cli.py`

 * *Files identical despite different names*

### Comparing `izihawa_textparser-0.1.98/izihawa_textparser/utils.py` & `izihawa_textparser-0.1.99/izihawa_textparser/utils.py`

 * *Files identical despite different names*

### Comparing `izihawa_textparser-0.1.98/pyproject.toml` & `izihawa_textparser-0.1.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "izihawa_textparser"
-version = "0.1.98"
+version = "0.1.99"
 description = ""
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `izihawa_textparser-0.1.98/PKG-INFO` & `izihawa_textparser-0.1.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa_textparser
-Version: 0.1.98
+Version: 0.1.99
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

