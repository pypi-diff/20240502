# Comparing `tmp/deepface-0.0.90.tar.gz` & `tmp/deepface-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deepface-0.0.90.tar", last modified: Tue Apr 16 21:04:24 2024, max compression
+gzip compressed data, was "dist/deepface-0.0.91.tar", last modified: Thu May  2 07:27:07 2024, max compression
```

## Comparing `deepface-0.0.90.tar` & `deepface-0.0.91.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.599128 deepface-0.0.90/
--rw-r--r--   0 sefik      (501) staff       (20)     1077 2023-10-22 18:40:56.000000 deepface-0.0.90/LICENSE
--rw-r--r--   0 sefik      (501) staff       (20)    26049 2024-04-16 21:04:24.598521 deepface-0.0.90/PKG-INFO
--rw-r--r--   0 sefik      (501) staff       (20)    25497 2024-04-14 08:51:12.000000 deepface-0.0.90/README.md
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.574627 deepface-0.0.90/deepface/
--rw-r--r--   0 sefik      (501) staff       (20)    21984 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/DeepFace.py
--rw-r--r--   0 sefik      (501) staff       (20)       23 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.577052 deepface-0.0.90/deepface/api/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.577739 deepface-0.0.90/deepface/api/src/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/__init__.py
--rw-r--r--   0 sefik      (501) staff       (20)      306 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/api.py
--rw-r--r--   0 sefik      (501) staff       (20)      206 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/app.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.578013 deepface-0.0.90/deepface/api/src/modules/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/modules/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.578686 deepface-0.0.90/deepface/api/src/modules/core/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/modules/core/__init__.py
--rw-r--r--   0 sefik      (501) staff       (20)     3092 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/api/src/modules/core/routes.py
--rw-r--r--   0 sefik      (501) staff       (20)     1665 2024-02-04 13:08:55.000000 deepface-0.0.90/deepface/api/src/modules/core/service.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.582829 deepface-0.0.90/deepface/basemodels/
--rw-r--r--   0 sefik      (501) staff       (20)     4962 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/ArcFace.py
--rw-r--r--   0 sefik      (501) staff       (20)     2641 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/DeepID.py
--rw-r--r--   0 sefik      (501) staff       (20)     2872 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/Dlib.py
--rw-r--r--   0 sefik      (501) staff       (20)    61329 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/Facenet.py
--rw-r--r--   0 sefik      (501) staff       (20)     3712 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/FbDeepFace.py
--rw-r--r--   0 sefik      (501) staff       (20)     9811 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/GhostFaceNet.py
--rw-r--r--   0 sefik      (501) staff       (20)    17301 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/OpenFace.py
--rw-r--r--   0 sefik      (501) staff       (20)     2473 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/SFace.py
--rw-r--r--   0 sefik      (501) staff       (20)     5610 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/basemodels/VGGFace.py
--rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.90/deepface/basemodels/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.584800 deepface-0.0.90/deepface/commons/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.90/deepface/commons/__init__.py
--rw-r--r--   0 sefik      (501) staff       (20)      117 2024-02-02 20:17:38.000000 deepface-0.0.90/deepface/commons/constant.py
--rw-r--r--   0 sefik      (501) staff       (20)      951 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/commons/folder_utils.py
--rw-r--r--   0 sefik      (501) staff       (20)     4348 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/commons/image_utils.py
--rw-r--r--   0 sefik      (501) staff       (20)     1571 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/commons/logger.py
--rw-r--r--   0 sefik      (501) staff       (20)     1188 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/commons/package_utils.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.588679 deepface-0.0.90/deepface/detectors/
--rw-r--r--   0 sefik      (501) staff       (20)     7791 2024-04-16 19:12:52.000000 deepface-0.0.90/deepface/detectors/CenterFace.py
--rw-r--r--   0 sefik      (501) staff       (20)     7119 2024-04-16 19:12:52.000000 deepface-0.0.90/deepface/detectors/DetectorWrapper.py
--rw-r--r--   0 sefik      (501) staff       (20)     3787 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/Dlib.py
--rw-r--r--   0 sefik      (501) staff       (20)     2925 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/FastMtCnn.py
--rw-r--r--   0 sefik      (501) staff       (20)     2931 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/detectors/MediaPipe.py
--rw-r--r--   0 sefik      (501) staff       (20)     1745 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/detectors/MtCnn.py
--rw-r--r--   0 sefik      (501) staff       (20)     6038 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/detectors/OpenCv.py
--rw-r--r--   0 sefik      (501) staff       (20)     1733 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/detectors/RetinaFace.py
--rw-r--r--   0 sefik      (501) staff       (20)     5229 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/Ssd.py
--rw-r--r--   0 sefik      (501) staff       (20)     3434 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/Yolo.py
--rw-r--r--   0 sefik      (501) staff       (20)     5130 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/detectors/YuNet.py
--rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.90/deepface/detectors/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.590699 deepface-0.0.90/deepface/extendedmodels/
--rw-r--r--   0 sefik      (501) staff       (20)     2626 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/extendedmodels/Age.py
--rw-r--r--   0 sefik      (501) staff       (20)     3216 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/extendedmodels/Emotion.py
--rw-r--r--   0 sefik      (501) staff       (20)     2422 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/extendedmodels/Gender.py
--rw-r--r--   0 sefik      (501) staff       (20)     2422 2024-04-12 13:50:50.000000 deepface-0.0.90/deepface/extendedmodels/Race.py
--rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.90/deepface/extendedmodels/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.592789 deepface-0.0.90/deepface/models/
--rw-r--r--   0 sefik      (501) staff       (20)      577 2024-02-02 20:17:38.000000 deepface-0.0.90/deepface/models/Demography.py
--rw-r--r--   0 sefik      (501) staff       (20)     2882 2024-03-24 16:59:56.000000 deepface-0.0.90/deepface/models/Detector.py
--rw-r--r--   0 sefik      (501) staff       (20)     1029 2024-03-31 08:35:42.000000 deepface-0.0.90/deepface/models/FacialRecognition.py
--rw-r--r--   0 sefik      (501) staff       (20)        0 2024-01-20 12:27:18.000000 deepface-0.0.90/deepface/models/__init__.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.597962 deepface-0.0.90/deepface/modules/
--rw-r--r--   0 sefik      (501) staff       (20)        0 2024-01-13 23:12:01.000000 deepface-0.0.90/deepface/modules/__init__.py
--rw-r--r--   0 sefik      (501) staff       (20)     8291 2024-04-12 16:09:50.000000 deepface-0.0.90/deepface/modules/demography.py
--rw-r--r--   0 sefik      (501) staff       (20)     5820 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/modules/detection.py
--rw-r--r--   0 sefik      (501) staff       (20)     1674 2024-03-16 10:00:17.000000 deepface-0.0.90/deepface/modules/modeling.py
--rw-r--r--   0 sefik      (501) staff       (20)     3517 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/modules/preprocessing.py
--rw-r--r--   0 sefik      (501) staff       (20)    14173 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/modules/recognition.py
--rw-r--r--   0 sefik      (501) staff       (20)     4619 2024-04-13 07:27:53.000000 deepface-0.0.90/deepface/modules/representation.py
--rw-r--r--   0 sefik      (501) staff       (20)    31376 2024-04-12 16:09:50.000000 deepface-0.0.90/deepface/modules/streaming.py
--rw-r--r--   0 sefik      (501) staff       (20)    14303 2024-04-12 16:09:50.000000 deepface-0.0.90/deepface/modules/verification.py
-drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-04-16 21:04:24.576764 deepface-0.0.90/deepface.egg-info/
--rw-r--r--   0 sefik      (501) staff       (20)    26049 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/PKG-INFO
--rw-r--r--   0 sefik      (501) staff       (20)     1995 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/SOURCES.txt
--rw-r--r--   0 sefik      (501) staff       (20)        1 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/dependency_links.txt
--rw-r--r--   0 sefik      (501) staff       (20)       51 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/entry_points.txt
--rw-r--r--   0 sefik      (501) staff       (20)      216 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/requires.txt
--rw-r--r--   0 sefik      (501) staff       (20)        9 2024-04-16 21:04:24.000000 deepface-0.0.90/deepface.egg-info/top_level.txt
--rw-r--r--   0 sefik      (501) staff       (20)       27 2024-03-24 16:59:56.000000 deepface-0.0.90/package_info.json
--rw-r--r--   0 sefik      (501) staff       (20)      230 2024-04-13 07:27:53.000000 deepface-0.0.90/requirements.txt
--rw-r--r--   0 sefik      (501) staff       (20)       38 2024-04-16 21:04:24.599291 deepface-0.0.90/setup.cfg
--rw-r--r--   0 sefik      (501) staff       (20)     1201 2024-03-10 09:13:34.000000 deepface-0.0.90/setup.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.932185 deepface-0.0.91/
+-rw-r--r--   0 sefik      (501) staff       (20)     1077 2023-10-22 18:40:56.000000 deepface-0.0.91/LICENSE
+-rw-r--r--   0 sefik      (501) staff       (20)    26303 2024-05-02 07:27:07.931795 deepface-0.0.91/PKG-INFO
+-rw-r--r--   0 sefik      (501) staff       (20)    25755 2024-05-02 07:25:37.000000 deepface-0.0.91/README.md
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.900902 deepface-0.0.91/deepface/
+-rw-r--r--   0 sefik      (501) staff       (20)    22404 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/DeepFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)       23 2024-05-02 07:26:26.000000 deepface-0.0.91/deepface/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.903845 deepface-0.0.91/deepface/api/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.91/deepface/api/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.905317 deepface-0.0.91/deepface/api/src/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.91/deepface/api/src/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)      306 2024-02-04 13:08:55.000000 deepface-0.0.91/deepface/api/src/api.py
+-rw-r--r--   0 sefik      (501) staff       (20)      206 2024-02-04 13:08:55.000000 deepface-0.0.91/deepface/api/src/app.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.905927 deepface-0.0.91/deepface/api/src/modules/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.91/deepface/api/src/modules/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.907095 deepface-0.0.91/deepface/api/src/modules/core/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-02-04 13:08:55.000000 deepface-0.0.91/deepface/api/src/modules/core/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3092 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/api/src/modules/core/routes.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1665 2024-02-04 13:08:55.000000 deepface-0.0.91/deepface/api/src/modules/core/service.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.912909 deepface-0.0.91/deepface/basemodels/
+-rw-r--r--   0 sefik      (501) staff       (20)     4962 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/ArcFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2641 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/DeepID.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2872 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/Dlib.py
+-rw-r--r--   0 sefik      (501) staff       (20)    61329 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/Facenet.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3712 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/FbDeepFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     9811 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/GhostFaceNet.py
+-rw-r--r--   0 sefik      (501) staff       (20)    17301 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/OpenFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2473 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/SFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5610 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/basemodels/VGGFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.91/deepface/basemodels/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.915171 deepface-0.0.91/deepface/commons/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.91/deepface/commons/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)      117 2024-02-02 20:17:38.000000 deepface-0.0.91/deepface/commons/constant.py
+-rw-r--r--   0 sefik      (501) staff       (20)      951 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/commons/folder_utils.py
+-rw-r--r--   0 sefik      (501) staff       (20)     4348 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/commons/image_utils.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1571 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/commons/logger.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1188 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/commons/package_utils.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.921233 deepface-0.0.91/deepface/detectors/
+-rw-r--r--   0 sefik      (501) staff       (20)     7791 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/detectors/CenterFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     7119 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/detectors/DetectorWrapper.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3787 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/detectors/Dlib.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2925 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/detectors/FastMtCnn.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2931 2024-03-24 16:59:56.000000 deepface-0.0.91/deepface/detectors/MediaPipe.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1745 2024-03-24 16:59:56.000000 deepface-0.0.91/deepface/detectors/MtCnn.py
+-rw-r--r--   0 sefik      (501) staff       (20)     6038 2024-03-24 16:59:56.000000 deepface-0.0.91/deepface/detectors/OpenCv.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1733 2024-03-24 16:59:56.000000 deepface-0.0.91/deepface/detectors/RetinaFace.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5229 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/detectors/Ssd.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3434 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/detectors/Yolo.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5130 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/detectors/YuNet.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.91/deepface/detectors/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.923265 deepface-0.0.91/deepface/extendedmodels/
+-rw-r--r--   0 sefik      (501) staff       (20)     2626 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/extendedmodels/Age.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3216 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/extendedmodels/Emotion.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2422 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/extendedmodels/Gender.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2422 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/extendedmodels/Race.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2021-09-07 17:19:21.000000 deepface-0.0.91/deepface/extendedmodels/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.925488 deepface-0.0.91/deepface/models/
+-rw-r--r--   0 sefik      (501) staff       (20)      577 2024-02-02 20:17:38.000000 deepface-0.0.91/deepface/models/Demography.py
+-rw-r--r--   0 sefik      (501) staff       (20)     2882 2024-03-24 16:59:56.000000 deepface-0.0.91/deepface/models/Detector.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1029 2024-03-31 08:35:42.000000 deepface-0.0.91/deepface/models/FacialRecognition.py
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-01-20 12:27:18.000000 deepface-0.0.91/deepface/models/__init__.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.930749 deepface-0.0.91/deepface/modules/
+-rw-r--r--   0 sefik      (501) staff       (20)        0 2024-01-13 23:12:01.000000 deepface-0.0.91/deepface/modules/__init__.py
+-rw-r--r--   0 sefik      (501) staff       (20)     8291 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/modules/demography.py
+-rw-r--r--   0 sefik      (501) staff       (20)     5820 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/modules/detection.py
+-rw-r--r--   0 sefik      (501) staff       (20)     1674 2024-03-16 10:00:17.000000 deepface-0.0.91/deepface/modules/modeling.py
+-rw-r--r--   0 sefik      (501) staff       (20)     3517 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/modules/preprocessing.py
+-rw-r--r--   0 sefik      (501) staff       (20)    14173 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/modules/recognition.py
+-rw-r--r--   0 sefik      (501) staff       (20)     4619 2024-05-02 07:25:37.000000 deepface-0.0.91/deepface/modules/representation.py
+-rw-r--r--   0 sefik      (501) staff       (20)    31376 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/modules/streaming.py
+-rw-r--r--   0 sefik      (501) staff       (20)    14725 2024-04-30 19:23:53.000000 deepface-0.0.91/deepface/modules/verification.py
+drwxr-xr-x   0 sefik      (501) staff       (20)        0 2024-05-02 07:27:07.903502 deepface-0.0.91/deepface.egg-info/
+-rw-r--r--   0 sefik      (501) staff       (20)    26303 2024-05-02 07:27:07.000000 deepface-0.0.91/deepface.egg-info/PKG-INFO
+-rw-r--r--   0 sefik      (501) staff       (20)     1995 2024-05-02 07:27:07.000000 deepface-0.0.91/deepface.egg-info/SOURCES.txt
+-rw-r--r--   0 sefik      (501) staff       (20)        1 2024-05-02 07:27:07.000000 deepface-0.0.91/deepface.egg-info/dependency_links.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       51 2024-05-02 07:27:07.000000 deepface-0.0.91/deepface.egg-info/entry_points.txt
+-rw-r--r--   0 sefik      (501) staff       (20)      216 2024-05-02 07:27:07.000000 deepface-0.0.91/deepface.egg-info/requires.txt
+-rw-r--r--   0 sefik      (501) staff       (20)        9 2024-05-02 07:27:07.000000 deepface-0.0.91/deepface.egg-info/top_level.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       27 2024-05-02 07:26:16.000000 deepface-0.0.91/package_info.json
+-rw-r--r--   0 sefik      (501) staff       (20)      230 2024-04-30 19:23:53.000000 deepface-0.0.91/requirements.txt
+-rw-r--r--   0 sefik      (501) staff       (20)       38 2024-05-02 07:27:07.932367 deepface-0.0.91/setup.cfg
+-rw-r--r--   0 sefik      (501) staff       (20)     1220 2024-05-02 07:25:37.000000 deepface-0.0.91/setup.py
```

### Comparing `deepface-0.0.90/LICENSE` & `deepface-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/PKG-INFO` & `deepface-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deepface
-Version: 0.0.90
+Version: 0.0.91
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/serengil/deepface
 Author: Sefik Ilkin Serengil
 Author-email: serengil@gmail.com
