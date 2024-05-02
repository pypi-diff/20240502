# Comparing `tmp/VisionCraft-0.1.25.tar.gz` & `tmp/VisionCraft-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraft-0.1.25.tar", last modified: Wed May  1 08:52:51 2024, max compression
+gzip compressed data, was "VisionCraft-0.1.26.tar", last modified: Wed May  1 16:05:05 2024, max compression
```

## Comparing `VisionCraft-0.1.25.tar` & `VisionCraft-0.1.26.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.803967 VisionCraft-0.1.25/
--rw-rw-rw-   0        0        0     1090 2024-02-08 13:43:37.000000 VisionCraft-0.1.25/LICENSE
--rw-rw-rw-   0        0        0    17602 2024-05-01 08:52:51.750570 VisionCraft-0.1.25/PKG-INFO
--rw-rw-rw-   0        0        0    16590 2024-04-01 14:42:43.000000 VisionCraft-0.1.25/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.427580 VisionCraft-0.1.25/VisionCraft/
--rw-rw-rw-   0        0        0       25 2024-02-13 16:58:32.000000 VisionCraft-0.1.25/VisionCraft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.454182 VisionCraft-0.1.25/VisionCraft/craft/
--rw-rw-rw-   0        0        0      312 2024-02-13 16:59:09.000000 VisionCraft-0.1.25/VisionCraft/craft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.457991 VisionCraft-0.1.25/VisionCraft/help/
-drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.705453 VisionCraft-0.1.25/VisionCraft/help/Experiment/
--rw-rw-rw-   0        0        0  3004238 2024-04-18 03:58:39.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp1.ipynb
--rw-rw-rw-   0        0        0  2216233 2024-04-18 03:58:46.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp2.ipynb
--rw-rw-rw-   0        0        0  1201342 2024-04-18 04:05:06.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp3.ipynb
--rw-rw-rw-   0        0        0  1262767 2024-04-18 04:05:35.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp4.ipynb
--rw-rw-rw-   0        0        0   332016 2024-04-18 04:05:28.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp5.ipynb
--rw-rw-rw-   0        0        0   379367 2024-04-18 04:05:40.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp6.ipynb
--rw-rw-rw-   0        0        0  1423296 2024-04-18 04:06:03.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp7.ipynb
--rw-rw-rw-   0        0        0   517272 2024-04-18 04:12:36.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp8.ipynb
--rw-rw-rw-   0        0        0   287542 2024-04-18 04:12:40.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp9.ipynb
--rw-rw-rw-   0        0        0       41 2024-04-18 05:38:17.000000 VisionCraft-0.1.25/VisionCraft/help/Experiment/__init__.py
--rw-rw-rw-   0        0        0       30 2024-02-13 16:59:03.000000 VisionCraft-0.1.25/VisionCraft/help/__init__.py
--rw-rw-rw-   0        0        0    25401 2024-05-01 08:27:11.000000 VisionCraft-0.1.25/VisionCraft/help/exp.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.743547 VisionCraft-0.1.25/VisionCraft/vision/
--rw-rw-rw-   0        0        0      777 2024-02-13 16:59:20.000000 VisionCraft-0.1.25/VisionCraft/vision/__init__.py
--rw-rw-rw-   0        0        0     9771 2024-04-09 15:52:59.000000 VisionCraft-0.1.25/VisionCraft/vision/filter.py
--rw-rw-rw-   0        0        0     2117 2024-05-01 08:19:30.000000 VisionCraft-0.1.25/VisionCraft/vision/huffman.py
--rw-rw-rw-   0        0        0     6836 2024-03-13 03:13:00.000000 VisionCraft-0.1.25/VisionCraft/vision/processing.py
--rw-rw-rw-   0        0        0     7996 2024-04-03 08:40:46.000000 VisionCraft-0.1.25/VisionCraft/vision/segmentation.py
--rw-rw-rw-   0        0        0     9901 2024-03-13 03:13:52.000000 VisionCraft-0.1.25/VisionCraft/vision/transform.py
--rw-rw-rw-   0        0        0     9303 2024-03-13 03:14:28.000000 VisionCraft-0.1.25/VisionCraft/vision/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:52:51.446164 VisionCraft-0.1.25/VisionCraft.egg-info/
--rw-rw-rw-   0        0        0    17602 2024-05-01 08:52:49.000000 VisionCraft-0.1.25/VisionCraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      916 2024-05-01 08:52:51.000000 VisionCraft-0.1.25/VisionCraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 08:52:49.000000 VisionCraft-0.1.25/VisionCraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-01 08:52:49.000000 VisionCraft-0.1.25/VisionCraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-01 08:52:49.000000 VisionCraft-0.1.25/VisionCraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 08:52:51.804967 VisionCraft-0.1.25/setup.cfg
--rw-rw-rw-   0        0        0     1280 2024-05-01 08:52:28.000000 VisionCraft-0.1.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:05:05.888041 VisionCraft-0.1.26/
+-rw-rw-rw-   0        0        0     1090 2024-02-08 13:43:37.000000 VisionCraft-0.1.26/LICENSE
+-rw-rw-rw-   0        0        0    17602 2024-05-01 16:05:05.880638 VisionCraft-0.1.26/PKG-INFO
+-rw-rw-rw-   0        0        0    16590 2024-04-01 14:42:43.000000 VisionCraft-0.1.26/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 16:05:05.641317 VisionCraft-0.1.26/VisionCraft/
+-rw-rw-rw-   0        0        0       25 2024-02-13 16:58:32.000000 VisionCraft-0.1.26/VisionCraft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:05:05.698370 VisionCraft-0.1.26/VisionCraft/craft/
+-rw-rw-rw-   0        0        0      312 2024-02-13 16:59:09.000000 VisionCraft-0.1.26/VisionCraft/craft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:05:05.707324 VisionCraft-0.1.26/VisionCraft/help/
+drwxrwxrwx   0        0        0        0 2024-05-01 16:05:05.840544 VisionCraft-0.1.26/VisionCraft/help/Experiment/
+-rw-rw-rw-   0        0        0  3004238 2024-04-18 03:58:39.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp1.ipynb
+-rw-rw-rw-   0        0        0  2216233 2024-04-18 03:58:46.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp2.ipynb
+-rw-rw-rw-   0        0        0  1201342 2024-04-18 04:05:06.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp3.ipynb
+-rw-rw-rw-   0        0        0  1262767 2024-04-18 04:05:35.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp4.ipynb
+-rw-rw-rw-   0        0        0   332016 2024-04-18 04:05:28.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp5.ipynb
+-rw-rw-rw-   0        0        0   379367 2024-04-18 04:05:40.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp6.ipynb
+-rw-rw-rw-   0        0        0  1423296 2024-04-18 04:06:03.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp7.ipynb
+-rw-rw-rw-   0        0        0   517272 2024-04-18 04:12:36.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp8.ipynb
+-rw-rw-rw-   0        0        0   287542 2024-04-18 04:12:40.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp9.ipynb
+-rw-rw-rw-   0        0        0       41 2024-04-18 05:38:17.000000 VisionCraft-0.1.26/VisionCraft/help/Experiment/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-02-13 16:59:03.000000 VisionCraft-0.1.26/VisionCraft/help/__init__.py
+-rw-rw-rw-   0        0        0    27389 2024-05-01 16:04:40.000000 VisionCraft-0.1.26/VisionCraft/help/exp.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:05:05.872607 VisionCraft-0.1.26/VisionCraft/vision/
+-rw-rw-rw-   0        0        0      777 2024-02-13 16:59:20.000000 VisionCraft-0.1.26/VisionCraft/vision/__init__.py
+-rw-rw-rw-   0        0        0     9771 2024-04-09 15:52:59.000000 VisionCraft-0.1.26/VisionCraft/vision/filter.py
+-rw-rw-rw-   0        0        0     2117 2024-05-01 08:19:30.000000 VisionCraft-0.1.26/VisionCraft/vision/huffman.py
+-rw-rw-rw-   0        0        0     6836 2024-03-13 03:13:00.000000 VisionCraft-0.1.26/VisionCraft/vision/processing.py
+-rw-rw-rw-   0        0        0     7996 2024-04-03 08:40:46.000000 VisionCraft-0.1.26/VisionCraft/vision/segmentation.py
+-rw-rw-rw-   0        0        0     9901 2024-03-13 03:13:52.000000 VisionCraft-0.1.26/VisionCraft/vision/transform.py
+-rw-rw-rw-   0        0        0     9303 2024-03-13 03:14:28.000000 VisionCraft-0.1.26/VisionCraft/vision/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:05:05.691347 VisionCraft-0.1.26/VisionCraft.egg-info/
+-rw-rw-rw-   0        0        0    17602 2024-05-01 16:05:03.000000 VisionCraft-0.1.26/VisionCraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      916 2024-05-01 16:05:04.000000 VisionCraft-0.1.26/VisionCraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:05:03.000000 VisionCraft-0.1.26/VisionCraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-01 16:05:03.000000 VisionCraft-0.1.26/VisionCraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 16:05:03.000000 VisionCraft-0.1.26/VisionCraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:05:05.888041 VisionCraft-0.1.26/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2024-05-01 16:04:36.000000 VisionCraft-0.1.26/setup.py
```

### Comparing `VisionCraft-0.1.25/LICENSE` & `VisionCraft-0.1.26/LICENSE`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/PKG-INFO` & `VisionCraft-0.1.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraft
-Version: 0.1.25
+Version: 0.1.26
 Summary: Computer Vision Library to help do CV much faster, Updated Filters
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,CNN,cv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VisionCraft-0.1.25/README.md` & `VisionCraft-0.1.26/README.md`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp1.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp1.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp2.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp2.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp3.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp3.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp4.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp4.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp5.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp5.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp6.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp6.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp7.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp7.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp8.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp8.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/Experiment/Exp9.ipynb` & `VisionCraft-0.1.26/VisionCraft/help/Experiment/Exp9.ipynb`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/help/exp.py` & `VisionCraft-0.1.26/VisionCraft/help/exp.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,16 @@
 img_HLS = cv2.cvtColor(img, cv2.COLOR_BGR2HLS)
 plt.imshow(img_HLS, cmap="gray")
 plt.axis("off")
 plt.show()
 
 """## **Different Thresholding Methods in CV2**"""
 
-_, img_thres = cv2.threshold(img, 150, 255, cv2.THRESH_BINARY)
+img = cv2.imread("/content/drive/MyDrive/dip_Images/Fig0354(a)(einstein_orig).tif")
+_, img_thres = cv2.threshold(img, 127, 255, cv2.THRESH_BINARY)
 plt.imshow(img_thres)
 plt.axis("off")
 plt.show()
 
 _, img_thres = cv2.threshold(img, 150, 255, cv2.THRESH_BINARY_INV)
 plt.imshow(img_thres)
 plt.axis("off")
@@ -288,15 +289,18 @@
 for index in range(len(image_paths)):
     img = cv2.imread(image_paths[index], 1)
     imShow(title=img_type[index], image= img, subplot=True, row=4,col=2,num=2*index+1)
     plt.subplot(4,2,2*index+2)
     plt.hist(img.ravel(),256,[0,256])
 plt.show()
 
-"""## **Histogram Equilization**"""
+"""## **Histogram Equilization**
+
+### **Method I**
+"""
 
 def Histogram_Equilization(path:str):
     plt.figure(figsize=(14,10))
     img = cv2.imread(path,1)
     imShow("Original Image", img, subplot=True, row=2, col=2, num=1)
     plt.subplot(2,2,2)
     plt.hist(img.ravel(),256,[0,256])
@@ -305,14 +309,70 @@
     imShow("Histogram Equilization", img, row=2, col=2, num=3, subplot=True)
     plt.subplot(2,2,4)
     plt.hist(img.ravel(),256,[0,256])
 
 Histogram_Equilization("/content/drive/MyDrive/dip_Images/Fig0316(2)(2nd_from_top).tif")
 plt.show()
 
+"""### **Method II**"""
+
+import pandas as pd
+
+def histogramEquilization(img):
+
+    img1 = np.copy(img)
+    freq = {}
+    for row in range(img.shape[0]):
+        for col in range(img.shape[1]):
+            r = img[row][col]
+            if r in freq:
+                freq[r] += 1
+            else:
+                freq[r] = 1
+
+    for i in range(256):
+        if i not in freq:
+            freq[i] = 0
+    data = {
+        "GrayLevel":list(freq.keys()),
+        "Nk":list(freq.values())
+    }
+
+    df = pd.DataFrame(data)
+    df = df.sort_values(by="GrayLevel")
+    df.reset_index(inplace=True, drop=True)
+    df["PDF"] = df["Nk"]/(img.shape[0]*img.shape[1])
+    df["CDF"] = df["PDF"].cumsum()
+    df["Sk"] = df["CDF"]*255
+    df["New_Histogram"] = df["Sk"].apply(lambda x:round(x))
+    grouped_df = df[['New_Histogram', 'Nk']].groupby('New_Histogram').sum().reset_index()
+    for row in range(img.shape[0]):
+        for col in range(img.shape[1]):
+            r = img[row][col]
+            img1[row][col] = df.loc[r,"New_Histogram"]
+
+    return df, img1, grouped_df
+
+plt.figure(figsize=(14,10))
+img = cv2.imread("/content/drive/MyDrive/dip_Images/Fig0316(2)(2nd_from_top).tif", 1)
+
+imShow("Original Image", img, subplot=True, row=2, col=2, num=1)
+plt.subplot(2,2,2)
+plt.hist(img.ravel(),256,[0,256])
+img = cv2.imread("/content/drive/MyDrive/dip_Images/Fig0316(2)(2nd_from_top).tif", 0)
+df, eq_img, grouped_df = histogramEquilization(img)
+imShow("Histogram Equilization", eq_img, row=2, col=2, num=3, subplot=True)
+plt.subplot(2,2,4)
+plt.hist(eq_img.ravel(),256,[0,256])
+plt.show()
+
+df
+
+grouped_df
+
 """# **Exp 5**
 
 ## **Box Filter**
 """
 
 img = cv2.imread("/content/drive/MyDrive/dip_Images/Fig0333(a)(test_pattern_blurring_orig).tif", 0)
 
@@ -353,48 +413,52 @@
 img = cv2.imread("/content/drive/MyDrive/dip_Images/Fig0333(a)(test_pattern_blurring_orig).tif", 0)
 imShow("Original Image", img, subplot=True, row=1, col=3, num=1)
 imShow("3x3 Image", weighted_filter(3,img), subplot=True, row=1, col=3, num=2)
 imShow("5x5 Image", weighted_filter(5,img), subplot=True, row=1, col=3, num=3)
 
 """## **Median Filter**"""
 
-filter_size = 3
+filter_size = 5
 
 rows, cols = img.shape
-img1 = np.pad(img, pad_width=int(np.floor(filter_size/2)), mode='constant', constant_values=255)
+img1 = np.pad(img, pad_width=filter_size//2, mode='constant', constant_values=255)
 filtered_img = np.zeros_like(img)
 for row in range(rows):
     for col in range(cols):
         replace = np.median(img1[row:row+filter_size, col:col+filter_size])
         filtered_img[row,col]=  replace
 
 plt.figure(figsize=(5, 3))
 imShow("Original Image",img, subplot=True, row=1,col=2, num=1)
 imShow("Median Filter",filtered_img,subplot=True, row=1, col=2, num=2)
 plt.show()
 
 """## **Min Filter**"""
 
+filter_size = 5
+
 rows, cols = img.shape
-img1 = np.pad(img, pad_width=int(np.floor(filter_size/2)), mode='constant', constant_values=255)
+img1 = np.pad(img, pad_width=filter_size//2, mode='constant', constant_values=255)
 filtered_img = np.zeros_like(img)
 for row in range(rows):
     for col in range(cols):
         replace = np.min(img1[row:row+filter_size, col:col+filter_size])
         filtered_img[row,col]=  replace
 
 plt.figure(figsize=(5, 3))
 imShow("Original Image",img, subplot=True, row=1,col=2, num=1)
 imShow("Min Filter",filtered_img,subplot=True, row=1,col=2, num=2)
 plt.show()
 
 """## **Max Filter**"""
 
+filter_size = 5
+
 rows, cols = img.shape
-img1 = np.pad(img, pad_width=int(np.floor(filter_size/2)), mode='constant', constant_values=255)
+img1 = np.pad(img, pad_width=filter_size//2, mode='constant', constant_values=255)
 filtered_img = np.zeros_like(img)
 for row in range(rows):
     for col in range(cols):
         replace = np.max(img1[row:row+filter_size, col:col+filter_size])
         filtered_img[row,col]=  replace
 
 plt.figure(figsize=(5, 3))
@@ -483,15 +547,14 @@
 imShow("Original Image", image=img, subplot=True, row=1, col=2, num=1)
 delta = 3
 Tnew = np.min(img)+1
 while abs(T-Tnew) >= delta:
     T = Tnew
     rows, cols = img.shape
     totalCells = rows*cols
-
     G1 = []
     G2 = []
     for row in range(rows):
         for col in range(cols):
             if img[row][col] > T:
                 G1.append(img[row][col])
             else:
@@ -613,33 +676,39 @@
 imShow(title=f"New Image ({new_height} x {new_width})", image=img, subplot=True, row=1, col=2, num=2)
 
 """## **Method I**
 
 ### **DCT**
 """
 
-N = 8
-def dct2D(block, N = N):
-    DCT_matrix = np.zeros((N, N))
-    for u in range(N):
+import numpy as np
+
+def dct_2D(image):
+    M, N = image.shape
+    dct_image = np.zeros_like(image, dtype=np.float32)
+
+    for u in range(M):
         for v in range(N):
-            au = (1/(N))**0.5 if u == 0 else (2/(N))**0.5
-            av = (1/(N))**0.5 if v == 0 else (2/(N))**0.5
-            dct_sum = 0
-            for x in range(N):
+            cu = np.sqrt(1/N) if u == 0 else np.sqrt(2/N)
+            cv = np.sqrt(1/N) if v == 0 else np.sqrt(2/N)
+
+            sum_dct = 0
+            for x in range(M):
                 for y in range(N):
-                    dct_sum += block[x, y] * np.cos(((2 * x + 1) * u * np.pi) / (2 * N)) * np.cos(((2 * y + 1) * v * np.pi) / (2 * N))
-            DCT_matrix[u, v] = au * av * dct_sum
-    return DCT_matrix
+                    sum_dct += image[x, y] * np.cos(((2*x + 1) * u * np.pi) / (2 * M)) * np.cos(((2*y + 1) * v * np.pi) / (2 * N))
+
+            dct_image[u, v] =  cu * cv * sum_dct
+
+    return dct_image
 
 
 blocks = [img[i:i+N, j:j+N] for i in range(0, new_height, N) for j in range(0, new_width, N)]
 
 
-dct_blocks = [dct2D(block) for block in blocks]
+dct_blocks = [dct_2D(block) for block in blocks]
 
 new_img = np.zeros((new_height, new_width))
 idx = 0
 for i in range(0, new_height, N):
     for j in range(0, new_width, N):
         new_img[i:i+N, j:j+N] = dct_blocks[idx]
         idx += 1
@@ -647,31 +716,40 @@
 
 new_img = np.round(new_img)
 
 imShow(image=new_img)
 
 """### **IDCT**"""
 
-def idct2D(block, N = N):
-    IDCT_matrix = np.zeros((N, N))
-    for u in range(N):
-        for v in range(N):
-            au = (1/(N))**0.5 if u == 0 else (2/(N))**0.5
-            av = (1/(N))**0.5 if v == 0 else (2/(N))**0.5
-            idct_sum = 0
-            for x in range(N):
-                for y in range(N):
-                    idct_sum += block[x, y] * np.cos(((2 * x + 1) * u * np.pi) / (2 * N)) * np.cos(((2 * y + 1) * v * np.pi) / (2 * N))
-            IDCT_matrix[u, v] = au * av * idct_sum
-    return IDCT_matrix
+import numpy as np
+
+def idct_2D(dct_image):
+    M, N = dct_image.shape
+    image = np.zeros_like(dct_image, dtype=np.float32)
+
+    for x in range(M):
+        for y in range(N):
+            sum_idct = 0
+            for u in range(M):
+                for v in range(N):
+                    cu = np.sqrt(1/N) if u == 0 else np.sqrt(2/N)
+                    cv = np.sqrt(1/N) if v == 0 else np.sqrt(2/N)
+                    sum_idct += cu * cv * dct_image[u, v] * np.cos(((2*x + 1) * u * np.pi) / (2 * M)) * np.cos(((2*y + 1) * v * np.pi) / (2 * N))
+
+            image[x, y] = sum_idct
+
+    return image
+
 
 
+N = 8
+
 blocks = [new_img[i:i+N, j:j+N] for i in range(0, new_height, N) for j in range(0, new_width, N)]
 
-idct_blocks = [dct2D(block) for block in blocks]
+idct_blocks = [idct_2D(block) for block in blocks]
 
 og_img = np.zeros((new_height, new_width))
 idx = 0
 for i in range(0, new_height, N):
     for j in range(0, new_width, N):
         og_img[i:i+N, j:j+N] = idct_blocks[idx]
         idx += 1
@@ -693,19 +771,19 @@
 
 """## **Method II**
 
 ### **DCT**
 """
 
 img = cv2.imread("/content/cameraman.png", 0)
-dct_img = cv2.dct(cv2.dct(np.float32(img)))
+dct_img = cv2.dct((np.float32(img)))
 
 """### **IDCT**"""
 
-idct_img = cv2.idct(cv2.idct(np.float32(dct_img)))
+idct_img = cv2.idct(np.float32(dct_img))
 imShow("Original Image", img, subplot=True, row=1, col=3, num=1)
 imShow("DCT Image", dct_img, subplot=True, row=1, col=3, num=2)
 imShow("IDCT Image", idct_img, subplot=True, row=1, col=3, num=3)
 
 """# **Exp 9**
 
 ## **Huffman**
@@ -801,14 +879,19 @@
 
     print("Entropy: ", entropy)
     print("Efficiency: ", entropy*100/Lavg, "%")
     print("Redundancy:", 1-entropy/Lavg)
 
 calculate_metrics(hashmap, huffman_codes)
 
+# Compression = 1/1-R
+# R = Redundancy
+
+print("Compression Ratio = ", 1/(1- 0.0061210402945277576))
+
 """### **Method II**
 
 #### **Note**: I am not sure if this method is allowed or Not if possible get it confirmed from College Faculty
 """
 
 import cv2
 import huffman
@@ -824,16 +907,14 @@
     for col in range(cols):
         pixel = img[row][col]
         if pixel not in hashmap:
             hashmap[pixel] = 1
         else:
             hashmap[pixel] += 1
 
-
-
 symbol_freq_pairs = [(key, value) for key, value in hashmap.items()]
 
 
 codebook = huffman.codebook(symbol_freq_pairs)
 
 
 print("Huffman Codes:")
```

