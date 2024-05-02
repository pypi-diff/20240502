# Comparing `tmp/nodespecs-0.0.8.tar.gz` & `tmp/nodespecs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodespecs-0.0.8.tar", last modified: Wed May  1 16:27:48 2024, max compression
+gzip compressed data, was "nodespecs-0.0.9.tar", last modified: Wed May  1 18:32:46 2024, max compression
```

## Comparing `nodespecs-0.0.8.tar` & `nodespecs-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.848773 nodespecs-0.0.8/
--rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     7653 2024-05-01 16:27:48.845782 nodespecs-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5756 2024-05-01 15:19:14.000000 nodespecs-0.0.8/README.md
--rw-rw-rw-   0        0        0      902 2024-05-01 15:31:23.000000 nodespecs-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 16:27:48.848773 nodespecs-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.802201 nodespecs-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.843785 nodespecs-0.0.8/src/nodespecs.egg-info/
--rw-rw-rw-   0        0        0     7653 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.835817 nodespecs-0.0.8/src/specs/
--rw-rw-rw-   0        0        0      210 2024-05-01 15:49:09.000000 nodespecs-0.0.8/src/specs/__init__.py
--rw-rw-rw-   0        0        0      777 2024-05-01 16:26:19.000000 nodespecs-0.0.8/src/specs/__main__.py
--rw-rw-rw-   0        0        0     1545 2024-05-01 16:16:52.000000 nodespecs-0.0.8/src/specs/benchmark.py
--rw-rw-rw-   0        0        0      488 2024-04-23 20:58:02.000000 nodespecs-0.0.8/src/specs/cmd.py
-drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.840799 nodespecs-0.0.8/src/specs/communicate/
--rw-rw-rw-   0        0        0    17137 2024-05-01 15:19:14.000000 nodespecs-0.0.8/src/specs/communicate/pp.py
--rw-rw-rw-   0        0        0     2783 2024-05-01 15:44:00.000000 nodespecs-0.0.8/src/specs/communicate/tcpsocket.py
--rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.8/src/specs/cpuinfo.py
--rw-rw-rw-   0        0        0     7675 2024-05-01 16:16:25.000000 nodespecs-0.0.8/src/specs/hardware.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:32:46.293640 nodespecs-0.0.9/
+-rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     8450 2024-05-01 18:32:46.292200 nodespecs-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6553 2024-05-01 18:27:01.000000 nodespecs-0.0.9/README.md
+-rw-rw-rw-   0        0        0      902 2024-05-01 18:23:46.000000 nodespecs-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 18:32:46.293640 nodespecs-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 18:32:46.243442 nodespecs-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 18:32:46.289210 nodespecs-0.0.9/src/nodespecs.egg-info/
+-rw-rw-rw-   0        0        0     8450 2024-05-01 18:32:46.000000 nodespecs-0.0.9/src/nodespecs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-05-01 18:32:46.000000 nodespecs-0.0.9/src/nodespecs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 18:32:46.000000 nodespecs-0.0.9/src/nodespecs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-01 18:32:46.000000 nodespecs-0.0.9/src/nodespecs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-05-01 18:32:46.000000 nodespecs-0.0.9/src/nodespecs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-01 18:32:46.000000 nodespecs-0.0.9/src/nodespecs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 18:32:46.281618 nodespecs-0.0.9/src/specs/
+-rw-rw-rw-   0        0        0      162 2024-05-01 18:23:59.000000 nodespecs-0.0.9/src/specs/__init__.py
+-rw-rw-rw-   0        0        0      949 2024-05-01 18:29:48.000000 nodespecs-0.0.9/src/specs/__main__.py
+-rw-rw-rw-   0        0        0     1661 2024-05-01 18:30:48.000000 nodespecs-0.0.9/src/specs/benchmark.py
+-rw-rw-rw-   0        0        0      623 2024-05-01 17:30:24.000000 nodespecs-0.0.9/src/specs/cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:32:46.286218 nodespecs-0.0.9/src/specs/communicate/
+-rw-rw-rw-   0        0        0    17137 2024-05-01 15:19:14.000000 nodespecs-0.0.9/src/specs/communicate/pp.py
+-rw-rw-rw-   0        0        0     2783 2024-05-01 15:44:00.000000 nodespecs-0.0.9/src/specs/communicate/tcpsocket.py
+-rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.9/src/specs/cpuinfo.py
+-rw-rw-rw-   0        0        0     7675 2024-05-01 16:16:25.000000 nodespecs-0.0.9/src/specs/hardware.py
```

### Comparing `nodespecs-0.0.8/LICENSE` & `nodespecs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.8/PKG-INFO` & `nodespecs-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.8
+Version: 0.0.9
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -37,14 +37,21 @@
 pip install nodespecs
 python -m specs
 python -c "import specs; specs.bench_cpu()"
 python -c "import specs; specs.info_gpu()"
 ```
 
 ```shell
