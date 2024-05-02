# Comparing `tmp/mnist_separator-1.0.1.tar.gz` & `tmp/mnist_separator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnist_separator-1.0.1.tar", max compression
+gzip compressed data, was "mnist_separator-1.0.2.tar", max compression
```

## Comparing `mnist_separator-1.0.1.tar` & `mnist_separator-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      227 2024-04-12 10:18:12.545299 mnist_separator-1.0.1/README.md
--rw-r--r--   0        0        0     6148 2024-05-01 10:18:04.995684 mnist_separator-1.0.1/mnist_separator/.DS_Store
--rw-r--r--   0        0        0      153 2024-04-14 09:35:52.610037 mnist_separator-1.0.1/mnist_separator/__init__.py
--rw-r--r--   0        0        0     6148 2024-05-01 10:16:49.451202 mnist_separator-1.0.1/mnist_separator/src/.DS_Store
--rw-r--r--   0        0        0      553 2024-05-01 09:09:55.015615 mnist_separator-1.0.1/mnist_separator/src/clean_all.py
--rw-r--r--   0        0        0     2820 2024-05-01 09:09:54.914737 mnist_separator-1.0.1/mnist_separator/src/convert_data.py
--rw-r--r--   0        0        0     2076 2024-05-01 09:09:54.986197 mnist_separator-1.0.1/mnist_separator/src/create_dirs.py
--rw-r--r--   0        0        0      742 2024-05-01 09:09:54.933525 mnist_separator-1.0.1/mnist_separator/src/get_similarity.py
--rw-r--r--   0        0        0     1263 2024-05-01 09:09:54.943065 mnist_separator-1.0.1/mnist_separator/src/get_similarity_group.py
--rw-r--r--   0        0        0      690 2024-05-01 09:09:55.006521 mnist_separator-1.0.1/mnist_separator/src/glbl.py
--rw-r--r--   0        0        0     3103 2024-05-01 09:09:54.937102 mnist_separator-1.0.1/mnist_separator/src/go.py
--rw-r--r--   0        0        0     1894 2024-05-01 09:09:54.920794 mnist_separator-1.0.1/mnist_separator/src/import_mnist.py
--rw-r--r--   0        0        0      181 2024-05-01 09:09:55.010646 mnist_separator-1.0.1/mnist_separator/src/init.py
--rw-r--r--   0        0        0     1386 2024-05-01 09:09:54.917665 mnist_separator-1.0.1/mnist_separator/src/save_result.py
--rw-r--r--   0        0        0      825 2024-05-01 09:09:54.992801 mnist_separator-1.0.1/mnist_separator/src/timer.py
--rw-r--r--   0        0        0     4104 2024-05-01 09:09:55.002347 mnist_separator-1.0.1/mnist_separator/src/to_canonical.py
--rw-r--r--   0        0        0      663 2024-05-01 09:09:54.974542 mnist_separator-1.0.1/mnist_separator/src/utils_directory.py
--rw-r--r--   0        0        0      600 2024-05-01 09:09:54.951657 mnist_separator-1.0.1/mnist_separator/src/utils_list.py
--rw-r--r--   0        0        0      497 2024-05-01 10:50:28.880241 mnist_separator-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mnist_separator-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-04-12 10:18:12.545299 mnist_separator-1.0.2/README.md
+-rw-r--r--   0        0        0     6148 2024-05-02 14:50:49.508177 mnist_separator-1.0.2/mnist_separator/.DS_Store
+-rw-r--r--   0        0        0      177 2024-05-02 14:31:44.020164 mnist_separator-1.0.2/mnist_separator/__init__.py
+-rw-r--r--   0        0        0     6148 2024-05-02 14:58:00.574752 mnist_separator-1.0.2/mnist_separator/src/.DS_Store
+-rw-r--r--   0        0        0      553 2024-05-02 03:22:36.857384 mnist_separator-1.0.2/mnist_separator/src/clean_all.py
+-rw-r--r--   0        0        0     2820 2024-05-02 03:22:36.842248 mnist_separator-1.0.2/mnist_separator/src/convert_data.py
+-rw-r--r--   0        0        0     2076 2024-05-02 03:22:36.911146 mnist_separator-1.0.2/mnist_separator/src/create_dirs.py
+-rw-r--r--   0        0        0      722 2024-05-02 03:22:36.863875 mnist_separator-1.0.2/mnist_separator/src/get_similarity.py
+-rw-r--r--   0        0        0     1263 2024-05-02 03:22:36.903410 mnist_separator-1.0.2/mnist_separator/src/get_similarity_group.py
+-rw-r--r--   0        0        0      690 2024-05-02 03:22:36.899832 mnist_separator-1.0.2/mnist_separator/src/glbl.py
+-rw-r--r--   0        0        0     3103 2024-05-02 03:22:36.887208 mnist_separator-1.0.2/mnist_separator/src/go.py
+-rw-r--r--   0        0        0      181 2024-05-02 03:22:36.821442 mnist_separator-1.0.2/mnist_separator/src/init.py
+-rw-r--r--   0        0        0      970 2024-05-02 14:35:43.534234 mnist_separator-1.0.2/mnist_separator/src/load_data.py
+-rw-r--r--   0        0        0     1012 2024-05-02 03:22:36.836421 mnist_separator-1.0.2/mnist_separator/src/load_samples.py
+-rw-r--r--   0        0        0     1386 2024-05-02 03:22:36.848610 mnist_separator-1.0.2/mnist_separator/src/save_result.py
+-rw-r--r--   0        0        0      825 2024-05-02 03:22:36.833593 mnist_separator-1.0.2/mnist_separator/src/timer.py
+-rw-r--r--   0        0        0     4104 2024-05-02 03:22:36.896651 mnist_separator-1.0.2/mnist_separator/src/to_canonical.py
+-rw-r--r--   0        0        0      663 2024-05-02 14:27:33.572174 mnist_separator-1.0.2/mnist_separator/src/utils_directory.py
+-rw-r--r--   0        0        0      600 2024-05-02 03:22:36.907332 mnist_separator-1.0.2/mnist_separator/src/utils_list.py
+-rw-r--r--   0        0        0      497 2024-05-02 15:08:13.003138 mnist_separator-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mnist_separator-1.0.2/PKG-INFO
```

### Comparing `mnist_separator-1.0.1/mnist_separator/.DS_Store` & `mnist_separator-1.0.2/mnist_separator/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0005 0000 0003  ................
 00000110: 0073 0072 0063 6c67 3153 636f 6d70 0000  .s.r.clg1Scomp..
