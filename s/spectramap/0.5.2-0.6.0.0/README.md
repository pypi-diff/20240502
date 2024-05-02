# Comparing `tmp/spectramap-0.5.2.tar.gz` & `tmp/spectramap-0.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectramap-0.5.2.tar", last modified: Sat Jul 16 18:02:44 2022, max compression
+gzip compressed data, was "spectramap-0.6.0.0.tar", last modified: Thu May  2 21:30:21 2024, max compression
```

## Comparing `spectramap-0.5.2.tar` & `spectramap-0.6.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-07-16 18:02:44.140886 spectramap-0.5.2/
--rw-rw-rw-   0        0        0     1091 2022-01-13 15:36:20.000000 spectramap-0.5.2/LICENSE
--rw-rw-rw-   0        0        0    19431 2022-07-16 18:02:44.137887 spectramap-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    18462 2022-07-16 17:44:23.000000 spectramap-0.5.2/README.md
--rw-rw-rw-   0        0        0      108 2022-01-13 15:36:21.000000 spectramap-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-16 18:02:44.140886 spectramap-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1045 2022-07-16 17:28:06.000000 spectramap-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-16 18:02:44.041947 spectramap-0.5.2/src/
-drwxrwxrwx   0        0        0        0 2022-07-16 18:02:44.079924 spectramap-0.5.2/src/spectramap/
--rw-rw-rw-   0        0        0        0 2022-01-19 17:39:13.000000 spectramap-0.5.2/src/spectramap/__init__.py
--rw-rw-rw-   0        0        0   115853 2022-07-16 17:58:37.000000 spectramap-0.5.2/src/spectramap/spmap.py
-drwxrwxrwx   0        0        0        0 2022-07-16 18:02:44.134889 spectramap-0.5.2/src/spectramap.egg-info/
--rw-rw-rw-   0        0        0    19431 2022-07-16 18:02:43.000000 spectramap-0.5.2/src/spectramap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2022-07-16 18:02:44.000000 spectramap-0.5.2/src/spectramap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-16 18:02:43.000000 spectramap-0.5.2/src/spectramap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2022-07-16 18:02:43.000000 spectramap-0.5.2/src/spectramap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-07-16 18:02:43.000000 spectramap-0.5.2/src/spectramap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 21:30:21.986589 spectramap-0.6.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-25 10:12:00.000000 spectramap-0.6.0.0/LICENSE
+-rw-rw-rw-   0        0        0     6829 2024-05-02 21:30:21.984079 spectramap-0.6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6041 2024-05-02 20:32:48.000000 spectramap-0.6.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-02-25 10:12:00.000000 spectramap-0.6.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 21:30:21.987101 spectramap-0.6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2024-05-02 21:10:29.000000 spectramap-0.6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:30:21.958524 spectramap-0.6.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 21:30:21.970403 spectramap-0.6.0.0/src/spectramap/
+-rw-rw-rw-   0        0        0        0 2023-02-25 10:12:00.000000 spectramap-0.6.0.0/src/spectramap/__init__.py
+-rw-rw-rw-   0        0        0    33727 2024-05-02 20:28:23.000000 spectramap-0.6.0.0/src/spectramap/spectramap.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:30:21.984079 spectramap-0.6.0.0/src/spectramap.egg-info/
+-rw-rw-rw-   0        0        0     6829 2024-05-02 21:30:21.000000 spectramap-0.6.0.0/src/spectramap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-02 21:30:21.000000 spectramap-0.6.0.0/src/spectramap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 21:30:21.000000 spectramap-0.6.0.0/src/spectramap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-02 21:30:21.000000 spectramap-0.6.0.0/src/spectramap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 21:30:21.000000 spectramap-0.6.0.0/src/spectramap.egg-info/top_level.txt
```

### Comparing `spectramap-0.5.2/LICENSE` & `spectramap-0.6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectramap-0.5.2/setup.py` & `spectramap-0.6.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spectramap",
-    version="0.5.2",
+    version="0.6.0.0",
     author="Juan David Muñoz-Bolaños",
     author_email="jmunozbolanos@gmail.com",
     description="Hyperspectral package for spectroscopists",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/spectramap/spectramap",
+    url="https://github.com/MicroscopeMaestro/spectramap",
     project_urls={
-        "Bug Tracker": "https://github.com/spectramap/spectramap",
+        "Bug Tracker": "https://github.com/MicroscopeMaestro/spectramap",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 	"Intended Audience :: Science/Research",
 	"Development Status :: 3 - Alpha",
 	"Topic :: Software Development :: Bug Tracking"
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
-    install_requires=["scikit-learn", "pyspectra", "scipy"],
+    python_requires=">=3.7",
+    install_requires=["scikit-learn", "scipy", "numpy"],
 )
```

