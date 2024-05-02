# Comparing `tmp/ngclearn-1.0b3.tar.gz` & `tmp/ngclearn-1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngclearn-1.0b3.tar", last modified: Sun Apr 14 20:41:22 2024, max compression
+gzip compressed data, was "ngclearn-1.0b4.tar", last modified: Thu May  2 19:09:59 2024, max compression
```

## Comparing `ngclearn-1.0b3.tar` & `ngclearn-1.0b4.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.783771 ngclearn-1.0b3/
--rw-rw-r--   0 ago       (1001) ago       (1001)      368 2024-03-27 21:42:18.000000 ngclearn-1.0b3/AUTHORS
--rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-03-27 21:42:18.000000 ngclearn-1.0b3/LICENSE
--rw-r--r--   0 ago       (1001) ago       (1001)     8238 2024-04-14 20:41:22.783771 ngclearn-1.0b3/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     6514 2024-04-14 20:41:04.000000 ngclearn-1.0b3/README.md
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.775771 ngclearn-1.0b3/ngclearn/
--rw-rw-r--   0 ago       (1001) ago       (1001)      706 2024-03-29 23:12:24.000000 ngclearn-1.0b3/ngclearn/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.775771 ngclearn-1.0b3/ngclearn/commands/
--rw-rw-r--   0 ago       (1001) ago       (1001)       33 2024-03-28 23:58:59.000000 ngclearn-1.0b3/ngclearn/commands/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.775771 ngclearn-1.0b3/ngclearn/components/
--rw-rw-r--   0 ago       (1001) ago       (1001)     1087 2024-04-04 05:00:32.000000 ngclearn-1.0b3/ngclearn/components/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1081 2024-03-28 22:29:48.000000 ngclearn-1.0b3/ngclearn/components/baseComponentTemplate.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/input_encoders/
--rw-rw-r--   0 ago       (1001) ago       (1001)      118 2024-03-30 04:48:51.000000 ngclearn-1.0b3/ngclearn/components/input_encoders/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3576 2024-03-30 04:48:51.000000 ngclearn-1.0b3/ngclearn/components/input_encoders/bernoulliCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     8904 2024-04-01 16:58:48.000000 ngclearn-1.0b3/ngclearn/components/input_encoders/latencyCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3933 2024-03-30 20:38:16.000000 ngclearn-1.0b3/ngclearn/components/input_encoders/poissonCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/neurons/
--rw-rw-r--   0 ago       (1001) ago       (1001)      486 2024-04-01 02:25:22.000000 ngclearn-1.0b3/ngclearn/components/neurons/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/neurons/graded/
--rw-rw-r--   0 ago       (1001) ago       (1001)      178 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/components/neurons/graded/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5403 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/neurons/graded/gaussianErrorCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5439 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/neurons/graded/laplacianErrorCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9968 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/neurons/graded/rateCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/neurons/spiking/
--rw-rw-r--   0 ago       (1001) ago       (1001)    11036 2024-03-28 22:31:05.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/LIFCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      247 2024-04-01 02:25:22.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     8887 2024-04-07 17:56:32.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)    11228 2024-04-06 18:49:10.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/izhikevichCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    11707 2024-03-28 22:31:11.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/quadLIFCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    14148 2024-04-13 21:17:29.000000 ngclearn-1.0b3/ngclearn/components/neurons/spiking/sLIFCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/other/
--rw-rw-r--   0 ago       (1001) ago       (1001)       64 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/components/other/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     4379 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/other/expKernel.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     5084 2024-04-09 02:58:27.000000 ngclearn-1.0b3/ngclearn/components/other/varTrace.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/synapses/
--rw-rw-r--   0 ago       (1001) ago       (1001)      160 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/components/synapses/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     8378 2024-03-28 22:31:56.000000 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/expSTDPSynapse.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    10875 2024-04-13 20:58:40.000000 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/hebbianSynapse.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9793 2024-04-09 23:34:39.000000 ngclearn-1.0b3/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      263 2024-03-29 00:03:17.000000 ngclearn-1.0b3/ngclearn/components/wrappers.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/
--rwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/__init__.py
--rw-r--r--   0 ago       (1001) ago       (1001)     3232 2024-04-05 17:47:38.000000 ngclearn-1.0b3/ngclearn/utils/data_loader.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/density/
--rw-r--r--   0 ago       (1001) ago       (1001)        0 2024-03-28 00:06:24.000000 ngclearn-1.0b3/ngclearn/utils/density/__init__.py
--rw-r--r--   0 ago       (1001) ago       (1001)     2816 2024-03-28 02:06:50.000000 ngclearn-1.0b3/ngclearn/utils/density/gmm.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/diffeq/
--rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-04-06 17:34:24.000000 ngclearn-1.0b3/ngclearn/utils/diffeq/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5253 2024-04-06 22:55:59.000000 ngclearn-1.0b3/ngclearn/utils/diffeq/ode_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     1629 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/io_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5470 2024-04-12 02:40:59.000000 ngclearn-1.0b3/ngclearn/utils/metric_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)    18320 2024-04-12 15:57:53.000000 ngclearn-1.0b3/ngclearn/utils/model_utils.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/optim/
--rw-rw-r--   0 ago       (1001) ago       (1001)       46 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/optim/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3090 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/optim/adam.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)      783 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/optim/opt.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     1122 2024-04-05 17:34:57.000000 ngclearn-1.0b3/ngclearn/utils/optim/sgd.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3164 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/patch_utils.py
--rw-r--r--   0 ago       (1001) ago       (1001)     3809 2024-04-12 16:30:37.000000 ngclearn-1.0b3/ngclearn/utils/surrogate_fx.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn/utils/viz/
--rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b3/ngclearn/utils/viz/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3382 2024-04-08 02:28:58.000000 ngclearn-1.0b3/ngclearn/utils/viz/dim_reduce.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     6699 2024-04-03 17:27:35.000000 ngclearn-1.0b3/ngclearn/utils/viz/raster.py
--rw-r--r--   0 ago       (1001) ago       (1001)     2513 2024-04-03 17:26:57.000000 ngclearn-1.0b3/ngclearn/utils/viz/spike_plot.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     4922 2024-03-30 16:17:15.000000 ngclearn-1.0b3/ngclearn/utils/viz/synapse_plot.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-04-14 20:41:22.779771 ngclearn-1.0b3/ngclearn.egg-info/
--rw-r--r--   0 ago       (1001) ago       (1001)     8238 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     2119 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/SOURCES.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/dependency_links.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/requires.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       28 2024-04-14 20:41:22.000000 ngclearn-1.0b3/ngclearn.egg-info/top_level.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)     1838 2024-04-14 20:40:42.000000 ngclearn-1.0b3/pyproject.toml
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-30 18:06:06.000000 ngclearn-1.0b3/requirements.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-04-14 20:41:22.783771 ngclearn-1.0b3/setup.cfg
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.754975 ngclearn-1.0b4/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      368 2024-03-27 21:42:18.000000 ngclearn-1.0b4/AUTHORS
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-03-27 21:42:18.000000 ngclearn-1.0b4/LICENSE
+-rw-r--r--   0 ago       (1001) ago       (1001)     7754 2024-05-02 19:09:59.754975 ngclearn-1.0b4/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6030 2024-05-02 19:09:14.000000 ngclearn-1.0b4/README.md
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.658976 ngclearn-1.0b4/UPDATED_cells/
+-rw-r--r--   0 ago       (1001) ago       (1001)    13935 2024-04-23 19:01:05.000000 ngclearn-1.0b4/UPDATED_cells/LIFCell.py
+-rw-r--r--   0 ago       (1001) ago       (1001)    14887 2024-04-22 01:12:58.000000 ngclearn-1.0b4/UPDATED_cells/older_sLIF.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.670976 ngclearn-1.0b4/ngclearn/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      706 2024-05-02 19:09:05.000000 ngclearn-1.0b4/ngclearn/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.674976 ngclearn-1.0b4/ngclearn/commands/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       33 2024-03-28 23:58:59.000000 ngclearn-1.0b4/ngclearn/commands/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.674976 ngclearn-1.0b4/ngclearn/components/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1087 2024-04-04 05:00:32.000000 ngclearn-1.0b4/ngclearn/components/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1081 2024-03-28 22:29:48.000000 ngclearn-1.0b4/ngclearn/components/baseComponentTemplate.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.674976 ngclearn-1.0b4/ngclearn/components/input_encoders/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      118 2024-03-30 04:48:51.000000 ngclearn-1.0b4/ngclearn/components/input_encoders/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3568 2024-04-17 19:56:59.000000 ngclearn-1.0b4/ngclearn/components/input_encoders/bernoulliCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     8904 2024-04-01 16:58:48.000000 ngclearn-1.0b4/ngclearn/components/input_encoders/latencyCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3933 2024-03-30 20:38:16.000000 ngclearn-1.0b4/ngclearn/components/input_encoders/poissonCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.674976 ngclearn-1.0b4/ngclearn/components/neurons/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      486 2024-04-01 02:25:22.000000 ngclearn-1.0b4/ngclearn/components/neurons/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.678976 ngclearn-1.0b4/ngclearn/components/neurons/graded/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      178 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/components/neurons/graded/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5403 2024-04-15 21:14:40.000000 ngclearn-1.0b4/ngclearn/components/neurons/graded/gaussianErrorCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5439 2024-04-09 02:58:27.000000 ngclearn-1.0b4/ngclearn/components/neurons/graded/laplacianErrorCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9985 2024-04-25 16:59:38.000000 ngclearn-1.0b4/ngclearn/components/neurons/graded/rateCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.690976 ngclearn-1.0b4/ngclearn/components/neurons/spiking/
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11036 2024-03-28 22:31:05.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/LIFCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      247 2024-04-01 02:25:22.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9077 2024-04-23 18:48:03.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    11418 2024-04-23 18:48:14.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/izhikevichCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11707 2024-03-28 22:31:11.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/quadLIFCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    15059 2024-04-27 16:21:39.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/sLIFCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.694975 ngclearn-1.0b4/ngclearn/components/other/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       64 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/components/other/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     4379 2024-04-09 02:58:27.000000 ngclearn-1.0b4/ngclearn/components/other/expKernel.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     5084 2024-04-15 21:33:31.000000 ngclearn-1.0b4/ngclearn/components/other/varTrace.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.694975 ngclearn-1.0b4/ngclearn/components/synapses/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      160 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/components/synapses/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.698975 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     8378 2024-03-28 22:31:56.000000 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/expSTDPSynapse.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11195 2024-04-18 22:52:48.000000 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/hebbianSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9793 2024-04-09 23:34:39.000000 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      263 2024-03-29 00:03:17.000000 ngclearn-1.0b4/ngclearn/components/wrappers.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.698975 ngclearn-1.0b4/ngclearn/utils/
+-rwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/__init__.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     3232 2024-04-05 17:47:38.000000 ngclearn-1.0b4/ngclearn/utils/data_loader.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.702975 ngclearn-1.0b4/ngclearn/utils/density/
+-rw-r--r--   0 ago       (1001) ago       (1001)        0 2024-03-28 00:06:24.000000 ngclearn-1.0b4/ngclearn/utils/density/__init__.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     2816 2024-03-28 02:06:50.000000 ngclearn-1.0b4/ngclearn/utils/density/gmm.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.726975 ngclearn-1.0b4/ngclearn/utils/diffeq/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-04-06 17:34:24.000000 ngclearn-1.0b4/ngclearn/utils/diffeq/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     6043 2024-04-23 18:35:18.000000 ngclearn-1.0b4/ngclearn/utils/diffeq/_ode_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     6586 2024-04-23 18:39:06.000000 ngclearn-1.0b4/ngclearn/utils/diffeq/ode_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     1629 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/io_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5638 2024-04-27 19:34:14.000000 ngclearn-1.0b4/ngclearn/utils/metric_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    19071 2024-04-27 19:34:14.000000 ngclearn-1.0b4/ngclearn/utils/model_utils.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.754975 ngclearn-1.0b4/ngclearn/utils/optim/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       46 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/optim/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3090 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/optim/adam.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)      783 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/optim/opt.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     1122 2024-04-05 17:34:57.000000 ngclearn-1.0b4/ngclearn/utils/optim/sgd.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3164 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/patch_utils.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     5690 2024-04-17 20:19:32.000000 ngclearn-1.0b4/ngclearn/utils/surrogate_fx.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.754975 ngclearn-1.0b4/ngclearn/utils/viz/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/viz/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3503 2024-05-01 23:29:33.000000 ngclearn-1.0b4/ngclearn/utils/viz/dim_reduce.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     6699 2024-04-03 17:27:35.000000 ngclearn-1.0b4/ngclearn/utils/viz/raster.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     2513 2024-04-03 17:26:57.000000 ngclearn-1.0b4/ngclearn/utils/viz/spike_plot.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     4936 2024-04-19 16:42:21.000000 ngclearn-1.0b4/ngclearn/utils/viz/synapse_plot.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.754975 ngclearn-1.0b4/ngclearn.egg-info/
+-rw-r--r--   0 ago       (1001) ago       (1001)     7754 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2208 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/requires.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       67 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/top_level.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1838 2024-05-02 19:08:29.000000 ngclearn-1.0b4/pyproject.toml
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-02 19:09:51.000000 ngclearn-1.0b4/requirements.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-05-02 19:09:59.754975 ngclearn-1.0b4/setup.cfg
```

### Comparing `ngclearn-1.0b3/LICENSE` & `ngclearn-1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/PKG-INFO` & `ngclearn-1.0b4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngclearn
-Version: 1.0b3
+Version: 1.0b4
 Summary: Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems.
 Author-email: Alexander Ororbia <ago@cs.rit.edu>, William Gebhardt <wdg1351@rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-learn
 Project-URL: Documentation, https://ngc-learn.readthedocs.io/
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/main/history.txt
@@ -48,16 +48,16 @@
 
 It is currently maintained by the
 <a href="https://www.cs.rit.edu/~ago/nac_lab.html">Neural Adaptive Computing (NAC) laboratory</a>.
 
 ## <b>Documentation</b>
 
 Official documentation, including tutorials, can be found
