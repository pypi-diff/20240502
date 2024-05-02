# Comparing `tmp/clustering_algorithms-0.2.0.tar.gz` & `tmp/clustering_algorithms-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustering_algorithms-0.2.0.tar", last modified: Mon Mar 25 10:49:34 2024, max compression
+gzip compressed data, was "clustering_algorithms-0.3.0.tar", last modified: Thu May  2 10:47:04 2024, max compression
```

## Comparing `clustering_algorithms-0.2.0.tar` & `clustering_algorithms-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-25 10:49:34.199904 clustering_algorithms-0.2.0/
--rw-r--r--   0 user       (502) staff       (20)      595 2024-03-25 10:49:34.199683 clustering_algorithms-0.2.0/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      104 2024-03-23 14:37:19.000000 clustering_algorithms-0.2.0/README.md
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-25 10:49:34.198530 clustering_algorithms-0.2.0/clustering_algorithms/
--rw-r--r--   0 user       (502) staff       (20)        0 2024-03-22 15:22:00.000000 clustering_algorithms-0.2.0/clustering_algorithms/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     2027 2024-03-25 10:44:38.000000 clustering_algorithms-0.2.0/clustering_algorithms/c_means.py
--rw-r--r--   0 user       (502) staff       (20)     2040 2024-03-25 10:44:23.000000 clustering_algorithms-0.2.0/clustering_algorithms/clustering_algorithm.py
--rw-r--r--   0 user       (502) staff       (20)     1504 2024-03-25 10:45:30.000000 clustering_algorithms-0.2.0/clustering_algorithms/k_means.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-25 10:49:34.199468 clustering_algorithms-0.2.0/clustering_algorithms.egg-info/
--rw-r--r--   0 user       (502) staff       (20)      595 2024-03-25 10:49:34.000000 clustering_algorithms-0.2.0/clustering_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      394 2024-03-25 10:49:34.000000 clustering_algorithms-0.2.0/clustering_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2024-03-25 10:49:34.000000 clustering_algorithms-0.2.0/clustering_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)        6 2024-03-25 10:49:34.000000 clustering_algorithms-0.2.0/clustering_algorithms.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       22 2024-03-25 10:49:34.000000 clustering_algorithms-0.2.0/clustering_algorithms.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)      632 2024-03-25 10:49:01.000000 clustering_algorithms-0.2.0/pyproject.toml
--rw-r--r--   0 user       (502) staff       (20)       38 2024-03-25 10:49:34.199965 clustering_algorithms-0.2.0/setup.cfg
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 10:47:04.902191 clustering_algorithms-0.3.0/
+-rw-r--r--   0 user       (502) staff       (20)      595 2024-05-02 10:47:04.902003 clustering_algorithms-0.3.0/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      104 2024-03-23 14:37:19.000000 clustering_algorithms-0.3.0/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 10:47:04.900490 clustering_algorithms-0.3.0/clustering_algorithms/
+-rw-r--r--   0 user       (502) staff       (20)        0 2024-03-22 15:22:00.000000 clustering_algorithms-0.3.0/clustering_algorithms/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     2040 2024-05-02 09:48:24.000000 clustering_algorithms-0.3.0/clustering_algorithms/c_means.py
+-rw-r--r--   0 user       (502) staff       (20)     2149 2024-05-02 09:07:19.000000 clustering_algorithms-0.3.0/clustering_algorithms/clustering_algorithm.py
+-rw-r--r--   0 user       (502) staff       (20)     2264 2024-05-02 10:44:28.000000 clustering_algorithms-0.3.0/clustering_algorithms/k_means.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 10:47:04.901784 clustering_algorithms-0.3.0/clustering_algorithms.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)      595 2024-05-02 10:47:04.000000 clustering_algorithms-0.3.0/clustering_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      451 2024-05-02 10:47:04.000000 clustering_algorithms-0.3.0/clustering_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2024-05-02 10:47:04.000000 clustering_algorithms-0.3.0/clustering_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)        6 2024-05-02 10:47:04.000000 clustering_algorithms-0.3.0/clustering_algorithms.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       22 2024-05-02 10:47:04.000000 clustering_algorithms-0.3.0/clustering_algorithms.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)      632 2024-05-02 10:45:38.000000 clustering_algorithms-0.3.0/pyproject.toml
+-rw-r--r--   0 user       (502) staff       (20)       38 2024-05-02 10:47:04.902244 clustering_algorithms-0.3.0/setup.cfg
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 10:47:04.901585 clustering_algorithms-0.3.0/tests/
+-rw-r--r--   0 user       (502) staff       (20)      338 2024-05-02 08:21:08.000000 clustering_algorithms-0.3.0/tests/test_clustering_algorithm.py
+-rw-r--r--   0 user       (502) staff       (20)     1335 2024-05-02 10:20:00.000000 clustering_algorithms-0.3.0/tests/test_k_means.py
```

### Comparing `clustering_algorithms-0.2.0/PKG-INFO` & `clustering_algorithms-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustering_algorithms
-Version: 0.2.0
+Version: 0.3.0
 Summary: Clustering algorithms powered by Numpy
 Author-email: Yan Georget <yan.georget@gmail.com>
 Project-URL: Homepage, https://github.com/yangeorget/clustering-algorithms
 Project-URL: Issues, https://github.com/yangeorget/clustering-algorithms
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `clustering_algorithms-0.2.0/clustering_algorithms/c_means.py` & `clustering_algorithms-0.3.0/clustering_algorithms/c_means.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from numpy.typing import NDArray
 
 from clustering_algorithms.clustering_algorithm import ClusteringAlgorithm
 
 
 class CMeans(ClusteringAlgorithm):
     """
-    A Numpy implementation of the C-Means clustering_algorithms algorithm.
+    A Numpy implementation of the C-Means clustering algorithm.
     """
 
     def __init__(self, k: int, iterations: int, m: int = 2):
         """
         :param k: the number of clusters
         :param iterations: the number of iterations
         :param m: the fuzzifier factor (should be > 1, defaults to 2)
@@ -26,15 +26,15 @@
         :param points: a nxd matrix
         :param weights: a nxk matrix
         :return: a kxd matrix where k is the number of clusters and d the number of dimensions
         """
         wm = weights**self.m
         return (points.T @ wm / np.sum(wm, axis=0)).T
 
-    def init(self, points: NDArray) -> Sequence[NDArray]:
+    def init(self, points: NDArray, method: str = "random") -> Sequence[NDArray]:
         n = points.shape[0]
         weights = np.array(np.random.dirichlet(np.ones(self.k), n))
         centroids = self.compute_centroids(points, weights)
         return centroids, weights
 
     def fit(self, points: NDArray) -> Sequence[NDArray]:
         centroids, weights = self.init(points)
```

