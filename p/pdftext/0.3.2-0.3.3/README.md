# Comparing `tmp/pdftext-0.3.2.tar.gz` & `tmp/pdftext-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.3.2.tar", max compression
+gzip compressed data, was "pdftext-0.3.3.tar", max compression
```

## Comparing `pdftext-0.3.2.tar` & `pdftext-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-04-30 19:12:36.352403 pdftext-0.3.2/LICENSE
--rw-r--r--   0        0        0     7084 2024-04-30 19:12:36.356402 pdftext-0.3.2/README.md
--rw-r--r--   0        0        0     1581 2024-04-30 19:12:36.356402 pdftext-0.3.2/extract_text.py
--rw-r--r--   0        0        0    14097 2024-04-30 19:12:36.356402 pdftext-0.3.2/models/dt.joblib
--rw-r--r--   0        0        0     2144 2024-04-30 19:12:36.356402 pdftext-0.3.2/pdftext/extraction.py
--rw-r--r--   0        0        0     7052 2024-04-30 19:12:36.356402 pdftext-0.3.2/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-04-30 19:12:36.356402 pdftext-0.3.2/pdftext/model.py
--rw-r--r--   0        0        0     3752 2024-04-30 19:12:36.356402 pdftext-0.3.2/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     4707 2024-04-30 19:12:36.356402 pdftext-0.3.2/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     3222 2024-04-30 19:12:36.356402 pdftext-0.3.2/pdftext/postprocessing.py
--rw-r--r--   0        0        0      579 2024-04-30 19:12:36.356402 pdftext-0.3.2/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-04-30 19:12:36.356402 pdftext-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8060 1970-01-01 00:00:00.000000 pdftext-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-05-02 17:27:01.276151 pdftext-0.3.3/LICENSE
+-rw-r--r--   0        0        0     7170 2024-05-02 17:27:01.276151 pdftext-0.3.3/README.md
+-rw-r--r--   0        0        0     1726 2024-05-02 17:27:01.276151 pdftext-0.3.3/extract_text.py
+-rw-r--r--   0        0        0    14097 2024-05-02 17:27:01.280151 pdftext-0.3.3/models/dt.joblib
+-rw-r--r--   0        0        0     2426 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/extraction.py
+-rw-r--r--   0        0        0     7242 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/model.py
+-rw-r--r--   0        0        0     3752 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4653 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     3222 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      579 2024-05-02 17:27:01.280151 pdftext-0.3.3/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-05-02 17:27:01.280151 pdftext-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8146 1970-01-01 00:00:00.000000 pdftext-0.3.3/PKG-INFO
```

### Comparing `pdftext-0.3.2/LICENSE` & `pdftext-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.2/README.md` & `pdftext-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--json` specifies json output
 - `--sort` will attempt to sort in reading order if specified.
 - `--pages` will specify pages (comma separated) to extract
+- `--keep_chars` will keep individual characters in the json output
 
 The output will be a json list, with each item in the list corresponding to a single page in the input pdf (in order).  Each page will include the following keys:
 
 - `bbox` - the page bbox, in `[x1, y1, x2, y2]` format
 - `rotation` - how much the page is rotated, in degrees (`0`, `90`, `180`, or `270`)
 - `page` - the index of the page
 - `blocks` - the blocks that make up the text in the pdf.  Approximately equal to a paragraph.
@@ -80,15 +81,15 @@
 Extract structured blocks and lines:
 
 ```python
 import pypdfium2 as pdfium
 from pdftext.extraction import dictionary_output
 
 pdf = pdfium.PdfDocument(PDF_PATH)
-text = dictionary_output(pdf, sort=False, page_range=[1,2,3]) # Optional arguments explained above
+text = dictionary_output(pdf, sort=False, page_range=[1,2,3], keep_chars=False) # Optional arguments explained above
 ```
 
 If you want more customization, check out the `pdftext.extraction._get_pages` function for a starting point to dig deeper.  pdftext is a pretty thin wrapper around [pypdfium2](https://pypdfium2.readthedocs.io/en/stable/), so you might want to look at the documentation for that as well.
 
 # Benchmarks
 
 I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual character/line/block and bbox information.
```

