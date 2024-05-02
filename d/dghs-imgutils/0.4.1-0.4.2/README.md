# Comparing `tmp/dghs-imgutils-0.4.1.tar.gz` & `tmp/dghs_imgutils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs-imgutils-0.4.1.tar", last modified: Wed Mar 20 09:03:22 2024, max compression
+gzip compressed data, was "dghs_imgutils-0.4.2.tar", last modified: Thu May  2 15:51:45 2024, max compression
```

## Comparing `dghs-imgutils-0.4.1.tar` & `dghs_imgutils-0.4.2.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.612613 dghs-imgutils-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-20 09:02:36.000000 dghs-imgutils-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-20 09:02:36.000000 dghs-imgutils-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19054 2024-03-20 09:03:22.612613 dghs-imgutils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-03-20 09:02:36.000000 dghs-imgutils-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.608613 dghs-imgutils-0.4.1/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19054 2024-03-20 09:03:22.000000 dghs-imgutils-0.4.1/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-20 09:03:22.000000 dghs-imgutils-0.4.1/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 09:03:22.000000 dghs-imgutils-0.4.1/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-20 09:03:22.000000 dghs-imgutils-0.4.1/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 09:03:22.000000 dghs-imgutils-0.4.1/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.596613 dghs-imgutils-0.4.1/imgutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.596613 dghs-imgutils-0.4.1/imgutils/ascii/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/ascii/drawing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.596613 dghs-imgutils-0.4.1/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.600612 dghs-imgutils-0.4.1/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.600612 dghs-imgutils-0.4.1/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/censor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/eye.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/halfbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/hand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.600612 dghs-imgutils-0.4.1/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.600612 dghs-imgutils-0.4.1/imgutils/generic/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/generic/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.600612 dghs-imgutils-0.4.1/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/metrics/aesthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21967 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/metrics/ccip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.600612 dghs-imgutils-0.4.1/imgutils/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/ocr/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/ocr/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/ocr/recognize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.604612 dghs-imgutils-0.4.1/imgutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/operate/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/operate/censor_.py
--rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/operate/emoji_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)    83886 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/operate/heart_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/operate/imgcensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    74310 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/operate/smile_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/operate/squeeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.604612 dghs-imgutils-0.4.1/imgutils/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/pose/dwpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/pose/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/pose/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.604612 dghs-imgutils-0.4.1/imgutils/restore/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/restore/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/restore/nafnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/restore/scunet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.604612 dghs-imgutils-0.4.1/imgutils/sd/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/sd/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/sd/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.604612 dghs-imgutils-0.4.1/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.604612 dghs-imgutils-0.4.1/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.604612 dghs-imgutils-0.4.1/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/utils/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/utils/onnxruntime.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/utils/tqdm_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:03:22.608613 dghs-imgutils-0.4.1/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/aicheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/bangumi_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/completeness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/nsfw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/portrait.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/real.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/style_age.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/teen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/requirements-model.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 09:03:22.612613 dghs-imgutils-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-03-20 09:02:37.000000 dghs-imgutils-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.806495 dghs_imgutils-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 15:50:56.000000 dghs_imgutils-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 15:50:56.000000 dghs_imgutils-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19054 2024-05-02 15:51:45.806495 dghs_imgutils-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-02 15:50:56.000000 dghs_imgutils-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.798495 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19054 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 15:51:45.000000 dghs_imgutils-0.4.2/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ascii/drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/censor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/halfbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/hand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.790495 dghs_imgutils-0.4.2/imgutils/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/generic/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21967 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/ccip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/dbaesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ocr/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ocr/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/ocr/recognize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/censor_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/emoji_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83886 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/heart_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/imgcensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74310 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/smile_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/operate/squeeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/pose/dwpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/pose/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/pose/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/restore/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/restore/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/restore/nafnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/restore/scunet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/sd/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/sd/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.794495 dghs_imgutils-0.4.2/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.798495 dghs_imgutils-0.4.2/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.798495 dghs_imgutils-0.4.2/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/utils/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/utils/onnxruntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/utils/tqdm_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:51:45.798495 dghs_imgutils-0.4.2/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/aicheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/bangumi_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/dbrating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/nsfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/portrait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/style_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/teen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-model.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:51:45.806495 dghs_imgutils-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-02 15:50:58.000000 dghs_imgutils-0.4.2/setup.py
```

### Comparing `dghs-imgutils-0.4.1/LICENSE` & `dghs_imgutils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/PKG-INFO` & `dghs_imgutils-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.4.1
+Version: 0.4.2
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d7
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,17 +31,14 @@
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: emoji>=2.5.0
 Requires-Dist: pilmoji>=1.3.0
 Requires-Dist: shapely
 Requires-Dist: pyclipper
 Requires-Dist: deprecation>=2.0.0
