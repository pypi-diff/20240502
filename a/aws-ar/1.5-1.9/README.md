# Comparing `tmp/aws-ar-1.5.tar.gz` & `tmp/aws-ar-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ar-1.5.tar", last modified: Thu May  2 18:19:09 2024, max compression
+gzip compressed data, was "aws-ar-1.9.tar", last modified: Thu May  2 18:27:08 2024, max compression
```

## Comparing `aws-ar-1.5.tar` & `aws-ar-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:19:09.373436 aws-ar-1.5/
--rw-r--r--   0 shashankdubey   (501) staff       (20)     1716 2024-05-02 18:19:09.373260 aws-ar-1.5/PKG-INFO
--rw-r--r--   0 shashankdubey   (501) staff       (20)     1543 2024-05-02 18:12:31.000000 aws-ar-1.5/README.md
-drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:19:09.372320 aws-ar-1.5/aws_ar/
--rw-r--r--   0 shashankdubey   (501) staff       (20)        0 2024-05-02 13:26:47.000000 aws-ar-1.5/aws_ar/__init__.py
--rw-r--r--   0 shashankdubey   (501) staff       (20)     1652 2024-05-02 15:50:14.000000 aws-ar-1.5/aws_ar/aws_ar.py
-drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:19:09.373061 aws-ar-1.5/aws_ar.egg-info/
--rw-r--r--   0 shashankdubey   (501) staff       (20)     1716 2024-05-02 18:19:09.000000 aws-ar-1.5/aws_ar.egg-info/PKG-INFO
--rw-r--r--   0 shashankdubey   (501) staff       (20)      236 2024-05-02 18:19:09.000000 aws-ar-1.5/aws_ar.egg-info/SOURCES.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)        1 2024-05-02 18:19:09.000000 aws-ar-1.5/aws_ar.egg-info/dependency_links.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)       46 2024-05-02 18:19:09.000000 aws-ar-1.5/aws_ar.egg-info/entry_points.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)        6 2024-05-02 18:19:09.000000 aws-ar-1.5/aws_ar.egg-info/requires.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)        7 2024-05-02 18:19:09.000000 aws-ar-1.5/aws_ar.egg-info/top_level.txt
--rw-r--r--   0 shashankdubey   (501) staff       (20)       38 2024-05-02 18:19:09.373474 aws-ar-1.5/setup.cfg
--rw-r--r--   0 shashankdubey   (501) staff       (20)      600 2024-05-02 18:18:58.000000 aws-ar-1.5/setup.py
+drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:27:08.942865 aws-ar-1.9/
+-rw-r--r--   0 shashankdubey   (501) staff       (20)     1713 2024-05-02 18:27:08.942673 aws-ar-1.9/PKG-INFO
+-rw-r--r--   0 shashankdubey   (501) staff       (20)     1540 2024-05-02 18:26:46.000000 aws-ar-1.9/README.md
+drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:27:08.941773 aws-ar-1.9/aws_ar/
+-rw-r--r--   0 shashankdubey   (501) staff       (20)        0 2024-05-02 13:26:47.000000 aws-ar-1.9/aws_ar/__init__.py
+-rw-r--r--   0 shashankdubey   (501) staff       (20)     1652 2024-05-02 15:50:14.000000 aws-ar-1.9/aws_ar/aws_ar.py
+drwxr-xr-x   0 shashankdubey   (501) staff       (20)        0 2024-05-02 18:27:08.942489 aws-ar-1.9/aws_ar.egg-info/
+-rw-r--r--   0 shashankdubey   (501) staff       (20)     1713 2024-05-02 18:27:08.000000 aws-ar-1.9/aws_ar.egg-info/PKG-INFO
+-rw-r--r--   0 shashankdubey   (501) staff       (20)      236 2024-05-02 18:27:08.000000 aws-ar-1.9/aws_ar.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)        1 2024-05-02 18:27:08.000000 aws-ar-1.9/aws_ar.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)       46 2024-05-02 18:27:08.000000 aws-ar-1.9/aws_ar.egg-info/entry_points.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)        6 2024-05-02 18:27:08.000000 aws-ar-1.9/aws_ar.egg-info/requires.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)        7 2024-05-02 18:27:08.000000 aws-ar-1.9/aws_ar.egg-info/top_level.txt
+-rw-r--r--   0 shashankdubey   (501) staff       (20)       38 2024-05-02 18:27:08.942902 aws-ar-1.9/setup.cfg
+-rw-r--r--   0 shashankdubey   (501) staff       (20)      600 2024-05-02 18:27:02.000000 aws-ar-1.9/setup.py
```

### Comparing `aws-ar-1.5/PKG-INFO` & `aws-ar-1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: aws-ar
-Version: 1.5
+Version: 1.9
 Summary: Command Line Utility for Configuring Assumed AWS IAM Role Credentials
 Author: Shashank Dubey
 Requires-Dist: boto3
 