-<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo, 
-which implements several historical models, can be found 
+<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo,
+which implements several historical models, can be found
 <a href="https://github.com/NACLab/ngc-museum">here</a>.
 
 The official blog-post related to the source paper behind this software library
 can be found
 <a href="https://go.nature.com/3rgl1K8">here</a>.<br>
 You can find the related paper <a href="https://www.nature.com/articles/s41467-022-29632-7">right here</a>, which
 was selected to appear in the Nature <i>Neuromorphic Hardware and Computing Collection</i> in 2023 and was
@@ -99,38 +99,27 @@
 $ pip install ngclearn
 </pre>
 
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
-<!--
-<i>Setup:</i> To install ngc-learn, you can run (at the top-level of the
-the <code>ngclearn</code> directory) the following bash command:
-<pre>
-$ python install .
-</pre>
-
-Running the above pip install will automatically install the CPU
-version of JAX. If you want to use the GPU version instead, make sure to,
-before running the above, to install JAX via the correct pip command
-with the proper CUDA flags (depending on which CUDA is configured for your system)
-as per their
-<a href="https://jax.readthedocs.io/en/latest/installation.html">installation instructions</a>.
--->
-
-<!--
-(If you want to set up/install dependencies a priori, try running
-`$ pip install -r requirements.txt` first before pip installing ngc-learn.)
--->
-
 If the installation was successful, you should see the following if you test
 it against your Python interpreter, i.e., run the <code>$ python</code> command
-and complete the following sequence of steps as depicted in the screenshot below:<br>
-<img src="docs/images/test_ngclearn_install.png" width="512">
+and complete the following sequence of steps as depicted in the screenshot below
+(you should see at the bottom of your output something akin to the
+right major and minor version of ngc-learn):
+
+```console
+Python 3.11.4 (main, MONTH  DAY YEAR, TIME) [GCC XX.X.X] on linux
+Type "help", "copyright", "credits" or "license" for more information.
+>>> import ngclearn
+>>> ngclearn.__version__
+'1.0b3'
+```
 
 <i>Note:</i> For access to the previous Tensorflow-2 version of ngc-learn (of
 which we no longer support), please visit the repo for
 <a href="https://github.com/NACLab/ngc-learn-legacy"><i>ngc-learn-legacy</i></a>.
 
 ## <b>Attribution:</b>
 
@@ -168,15 +157,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.0.3-Beta <!-- -Alpha -->
+1.0.4-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngclearn Version: 1.0b3 Summary: Simulation
+Metadata-Version: 2.1 Name: ngclearn Version: 1.0b4 Summary: Simulation
 software for building and analyzing arbitrary predictive coding, spiking
 network, and biomimetic neural systems. Author-email: Alexander Ororbia
 cs.rit.edu>, William Gebhardt
 rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-learn Project-URL: Documentation, https://ngc-
 learn.readthedocs.io/ Project-URL: Lab Page, https://www.cs.rit.edu/~ago/
 nac_lab.html Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/
