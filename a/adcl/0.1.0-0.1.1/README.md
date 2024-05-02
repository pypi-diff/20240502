# Comparing `tmp/adcl-0.1.0.tar.gz` & `tmp/adcl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adcl-0.1.0.tar", last modified: Wed May  1 19:54:24 2024, max compression
+gzip compressed data, was "dist\adcl-0.1.1.tar", last modified: Thu May  2 06:39:41 2024, max compression
```

## Comparing `adcl-0.1.0.tar` & `adcl-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 19:54:24.570275 adcl-0.1.0/
--rw-rw-rw-   0        0        0     4754 2024-05-01 19:54:24.569305 adcl-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3688 2024-05-01 19:45:38.000000 adcl-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 19:54:24.568280 adcl-0.1.0/adcl.egg-info/
--rw-rw-rw-   0        0        0     4754 2024-05-01 19:54:24.000000 adcl-0.1.0/adcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2024-05-01 19:54:24.000000 adcl-0.1.0/adcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 19:54:24.000000 adcl-0.1.0/adcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      245 2024-05-01 19:54:24.000000 adcl-0.1.0/adcl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 19:54:24.000000 adcl-0.1.0/adcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 19:54:24.570275 adcl-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      759 2024-05-01 19:52:29.000000 adcl-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:39:41.000000 adcl-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-05-01 20:17:28.000000 adcl-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4292 2024-05-02 06:39:41.000000 adcl-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3754 2024-05-01 20:17:28.000000 adcl-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 06:39:41.000000 adcl-0.1.1/adcl/
+-rw-rw-rw-   0        0        0       35 2024-05-01 20:17:28.000000 adcl-0.1.1/adcl/__init__.py
+-rw-rw-rw-   0        0        0    53906 2024-05-01 20:17:28.000000 adcl-0.1.1/adcl/data_preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:39:41.000000 adcl-0.1.1/adcl.egg-info/
+-rw-rw-rw-   0        0        0     4292 2024-05-02 06:39:41.000000 adcl-0.1.1/adcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-02 06:39:41.000000 adcl-0.1.1/adcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 06:39:41.000000 adcl-0.1.1/adcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      233 2024-05-02 06:39:41.000000 adcl-0.1.1/adcl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-02 06:39:41.000000 adcl-0.1.1/adcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 06:39:41.000000 adcl-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      759 2024-05-02 06:32:22.000000 adcl-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `adcl-0.1.0/PKG-INFO` & `adcl-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,21 @@
 Metadata-Version: 2.1
 Name: adcl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data preprocessing and cleaning tools for data science projects
 Home-page: https://github.com/maykov-stepan/ADCL-Automatic-Data-Cleaning
 Author: Maykov Stepan
 Author-email: steve19992@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: python==3.7
-Requires-Dist: numpy==1.21.6
-Requires-Dist: pandas==1.3.5
-Requires-Dist: tensorflow==2.11.0
-Requires-Dist: mxnet==1.4.0
-Requires-Dist: openml==0.14.1
-Requires-Dist: scipy==1.5.4
-Requires-Dist: dtaidistance==2.3.11
-Requires-Dist: matrixprofile==1.1.10
-Requires-Dist: datawig==0.2.0
-Requires-Dist: pyod==1.1.3
-Requires-Dist: adtk==0.6.2
-Requires-Dist: scikit-learn==1.0.2
-Requires-Dist: matplotlib==3.5.3
-Requires-Dist: category-encoders==2.6.3
+License-File: LICENSE
 
 # README for ADCL-Automatic-Data-Cleaning Project
 
 ## Overview
 ADCL-Automatic-Data-Cleaning is a Python package designed to facilitate automated data cleaning, particularly leveraging deep learning techniques. This project focuses on improving accuracy and efficiency in preprocessing tasks essential for data science and machine learning workflows.
 
 ## Features
```

