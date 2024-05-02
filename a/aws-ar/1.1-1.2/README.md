# Comparing `tmp/aws-ar-1.1.tar.gz` & `tmp/aws-ar-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ar-1.1.tar", last modified: Thu May  2 17:43:21 2024, max compression
+gzip compressed data, was "aws-ar-1.2.tar", last modified: Thu May  2 18:15:10 2024, max compression
```

## Comparing `aws-ar-1.1.tar` & `aws-ar-1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 17:43:21.981138 aws-ar-1.1/
--rw-r--r--   0 shashankdubey   (501) staff       (20)       92 2024-05-02 17:43:21.980954 aws-ar-1.1/PKG-INFO
-drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 17:43:21.980045 aws-ar-1.1/aws_ar/
--rw-r--r--   0 shashankdubey   (501) staff       (20)        0 2024-05-02 13:26:47.000000 aws-ar-1.1/aws_ar/__init__.py
--rw-r--r--   0 shashankdubey   (501) staff       (20)     1652 2024-05-02 15:50:14.000000 aws-ar-1.1/aws_ar/aws_ar.py
-drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 17:43:21.980771 aws-ar-1.1/aws_ar.egg-info/
--rw-r--r--   0 shashankdubey   (501) staff       (20)       92 2024-05-02 17:43:21.000000 aws-ar-1.1/aws_ar.egg-info/PKG-INFO
--rw-r--r--   0 shashankdubey   (501) staff       (20)      226 2024-05-02 17:43:21.000000 aws-ar-1.1/aws_ar.egg-info/SOURCES.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)        1 2024-05-02 17:43:21.000000 aws-ar-1.1/aws_ar.egg-info/dependency_links.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)       46 2024-05-02 17:43:21.000000 aws-ar-1.1/aws_ar.egg-info/entry_points.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)        6 2024-05-02 17:43:21.000000 aws-ar-1.1/aws_ar.egg-info/requires.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)        7 2024-05-02 17:43:21.000000 aws-ar-1.1/aws_ar.egg-info/top_level.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)       38 2024-05-02 17:43:21.981183 aws-ar-1.1/setup.cfg
--rw-r--r--   0 shashankdubey   (501) staff       (20)      390 2024-05-02 17:42:48.000000 aws-ar-1.1/setup.py
+drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:15:10.607092 aws-ar-1.2/
+-rw-r--r--   0 shashankdubey   (501) staff       (20)       92 2024-05-02 18:15:10.606884 aws-ar-1.2/PKG-INFO
+-rw-r--r--   0 shashankdubey   (501) staff       (20)     1543 2024-05-02 18:12:31.000000 aws-ar-1.2/README.md
+drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:15:10.605861 aws-ar-1.2/aws_ar/
+-rw-r--r--   0 shashankdubey   (501) staff       (20)        0 2024-05-02 13:26:47.000000 aws-ar-1.2/aws_ar/__init__.py
+-rw-r--r--   0 shashankdubey   (501) staff       (20)     1652 2024-05-02 15:50:14.000000 aws-ar-1.2/aws_ar/aws_ar.py
+drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:15:10.606672 aws-ar-1.2/aws_ar.egg-info/
+-rw-r--r--   0 shashankdubey   (501) staff       (20)       92 2024-05-02 18:15:10.000000 aws-ar-1.2/aws_ar.egg-info/PKG-INFO
+-rw-r--r--   0 shashankdubey   (501) staff       (20)      236 2024-05-02 18:15:10.000000 aws-ar-1.2/aws_ar.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)        1 2024-05-02 18:15:10.000000 aws-ar-1.2/aws_ar.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)       46 2024-05-02 18:15:10.000000 aws-ar-1.2/aws_ar.egg-info/entry_points.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)        6 2024-05-02 18:15:10.000000 aws-ar-1.2/aws_ar.egg-info/requires.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)        7 2024-05-02 18:15:10.000000 aws-ar-1.2/aws_ar.egg-info/top_level.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)       38 2024-05-02 18:15:10.607132 aws-ar-1.2/setup.cfg
+-rw-r--r--   0 shashankdubey   (501) staff       (20)      390 2024-05-02 18:14:59.000000 aws-ar-1.2/setup.py
```

### Comparing `aws-ar-1.1/aws_ar/aws_ar.py` & `aws-ar-1.2/aws_ar/aws_ar.py`

 * *Files identical despite different names*