@@ -55,20 +55,23 @@
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn (CPU version) is through pip:
 $ pip install ngclearn
 The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
 this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
 20.04. If the installation was successful, you should see the following if you
 test it against your Python interpreter, i.e., run the $ python command and
-complete the following sequence of steps as depicted in the screenshot below:
-[docs/images/test_ngclearn_install.png]Note: For access to the previous
-Tensorflow-2 version of ngc-learn (of which we no longer support), please visit
-the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you use this code in any form
-in your project(s), please cite its source paper (as well as ngc-learn's
-official software citation):
+complete the following sequence of steps as depicted in the screenshot below
+(you should see at the bottom of your output something akin to the right major
+and minor version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY
+YEAR, TIME) [GCC XX.X.X] on linux Type "help", "copyright", "credits" or
+"license" for more information. >>> import ngclearn >>> ngclearn.__version__
+'1.0b3' ``` Note: For access to the previous Tensorflow-2 version of ngc-learn
+(of which we no longer support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ##
+AAttttrriibbuuttiioonn:: If you use this code in any form in your project(s), please cite
+its source paper (as well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
   journal={Nature Communications},
   year={2022},
   month={Apr},
   day={19},
@@ -84,15 +87,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.0.3-Beta Author: Alexander G. Ororbia II
+1.0.4-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.0b3/README.md` & `ngclearn-1.0b4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 It is currently maintained by the
 <a href="https://www.cs.rit.edu/~ago/nac_lab.html">Neural Adaptive Computing (NAC) laboratory</a>.
 
 ## <b>Documentation</b>
 
 Official documentation, including tutorials, can be found
-<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo, 
-which implements several historical models, can be found 
+<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo,
+which implements several historical models, can be found
 <a href="https://github.com/NACLab/ngc-museum">here</a>.
 
 The official blog-post related to the source paper behind this software library
 can be found
 <a href="https://go.nature.com/3rgl1K8">here</a>.<br>
 You can find the related paper <a href="https://www.nature.com/articles/s41467-022-29632-7">right here</a>, which
 was selected to appear in the Nature <i>Neuromorphic Hardware and Computing Collection</i> in 2023 and was
@@ -61,38 +61,27 @@
 $ pip install ngclearn
 </pre>
 
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
-<!--
-<i>Setup:</i> To install ngc-learn, you can run (at the top-level of the
-the <code>ngclearn</code> directory) the following bash command:
-<pre>
-$ python install .
-</pre>
-
-Running the above pip install will automatically install the CPU
-version of JAX. If you want to use the GPU version instead, make sure to,
-before running the above, to install JAX via the correct pip command
-with the proper CUDA flags (depending on which CUDA is configured for your system)
-as per their
-<a href="https://jax.readthedocs.io/en/latest/installation.html">installation instructions</a>.
--->
-
-<!--
-(If you want to set up/install dependencies a priori, try running
-`$ pip install -r requirements.txt` first before pip installing ngc-learn.)
--->
-
 If the installation was successful, you should see the following if you test
 it against your Python interpreter, i.e., run the <code>$ python</code> command
-and complete the following sequence of steps as depicted in the screenshot below:<br>
-<img src="docs/images/test_ngclearn_install.png" width="512">
+and complete the following sequence of steps as depicted in the screenshot below
+(you should see at the bottom of your output something akin to the
+right major and minor version of ngc-learn):
+
+```console
+Python 3.11.4 (main, MONTH  DAY YEAR, TIME) [GCC XX.X.X] on linux
+Type "help", "copyright", "credits" or "license" for more information.
+>>> import ngclearn
+>>> ngclearn.__version__
+'1.0b3'
+```
 
 <i>Note:</i> For access to the previous Tensorflow-2 version of ngc-learn (of
 which we no longer support), please visit the repo for
 <a href="https://github.com/NACLab/ngc-learn-legacy"><i>ngc-learn-legacy</i></a>.
 
 ## <b>Attribution:</b>
 
@@ -130,15 +119,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.0.3-Beta <!-- -Alpha -->
+1.0.4-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -31,20 +31,23 @@
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn (CPU version) is through pip:
 $ pip install ngclearn
 The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
 this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
 20.04. If the installation was successful, you should see the following if you
 test it against your Python interpreter, i.e., run the $ python command and
-complete the following sequence of steps as depicted in the screenshot below:
-[docs/images/test_ngclearn_install.png]Note: For access to the previous
-Tensorflow-2 version of ngc-learn (of which we no longer support), please visit
-the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you use this code in any form
-in your project(s), please cite its source paper (as well as ngc-learn's
-official software citation):
+complete the following sequence of steps as depicted in the screenshot below
+(you should see at the bottom of your output something akin to the right major
+and minor version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY
+YEAR, TIME) [GCC XX.X.X] on linux Type "help", "copyright", "credits" or
+"license" for more information. >>> import ngclearn >>> ngclearn.__version__
+'1.0b3' ``` Note: For access to the previous Tensorflow-2 version of ngc-learn
+(of which we no longer support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ##
+AAttttrriibbuuttiioonn:: If you use this code in any form in your project(s), please cite
+its source paper (as well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
   journal={Nature Communications},
   year={2022},
   month={Apr},
   day={19},
@@ -60,15 +63,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.0.3-Beta Author: Alexander G. Ororbia II
+1.0.4-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.0b3/ngclearn/__init__.py` & `ngclearn-1.0b4/ngclearn/__init__.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/__init__.py` & `ngclearn-1.0b4/ngclearn/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/baseComponentTemplate.py` & `ngclearn-1.0b4/ngclearn/components/baseComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/input_encoders/bernoulliCell.py` & `ngclearn-1.0b4/ngclearn/components/input_encoders/bernoulliCell.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @jit
 def sample_bernoulli(dkey, data):
     """
     Samples a Bernoulli spike train on-the-fly
 
     Args:
         dkey: JAX key to drive stochasticity/noise
-        
+
         data: sensory data (vector/matrix)
 
     Returns:
         binary spikes
     """
     s_t = random.bernoulli(dkey, p=data).astype(jnp.float32)
     return s_t
```

### Comparing `ngclearn-1.0b3/ngclearn/components/input_encoders/latencyCell.py` & `ngclearn-1.0b4/ngclearn/components/input_encoders/latencyCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/input_encoders/poissonCell.py` & `ngclearn-1.0b4/ngclearn/components/input_encoders/poissonCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/neurons/graded/gaussianErrorCell.py` & `ngclearn-1.0b4/ngclearn/components/neurons/graded/gaussianErrorCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/neurons/graded/laplacianErrorCell.py` & `ngclearn-1.0b4/ngclearn/components/neurons/graded/laplacianErrorCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/neurons/graded/rateCell.py` & `ngclearn-1.0b4/ngclearn/components/neurons/graded/rateCell.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         elif priorType == "cauchy":  ## Cauchy dist: x ~ (1.0 + tf.math.square(z))
             z_leak = (z * 2)/(1. + jnp.square(z))
         elif priorType == "exp":  ## Exp dist: x ~ -exp(-x^2)
             z_leak = jnp.exp(-jnp.square(z)) * z * 2
     dz_dt = (-z_leak * leak_gamma + (j + j_td)) * (1./tau_m)
     return dz_dt
 
-def _dfz(z, params): ## diff-eq dynamics wrapper
+def _dfz(t, z, params): ## diff-eq dynamics wrapper
     j, j_td, tau_m, leak_gamma, priorType = params
     dz_dt = _dfz_internal(z, j, j_td, tau_m, leak_gamma, priorType)
     return dz_dt
 
 @jit
 def modulate(j, dfx_val):
     """
@@ -66,18 +66,18 @@
         priorType: scale-shift prior distribution to impose over neural dynamics
 
     Returns:
         New value of membrane/state for next time step
     """
     if integType == 1:
         params = (j, j_td, tau_m, leak_gamma, priorType)
-        _z = step_rk2(z, params, _dfz, dt)
+        _, _z = step_rk2(0., z, _dfz, dt, params)
     else:
         params = (j, j_td, tau_m, leak_gamma, priorType)
-        _z = step_euler(z, params, _dfz, dt)
+        _, _z = step_euler(0., z, _dfz, dt, params)
     return _z
 
 @jit
 def run_cell_stateless(j):
     """
     A simplification of running a stateless set of dynamics over j (an identity
     functional form of dynamics).
```

### Comparing `ngclearn-1.0b3/ngclearn/components/neurons/spiking/LIFCell.py` & `ngclearn-1.0b4/ngclearn/components/neurons/spiking/LIFCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py` & `ngclearn-1.0b4/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 
 @jit
 def _dfv_internal(j, v, w, a, b, g, tau_m): ## raw voltage dynamics
     dv_dt = v - jnp.power(v, 3)/g - w + j ## dv/dt
     dv_dt = dv_dt * (1./tau_m)
     return dv_dt
 
-def _dfv(v, params): ## voltage dynamics wrapper
+def _dfv(t, v, params): ## voltage dynamics wrapper
     j, w, a, b, g, tau_m = params
     dv_dt = _dfv_internal(j, v, w, a, b, g, tau_m)
     return dv_dt
 
 @jit
 def _dfw_internal(j, v, w, a, b, g, tau_w): ## raw recovery dynamics
     dw_dt = v + a - b * w ## dw/dt
     dw_dt = dw_dt * (1./tau_w)
     return dw_dt
 
-def _dfw(w, params): ## recovery dynamics wrapper
+def _dfw(t, w, params): ## recovery dynamics wrapper
     j, v, a, b, g, tau_m = params
     dv_dt = _dfw_internal(j, v, w, a, b, g, tau_m)
     return dv_dt
 
 @jit
 def _emit_spike(v, v_thr):
     s = (v > v_thr).astype(jnp.float32)
@@ -79,22 +79,22 @@
         integType: integration type to use (0 --> Euler/RK1, 1 --> Midpoint/RK2)
 
     Returns:
         updated voltage, updated recovery, spikes
     """
     if integType == 1:
         v_params = (j, w, a, b, g, tau_m)
-        _v = step_rk2(v, v_params, _dfv, dt)
+        _, _v = step_rk2(0., v, _dfv, dt, v_params) #_v = step_rk2(v, v_params, _dfv, dt)
         w_params = (j, v, a, b, g, tau_w)
-        _w = step_rk2(w, w_params, _dfw, dt)
+        _, _w = step_rk2(0., w, _dfw, dt, w_params) #_w = step_rk2(w, w_params, _dfw, dt)
     else: # integType == 0 (default -- Euler)
         v_params = (j, w, a, b, g, tau_m)
-        _v = step_euler(v, v_params, _dfv, dt)
+        _, _v = step_euler(0., v, _dfv, dt, v_params) #_v = step_euler(v, v_params, _dfv, dt)
         w_params = (j, v, a, b, g, tau_w)
-        _w = step_euler(w, w_params, _dfw, dt)
+        _, _w = step_euler(0., w, _dfw, dt, w_params) #_w = step_euler(w, w_params, _dfw, dt)
     #s = (_v > v_thr).astype(jnp.float32)
     s = _emit_spike(_v, v_thr)
     return _v, _w, s
 
 class FitzhughNagumoCell(Component):
     """
     The Fitzhugh-Nagumo neuronal cell model; a two-variable simplification
```

### Comparing `ngclearn-1.0b3/ngclearn/components/neurons/spiking/izhikevichCell.py` & `ngclearn-1.0b4/ngclearn/components/neurons/spiking/izhikevichCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 @jit
 def _dfv_internal(j, v, w, b, tau_m): ## raw voltage dynamics
     ## (v^2 * 0.04 + v * 5 + 140 - u + j) * a, where a = (1./tau_m) (w = u)
     dv_dt = (jnp.square(v) * 0.04 + v * 5. + 140. - w + j)
     dv_dt = dv_dt * (1./tau_m)
     return dv_dt
 
-def _dfv(v, params): ## voltage dynamics wrapper
+def _dfv(t, v, params): ## voltage dynamics wrapper
     j, w, b, tau_m = params
     dv_dt = _dfv_internal(j, v, w, b, tau_m)
     return dv_dt
 
 @jit
 def _dfw_internal(j, v, w, b, tau_w): ## raw recovery dynamics
     ## (v * b - u) from (v * b - u) * a (Izh. form)  (w = u)
     dw_dt = (v * b - w)
     dw_dt = dw_dt * (1./tau_w)
     return dw_dt
 
-def _dfw(w, params): ## recovery dynamics wrapper
+def _dfw(t, w, params): ## recovery dynamics wrapper
     j, v, b, tau_w = params
     dv_dt = _dfw_internal(j, v, w, b, tau_w)
     return dv_dt
 
 def _post_process(s, _v, _w, v, w, c, d): ## internal post-processing routine
     # this step is specific to izh neuronal cells, where, after dynamics
     # have evolved for a step in term, we then use the variables c and d
@@ -108,22 +108,22 @@
     _j = _modify_current(j, R_m)
     #_j = jnp.maximum(-30.0, _j) ## lower-bound/clip input current
     ## check for spikes
     s = _emit_spike(v, v_thr)
     ## for non-spikes, evolve according to dynamics
     if integType == 1:
         v_params = (_j, w, b, tau_m)
-        _v = step_rk2(v, v_params, _dfv, dt)
+        _, _v = step_rk2(0., v, _dfv, dt, v_params) #_v = step_rk2(v, v_params, _dfv, dt)
         w_params = (_j, v, b, tau_w)
-        _w = step_rk2(w, w_params, _dfw, dt)
+        _, _w = step_rk2(0., w, _dfw, dt, w_params) #_w = step_rk2(w, w_params, _dfw, dt)
     else: # integType == 0 (default -- Euler)
         v_params = (_j, w, b, tau_m)
-        _v = step_euler(v, v_params, _dfv, dt)
+        _, _v = step_euler(0., v, _dfv, dt, v_params) #_v = step_euler(v, v_params, _dfv, dt)
         w_params = (_j, v, b, tau_w)
-        _w = step_euler(w, w_params, _dfw, dt)
+        _, _w = step_euler(0., w, _dfw, dt, w_params) #_w = step_euler(w, w_params, _dfw, dt)
     ## for spikes, snap to particular states
     _v, _w = _post_process(s, _v, _w, v, w, c, d)
     return  _v, _w, s
 
 class IzhikevichCell(Component): ## Izhikevich neuronal cell
     """
     A spiking cell based on Izhikevich's model of neuronal dynamics. Note that
```

### Comparing `ngclearn-1.0b3/ngclearn/components/neurons/spiking/quadLIFCell.py` & `ngclearn-1.0b4/ngclearn/components/neurons/spiking/quadLIFCell.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/neurons/spiking/sLIFCell.py` & `ngclearn-1.0b4/UPDATED_cells/older_sLIF.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from ngcsimlib.component import Component
 from jax import numpy as jnp, random, jit
 from functools import partial
 import time, sys
+from ngclearn.utils.diffeq.ode_utils import get_integrator_code, \
+                                            step_euler, step_rk2
 from ngclearn.utils.surrogate_fx import secant_lif_estimator
 
 @jit
 def update_times(t, s, tols):
     """
     Updates time-of-last-spike (tols) variable.
 
@@ -52,22 +54,34 @@
     """
     _j = j * R_m
     if inh_R > 0.:
         _j = _j - (jnp.matmul(spikes, inh_weights) * inh_R)
     return _j
 
 ## co-routines for run_cell
-@partial(jit, static_argnums=[4,5,6])
-def _update_voltage(dt, j, v, rfr, tau_m, refract_T, v_min=None):
+# @partial(jit, static_argnums=[4,5,6])
+# def _update_voltage(dt, j, v, rfr, tau_m, refract_T, v_min=None):
+#     mask = (rfr >= refract_T).astype(jnp.float32) # get refractory mask
+#     _v = (v + (-v + j) * (dt / tau_m)) * mask
+#     if v_min is not None:
+#         _v = jnp.maximum(v_min, _v)
+#     #_v = v + (-v) * (dt / tau_m) + j * mask
+#     return _v, mask
+
+@jit
+def _dfv_internal(j, v, rfr, tau_m, refract_T): ## raw voltage dynamics
     mask = (rfr >= refract_T).astype(jnp.float32) # get refractory mask
-    _v = (v + (-v + j) * (dt / tau_m)) * mask
-    if v_min is not None:
-        _v = jnp.maximum(v_min, _v)
-    #_v = v + (-v) * (dt / tau_m) + j * mask
-    return _v, mask
+    dv_dt = ((-v + j) * (dt / tau_m)) * mask
+    dv_dt = dv_dt * (1./tau_m)
+    return dv_dt
+
+def _dfv(v, params): ## voltage dynamics wrapper
+    j, rfr, tau_m, refract_T = params
+    dv_dt = _dfv_internal(j, v, rfr, tau_m, refract_T)
+    return dv_dt
 
 @jit
 def _hyperpolarize(v, s):
     _v = (1. - s) * v ## hyper-polarize cells
     return _v
 
 @partial(jit, static_argnums=[3,4,5])
@@ -124,28 +138,33 @@
         sticky_spikes: if True, then spikes are pinned at value of action potential
             (i.e., 1) for as long as the relative refractory occurs (this recovers
             the source paper's core spiking process)
 
     Returns:
         voltage(t+dt), spikes, threshold(t+dt), updated refactory variables
     """
-    new_voltage, mask = _update_voltage(dt, j, v, rfr, tau_m, refract_T, v_min)
-    spikes = spike_fx(new_voltage, v_thr)
-    new_voltage = _hyperpolarize(new_voltage, spikes)
+    #new_voltage, mask = _update_voltage(dt, j, v, rfr, tau_m, refract_T, v_min)
+    v_params = (j, rfr, tau_m, refract_T)
+    _v = step_euler(v, v_params, _dfv, dt)
+    # if v_min is not None:
+    #     _v = jnp.maximum(v_min, _v)
+    spikes = spike_fx(_v, v_thr)
+    _v = _hyperpolarize(_v, spikes)
     new_thr = _update_threshold(dt, v_thr, spikes, thrGain, thrLeak, rho_b)
     _rfr, spikes = _update_refract_and_spikes(dt, rfr, spikes, mask, sticky_spikes)
-    return new_voltage, spikes, new_thr, _rfr
+    return _v, spikes, new_thr, _rfr
 
 class SLIFCell(Component): ## leaky integrate-and-fire cell
     """
     A spiking cell based on a simplified leaky integrate-and-fire (sLIF) model.
     This neuronal cell notably contains functionality required by the computational
     model employed by (Samadi et al., 2017, i.e., a surrogate derivative function
     and "sticky spikes") as well as the additional incorporation of an adaptive
-    threshold (per unit) scheme.
+    threshold (per unit) scheme. (Note that this particular spiking cell only
+    supports Euler integration of its voltage dynamics.)
 
     | Reference:
     | Samadi, Arash, Timothy P. Lillicrap, and Douglas B. Tweed. "Deep learning with
     | dynamic spiking neurons and fixed feedback weights." Neural computation 29.3
     | (2017): 578-602.
 
     Args:
@@ -340,15 +359,15 @@
         if self.refract is None:
             self.refract = jnp.zeros((self.batch_size, self.n_units)) + self.refract_T
         ## run one step of Euler integration over neuronal dynamics
         j_curr = self.current
         ## apply simplified inhibitory pressure
         j_curr = modify_current(j_curr, self.spikes, self.inh_weights, self.R_m, self.inh_R)
         self.current = j_curr # None ## store electrical current
-        self.surrogate = self.d_spike_fx(j_curr, self.voltage, self.threshold, c1=0.82, c2=0.08)
+        self.surrogate = self.d_spike_fx(j_curr, c1=0.82, c2=0.08)
         self.voltage, self.spikes, self.threshold, self.refract = \
             run_cell(dt, j_curr, self.voltage, self.threshold, self.tau_m,
                      self.refract, self.spike_fx, self.refract_T, self.thrGain, self.thrLeak,
                      self.rho_b, sticky_spikes=self.sticky_spikes, v_min=self.v_min)
         ## update tols
         self.timeOfLastSpike = update_times(t, self.spikes, self.timeOfLastSpike)
```

### Comparing `ngclearn-1.0b3/ngclearn/components/other/expKernel.py` & `ngclearn-1.0b4/ngclearn/components/other/expKernel.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/other/varTrace.py` & `ngclearn-1.0b4/ngclearn/components/other/varTrace.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/synapses/hebbian/expSTDPSynapse.py` & `ngclearn-1.0b4/ngclearn/components/synapses/hebbian/expSTDPSynapse.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/components/synapses/hebbian/hebbianSynapse.py` & `ngclearn-1.0b4/ngclearn/components/synapses/hebbian/hebbianSynapse.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,30 +65,33 @@
         if is_nonnegative == True:
             _W = jnp.clip(_W, 0., w_bound)
         else:
             _W = jnp.clip(_W, -w_bound, w_bound)
     return _W
 
 @jit
-def compute_layer(inp, weight, biases):
+def compute_layer(inp, weight, biases, Rscale):
     """
     Applies the transformation/projection induced by the synaptic efficacie
     associated with this synaptic cable
 
     Args:
         inp: signal input to run through this synaptic cable
 
         weight: this cable's synaptic value matrix
 
         biases: this cable's bias value vector
 
+        Rscale: scale factor to apply to synapses before transform applied
+            to input values
+
     Returns:
         a projection/transformation of input "inp"
     """
-    return jnp.matmul(inp, weight) + biases
+    return jnp.matmul(inp, weight * Rscale) + biases
 
 class HebbianSynapse(Component):
     """
     A synaptic cable that adjusts its efficacies via a two-factor Hebbian
     adjustment rule.
 
     Args:
@@ -131,14 +134,17 @@
                 a negative learning rate will mean a descent form of the
                 `optim_scheme` is being employed
 
         pre_wght: pre-synaptic weighting factor (Default: 1.)
 
         post_wght: post-synaptic weighting factor (Default: 1.)
 
+        Rscale: a fixed scaling factor to apply to synaptic transform
+            (Default: 1.), i.e., yields: out = ((W * Rscale) * in) + b
+
         key: PRNG key to control determinism of any underlying random values
             associated with this synaptic cable
 
         useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
 
         directory: string indicating directory on disk to save synaptic parameter
             values to (i.e., initial threshold values and any persistent adaptive
@@ -206,25 +212,26 @@
     @postsynapticCompartment.setter
     def postsynapticCompartment(self, x):
         self.compartments[self.postsynapticCompartmentName()] = x
 
     # Define Functions
     def __init__(self, name, shape, eta=0., wInit=("uniform", 0., 0.3),
                  bInit=None, w_bound=1., is_nonnegative=False, w_decay=0.,
-                 signVal=1., optim_type="sgd", pre_wght=1., post_wght=1., 
-                 key=None, useVerboseDict=False, directory=None, **kwargs):
+                 signVal=1., optim_type="sgd", pre_wght=1., post_wght=1.,
+                 Rscale=1., key=None, useVerboseDict=False, directory=None, **kwargs):
         super().__init__(name, useVerboseDict, **kwargs)
 
         ## random Number Set up
         self.key = key
         if self.key is None:
             self.key = random.PRNGKey(time.time_ns())
 
         ## synaptic plasticity properties and characteristics
         self.shape = shape
+        self.Rscale = Rscale
         self.w_bounds = w_bound
         self.w_decay = w_decay ## synaptic decay
         self.pre_wght = pre_wght
         self.post_wght = post_wght
         self.eta = eta
         self.wInit = wInit
         self.bInit = bInit
@@ -256,16 +263,16 @@
     def verify_connections(self):
         self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
 
     def advance_state(self, **kwargs):
         biases = 0.
         if self.bInit != None:
             biases = self.biases
-        self.outputCompartment = compute_layer(self.inputCompartment,
-                                               self.weights, biases)
+        self.outputCompartment = compute_layer(self.inputCompartment, self.weights,
+                                               biases, self.Rscale)
 
     def evolve(self, t, dt, **kwargs):
         dW, db = calc_update(self.presynapticCompartment, self.postsynapticCompartment,
                              self.weights, self.w_bounds, is_nonnegative=self.is_nonnegative,
                              signVal=self.signVal, w_decay=self.w_decay,
                              pre_wght=self.pre_wght, post_wght=self.post_wght)
         self.dW = dW
@@ -300,9 +307,9 @@
         else:
             jnp.savez(file_name, weights=self.weights)
 
     def load(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
         data = jnp.load(file_name)
         self.weights = data['weights']
-        if self.bInit != None:
+        if "biases" in data.keys():
             self.biases = data['biases']
```

### Comparing `ngclearn-1.0b3/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py` & `ngclearn-1.0b4/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/data_loader.py` & `ngclearn-1.0b4/ngclearn/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/density/gmm.py` & `ngclearn-1.0b4/ngclearn/utils/density/gmm.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/diffeq/ode_utils.py` & `ngclearn-1.0b4/ngclearn/utils/diffeq/_ode_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     #     intgFlag = 3
     else:
         if integrationType != "euler" or integrationType == "rk1":
             print("ERROR: unrecognized integration method {} provided! Defaulting \
                   to RK-1/Euler routine".format(integrationType))
     return intgFlag
 
-def step_euler(x, params, dfx, dt, dt_div=1., x_scale=1.): ## RK-1 routine
+def step_euler(x, params, dfx, dt, dt_div=1., t=None, x_scale=1.): ## RK-1 routine
     """
     Iteratively integrates one step forward via the Euler method, i.e., a
     first-order Runge-Kutta (RK-1) step.
 
     Args:
         x: current variable values to advance/iteratively integrate (at time `t`)
 
@@ -45,55 +45,66 @@
         dfx: (ordinary) differential equation co-routine (as implemented in an
             ngc-learn component)
 
         dt: integration time step (also referred to as `h` in mathematics)
 
         dt_div: factor to divide `dt` by (Default: 1)
 
+        t: (optional) time step (for equations that use t in dt)
+
         x_scale: dampening factor to scale `x` by (Default: 1)
 
     Returns:
         variable values iteratively integrated/advanced to next step (`t + dt`)
     """
-    dx_dt = dfx(x, params) ## assumed will be a jit-i-fied function
+    _t = t
+    if _t == None:
+        _t = 0.
+    dx_dt = dfx(x, params, _t) ## assumed will be a jit-i-fied function
+    print("{} dy: {}  y_ {} dt {}".format(_t, dx_dt, x, dt))
+    print("Out: ",(x + dx_dt * dt))
     return _step_forward(x, dx_dt, dt, dt_div, x_scale) ## jit-i-fied function
 
-def step_rk2(x, params, dfx, dt): ## RK-2 routine
+def step_rk2(x, params, dfx, dt, t=None): ## RK-2 routine
     """
-    Iteratively integrates one step forward via the midpoint method, i.e., a
+    Iteratively integrates one step forward via the (explicit) midpoint method, i.e., a
     second-order Runge-Kutta (RK-2) step. (Note: ngc-learn internally recognizes
     "rk2" or "midpoint" for this routine)
 
     Args:
         x: current variable values to advance/iteratively integrate (at time `t`)
 
         params: tuple containing configuration values/hyper-parameters for the
             (ordinary) differential equation an ngc-learn component will provide
 
         dfx: (ordinary) differential equation co-routine (as implemented in an
             ngc-learn component)
 
         dt: integration time step (also referred to as `h` in mathematics)
 
-        dt_div: factor to divide `dt` by (Default: 1)
-
-        x_scale: dampening factor to scale `x` by (Default: 1)
+        t: (optional) time step (for equations that use t in dt)
 
     Returns:
         variable values iteratively integrated/advanced to next step (`t + dt`)
     """
-    _x1 = step_euler(x, params, dfx, dt, dt_div=2.)
-    dx_dt = dfx(_x1, params) ## assumed will be a jit-i-fied function
+    _t = t
+    if _t == None:
+        _t = 0.
+    #print("-- midpoint --")
+    #_x1 = step_euler(x, params, dfx, dt, dt_div=2.) # k1 is inside here
+    _dx_dt = dfx(x, params, _t/2.) ## assumed will be a jit-i-fied function
+    _x1 =  _step_forward(x, _dx_dt, dt, dt_div=2.)
+    dx_dt = dfx(_x1, params, (_t + dt)/2.) ## k2
     _x2 = _step_forward(x, dx_dt, dt) ## get 2nd order estimate
     return _x2
 
-def step_rk2_heun(x, params, dfx, dt): ## Heun's method routine
+def step_rk2_heun(x, params, dfx, dt, t=None): ## Heun's method routine
     """
     Iteratively integrates one step forward via Heun's method, i.e., a
-    second-order Runge-Kutta (RK-2) error-corrected step.
+    second-order Runge-Kutta (RK-2) error-corrected step (or the explicit trapezoid method).
     (Note: ngc-learn internally recognizes "rk2_heun" or "heun" for this routine)
 
     | Reference:
     | Ascher, Uri M., and Linda R. Petzold. Computer methods for ordinary
     | differential equations and differential-algebraic equations. Society for
     | Industrial and Applied Mathematics, 1998.
 
@@ -104,31 +115,43 @@
             (ordinary) differential equation an ngc-learn component will provide
 
         dfx: (ordinary) differential equation co-routine (as implemented in an
             ngc-learn component)
 
         dt: integration time step (also referred to as `h` in mathematics)
 
-        dt_div: factor to divide `dt` by (Default: 1)
-
-        x_scale: dampening factor to scale `x` by (Default: 1)
+        t: (optional) time step (for equations that use t in dt)
 
     Returns:
         variable values iteratively integrated/advanced to next step (`t + dt`)
     """
-    ## perform Euler estimate
-    dx_dt = dfx(x, params)
-    _x1 = _step_forward(x, dx_dt, dt, dt_div=1.)
-    ## compute
-    dx1_dt = dfx(_x1, params) ## obtain differential at intermediate step
-    dx = _avg(dx_dt, dx1_dt) ## get corrected flow (sum of over/under estimates)
-    _x2 = _step_forward(x, dx, dt, dt_div=1.) ## get 2nd order estimate
+    _t = t
+    if _t == None:
+        _t = 0.
+    #print("-- trapezoid --")
+    ## apply Heun's formulas to update y
+    k1 = dx_dt = dfx(x, params, _t) # k1
+    #print("k1: ",k1)
+    _x = _step_forward(x, k1, dt, dt_div=1.)
+    k2 = dfx(_x, params, _t + dt)
+    #print("k2: ",k2)
+    k_sum = _add(k1, k2)
+    #print(k_sum/2.)
+    _x2 = _step_forward(x, k_sum, dt, dt_div=2.) ## get 2nd order estimate
+    # ## compute
+    # dx1_dt = dfx(_x1, params) ## obtain differential at intermediate step
+    # dx = _avg(dx_dt, dx1_dt) ## get corrected flow (sum of over/under estimates)
+    # _x2 = _step_forward(x, dx, dt, dt_div=1.) ## get 2nd order estimate
     return _x2
 
 @jit
 def _avg(y1, y2): ## fast co-routine for simple midpoint/average
     return (y1 + y2)/2.
 
+@jit
+def _add(y1, y2): ## fast co-routine for simple addition
+    return (y1 + y2)
+
 @jit #@partial(jit, static_argnums=[3, 4])
 def _step_forward(x, dx_dt, dt, dt_div=1., x_scale=1.): ## internal integration co-routine
     _x = x * x_scale + dx_dt * (dt/dt_div)
     return _x
```

### Comparing `ngclearn-1.0b3/ngclearn/utils/io_utils.py` & `ngclearn-1.0b4/ngclearn/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/metric_utils.py` & `ngclearn-1.0b4/ngclearn/utils/metric_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     loss = -(x * jnp.log(p_))
     nll = jnp.sum(loss, axis=1, keepdims=True) #/(y_true.shape[0] * 1.0)
     if preserve_batch == False:
         nll = jnp.mean(nll)
     return nll #tf.reduce_mean(nll)
 
 @jit
-def measure_MSE(mu, x):
+def measure_MSE(mu, x, preserve_batch=False):
     """
     Measures mean squared error (MSE), or the negative Gaussian log likelihood
     with variance of 1.0. Note: If batch is preserved, this returns a column
     vector where each row is the MSE(mu, x) for that row's datapoint.
 
     Args:
         mu: predicted values (mean); (N x D matrix)
@@ -117,17 +117,19 @@
         preserve_batch: if True, will return one score per sample in batch
             (Default: False), otherwise, returns scalar mean score
 
     Returns:
         an (N x 1) column vector (if preserve_batch=True) OR (1,1) scalar otherwise
     """
     diff = mu - x
-    se = jnp.square(diff) #diff * diff # squared error
-    # NLL = -( -se )
-    return jnp.sum(se, axis=1, keepdims=True) # tf.math.reduce_mean(se)
+    se = jnp.square(diff) ## squared error
+    mse = jnp.sum(se, axis=1, keepdims=True) # technically se at this point
+    if preserve_batch == False:
+        mse = jnp.mean(mse) # this is proper mse
+    return mse
 
 @jit
 def measure_BCE(p, x, offset=1e-7, preserve_batch=False): #1e-10
     """
     Calculates the negative Bernoulli log likelihood or binary cross entropy (BCE).
     Note: If batch is preserved, this returns a column vector where each row is
     the BCE(p, x) for that row's datapoint.
@@ -142,8 +144,11 @@
         preserve_batch: if True, will return one score per sample in batch
             (Default: False), otherwise, returns scalar mean score
 
     Returns:
         an (N x 1) column vector (if preserve_batch=True) OR (1,1) scalar otherwise
     """
     p_ = jnp.clip(p, offset, 1 - offset)
-    return -jnp.sum(x * jnp.log(p_) + (1.0 - x) * jnp.log(1.0 - p_),axis=1, keepdims=True)
+    bce = -jnp.sum(x * jnp.log(p_) + (1.0 - x) * jnp.log(1.0 - p_),axis=1, keepdims=True)
+    if preserve_batch == False:
+        bce = jnp.mean(bce)
+    return bce
```

### Comparing `ngclearn-1.0b3/ngclearn/utils/model_utils.py` & `ngclearn-1.0b4/ngclearn/utils/model_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     loss = -(x * jnp.log(p_))
     nll = jnp.sum(loss, axis=1, keepdims=True) #/(y_true.shape[0] * 1.0)
     if preserve_batch == False:
         nll = jnp.mean(nll)
     return nll #tf.reduce_mean(nll)
 
 @jit
-def measure_MSE(mu, x):
+def measure_MSE(mu, x, preserve_batch=False):
     """
     Measures mean squared error (MSE), or the negative Gaussian log likelihood
     with variance of 1.0. Note: If batch is preserved, this returns a column
     vector where each row is the MSE(mu, x) for that row's datapoint.
 
     Args:
         mu: predicted values (mean); (N x D matrix)
@@ -119,17 +119,19 @@
         preserve_batch: if True, will return one score per sample in batch
             (Default: False), otherwise, returns scalar mean score
 
     Returns:
         an (N x 1) column vector (if preserve_batch=True) OR (1,1) scalar otherwise
     """
     diff = mu - x
-    se = jnp.square(diff) #diff * diff # squared error
-    # NLL = -( -se )
-    return jnp.sum(se, axis=1, keepdims=True) # tf.math.reduce_mean(se)
+    se = jnp.square(diff) ## squared error
+    mse = jnp.sum(se, axis=1, keepdims=True) # technically se at this point
+    if preserve_batch == False:
+        mse = jnp.mean(mse) # this is proper mse
+    return mse
 
 @jit
 def measure_BCE(p, x, offset=1e-7, preserve_batch=False): #1e-10
     """
     Calculates the negative Bernoulli log likelihood or binary cross entropy (BCE).
     Note: If batch is preserved, this returns a column vector where each row is
     the BCE(p, x) for that row's datapoint.
@@ -144,17 +146,20 @@
         preserve_batch: if True, will return one score per sample in batch
             (Default: False), otherwise, returns scalar mean score
 
     Returns:
         an (N x 1) column vector (if preserve_batch=True) OR (1,1) scalar otherwise
     """
     p_ = jnp.clip(p, offset, 1 - offset)
-    return -jnp.sum(x * jnp.log(p_) + (1.0 - x) * jnp.log(1.0 - p_),axis=1, keepdims=True)
+    bce = -jnp.sum(x * jnp.log(p_) + (1.0 - x) * jnp.log(1.0 - p_),axis=1, keepdims=True)
+    if preserve_batch == False:
+        bce = jnp.mean(bce)
+    return bce
 
-def create_function(fun_name):
+def create_function(fun_name, args=None):
     """
     Activation function creation routine.
 
     Args:
         fun_name: string name of activation function to produce
             (Currently supports: "tanh", "relu", "lrelu", "identity")
 
@@ -177,14 +182,20 @@
         dfx = d_lrelu
     elif fun_name == "relu6":
         fx = relu6
         dfx = d_relu6
     elif fun_name == "softplus":
         fx = softplus
         dfx = d_softplus
+    elif fun_name == "unit_threshold":
+        fx = threshold ## default threshold is 1 (thus unit)
+        dfx = d_threshold ## STE approximation
+    elif "heaviside" in fun_name:
+        fx = heaviside
+        dfx = d_heaviside ## STE approximation
     elif fun_name == "identity":
         fx = identity
         dfx = d_identity
     else:
         raise RuntimeError(
             "Activition function (" + fun_name + ") is not recognized/supported!"
             )
@@ -513,14 +524,30 @@
     Returns:
         output (tensor) derivative value (with respect to input argument)
     """
     ## d/dx of softplus = logistic sigmoid
     return nn.sigmoid(x)
 
 @jit
+def threshold(x, thr=1.):
+    return (x >= thr).astype(jnp.float32)
+
+@jit
+def d_threshold(x, thr=1.):
+    return x * 0. + 1. ## straight-thru estimator
+
+@jit
+def heaviside(x):
+    return (x >= 0.).astype(jnp.float32)
+
+@jit
+def d_heaviside(x):
+    return x * 0. + 1. ## straight-thru estimator
+
+@jit
 def sigmoid(x):
     return nn.sigmoid(x)
 
 @jit
 def d_sigmoid(x):
     sigm_x = nn.sigmoid(x) ## pre-compute once
     return sigm_x * (1. - sigm_x)
```

### Comparing `ngclearn-1.0b3/ngclearn/utils/optim/adam.py` & `ngclearn-1.0b4/ngclearn/utils/optim/adam.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/optim/opt.py` & `ngclearn-1.0b4/ngclearn/utils/optim/opt.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/optim/sgd.py` & `ngclearn-1.0b4/ngclearn/utils/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/patch_utils.py` & `ngclearn-1.0b4/ngclearn/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/viz/dim_reduce.py` & `ngclearn-1.0b4/ngclearn/utils/viz/dim_reduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         ipca = IncrementalPCA(n_components=2, batch_size=batch_size)
         ipca.fit(vectors)
         z_2D = ipca.transform(vectors)
     else:
         z_2D = vectors
     return z_2D
 
-def extract_tsne_latents(vectors, perplexity=30): ## tSNE mapping routine
+def extract_tsne_latents(vectors, perplexity=30, n_pca_comp=32): ## tSNE mapping routine
     """
     Projects collection of K vectors (stored in a matrix) to a two-dimensional (2D)
     visualization space via the t-distributed stochastic neighbor embedding
     algorithm (t-SNE). This algorithm also uses PCA to produce an
     intermediate project to speed up the t-SNE final mapping step. Note that
     if the input already has a 2D dimensionality, the original input is returned.
 
@@ -42,34 +42,36 @@
         vectors: a matrix/codebook of (K x D) vectors to project
 
         perplexity: the perplexity control factor for t-SNE (Default: 30)
 
     Returns:
         a matrix (K x 2) of projected vectors (to 2D space)
     """
-    batch_size = 50
+    batch_size = 500 #50
     z_dim = vectors.shape[1]
     z_2D = None
     if z_dim != 2:
         print(" > Projecting latents via iPCA...")
-        n_comp = 32 #10 #16 #50
+        n_comp = n_pca_comp #32 #10 #16 #50
+        if n_comp > batch_size:
+            batch_size = n_comp
         if vectors.shape[1] < n_comp:
             n_comp = vectors.shape[1] - 2 #z_top.shape[1]-2
             n_comp = max(2, n_comp)
         ipca = IncrementalPCA(n_components=n_comp, batch_size=batch_size)
         ipca.fit(vectors)
         z_2D = ipca.transform(vectors)
         print(" PCA.lat.shape = ",z_2D.shape)
         print(" > Finishing projection via t-SNE...")
         z_2D = TSNE(n_components=2,perplexity=perplexity, verbose=1).fit_transform(z_2D)
     else:
         z_2D = vectors
     return z_2D
 
-def plot_latents(code_vectors, labels, plot_fname="2Dcode_plot.jpg"):
+def plot_latents(code_vectors, labels, plot_fname="2Dcode_plot.jpg", alpha=1.):
     """
     Produces a label-overlaid (label map to distinct colors) scatterplot for
     visualizing two-dimensional latent codes (produced by either PCA or t-SNE).
 
     Args:
         code_vectors: a matrix of shape (K x 2) with vectors to plot/visualize
 
@@ -80,12 +82,12 @@
         plot_fname: /path/to/plot_fname.<suffix> for saving the plot to disk
     """
     print(" > Plotting 2D latent encodings...")
     lab = labels
     if lab.shape[1] > 1: ## extract integer class labels from a one-hot matrix
         lab = np.argmax(lab, 1)
     plt.figure(figsize=(8, 6))
-    plt.scatter(code_vectors[:, 0], code_vectors[:, 1], c=lab, cmap=cmap)
+    plt.scatter(code_vectors[:, 0], code_vectors[:, 1], c=lab, cmap=cmap, alpha=alpha)
     plt.colorbar()
     plt.grid()
     plt.savefig("{0}".format(plot_fname), dpi=300)
     plt.clf()
```

### Comparing `ngclearn-1.0b3/ngclearn/utils/viz/raster.py` & `ngclearn-1.0b4/ngclearn/utils/viz/raster.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/viz/spike_plot.py` & `ngclearn-1.0b4/ngclearn/utils/viz/spike_plot.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b3/ngclearn/utils/viz/synapse_plot.py` & `ngclearn-1.0b4/ngclearn/utils/viz/synapse_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
             plt.subplot(n_rows_total, n_cols_total, point)
             filter = T[i, :]
             plt.imshow(np.reshape(filter, (sizes[idx][0], sizes[idx][1])), cmap=plt.cm.bone, interpolation='nearest')
             plt.axis("off")
 
     plt.subplots_adjust(top=0.9)
     plt.savefig(prefix+suffix, bbox_inches='tight')
+    plt.clf()
     plt.close()
 
 def visualize_labels(thetas, sizes, prefix, space_width=None, widths=None, suffix='.jpg'):
     """
 
     Args:
         thetas:
```

### Comparing `ngclearn-1.0b3/ngclearn.egg-info/PKG-INFO` & `ngclearn-1.0b4/ngclearn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngclearn
-Version: 1.0b3
+Version: 1.0b4
 Summary: Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems.
 Author-email: Alexander Ororbia <ago@cs.rit.edu>, William Gebhardt <wdg1351@rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-learn
 Project-URL: Documentation, https://ngc-learn.readthedocs.io/
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/main/history.txt
@@ -48,16 +48,16 @@
 
 It is currently maintained by the
 <a href="https://www.cs.rit.edu/~ago/nac_lab.html">Neural Adaptive Computing (NAC) laboratory</a>.
 
 ## <b>Documentation</b>
 
 Official documentation, including tutorials, can be found
-<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo, 
-which implements several historical models, can be found 
+<a href="https://ngc-learn.readthedocs.io/en/latest/#">here</a>. The model museum repo,
+which implements several historical models, can be found
 <a href="https://github.com/NACLab/ngc-museum">here</a>.
 
 The official blog-post related to the source paper behind this software library
 can be found
 <a href="https://go.nature.com/3rgl1K8">here</a>.<br>
 You can find the related paper <a href="https://www.nature.com/articles/s41467-022-29632-7">right here</a>, which
 was selected to appear in the Nature <i>Neuromorphic Hardware and Computing Collection</i> in 2023 and was
@@ -99,38 +99,27 @@
 $ pip install ngclearn
 </pre>
 
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
-<!--
-<i>Setup:</i> To install ngc-learn, you can run (at the top-level of the
-the <code>ngclearn</code> directory) the following bash command:
-<pre>
-$ python install .
-</pre>
-
-Running the above pip install will automatically install the CPU
-version of JAX. If you want to use the GPU version instead, make sure to,
-before running the above, to install JAX via the correct pip command
-with the proper CUDA flags (depending on which CUDA is configured for your system)
-as per their
-<a href="https://jax.readthedocs.io/en/latest/installation.html">installation instructions</a>.
--->
-
-<!--
-(If you want to set up/install dependencies a priori, try running
-`$ pip install -r requirements.txt` first before pip installing ngc-learn.)
--->
-
 If the installation was successful, you should see the following if you test
 it against your Python interpreter, i.e., run the <code>$ python</code> command
-and complete the following sequence of steps as depicted in the screenshot below:<br>
-<img src="docs/images/test_ngclearn_install.png" width="512">
+and complete the following sequence of steps as depicted in the screenshot below
+(you should see at the bottom of your output something akin to the
+right major and minor version of ngc-learn):
+
+```console
+Python 3.11.4 (main, MONTH  DAY YEAR, TIME) [GCC XX.X.X] on linux
+Type "help", "copyright", "credits" or "license" for more information.
+>>> import ngclearn
+>>> ngclearn.__version__
+'1.0b3'
+```
 
 <i>Note:</i> For access to the previous Tensorflow-2 version of ngc-learn (of
 which we no longer support), please visit the repo for
 <a href="https://github.com/NACLab/ngc-learn-legacy"><i>ngc-learn-legacy</i></a>.
 
 ## <b>Attribution:</b>
 
@@ -168,15 +157,15 @@
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 <pre>
 $ python install -e .
 </pre>
 
 **Version:**<br>
-1.0.3-Beta <!-- -Alpha -->
+1.0.4-Beta <!-- -Alpha -->
 
 Author:
 Alexander G. Ororbia II<br>
 Director, Neural Adaptive Computing (NAC) Laboratory<br>
 Rochester Institute of Technology, Department of Computer Science
 
 ## <b>Copyright:</b>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngclearn Version: 1.0b3 Summary: Simulation
+Metadata-Version: 2.1 Name: ngclearn Version: 1.0b4 Summary: Simulation
 software for building and analyzing arbitrary predictive coding, spiking
 network, and biomimetic neural systems. Author-email: Alexander Ororbia
 cs.rit.edu>, William Gebhardt
 rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-learn Project-URL: Documentation, https://ngc-
 learn.readthedocs.io/ Project-URL: Lab Page, https://www.cs.rit.edu/~ago/
 nac_lab.html Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/
@@ -55,20 +55,23 @@
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
 learn (CPU version) is through pip:
 $ pip install ngclearn
 The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
 this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
 20.04. If the installation was successful, you should see the following if you
 test it against your Python interpreter, i.e., run the $ python command and
-complete the following sequence of steps as depicted in the screenshot below:
-[docs/images/test_ngclearn_install.png]Note: For access to the previous
-Tensorflow-2 version of ngc-learn (of which we no longer support), please visit
-the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you use this code in any form
-in your project(s), please cite its source paper (as well as ngc-learn's
-official software citation):
+complete the following sequence of steps as depicted in the screenshot below
+(you should see at the bottom of your output something akin to the right major
+and minor version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY
+YEAR, TIME) [GCC XX.X.X] on linux Type "help", "copyright", "credits" or
+"license" for more information. >>> import ngclearn >>> ngclearn.__version__
+'1.0b3' ``` Note: For access to the previous Tensorflow-2 version of ngc-learn
+(of which we no longer support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ##
+AAttttrriibbuuttiioonn:: If you use this code in any form in your project(s), please cite
+its source paper (as well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
   journal={Nature Communications},
   year={2022},
   month={Apr},
   day={19},
@@ -84,15 +87,15 @@
 [contributing guidelines](CONTRIBUTING.md). SSoouurrccee CCooddee You can check/pull the
 latest source code for this library via:
 $ git clone https://github.com/NACLab/ngc-learn.git
 If you are working on and developing with ngc-learn pulled from the github
 repo, then run the following command to set up an editable install:
 $ python install -e .
 **Version:**
-1.0.3-Beta Author: Alexander G. Ororbia II
+1.0.4-Beta Author: Alexander G. Ororbia II
 Director, Neural Adaptive Computing (NAC) Laboratory
 Rochester Institute of Technology, Department of Computer Science ## CCooppyyrriigghhtt::
 Copyright (C) 2021 The Neural Adaptive Computing Laboratory - All Rights
 Reserved
 You may use, distribute and modify this code under the terms of the BSD 3-
 clause license. You should have received a copy of the BSD 3-clause license
 with this software.
```

### Comparing `ngclearn-1.0b3/ngclearn.egg-info/SOURCES.txt` & `ngclearn-1.0b4/ngclearn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 AUTHORS
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
+UPDATED_cells/LIFCell.py
+UPDATED_cells/older_sLIF.py
 ngclearn/__init__.py
 ngclearn.egg-info/PKG-INFO
 ngclearn.egg-info/SOURCES.txt
 ngclearn.egg-info/dependency_links.txt
 ngclearn.egg-info/requires.txt
 ngclearn.egg-info/top_level.txt
 ngclearn/commands/__init__.py
@@ -42,14 +44,15 @@
 ngclearn/utils/metric_utils.py
 ngclearn/utils/model_utils.py
 ngclearn/utils/patch_utils.py
 ngclearn/utils/surrogate_fx.py
 ngclearn/utils/density/__init__.py
 ngclearn/utils/density/gmm.py
 ngclearn/utils/diffeq/__init__.py
+ngclearn/utils/diffeq/_ode_utils.py
 ngclearn/utils/diffeq/ode_utils.py
 ngclearn/utils/optim/__init__.py
 ngclearn/utils/optim/adam.py
 ngclearn/utils/optim/opt.py
 ngclearn/utils/optim/sgd.py
 ngclearn/utils/viz/__init__.py
 ngclearn/utils/viz/dim_reduce.py
```

### Comparing `ngclearn-1.0b3/pyproject.toml` & `ngclearn-1.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ngclearn"
-version = "1.0.beta3"
+version = "1.0.beta4"
 description = "Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems."
 authors = [
   {name = "Alexander Ororbia", email = "ago@cs.rit.edu"},
   {name = "William Gebhardt", email = "wdg1351@rit.edu"},
 ]
 readme = "README.md"
 keywords = ['python', 'ngc-learn', 'predictive-processing', 'predictive-coding',
```