-# AWS-AR: AWS Assume Role CLI Utility
+AWS-AR: AWS Assume Role CLI Utility
+===================================
 
 AWS-AR is a command-line utility that simplifies the process of configuring assumed AWS IAM role credentials in your local AWS configuration files `($HOME/.aws/config and $HOME/.aws/credentials)`. This tool allows you to assume an IAM role and automatically update your AWS CLI configuration with the temporary security credentials obtained from the assumed role.
 
 ### Features
 
-- Assume an AWS IAM role and obtain temporary security credentials.
-- Update AWS CLI configuration files ($HOME/.aws/config and $HOME/.aws/credentials) with the assumed role credentials.
-- Supports specifying the ARN of the IAM role, AWS CLI profile, and optionally creating a new profile for the assumed role.
+*   Assume an AWS IAM role and obtain temporary security credentials.
+*   Update AWS CLI configuration files ($HOME/.aws/config and $HOME/.aws/credentials) with the assumed role credentials.
+*   Supports specifying the ARN of the IAM role, AWS CLI profile, and optionally creating a new profile for the assumed role.
 
 ### Installation
 
 You can install AWS-AR using pip:
 
-```bash
-pip install aws-ar
-```
+    pip install aws-ar
+    
 
 ### Usage
 
 Assuming an IAM role and updating AWS CLI configuration:
 
-```bash
-aws-ar --assume-role-arn <role_arn> --profile <existing_profile> --set-new-profile <new_profile>
-```
-- <role_arn>: The ARN of the IAM role to assume.
-- <existing_profile>: The name of the existing AWS CLI profile to use for assuming the role.
-- <new_profile>: The name of the new profile to be created with the assumed role credentials.
+    aws-ar --assume-role-arn <role_arn> --profile <existing_profile> --set-new-profile <new_profile>
+    
+
+*   : The ARN of the IAM role to assume.
+*   : The name of the existing AWS CLI profile to use for assuming the role.
+*   : The name of the new profile to be created with the assumed role credentials.
 
 ### Example:
 
-```bash
-aws-ar --assume-role-arn arn:aws:iam::123456789012:role/MyRole --profile default --set-new-profile assumed-role
-```
+    aws-ar --assume-role-arn arn:aws:iam::123456789012:role/MyRole --profile default --set-new-profile assumed-role
+    
 
 This command assumes the IAM role MyRole, uses the default AWS CLI profile for authentication, and creates a new profile named assumed-role with the assumed role credentials.
```

### Comparing `aws-ar-1.5/README.md` & `aws-ar-1.9/aws_ar.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-# AWS-AR: AWS Assume Role CLI Utility
+Metadata-Version: 2.1
+Name: aws-ar
+Version: 1.9
+Summary: Command Line Utility for Configuring Assumed AWS IAM Role Credentials
+Author: Shashank Dubey
+Requires-Dist: boto3
+
+AWS-AR: AWS Assume Role CLI Utility
+===================================
 
 AWS-AR is a command-line utility that simplifies the process of configuring assumed AWS IAM role credentials in your local AWS configuration files `($HOME/.aws/config and $HOME/.aws/credentials)`. This tool allows you to assume an IAM role and automatically update your AWS CLI configuration with the temporary security credentials obtained from the assumed role.
 
 ### Features
 
-- Assume an AWS IAM role and obtain temporary security credentials.
-- Update AWS CLI configuration files ($HOME/.aws/config and $HOME/.aws/credentials) with the assumed role credentials.
-- Supports specifying the ARN of the IAM role, AWS CLI profile, and optionally creating a new profile for the assumed role.
+*   Assume an AWS IAM role and obtain temporary security credentials.
+*   Update AWS CLI configuration files ($HOME/.aws/config and $HOME/.aws/credentials) with the assumed role credentials.
+*   Supports specifying the ARN of the IAM role, AWS CLI profile, and optionally creating a new profile for the assumed role.
 
 ### Installation
 
 You can install AWS-AR using pip:
 
-```bash
-pip install aws-ar
-```
+    pip install aws-ar
+    
 
 ### Usage
 
 Assuming an IAM role and updating AWS CLI configuration:
 
