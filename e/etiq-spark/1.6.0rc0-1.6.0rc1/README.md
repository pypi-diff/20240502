# Comparing `tmp/etiq_spark-1.6.0rc0-cp39-cp39-win_amd64.whl.zip` & `tmp/etiq_spark-1.6.0rc1-cp37-cp37m-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 440900 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  1313280 b- defN 24-Apr-25 14:37 etiq/spark.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1317 b- defN 24-Apr-25 14:37 etiq/spark.pyi
--rw-rw-rw-  2.0 fat     2078 b- defN 24-Apr-25 14:37 etiq_spark-1.6.0rc0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 24-Apr-25 14:37 etiq_spark-1.6.0rc0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-25 14:36 etiq_spark-1.6.0rc0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      481 b- defN 24-Apr-25 14:37 etiq_spark-1.6.0rc0.dist-info/RECORD
-6 files, 1317255 bytes uncompressed, 440032 bytes compressed:  66.6%
+Zip file size: 549011 bytes, number of entries: 6
+-rw-r--r--  2.0 unx  1745336 b- defN 24-May-02 14:34 etiq/spark.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-02 14:34 etiq/spark.pyi
+-rw-r--r--  2.0 unx     2027 b- defN 24-May-02 14:34 etiq_spark-1.6.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       96 b- defN 24-May-02 14:34 etiq_spark-1.6.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-02 14:33 etiq_spark-1.6.0rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      494 b- defN 24-May-02 14:34 etiq_spark-1.6.0rc1.dist-info/RECORD
+6 files, 1749275 bytes uncompressed, 548117 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: etiq/spark.cp39-win_amd64.pyd
+Filename: etiq/spark.cpython-37m-x86_64-linux-gnu.so
 Comment: 
 
 Filename: etiq/spark.pyi
 Comment: 
 
-Filename: etiq_spark-1.6.0rc0.dist-info/METADATA
+Filename: etiq_spark-1.6.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: etiq_spark-1.6.0rc0.dist-info/WHEEL
+Filename: etiq_spark-1.6.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: etiq_spark-1.6.0rc0.dist-info/top_level.txt
+Filename: etiq_spark-1.6.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: etiq_spark-1.6.0rc0.dist-info/RECORD
+Filename: etiq_spark-1.6.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `etiq_spark-1.6.0rc0.dist-info/METADATA` & `etiq_spark-1.6.0rc1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1
-Name: etiq-spark
-Version: 1.6.0rc0
-Summary: This is an optional, extension to the etiq library to provide spark datasets
-Author-email: ETIQ AI <devops@etiq.ai>
-Project-URL: homepage, https://etiq.ai
-Keywords: ai,bias,etiq,fairness
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Framework :: IPython
-Classifier: Framework :: Jupyter
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: <3.12,>=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: etiq ==1.6.0rc0
-Requires-Dist: pyspark[pandas_on_spark] >=3.3.2
-
-# ETIQ AI
-
-Etiq helps companies test and monitor ML models. For data science & ML teams,
-Etiq tests ML algorithms, identifying issues and preventing accuracy loss in
-both building & production stages. Etiq helps identify the following issue
-types in the dataset/model: Bias, Data Leakage, Accuracy Issues, Drift, across
-both pre-production and production stages. Additionally, Etiq helps identify
-which segments are impacted by each issue type and provides modular tests
-that you can plug at different points in your pipeline.
-
-## Getting Started
-
-To get started with this package, view our quickstart guide at
-https://docs.etiq.ai/
-
-
-## Licence
-
-This library is distributed under the Creative Commons "Attribution-NoDerivatives 4.0
-International (CC BY-ND 4.0)":
-
-https://creativecommons.org/licenses/by-nd/4.0/
+Metadata-Version: 2.1
+Name: etiq-spark
+Version: 1.6.0rc1
+Summary: This is an optional, extension to the etiq library to provide spark datasets
+Author-email: ETIQ AI <devops@etiq.ai>
+Project-URL: homepage, https://etiq.ai
+Keywords: ai,bias,etiq,fairness
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Framework :: IPython
+Classifier: Framework :: Jupyter
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: <3.12,>=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: etiq ==1.6.0rc1
+Requires-Dist: pyspark[pandas_on_spark] >=3.3.2
+
+# ETIQ AI
+
+Etiq helps companies test and monitor ML models. For data science & ML teams,
+Etiq tests ML algorithms, identifying issues and preventing accuracy loss in
+both building & production stages. Etiq helps identify the following issue
+types in the dataset/model: Bias, Data Leakage, Accuracy Issues, Drift, across
+both pre-production and production stages. Additionally, Etiq helps identify
+which segments are impacted by each issue type and provides modular tests
+that you can plug at different points in your pipeline.
+
+## Getting Started
+
+To get started with this package, view our quickstart guide at
+https://docs.etiq.ai/
+
+
+## Licence
+
+This library is distributed under the Creative Commons "Attribution-NoDerivatives 4.0
+International (CC BY-ND 4.0)":
+
+https://creativecommons.org/licenses/by-nd/4.0/
```