+# for the machine not compatible with psutil
+python -m specs -l=1
+
+python -m specs -u="bcpu"
+```
+
+```shell
 ## server
 python -c "import specs; specs.server()"
 
 ## client upload wt progress bar
 python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
 
 ## client upload wo progress bar
@@ -87,47 +94,58 @@
 sudo apt install python3-pip
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
-| Nickname                      | CPU                                            | Arch   | OS            | Benchmarking | Comb                                                         | Score |
-| ----------------------------- | ---------------------------------------------- | ------ | ------------- | ------------ | ------------------------------------------------------------ | ----- |
-| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
-| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
-| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
-| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
-| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
-| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
-| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
-| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64 | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
-| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
-| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
-| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux         | 43.078       |                                                              |       |
-| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux         | 49.396       |                                                              |       |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows       | 62.969       |                                                              |       |
-| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
-| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64 | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
-
-### GPU collection
+| Nickname                      | CPU                                            | Arch    | OS            | Benchmarking | Comb                                                         | Score |
+| ----------------------------- | ---------------------------------------------- | ------- | ------------- | ------------ | ------------------------------------------------------------ | ----- |
+| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64   | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
+| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64   | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
+| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64   | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
+| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64   | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
+| oracle cloudshell             | ARM Cortex-A53                                 | aarch64 | Linux         | 27.489       |                                                              |       |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64  | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
+| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64  | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
+| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64   | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
+| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64  | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64  | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
+| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64   | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
+| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64  | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
+| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64  | Linux         | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64  | Linux         | 49.396       |                                                              |       |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64   | Windows       | 62.969       |                                                              |       |
+| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64  | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
+| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64  | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
 
+* Note
+  * Kinds of Arch explanation[^1] 
 
+### GPU collection
 
 | id    | name                    | total memory | Synthetic benchmark | CUDA API |
 | ----- | ----------------------- | ------------ | ------------------- | -------- |
 | 17    | NVIDIA GeForce RTX 4060 | 8188.0MB     | 50.69               | NA       |
 | colab | Tesla T4                | 15360.0MB    | 28.16               | 70627    |
 | dell  | NVIDIA T600 Laptop GPU  | 4096.0MB     | 16.69               | 26600    |
 | 01    | Quadro M4000            | 8192.0MB     | 17.27               | 16648    |
 
 
 
 
