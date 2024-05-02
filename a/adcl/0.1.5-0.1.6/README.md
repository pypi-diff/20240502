# Comparing `tmp/adcl-0.1.5.tar.gz` & `tmp/adcl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adcl-0.1.5.tar", last modified: Thu May  2 07:05:48 2024, max compression
+gzip compressed data, was "dist\adcl-0.1.6.tar", last modified: Thu May  2 07:08:57 2024, max compression
```

## Comparing `adcl-0.1.5.tar` & `adcl-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 07:05:48.000000 adcl-0.1.5/
--rw-rw-rw-   0        0        0     1091 2024-05-01 20:17:28.000000 adcl-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      967 2024-05-02 07:05:48.000000 adcl-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3754 2024-05-01 20:17:28.000000 adcl-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl/
--rw-rw-rw-   0        0        0       35 2024-05-01 20:17:28.000000 adcl-0.1.5/adcl/__init__.py
--rw-rw-rw-   0        0        0    53906 2024-05-01 20:17:28.000000 adcl-0.1.5/adcl/data_preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/
--rw-rw-rw-   0        0        0      967 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      131 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-02 07:05:48.000000 adcl-0.1.5/adcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 07:05:48.000000 adcl-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1862 2024-05-02 07:04:43.000000 adcl-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:08:57.000000 adcl-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2024-05-01 20:17:28.000000 adcl-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4567 2024-05-02 07:08:57.000000 adcl-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3754 2024-05-01 20:17:28.000000 adcl-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 07:08:57.000000 adcl-0.1.6/adcl/
+-rw-rw-rw-   0        0        0       35 2024-05-01 20:17:28.000000 adcl-0.1.6/adcl/__init__.py
+-rw-rw-rw-   0        0        0    53906 2024-05-01 20:17:28.000000 adcl-0.1.6/adcl/data_preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:08:57.000000 adcl-0.1.6/adcl.egg-info/
+-rw-rw-rw-   0        0        0     4567 2024-05-02 07:08:57.000000 adcl-0.1.6/adcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-02 07:08:57.000000 adcl-0.1.6/adcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 07:08:57.000000 adcl-0.1.6/adcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-02 07:05:48.000000 adcl-0.1.6/adcl.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      131 2024-05-02 07:08:57.000000 adcl-0.1.6/adcl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-02 07:08:57.000000 adcl-0.1.6/adcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 07:08:57.000000 adcl-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2024-05-02 07:08:19.000000 adcl-0.1.6/setup.py
```

### Comparing `adcl-0.1.5/LICENSE` & `adcl-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adcl-0.1.5/README.md` & `adcl-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `adcl-0.1.5/adcl/data_preprocessing.py` & `adcl-0.1.6/adcl/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `adcl-0.1.5/setup.py` & `adcl-0.1.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from setuptools import setup, find_packages
 
 setup(
     name='adcl',
-    version='0.1.5',
-    description='Automatic Data Cleaning and Preprocessing Library',
-    long_description='''This package provides comprehensive data cleaning,
-                        preprocessing, and outlier detection functionalities
-                        tailored for machine learning and data science projects.''',
-    author='Your Name',
-    author_email='your.email@example.com',
-    url='https://github.com/yourgithub/ADCL-Automatic-Data-Cleaning',
+    version='0.1.6',
+    author='Maykov Stepan',
+    author_email='steve19992@mail.ru',
+    description='Data preprocessing and cleaning tools for data science projects',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    url='https://github.com/maykov-stepan/ADCL-Automatic-Data-Cleaning',
     packages=find_packages(),
     install_requires=[
-        'numpy>=1.16.2,<1.17.0',  # Adjusted to accommodate mxnet's requirements
-        'matplotlib>=3.5.3',      # Ensure this is compatible with other dependencies
-        'adtk>=0.6.2',            # Advanced data analysis toolkit
-        'category-encoders>=2.6.3',  # For categorical variable encoding
-        'dtaidistance',           # Dynamic Time Warping (DTW) distance calculation library
-        'matrixprofile>=1.1.10',  # Matrix profile for time-series analysis
-        'mxnet==1.7.0.post2'      # Deep learning framework
+        'numpy>=1.16.2,<1.17.0',  # Maintained compatibility with other dependencies
+        'matplotlib==3.2.2',      # Downgraded to maintain compatibility with numpy version
+        'adtk>=0.6.2',
+        'category-encoders>=2.6.3',
+        'dtaidistance',
+        'matrixprofile>=1.1.10',
+        'mxnet==1.7.0.post2',     # Ensure compatibility
         # Add any additional dependencies your package might require
     ],
-    python_requires='>=3.7,<3.8',  # Compatible Python versions
+    python_requires='>=3.7,<3.8',  # Specify compatible Python versions
     classifiers=[
-        'Development Status :: 4 - Beta',  # Change as appropriate
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Natural Language :: English',
-        'License :: OSI Approved :: MIT License',  # Ensure license matches your choice
+        'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     keywords='data cleaning, preprocessing, data science, machine learning',
     license='MIT',
     include_package_data=True,
     zip_safe=False
-)
+)
```