### Comparing `pdftext-0.3.2/extract_text.py` & `pdftext-0.3.3/extract_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,25 @@
     parser = argparse.ArgumentParser(description="Extract plain text from PDF.  Not guaranteed to be in order.")
     parser.add_argument("pdf_path", type=str, help="Path to the PDF file")
     parser.add_argument("--out_path", type=str, help="Path to the output text file, defaults to stdout", default=None)
     parser.add_argument("--json", action="store_true", help="Output json instead of plain text", default=False)
     parser.add_argument("--sort", action="store_true", help="Attempt to sort the text by reading order", default=False)
     parser.add_argument("--keep_hyphens", action="store_true", help="Keep hyphens in words", default=False)
     parser.add_argument("--pages", type=str, help="Comma separated pages to extract, like 1,2,3", default=None)
+    parser.add_argument("--keep_chars", action="store_true", help="Keep character level information", default=False)
     args = parser.parse_args()
 
     pdf_doc = pdfium.PdfDocument(args.pdf_path)
     pages = None
     if args.pages is not None:
         pages = [int(p) for p in args.pages.split(",")]
         assert all(p <= len(pdf_doc) for p in pages), "Invalid page number(s) provided"
 
     if args.json:
-        text = dictionary_output(pdf_doc, sort=args.sort, page_range=pages)
+        text = dictionary_output(pdf_doc, sort=args.sort, page_range=pages, keep_chars=args.keep_chars)
         text = json.dumps(text)
     else:
         text = plain_text_output(pdf_doc, sort=args.sort, hyphens=args.keep_hyphens, page_range=pages)
 
     if args.out_path is None:
         print(text)
     else:
```

### Comparing `pdftext-0.3.2/models/dt.joblib` & `pdftext-0.3.3/models/dt.joblib`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.2/pdftext/extraction.py` & `pdftext-0.3.3/pdftext/extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     pages = _get_pages(pdf_doc, model, page_range)
     text = []
     for page in pages:
         text.append(merge_text(page, sort=sort, hyphens=hyphens).strip())
     return text
 
 
-def dictionary_output(pdf_doc, sort=False, model=None, page_range=None):
+def dictionary_output(pdf_doc, sort=False, model=None, page_range=None, keep_chars=False):
     pages = _get_pages(pdf_doc, model, page_range)
     for page in pages:
         for block in page["blocks"]:
             bad_keys = [key for key in block.keys() if key not in ["lines", "bbox"]]
             for key in bad_keys:
                 del block[key]
             for line in block["lines"]:
@@ -40,12 +40,18 @@
                 for key in bad_keys:
                     del line[key]
                 for span in line["spans"]:
                     span["bbox"] = unnormalize_bbox(span["bbox"], page["width"], page["height"])
                     span["text"] = postprocess_text(span["text"])
                     span["text"] = handle_hyphens(span["text"], keep_hyphens=True)
 
+                    if not keep_chars:
+                        del span["chars"]
+                    else:
+                        for char in span["chars"]:
+                            char["bbox"] = unnormalize_bbox(char["bbox"], page["width"], page["height"])
+
                 line["bbox"] = unnormalize_bbox(line["bbox"], page["width"], page["height"])
             block["bbox"] = unnormalize_bbox(block["bbox"], page["width"], page["height"])
         if sort:
             page["blocks"] = sort_blocks(page["blocks"])
     return pages
```

### Comparing `pdftext-0.3.2/pdftext/inference.py` & `pdftext-0.3.3/pdftext/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,19 @@
                         min([bbox[1] for bbox in char_bboxes]),
                         max([bbox[2] for bbox in char_bboxes]),
                         max([bbox[3] for bbox in char_bboxes])]
         span["text"] = "".join([char["char"] for char in span["chars"]])
         span["char_start_idx"] = span["chars"][0]["char_idx"]
         span["char_end_idx"] = span["chars"][-1]["char_idx"]
 
-    del span["chars"]
+    # Remove unneeded keys from the characters
+    for char in span["chars"]:
+        del_keys = [k for k in list(char.keys()) if k not in ["char", "bbox"]]
+        for key in del_keys:
+            del char[key]
     line["spans"].append(span)
     span = {"chars": []}
     return span
 
 
 def update_line(block, line):
     block["lines"].append(line)
```

### Comparing `pdftext-0.3.2/pdftext/pdf/chars.py` & `pdftext-0.3.3/pdftext/pdf/chars.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.2/pdftext/pdf/utils.py` & `pdftext-0.3.3/pdftext/pdf/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     y1 = round(y1 * page_height, 1)
     x2 = round(x2 * page_width, 1)
     y2 = round(y2 * page_height, 1)
     return x1, y1, x2, y2
 
 
 def get_fontname(textpage, char_index):
