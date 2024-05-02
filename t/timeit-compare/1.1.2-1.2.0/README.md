# Comparing `tmp/timeit_compare-1.1.2.tar.gz` & `tmp/timeit_compare-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeit_compare-1.1.2.tar", last modified: Mon Apr 22 15:18:03 2024, max compression
+gzip compressed data, was "timeit_compare-1.2.0.tar", last modified: Thu May  2 15:07:03 2024, max compression
```

## Comparing `timeit_compare-1.1.2.tar` & `timeit_compare-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 15:18:03.470808 timeit_compare-1.1.2/
--rw-rw-rw-   0        0        0     1089 2024-04-13 14:44:22.000000 timeit_compare-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     4456 2024-04-22 15:18:03.470808 timeit_compare-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3515 2024-04-22 14:46:46.000000 timeit_compare-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 15:18:03.470808 timeit_compare-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1224 2024-04-22 14:49:40.000000 timeit_compare-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:18:03.470808 timeit_compare-1.1.2/timeit_compare.egg-info/
--rw-rw-rw-   0        0        0     4456 2024-04-22 15:18:03.000000 timeit_compare-1.1.2/timeit_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-04-22 15:18:03.000000 timeit_compare-1.1.2/timeit_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 15:18:03.000000 timeit_compare-1.1.2/timeit_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-22 15:18:03.000000 timeit_compare-1.1.2/timeit_compare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17834 2024-04-22 13:54:40.000000 timeit_compare-1.1.2/timeit_compare.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:07:03.304433 timeit_compare-1.2.0/
+-rw-rw-rw-   0        0        0     1089 2024-04-13 14:44:22.000000 timeit_compare-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3916 2024-05-02 15:07:03.303054 timeit_compare-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2024-05-02 10:48:47.000000 timeit_compare-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 15:07:03.304433 timeit_compare-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1248 2024-04-29 17:34:19.000000 timeit_compare-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:07:03.301429 timeit_compare-1.2.0/timeit_compare.egg-info/
+-rw-rw-rw-   0        0        0     3916 2024-05-02 15:07:03.000000 timeit_compare-1.2.0/timeit_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-05-02 15:07:03.000000 timeit_compare-1.2.0/timeit_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 15:07:03.000000 timeit_compare-1.2.0/timeit_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-02 15:07:03.000000 timeit_compare-1.2.0/timeit_compare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25810 2024-05-02 11:05:39.000000 timeit_compare-1.2.0/timeit_compare.py
```

### Comparing `timeit_compare-1.1.2/LICENSE` & `timeit_compare-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeit_compare-1.1.2/PKG-INFO` & `timeit_compare-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: timeit_compare
-Version: 1.1.2
-Summary: A method based on timeit that can help you to call timeit.timeit for several statements and provide comparison results.
+Version: 1.2.0
+Summary: Based on the timeit library, timeit_compare can time multiple statements and provide comparison results.
 Home-page: https://github.com/AomandeNiuma/timeit_compare
 Author: Liu Wei
 Author-email: 23S112099@stu.hit.edu.cn
 Maintainer: Liu Wei
 Maintainer-email: 23S112099@stu.hit.edu.cn
 License: MIT
+Keywords: timeit_compare,timeit,performance
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,22 +20,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # timeit_compare
 
-A method based on timeit that can help you to call timeit.timeit for several
-statements and provide comparison results.
+Based on the timeit library, timeit_compare can time multiple statements and 
+provide comparison results.
 
 ------------------------------
 
 ## Installation
 
-You can run the following command to install the package
+You can run the following command to install the package.
 
 ```commandline
 pip install timeit_compare
 ```
 
 ------------------------------
 