### Comparing `VisionCraft-0.1.25/VisionCraft/vision/__init__.py` & `VisionCraft-0.1.26/VisionCraft/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/vision/filter.py` & `VisionCraft-0.1.26/VisionCraft/vision/filter.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/vision/huffman.py` & `VisionCraft-0.1.26/VisionCraft/vision/huffman.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/vision/processing.py` & `VisionCraft-0.1.26/VisionCraft/vision/processing.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/vision/segmentation.py` & `VisionCraft-0.1.26/VisionCraft/vision/segmentation.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/vision/transform.py` & `VisionCraft-0.1.26/VisionCraft/vision/transform.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft/vision/utils.py` & `VisionCraft-0.1.26/VisionCraft/vision/utils.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/VisionCraft.egg-info/PKG-INFO` & `VisionCraft-0.1.26/VisionCraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraft
-Version: 0.1.25
+Version: 0.1.26
 Summary: Computer Vision Library to help do CV much faster, Updated Filters
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,CNN,cv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VisionCraft-0.1.25/VisionCraft.egg-info/SOURCES.txt` & `VisionCraft-0.1.26/VisionCraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.1.25/setup.py` & `VisionCraft-0.1.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.25'
+VERSION = '0.1.26'
 DESCRIPTION = 'Computer Vision Library to help do CV much faster, Updated Filters'
 LONG_DESCRIPTION = 'Simplifying computer vision tasks with Python. Visualize, transform, and analyze images effortlessly. Ideal for students, researchers, and developers. Enhance your computer vision projects!'
 
 # Setting up    
 setup(
     name="VisionCraft",
     version=VERSION,
```