-```bash
-aws-ar --assume-role-arn <role_arn> --profile <existing_profile> --set-new-profile <new_profile>
-```
-- <role_arn>: The ARN of the IAM role to assume.
-- <existing_profile>: The name of the existing AWS CLI profile to use for assuming the role.
-- <new_profile>: The name of the new profile to be created with the assumed role credentials.
+    aws-ar --assume-role-arn <role_arn> --profile <existing_profile> --set-new-profile <new_profile>
+    
+
+*   : The ARN of the IAM role to assume.
+*   : The name of the existing AWS CLI profile to use for assuming the role.
+*   : The name of the new profile to be created with the assumed role credentials.
 
 ### Example:
 
-```bash
-aws-ar --assume-role-arn arn:aws:iam::123456789012:role/MyRole --profile default --set-new-profile assumed-role
-```
+    aws-ar --assume-role-arn arn:aws:iam::123456789012:role/MyRole --profile default --set-new-profile assumed-role
+    
 
-This command assumes the IAM role MyRole, uses the default AWS CLI profile for authentication, and creates a new profile named assumed-role with the assumed role credentials.
+This command assumes the IAM role MyRole, uses the default AWS CLI profile for authentication, and creates a new profile named assumed-role with the assumed role credentials.
```

### Comparing `aws-ar-1.5/aws_ar/aws_ar.py` & `aws-ar-1.9/aws_ar/aws_ar.py`

 * *Files identical despite different names*

### Comparing `aws-ar-1.5/aws_ar.egg-info/PKG-INFO` & `aws-ar-1.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-Metadata-Version: 2.1
-Name: aws-ar
-Version: 1.5
-Summary: Command Line Utility for Configuring Assumed AWS IAM Role Credentials
-Author: Shashank Dubey
-Requires-Dist: boto3
-
-# AWS-AR: AWS Assume Role CLI Utility
+AWS-AR: AWS Assume Role CLI Utility
+===================================
 
 AWS-AR is a command-line utility that simplifies the process of configuring assumed AWS IAM role credentials in your local AWS configuration files `($HOME/.aws/config and $HOME/.aws/credentials)`. This tool allows you to assume an IAM role and automatically update your AWS CLI configuration with the temporary security credentials obtained from the assumed role.
 
 ### Features
 
-- Assume an AWS IAM role and obtain temporary security credentials.
-- Update AWS CLI configuration files ($HOME/.aws/config and $HOME/.aws/credentials) with the assumed role credentials.
-- Supports specifying the ARN of the IAM role, AWS CLI profile, and optionally creating a new profile for the assumed role.
+*   Assume an AWS IAM role and obtain temporary security credentials.
+*   Update AWS CLI configuration files ($HOME/.aws/config and $HOME/.aws/credentials) with the assumed role credentials.
+*   Supports specifying the ARN of the IAM role, AWS CLI profile, and optionally creating a new profile for the assumed role.
 
 ### Installation
 
 You can install AWS-AR using pip:
 
-```bash
-pip install aws-ar
-```
+    pip install aws-ar
+    
 
 ### Usage
 
 Assuming an IAM role and updating AWS CLI configuration:
 
-```bash
-aws-ar --assume-role-arn <role_arn> --profile <existing_profile> --set-new-profile <new_profile>
-```
-- <role_arn>: The ARN of the IAM role to assume.
-- <existing_profile>: The name of the existing AWS CLI profile to use for assuming the role.
-- <new_profile>: The name of the new profile to be created with the assumed role credentials.
+    aws-ar --assume-role-arn <role_arn> --profile <existing_profile> --set-new-profile <new_profile>
+    
+
+*   : The ARN of the IAM role to assume.
+*   : The name of the existing AWS CLI profile to use for assuming the role.
+*   : The name of the new profile to be created with the assumed role credentials.
 
 ### Example:
 
-```bash
-aws-ar --assume-role-arn arn:aws:iam::123456789012:role/MyRole --profile default --set-new-profile assumed-role
-```
+    aws-ar --assume-role-arn arn:aws:iam::123456789012:role/MyRole --profile default --set-new-profile assumed-role
+    
 
-This command assumes the IAM role MyRole, uses the default AWS CLI profile for authentication, and creates a new profile named assumed-role with the assumed role credentials.
+This command assumes the IAM role MyRole, uses the default AWS CLI profile for authentication, and creates a new profile named assumed-role with the assumed role credentials.
```

### Comparing `aws-ar-1.5/setup.py` & `aws-ar-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 setup(
     name='aws-ar',
     summary='Command Line Utility for Configuring Assumed AWS IAM Role Credentials',
     description='Command Line Utility for Configuring Assumed AWS IAM Role Credentials',  
     long_description=long_description,
-    version='1.5',
+    version='1.9',
     author='Shashank Dubey',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'aws-ar = aws_ar.aws_ar:main'
         ]
     },
```

