# Comparing `tmp/qg_toolkit-1.0.18.tar.gz` & `tmp/qg_toolkit-1.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.18.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.19.tar", max compression
```

## Comparing `qg_toolkit-1.0.18.tar` & `qg_toolkit-1.0.19.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      854 2024-04-29 17:18:57.900555 qg_toolkit-1.0.18/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.18/qg_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/__init__.py
--rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
--rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
--rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
--rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
--rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
--rw-r--r--   0        0        0    37946 2024-04-29 17:00:55.850149 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
--rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
--rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
--rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
--rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
--rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
--rw-r--r--   0        0        0     2349 2024-04-27 11:14:05.254088 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
--rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
--rw-r--r--   0        0        0   101372 2024-04-29 17:00:55.853150 qg_toolkit-1.0.18/qg_toolkit/qgalxe/galxe.py
--rw-r--r--   0        0        0     2750 2024-04-29 17:00:55.851150 qg_toolkit-1.0.18/qg_toolkit/qgalxe/GeetestFullPageV4.py
--rw-r--r--   0        0        0     3795 2024-04-29 17:00:55.851150 qg_toolkit-1.0.18/qg_toolkit/qgalxe/GeetestSlideV4.py
--rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.18/qg_toolkit/qtweepy/__init__.py
--rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/__init__.py
--rw-r--r--   0        0        0     4912 2024-04-29 17:00:55.853150 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
--rw-r--r--   0        0        0       44 2024-04-29 17:00:55.854150 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
--rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.18/qg_toolkit/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.18/qg_toolkit/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0      279 2024-04-29 17:00:55.855149 qg_toolkit-1.0.18/qg_toolkit/test/demo.yaml
--rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.18/qg_toolkit/test/test.py
--rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.18/qg_toolkit/tools/__init__.py
--rw-r--r--   0        0        0     5391 2024-04-29 17:18:03.385731 qg_toolkit-1.0.18/qg_toolkit/tools/cui_qiu_client.py
--rw-r--r--   0        0        0     1245 2024-04-29 17:00:55.856150 qg_toolkit-1.0.18/qg_toolkit/tools/date_util.py
--rw-r--r--   0        0        0    12289 2024-04-29 17:00:55.857149 qg_toolkit-1.0.18/qg_toolkit/tools/discord.py
--rw-r--r--   0        0        0     5905 2024-04-29 05:37:22.967370 qg_toolkit-1.0.18/qg_toolkit/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.18/qg_toolkit/tools/qg_crypto.py
--rw-r--r--   0        0        0    36155 2024-04-29 17:00:55.858150 qg_toolkit-1.0.18/qg_toolkit/tools/qg_eth.py
--rw-r--r--   0        0        0     3641 2024-04-29 17:18:33.161050 qg_toolkit-1.0.18/qg_toolkit/tools/qg_file.py
--rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.18/qg_toolkit/tools/qg_models.py
--rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.18/qg_toolkit/tools/qg_random.py
--rw-r--r--   0        0        0     6168 2024-04-29 05:55:33.712699 qg_toolkit-1.0.18/qg_toolkit/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.18/qg_toolkit/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.18/qg_toolkit/tools/qproxy.py
--rw-r--r--   0        0        0     1239 2024-04-29 17:00:55.858150 qg_toolkit-1.0.18/qg_toolkit/tools/random_tool.py
--rw-r--r--   0        0        0     6068 2024-04-27 13:05:30.422039 qg_toolkit-1.0.18/qg_toolkit/tools/rpc.py
--rw-r--r--   0        0        0    72567 2024-04-29 17:16:01.332559 qg_toolkit-1.0.18/qg_toolkit/tools/twitter.py
--rw-r--r--   0        0        0     4182 2024-04-29 17:16:29.644862 qg_toolkit-1.0.18/qg_toolkit/tools/yescaptcha.py
--rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.18/README.md
--rw-r--r--   0        0        0      133 2024-04-29 17:18:57.893558 qg_toolkit-1.0.18/tea.yaml
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 qg_toolkit-1.0.18/PKG-INFO
+-rw-r--r--   0        0        0      854 2024-05-02 09:58:36.462299 qg_toolkit-1.0.19/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.19/qg_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
+-rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
+-rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
+-rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
+-rw-r--r--   0        0        0    37946 2024-04-29 17:00:55.850149 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
+-rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
+-rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
+-rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
+-rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
+-rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
+-rw-r--r--   0        0        0     2349 2024-04-27 11:14:05.254088 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
+-rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
+-rw-r--r--   0        0        0   101372 2024-04-29 17:00:55.853150 qg_toolkit-1.0.19/qg_toolkit/qgalxe/galxe.py
+-rw-r--r--   0        0        0     5383 2024-05-02 09:57:56.938543 qg_toolkit-1.0.19/qg_toolkit/qgalxe/GeetestFullPageV4.py
+-rw-r--r--   0        0        0     3795 2024-04-29 17:00:55.851150 qg_toolkit-1.0.19/qg_toolkit/qgalxe/GeetestSlideV4.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.19/qg_toolkit/qtweepy/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/__init__.py
+-rw-r--r--   0        0        0     4912 2024-04-29 17:00:55.853150 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       44 2024-04-29 17:00:55.854150 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.19/qg_toolkit/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.19/qg_toolkit/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0      279 2024-04-29 17:00:55.855149 qg_toolkit-1.0.19/qg_toolkit/test/demo.yaml
+-rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.19/qg_toolkit/test/test.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.19/qg_toolkit/tools/__init__.py
+-rw-r--r--   0        0        0     5391 2024-04-29 17:18:03.385731 qg_toolkit-1.0.19/qg_toolkit/tools/cui_qiu_client.py
+-rw-r--r--   0        0        0     1245 2024-04-29 17:00:55.856150 qg_toolkit-1.0.19/qg_toolkit/tools/date_util.py
+-rw-r--r--   0        0        0    12289 2024-04-29 17:00:55.857149 qg_toolkit-1.0.19/qg_toolkit/tools/discord.py
+-rw-r--r--   0        0        0     5905 2024-04-29 05:37:22.967370 qg_toolkit-1.0.19/qg_toolkit/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.19/qg_toolkit/tools/qg_crypto.py
+-rw-r--r--   0        0        0    36155 2024-04-29 17:00:55.858150 qg_toolkit-1.0.19/qg_toolkit/tools/qg_eth.py
+-rw-r--r--   0        0        0     3710 2024-05-02 09:57:56.939543 qg_toolkit-1.0.19/qg_toolkit/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.19/qg_toolkit/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.19/qg_toolkit/tools/qg_random.py
+-rw-r--r--   0        0        0     6168 2024-04-29 05:55:33.712699 qg_toolkit-1.0.19/qg_toolkit/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.19/qg_toolkit/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.19/qg_toolkit/tools/qproxy.py
+-rw-r--r--   0        0        0     1239 2024-04-29 17:00:55.858150 qg_toolkit-1.0.19/qg_toolkit/tools/random_tool.py
+-rw-r--r--   0        0        0     6113 2024-05-02 06:59:59.061718 qg_toolkit-1.0.19/qg_toolkit/tools/rpc.py
+-rw-r--r--   0        0        0    72567 2024-04-29 17:16:01.332559 qg_toolkit-1.0.19/qg_toolkit/tools/twitter.py
+-rw-r--r--   0        0        0     4182 2024-04-29 17:16:29.644862 qg_toolkit-1.0.19/qg_toolkit/tools/yescaptcha.py
+-rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.19/README.md
+-rw-r--r--   0        0        0      133 2024-05-02 09:59:11.389046 qg_toolkit-1.0.19/tea.yaml
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 qg_toolkit-1.0.19/PKG-INFO
```

### Comparing `qg_toolkit-1.0.18/pyproject.toml` & `qg_toolkit-1.0.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.18"
+version = "1.0.19"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qg_toolkit"}]
 include = [{path = "tea.yaml"}]