+## Feature in develop
+1. Streaming upload server in Python extended from [uploadserver](https://github.com/Densaugeo/uploadserver).
+2. [py-ios-device](https://github.com/YueChen-C/py-ios-device) python based Apple instruments protocol，you can get CPU, Memory and other metrics from real iOS devices
+
+
+
+
 
 Performance source
 
 * https://browser.geekbench.com/
   * 
 * https://technical.city/en/video/GeForce-RTX-4060-vs-Tesla-T4
 * https://technical.city/en/video/Tesla-T4-vs-T600
+
+[^1]: [mainstream CPU architecture](https://jinsanity07git.github.io/post/mainstream%20CPU%20architecture.html)
```

### Comparing `nodespecs-0.0.8/README.md` & `nodespecs-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 pip install nodespecs
 python -m specs
 python -c "import specs; specs.bench_cpu()"
 python -c "import specs; specs.info_gpu()"
 ```
 
 ```shell
+# for the machine not compatible with psutil
+python -m specs -l=1
+
+python -m specs -u="bcpu"
+```
+
+```shell
 ## server
 python -c "import specs; specs.server()"
 
 ## client upload wt progress bar
 python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
 
 ## client upload wo progress bar
@@ -59,47 +66,58 @@
 sudo apt install python3-pip
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
-| Nickname                      | CPU                                            | Arch   | OS            | Benchmarking | Comb                                                         | Score |
-| ----------------------------- | ---------------------------------------------- | ------ | ------------- | ------------ | ------------------------------------------------------------ | ----- |
-| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
-| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
-| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
-| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
-| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
-| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
-| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
-| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64 | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
-| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
-| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
-| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux         | 43.078       |                                                              |       |
-| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux         | 49.396       |                                                              |       |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows       | 62.969       |                                                              |       |
-| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
-| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64 | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
-
-### GPU collection
+| Nickname                      | CPU                                            | Arch    | OS            | Benchmarking | Comb                                                         | Score |
+| ----------------------------- | ---------------------------------------------- | ------- | ------------- | ------------ | ------------------------------------------------------------ | ----- |
+| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64   | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
+| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64   | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
+| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64   | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
+| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64   | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
+| oracle cloudshell             | ARM Cortex-A53                                 | aarch64 | Linux         | 27.489       |                                                              |       |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64  | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
+| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64  | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
+| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64   | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
+| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64  | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64  | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
+| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64   | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
+| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64  | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
+| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64  | Linux         | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64  | Linux         | 49.396       |                                                              |       |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64   | Windows       | 62.969       |                                                              |       |
+| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64  | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
+| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64  | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
 
+* Note
+  * Kinds of Arch explanation[^1] 
 
+### GPU collection
 
 | id    | name                    | total memory | Synthetic benchmark | CUDA API |
 | ----- | ----------------------- | ------------ | ------------------- | -------- |
 | 17    | NVIDIA GeForce RTX 4060 | 8188.0MB     | 50.69               | NA       |
 | colab | Tesla T4                | 15360.0MB    | 28.16               | 70627    |
 | dell  | NVIDIA T600 Laptop GPU  | 4096.0MB     | 16.69               | 26600    |
 | 01    | Quadro M4000            | 8192.0MB     | 17.27               | 16648    |
 
 
 
 
+## Feature in develop
+1. Streaming upload server in Python extended from [uploadserver](https://github.com/Densaugeo/uploadserver).
+2. [py-ios-device](https://github.com/YueChen-C/py-ios-device) python based Apple instruments protocol，you can get CPU, Memory and other metrics from real iOS devices
+
+
+
+
 
 Performance source
 
 * https://browser.geekbench.com/
   * 
 * https://technical.city/en/video/GeForce-RTX-4060-vs-Tesla-T4
 * https://technical.city/en/video/Tesla-T4-vs-T600
+
+[^1]: [mainstream CPU architecture](https://jinsanity07git.github.io/post/mainstream%20CPU%20architecture.html)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nodespecs-0.0.8/pyproject.toml` & `nodespecs-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodespecs"
-version = "0.0.8"
+version = "0.0.9"
 description = "The specs summarize utilities for computer instance"
 readme = "README.md"
 authors = [{ name = "jinsanity", email = "jinsanityff@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodespecs-0.0.8/src/nodespecs.egg-info/PKG-INFO` & `nodespecs-0.0.9/src/nodespecs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.8
+Version: 0.0.9
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -37,14 +37,21 @@
 pip install nodespecs
 python -m specs
 python -c "import specs; specs.bench_cpu()"
 python -c "import specs; specs.info_gpu()"
 ```
 
 ```shell
+# for the machine not compatible with psutil
+python -m specs -l=1
+
+python -m specs -u="bcpu"
+```
+
+```shell
 ## server
 python -c "import specs; specs.server()"
 
 ## client upload wt progress bar
 python -c "import specs; specs.client('172.25.1.175', 12345,'./README.md',False)"
 
 ## client upload wo progress bar
@@ -87,47 +94,58 @@
 sudo apt install python3-pip
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
-| Nickname                      | CPU                                            | Arch   | OS            | Benchmarking | Comb                                                         | Score |
-| ----------------------------- | ---------------------------------------------- | ------ | ------------- | ------------ | ------------------------------------------------------------ | ----- |
-| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
-| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
-| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
-| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
-| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
-| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
-| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
-| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64 | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
-| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
-| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
-| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux         | 43.078       |                                                              |       |
-| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux         | 49.396       |                                                              |       |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows       | 62.969       |                                                              |       |
-| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
-| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64 | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
-
-### GPU collection
+| Nickname                      | CPU                                            | Arch    | OS            | Benchmarking | Comb                                                         | Score |
+| ----------------------------- | ---------------------------------------------- | ------- | ------------- | ------------ | ------------------------------------------------------------ | ----- |
+| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64   | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
+| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64   | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
+| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64   | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
+| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64   | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
+| oracle cloudshell             | ARM Cortex-A53                                 | aarch64 | Linux         | 27.489       |                                                              |       |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64  | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
+| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64  | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
+| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64   | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
+| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64  | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64  | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
+| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64   | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
+| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64  | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
+| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64  | Linux         | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64  | Linux         | 49.396       |                                                              |       |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64   | Windows       | 62.969       |                                                              |       |
+| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64  | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
+| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64  | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
 
+* Note
+  * Kinds of Arch explanation[^1] 
 
+### GPU collection
 
 | id    | name                    | total memory | Synthetic benchmark | CUDA API |
 | ----- | ----------------------- | ------------ | ------------------- | -------- |
 | 17    | NVIDIA GeForce RTX 4060 | 8188.0MB     | 50.69               | NA       |
 | colab | Tesla T4                | 15360.0MB    | 28.16               | 70627    |
 | dell  | NVIDIA T600 Laptop GPU  | 4096.0MB     | 16.69               | 26600    |
 | 01    | Quadro M4000            | 8192.0MB     | 17.27               | 16648    |
 
 
 
 
+## Feature in develop
+1. Streaming upload server in Python extended from [uploadserver](https://github.com/Densaugeo/uploadserver).
+2. [py-ios-device](https://github.com/YueChen-C/py-ios-device) python based Apple instruments protocol，you can get CPU, Memory and other metrics from real iOS devices
+
+
+
+
 
 Performance source
 
 * https://browser.geekbench.com/
   * 
 * https://technical.city/en/video/GeForce-RTX-4060-vs-Tesla-T4
 * https://technical.city/en/video/Tesla-T4-vs-T600
+
+[^1]: [mainstream CPU architecture](https://jinsanity07git.github.io/post/mainstream%20CPU%20architecture.html)
```

### Comparing `nodespecs-0.0.8/src/specs/benchmark.py` & `nodespecs-0.0.9/src/specs/benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 #!/usr/bin/python3
 #Python CPU Benchmark by Alex Dedyura (Windows, macOS, Linux)
 #https://github.com/alexdedyura/cpu-benchmark
 
 import time
 import platform
-from . import cpuinfo
 
 def info_plat():
+  from . import cpuinfo
+  from .hardware import info_sys
   print('CPU: ' + cpuinfo.get_cpu_info().get('brand_raw', "Unknown"))
   print('Arch: ' + cpuinfo.get_cpu_info().get('arch_string_raw', "Unknown"))
   print('OS: ' + platform.system(), platform.release())
   print('Python: ' + platform.python_version())
+  info_sys()
 
 
 def bench_cpu():
   print('Python CPU Benchmark (Windows, macOS(Darwin), Linux)')
-  info_plat()
+  try:
+    info_plat()
+  except Exception as e:
+    print (str(e))
+    pass
   print('\nBenchmarking: \n')
 
   start_benchmark = 10000 # change this if you like (sample: 1000, 5000, etc)
   start_benchmark = int(start_benchmark)
 
   repeat_benchmark = 10 # attemps, change this if you like (sample: 3, 5, etc)
   repeat_benchmark = int(repeat_benchmark)
```

### Comparing `nodespecs-0.0.8/src/specs/communicate/pp.py` & `nodespecs-0.0.9/src/specs/communicate/pp.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.8/src/specs/communicate/tcpsocket.py` & `nodespecs-0.0.9/src/specs/communicate/tcpsocket.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.8/src/specs/cpuinfo.py` & `nodespecs-0.0.9/src/specs/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.8/src/specs/hardware.py` & `nodespecs-0.0.9/src/specs/hardware.py`

 * *Files identical despite different names*