-Provides-Extra: model
-Requires-Dist: torch; extra == "model"
-Requires-Dist: safetensors; extra == "model"
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
 Requires-Dist: pytest~=6.2.5; extra == "test"
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
@@ -52,14 +49,17 @@
 Requires-Dist: pytest-benchmark~=3.4.0; extra == "test"
 Requires-Dist: easydict<2,>=1.7; extra == "test"
 Requires-Dist: testtools>=2; extra == "test"
 Requires-Dist: where>=1.0.2; extra == "test"
 Requires-Dist: pytest-image-diff>=0.0.11; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: natsort; extra == "test"
+Provides-Extra: model
+Requires-Dist: torch; extra == "model"
+Requires-Dist: safetensors; extra == "model"
 Provides-Extra: doc
 Requires-Dist: Jinja2~=3.0.0; extra == "doc"
 Requires-Dist: sphinx>=3.2.0; extra == "doc"
 Requires-Dist: sphinx_rtd_theme>=0.4.3; extra == "doc"
 Requires-Dist: enum_tools~=0.9.0; extra == "doc"
 Requires-Dist: sphinx-toolbox; extra == "doc"
 Requires-Dist: plantumlcli>=0.0.2; extra == "doc"
```

### Comparing `dghs-imgutils-0.4.1/README.md` & `dghs_imgutils-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/dghs_imgutils.egg-info/PKG-INFO` & `dghs_imgutils-0.4.2/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.4.1
+Version: 0.4.2
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d7
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,17 +31,14 @@
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: emoji>=2.5.0
 Requires-Dist: pilmoji>=1.3.0
 Requires-Dist: shapely
 Requires-Dist: pyclipper
 Requires-Dist: deprecation>=2.0.0
-Provides-Extra: model
-Requires-Dist: torch; extra == "model"
-Requires-Dist: safetensors; extra == "model"
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
 Requires-Dist: pytest~=6.2.5; extra == "test"
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
@@ -52,14 +49,17 @@
 Requires-Dist: pytest-benchmark~=3.4.0; extra == "test"
 Requires-Dist: easydict<2,>=1.7; extra == "test"
 Requires-Dist: testtools>=2; extra == "test"
 Requires-Dist: where>=1.0.2; extra == "test"
 Requires-Dist: pytest-image-diff>=0.0.11; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: natsort; extra == "test"
+Provides-Extra: model
+Requires-Dist: torch; extra == "model"
+Requires-Dist: safetensors; extra == "model"
 Provides-Extra: doc
 Requires-Dist: Jinja2~=3.0.0; extra == "doc"
 Requires-Dist: sphinx>=3.2.0; extra == "doc"
 Requires-Dist: sphinx_rtd_theme>=0.4.3; extra == "doc"
 Requires-Dist: enum_tools~=0.9.0; extra == "doc"
 Requires-Dist: sphinx-toolbox; extra == "doc"
 Requires-Dist: plantumlcli>=0.0.2; extra == "doc"
```

### Comparing `dghs-imgutils-0.4.1/dghs_imgutils.egg-info/SOURCES.txt` & `dghs_imgutils-0.4.2/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 imgutils/edge/lineart.py
 imgutils/edge/lineart_anime.py
 imgutils/generic/__init__.py
 imgutils/generic/classify.py
 imgutils/metrics/__init__.py
 imgutils/metrics/aesthetic.py
 imgutils/metrics/ccip.py
+imgutils/metrics/dbaesthetic.py
 imgutils/metrics/lpips.py
 imgutils/metrics/psnr_.py
 imgutils/ocr/__init__.py
 imgutils/ocr/detect.py
 imgutils/ocr/entry.py
 imgutils/ocr/recognize.py
 imgutils/operate/__init__.py
@@ -88,14 +89,15 @@
 imgutils/utils/tqdm_.py
 imgutils/validate/__init__.py
 imgutils/validate/aicheck.py
 imgutils/validate/bangumi_char.py
 imgutils/validate/classify.py
 imgutils/validate/color.py
 imgutils/validate/completeness.py
+imgutils/validate/dbrating.py
 imgutils/validate/monochrome.py
 imgutils/validate/nsfw.py
 imgutils/validate/portrait.py
 imgutils/validate/rating.py
 imgutils/validate/real.py
 imgutils/validate/safe.py
 imgutils/validate/style_age.py