### Comparing `clustering_algorithms-0.2.0/clustering_algorithms/clustering_algorithm.py` & `clustering_algorithms-0.3.0/clustering_algorithms/clustering_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,44 +7,45 @@
 # mypy: disable-error-code=empty-body
 class ClusteringAlgorithm:
     """
     An abstract clustering algorithm.
     Clustering algorithms produce models that are set of centroids.
     """
 
-    def __init__(self, k: int, iterations: int):
+    def __init__(self, k: int, iterations: int = 1):
         """
         :param k: the number of clusters
         :param iterations: the number of iterations
         """
         self.iterations = iterations
         self.k = k
 
-    def init(self, points: NDArray) -> Union[NDArray, Sequence[NDArray]]:
+    def init(self, points: NDArray, method: str = "random") -> Union[NDArray, Sequence[NDArray]]:
         """
         Inits the model.
         :param points: the training set
-        :return: a sequence of arrays including a set of centroids
+        :param method: the init method, defaults to "random"
+        :return: a sequence of arrays starting with, at least: a set of centroids
         """
         pass
 
     def fit(self, points: NDArray) -> Sequence[NDArray]:
         """
         Fits a model to the training set (the points).
         :param points: the training set
-        :return: a sequence of arrays including a set of centroids, the corresponding clusters
+        :return: a sequence of arrays starting with, at least : a set of centroids, the corresponding clusters
         """
         pass
 
     def predict(self, points: NDArray, centroids: NDArray) -> NDArray:
         """
         Applies the model to a set of points.
         :param points: a new set of points
         :param centroids: the centroids
-        :return: for each point, the clustering_algorithms output
+        :return: for each point, the clustering output
         """
         pass
 
     def distances(self, points: NDArray, centroids: NDArray) -> NDArray:
         """
         Computes the distances between points and centroids.
         :param points: a nxd matrix
```

### Comparing `clustering_algorithms-0.2.0/clustering_algorithms/k_means.py` & `clustering_algorithms-0.3.0/clustering_algorithms/k_means.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,18 +16,31 @@
         Computes the centroid given the clusters.
         :param points: a nxd matrix
         :param clusters: a nx1 matrix
         :return: a kxd matrix where k is the number of clusters and d the number of dimensions
         """
         return np.array([np.mean(points[clusters == j], axis=0) for j in range(self.k)])
 
-    def init(self, points: NDArray) -> NDArray:
-        # TODO : kmeans++
+    def init(self, points: NDArray, method: str = "kmeans++") -> NDArray:
         n = points.shape[0]
-        return points[np.random.choice(n, self.k, replace=False), :]
+        if method == "random":
+            return points[np.random.choice(n, self.k, replace=False), :]
+        else:  # kmeans++
+            centroids = np.zeros((self.k, points.shape[1]))
+            centroids[0] = points[np.random.choice(n)]
+            min_distances = None
+            for i in range(1, self.k):
+                centroid_distances = self.distances(points, centroids[i - 1]).flatten()
+                if min_distances is not None:
+                    min_distances = np.min(np.vstack((min_distances, centroid_distances)), axis=0)
+                else:
+                    min_distances = centroid_distances
+                squared_min_distances = min_distances**2
+                centroids[i] = points[np.random.choice(n, p=squared_min_distances / np.sum(squared_min_distances))]
+            return centroids
 
     def fit(self, points: NDArray) -> Sequence[NDArray]:
         centroids = self.init(points)
         for iteration in range(self.iterations):
             clusters = self.predict(points, centroids)
             self.log_iteration(iteration, centroids, clusters)
             new_centroids = self.compute_centroids(points, clusters)
```

### Comparing `clustering_algorithms-0.2.0/clustering_algorithms.egg-info/PKG-INFO` & `clustering_algorithms-0.3.0/clustering_algorithms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustering_algorithms
-Version: 0.2.0
+Version: 0.3.0
 Summary: Clustering algorithms powered by Numpy
 Author-email: Yan Georget <yan.georget@gmail.com>
 Project-URL: Homepage, https://github.com/yangeorget/clustering-algorithms
 Project-URL: Issues, https://github.com/yangeorget/clustering-algorithms
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `clustering_algorithms-0.2.0/pyproject.toml` & `clustering_algorithms-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clustering_algorithms"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Yan Georget", email="yan.georget@gmail.com" },
 ]
 description = "Clustering algorithms powered by Numpy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