-00000120: 0000 0000 69a8 0000 0003 0073 0072 0063  ....i......s.r.c
-00000130: 6d6f 4444 626c 6f62 0000 0008 dbc1 3806  moDDblob......8.
-00000140: 27f1 c541 0000 0003 0073 0072 0063 6d6f  '..A.....s.r.cmo
-00000150: 6444 626c 6f62 0000 0008 dbc1 3806 27f1  dDblob......8.'.
+00000120: 0000 0000 69ec 0000 0003 0073 0072 0063  ....i......s.r.c
+00000130: 6d6f 4444 626c 6f62 0000 0008 30eb 0977  moDDblob....0..w
+00000140: eff1 c541 0000 0003 0073 0072 0063 6d6f  ...A.....s.r.cmo
+00000150: 6444 626c 6f62 0000 0008 30eb 0977 eff1  dDblob....0..w..
 00000160: c541 0000 0003 0073 0072 0063 7068 3153  .A.....s.r.cph1S
-00000170: 636f 6d70 0000 0000 0001 1000 0000 0003  comp............
+00000170: 636f 6d70 0000 0000 0001 2000 0000 0003  comp...... .....
 00000180: 0073 0072 0063 7653 726e 6c6f 6e67 0000  .s.r.cvSrnlong..
 00000190: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/.DS_Store` & `mnist_separator-1.0.2/mnist_separator/src/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0000 8949 0000 000b 005f 005f 0070  .....I....._._.p
+00000130: 0000 0000 9e85 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 2005 7295  moDDblob.... .r.
-00000160: 1cf1 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 c2f4 4b4f  moDDblob......KO
+00000160: eef1 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 2005 7295 1cf1  dDblob.... .r...
+00000180: 6444 626c 6f62 0000 0008 c2f4 4b4f eef1  dDblob......KO..
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0001 1000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0001 4000 0000 0000  comp......@.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/clean_all.py` & `mnist_separator-1.0.2/mnist_separator/src/clean_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # clean_all.py
 
 from pathlib import Path
 
 from mnist_separator.src import glbl
 from mnist_separator.src.utils_directory import init_directory
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/convert_data.py` & `mnist_separator-1.0.2/mnist_separator/src/convert_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # convert_data.py
 
 import cv2 as cv
 import os
 from pathlib import Path
 
 from mnist_separator.src import glbl
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/create_dirs.py` & `mnist_separator-1.0.2/mnist_separator/src/create_dirs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # create_dirs.py
 
 from pathlib import Path
 import os
 
 
 def create_dirs():
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/get_similarity.py` & `mnist_separator-1.0.2/mnist_separator/src/get_similarity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# May-01-2024
+# May-02-2024
 # get_similarity.py
 
 import sys
 import cv2 as cv
 
 from mnist_separator.src.to_canonical import to_canonical
