# Comparing `tmp/cyzutils-0.0.3.tar.gz` & `tmp/cyzutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyzutils-0.0.3.tar", last modified: Thu May  2 16:13:08 2024, max compression
+gzip compressed data, was "cyzutils-0.0.4.tar", last modified: Thu May  2 16:26:26 2024, max compression
```

## Comparing `cyzutils-0.0.3.tar` & `cyzutils-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:13:08.455174 cyzutils-0.0.3/
--rw-r--r--   0 cyz        (501) staff       (20)     1024 2024-05-02 16:13:08.455001 cyzutils-0.0.3/PKG-INFO
--rw-rw-rw-   0 cyz        (501) staff       (20)      835 2024-05-02 16:12:29.000000 cyzutils-0.0.3/README.md
-drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:13:08.453287 cyzutils-0.0.3/cyzutils/
--rw-rw-rw-   0 cyz        (501) staff       (20)       19 2024-04-08 07:21:05.000000 cyzutils-0.0.3/cyzutils/__init__.py
--rw-rw-rw-   0 cyz        (501) staff       (20)     2082 2024-04-30 11:34:25.000000 cyzutils-0.0.3/cyzutils/mail.py
--rw-r--r--   0 cyz        (501) staff       (20)     1468 2024-05-02 16:09:18.000000 cyzutils-0.0.3/cyzutils/run_py.py
-drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:13:08.454824 cyzutils-0.0.3/cyzutils.egg-info/
--rw-r--r--   0 cyz        (501) staff       (20)     1024 2024-05-02 16:13:08.000000 cyzutils-0.0.3/cyzutils.egg-info/PKG-INFO
--rw-r--r--   0 cyz        (501) staff       (20)      203 2024-05-02 16:13:08.000000 cyzutils-0.0.3/cyzutils.egg-info/SOURCES.txt
--rw-r--r--   0 cyz        (501) staff       (20)        1 2024-05-02 16:13:08.000000 cyzutils-0.0.3/cyzutils.egg-info/dependency_links.txt
--rw-r--r--   0 cyz        (501) staff       (20)        9 2024-05-02 16:13:08.000000 cyzutils-0.0.3/cyzutils.egg-info/top_level.txt
--rw-r--r--   0 cyz        (501) staff       (20)       38 2024-05-02 16:13:08.455211 cyzutils-0.0.3/setup.cfg
--rw-rw-rw-   0 cyz        (501) staff       (20)     1116 2024-05-02 14:55:34.000000 cyzutils-0.0.3/setup.py
+drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:26:26.410784 cyzutils-0.0.4/
+-rw-r--r--   0 cyz        (501) staff       (20)     1039 2024-05-02 16:26:26.410620 cyzutils-0.0.4/PKG-INFO
+-rw-rw-rw-   0 cyz        (501) staff       (20)      850 2024-05-02 16:24:06.000000 cyzutils-0.0.4/README.md
+drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:26:26.409644 cyzutils-0.0.4/cyzutils/
+-rw-rw-rw-   0 cyz        (501) staff       (20)       46 2024-05-02 16:24:56.000000 cyzutils-0.0.4/cyzutils/__init__.py
+-rw-r--r--   0 cyz        (501) staff       (20)     1439 2024-05-02 16:23:06.000000 cyzutils-0.0.4/cyzutils/run_py.py
+-rw-rw-rw-   0 cyz        (501) staff       (20)     2092 2024-05-02 16:24:49.000000 cyzutils-0.0.4/cyzutils/send_mail.py
+drwxr-xr-x   0 cyz        (501) staff       (20)        0 2024-05-02 16:26:26.410435 cyzutils-0.0.4/cyzutils.egg-info/
+-rw-r--r--   0 cyz        (501) staff       (20)     1039 2024-05-02 16:26:26.000000 cyzutils-0.0.4/cyzutils.egg-info/PKG-INFO
+-rw-r--r--   0 cyz        (501) staff       (20)      208 2024-05-02 16:26:26.000000 cyzutils-0.0.4/cyzutils.egg-info/SOURCES.txt
+-rw-r--r--   0 cyz        (501) staff       (20)        1 2024-05-02 16:26:26.000000 cyzutils-0.0.4/cyzutils.egg-info/dependency_links.txt
+-rw-r--r--   0 cyz        (501) staff       (20)        9 2024-05-02 16:26:26.000000 cyzutils-0.0.4/cyzutils.egg-info/top_level.txt
+-rw-r--r--   0 cyz        (501) staff       (20)       38 2024-05-02 16:26:26.410822 cyzutils-0.0.4/setup.cfg
+-rw-rw-rw-   0 cyz        (501) staff       (20)     1116 2024-05-02 16:26:05.000000 cyzutils-0.0.4/setup.py
```

### Comparing `cyzutils-0.0.3/PKG-INFO` & `cyzutils-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyzutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: my utils
 Home-page: https://github.com/cyz020403
 Author: cyz020403
 Author-email: cyz020403@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
 mail('subject', 'content') # send to myself
 ```
 
 ---
 
 Run python file with cmd
 
-Each command line argument is required to be given in a list
+Each command line parameter needs to be given as a list or a specific value
 
 No limit on the number of command line parameters
 
 ```python
 # run python cmd
 from cyzutils import run_py
 run_py(fail_path, arg1_name=arg1_list, arg2_name=arg2_list)