### Comparing `adcl-0.1.0/README.md` & `adcl-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# README for ADCL-Automatic-Data-Cleaning Project
-
-## Overview
-ADCL-Automatic-Data-Cleaning is a Python package designed to facilitate automated data cleaning, particularly leveraging deep learning techniques. This project focuses on improving accuracy and efficiency in preprocessing tasks essential for data science and machine learning workflows.
-
-## Features
-- **Data Preprocessing:** Standardize, normalize, and format your data for machine learning models.
-- **Missing Value Imputation:** Implements various techniques for handling missing data in both cross-sectional and time-series datasets.
-- **Outlier Detection:** Identifies and manages outliers using multiple strategies, improving the robustness of your models.
-- **Encoding and Transformation:** Converts categorical data into a machine-readable format using various encoding techniques.
-- **Time Series Handling:** Special functions for processing time-dependent data.
-
-## Repository Structure
-- `data_preprocessing/`
-  - **data_preprocessing.py**: Core library file containing all preprocessing functions, including data cleaning, encoding, and preparation.
-- `examples/`
-  - **example_usage.ipynb**: Jupyter notebook demonstrating how to use the preprocessing functions.
-- `missing_values_imputation_test/`
-  - **missing_values_cross_sectional.ipynb**: Notebook for testing missing value imputation in cross-sectional data.
-  - **missing_values_time_series.ipynb**: Notebook for testing missing value imputation in time series data.
-- `cross_miss_results/`: Folder containing the results from the cross-sectional missing value tests.
-- `time_miss_results/`: Folder containing the results from the time series missing value tests.
-- **LICENSE**: The project is open-sourced under the MIT license.
-
-## Installation
-To get started with ADCL, clone this repository and install the required packages:
-
-```bash
-git clone https://github.com/yourgithub/ADCL-Automatic-Data-Cleaning.git
-cd ADCL-Automatic-Data-Cleaning
-pip install -r requirements.txt
-```
-
-## Usage
-### Data Preprocessing
-You can preprocess your datasets by importing functions from `data_preprocessing.py`. For example:
-
-```python
-from data_preprocessing import process_data
-filepath = 'shares_datasets/AAPL.csv'
-df_train, df_test, y_column_name, date_col = process_data(train_input=filepath, test_input=None, separator=',', na_values='?', target_var=None, data_type='time', file_type=None, datetime_col='Date')
-```
-
-### Missing Value Handling
-Handle missing values by choosing an appropriate method from the library. An example usage for time series data:
-
-```python
-from data_preprocessing import missing_values_handling
-X_train_mis, X_test_mis = missing_values_handling(df_train=X_train_enc, df_test=X_test_enc
-                                                  , datetime_col=date_col, imputation_method='auto'
-                                                  , n_steps=10, order=3)
-```
-
-### Example Notebooks
-For the detailed examples, refer to the notebooks in the `examples/` directory. These notebooks provide comprehensive guides on utilizing the package's functionalities effectively.
-
-## Contributing
-Contributions are welcome! If you have suggestions for improving the library, feel free to fork the repository and submit a pull request.
-
-## License
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-## Contact
-For any queries or further information, please contact steve19992@mail.ru.
-
-By providing structured guidance on using the package and clearly explaining what each part of the package does, users of all levels can effectively integrate ADCL into their data cleaning and preprocessing workflows.
+# README for ADCL-Automatic-Data-Cleaning Project
+
+## Overview
+ADCL-Automatic-Data-Cleaning is a Python package designed to facilitate automated data cleaning, particularly leveraging deep learning techniques. This project focuses on improving accuracy and efficiency in preprocessing tasks essential for data science and machine learning workflows.
+
+## Features
+- **Data Preprocessing:** Standardize, normalize, and format your data for machine learning models.
+- **Missing Value Imputation:** Implements various techniques for handling missing data in both cross-sectional and time-series datasets.
+- **Outlier Detection:** Identifies and manages outliers using multiple strategies, improving the robustness of your models.
+- **Encoding and Transformation:** Converts categorical data into a machine-readable format using various encoding techniques.
+- **Time Series Handling:** Special functions for processing time-dependent data.
+
+## Repository Structure
+- `data_preprocessing/`
+  - **data_preprocessing.py**: Core library file containing all preprocessing functions, including data cleaning, encoding, and preparation.
+- `examples/`
+  - **example_usage.ipynb**: Jupyter notebook demonstrating how to use the preprocessing functions.
+- `missing_values_imputation_test/`
+  - **missing_values_cross_sectional.ipynb**: Notebook for testing missing value imputation in cross-sectional data.
+  - **missing_values_time_series.ipynb**: Notebook for testing missing value imputation in time series data.
+- `cross_miss_results/`: Folder containing the results from the cross-sectional missing value tests.
+- `time_miss_results/`: Folder containing the results from the time series missing value tests.
+- **LICENSE**: The project is open-sourced under the MIT license.
+
+## Installation
+To get started with ADCL, clone this repository and install the required packages:
+
+```bash
+git clone https://github.com/yourgithub/ADCL-Automatic-Data-Cleaning.git
+cd ADCL-Automatic-Data-Cleaning
+pip install -r requirements.txt
+```
+
+## Usage
+### Data Preprocessing
+You can preprocess your datasets by importing functions from `data_preprocessing.py`. For example:
+
+```python
+from data_preprocessing import process_data
+filepath = 'shares_datasets/AAPL.csv'
+df_train, df_test, y_column_name, date_col = process_data(train_input=filepath, test_input=None, separator=',', na_values='?', target_var=None, data_type='time', file_type=None, datetime_col='Date')
+```
+
+### Missing Value Handling
+Handle missing values by choosing an appropriate method from the library. An example usage for time series data:
+
+```python
+from data_preprocessing import missing_values_handling
+X_train_mis, X_test_mis = missing_values_handling(df_train=X_train_enc, df_test=X_test_enc
+                                                  , datetime_col=date_col, imputation_method='auto'
+                                                  , n_steps=10, order=3)
+```
+
+### Example Notebooks
+For the detailed examples, refer to the notebooks in the `examples/` directory. These notebooks provide comprehensive guides on utilizing the package's functionalities effectively.
+
+## Contributing
+Contributions are welcome! If you have suggestions for improving the library, feel free to fork the repository and submit a pull request.
+
+## License
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+
+## Contact
+For any queries or further information, please contact steve19992@mail.ru.
+
+By providing structured guidance on using the package and clearly explaining what each part of the package does, users of all levels can effectively integrate ADCL into their data cleaning and preprocessing workflows.
```

### Comparing `adcl-0.1.0/adcl.egg-info/PKG-INFO` & `adcl-0.1.1/adcl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,21 @@
 Metadata-Version: 2.1
 Name: adcl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data preprocessing and cleaning tools for data science projects
 Home-page: https://github.com/maykov-stepan/ADCL-Automatic-Data-Cleaning
 Author: Maykov Stepan
 Author-email: steve19992@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: python==3.7