```

### Comparing `dghs-imgutils-0.4.1/dghs_imgutils.egg-info/requires.txt` & `dghs_imgutils-0.4.2/dghs_imgutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/ascii/drawing.py` & `dghs_imgutils-0.4.2/imgutils/ascii/drawing.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/config/meta.py` & `dghs_imgutils-0.4.2/imgutils/config/meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.4.1'
+__VERSION__ = '0.4.2'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992, 7eu7d7'
```

### Comparing `dghs-imgutils-0.4.1/imgutils/data/background.py` & `dghs_imgutils-0.4.2/imgutils/data/background.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/data/decode.py` & `dghs_imgutils-0.4.2/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/data/encode.py` & `dghs_imgutils-0.4.2/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/data/image.py` & `dghs_imgutils-0.4.2/imgutils/data/image.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/data/layer.py` & `dghs_imgutils-0.4.2/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/__init__.py` & `dghs_imgutils-0.4.2/imgutils/detect/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/_yolo.py` & `dghs_imgutils-0.4.2/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/censor.py` & `dghs_imgutils-0.4.2/imgutils/detect/censor.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/eye.py` & `dghs_imgutils-0.4.2/imgutils/detect/eye.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/face.py` & `dghs_imgutils-0.4.2/imgutils/detect/face.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/halfbody.py` & `dghs_imgutils-0.4.2/imgutils/detect/halfbody.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/hand.py` & `dghs_imgutils-0.4.2/imgutils/detect/hand.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/head.py` & `dghs_imgutils-0.4.2/imgutils/detect/head.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/person.py` & `dghs_imgutils-0.4.2/imgutils/detect/person.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/text.py` & `dghs_imgutils-0.4.2/imgutils/detect/text.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/detect/visual.py` & `dghs_imgutils-0.4.2/imgutils/detect/visual.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/edge/__init__.py` & `dghs_imgutils-0.4.2/imgutils/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/edge/_base.py` & `dghs_imgutils-0.4.2/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/edge/canny.py` & `dghs_imgutils-0.4.2/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/edge/lineart.py` & `dghs_imgutils-0.4.2/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/edge/lineart_anime.py` & `dghs_imgutils-0.4.2/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/generic/classify.py` & `dghs_imgutils-0.4.2/imgutils/generic/classify.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/metrics/aesthetic.py` & `dghs_imgutils-0.4.2/imgutils/metrics/aesthetic.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,22 +6,28 @@
     .. image:: aesthetic_full.plot.py.svg
         :align: center
 
     This is an overall benchmark of all the operations in aesthetic models:
 
     .. image:: aesthetic_benchmark.plot.py.svg
         :align: center
+
+    .. warning::
+        These model is deprecated due to the poor effectiveness.
+        Please use `imgutils.metrics.aesthetic.anime_dbaesthetic` for better evaluation.
 """
 from functools import lru_cache
 
 import cv2
 import numpy as np
 from PIL import Image
+from deprecation import deprecated
 from huggingface_hub import hf_hub_download
 
+from ..config.meta import __VERSION__
 from ..data import ImageTyping, load_image
 from ..utils import open_onnx_model
 
 __all__ = [
     'get_aesthetic_score',
 ]
 
@@ -43,14 +49,16 @@
     ph, pw = s - h, s - w
     img_input = np.zeros([s, s, 3], dtype=np.float32)
     img_input[ph // 2:ph // 2 + h, pw // 2:pw // 2 + w] = cv2.resize(img, (w, h))
     img_input = np.transpose(img_input, (2, 0, 1))
     return img_input[np.newaxis, :]
 
 
+@deprecated(deprecated_in='0.4.2', removed_in='1.0.0', current_version=__VERSION__,
+            details='Deprecated due to the low effectiveness.')
 def get_aesthetic_score(image: ImageTyping):
     """
     Overview:
         Get aesthetic score for image.
 
     :param image: Original image.
     :return: Score of aesthetic.