-License: UNKNOWN
+License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,22 +26,23 @@
 
 [![Blog](https://img.shields.io/:blog-sefiks.com-blue.svg?style=flat&logo=wordpress)](https://sefiks.com)
 [![YouTube](https://img.shields.io/:youtube-@sefiks-red.svg?style=flat&logo=youtube)](https://www.youtube.com/@sefiks?sub_confirmation=1)
 [![Twitter](https://img.shields.io/:follow-@serengil-blue.svg?style=flat&logo=twitter)](https://twitter.com/intent/user?screen_name=serengil)
 [![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dserengil%26type%3Dpatrons&style=flat)](https://www.patreon.com/serengil?repo=deepface)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/serengil?logo=GitHub&color=lightgray)](https://github.com/sponsors/serengil)
 
+[![DOI](http://img.shields.io/:DOI-10.17671/gazibtd.1399077-blue.svg?style=flat)](https://doi.org/10.17671/gazibtd.1399077)
 [![DOI](http://img.shields.io/:DOI-10.1109/ASYU50717.2020.9259802-blue.svg?style=flat)](https://doi.org/10.1109/ASYU50717.2020.9259802)
 [![DOI](http://img.shields.io/:DOI-10.1109/ICEET53442.2021.9659697-blue.svg?style=flat)](https://doi.org/10.1109/ICEET53442.2021.9659697)
 
 </div>
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/deepface-icon-labeled.png" width="200" height="240"></p>
 
-Deepface is a lightweight [face recognition](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) and facial attribute analysis ([age](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [gender](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [emotion](https://sefiks.com/2018/01/01/facial-expression-recognition-with-keras/) and [race](https://sefiks.com/2019/11/11/race-and-ethnicity-prediction-in-keras/)) framework for python. It is a hybrid face recognition framework wrapping **state-of-the-art** models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/), [`Google FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`Facebook DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`.
+Deepface is a lightweight [face recognition](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) and facial attribute analysis ([age](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [gender](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [emotion](https://sefiks.com/2018/01/01/facial-expression-recognition-with-keras/) and [race](https://sefiks.com/2019/11/11/race-and-ethnicity-prediction-in-keras/)) framework for python. It is a hybrid face recognition framework wrapping **state-of-the-art** models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/), [`FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`.
 
 Experiments show that human beings have 97.53% accuracy on facial recognition tasks whereas those models already reached and passed that accuracy level.
 
 ## Installation [![PyPI](https://img.shields.io/pypi/v/deepface.svg)](https://pypi.org/project/deepface/) [![Conda](https://img.shields.io/conda/vn/conda-forge/deepface.svg)](https://anaconda.org/conda-forge/deepface)
 
 The easiest way to install deepface is to download it from [`PyPI`](https://pypi.org/project/deepface/). It's going to install the library itself and its prerequisites as well.
 
@@ -103,24 +104,24 @@
 ```
 
 This function returns an array as embedding. The size of the embedding array would be different based on the model name. For instance, VGG-Face is the default model and it represents facial images as 4096 dimensional vectors.
 
 ```python
 embedding = embedding_objs[0]["embedding"]
 assert isinstance(embedding, list)
-assert model_name = "VGG-Face" and len(embedding) == 4096
+assert model_name == "VGG-Face" and len(embedding) == 4096
 ```
 
 Here, embedding is also [plotted](https://sefiks.com/2020/05/01/a-gentle-introduction-to-face-recognition-in-deep-learning/) with 4096 slots horizontally. Each slot is corresponding to a dimension value in the embedding vector and dimension value is explained in the colorbar on the right. Similar to 2D barcodes, vertical dimension stores no information in the illustration.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/embedding.jpg" width="95%" height="95%"></p>
 
 **Face recognition models** - [`Demo`](https://youtu.be/i_MOwvhbLdI)
 
-Deepface is a **hybrid** face recognition package. It currently wraps many **state-of-the-art** face recognition models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) , [`Google FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`Facebook DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`. The default configuration uses VGG-Face model.
+Deepface is a **hybrid** face recognition package. It currently wraps many **state-of-the-art** face recognition models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) , [`FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`. The default configuration uses VGG-Face model.
 
 ```python
 models = [
   "VGG-Face", 
   "Facenet", 
   "Facenet512", 
   "OpenFace", 
@@ -148,28 +149,29 @@
 embedding_objs = DeepFace.represent(img_path = "img.jpg", 
       model_name = models[2]
 )
 ```
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/model-portfolio-20240316.jpg" width="95%" height="95%"></p>
 
-FaceNet, VGG-Face, ArcFace and Dlib are [overperforming](https://youtu.be/i_MOwvhbLdI) ones based on experiments. You can find out the scores of those models below on [Labeled Faces in the Wild](https://sefiks.com/2020/08/27/labeled-faces-in-the-wild-for-face-recognition/) set declared by its creators. 
+FaceNet, VGG-Face, ArcFace and Dlib are overperforming ones based on experiments - see [`BENCHMARKS`](https://github.com/serengil/deepface/tree/master/benchmarks) for more details. You can find the measured scores of various models in DeepFace and the reported scores from their original studies in the following table.
 
-| Model          | Declared LFW Score |
-| -------------- | ------------------ |
-| VGG-Face       | 98.9%              |
-| Facenet        | 99.2%              |
-| Facenet512     | 99.6%              |
-| OpenFace       | 92.9%              |
-| DeepID         | 97.4%              |
-| Dlib           | 99.3 %             |
-| SFace          | 99.5%              |
-| ArcFace        | 99.5%              |
-| GhostFaceNet   | 99.7%              |
-| *Human-beings* | *97.5%*            |
+| Model          | Measured Score | Declared Score     |
+| -------------- | -------------- | ------------------ |
+| Facenet512     | 98.4%          | 99.6%              |
+| Human-beings   | 97.5%          | 97.5%              |
+| Facenet        | 97.4%          | 99.2%              |
+| Dlib           | 96.8%          | 99.3 %             |
+| VGG-Face       | 96.7%          | 98.9%              |
+| ArcFace        | 96.7%          | 99.5%              |
+| GhostFaceNet   | 93.3%          | 99.7%              |
+| SFace          | 93.0%          | 99.5%              |
+| OpenFace       | 78.7%          | 92.9%              |
+| DeepFace       | 69.0%          | 97.3%              |
+| DeepID         | 66.5%          | 97.4%              |
 
 Conducting experiments with those models within DeepFace may reveal disparities compared to the original studies, owing to the adoption of distinct detection or normalization techniques. Furthermore, some models have been released solely with their backbones, lacking pre-trained weights. Thus, we are utilizing their re-implementations instead of the original pre-trained weights.
 
 **Similarity**
 
 Face recognition models are regular [convolutional neural networks](https://sefiks.com/2018/03/23/convolutional-autoencoder-clustering-images-with-neural-networks/) and they are responsible to represent faces as vectors. We expect that a face pair of same person should be [more similar](https://sefiks.com/2020/05/22/fine-tuning-the-threshold-in-face-recognition/) than a face pair of different persons.
 
@@ -206,15 +208,15 @@
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/stock-2.jpg" width="95%" height="95%"></p>
 
 Age model got ± 4.65 MAE; gender model got 97.44% accuracy, 96.29% precision and 95.05% recall as mentioned in its [tutorial](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/).
 
 
 **Face Detectors** - [`Demo`](https://youtu.be/GZ2p2hj2H5k)
 
-Face detection and alignment are important early stages of a modern face recognition pipeline. Experiments show that just alignment increases the face recognition accuracy almost 1%. [`OpenCV`](https://sefiks.com/2020/02/23/face-alignment-for-face-recognition-in-python-within-opencv/), [`Ssd`](https://sefiks.com/2020/08/25/deep-face-detection-with-opencv-in-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/),  [`MtCnn`](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/), `Faster MTCNN`, [`RetinaFace`](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/), [`MediaPipe`](https://sefiks.com/2022/01/14/deep-face-detection-with-mediapipe/), `Yolo`, `YuNet` and `CenterFace` detectors are wrapped in deepface.
+Face detection and alignment are important early stages of a modern face recognition pipeline. Experiments show that just alignment increases the face recognition accuracy almost 1%. [`OpenCV`](https://sefiks.com/2020/02/23/face-alignment-for-face-recognition-in-python-within-opencv/), [`Ssd`](https://sefiks.com/2020/08/25/deep-face-detection-with-opencv-in-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/),  [`MtCnn`](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/), `Faster MtCnn`, [`RetinaFace`](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/), [`MediaPipe`](https://sefiks.com/2022/01/14/deep-face-detection-with-mediapipe/), `Yolo`, `YuNet` and `CenterFace` detectors are wrapped in deepface.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/detector-portfolio-v6.jpg" width="95%" height="95%"></p>
 
 All deepface functions accept an optional detector backend input argument. You can switch among those detectors with this argument. OpenCV is the default detector.
 
 ```python
 backends = [
@@ -258,15 +260,15 @@
 )
 ```
 
 Face recognition models are actually CNN models and they expect standard sized inputs. So, resizing is required before representation. To avoid deformation, deepface adds black padding pixels according to the target size argument after detection and alignment.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/detector-outputs-20240414.jpg" width="90%" height="90%"></p>
 
-[RetinaFace](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/) and [MTCNN](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/) seem to overperform in detection and alignment stages but they are much slower. If the speed of your pipeline is more important, then you should use opencv or ssd. On the other hand, if you consider the accuracy, then you should use retinaface or mtcnn.
+[RetinaFace](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/) and [MtCnn](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/) seem to overperform in detection and alignment stages but they are much slower. If the speed of your pipeline is more important, then you should use opencv or ssd. On the other hand, if you consider the accuracy, then you should use retinaface or mtcnn.
 
 The performance of RetinaFace is very satisfactory even in the crowd as seen in the following illustration. Besides, it comes with an incredible facial landmark detection performance. Highlighted red points show some facial landmarks such as eyes, nose and mouth. That's why, alignment score of RetinaFace is high as well.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/retinaface-results.jpeg" width="90%" height="90%">
 <br><em>The Yellow Angels - Fenerbahce Women's Volleyball Team</em>
 </p>
 
@@ -328,18 +330,14 @@
 
 #facial analysis
 $ deepface analyze -img_path tests/dataset/img1.jpg
 ```
 
 You can also run these commands if you are running deepface with docker. Please follow the instructions in the [shell script](https://github.com/serengil/deepface/blob/master/scripts/dockerize.sh#L17).
 
-## FAQ and Troubleshooting
-
-If you believe you have identified a bug or encountered a limitation in DeepFace that is not covered in the [existing issues](https://github.com/serengil/deepface/issues) or [closed issues](https://github.com/serengil/deepface/issues?q=is%3Aissue+is%3Aclosed), kindly open a new issue. Ensure that your submission includes clear and detailed reproduction steps, such as your Python version, your DeepFace version, versions of dependent packages (provided by pip freeze), specifics of any exception messages, details about how you are calling DeepFace, and the input image(s) you are using.
-
 ## Contribution
 
 Pull requests are more than welcome! If you are planning to contribute a large patch, please create an issue first to get any upfront questions or design decisions out of the way first.
 
 Before creating a PR, you should run the unit tests and linting locally by running `make test && make lint` command. Once a PR sent, GitHub test workflow will be run automatically and unit test and linting jobs will be available in [GitHub actions](https://github.com/serengil/deepface/actions) before approval.
 
 ## Support
@@ -352,30 +350,45 @@
 <img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/patreon.png" width="30%" height="30%">
 </a>
 
 ## Citation
 
 Please cite deepface in your publications if it helps your research - see [`CITATIONS`](https://github.com/serengil/deepface/blob/master/CITATION.md) for more details. Here are its BibTex entries:
 
-If you use deepface in your research for facial recogntion purposes, please cite this publication.
+If you use deepface in your research for facial recogntion purposes, please cite these publications:
+
+```BibTeX
+@article{serengil2024lightface,
+  title         = {A Benchmark of Facial Recognition Pipelines and Co-Usability Performances of Modules},
+  author        = {Serengil, Sefik Ilkin and Ozpinar, Alper},
+  journal       = {Bilisim Teknolojileri Dergisi},
+  volume        = {17},
+  number        = {2},
+  pages         = {95-107},
+  year          = {2024},
+  doi           = {10.17671/gazibtd.1399077},
+  url           = {https://dergipark.org.tr/en/pub/gazibtd/issue/84331/1399077},
+  publisher     = {Gazi University}
+}
+```
 
 ```BibTeX
 @inproceedings{serengil2020lightface,
   title        = {LightFace: A Hybrid Deep Face Recognition Framework},
   author       = {Serengil, Sefik Ilkin and Ozpinar, Alper},
   booktitle    = {2020 Innovations in Intelligent Systems and Applications Conference (ASYU)},
   pages        = {23-27},
   year         = {2020},
   doi          = {10.1109/ASYU50717.2020.9259802},
   url          = {https://ieeexplore.ieee.org/document/9259802},
   organization = {IEEE}
 }
 ```
 
-If you use deepface in your research for facial attribute analysis purposes such as age, gender, emotion or ethnicity prediction or face detection purposes, please cite this publication.
+If you use deepface in your research for facial attribute analysis purposes such as age, gender, emotion or ethnicity prediction, please cite this publication.
 
 ```BibTeX
 @inproceedings{serengil2021lightface,
   title        = {HyperExtended LightFace: A Facial Attribute Analysis Framework},
   author       = {Serengil, Sefik Ilkin and Ozpinar, Alper},
   booktitle    = {2021 International Conference on Engineering and Emerging Technologies (ICEET)},
   pages        = {1-4},
@@ -388,16 +401,13 @@
 
 Also, if you use deepface in your GitHub projects, please add `deepface` in the `requirements.txt`.
 
 ## Licence
 
 DeepFace is licensed under the MIT License - see [`LICENSE`](https://github.com/serengil/deepface/blob/master/LICENSE) for more details.
 
-DeepFace wraps some external face recognition models: [VGG-Face](http://www.robots.ox.ac.uk/~vgg/software/vgg_face/), [Facenet](https://github.com/davidsandberg/facenet/blob/master/LICENSE.md), [OpenFace](https://github.com/iwantooxxoox/Keras-OpenFace/blob/master/LICENSE), [DeepFace](https://github.com/swghosh/DeepFace), [DeepID](https://github.com/Ruoyiran/DeepID/blob/master/LICENSE.md), [ArcFace](https://github.com/leondgarse/Keras_insightface/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/dlib/LICENSE.txt), [SFace](https://github.com/opencv/opencv_zoo/blob/master/models/face_recognition_sface/LICENSE) and [GhostFaceNet](https://github.com/HamadYA/GhostFaceNets/blob/main/LICENSE). Besides, age, gender and race / ethnicity models were trained on the backbone of VGG-Face with transfer learning. 
-
-Similarly, DeepFace wraps many face detectors: [OpenCv](https://github.com/opencv/opencv/blob/4.x/LICENSE), [Ssd](https://github.com/opencv/opencv/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/LICENSE.txt), [MtCnn](https://github.com/ipazc/mtcnn/blob/master/LICENSE), [Fast MtCnn](https://github.com/timesler/facenet-pytorch/blob/master/LICENSE.md), [RetinaFace](https://github.com/serengil/retinaface/blob/master/LICENSE), [MediaPipe](https://github.com/google/mediapipe/blob/master/LICENSE), [YuNet](https://github.com/ShiqiYu/libfacedetection/blob/master/LICENSE), [Yolo](https://github.com/derronqi/yolov8-face/blob/main/LICENSE) and [CenterFace](https://github.com/Star-Clouds/CenterFace/blob/master/LICENSE).
+DeepFace wraps some external face recognition models: [VGG-Face](http://www.robots.ox.ac.uk/~vgg/software/vgg_face/), [Facenet](https://github.com/davidsandberg/facenet/blob/master/LICENSE.md), [OpenFace](https://github.com/iwantooxxoox/Keras-OpenFace/blob/master/LICENSE), [DeepFace](https://github.com/swghosh/DeepFace), [DeepID](https://github.com/Ruoyiran/DeepID/blob/master/LICENSE.md), [ArcFace](https://github.com/leondgarse/Keras_insightface/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/dlib/LICENSE.txt), [SFace](https://github.com/opencv/opencv_zoo/blob/master/models/face_recognition_sface/LICENSE) and [GhostFaceNet](https://github.com/HamadYA/GhostFaceNets/blob/main/LICENSE). Besides, age, gender and race / ethnicity models were trained on the backbone of VGG-Face with transfer learning. Similarly, DeepFace wraps many face detectors: [OpenCv](https://github.com/opencv/opencv/blob/4.x/LICENSE), [Ssd](https://github.com/opencv/opencv/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/LICENSE.txt), [MtCnn](https://github.com/ipazc/mtcnn/blob/master/LICENSE), [Fast MtCnn](https://github.com/timesler/facenet-pytorch/blob/master/LICENSE.md), [RetinaFace](https://github.com/serengil/retinaface/blob/master/LICENSE), [MediaPipe](https://github.com/google/mediapipe/blob/master/LICENSE), [YuNet](https://github.com/ShiqiYu/libfacedetection/blob/master/LICENSE), [Yolo](https://github.com/derronqi/yolov8-face/blob/main/LICENSE) and [CenterFace](https://github.com/Star-Clouds/CenterFace/blob/master/LICENSE). License types will be inherited when you intend to utilize those models. Please check the license types of those models for production purposes.
 
-Licence types will be inherited if you are going to use those models. Please check the license types of those models for production purposes.
 
 DeepFace [logo](https://thenounproject.com/term/face-recognition/2965879/) is created by [Adrien Coquet](https://thenounproject.com/coquet_adrien/) and it is licensed under [Creative Commons: By Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/).
```

### Comparing `deepface-0.0.90/README.md` & `deepface-0.0.91/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 
 [![Blog](https://img.shields.io/:blog-sefiks.com-blue.svg?style=flat&logo=wordpress)](https://sefiks.com)
 [![YouTube](https://img.shields.io/:youtube-@sefiks-red.svg?style=flat&logo=youtube)](https://www.youtube.com/@sefiks?sub_confirmation=1)
 [![Twitter](https://img.shields.io/:follow-@serengil-blue.svg?style=flat&logo=twitter)](https://twitter.com/intent/user?screen_name=serengil)
 [![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dserengil%26type%3Dpatrons&style=flat)](https://www.patreon.com/serengil?repo=deepface)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/serengil?logo=GitHub&color=lightgray)](https://github.com/sponsors/serengil)
 
+[![DOI](http://img.shields.io/:DOI-10.17671/gazibtd.1399077-blue.svg?style=flat)](https://doi.org/10.17671/gazibtd.1399077)
 [![DOI](http://img.shields.io/:DOI-10.1109/ASYU50717.2020.9259802-blue.svg?style=flat)](https://doi.org/10.1109/ASYU50717.2020.9259802)
 [![DOI](http://img.shields.io/:DOI-10.1109/ICEET53442.2021.9659697-blue.svg?style=flat)](https://doi.org/10.1109/ICEET53442.2021.9659697)
 
 </div>
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/deepface-icon-labeled.png" width="200" height="240"></p>
 
-Deepface is a lightweight [face recognition](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) and facial attribute analysis ([age](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [gender](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [emotion](https://sefiks.com/2018/01/01/facial-expression-recognition-with-keras/) and [race](https://sefiks.com/2019/11/11/race-and-ethnicity-prediction-in-keras/)) framework for python. It is a hybrid face recognition framework wrapping **state-of-the-art** models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/), [`Google FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`Facebook DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`.
+Deepface is a lightweight [face recognition](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) and facial attribute analysis ([age](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [gender](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [emotion](https://sefiks.com/2018/01/01/facial-expression-recognition-with-keras/) and [race](https://sefiks.com/2019/11/11/race-and-ethnicity-prediction-in-keras/)) framework for python. It is a hybrid face recognition framework wrapping **state-of-the-art** models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/), [`FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`.
 
 Experiments show that human beings have 97.53% accuracy on facial recognition tasks whereas those models already reached and passed that accuracy level.
 
 ## Installation [![PyPI](https://img.shields.io/pypi/v/deepface.svg)](https://pypi.org/project/deepface/) [![Conda](https://img.shields.io/conda/vn/conda-forge/deepface.svg)](https://anaconda.org/conda-forge/deepface)
 
 The easiest way to install deepface is to download it from [`PyPI`](https://pypi.org/project/deepface/). It's going to install the library itself and its prerequisites as well.
 
@@ -87,24 +88,24 @@
 ```
 
 This function returns an array as embedding. The size of the embedding array would be different based on the model name. For instance, VGG-Face is the default model and it represents facial images as 4096 dimensional vectors.
 
 ```python
 embedding = embedding_objs[0]["embedding"]
 assert isinstance(embedding, list)
-assert model_name = "VGG-Face" and len(embedding) == 4096
+assert model_name == "VGG-Face" and len(embedding) == 4096
 ```
 
 Here, embedding is also [plotted](https://sefiks.com/2020/05/01/a-gentle-introduction-to-face-recognition-in-deep-learning/) with 4096 slots horizontally. Each slot is corresponding to a dimension value in the embedding vector and dimension value is explained in the colorbar on the right. Similar to 2D barcodes, vertical dimension stores no information in the illustration.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/embedding.jpg" width="95%" height="95%"></p>
 
 **Face recognition models** - [`Demo`](https://youtu.be/i_MOwvhbLdI)
 
-Deepface is a **hybrid** face recognition package. It currently wraps many **state-of-the-art** face recognition models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) , [`Google FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`Facebook DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`. The default configuration uses VGG-Face model.
+Deepface is a **hybrid** face recognition package. It currently wraps many **state-of-the-art** face recognition models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) , [`FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`. The default configuration uses VGG-Face model.
 
 ```python
 models = [
   "VGG-Face", 
   "Facenet", 
   "Facenet512", 
   "OpenFace", 
@@ -132,28 +133,29 @@
 embedding_objs = DeepFace.represent(img_path = "img.jpg", 
       model_name = models[2]
 )
 ```
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/model-portfolio-20240316.jpg" width="95%" height="95%"></p>
 
-FaceNet, VGG-Face, ArcFace and Dlib are [overperforming](https://youtu.be/i_MOwvhbLdI) ones based on experiments. You can find out the scores of those models below on [Labeled Faces in the Wild](https://sefiks.com/2020/08/27/labeled-faces-in-the-wild-for-face-recognition/) set declared by its creators. 
+FaceNet, VGG-Face, ArcFace and Dlib are overperforming ones based on experiments - see [`BENCHMARKS`](https://github.com/serengil/deepface/tree/master/benchmarks) for more details. You can find the measured scores of various models in DeepFace and the reported scores from their original studies in the following table.
 
-| Model          | Declared LFW Score |
-| -------------- | ------------------ |
-| VGG-Face       | 98.9%              |
-| Facenet        | 99.2%              |
-| Facenet512     | 99.6%              |
-| OpenFace       | 92.9%              |
-| DeepID         | 97.4%              |
-| Dlib           | 99.3 %             |
-| SFace          | 99.5%              |
-| ArcFace        | 99.5%              |
-| GhostFaceNet   | 99.7%              |
-| *Human-beings* | *97.5%*            |
+| Model          | Measured Score | Declared Score     |
+| -------------- | -------------- | ------------------ |
+| Facenet512     | 98.4%          | 99.6%              |
+| Human-beings   | 97.5%          | 97.5%              |
+| Facenet        | 97.4%          | 99.2%              |
+| Dlib           | 96.8%          | 99.3 %             |
+| VGG-Face       | 96.7%          | 98.9%              |
+| ArcFace        | 96.7%          | 99.5%              |
+| GhostFaceNet   | 93.3%          | 99.7%              |
+| SFace          | 93.0%          | 99.5%              |
+| OpenFace       | 78.7%          | 92.9%              |
+| DeepFace       | 69.0%          | 97.3%              |
+| DeepID         | 66.5%          | 97.4%              |
 
 Conducting experiments with those models within DeepFace may reveal disparities compared to the original studies, owing to the adoption of distinct detection or normalization techniques. Furthermore, some models have been released solely with their backbones, lacking pre-trained weights. Thus, we are utilizing their re-implementations instead of the original pre-trained weights.
 
 **Similarity**
 
 Face recognition models are regular [convolutional neural networks](https://sefiks.com/2018/03/23/convolutional-autoencoder-clustering-images-with-neural-networks/) and they are responsible to represent faces as vectors. We expect that a face pair of same person should be [more similar](https://sefiks.com/2020/05/22/fine-tuning-the-threshold-in-face-recognition/) than a face pair of different persons.
 
@@ -190,15 +192,15 @@
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/stock-2.jpg" width="95%" height="95%"></p>
 
 Age model got ± 4.65 MAE; gender model got 97.44% accuracy, 96.29% precision and 95.05% recall as mentioned in its [tutorial](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/).
 
 
 **Face Detectors** - [`Demo`](https://youtu.be/GZ2p2hj2H5k)
 
-Face detection and alignment are important early stages of a modern face recognition pipeline. Experiments show that just alignment increases the face recognition accuracy almost 1%. [`OpenCV`](https://sefiks.com/2020/02/23/face-alignment-for-face-recognition-in-python-within-opencv/), [`Ssd`](https://sefiks.com/2020/08/25/deep-face-detection-with-opencv-in-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/),  [`MtCnn`](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/), `Faster MTCNN`, [`RetinaFace`](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/), [`MediaPipe`](https://sefiks.com/2022/01/14/deep-face-detection-with-mediapipe/), `Yolo`, `YuNet` and `CenterFace` detectors are wrapped in deepface.
+Face detection and alignment are important early stages of a modern face recognition pipeline. Experiments show that just alignment increases the face recognition accuracy almost 1%. [`OpenCV`](https://sefiks.com/2020/02/23/face-alignment-for-face-recognition-in-python-within-opencv/), [`Ssd`](https://sefiks.com/2020/08/25/deep-face-detection-with-opencv-in-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/),  [`MtCnn`](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/), `Faster MtCnn`, [`RetinaFace`](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/), [`MediaPipe`](https://sefiks.com/2022/01/14/deep-face-detection-with-mediapipe/), `Yolo`, `YuNet` and `CenterFace` detectors are wrapped in deepface.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/detector-portfolio-v6.jpg" width="95%" height="95%"></p>
 
 All deepface functions accept an optional detector backend input argument. You can switch among those detectors with this argument. OpenCV is the default detector.
 
 ```python
 backends = [
@@ -242,15 +244,15 @@
 )
 ```
 
 Face recognition models are actually CNN models and they expect standard sized inputs. So, resizing is required before representation. To avoid deformation, deepface adds black padding pixels according to the target size argument after detection and alignment.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/detector-outputs-20240414.jpg" width="90%" height="90%"></p>
 
-[RetinaFace](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/) and [MTCNN](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/) seem to overperform in detection and alignment stages but they are much slower. If the speed of your pipeline is more important, then you should use opencv or ssd. On the other hand, if you consider the accuracy, then you should use retinaface or mtcnn.
+[RetinaFace](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/) and [MtCnn](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/) seem to overperform in detection and alignment stages but they are much slower. If the speed of your pipeline is more important, then you should use opencv or ssd. On the other hand, if you consider the accuracy, then you should use retinaface or mtcnn.
 
 The performance of RetinaFace is very satisfactory even in the crowd as seen in the following illustration. Besides, it comes with an incredible facial landmark detection performance. Highlighted red points show some facial landmarks such as eyes, nose and mouth. That's why, alignment score of RetinaFace is high as well.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/retinaface-results.jpeg" width="90%" height="90%">
 <br><em>The Yellow Angels - Fenerbahce Women's Volleyball Team</em>
 </p>
 
@@ -312,18 +314,14 @@
 
 #facial analysis
 $ deepface analyze -img_path tests/dataset/img1.jpg
 ```
 
 You can also run these commands if you are running deepface with docker. Please follow the instructions in the [shell script](https://github.com/serengil/deepface/blob/master/scripts/dockerize.sh#L17).
 
-## FAQ and Troubleshooting
-
-If you believe you have identified a bug or encountered a limitation in DeepFace that is not covered in the [existing issues](https://github.com/serengil/deepface/issues) or [closed issues](https://github.com/serengil/deepface/issues?q=is%3Aissue+is%3Aclosed), kindly open a new issue. Ensure that your submission includes clear and detailed reproduction steps, such as your Python version, your DeepFace version, versions of dependent packages (provided by pip freeze), specifics of any exception messages, details about how you are calling DeepFace, and the input image(s) you are using.
-
 ## Contribution
 
 Pull requests are more than welcome! If you are planning to contribute a large patch, please create an issue first to get any upfront questions or design decisions out of the way first.
 
 Before creating a PR, you should run the unit tests and linting locally by running `make test && make lint` command. Once a PR sent, GitHub test workflow will be run automatically and unit test and linting jobs will be available in [GitHub actions](https://github.com/serengil/deepface/actions) before approval.
 
 ## Support
@@ -336,30 +334,45 @@
 <img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/patreon.png" width="30%" height="30%">
 </a>
 
 ## Citation
 
 Please cite deepface in your publications if it helps your research - see [`CITATIONS`](https://github.com/serengil/deepface/blob/master/CITATION.md) for more details. Here are its BibTex entries:
 
-If you use deepface in your research for facial recogntion purposes, please cite this publication.
+If you use deepface in your research for facial recogntion purposes, please cite these publications:
+
+```BibTeX
+@article{serengil2024lightface,
+  title         = {A Benchmark of Facial Recognition Pipelines and Co-Usability Performances of Modules},
+  author        = {Serengil, Sefik Ilkin and Ozpinar, Alper},
+  journal       = {Bilisim Teknolojileri Dergisi},
+  volume        = {17},
+  number        = {2},
+  pages         = {95-107},
+  year          = {2024},
+  doi           = {10.17671/gazibtd.1399077},
+  url           = {https://dergipark.org.tr/en/pub/gazibtd/issue/84331/1399077},
+  publisher     = {Gazi University}
+}
+```
 
 ```BibTeX
 @inproceedings{serengil2020lightface,
   title        = {LightFace: A Hybrid Deep Face Recognition Framework},
   author       = {Serengil, Sefik Ilkin and Ozpinar, Alper},
   booktitle    = {2020 Innovations in Intelligent Systems and Applications Conference (ASYU)},
   pages        = {23-27},
   year         = {2020},
   doi          = {10.1109/ASYU50717.2020.9259802},
   url          = {https://ieeexplore.ieee.org/document/9259802},
   organization = {IEEE}
 }
 ```
 
-If you use deepface in your research for facial attribute analysis purposes such as age, gender, emotion or ethnicity prediction or face detection purposes, please cite this publication.
+If you use deepface in your research for facial attribute analysis purposes such as age, gender, emotion or ethnicity prediction, please cite this publication.
 
 ```BibTeX
 @inproceedings{serengil2021lightface,
   title        = {HyperExtended LightFace: A Facial Attribute Analysis Framework},
   author       = {Serengil, Sefik Ilkin and Ozpinar, Alper},
   booktitle    = {2021 International Conference on Engineering and Emerging Technologies (ICEET)},
   pages        = {1-4},
@@ -372,14 +385,11 @@
 
 Also, if you use deepface in your GitHub projects, please add `deepface` in the `requirements.txt`.
 
 ## Licence
 
 DeepFace is licensed under the MIT License - see [`LICENSE`](https://github.com/serengil/deepface/blob/master/LICENSE) for more details.
 
-DeepFace wraps some external face recognition models: [VGG-Face](http://www.robots.ox.ac.uk/~vgg/software/vgg_face/), [Facenet](https://github.com/davidsandberg/facenet/blob/master/LICENSE.md), [OpenFace](https://github.com/iwantooxxoox/Keras-OpenFace/blob/master/LICENSE), [DeepFace](https://github.com/swghosh/DeepFace), [DeepID](https://github.com/Ruoyiran/DeepID/blob/master/LICENSE.md), [ArcFace](https://github.com/leondgarse/Keras_insightface/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/dlib/LICENSE.txt), [SFace](https://github.com/opencv/opencv_zoo/blob/master/models/face_recognition_sface/LICENSE) and [GhostFaceNet](https://github.com/HamadYA/GhostFaceNets/blob/main/LICENSE). Besides, age, gender and race / ethnicity models were trained on the backbone of VGG-Face with transfer learning. 
-
-Similarly, DeepFace wraps many face detectors: [OpenCv](https://github.com/opencv/opencv/blob/4.x/LICENSE), [Ssd](https://github.com/opencv/opencv/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/LICENSE.txt), [MtCnn](https://github.com/ipazc/mtcnn/blob/master/LICENSE), [Fast MtCnn](https://github.com/timesler/facenet-pytorch/blob/master/LICENSE.md), [RetinaFace](https://github.com/serengil/retinaface/blob/master/LICENSE), [MediaPipe](https://github.com/google/mediapipe/blob/master/LICENSE), [YuNet](https://github.com/ShiqiYu/libfacedetection/blob/master/LICENSE), [Yolo](https://github.com/derronqi/yolov8-face/blob/main/LICENSE) and [CenterFace](https://github.com/Star-Clouds/CenterFace/blob/master/LICENSE).
+DeepFace wraps some external face recognition models: [VGG-Face](http://www.robots.ox.ac.uk/~vgg/software/vgg_face/), [Facenet](https://github.com/davidsandberg/facenet/blob/master/LICENSE.md), [OpenFace](https://github.com/iwantooxxoox/Keras-OpenFace/blob/master/LICENSE), [DeepFace](https://github.com/swghosh/DeepFace), [DeepID](https://github.com/Ruoyiran/DeepID/blob/master/LICENSE.md), [ArcFace](https://github.com/leondgarse/Keras_insightface/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/dlib/LICENSE.txt), [SFace](https://github.com/opencv/opencv_zoo/blob/master/models/face_recognition_sface/LICENSE) and [GhostFaceNet](https://github.com/HamadYA/GhostFaceNets/blob/main/LICENSE). Besides, age, gender and race / ethnicity models were trained on the backbone of VGG-Face with transfer learning. Similarly, DeepFace wraps many face detectors: [OpenCv](https://github.com/opencv/opencv/blob/4.x/LICENSE), [Ssd](https://github.com/opencv/opencv/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/LICENSE.txt), [MtCnn](https://github.com/ipazc/mtcnn/blob/master/LICENSE), [Fast MtCnn](https://github.com/timesler/facenet-pytorch/blob/master/LICENSE.md), [RetinaFace](https://github.com/serengil/retinaface/blob/master/LICENSE), [MediaPipe](https://github.com/google/mediapipe/blob/master/LICENSE), [YuNet](https://github.com/ShiqiYu/libfacedetection/blob/master/LICENSE), [Yolo](https://github.com/derronqi/yolov8-face/blob/main/LICENSE) and [CenterFace](https://github.com/Star-Clouds/CenterFace/blob/master/LICENSE). License types will be inherited when you intend to utilize those models. Please check the license types of those models for production purposes.
 
-Licence types will be inherited if you are going to use those models. Please check the license types of those models for production purposes.
 
 DeepFace [logo](https://thenounproject.com/term/face-recognition/2965879/) is created by [Adrien Coquet](https://thenounproject.com/coquet_adrien/) and it is licensed under [Creative Commons: By Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/).
```

### Comparing `deepface-0.0.90/deepface/DeepFace.py` & `deepface-0.0.91/deepface/DeepFace.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     detector_backend: str = "opencv",
     distance_metric: str = "cosine",
     enforce_detection: bool = True,
     align: bool = True,
     expand_percentage: int = 0,
     normalization: str = "base",
     silent: bool = False,
+    threshold: Optional[float] = None,
 ) -> Dict[str, Any]:
     """
     Verify if an image pair represents the same person or different persons.
     Args:
         img1_path (str or np.ndarray or List[float]): Path to the first image.
             Accepts exact image path as a string, numpy array (BGR), base64 encoded images
             or pre-calculated embeddings.
@@ -103,14 +104,19 @@
 
         normalization (string): Normalize the input image before feeding it to the model.
             Options: base, raw, Facenet, Facenet2018, VGGFace, VGGFace2, ArcFace (default is base)
 
         silent (boolean): Suppress or allow some log messages for a quieter analysis process
             (default is False).
 
+        threshold (float): Specify a threshold to determine whether a pair represents the same
+            person or different individuals. This threshold is used for comparing distances.
+            If left unset, default pre-tuned threshold values will be applied based on the specified
+            model name and distance metric (default is None).
+
     Returns:
         result (dict): A dictionary containing verification results with following keys.
 
         - 'verified' (bool): Indicates whether the images represent the same person (True)
             or different persons (False).
 
         - 'distance' (float): The distance measure between the face vectors.
@@ -139,14 +145,15 @@
         detector_backend=detector_backend,
         distance_metric=distance_metric,
         enforce_detection=enforce_detection,
         align=align,
         expand_percentage=expand_percentage,
         normalization=normalization,
         silent=silent,
+        threshold=threshold,
     )
 
 
 def analyze(
     img_path: Union[str, np.ndarray],
     actions: Union[tuple, list] = ("emotion", "age", "gender", "race"),
     enforce_detection: bool = True,
```

### Comparing `deepface-0.0.90/deepface/api/src/modules/core/routes.py` & `deepface-0.0.91/deepface/api/src/modules/core/routes.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/api/src/modules/core/service.py` & `deepface-0.0.91/deepface/api/src/modules/core/service.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/ArcFace.py` & `deepface-0.0.91/deepface/basemodels/ArcFace.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/DeepID.py` & `deepface-0.0.91/deepface/basemodels/DeepID.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/Dlib.py` & `deepface-0.0.91/deepface/basemodels/Dlib.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/Facenet.py` & `deepface-0.0.91/deepface/basemodels/Facenet.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/FbDeepFace.py` & `deepface-0.0.91/deepface/basemodels/FbDeepFace.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/GhostFaceNet.py` & `deepface-0.0.91/deepface/basemodels/GhostFaceNet.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/OpenFace.py` & `deepface-0.0.91/deepface/basemodels/OpenFace.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/SFace.py` & `deepface-0.0.91/deepface/basemodels/SFace.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/basemodels/VGGFace.py` & `deepface-0.0.91/deepface/basemodels/VGGFace.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/commons/folder_utils.py` & `deepface-0.0.91/deepface/commons/folder_utils.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/commons/image_utils.py` & `deepface-0.0.91/deepface/commons/image_utils.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/commons/logger.py` & `deepface-0.0.91/deepface/commons/logger.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/commons/package_utils.py` & `deepface-0.0.91/deepface/commons/package_utils.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/CenterFace.py` & `deepface-0.0.91/deepface/detectors/CenterFace.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/DetectorWrapper.py` & `deepface-0.0.91/deepface/detectors/DetectorWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/Dlib.py` & `deepface-0.0.91/deepface/detectors/Dlib.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/FastMtCnn.py` & `deepface-0.0.91/deepface/detectors/FastMtCnn.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/MediaPipe.py` & `deepface-0.0.91/deepface/detectors/MediaPipe.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/MtCnn.py` & `deepface-0.0.91/deepface/detectors/MtCnn.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/OpenCv.py` & `deepface-0.0.91/deepface/detectors/OpenCv.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/RetinaFace.py` & `deepface-0.0.91/deepface/detectors/RetinaFace.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/Ssd.py` & `deepface-0.0.91/deepface/detectors/Ssd.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/Yolo.py` & `deepface-0.0.91/deepface/detectors/Yolo.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/detectors/YuNet.py` & `deepface-0.0.91/deepface/detectors/YuNet.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/extendedmodels/Age.py` & `deepface-0.0.91/deepface/extendedmodels/Age.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/extendedmodels/Emotion.py` & `deepface-0.0.91/deepface/extendedmodels/Emotion.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/extendedmodels/Gender.py` & `deepface-0.0.91/deepface/extendedmodels/Gender.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/extendedmodels/Race.py` & `deepface-0.0.91/deepface/extendedmodels/Race.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/models/Demography.py` & `deepface-0.0.91/deepface/models/Demography.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/models/Detector.py` & `deepface-0.0.91/deepface/models/Detector.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/models/FacialRecognition.py` & `deepface-0.0.91/deepface/models/FacialRecognition.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/modules/demography.py` & `deepface-0.0.91/deepface/modules/demography.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/modules/detection.py` & `deepface-0.0.91/deepface/modules/detection.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/modules/modeling.py` & `deepface-0.0.91/deepface/modules/modeling.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/modules/preprocessing.py` & `deepface-0.0.91/deepface/modules/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/modules/recognition.py` & `deepface-0.0.91/deepface/modules/recognition.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/modules/representation.py` & `deepface-0.0.91/deepface/modules/representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         if len(img.shape) != 3:
             raise ValueError(f"Input img must be 3 dimensional but it is {img.shape}")
 
         # make dummy region and confidence to keep compatibility with `extract_faces`
         img_objs = [
             {
                 "face": img,
-                "facial_area": {"x": 0, "y": 0, "w": img.shape[1], "h": img.shape[2]},
+                "facial_area": {"x": 0, "y": 0, "w": img.shape[0], "h": img.shape[1]},
                 "confidence": 0,
             }
         ]
     # ---------------------------------
 
     for img_obj in img_objs:
         img = img_obj["face"]
```

### Comparing `deepface-0.0.90/deepface/modules/streaming.py` & `deepface-0.0.91/deepface/modules/streaming.py`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/deepface/modules/verification.py` & `deepface-0.0.91/deepface/modules/verification.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # built-in dependencies
 import time
-from typing import Any, Dict, Union, List, Tuple
+from typing import Any, Dict, Optional, Union, List, Tuple
 
 # 3rd party dependencies
 import numpy as np
 
 # project dependencies
 from deepface.modules import representation, detection, modeling
 from deepface.models.FacialRecognition import FacialRecognition
@@ -20,14 +20,15 @@
     detector_backend: str = "opencv",
     distance_metric: str = "cosine",
     enforce_detection: bool = True,
     align: bool = True,
     expand_percentage: int = 0,
     normalization: str = "base",
     silent: bool = False,
+    threshold: Optional[float] = None,
 ) -> Dict[str, Any]:
     """
     Verify if an image pair represents the same person or different persons.
 
     The verification function converts facial images to vectors and calculates the similarity
     between those vectors. Vectors of images of the same person should exhibit higher similarity
     (or lower distance) than vectors of images of different persons.
@@ -59,14 +60,19 @@
         expand_percentage (int): expand detected facial area with a percentage (default is 0).
 
         normalization (string): Normalize the input image before feeding it to the model.
             Options: base, raw, Facenet, Facenet2018, VGGFace, VGGFace2, ArcFace (default is base)
 
         silent (boolean): Suppress or allow some log messages for a quieter analysis process
             (default is False).
+        
+        threshold (float): Specify a threshold to determine whether a pair represents the same
+            person or different individuals. This threshold is used for comparing distances.
+            If left unset, default pre-tuned threshold values will be applied based on the specified
+            model name and distance metric (default is None).
 
     Returns:
         result (dict): A dictionary containing verification results.
 
         - 'verified' (bool): Indicates whether the images represent the same person (True)
             or different persons (False).
 
@@ -182,15 +188,15 @@
             distance = find_distance(img1_embedding, img2_embedding, distance_metric)
             distances.append(distance)
             facial_areas.append(
                 (img1_facial_areas[idx] or no_facial_area, img2_facial_areas[idy] or no_facial_area)
             )
 
     # find the face pair with minimum distance
-    threshold = find_threshold(model_name, distance_metric)
+    threshold = threshold or find_threshold(model_name, distance_metric)
     distance = float(min(distances))  # best distance
     facial_areas = facial_areas[np.argmin(distances)]
 
     toc = time.time()
 
     resp_obj = {
         "verified": distance <= threshold,
```

### Comparing `deepface-0.0.90/deepface.egg-info/PKG-INFO` & `deepface-0.0.91/deepface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deepface
-Version: 0.0.90
+Version: 0.0.91
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/serengil/deepface
 Author: Sefik Ilkin Serengil
 Author-email: serengil@gmail.com
-License: UNKNOWN
+License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,22 +26,23 @@
 
 [![Blog](https://img.shields.io/:blog-sefiks.com-blue.svg?style=flat&logo=wordpress)](https://sefiks.com)
 [![YouTube](https://img.shields.io/:youtube-@sefiks-red.svg?style=flat&logo=youtube)](https://www.youtube.com/@sefiks?sub_confirmation=1)
 [![Twitter](https://img.shields.io/:follow-@serengil-blue.svg?style=flat&logo=twitter)](https://twitter.com/intent/user?screen_name=serengil)
 [![Support me on Patreon](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dserengil%26type%3Dpatrons&style=flat)](https://www.patreon.com/serengil?repo=deepface)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/serengil?logo=GitHub&color=lightgray)](https://github.com/sponsors/serengil)
 
+[![DOI](http://img.shields.io/:DOI-10.17671/gazibtd.1399077-blue.svg?style=flat)](https://doi.org/10.17671/gazibtd.1399077)
 [![DOI](http://img.shields.io/:DOI-10.1109/ASYU50717.2020.9259802-blue.svg?style=flat)](https://doi.org/10.1109/ASYU50717.2020.9259802)
 [![DOI](http://img.shields.io/:DOI-10.1109/ICEET53442.2021.9659697-blue.svg?style=flat)](https://doi.org/10.1109/ICEET53442.2021.9659697)
 
 </div>
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/deepface-icon-labeled.png" width="200" height="240"></p>
 
-Deepface is a lightweight [face recognition](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) and facial attribute analysis ([age](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [gender](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [emotion](https://sefiks.com/2018/01/01/facial-expression-recognition-with-keras/) and [race](https://sefiks.com/2019/11/11/race-and-ethnicity-prediction-in-keras/)) framework for python. It is a hybrid face recognition framework wrapping **state-of-the-art** models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/), [`Google FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`Facebook DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`.
+Deepface is a lightweight [face recognition](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) and facial attribute analysis ([age](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [gender](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/), [emotion](https://sefiks.com/2018/01/01/facial-expression-recognition-with-keras/) and [race](https://sefiks.com/2019/11/11/race-and-ethnicity-prediction-in-keras/)) framework for python. It is a hybrid face recognition framework wrapping **state-of-the-art** models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/), [`FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`.
 
 Experiments show that human beings have 97.53% accuracy on facial recognition tasks whereas those models already reached and passed that accuracy level.
 
 ## Installation [![PyPI](https://img.shields.io/pypi/v/deepface.svg)](https://pypi.org/project/deepface/) [![Conda](https://img.shields.io/conda/vn/conda-forge/deepface.svg)](https://anaconda.org/conda-forge/deepface)
 
 The easiest way to install deepface is to download it from [`PyPI`](https://pypi.org/project/deepface/). It's going to install the library itself and its prerequisites as well.
 
@@ -103,24 +104,24 @@
 ```
 
 This function returns an array as embedding. The size of the embedding array would be different based on the model name. For instance, VGG-Face is the default model and it represents facial images as 4096 dimensional vectors.
 
 ```python
 embedding = embedding_objs[0]["embedding"]
 assert isinstance(embedding, list)
-assert model_name = "VGG-Face" and len(embedding) == 4096
+assert model_name == "VGG-Face" and len(embedding) == 4096
 ```
 
 Here, embedding is also [plotted](https://sefiks.com/2020/05/01/a-gentle-introduction-to-face-recognition-in-deep-learning/) with 4096 slots horizontally. Each slot is corresponding to a dimension value in the embedding vector and dimension value is explained in the colorbar on the right. Similar to 2D barcodes, vertical dimension stores no information in the illustration.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/embedding.jpg" width="95%" height="95%"></p>
 
 **Face recognition models** - [`Demo`](https://youtu.be/i_MOwvhbLdI)
 
-Deepface is a **hybrid** face recognition package. It currently wraps many **state-of-the-art** face recognition models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) , [`Google FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`Facebook DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`. The default configuration uses VGG-Face model.
+Deepface is a **hybrid** face recognition package. It currently wraps many **state-of-the-art** face recognition models: [`VGG-Face`](https://sefiks.com/2018/08/06/deep-face-recognition-with-keras/) , [`FaceNet`](https://sefiks.com/2018/09/03/face-recognition-with-facenet-in-keras/), [`OpenFace`](https://sefiks.com/2019/07/21/face-recognition-with-openface-in-keras/), [`DeepFace`](https://sefiks.com/2020/02/17/face-recognition-with-facebook-deepface-in-keras/), [`DeepID`](https://sefiks.com/2020/06/16/face-recognition-with-deepid-in-keras/), [`ArcFace`](https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/), `SFace` and `GhostFaceNet`. The default configuration uses VGG-Face model.
 
 ```python
 models = [
   "VGG-Face", 
   "Facenet", 
   "Facenet512", 
   "OpenFace", 
@@ -148,28 +149,29 @@
 embedding_objs = DeepFace.represent(img_path = "img.jpg", 
       model_name = models[2]
 )
 ```
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/model-portfolio-20240316.jpg" width="95%" height="95%"></p>
 
-FaceNet, VGG-Face, ArcFace and Dlib are [overperforming](https://youtu.be/i_MOwvhbLdI) ones based on experiments. You can find out the scores of those models below on [Labeled Faces in the Wild](https://sefiks.com/2020/08/27/labeled-faces-in-the-wild-for-face-recognition/) set declared by its creators. 
+FaceNet, VGG-Face, ArcFace and Dlib are overperforming ones based on experiments - see [`BENCHMARKS`](https://github.com/serengil/deepface/tree/master/benchmarks) for more details. You can find the measured scores of various models in DeepFace and the reported scores from their original studies in the following table.
 
-| Model          | Declared LFW Score |
-| -------------- | ------------------ |
-| VGG-Face       | 98.9%              |
-| Facenet        | 99.2%              |
-| Facenet512     | 99.6%              |
-| OpenFace       | 92.9%              |
-| DeepID         | 97.4%              |
-| Dlib           | 99.3 %             |
-| SFace          | 99.5%              |
-| ArcFace        | 99.5%              |
-| GhostFaceNet   | 99.7%              |
-| *Human-beings* | *97.5%*            |
+| Model          | Measured Score | Declared Score     |
+| -------------- | -------------- | ------------------ |
+| Facenet512     | 98.4%          | 99.6%              |
+| Human-beings   | 97.5%          | 97.5%              |
+| Facenet        | 97.4%          | 99.2%              |
+| Dlib           | 96.8%          | 99.3 %             |
+| VGG-Face       | 96.7%          | 98.9%              |
+| ArcFace        | 96.7%          | 99.5%              |
+| GhostFaceNet   | 93.3%          | 99.7%              |
+| SFace          | 93.0%          | 99.5%              |
+| OpenFace       | 78.7%          | 92.9%              |
+| DeepFace       | 69.0%          | 97.3%              |
+| DeepID         | 66.5%          | 97.4%              |
 
 Conducting experiments with those models within DeepFace may reveal disparities compared to the original studies, owing to the adoption of distinct detection or normalization techniques. Furthermore, some models have been released solely with their backbones, lacking pre-trained weights. Thus, we are utilizing their re-implementations instead of the original pre-trained weights.
 
 **Similarity**
 
 Face recognition models are regular [convolutional neural networks](https://sefiks.com/2018/03/23/convolutional-autoencoder-clustering-images-with-neural-networks/) and they are responsible to represent faces as vectors. We expect that a face pair of same person should be [more similar](https://sefiks.com/2020/05/22/fine-tuning-the-threshold-in-face-recognition/) than a face pair of different persons.
 
@@ -206,15 +208,15 @@
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/stock-2.jpg" width="95%" height="95%"></p>
 
 Age model got ± 4.65 MAE; gender model got 97.44% accuracy, 96.29% precision and 95.05% recall as mentioned in its [tutorial](https://sefiks.com/2019/02/13/apparent-age-and-gender-prediction-in-keras/).
 
 
 **Face Detectors** - [`Demo`](https://youtu.be/GZ2p2hj2H5k)
 
-Face detection and alignment are important early stages of a modern face recognition pipeline. Experiments show that just alignment increases the face recognition accuracy almost 1%. [`OpenCV`](https://sefiks.com/2020/02/23/face-alignment-for-face-recognition-in-python-within-opencv/), [`Ssd`](https://sefiks.com/2020/08/25/deep-face-detection-with-opencv-in-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/),  [`MtCnn`](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/), `Faster MTCNN`, [`RetinaFace`](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/), [`MediaPipe`](https://sefiks.com/2022/01/14/deep-face-detection-with-mediapipe/), `Yolo`, `YuNet` and `CenterFace` detectors are wrapped in deepface.
+Face detection and alignment are important early stages of a modern face recognition pipeline. Experiments show that just alignment increases the face recognition accuracy almost 1%. [`OpenCV`](https://sefiks.com/2020/02/23/face-alignment-for-face-recognition-in-python-within-opencv/), [`Ssd`](https://sefiks.com/2020/08/25/deep-face-detection-with-opencv-in-python/), [`Dlib`](https://sefiks.com/2020/07/11/face-recognition-with-dlib-in-python/),  [`MtCnn`](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/), `Faster MtCnn`, [`RetinaFace`](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/), [`MediaPipe`](https://sefiks.com/2022/01/14/deep-face-detection-with-mediapipe/), `Yolo`, `YuNet` and `CenterFace` detectors are wrapped in deepface.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/detector-portfolio-v6.jpg" width="95%" height="95%"></p>
 
 All deepface functions accept an optional detector backend input argument. You can switch among those detectors with this argument. OpenCV is the default detector.
 
 ```python
 backends = [
@@ -258,15 +260,15 @@
 )
 ```
 
 Face recognition models are actually CNN models and they expect standard sized inputs. So, resizing is required before representation. To avoid deformation, deepface adds black padding pixels according to the target size argument after detection and alignment.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/detector-outputs-20240414.jpg" width="90%" height="90%"></p>
 
-[RetinaFace](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/) and [MTCNN](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/) seem to overperform in detection and alignment stages but they are much slower. If the speed of your pipeline is more important, then you should use opencv or ssd. On the other hand, if you consider the accuracy, then you should use retinaface or mtcnn.
+[RetinaFace](https://sefiks.com/2021/04/27/deep-face-detection-with-retinaface-in-python/) and [MtCnn](https://sefiks.com/2020/09/09/deep-face-detection-with-mtcnn-in-python/) seem to overperform in detection and alignment stages but they are much slower. If the speed of your pipeline is more important, then you should use opencv or ssd. On the other hand, if you consider the accuracy, then you should use retinaface or mtcnn.
 
 The performance of RetinaFace is very satisfactory even in the crowd as seen in the following illustration. Besides, it comes with an incredible facial landmark detection performance. Highlighted red points show some facial landmarks such as eyes, nose and mouth. That's why, alignment score of RetinaFace is high as well.
 
 <p align="center"><img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/retinaface-results.jpeg" width="90%" height="90%">
 <br><em>The Yellow Angels - Fenerbahce Women's Volleyball Team</em>
 </p>
 
@@ -328,18 +330,14 @@
 
 #facial analysis
 $ deepface analyze -img_path tests/dataset/img1.jpg
 ```
 
 You can also run these commands if you are running deepface with docker. Please follow the instructions in the [shell script](https://github.com/serengil/deepface/blob/master/scripts/dockerize.sh#L17).
 
-## FAQ and Troubleshooting
-
-If you believe you have identified a bug or encountered a limitation in DeepFace that is not covered in the [existing issues](https://github.com/serengil/deepface/issues) or [closed issues](https://github.com/serengil/deepface/issues?q=is%3Aissue+is%3Aclosed), kindly open a new issue. Ensure that your submission includes clear and detailed reproduction steps, such as your Python version, your DeepFace version, versions of dependent packages (provided by pip freeze), specifics of any exception messages, details about how you are calling DeepFace, and the input image(s) you are using.
-
 ## Contribution
 
 Pull requests are more than welcome! If you are planning to contribute a large patch, please create an issue first to get any upfront questions or design decisions out of the way first.
 
 Before creating a PR, you should run the unit tests and linting locally by running `make test && make lint` command. Once a PR sent, GitHub test workflow will be run automatically and unit test and linting jobs will be available in [GitHub actions](https://github.com/serengil/deepface/actions) before approval.
 
 ## Support
@@ -352,30 +350,45 @@
 <img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/patreon.png" width="30%" height="30%">
 </a>
 
 ## Citation
 
 Please cite deepface in your publications if it helps your research - see [`CITATIONS`](https://github.com/serengil/deepface/blob/master/CITATION.md) for more details. Here are its BibTex entries:
 
-If you use deepface in your research for facial recogntion purposes, please cite this publication.
+If you use deepface in your research for facial recogntion purposes, please cite these publications:
+
+```BibTeX
+@article{serengil2024lightface,
+  title         = {A Benchmark of Facial Recognition Pipelines and Co-Usability Performances of Modules},
+  author        = {Serengil, Sefik Ilkin and Ozpinar, Alper},
+  journal       = {Bilisim Teknolojileri Dergisi},
+  volume        = {17},
+  number        = {2},
+  pages         = {95-107},
+  year          = {2024},
+  doi           = {10.17671/gazibtd.1399077},
+  url           = {https://dergipark.org.tr/en/pub/gazibtd/issue/84331/1399077},
+  publisher     = {Gazi University}
+}
+```
 
 ```BibTeX
 @inproceedings{serengil2020lightface,
   title        = {LightFace: A Hybrid Deep Face Recognition Framework},
   author       = {Serengil, Sefik Ilkin and Ozpinar, Alper},
   booktitle    = {2020 Innovations in Intelligent Systems and Applications Conference (ASYU)},
   pages        = {23-27},
   year         = {2020},
   doi          = {10.1109/ASYU50717.2020.9259802},
   url          = {https://ieeexplore.ieee.org/document/9259802},
   organization = {IEEE}
 }
 ```
 
-If you use deepface in your research for facial attribute analysis purposes such as age, gender, emotion or ethnicity prediction or face detection purposes, please cite this publication.
+If you use deepface in your research for facial attribute analysis purposes such as age, gender, emotion or ethnicity prediction, please cite this publication.
 
 ```BibTeX
 @inproceedings{serengil2021lightface,
   title        = {HyperExtended LightFace: A Facial Attribute Analysis Framework},
   author       = {Serengil, Sefik Ilkin and Ozpinar, Alper},
   booktitle    = {2021 International Conference on Engineering and Emerging Technologies (ICEET)},
   pages        = {1-4},
@@ -388,16 +401,13 @@
 
 Also, if you use deepface in your GitHub projects, please add `deepface` in the `requirements.txt`.
 
 ## Licence
 
 DeepFace is licensed under the MIT License - see [`LICENSE`](https://github.com/serengil/deepface/blob/master/LICENSE) for more details.
 
-DeepFace wraps some external face recognition models: [VGG-Face](http://www.robots.ox.ac.uk/~vgg/software/vgg_face/), [Facenet](https://github.com/davidsandberg/facenet/blob/master/LICENSE.md), [OpenFace](https://github.com/iwantooxxoox/Keras-OpenFace/blob/master/LICENSE), [DeepFace](https://github.com/swghosh/DeepFace), [DeepID](https://github.com/Ruoyiran/DeepID/blob/master/LICENSE.md), [ArcFace](https://github.com/leondgarse/Keras_insightface/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/dlib/LICENSE.txt), [SFace](https://github.com/opencv/opencv_zoo/blob/master/models/face_recognition_sface/LICENSE) and [GhostFaceNet](https://github.com/HamadYA/GhostFaceNets/blob/main/LICENSE). Besides, age, gender and race / ethnicity models were trained on the backbone of VGG-Face with transfer learning. 
-
-Similarly, DeepFace wraps many face detectors: [OpenCv](https://github.com/opencv/opencv/blob/4.x/LICENSE), [Ssd](https://github.com/opencv/opencv/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/LICENSE.txt), [MtCnn](https://github.com/ipazc/mtcnn/blob/master/LICENSE), [Fast MtCnn](https://github.com/timesler/facenet-pytorch/blob/master/LICENSE.md), [RetinaFace](https://github.com/serengil/retinaface/blob/master/LICENSE), [MediaPipe](https://github.com/google/mediapipe/blob/master/LICENSE), [YuNet](https://github.com/ShiqiYu/libfacedetection/blob/master/LICENSE), [Yolo](https://github.com/derronqi/yolov8-face/blob/main/LICENSE) and [CenterFace](https://github.com/Star-Clouds/CenterFace/blob/master/LICENSE).
+DeepFace wraps some external face recognition models: [VGG-Face](http://www.robots.ox.ac.uk/~vgg/software/vgg_face/), [Facenet](https://github.com/davidsandberg/facenet/blob/master/LICENSE.md), [OpenFace](https://github.com/iwantooxxoox/Keras-OpenFace/blob/master/LICENSE), [DeepFace](https://github.com/swghosh/DeepFace), [DeepID](https://github.com/Ruoyiran/DeepID/blob/master/LICENSE.md), [ArcFace](https://github.com/leondgarse/Keras_insightface/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/dlib/LICENSE.txt), [SFace](https://github.com/opencv/opencv_zoo/blob/master/models/face_recognition_sface/LICENSE) and [GhostFaceNet](https://github.com/HamadYA/GhostFaceNets/blob/main/LICENSE). Besides, age, gender and race / ethnicity models were trained on the backbone of VGG-Face with transfer learning. Similarly, DeepFace wraps many face detectors: [OpenCv](https://github.com/opencv/opencv/blob/4.x/LICENSE), [Ssd](https://github.com/opencv/opencv/blob/master/LICENSE), [Dlib](https://github.com/davisking/dlib/blob/master/LICENSE.txt), [MtCnn](https://github.com/ipazc/mtcnn/blob/master/LICENSE), [Fast MtCnn](https://github.com/timesler/facenet-pytorch/blob/master/LICENSE.md), [RetinaFace](https://github.com/serengil/retinaface/blob/master/LICENSE), [MediaPipe](https://github.com/google/mediapipe/blob/master/LICENSE), [YuNet](https://github.com/ShiqiYu/libfacedetection/blob/master/LICENSE), [Yolo](https://github.com/derronqi/yolov8-face/blob/main/LICENSE) and [CenterFace](https://github.com/Star-Clouds/CenterFace/blob/master/LICENSE). License types will be inherited when you intend to utilize those models. Please check the license types of those models for production purposes.
 
-Licence types will be inherited if you are going to use those models. Please check the license types of those models for production purposes.
 
 DeepFace [logo](https://thenounproject.com/term/face-recognition/2965879/) is created by [Adrien Coquet](https://thenounproject.com/coquet_adrien/) and it is licensed under [Creative Commons: By Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/).
```

### Comparing `deepface-0.0.90/deepface.egg-info/SOURCES.txt` & `deepface-0.0.91/deepface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepface-0.0.90/setup.py` & `deepface-0.0.91/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,9 +29,10 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": ["deepface = deepface.DeepFace:cli"],
     },
     python_requires=">=3.7",
+    license="MIT",
     install_requires=requirements,
 )
```