-from one_with_another.src.calc_similarity import calc_similarity
+from one_with_another import calc_similarity
 
 
 def get_similarity(path_1: str, path_2: str) -> float:
 
     image1_mnist = cv.imread(path_1, cv.IMREAD_UNCHANGED)
     if image1_mnist is None:
         print(f'\nERROR: Unable to read {path_1}.')
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/get_similarity_group.py` & `mnist_separator-1.0.2/mnist_separator/src/get_similarity_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # get_similarity_group.py
 
 import os
 import cv2 as cv
 import numpy as np
 
 from one_with_another.src.calc_similarity import calc_similarity
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/glbl.py` & `mnist_separator-1.0.2/mnist_separator/src/glbl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # glbl.py
 
 
 result_name: str = '_RESULT_'
 
 path_test_mnist: str = ''
 path_train_0_mnist: str = ''
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/go.py` & `mnist_separator-1.0.2/mnist_separator/src/go.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # go.py
 
 import sys
 import os
 import numpy as np
 import random
 from tqdm import tqdm
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/import_mnist.py` & `mnist_separator-1.0.2/mnist_separator/src/load_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,17 @@
-# May-01-2024
-# import_mnist.py
+# May-02-2024
+# load_data.py
 
 import sys
 import os
 import shutil
 from pathlib import Path
 
 
-def import_train(dir_mnist, digit, num_images):
-
-    if dir_mnist.exists() and dir_mnist.is_dir():
-
-        dir_src = dir_mnist / 'data_train' / str(digit)
-
-        temp = 'train_' + str(digit)
-        dir_dst = Path.cwd() / '$mnist' / temp
-
-        # Get a list of files in the source directory
-        files = os.listdir(dir_src)
-
-        # Sort the files based on their creation time or modification time
-        files.sort(key=lambda x: os.path.getmtime(os.path.join(dir_src, x)))
-
-        # Copy each file from the source directory to the destination directory
-        n = 0
-        for file in files:
-            src_file_path = os.path.join(dir_src, file)
-            dst_file_path = os.path.join(dir_dst, file)
-            shutil.copy(src_file_path, dst_file_path)
-            n += 1
-            if n == num_images:
-                break
-    else:
-        sys.exit(f"\nDirectory {dir_mnist} does not exist.")
-
-
-def import_test(dir_mnist, digit, num_images):
+def load_data(dir_mnist, digit, num_images):
 
     if dir_mnist.exists() and dir_mnist.is_dir():
 
         dir_src = dir_mnist / 'data_test' / str(digit)
 
         dir_dst = Path.cwd() / '$mnist' / 'test'
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/save_result.py` & `mnist_separator-1.0.2/mnist_separator/src/save_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # save_result.py
 
 from mnist_separator.src import glbl
 from mnist_separator.src.utils_list import save_list
 
 
 def save_result(list_result_0, list_result_1,
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/timer.py` & `mnist_separator-1.0.2/mnist_separator/src/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # timer.py
 
 import time
 from pathlib import Path
 from datetime import date, datetime
 
 global timer_start
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/to_canonical.py` & `mnist_separator-1.0.2/mnist_separator/src/to_canonical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # to_canonical.py
 
 import cv2 as cv
 import numpy as np
 
 
 def to_canonical(image_in):
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/utils_directory.py` & `mnist_separator-1.0.2/mnist_separator/src/utils_directory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # utils_directory.py
 
 from pathlib import Path
 
 
 def init_directory(dir_name):
```

### Comparing `mnist_separator-1.0.1/mnist_separator/src/utils_list.py` & `mnist_separator-1.0.2/mnist_separator/src/utils_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-01-2024
+# May-02-2024
 # utils_list.py
 
 import os
 from pathlib import Path
 
 
 def save_list(list_name, dir_name, any_list):
```

### Comparing `mnist_separator-1.0.1/PKG-INFO` & `mnist_separator-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnist-separator
-Version: 1.0.1
+Version: 1.0.2
 Summary: mnist-separator is a new technology for recognizing handwritten numbers from the MNIST dataset
 License: MIT
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

