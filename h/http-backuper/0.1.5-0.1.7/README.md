# Comparing `tmp/http_backuper-0.1.5.tar.gz` & `tmp/http_backuper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_backuper-0.1.5.tar", last modified: Fri Aug  4 15:46:24 2023, max compression
+gzip compressed data, was "http_backuper-0.1.7.tar", last modified: Thu May  2 12:18:59 2024, max compression
```

## Comparing `http_backuper-0.1.5.tar` & `http_backuper-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-04 15:46:24.567272 http_backuper-0.1.5/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     1069 2023-08-03 16:49:27.000000 http_backuper-0.1.5/LICENSE
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      311 2023-08-04 15:46:24.567272 http_backuper-0.1.5/PKG-INFO
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     2077 2023-08-03 17:10:09.000000 http_backuper-0.1.5/README.md
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-04 15:46:24.567272 http_backuper-0.1.5/http_backuper/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:19.000000 http_backuper-0.1.5/http_backuper/__init__.py
--rwxrwxr-x   0 djbios    (1000) djbios    (1000)     9256 2023-08-04 15:46:12.000000 http_backuper-0.1.5/http_backuper/backuper.py
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     1136 2023-08-04 15:40:06.000000 http_backuper-0.1.5/http_backuper/models.py
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-04 15:46:24.567272 http_backuper-0.1.5/http_backuper.egg-info/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      311 2023-08-04 15:46:24.000000 http_backuper-0.1.5/http_backuper.egg-info/PKG-INFO
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      359 2023-08-04 15:46:24.000000 http_backuper-0.1.5/http_backuper.egg-info/SOURCES.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        1 2023-08-04 15:46:24.000000 http_backuper-0.1.5/http_backuper.egg-info/dependency_links.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      101 2023-08-04 15:46:24.000000 http_backuper-0.1.5/http_backuper.egg-info/entry_points.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       59 2023-08-04 15:46:24.000000 http_backuper-0.1.5/http_backuper.egg-info/requires.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       20 2023-08-04 15:46:24.000000 http_backuper-0.1.5/http_backuper.egg-info/top_level.txt
--rw-rw-r--   0 djbios    (1000) djbios    (1000)       38 2023-08-04 15:46:24.567272 http_backuper-0.1.5/setup.cfg
--rw-rw-r--   0 djbios    (1000) djbios    (1000)      698 2023-08-04 15:46:21.000000 http_backuper-0.1.5/setup.py
-drwxrwxr-x   0 djbios    (1000) djbios    (1000)        0 2023-08-04 15:46:24.567272 http_backuper-0.1.5/tests/
--rw-rw-r--   0 djbios    (1000) djbios    (1000)        0 2023-08-03 16:46:44.000000 http_backuper-0.1.5/tests/__init__.py
--rw-rw-r--   0 djbios    (1000) djbios    (1000)     8600 2023-08-03 17:01:17.000000 http_backuper-0.1.5/tests/tests.py
+drwxr-xr-x   0 djbios     (503) staff       (20)        0 2024-05-02 12:18:59.182566 http_backuper-0.1.7/
+-rw-r--r--   0 djbios     (503) staff       (20)     1069 2024-01-02 17:59:47.000000 http_backuper-0.1.7/LICENSE
+-rw-r--r--   0 djbios     (503) staff       (20)      460 2024-05-02 12:18:59.182353 http_backuper-0.1.7/PKG-INFO
+-rw-r--r--   0 djbios     (503) staff       (20)     2077 2024-01-02 17:59:47.000000 http_backuper-0.1.7/README.md
+drwxr-xr-x   0 djbios     (503) staff       (20)        0 2024-05-02 12:18:59.180578 http_backuper-0.1.7/http_backuper/
+-rw-r--r--   0 djbios     (503) staff       (20)        0 2024-01-02 17:59:47.000000 http_backuper-0.1.7/http_backuper/__init__.py
+-rwxr-xr-x   0 djbios     (503) staff       (20)     9542 2024-05-02 12:13:14.000000 http_backuper-0.1.7/http_backuper/backuper.py
+-rw-r--r--   0 djbios     (503) staff       (20)     1136 2024-01-02 17:59:47.000000 http_backuper-0.1.7/http_backuper/models.py
+drwxr-xr-x   0 djbios     (503) staff       (20)        0 2024-05-02 12:18:59.182143 http_backuper-0.1.7/http_backuper.egg-info/
+-rw-r--r--   0 djbios     (503) staff       (20)      460 2024-05-02 12:18:59.000000 http_backuper-0.1.7/http_backuper.egg-info/PKG-INFO
+-rw-r--r--   0 djbios     (503) staff       (20)      359 2024-05-02 12:18:59.000000 http_backuper-0.1.7/http_backuper.egg-info/SOURCES.txt
+-rw-r--r--   0 djbios     (503) staff       (20)        1 2024-05-02 12:18:59.000000 http_backuper-0.1.7/http_backuper.egg-info/dependency_links.txt
+-rw-r--r--   0 djbios     (503) staff       (20)      101 2024-05-02 12:18:59.000000 http_backuper-0.1.7/http_backuper.egg-info/entry_points.txt
+-rw-r--r--   0 djbios     (503) staff       (20)       59 2024-05-02 12:18:59.000000 http_backuper-0.1.7/http_backuper.egg-info/requires.txt
+-rw-r--r--   0 djbios     (503) staff       (20)       20 2024-05-02 12:18:59.000000 http_backuper-0.1.7/http_backuper.egg-info/top_level.txt
+-rw-r--r--   0 djbios     (503) staff       (20)       38 2024-05-02 12:18:59.182610 http_backuper-0.1.7/setup.cfg
+-rw-r--r--   0 djbios     (503) staff       (20)      698 2024-05-02 12:14:14.000000 http_backuper-0.1.7/setup.py
+drwxr-xr-x   0 djbios     (503) staff       (20)        0 2024-05-02 12:18:59.181781 http_backuper-0.1.7/tests/
+-rw-r--r--   0 djbios     (503) staff       (20)        0 2024-01-02 17:59:47.000000 http_backuper-0.1.7/tests/__init__.py
+-rw-r--r--   0 djbios     (503) staff       (20)     8600 2024-01-02 17:59:47.000000 http_backuper-0.1.7/tests/tests.py
```

### Comparing `http_backuper-0.1.5/LICENSE` & `http_backuper-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `http_backuper-0.1.5/README.md` & `http_backuper-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `http_backuper-0.1.5/http_backuper/backuper.py` & `http_backuper-0.1.7/http_backuper/backuper.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,38 +171,42 @@
 
 
 def job(backup_config: BackupSection, general_config: GeneralSection) -> None:
     logger.info(f"Starting backup {backup_config.name}")
     tar_stream = io.BytesIO()
     with tarfile.open(fileobj=tar_stream, mode="w:gz") as tar:
         for source in backup_config.sources:
-            if source.path:
-                if source.container_name:
-                    docker = DockerClient.from_env()
-                    add_container_path_to_tar(
-                        docker, source.container_name, source.path, tar
-                    )
-                else:
-                    add_path_to_tar(tar, source.path)
-            elif source.command:
-                if source.container_name:
-                    docker = DockerClient.from_env()
-                    run_command_in_container(
-                        client=docker,
-                        container_name=source.container_name,
-                        command=source.command,
-                        tar=tar,
-                        filename=source.name,
-                    )
-                else:
-                    run_command_on_host(
-                        command=source.command,
-                        tar=tar,
-                        filename=source.name,
-                    )
+            try:
+                if source.path:
+                    if source.container_name:
+                        docker = DockerClient.from_env()
+                        add_container_path_to_tar(
+                            docker, source.container_name, source.path, tar
+                        )
+                    else:
+                        add_path_to_tar(tar, source.path)
+                elif source.command:
+                    if source.container_name:
+                        docker = DockerClient.from_env()
+                        run_command_in_container(
+                            client=docker,
+                            container_name=source.container_name,
+                            command=source.command,
+                            tar=tar,
+                            filename=source.name,
+                        )
+                    else:
+                        run_command_on_host(
+                            command=source.command,
+                            tar=tar,
+                            filename=source.name,
+                        )
+            except Exception as e:
+                logger.error(f"Failed to backup source {source.name}: {e}")
+                return
 
     tar_stream.seek(0)
     if rp := general_config.requests_properties:
         headers = rp.get("headers") or {}
     else:
         headers = {}
 
@@ -236,15 +240,15 @@
       [Install]
       WantedBy=multi-user.target
       """
 
     with open("/etc/systemd/system/http_backuper.service", "w") as f:
         f.write(service_content)
 
-    subprocess.run(["cp", "-n", "./config.example.yml", "/etc/http_backuper/config.yml"])
+    subprocess.run(["cp", "-n", "./config.example.yml", "/etc/http_backuper/config.yml"])  # TODO fix this + mkdir
     subprocess.run(["systemctl", "daemon-reload"])
     subprocess.run(["systemctl", "enable", "http_backuper.service"])
     logger.info("Service installed and enabled.")
     return
 
 
 def main():
@@ -299,12 +303,12 @@
 
 
 if __name__ == "__main__":
     main()
 
 
 # TODO add arguments:
-#  -i to install as a service to linux
 # TODO better logging
 # TODO fail tolerance
 # TODO tests on commands
 # TODO ensure no memory leaks
+# TODO allow to run concrete backups by name from cli
```

### Comparing `http_backuper-0.1.5/http_backuper/models.py` & `http_backuper-0.1.7/http_backuper/models.py`

 * *Files identical despite different names*

### Comparing `http_backuper-0.1.5/setup.py` & `http_backuper-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='http_backuper',
-    version='0.1.5',
+    version='0.1.7',
     url='https://github.com/djbios/http_backuper',
     author='djbios',
     author_email='dorandval@gmail.com',
     description='A simple backup solution',
     packages=find_packages(),
     install_requires=[
         'pydantic<2', 'requests', 'schedule', 'docker', 'healthchecks_io', 'PyYAML',
```

### Comparing `http_backuper-0.1.5/tests/tests.py` & `http_backuper-0.1.7/tests/tests.py`

 * *Files identical despite different names*

