# Comparing `tmp/TH_camera_calibration-0.4.5.tar.gz` & `tmp/TH_camera_calibration-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TH_camera_calibration-0.4.5.tar", last modified: Sun Apr 21 07:13:19 2024, max compression
+gzip compressed data, was "TH_camera_calibration-0.4.6.tar", last modified: Thu May  2 17:14:57 2024, max compression
```

## Comparing `TH_camera_calibration-0.4.5.tar` & `TH_camera_calibration-0.4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 07:13:19.447379 TH_camera_calibration-0.4.5/
--rw-rw-rw-   0        0        0     2729 2024-04-21 07:13:19.444398 TH_camera_calibration-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     5238 2024-04-21 07:06:15.000000 TH_camera_calibration-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 07:13:19.427929 TH_camera_calibration-0.4.5/TH_camera_calibration.egg-info/
--rw-rw-rw-   0        0        0     2729 2024-04-21 07:13:19.000000 TH_camera_calibration-0.4.5/TH_camera_calibration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-21 07:13:19.000000 TH_camera_calibration-0.4.5/TH_camera_calibration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 07:13:19.000000 TH_camera_calibration-0.4.5/TH_camera_calibration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-04-21 07:13:19.000000 TH_camera_calibration-0.4.5/TH_camera_calibration.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-21 07:13:19.000000 TH_camera_calibration-0.4.5/TH_camera_calibration.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-21 07:13:19.436622 TH_camera_calibration-0.4.5/camera_calibration/
--rw-rw-rw-   0        0        0       51 2024-04-21 06:12:27.000000 TH_camera_calibration-0.4.5/camera_calibration/__init__.py
--rw-rw-rw-   0        0        0    13214 2024-04-21 05:58:38.000000 TH_camera_calibration-0.4.5/camera_calibration/camera_calibration.py
--rw-rw-rw-   0        0        0       42 2024-04-21 07:13:19.447379 TH_camera_calibration-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      481 2024-04-21 07:11:53.000000 TH_camera_calibration-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:14:57.313776 TH_camera_calibration-0.4.6/
+-rw-rw-rw-   0        0        0     2729 2024-05-02 17:14:57.312778 TH_camera_calibration-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5238 2024-04-21 07:06:15.000000 TH_camera_calibration-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 17:14:57.300783 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/
+-rw-rw-rw-   0        0        0     2729 2024-05-02 17:14:56.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-02 17:14:57.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 17:14:56.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-02 17:14:56.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-02 17:14:56.000000 TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 17:14:57.307779 TH_camera_calibration-0.4.6/camera_calibration/
+-rw-rw-rw-   0        0        0       51 2024-04-21 06:12:27.000000 TH_camera_calibration-0.4.6/camera_calibration/__init__.py
+-rw-rw-rw-   0        0        0    14163 2024-05-02 16:25:32.000000 TH_camera_calibration-0.4.6/camera_calibration/camera_calibration.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 17:14:57.314776 TH_camera_calibration-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      481 2024-05-02 16:28:44.000000 TH_camera_calibration-0.4.6/setup.py
```

### Comparing `TH_camera_calibration-0.4.5/PKG-INFO` & `TH_camera_calibration-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TH_camera_calibration
-Version: 0.4.5
+Version: 0.4.6
 Description-Content-Type: text/markdown
 
 # Calibration_camera
 
 Created on Sunday, April 21, 2024  
 Author: Tung Nguyen - Handsome  
 Reference: Camera Calibration by OpenCV ([OpenCV Tutorial](https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html))
```

### Comparing `TH_camera_calibration-0.4.5/README.md` & `TH_camera_calibration-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `TH_camera_calibration-0.4.5/TH_camera_calibration.egg-info/PKG-INFO` & `TH_camera_calibration-0.4.6/TH_camera_calibration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TH-camera-calibration
-Version: 0.4.5
+Version: 0.4.6
 Description-Content-Type: text/markdown
 
 # Calibration_camera
 
 Created on Sunday, April 21, 2024  
 Author: Tung Nguyen - Handsome  
 Reference: Camera Calibration by OpenCV ([OpenCV Tutorial](https://docs.opencv.org/4.x/dc/dbb/tutorial_py_calibration.html))
```