```

### Comparing `cyzutils-0.0.3/README.md` & `cyzutils-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 mail('subject', 'content') # send to myself
 ```
 
 ---
 
 Run python file with cmd
 
-Each command line argument is required to be given in a list
+Each command line parameter needs to be given as a list or a specific value
 
 No limit on the number of command line parameters
 
 ```python
 # run python cmd
 from cyzutils import run_py
 run_py(fail_path, arg1_name=arg1_list, arg2_name=arg2_list)
```

### Comparing `cyzutils-0.0.3/cyzutils/mail.py` & `cyzutils-0.0.4/cyzutils/send_mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import smtplib
 from email.mime.text import MIMEText
 from email.header import Header
 import base64
 
-def mail(subject, content, receiver='cyzhelper@qq.com', sender='cyzhelper@qq.com', passward='idzeantfoqclcdgi', \
+def send_mail(subject, content, receiver='cyzhelper@qq.com', sender='cyzhelper@qq.com', passward='idzeantfoqclcdgi', \
                from_nike_name='default', to_nike_name='default'):
     
     mail_host = "smtp.qq.com"
 
     if from_nike_name == 'default':
         from_nike_name = sender.split('@')[0]
     from_nike_name = base64.b64encode(from_nike_name.encode('utf-8')).decode()
@@ -34,15 +34,15 @@
         print('发送失败！！')
 
 
 if __name__ == '__main__':
     print('this is a use demo')
     subject = '嘎嘎gaga'
     content = 'gagaga gagagaga嘎嘎\n' + 'gaga! gaga!'
-    mail(subject, content)
+    send_mail(subject, content)
     # mail(subject, content, 'receiver@qq.com', 'sender@qq.com', 'passward')
 
 '''
 qq邮箱官网教程
 
 POP3/SMTP 设置方法
 用户名/帐户： 你的QQ邮箱完整的地址
```

### Comparing `cyzutils-0.0.3/cyzutils/run_py.py` & `cyzutils-0.0.4/cyzutils/run_py.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 '''
 
 import subprocess
 
 def run_py(file_path, **args):
     for key, value in args.items():
         if not isinstance(value, list):
-            raise ValueError(f'arg \'{key}\' must be list')
+            args[key] = [value]
     
     cmd = ['python', file_path]
     keys = list(args.keys())
     keys.reverse()
     values = [args[key] for key in keys]
     arg_list = nested_loop(**dict(zip(keys, values)))
 
     print('The following commands will be executed in sequence:')
     for arg in arg_list:
         arg = ' '.join(arg)
         print('python', file_path, arg)
-    if input('Do you want to continue? (y/n)') != 'y':
-        return
+    # if input('Do you want to continue? (y/n)') != 'y':
+    #     return
 
     for arg in arg_list:
         p = subprocess.Popen(cmd + arg)
         p.wait()
 
 
 
@@ -41,12 +41,12 @@
             res.append([f'--{key}', str(value)] + sub_args)
     return res
 
 def main():
     file_path = 'test/test.py'
     test1 = [1, 2]
     test2 = [3, 4]
-    test3 = [5, 6]
+    test3 = 5
     run_py(file_path, arg1=test1, arg2=test2, arg3=test3)
 
 if __name__ == '__main__':
     main()
```

### Comparing `cyzutils-0.0.3/cyzutils.egg-info/PKG-INFO` & `cyzutils-0.0.4/cyzutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyzutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: my utils
 Home-page: https://github.com/cyz020403
 Author: cyz020403
 Author-email: cyz020403@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
 mail('subject', 'content') # send to myself
 ```
 
 ---
 
 Run python file with cmd
 
-Each command line argument is required to be given in a list
+Each command line parameter needs to be given as a list or a specific value
 
 No limit on the number of command line parameters
 
 ```python
 # run python cmd
 from cyzutils import run_py
 run_py(fail_path, arg1_name=arg1_list, arg2_name=arg2_list)
```

### Comparing `cyzutils-0.0.3/setup.py` & `cyzutils-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='cyzutils',  # 必填，项目的名字，用户根据这个名字安装，pip install SpiderKeeper-new
-    version='0.0.3',  # 必填，项目的版本，建议遵循语义化版本规范
+    version='0.0.4',  # 必填，项目的版本，建议遵循语义化版本规范
     author='cyz020403',  # 项目的作者
     description='my utils',  # 项目的一个简短描述
     long_description=long_description,  # 项目的详细说明，通常读取 README.md 文件的内容
     long_description_content_type='text/markdown',  # 描述的格式，可选的值： text/plain, text/x-rst, and text/markdown
     author_email='cyz020403@gmail.com',  # 作者的有效邮箱地址
     url='https://github.com/cyz020403',  # 项目的源码地址
     license='MIT',
```