-Requires-Dist: numpy==1.21.6
-Requires-Dist: pandas==1.3.5
-Requires-Dist: tensorflow==2.11.0
-Requires-Dist: mxnet==1.4.0
-Requires-Dist: openml==0.14.1
-Requires-Dist: scipy==1.5.4
-Requires-Dist: dtaidistance==2.3.11
-Requires-Dist: matrixprofile==1.1.10
-Requires-Dist: datawig==0.2.0
-Requires-Dist: pyod==1.1.3
-Requires-Dist: adtk==0.6.2
-Requires-Dist: scikit-learn==1.0.2
-Requires-Dist: matplotlib==3.5.3
-Requires-Dist: category-encoders==2.6.3
+License-File: LICENSE
 
 # README for ADCL-Automatic-Data-Cleaning Project
 
 ## Overview
 ADCL-Automatic-Data-Cleaning is a Python package designed to facilitate automated data cleaning, particularly leveraging deep learning techniques. This project focuses on improving accuracy and efficiency in preprocessing tasks essential for data science and machine learning workflows.
 
 ## Features
```

### Comparing `adcl-0.1.0/setup.py` & `adcl-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='adcl',
-    version='0.1.0',
+    version='0.1.1',
     author='Maykov Stepan',
     author_email='steve19992@mail.ru',
     description='Data preprocessing and cleaning tools for data science projects',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maykov-stepan/ADCL-Automatic-Data-Cleaning',
     packages=find_packages(),
```