```

### Comparing `dghs-imgutils-0.4.1/imgutils/metrics/ccip.py` & `dghs_imgutils-0.4.2/imgutils/metrics/ccip.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/metrics/lpips.py` & `dghs_imgutils-0.4.2/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/metrics/psnr_.py` & `dghs_imgutils-0.4.2/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/ocr/__init__.py` & `dghs_imgutils-0.4.2/imgutils/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/ocr/detect.py` & `dghs_imgutils-0.4.2/imgutils/ocr/detect.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/ocr/entry.py` & `dghs_imgutils-0.4.2/imgutils/ocr/entry.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/ocr/recognize.py` & `dghs_imgutils-0.4.2/imgutils/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/operate/align.py` & `dghs_imgutils-0.4.2/imgutils/operate/align.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/operate/censor_.py` & `dghs_imgutils-0.4.2/imgutils/operate/censor_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/operate/emoji_censor.png` & `dghs_imgutils-0.4.2/imgutils/operate/emoji_censor.png`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/operate/heart_censor.png` & `dghs_imgutils-0.4.2/imgutils/operate/heart_censor.png`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/operate/imgcensor.py` & `dghs_imgutils-0.4.2/imgutils/operate/imgcensor.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/operate/smile_censor.png` & `dghs_imgutils-0.4.2/imgutils/operate/smile_censor.png`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/operate/squeeze.py` & `dghs_imgutils-0.4.2/imgutils/operate/squeeze.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/pose/dwpose.py` & `dghs_imgutils-0.4.2/imgutils/pose/dwpose.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/pose/format.py` & `dghs_imgutils-0.4.2/imgutils/pose/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/pose/visual.py` & `dghs_imgutils-0.4.2/imgutils/pose/visual.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/restore/adversarial.py` & `dghs_imgutils-0.4.2/imgutils/restore/adversarial.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/restore/nafnet.py` & `dghs_imgutils-0.4.2/imgutils/restore/nafnet.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/restore/scunet.py` & `dghs_imgutils-0.4.2/imgutils/restore/scunet.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/sd/metadata.py` & `dghs_imgutils-0.4.2/imgutils/sd/metadata.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/sd/model.py` & `dghs_imgutils-0.4.2/imgutils/sd/model.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/segment/isnetis.py` & `dghs_imgutils-0.4.2/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/__init__.py` & `dghs_imgutils-0.4.2/imgutils/tagging/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/blacklist.py` & `dghs_imgutils-0.4.2/imgutils/tagging/blacklist.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/character.py` & `dghs_imgutils-0.4.2/imgutils/tagging/character.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/deepdanbooru.py` & `dghs_imgutils-0.4.2/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/format.py` & `dghs_imgutils-0.4.2/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/match.py` & `dghs_imgutils-0.4.2/imgutils/tagging/match.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/mldanbooru.py` & `dghs_imgutils-0.4.2/imgutils/tagging/mldanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/order.py` & `dghs_imgutils-0.4.2/imgutils/tagging/order.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/overlap.py` & `dghs_imgutils-0.4.2/imgutils/tagging/overlap.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/tagging/wd14.py` & `dghs_imgutils-0.4.2/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/utils/area.py` & `dghs_imgutils-0.4.2/imgutils/utils/area.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/utils/onnxruntime.py` & `dghs_imgutils-0.4.2/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/utils/tqdm_.py` & `dghs_imgutils-0.4.2/imgutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/aicheck.py` & `dghs_imgutils-0.4.2/imgutils/validate/aicheck.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/bangumi_char.py` & `dghs_imgutils-0.4.2/imgutils/validate/bangumi_char.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/classify.py` & `dghs_imgutils-0.4.2/imgutils/validate/classify.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/color.py` & `dghs_imgutils-0.4.2/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/completeness.py` & `dghs_imgutils-0.4.2/imgutils/validate/completeness.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/monochrome.py` & `dghs_imgutils-0.4.2/imgutils/validate/monochrome.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/nsfw.py` & `dghs_imgutils-0.4.2/imgutils/validate/nsfw.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/portrait.py` & `dghs_imgutils-0.4.2/imgutils/validate/portrait.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/rating.py` & `dghs_imgutils-0.4.2/imgutils/validate/rating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Overview:
-    A model for rating anime images into 4 classes (``safe``, ``r15`` and ``r18``).
+    A model for rating anime images into 3 classes (``safe``, ``r15`` and ``r18``), based on sankaku rating system.
 
     The following are sample images for testing.
 
     .. collapse:: The following are sample images for testing. (WARNING: NSFW!!!)
 
         .. image:: rating.plot.py.svg
             :align: center
```

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/real.py` & `dghs_imgutils-0.4.2/imgutils/validate/real.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/safe.py` & `dghs_imgutils-0.4.2/imgutils/validate/safe.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/style_age.py` & `dghs_imgutils-0.4.2/imgutils/validate/style_age.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/teen.py` & `dghs_imgutils-0.4.2/imgutils/validate/teen.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/imgutils/validate/truncate.py` & `dghs_imgutils-0.4.2/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.4.1/setup.py` & `dghs_imgutils-0.4.2/setup.py`

 * *Files identical despite different names*