@@ -93,69 +94,56 @@
 
 [![output_example.png](https://raw.githubusercontent.com/AomandeNiuma/timeit_compare/main/output_example.png)](
 https://raw.githubusercontent.com/AomandeNiuma/timeit_compare/main/output_example.png)
 
 The output provides detailed results, including the mean, median, minimum,
 maximum and standard deviation of each function's running time.
 
-------------------------------
+You can also perform the following operations to obtain specific values:
+
+```python
+from timeit_compare import Compare
+
+cmp = Compare()
+for func in sum1, sum2, sum3, sum4, sum5:
+    cmp.add_timer(func)
+cmp.run()
+# cmp.print_results()
+
+result = cmp.get_result(0)  # get the result of the timer with index 0
+print(
+    result.time, result.repeat, result.number,
+    result.mean, result.median, result.min, result.max, result.std,
+    result.error, sep='\n'
+)
+# [3.3324892420678126e-06, 3.175742677501652e-06, 3.2153616044376503e-06, 3.267199346172507e-06, 3.2638434747711383e-06]
+# 5
+# 24405
+# 3.2509272689901518e-06
+# 3.2638434747711383e-06
+# 3.175742677501652e-06
+# 3.3324892420678126e-06
+# 5.916418598334957e-08
+# None
+
+fastest = cmp.get_fastest()  # get the result of the fastest timer
+print(fastest.index)  # 4
+```
 
-## Release Notes
+In a command line interface, call as follows:
 
-### Release 1.1.0
+```commandline
+python -m timeit_compare -s "n = 100" "s = 0;for i in range(1, n + 1):;    s += i" "sum(range(1, n + 1))" "(1 + n) * n // 2"
+```
 
-1. The results now show the time of one loop in seconds(s), milliseconds(ms),
-   microseconds(μs), or nanoseconds(ns) instead of the total time of each
-   repetition. The conversion relationship among time units is as follows:
-
-   ```
-   1(s) = 10^3(ms) = 10^6(μs) = 10^9(ns)
-   ```
-
-2. Now the compare function supports setting parameters setup and globals
-   separately for each statement. Keyword parameters setup and globals are
-   now used to set the default parameter values for each statement.
-
-   ```python
-   from timeit_compare import compare
-   
-   stmt = '(1 + n) * n // 2'
-   compare(
-       stmt,
-       (stmt, 'n = 100', {}),
-       (stmt, '', {'n': 100}),
-       setup='n = 100'
-   )
-   ```
-
-3. If parameter number is not given or is less than or equal to 0, it now
-   defaults to a value that makes the total running time not too long. You can
-   intentionally set it to a higher value to make the results more accurate.
-
-4. Command line calls are now supported.
-
-   ```commandline
-   python -m timeit_compare -s "n = 100" "(1 + n) * n / 2" "sum(range(1, n + 1))"
-   ```
-
-   Run the following command for help.
-
-   ```commandline
-   python -m timeit_compare -h
-   ```
-
-### Release 1.1.2
-
-1. Added a parameter: time, which represents approximate total running time of
-   all statements in seconds (default 1.0). When a positive value of number
-   parameter is not given, it will be used to estimate number. Ignored when
-   number is greater than 0.
+Run the following command for help:
 
-2. Corrected the error of representing sample standard deviation as population
-   standard deviation.
+```commandline
+python -m timeit_compare -h
+```
 
 ------------------------------
 
 ## Contact
 
 If you have any suggestions, please contact me at
 [23S112099@stu.hit.edu.cn](mailto:23S112099@stu.hit.edu.cn).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `timeit_compare-1.1.2/setup.py` & `timeit_compare-1.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='timeit_compare',
-    version='1.1.2',
+    version='1.2.0',
     py_modules=['timeit_compare'],
     license='MIT',
     python_requires='>=3.6.0',
-    description='A method based on timeit that can help you to call '
-                'timeit.timeit for several statements and provide '
-                'comparison results.',
+    description='Based on the timeit library, timeit_compare can time multiple '
+                'statements and provide comparison results.',
     long_description=long_description,
     long_description_content_type='text/markdown',
+    keywords=['timeit_compare', 'timeit', 'performance'],
     author='Liu Wei',
     author_email='23S112099@stu.hit.edu.cn',
     maintainer='Liu Wei',
     maintainer_email='23S112099@stu.hit.edu.cn',
     url='https://github.com/AomandeNiuma/timeit_compare',
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

### Comparing `timeit_compare-1.1.2/timeit_compare.egg-info/PKG-INFO` & `timeit_compare-1.2.0/timeit_compare.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: timeit_compare
-Version: 1.1.2
-Summary: A method based on timeit that can help you to call timeit.timeit for several statements and provide comparison results.
+Version: 1.2.0
+Summary: Based on the timeit library, timeit_compare can time multiple statements and provide comparison results.
 Home-page: https://github.com/AomandeNiuma/timeit_compare
 Author: Liu Wei
 Author-email: 23S112099@stu.hit.edu.cn
 Maintainer: Liu Wei
 Maintainer-email: 23S112099@stu.hit.edu.cn
 License: MIT
+Keywords: timeit_compare,timeit,performance
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,22 +20,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # timeit_compare
 
-A method based on timeit that can help you to call timeit.timeit for several
-statements and provide comparison results.
+Based on the timeit library, timeit_compare can time multiple statements and 
+provide comparison results.
 
 ------------------------------
 
 ## Installation
 
-You can run the following command to install the package
+You can run the following command to install the package.
 
 ```commandline
 pip install timeit_compare
 ```
 
 ------------------------------
 
@@ -93,69 +94,56 @@
 
 [![output_example.png](https://raw.githubusercontent.com/AomandeNiuma/timeit_compare/main/output_example.png)](
 https://raw.githubusercontent.com/AomandeNiuma/timeit_compare/main/output_example.png)
 
 The output provides detailed results, including the mean, median, minimum,
 maximum and standard deviation of each function's running time.
 
-------------------------------
+You can also perform the following operations to obtain specific values:
+
+```python
+from timeit_compare import Compare
+
+cmp = Compare()
+for func in sum1, sum2, sum3, sum4, sum5:
+    cmp.add_timer(func)
+cmp.run()
+# cmp.print_results()
+
+result = cmp.get_result(0)  # get the result of the timer with index 0
+print(
+    result.time, result.repeat, result.number,
+    result.mean, result.median, result.min, result.max, result.std,
+    result.error, sep='\n'
+)
+# [3.3324892420678126e-06, 3.175742677501652e-06, 3.2153616044376503e-06, 3.267199346172507e-06, 3.2638434747711383e-06]
+# 5
+# 24405
+# 3.2509272689901518e-06
+# 3.2638434747711383e-06
+# 3.175742677501652e-06
+# 3.3324892420678126e-06
+# 5.916418598334957e-08
+# None
+
+fastest = cmp.get_fastest()  # get the result of the fastest timer
+print(fastest.index)  # 4
+```
 
-## Release Notes
+In a command line interface, call as follows:
 
-### Release 1.1.0
+```commandline
+python -m timeit_compare -s "n = 100" "s = 0;for i in range(1, n + 1):;    s += i" "sum(range(1, n + 1))" "(1 + n) * n // 2"
+```
 
-1. The results now show the time of one loop in seconds(s), milliseconds(ms),
-   microseconds(μs), or nanoseconds(ns) instead of the total time of each
-   repetition. The conversion relationship among time units is as follows:
-
-   ```
-   1(s) = 10^3(ms) = 10^6(μs) = 10^9(ns)
-   ```
-
-2. Now the compare function supports setting parameters setup and globals
-   separately for each statement. Keyword parameters setup and globals are
-   now used to set the default parameter values for each statement.
-
-   ```python
-   from timeit_compare import compare
-   
-   stmt = '(1 + n) * n // 2'
-   compare(
-       stmt,
-       (stmt, 'n = 100', {}),
-       (stmt, '', {'n': 100}),
-       setup='n = 100'
-   )
-   ```
-
-3. If parameter number is not given or is less than or equal to 0, it now
-   defaults to a value that makes the total running time not too long. You can
-   intentionally set it to a higher value to make the results more accurate.
-
-4. Command line calls are now supported.
-
-   ```commandline
-   python -m timeit_compare -s "n = 100" "(1 + n) * n / 2" "sum(range(1, n + 1))"
-   ```
-
-   Run the following command for help.
-
-   ```commandline
-   python -m timeit_compare -h
-   ```
-
-### Release 1.1.2
-
-1. Added a parameter: time, which represents approximate total running time of
-   all statements in seconds (default 1.0). When a positive value of number
-   parameter is not given, it will be used to estimate number. Ignored when
-   number is greater than 0.
+Run the following command for help:
 
-2. Corrected the error of representing sample standard deviation as population
-   standard deviation.
+```commandline
+python -m timeit_compare -h
+```
 
 ------------------------------
 
 ## Contact
 
 If you have any suggestions, please contact me at
 [23S112099@stu.hit.edu.cn](mailto:23S112099@stu.hit.edu.cn).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