### Comparing `TH_camera_calibration-0.4.5/camera_calibration/camera_calibration.py` & `TH_camera_calibration-0.4.6/camera_calibration/camera_calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             calibrationDir (str, optional): The directory path where calibration images are stored. Defaults to None.
             savepath (str, optional): The directory path where the calibration data will be saved. Defaults to None.
             saveformat (str, optional): The format to save the calibration data. Options: "pkl", "yaml", or "npz". Defaults to "pkl".
             show_process_img (bool, optional): Flag to indicate whether to show the process images during calibration. Defaults to True.
             show_calibration_data (bool, optional): Flag to indicate whether to show the calibration data. Defaults to True.
         """
         if run:
+            valid_data_flag = False
             # FIND CHESSBOARD CORNERS - OBJECT POINTS AND IMAGE POINTS
             # termination criteria
             criteria = (cv.TERM_CRITERIA_EPS + cv.TERM_CRITERIA_MAX_ITER, 30, 0.001)
 
             # prepare object points, like (0,0,0), (1,0,0), (2,0,0) ....,(6,5,0)
             objp = np.zeros((chessboardSize[0] * chessboardSize[1], 3), np.float32)
             objp[:, :2] = np.mgrid[
@@ -67,14 +68,16 @@
             objp = objp * size_of_chessboard_squares_mm
 
             # Arrays to store object points and image points from all the images.
             objpoints = []  # 3d point in real world space
             imgpoints = []  # 2d points in image plane.
             all_images = []
             image_formats = ["*.jpg", "*.png"]
+            if not os.path.exists(calibrationDir):
+                raise FileNotFoundError("CalibrationDir path does not exit!")
             for image_format in image_formats:
                 images = glob.glob(os.path.join(calibrationDir, image_format))
                 all_images.extend(images)
             for image in all_images:
 
                 img = cv.imread(image)
                 gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
@@ -82,29 +85,33 @@
                 # Find the chess board corners
                 cornersFound, cornersOrg = cv.findChessboardCorners(
                     gray, chessboardSize, None
                 )
 
                 # If found, add object points, image points (after refining them)
                 if cornersFound == True:
-
+                    valid_data_flag = True
                     objpoints.append(objp)
                     cornersRefined = cv.cornerSubPix(
                         gray, cornersOrg, (11, 11), (-1, -1), criteria
                     )
                     imgpoints.append(cornersRefined)
 
                     if show_process_img:
                         # Draw and display the corners
                         cv.drawChessboardCorners(
                             img, chessboardSize, cornersRefined, cornersFound
                         )
                         cv.imshow("img", img)
                         cv.waitKey(1000)
             cv.destroyAllWindows()
+            if not valid_data_flag:
+                raise Exception(
+                    "All data is not valid, needs to be clearer to be able to identify the chessboard corners!"
+                )
             # CALIBRATION
             repError, cameraMatrix, distCoeff, rvecs, tvecs = cv.calibrateCamera(
                 objpoints, imgpoints, framesize, None, None
             )
             if show_calibration_data:
                 print("Camera Matrix: ", cameraMatrix)
                 print("\nDistortion Coefficent: ", distCoeff)
@@ -200,17 +207,15 @@
                 "Invalid format. Supported formats are: 'pkl', 'yaml', 'npz'"
             )
         if show_data:
             print(_cameraMatrix, _distCoeff)
         self.cameraMatrix = _cameraMatrix
         self.distCoeff = _distCoeff
 
-    def undistortion_img(
-        self, img, method="default", img_size=(1280, 720), verbose=False
-    ):
+    def undistort_img(self, img, method="default", img_size=(1280, 720), verbose=False):
         """
         Undistort an image.
 
         Args:
             img (numpy.ndarray): The image to undistort.
             method (str, optional): The method used for distortion removal. Options: "default" or "Remapping". Defaults to "default".
             img_size (tuple, optional): The size of the image (width, height). Defaults to (1280, 720).
@@ -255,40 +260,51 @@
             )
             dst = cv.remap(img, mapx, mapy, cv.INTER_LINEAR)
             # crop the image
             dst = dst[y : y + h, x : x + w]
         resize_img = cv.resize(dst, img_size)
         if verbose:
             print("\nRemove distortion succesfully!")
+            cv.imshow("Undistortion Image", resize_img)
         return resize_img
 
-    def undistortion_points(self, points, verbose=False):
-        """
-        Undistort a set of image points.
-
-        Args:
-            points (numpy.ndarray): The image points to undistort.
-            verbose (bool, optional): Flag to indicate whether to show the process images. Defaults to False.
-
-        Returns:
-            numpy.ndarray: The undistorted points.
-        """
-        if self.cameraMatrix is None or self.distCoeff is None:
-            raise ValueError(
-                "Need to read calibration data by using read_calibration_data function before removing distortion!"
-            )
-        points = np.array([points], dtype="float32")
-        # Undistort
-        undistorted_points = cv.undistortPoints(
-            points, self.cameraMatrix, self.distCoeff
-        )
-        undistorted_points_list = undistorted_points.squeeze().tolist()
-        if verbose:
-            print("\nRemove distortion succesfully!")
-        return undistorted_points_list
+    # def distortion_points(self, points, img, verbose=False):
+    #     """
+    #     Undistort a set of image points.
+
+    #     Args:
+    #         points (numpy.ndarray): The image points to undistort.
+    #         verbose (bool, optional): Flag to indicate whether to show the process images. Defaults to False.
+
+    #     Returns:
+    #         numpy.ndarray: The undistorted points.
+    #     """
+    #     if self.cameraMatrix is None or self.distCoeff is None:
+    #         raise ValueError(
+    #             "Need to read calibration data by using read_calibration_data function before removing distortion!"
+    #         )
+    #     points = np.array([points], dtype="float32")
+    #     # Undistort
+    #     h, w = img.shape[:2]
+
+    #     self.new_cameraMatrix, roi = cv.getOptimalNewCameraMatrix(
+    #         self.cameraMatrix, self.distCoeff, (w, h), 0, (w, h)
+    #     )
+    #     ptsTemp = np.array([], dtype="float32")
+    #     rtemp = ttemp = np.array([0, 0, 0], dtype="float32")
+    #     # ptsOut = cv.undistortPoints(points, self.new_cameraMatrix, None)
+    #     ptsTemp = cv.convertPointsToHomogeneous(points)
+    #     output = cv.projectPoints(
+    #         ptsTemp, rtemp, ttemp, self.cameraMatrix, self.distCoeff
+    #     )
+    #     if verbose:
+    #         print("\nRemove distortion succesfully!")
+    #         print("\nOriginal points:", points)
+    #         print("\nUndistorted points:", output)
+    #     return output
 
 
 if __name__ == "__main__":
 
     calibrator = CameraCalibration()
     calibrator.calculate_calibration_data(
         run=True,
```

