# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1714514471.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1714680794.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1714514471.tar", last modified: Tue Apr 30 22:03:55 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1714680794.tar", last modified: Thu May  2 20:16:18 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471.tar` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:03:55.043435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-30 22:03:55.043435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:03:55.031435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4080 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:03:55.031435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:03:55.035435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      940 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    15965 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15536 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:03:55.039435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:03:55.043435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108491 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14976 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91820 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:03:55.043435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-30 22:03:55.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-30 22:03:55.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:03:55.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 22:03:55.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 22:03:55.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-04-30 22:03:48.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 22:03:55.043435 pulumi_kubernetes_the_hard_way-0.0.21a1714514471/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:18.606025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-02 20:16:18.606025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:18.594025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4080 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:18.598025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:18.602025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      940 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    15965 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15536 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:18.602025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:18.606025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108491 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14976 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91820 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:18.606025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-02 20:16:18.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-02 20:16:18.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:16:18.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 20:16:18.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 20:16:18.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-02 20:16:12.000000 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:16:18.606025 pulumi_kubernetes_the_hard_way-0.0.21a1714680794/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1714514471
+Version: 0.0.21a1714680794
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/README.md` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1714514471
+Version: 0.0.21a1714680794
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1714514471/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.21a1714680794/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.10.0,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.21a1714514471"
+  version = "0.0.21a1714680794"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