-    n_bytes = settings.FONT_BUFFER_SIZE
+    n_bytes = pdfium_c.FPDFText_GetFontInfo(textpage, char_index, None, 0, None)
     buffer = ctypes.create_string_buffer(n_bytes)
     # Re-interpret the type from char to unsigned short as required by the function
     buffer_ptr = ctypes.cast(buffer, ctypes.POINTER(ctypes.c_ushort))
     flag_buffer = ctypes.c_int()
     flag_ptr = ctypes.pointer(flag_buffer)
     font_info = pdfium_c.FPDFText_GetFontInfo(textpage, char_index, buffer_ptr, n_bytes, flag_ptr)
     if font_info == 0:
@@ -58,21 +58,19 @@
         page_rotation = 1
     elif page_rotation == 180:
         page_rotation = 2
     elif page_rotation == 270:
         page_rotation = 3
     else:
         page_rotation = 0
-    device_x = ctypes.c_int()
-    device_y = ctypes.c_int()
-    device_x_ptr = ctypes.pointer(device_x)
-    device_y_ptr = ctypes.pointer(device_y)
     width = math.ceil(page_width)
     height = math.ceil(page_height)
-    pdfium_c.FPDF_PageToDevice(page, 0, 0, width, height, page_rotation, x, y, device_x_ptr, device_y_ptr)
+    device_x = ctypes.c_int()
+    device_y = ctypes.c_int()
+    pdfium_c.FPDF_PageToDevice(page, 0, 0, width, height, page_rotation, x, y, device_x, device_y)
     x = device_x.value
     y = device_y.value
     return x, y
 
 
 def pdfium_page_bbox_to_device_bbox(page, bbox, page_width, page_height, page_rotation):
     left_bottom = page_to_device(page, *bbox[:2], page_width, page_height, page_rotation)
@@ -131,8 +129,8 @@
     elif angle_deg == 180:
         bbox = [x2, y2, x1, y1]
         bbox = [width - bbox[0], height - bbox[1], width - bbox[2], height - bbox[3]]
     elif angle_deg == 270:
         bbox = rotate_page_bbox(bbox, 90, width, height)
         bbox = rotate_page_bbox(bbox, 180, width, height)
 
-    return bbox
+    return bbox
```

### Comparing `pdftext-0.3.2/pdftext/postprocessing.py` & `pdftext-0.3.3/pdftext/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.2/pdftext/settings.py` & `pdftext-0.3.3/pdftext/settings.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.2/pyproject.toml` & `pdftext-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.3.2"
+version = "0.3.3"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.3.2/PKG-INFO` & `pdftext-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.3.2
+Version: 0.3.3
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -60,14 +60,15 @@
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--json` specifies json output
 - `--sort` will attempt to sort in reading order if specified.
 - `--pages` will specify pages (comma separated) to extract
+- `--keep_chars` will keep individual characters in the json output
 
 The output will be a json list, with each item in the list corresponding to a single page in the input pdf (in order).  Each page will include the following keys:
 
 - `bbox` - the page bbox, in `[x1, y1, x2, y2]` format
 - `rotation` - how much the page is rotated, in degrees (`0`, `90`, `180`, or `270`)
 - `page` - the index of the page
 - `blocks` - the blocks that make up the text in the pdf.  Approximately equal to a paragraph.
@@ -103,15 +104,15 @@
 Extract structured blocks and lines:
 
 ```python
 import pypdfium2 as pdfium
 from pdftext.extraction import dictionary_output
 
 pdf = pdfium.PdfDocument(PDF_PATH)
-text = dictionary_output(pdf, sort=False, page_range=[1,2,3]) # Optional arguments explained above
+text = dictionary_output(pdf, sort=False, page_range=[1,2,3], keep_chars=False) # Optional arguments explained above
 ```
 
 If you want more customization, check out the `pdftext.extraction._get_pages` function for a starting point to dig deeper.  pdftext is a pretty thin wrapper around [pypdfium2](https://pypdfium2.readthedocs.io/en/stable/), so you might want to look at the documentation for that as well.
 
 # Benchmarks
 
 I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual character/line/block and bbox information.
```