```

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/gap.py` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/gap.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/mian.py` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/trace.py` & `qg_toolkit-1.0.19/qg_toolkit/geetest_captcha/geetest4_slide/trace.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qgalxe/galxe.py` & `qg_toolkit-1.0.19/qg_toolkit/qgalxe/galxe.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qgalxe/GeetestSlideV4.py` & `qg_toolkit-1.0.19/qg_toolkit/qgalxe/GeetestSlideV4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/account_checker.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/follow_each_other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/mavia.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/set_2fa.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/uploading_images.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/voter.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/voter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/xai.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/examples/xai.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/pyproject.toml` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/README.md` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/account.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/client.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/models.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.19/qg_toolkit/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/cui_qiu_client.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/cui_qiu_client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/date_util.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/date_util.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/discord.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/discord.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/qg_airdrop.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/qg_airdrop.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/qg_crypto.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/qg_eth.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/qg_eth.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/qg_file.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/qg_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,25 @@
 
     @staticmethod
     def read_yaml(file_path):
         with open(file_path, 'r') as file:
             return yaml.safe_load(file)
 
     @staticmethod
-    def url_params_to_object(url):
+    def url_params_to_object(url, key=None):
         # 解析URL
         parsed_url = urlparse(url)
         # 获取查询字符串参数并转换为字典对象
         query_params = parse_qs(parsed_url.query)
         # 处理字典对象，将每个参数的值转换为单个值而不是数组
         for key, value in query_params.items():
             query_params[key] = value[0]
         # 返回转换后的字典对象
+        if key:
+            return query_params.get(key)
         return query_params
 
     @staticmethod
     def csv_to_array(file_path, has_header=True, delimiter=','):
         """解汇csv文件，返回数组对象"""
         with open(file_path, 'r') as f:
             reader = csv.reader(f, delimiter=delimiter)
```

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/qg_random.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/qg_solana.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/qg_solana.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/qg_starknet.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/qproxy.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/random_tool.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/random_tool.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/rpc.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,16 @@
     # "avav": "https://rpc.ankr.com/avalanche",
     "avav": "https://avalanche.drpc.org",
     # "avav": "https://avax-pokt.nodies.app/ext/bc/C/rpc",
     "berachain": "https://artio.rpc.berachain.com",
     "kly": "https://public-en-cypress.klaytn.net",
     "blast": "https://sepolia.blast.io",
     "holesky": "https://ethereum-holesky.publicnode.com",
-    "katla": "https://rpc.katla.taiko.xyz"
+    "katla": "https://rpc.katla.taiko.xyz",
+    "hekla": "https://rpc.hekla.taiko.xyz"
 }
 # api接口
 bases = {
     "goerli": "https://api-goerli.etherscan.io/api",
     # "goerli": "https://eth-goerli.blockscout.com/api",
     "sepolia": "https://api-sepolia.etherscan.io/api",
     # "linea": "https://explorer.goerli.linea.build/api",
```

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/twitter.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/twitter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/qg_toolkit/tools/yescaptcha.py` & `qg_toolkit-1.0.19/qg_toolkit/tools/yescaptcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.18/PKG-INFO` & `qg_toolkit-1.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.18
+Version: 1.0.19
 Summary: qg_toolkit for Python!
 Author: qg
 Author-email: qg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

