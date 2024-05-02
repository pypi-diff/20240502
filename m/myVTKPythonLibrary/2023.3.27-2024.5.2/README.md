# Comparing `tmp/myVTKPythonLibrary-2023.3.27.tar.gz` & `tmp/myvtkpythonlibrary-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myVTKPythonLibrary-2023.3.27.tar", last modified: Mon Mar 27 12:22:51 2023, max compression
+gzip compressed data, was "myvtkpythonlibrary-2024.5.2.tar", last modified: Thu May  2 19:38:02 2024, max compression
```

## Comparing `myVTKPythonLibrary-2023.3.27.tar` & `myvtkpythonlibrary-2024.5.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:22:51.376275 myVTKPythonLibrary-2023.3.27/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/LICENSE
--rw-r--r--   0 root         (0) root         (0)      670 2023-03-27 12:22:51.376275 myVTKPythonLibrary-2023.3.27/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:22:51.374275 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/
--rw-rw-rw-   0 root         (0) root         (0)     2722 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2506 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addDeformationGradients.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addEquivDeviatoricStrainsFromDeformationGradients.py
--rwxrwxrwx   0 root         (0) root         (0)     2302 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addImageGradient.py
--rwxrwxrwx   0 root         (0) root         (0)     3705 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addImageHessian.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addJacobiansFromDeformationGradients.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addMappingFromPointsToCells.py
--rw-rw-rw-   0 root         (0) root         (0)     4956 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addMappingToCellData.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addMappingToPointData.py
--rw-rw-rw-   0 root         (0) root         (0)     2367 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addPDataNormals.py
--rwxrwxrwx   0 root         (0) root         (0)     2506 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addPhysicalGroupToMesh.py
--rw-rw-rw-   0 root         (0) root         (0)     5746 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addPrincipalDirections.py
--rw-rw-rw-   0 root         (0) root         (0)     4415 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addStrainsFromDeformationGradients.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addStrainsFromDisplacements.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addVertices.py
--rw-rw-rw-   0 root         (0) root         (0)     4370 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/array_algebra.py
--rw-rw-rw-   0 root         (0) root         (0)     5184 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1258 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createCharArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createDoubleArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1261 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createFloatArray.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createImage.py
--rw-rw-rw-   0 root         (0) root         (0)     1257 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createIntArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1258 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createLongArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1260 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createShortArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createUnsignedCharArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createUnsignedIntArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createUnsignedLongArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1276 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createUnsignedShortArray.py
--rw-rw-rw-   0 root         (0) root         (0)     6367 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/fast_array_algebra.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getCellCenters.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getCellLocator.py
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getClippedPDataUsingField.py
--rw-rw-rw-   0 root         (0) root         (0)     2509 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getClippedPDataUsingPlane.py
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getImageDimensionality.py
--rw-rw-rw-   0 root         (0) root         (0)     1451 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getImageDimensions.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getImageInterpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     3655 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getMaskFromMesh.py
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getMaskedImageUsingMesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getMassProperties.py
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getMeshVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     3435 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getOverlapCardinalities.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getPDataSurfaceArea.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getPointLocator.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getPointsInCell.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getThresholdedPData.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getThresholdedUGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getVoxels.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getWarpedMesh.py
--rwxrwxrwx   0 root         (0) root         (0)     1242 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/inp2vtk.py
--rwxrwxrwx   0 root         (0) root         (0)     3026 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/moveMeshBetweenImageSpaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/moveMeshWithWorldMatrix.py
--rwxrwxrwx   0 root         (0) root         (0)     1726 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/pdata2ugrid.py
--rwxrwxrwx   0 root         (0) root         (0)     1216 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/png2vti.py
--rwxrwxrwx   0 root         (0) root         (0)     1805 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/pnm2vti.py
--rw-rw-rw-   0 root         (0) root         (0)     2211 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readAbaqusDeformationGradientsFromDAT.py
--rw-rw-rw-   0 root         (0) root         (0)     3639 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readAbaqusMeshFromINP.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readAbaqusStressesFromDAT.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readDataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readDynaDeformationGradients.py
--rw-rw-rw-   0 root         (0) root         (0)     2976 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readDynaMesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1476 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readImage.py
--rw-rw-rw-   0 root         (0) root         (0)     3338 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readMatLabImage.py
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readPData.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readPNG.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readPNMImage.py
--rw-rw-rw-   0 root         (0) root         (0)     1563 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readSGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readSPoints.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readSTL.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readUGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     3965 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/rotateMatrixArray.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/rotatePointsWithCenterAndRotationMatrix.py
--rw-rw-rw-   0 root         (0) root         (0)     2384 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/rotateVectorArray.py
--rwxrwxrwx   0 root         (0) root         (0)     2082 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/ugrid2pdata.py
--rwxrwxrwx   0 root         (0) root         (0)     1182 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/vtk2stl.py
--rwxrwxrwx   0 root         (0) root         (0)     1208 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/vtk2vtu.py
--rwxrwxrwx   0 root         (0) root         (0)     1208 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/vtu2vtk.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeDataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1501 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeImage.py
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writePData.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeSGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     1214 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeSTL.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeUGrid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:22:51.376275 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary.egg-info/
--rw-r--r--   0 root         (0) root         (0)      670 2023-03-27 12:22:51.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3511 2023-03-27 12:22:51.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 12:22:51.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-27 12:22:51.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-27 12:22:51.000000 myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 12:22:51.376275 myVTKPythonLibrary-2023.3.27/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1186 2023-03-27 12:22:39.000000 myVTKPythonLibrary-2023.3.27/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:38:02.453144 myvtkpythonlibrary-2024.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-02 19:38:02.451144 myvtkpythonlibrary-2024.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:38:02.448144 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/
+-rw-rw-rw-   0 root         (0) root         (0)     2722 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addDeformationGradients.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addEquivDeviatoricStrainsFromDeformationGradients.py
+-rwxrwxrwx   0 root         (0) root         (0)     2302 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addImageGradient.py
+-rwxrwxrwx   0 root         (0) root         (0)     3705 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addImageHessian.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addJacobiansFromDeformationGradients.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addMappingFromPointsToCells.py
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addMappingToCellData.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addMappingToPointData.py
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addPDataNormals.py
+-rwxrwxrwx   0 root         (0) root         (0)     2506 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addPhysicalGroupToMesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addPrincipalDirections.py
+-rw-rw-rw-   0 root         (0) root         (0)     4415 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addStrainsFromDeformationGradients.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addStrainsFromDisplacements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addVertices.py
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/array_algebra.py
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createCharArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createDoubleArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createFloatArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createImage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createIntArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createLongArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createShortArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createUnsignedCharArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createUnsignedIntArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createUnsignedLongArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1276 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createUnsignedShortArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     6367 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/fast_array_algebra.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getCellCenters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getCellLocator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getClippedPDataUsingField.py
+-rw-rw-rw-   0 root         (0) root         (0)     2509 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getClippedPDataUsingPlane.py
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getImageDimensionality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getImageDimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getImageInterpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getMaskFromMesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getMaskedImageUsingMesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getMassProperties.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getMeshVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getOverlapCardinalities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getPDataSurfaceArea.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getPointLocator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getPointsInCell.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getThresholdedPData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getThresholdedUGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getVoxels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getWarpedMesh.py
+-rwxrwxrwx   0 root         (0) root         (0)     1242 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/inp2vtk.py
+-rwxrwxrwx   0 root         (0) root         (0)     3026 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/moveMeshBetweenImageSpaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/moveMeshWithWorldMatrix.py
+-rwxrwxrwx   0 root         (0) root         (0)     1726 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/pdata2ugrid.py
+-rwxrwxrwx   0 root         (0) root         (0)     1216 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/png2vti.py
+-rwxrwxrwx   0 root         (0) root         (0)     1805 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/pnm2vti.py
+-rw-rw-rw-   0 root         (0) root         (0)     2211 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readAbaqusDeformationGradientsFromDAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     3639 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readAbaqusMeshFromINP.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readAbaqusStressesFromDAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readDataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readDynaDeformationGradients.py
+-rw-rw-rw-   0 root         (0) root         (0)     2976 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readDynaMesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readImage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readMatLabImage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readPData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readPNG.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readPNMImage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readSGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readSPoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readSTL.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readUGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3965 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/rotateMatrixArray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/rotatePointsWithCenterAndRotationMatrix.py
+-rw-rw-rw-   0 root         (0) root         (0)     2384 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/rotateVectorArray.py
+-rwxrwxrwx   0 root         (0) root         (0)     2082 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/ugrid2pdata.py
+-rwxrwxrwx   0 root         (0) root         (0)     1182 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/vtk2stl.py
+-rwxrwxrwx   0 root         (0) root         (0)     1208 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/vtk2vtu.py
+-rwxrwxrwx   0 root         (0) root         (0)     1208 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/vtu2vtk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeDataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeImage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writePData.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeSGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeSTL.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeUGrid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:38:02.451144 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-02 19:38:02.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3511 2024-05-02 19:38:02.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 19:38:02.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-02 19:38:02.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-02 19:38:02.000000 myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 19:38:02.453144 myvtkpythonlibrary-2024.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-02 19:37:45.000000 myvtkpythonlibrary-2024.5.2/setup.py
```

### Comparing `myVTKPythonLibrary-2023.3.27/LICENSE` & `myvtkpythonlibrary-2024.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/__init__.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addDeformationGradients.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addDeformationGradients.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addEquivDeviatoricStrainsFromDeformationGradients.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addEquivDeviatoricStrainsFromDeformationGradients.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addImageGradient.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addImageGradient.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addImageHessian.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addImageHessian.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addJacobiansFromDeformationGradients.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addJacobiansFromDeformationGradients.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addMappingFromPointsToCells.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addMappingFromPointsToCells.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addMappingToCellData.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addMappingToCellData.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addMappingToPointData.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addMappingToPointData.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addPDataNormals.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addPDataNormals.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addPhysicalGroupToMesh.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addPhysicalGroupToMesh.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addPrincipalDirections.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addPrincipalDirections.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addStrainsFromDeformationGradients.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addStrainsFromDeformationGradients.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addStrainsFromDisplacements.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addStrainsFromDisplacements.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/addVertices.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/addVertices.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/array_algebra.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/array_algebra.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createCharArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createCharArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createDoubleArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createDoubleArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createFloatArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createFloatArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createImage.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createImage.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createIntArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createIntArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createLongArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createLongArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createShortArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createShortArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createUnsignedCharArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createUnsignedCharArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createUnsignedIntArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createUnsignedIntArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createUnsignedLongArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createUnsignedLongArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/createUnsignedShortArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/createUnsignedShortArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/fast_array_algebra.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/fast_array_algebra.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getCellCenters.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getCellCenters.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getCellLocator.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getCellLocator.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getClippedPDataUsingField.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getClippedPDataUsingField.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getClippedPDataUsingPlane.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getClippedPDataUsingPlane.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getImageDimensionality.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getImageDimensionality.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getImageDimensions.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getImageDimensions.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getImageInterpolator.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getImageInterpolator.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getMaskFromMesh.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getMaskFromMesh.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getMaskedImageUsingMesh.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getMaskedImageUsingMesh.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getMassProperties.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getMassProperties.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getMeshVolume.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getMeshVolume.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getOverlapCardinalities.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getOverlapCardinalities.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getPDataSurfaceArea.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getPDataSurfaceArea.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getPointLocator.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getPointLocator.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getPointsInCell.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getPointsInCell.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getThresholdedPData.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getThresholdedPData.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getThresholdedUGrid.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getThresholdedUGrid.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getVoxels.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getVoxels.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/getWarpedMesh.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/getWarpedMesh.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/inp2vtk.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/inp2vtk.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/moveMeshBetweenImageSpaces.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/moveMeshBetweenImageSpaces.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/moveMeshWithWorldMatrix.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/moveMeshWithWorldMatrix.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/pdata2ugrid.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/pdata2ugrid.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/png2vti.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/png2vti.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/pnm2vti.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/pnm2vti.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readAbaqusDeformationGradientsFromDAT.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readAbaqusDeformationGradientsFromDAT.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readAbaqusMeshFromINP.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readAbaqusMeshFromINP.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readAbaqusStressesFromDAT.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readAbaqusStressesFromDAT.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readDataSet.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readDataSet.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readDynaDeformationGradients.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readDynaDeformationGradients.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readDynaMesh.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readDynaMesh.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readImage.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readImage.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readMatLabImage.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readMatLabImage.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readPData.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readPData.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readPNG.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readPNG.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readPNMImage.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readPNMImage.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readSGrid.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readSGrid.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readSPoints.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readSPoints.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readSTL.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readSTL.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/readUGrid.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/readUGrid.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/rotateMatrixArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/rotateMatrixArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/rotatePointsWithCenterAndRotationMatrix.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/rotatePointsWithCenterAndRotationMatrix.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/rotateVectorArray.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/rotateVectorArray.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/ugrid2pdata.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/ugrid2pdata.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/vtk2stl.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/vtk2stl.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/vtk2vtu.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/vtk2vtu.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/vtu2vtk.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/vtu2vtk.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeDataSet.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeDataSet.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeImage.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeImage.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writePData.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writePData.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeSGrid.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeSGrid.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeSTL.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeSTL.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary/writeUGrid.py` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary/writeUGrid.py`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/myVTKPythonLibrary.egg-info/SOURCES.txt` & `myvtkpythonlibrary-2024.5.2/myVTKPythonLibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myVTKPythonLibrary-2023.3.27/setup.py` & `myvtkpythonlibrary-2024.5.2/setup.py`

 * *Files identical despite different names*

