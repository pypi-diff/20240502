# Comparing `tmp/mimllearning-0.2.7.tar.gz` & `tmp/mimllearning-0.2.8.tar.gz`

## Comparing `mimllearning-0.2.7.tar` & `mimllearning-0.2.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.7/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.7/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/data/bag.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/data/instance.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/tutorial/classifiers_tutorial.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/tutorial/datasets_tutorial.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/tutorial/demo_MIML.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/tutorial/tests.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.7/src/miml/tutorial/transformation_tutorial.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.7/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.7/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.8/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.8/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/instance.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/classifiers_tutorial.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/datasets_tutorial.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/demo_MIML.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/tests.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/transformation_tutorial.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.8/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.8/PKG-INFO
```

### Comparing `mimllearning-0.2.7/readme.md` & `mimllearning-0.2.8/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.2.8/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/classifier/miml_classifier.py` & `mimllearning-0.2.8/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.2.8/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/classifier/mi/iterated_discrim_apr_classifier.py` & `mimllearning-0.2.8/src/miml/classifier/mi/iterated_discrim_apr_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,28 +44,14 @@
 
         """
         if np.all(bag >= self.apr[0]):
             if np.all(bag <= self.apr[1]):
                 return 1
         return 0
 
-    def evaluate(self, x_test, y_test):
-        """
-
-        Parameters
-        ----------
-        x_test
-        y_test
-        """
-        results = np.zeros(y_test.shape)
-        for i, bag in enumerate(x_test):
-            result = self.predict_bag(bag)
-            results[i] = result
-        return results
-
     def generate_apr(self):
 
         self.positive_bag_indices = np.where(self.y_train == 1)[0]
 
         initial_bag_index = np.random.choice(self.positive_bag_indices)
         initial_index_instance = np.random.choice(self.x_train[initial_bag_index].shape[0])
         apr_min = apr_max = self.x_train[initial_bag_index][initial_index_instance]
@@ -96,15 +82,14 @@
             for bag_index in not_positives_bag_in_apr:
                 for instance in self.x_train[bag_index]:
                     apr_min = np.minimum(self.apr[0], instance)
                     apr_max = np.maximum(self.apr[1], instance)
                     apr = (apr_min, apr_max)
                     new_aprs.append(apr)
                     new_aprs_size.append(self.size(apr))
-            print(new_aprs_size)
 
             # actualizamos nuestro apr
             self.apr = new_aprs[new_aprs_size.index(min(new_aprs_size))]
 
     def discriminate(self, margin=0.1):
         selected_features = []
         negative_bag_indices = np.where(self.y_train == 0)[0]
```

### Comparing `mimllearning-0.2.7/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.2.8/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.2.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.2.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.2.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/data/arff_to_csv.py` & `mimllearning-0.2.8/src/miml/data/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/data/bag.py` & `mimllearning-0.2.8/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/data/instance.py` & `mimllearning-0.2.8/src/miml/data/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class Instance:
     """
     Class to manage MIML Instance data representation
     """
 
-    def __init__(self, values: np.ndarray = None, bag=None) -> None:
+    def __init__(self, values: list = None, bag=None) -> None:
         """
         Constructor of the class Instance
 
         Parameters
         ----------
         values : list[float], default=None
             Values for the instance attributes
```

### Comparing `mimllearning-0.2.7/src/miml/data/load_datasets.py` & `mimllearning-0.2.8/src/miml/data/load_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,21 +138,21 @@
             line = line[line.find(delimiter) + 1:]
             values = line[:line.find(delimiter, 2)]
             # Separamos los valores por instancias de la bolsa
             values = values.split("\\n")
 
             # El resto de la cadena se trata de las etiquetas
             labels = line[line.find(delimiter, 2) + 2:]
-            labels_values = np.array([int(i) for i in labels.split(",")], ndmin=1)
+            labels_values = [int(i) for i in labels.split(",")]
             # print("Labels: ", labels)
 
             values_list = []
             for v in values:
-                values_instance = np.array([float(i) for i in v.split(',')], ndmin=1)
-                instance = Instance(np.hstack((values_instance, labels_values)))
+                values_instance = [float(i) for i in v.split(',')]
+                instance = Instance(values_instance+labels_values)
                 if key not in dataset.data:
                     bag = Bag(key)
                     bag.add_instance(instance)
                     dataset.add_bag(bag)
                 else:
                     dataset.add_instance(key, instance)
```

### Comparing `mimllearning-0.2.7/src/miml/data/miml_dataset.py` & `mimllearning-0.2.8/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/datasets/miml_birds.arff` & `mimllearning-0.2.8/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/datasets/miml_birds.csv` & `mimllearning-0.2.8/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.2.8/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.2.8/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/test/data_test.py` & `mimllearning-0.2.8/src/miml/test/data_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
-from data.bag import Bag
-from data.instance import Instance
-from data.miml_dataset import MIMLDataset
+from miml.data.bag import Bag
+from miml.data.instance import Instance
+from miml.data.miml_dataset import MIMLDataset
 
 
 class TestData(unittest.TestCase):
     def test_instance(self):
         values = [2, 7, 5.09, 1, 0]
         instance = Instance(values)
         self.assertEqual(instance.get_number_attributes(), 5)
```

### Comparing `mimllearning-0.2.7/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.2.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.2.8/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.2.8/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.2.8/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/tutorial/classifiers_tutorial.py` & `mimllearning-0.2.8/src/miml/tutorial/classifiers_tutorial.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/tutorial/demo_MIML.ipynb` & `mimllearning-0.2.8/src/miml/tutorial/demo_MIML.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/src/miml/tutorial/tests.py` & `mimllearning-0.2.8/src/miml/tutorial/tests.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/README.md` & `mimllearning-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.7/pyproject.toml` & `mimllearning-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.2.7"
+version = "0.2.8"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.2.7/PKG-INFO` & `mimllearning-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.2.7
+Version: 0.2.8
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

