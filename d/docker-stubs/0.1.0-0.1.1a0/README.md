# Comparing `tmp/docker_stubs-0.1.0.tar.gz` & `tmp/docker_stubs-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_stubs-0.1.0.tar", max compression
+gzip compressed data, was "docker_stubs-0.1.1a0.tar", max compression
```

## Comparing `docker_stubs-0.1.0.tar` & `docker_stubs-0.1.1a0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0        0 2023-08-24 17:49:03.116853 docker_stubs-0.1.0/README.md
--rw-r--r--   0        0        0      217 2024-04-16 17:18:30.916948 docker_stubs-0.1.0/docker-stubs/__init__.pyi
--rw-r--r--   0        0        0      172 2024-04-16 17:18:30.917249 docker_stubs-0.1.0/docker-stubs/_version.pyi
--rw-r--r--   0        0        0       43 2024-04-16 17:18:30.917473 docker_stubs-0.1.0/docker-stubs/api/__init__.pyi
--rw-r--r--   0        0        0     1667 2024-04-16 17:58:45.854380 docker_stubs-0.1.0/docker-stubs/api/build.pyi
--rw-r--r--   0        0        0     2957 2024-04-16 18:06:55.547581 docker_stubs-0.1.0/docker-stubs/api/client.pyi
--rw-r--r--   0        0        0      541 2024-04-16 18:07:33.855357 docker_stubs-0.1.0/docker-stubs/api/config.pyi
--rw-r--r--   0        0        0     5100 2024-04-16 17:23:52.331889 docker_stubs-0.1.0/docker-stubs/api/container.pyi
--rw-r--r--   0        0        0      862 2024-04-16 19:00:31.020318 docker_stubs-0.1.0/docker-stubs/api/daemon.pyi
--rw-r--r--   0        0        0     1033 2024-04-16 18:29:49.014105 docker_stubs-0.1.0/docker-stubs/api/exec_api.pyi
--rw-r--r--   0        0        0     3385 2024-04-16 18:47:54.523987 docker_stubs-0.1.0/docker-stubs/api/image.pyi
--rw-r--r--   0        0        0     1883 2024-04-16 18:32:47.572806 docker_stubs-0.1.0/docker-stubs/api/network.pyi
--rw-r--r--   0        0        0     1206 2024-04-16 18:15:29.221214 docker_stubs-0.1.0/docker-stubs/api/plugin.pyi
--rw-r--r--   0        0        0      647 2024-04-16 18:47:54.517089 docker_stubs-0.1.0/docker-stubs/api/secret.pyi
--rw-r--r--   0        0        0     2255 2024-04-16 18:51:34.775620 docker_stubs-0.1.0/docker-stubs/api/service.pyi
--rw-r--r--   0        0        0     1859 2024-04-16 19:00:31.015951 docker_stubs-0.1.0/docker-stubs/api/swarm.pyi
--rw-r--r--   0        0        0      603 2024-04-16 19:00:31.018283 docker_stubs-0.1.0/docker-stubs/api/volume.pyi
--rw-r--r--   0        0        0     1929 2024-04-18 14:53:12.722434 docker_stubs-0.1.0/docker-stubs/auth.pyi
--rw-r--r--   0        0        0     2148 2024-04-18 14:53:12.718260 docker_stubs-0.1.0/docker-stubs/client.pyi
--rw-r--r--   0        0        0      574 2024-04-18 14:58:41.871486 docker_stubs-0.1.0/docker-stubs/constants.pyi
--rw-r--r--   0        0        0       82 2024-04-16 17:18:30.922340 docker_stubs-0.1.0/docker-stubs/context/__init__.pyi
--rw-r--r--   0        0        0     1083 2024-04-16 19:06:43.475837 docker_stubs-0.1.0/docker-stubs/context/api.pyi
--rw-r--r--   0        0        0      710 2024-04-17 17:54:03.953851 docker_stubs-0.1.0/docker-stubs/context/config.pyi
--rw-r--r--   0        0        0     1636 2024-04-17 16:58:41.372326 docker_stubs-0.1.0/docker-stubs/context/context.pyi
--rw-r--r--   0        0        0      328 2024-04-16 17:23:52.298994 docker_stubs-0.1.0/docker-stubs/credentials/__init__.pyi
--rw-r--r--   0        0        0       93 2024-04-16 17:18:30.923374 docker_stubs-0.1.0/docker-stubs/credentials/constants.pyi
--rw-r--r--   0        0        0      166 2024-04-16 17:18:30.923499 docker_stubs-0.1.0/docker-stubs/credentials/errors.pyi
--rw-r--r--   0        0        0      648 2024-04-17 17:54:03.962000 docker_stubs-0.1.0/docker-stubs/credentials/store.pyi
--rw-r--r--   0        0        0       58 2024-04-17 17:54:03.964177 docker_stubs-0.1.0/docker-stubs/credentials/utils.pyi
--rw-r--r--   0        0        0     2071 2024-04-18 14:58:41.869101 docker_stubs-0.1.0/docker-stubs/errors.pyi
--rw-r--r--   0        0        0        0 2024-04-16 17:18:30.924543 docker_stubs-0.1.0/docker-stubs/models/__init__.pyi
--rw-r--r--   0        0        0      423 2024-04-17 17:54:03.948951 docker_stubs-0.1.0/docker-stubs/models/configs.pyi
--rw-r--r--   0        0        0     3559 2024-04-17 17:54:03.943760 docker_stubs-0.1.0/docker-stubs/models/containers.pyi
--rw-r--r--   0        0        0     2446 2024-04-17 17:54:03.970791 docker_stubs-0.1.0/docker-stubs/models/images.pyi
--rw-r--r--   0        0        0      843 2024-04-17 17:54:03.959481 docker_stubs-0.1.0/docker-stubs/models/networks.pyi
--rw-r--r--   0        0        0      473 2024-04-17 17:54:03.968702 docker_stubs-0.1.0/docker-stubs/models/nodes.pyi
--rw-r--r--   0        0        0      977 2024-04-17 17:54:03.939751 docker_stubs-0.1.0/docker-stubs/models/plugins.pyi
--rw-r--r--   0        0        0      921 2024-04-17 17:54:03.946250 docker_stubs-0.1.0/docker-stubs/models/resource.pyi
--rw-r--r--   0        0        0      427 2024-04-17 17:54:03.936238 docker_stubs-0.1.0/docker-stubs/models/secrets.pyi
--rw-r--r--   0        0        0     1347 2024-04-17 17:54:03.973201 docker_stubs-0.1.0/docker-stubs/models/services.pyi
--rw-r--r--   0        0        0     1171 2024-04-17 17:54:03.966634 docker_stubs-0.1.0/docker-stubs/models/swarm.pyi
--rw-r--r--   0        0        0      563 2024-04-17 17:54:03.956489 docker_stubs-0.1.0/docker-stubs/models/volumes.pyi
--rw-r--r--   0        0        0      382 2024-04-16 17:23:52.320792 docker_stubs-0.1.0/docker-stubs/tls.pyi
--rw-r--r--   0        0        0      223 2024-04-16 17:18:30.928067 docker_stubs-0.1.0/docker-stubs/transport/__init__.pyi
--rw-r--r--   0        0        0      113 2024-04-16 17:18:30.928388 docker_stubs-0.1.0/docker-stubs/transport/basehttpadapter.pyi
--rw-r--r--   0        0        0     1206 2024-04-17 17:55:31.918412 docker_stubs-0.1.0/docker-stubs/transport/npipeconn.pyi
--rw-r--r--   0        0        0     1783 2024-04-16 17:23:52.359538 docker_stubs-0.1.0/docker-stubs/transport/npipesocket.pyi
--rw-r--r--   0        0        0     1793 2024-04-16 17:23:52.355880 docker_stubs-0.1.0/docker-stubs/transport/sshconn.pyi
--rw-r--r--   0        0        0     1166 2024-04-16 17:23:52.344844 docker_stubs-0.1.0/docker-stubs/transport/unixconn.pyi
--rw-r--r--   0        0        0     1157 2024-04-16 17:23:52.339840 docker_stubs-0.1.0/docker-stubs/types/__init__.pyi
--rw-r--r--   0        0        0       64 2024-04-16 17:18:30.929722 docker_stubs-0.1.0/docker-stubs/types/base.pyi
--rw-r--r--   0        0        0     5752 2024-04-16 17:23:52.411755 docker_stubs-0.1.0/docker-stubs/types/containers.pyi
--rw-r--r--   0        0        0      245 2024-04-16 17:18:30.930436 docker_stubs-0.1.0/docker-stubs/types/daemon.pyi
--rw-r--r--   0        0        0      323 2024-04-16 17:18:30.930584 docker_stubs-0.1.0/docker-stubs/types/healthcheck.pyi
--rw-r--r--   0        0        0      586 2024-04-18 14:58:41.873532 docker_stubs-0.1.0/docker-stubs/types/io.pyi
--rw-r--r--   0        0        0       57 2024-04-16 18:06:55.551441 docker_stubs-0.1.0/docker-stubs/types/misc_types.pyi
--rw-r--r--   0        0        0     1108 2024-04-16 17:23:52.364686 docker_stubs-0.1.0/docker-stubs/types/networks.pyi
--rw-r--r--   0        0        0     5856 2024-04-16 17:23:52.421277 docker_stubs-0.1.0/docker-stubs/types/services.pyi
--rw-r--r--   0        0        0     1261 2024-04-16 17:23:52.363841 docker_stubs-0.1.0/docker-stubs/types/swarm.pyi
--rw-r--r--   0        0        0     1274 2024-04-16 17:23:52.350223 docker_stubs-0.1.0/docker-stubs/utils/__init__.pyi
--rw-r--r--   0        0        0     1147 2024-04-16 17:23:52.364092 docker_stubs-0.1.0/docker-stubs/utils/build.pyi
--rw-r--r--   0        0        0      379 2024-04-16 17:18:30.932170 docker_stubs-0.1.0/docker-stubs/utils/config.pyi
--rw-r--r--   0        0        0      162 2024-04-16 17:18:30.932297 docker_stubs-0.1.0/docker-stubs/utils/decorators.pyi
--rw-r--r--   0        0        0       84 2024-04-16 17:18:30.932537 docker_stubs-0.1.0/docker-stubs/utils/fnmatch.pyi
--rw-r--r--   0        0        0      465 2024-04-16 17:23:52.354730 docker_stubs-0.1.0/docker-stubs/utils/json_stream.pyi
--rw-r--r--   0        0        0      347 2024-04-16 17:18:30.932833 docker_stubs-0.1.0/docker-stubs/utils/ports.pyi
--rw-r--r--   0        0        0      383 2024-04-16 17:18:30.933261 docker_stubs-0.1.0/docker-stubs/utils/proxy.pyi
--rw-r--r--   0        0        0      580 2024-04-16 17:18:30.933431 docker_stubs-0.1.0/docker-stubs/utils/socket.pyi
--rw-r--r--   0        0        0     1512 2024-04-16 18:18:44.318142 docker_stubs-0.1.0/docker-stubs/utils/utils.pyi
--rw-r--r--   0        0        0        0 2024-04-16 17:18:30.933791 docker_stubs-0.1.0/docker-stubs/version.pyi
--rw-r--r--   0        0        0      428 2024-04-16 15:19:12.512429 docker_stubs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 docker_stubs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-18 16:56:58.965789 docker_stubs-0.1.1a0/README.md
+-rw-r--r--   0        0        0      217 2024-04-16 17:18:30.916948 docker_stubs-0.1.1a0/docker-stubs/__init__.pyi
+-rw-r--r--   0        0        0      172 2024-04-18 16:56:58.965914 docker_stubs-0.1.1a0/docker-stubs/_version.pyi
+-rw-r--r--   0        0        0       43 2024-04-16 17:18:30.917473 docker_stubs-0.1.1a0/docker-stubs/api/__init__.pyi
+-rw-r--r--   0        0        0     1796 2024-05-02 14:01:35.366522 docker_stubs-0.1.1a0/docker-stubs/api/build.pyi
+-rw-r--r--   0        0        0     3005 2024-05-02 14:01:35.366708 docker_stubs-0.1.1a0/docker-stubs/api/client.pyi
+-rw-r--r--   0        0        0      638 2024-05-02 14:01:35.366875 docker_stubs-0.1.1a0/docker-stubs/api/config.pyi
+-rw-r--r--   0        0        0     5100 2024-04-18 16:56:58.966683 docker_stubs-0.1.1a0/docker-stubs/api/container.pyi
+-rw-r--r--   0        0        0      885 2024-05-02 14:01:35.367056 docker_stubs-0.1.1a0/docker-stubs/api/daemon.pyi
+-rw-r--r--   0        0        0     1057 2024-05-02 14:01:35.367234 docker_stubs-0.1.1a0/docker-stubs/api/exec_api.pyi
+-rw-r--r--   0        0        0     3540 2024-05-02 14:01:35.367527 docker_stubs-0.1.1a0/docker-stubs/api/image.pyi
+-rw-r--r--   0        0        0     1827 2024-05-02 14:01:35.367701 docker_stubs-0.1.1a0/docker-stubs/api/network.pyi
+-rw-r--r--   0        0        0     1296 2024-05-02 14:01:35.367890 docker_stubs-0.1.1a0/docker-stubs/api/plugin.pyi
+-rw-r--r--   0        0        0      648 2024-05-02 14:01:35.368193 docker_stubs-0.1.1a0/docker-stubs/api/secret.pyi
+-rw-r--r--   0        0        0     2340 2024-05-02 14:01:35.368374 docker_stubs-0.1.1a0/docker-stubs/api/service.pyi
+-rw-r--r--   0        0        0     2071 2024-05-02 14:01:35.368549 docker_stubs-0.1.1a0/docker-stubs/api/swarm.pyi
+-rw-r--r--   0        0        0      751 2024-05-02 14:01:35.368709 docker_stubs-0.1.1a0/docker-stubs/api/volume.pyi
+-rw-r--r--   0        0        0     1932 2024-05-02 14:01:35.368882 docker_stubs-0.1.1a0/docker-stubs/auth.pyi
+-rw-r--r--   0        0        0     2574 2024-05-02 14:01:35.369055 docker_stubs-0.1.1a0/docker-stubs/client.pyi
+-rw-r--r--   0        0        0      574 2024-04-18 16:56:58.969412 docker_stubs-0.1.1a0/docker-stubs/constants.pyi
+-rw-r--r--   0        0        0       82 2024-04-16 17:18:30.922340 docker_stubs-0.1.1a0/docker-stubs/context/__init__.pyi
+-rw-r--r--   0        0        0     1083 2024-04-18 16:56:58.969629 docker_stubs-0.1.1a0/docker-stubs/context/api.pyi
+-rw-r--r--   0        0        0      710 2024-04-18 16:56:58.969831 docker_stubs-0.1.1a0/docker-stubs/context/config.pyi
+-rw-r--r--   0        0        0     1869 2024-05-02 14:01:35.369229 docker_stubs-0.1.1a0/docker-stubs/context/context.pyi
+-rw-r--r--   0        0        0      328 2024-04-16 17:23:52.298994 docker_stubs-0.1.1a0/docker-stubs/credentials/__init__.pyi
+-rw-r--r--   0        0        0       93 2024-04-16 17:18:30.923374 docker_stubs-0.1.1a0/docker-stubs/credentials/constants.pyi
+-rw-r--r--   0        0        0      166 2024-04-16 17:18:30.923499 docker_stubs-0.1.1a0/docker-stubs/credentials/errors.pyi
+-rw-r--r--   0        0        0      668 2024-05-02 14:01:35.369424 docker_stubs-0.1.1a0/docker-stubs/credentials/store.pyi
+-rw-r--r--   0        0        0       58 2024-04-18 16:56:58.970379 docker_stubs-0.1.1a0/docker-stubs/credentials/utils.pyi
+-rw-r--r--   0        0        0     2071 2024-05-02 14:01:35.369600 docker_stubs-0.1.1a0/docker-stubs/errors.pyi
+-rw-r--r--   0        0        0        0 2024-04-16 17:18:30.924543 docker_stubs-0.1.1a0/docker-stubs/models/__init__.pyi
+-rw-r--r--   0        0        0      423 2024-04-18 16:56:58.970819 docker_stubs-0.1.1a0/docker-stubs/models/configs.pyi
+-rw-r--r--   0        0        0    10405 2024-05-02 14:01:35.372072 docker_stubs-0.1.1a0/docker-stubs/models/containers.pyi
+-rw-r--r--   0        0        0     4347 2024-05-02 14:01:35.372359 docker_stubs-0.1.1a0/docker-stubs/models/images.pyi
+-rw-r--r--   0        0        0      843 2024-04-18 16:56:58.971423 docker_stubs-0.1.1a0/docker-stubs/models/networks.pyi
+-rw-r--r--   0        0        0      605 2024-05-02 14:01:35.372542 docker_stubs-0.1.1a0/docker-stubs/models/nodes.pyi
+-rw-r--r--   0        0        0      977 2024-04-18 16:56:58.971815 docker_stubs-0.1.1a0/docker-stubs/models/plugins.pyi
+-rw-r--r--   0        0        0     1046 2024-05-02 14:01:35.372714 docker_stubs-0.1.1a0/docker-stubs/models/resource.pyi
+-rw-r--r--   0        0        0      427 2024-04-18 16:56:58.972231 docker_stubs-0.1.1a0/docker-stubs/models/secrets.pyi
+-rw-r--r--   0        0        0     1534 2024-05-02 14:01:35.372886 docker_stubs-0.1.1a0/docker-stubs/models/services.pyi
+-rw-r--r--   0        0        0     1314 2024-05-02 14:01:35.373075 docker_stubs-0.1.1a0/docker-stubs/models/swarm.pyi
+-rw-r--r--   0        0        0      563 2024-04-18 16:56:58.972796 docker_stubs-0.1.1a0/docker-stubs/models/volumes.pyi
+-rw-r--r--   0        0        0      382 2024-04-18 16:56:58.973000 docker_stubs-0.1.1a0/docker-stubs/tls.pyi
+-rw-r--r--   0        0        0      223 2024-04-18 16:56:58.973175 docker_stubs-0.1.1a0/docker-stubs/transport/__init__.pyi
+-rw-r--r--   0        0        0      113 2024-04-16 17:18:30.928388 docker_stubs-0.1.1a0/docker-stubs/transport/basehttpadapter.pyi
+-rw-r--r--   0        0        0     1217 2024-05-02 14:01:35.373272 docker_stubs-0.1.1a0/docker-stubs/transport/npipeconn.pyi
+-rw-r--r--   0        0        0     1783 2024-04-16 17:23:52.359538 docker_stubs-0.1.1a0/docker-stubs/transport/npipesocket.pyi
+-rw-r--r--   0        0        0     1793 2024-04-16 17:23:52.355880 docker_stubs-0.1.1a0/docker-stubs/transport/sshconn.pyi
+-rw-r--r--   0        0        0     1166 2024-04-16 17:23:52.344844 docker_stubs-0.1.1a0/docker-stubs/transport/unixconn.pyi
+-rw-r--r--   0        0        0     1157 2024-04-16 17:23:52.339840 docker_stubs-0.1.1a0/docker-stubs/types/__init__.pyi
+-rw-r--r--   0        0        0      517 2024-05-02 14:01:35.373405 docker_stubs-0.1.1a0/docker-stubs/types/_io.pyi
+-rw-r--r--   0        0        0      397 2024-05-02 14:01:35.373574 docker_stubs-0.1.1a0/docker-stubs/types/base.pyi
+-rw-r--r--   0        0        0     7430 2024-05-02 14:01:35.374229 docker_stubs-0.1.1a0/docker-stubs/types/containers.pyi
+-rw-r--r--   0        0        0      245 2024-04-16 17:18:30.930436 docker_stubs-0.1.1a0/docker-stubs/types/daemon.pyi
+-rw-r--r--   0        0        0      323 2024-04-16 17:18:30.930584 docker_stubs-0.1.1a0/docker-stubs/types/healthcheck.pyi
+-rw-r--r--   0        0        0       58 2024-05-02 14:01:35.374400 docker_stubs-0.1.1a0/docker-stubs/types/misc_types.pyi
+-rw-r--r--   0        0        0     1108 2024-04-16 17:23:52.364686 docker_stubs-0.1.1a0/docker-stubs/types/networks.pyi
+-rw-r--r--   0        0        0     5856 2024-04-16 17:23:52.421277 docker_stubs-0.1.1a0/docker-stubs/types/services.pyi
+-rw-r--r--   0        0        0     1261 2024-04-16 17:23:52.363841 docker_stubs-0.1.1a0/docker-stubs/types/swarm.pyi
+-rw-r--r--   0        0        0     1274 2024-04-18 16:56:58.974290 docker_stubs-0.1.1a0/docker-stubs/utils/__init__.pyi
+-rw-r--r--   0        0        0     1147 2024-04-18 16:56:58.974544 docker_stubs-0.1.1a0/docker-stubs/utils/build.pyi
+-rw-r--r--   0        0        0      379 2024-04-16 17:18:30.932170 docker_stubs-0.1.1a0/docker-stubs/utils/config.pyi
+-rw-r--r--   0        0        0      162 2024-04-16 17:18:30.932297 docker_stubs-0.1.1a0/docker-stubs/utils/decorators.pyi
+-rw-r--r--   0        0        0       84 2024-04-16 17:18:30.932537 docker_stubs-0.1.1a0/docker-stubs/utils/fnmatch.pyi
+-rw-r--r--   0        0        0      586 2024-05-02 14:01:35.375153 docker_stubs-0.1.1a0/docker-stubs/utils/json_stream.pyi
+-rw-r--r--   0        0        0      347 2024-04-16 17:18:30.932833 docker_stubs-0.1.1a0/docker-stubs/utils/ports.pyi
+-rw-r--r--   0        0        0      383 2024-04-16 17:18:30.933261 docker_stubs-0.1.1a0/docker-stubs/utils/proxy.pyi
+-rw-r--r--   0        0        0      580 2024-04-16 17:18:30.933431 docker_stubs-0.1.1a0/docker-stubs/utils/socket.pyi
+-rw-r--r--   0        0        0     1560 2024-05-02 14:01:35.375311 docker_stubs-0.1.1a0/docker-stubs/utils/utils.pyi
+-rw-r--r--   0        0        0        0 2024-04-16 17:18:30.933791 docker_stubs-0.1.1a0/docker-stubs/version.pyi
+-rw-r--r--   0        0        0      624 2024-05-02 14:04:57.449021 docker_stubs-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 docker_stubs-0.1.1a0/PKG-INFO
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/build.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/build.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,54 @@
-from collections.abc import Generator
-from typing import AnyStr
+from typing import AnyStr, BinaryIO, Iterator
 from typing import TypedDict
 
 from .. import auth as auth, constants as constants, errors as errors, utils as utils
 from _typeshed import Incomplete
 
-from ..types.io import ResponseResult
-from ..types.io import PathType
-
+from ..types._io import PathType, ResponseResult
 
 class ContainerLimitsDict(TypedDict, total=False):
     memory: int
     memswap: int
     cpushares: int
     cpusetcpus: str
 
-
 class BuildApiMixin:
     def build(
         self,
         path: str | None = ...,
         tag: str | None = ...,
         quiet: bool = ...,
-        fileobj: Incomplete | None = ...,
+        fileobj: BinaryIO | None = ...,
         nocache: bool = ...,
         rm: bool = ...,
         timeout: int | None = ...,
         custom_context: bool = ...,
         encoding: str | None = ...,
         pull: bool = ...,
         forcerm: bool = ...,
         dockerfile: str | None = ...,
-        container_limits: dict | None = ...,
+        container_limits: dict[Incomplete, Incomplete] | None = ...,
         decode: bool = ...,
-        buildargs: dict | None = ...,
+        buildargs: dict[Incomplete, Incomplete] | None = ...,
         gzip: bool = ...,
         shmsize: int | None = ...,
-        labels: dict | None = ...,
-        cache_from: list | None = ...,
+        labels: dict[Incomplete, Incomplete] | None = ...,
+        cache_from: list[Incomplete] | None = ...,
         target: str | None = ...,
         network_mode: str | None = ...,
         squash: bool | None = ...,
-        extra_hosts: dict | None = ...,
+        extra_hosts: dict[Incomplete, Incomplete] | None = ...,
         platform: str | None = ...,
         isolation: str | None = ...,
         use_config_proxy: bool = ...,
-    ) -> Generator[ResponseResult, None, None]: ...
+    ) -> Iterator[ResponseResult]: ...
     def prune_builds(
         self,
-        filters: dict | None = ...,
+        filters: dict[Incomplete, Incomplete] | None = ...,
         keep_storage: int | None = ...,
         all: bool | None = ...,
-    ): ...
+    ) -> dict[Incomplete, Incomplete]: ...
 
-def process_dockerfile(dockerfile: PathType, path: PathType) -> tuple[PathType | None, AnyStr | None]: ...
+def process_dockerfile(
+    dockerfile: PathType[str], path: PathType[str]
+) -> tuple[PathType[str] | None, AnyStr | None]: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/client.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -65,24 +65,24 @@
     ServiceApiMixin,
     SwarmApiMixin,
     VolumeApiMixin,
 ):
     __attrs__: list[str]
     base_url: str
     timeout: int
-    credstore_env: dict
+    credstore_env: dict[Incomplete, Incomplete]
     def __init__(
         self,
         base_url: str | None = ...,
         version: str | None = ...,
         timeout: int = ...,
         tls: bool | TLSConfig = ...,
         user_agent: str = ...,
         num_pools: int | None = ...,
-        credstore_env: dict | None = ...,
+        credstore_env: dict[Incomplete, Incomplete] | None = ...,
         use_ssh_client: bool = ...,
         max_pool_size: int = ...,
     ) -> None: ...
     @property
     def api_version(self) -> str: ...
     def get_adapter(self, url: str) -> BaseAdapter: ...
     def reload_config(self, dockercfg_path: str | None = ...) -> None: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/config.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/secret.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Literal
+from docker.types import DriverConfig
 
-from .. import utils as utils
-from ..types.io import JsonDict
-from ..types.io import JsonList
-from ..types.misc_types import TrueOnSuccess
+from .. import errors as errors, utils as utils
+from _typeshed import Incomplete
 
+from ..types._io import JsonDict
+from ..types._io import JsonList
+from ..types.misc_types import TrueOnSuccess
 
-class ConfigApiMixin:
-    def create_config(
+class SecretApiMixin:
+    def create_secret(
         self,
         name: str,
         data: bytes,
-        labels: dict | None = ...,
-        templating: dict | None = ...,
+        labels: dict[str, Incomplete] | None = ...,
+        driver: DriverConfig | None = ...,
     ) -> JsonDict: ...
-    def inspect_config(self, id: str) -> JsonDict: ...
-    def remove_config(self, id) -> TrueOnSuccess: ...
-    def configs(self, filters: dict | None = ...) -> JsonList: ...
+    def inspect_secret(self, id: str) -> JsonDict: ...
+    def remove_secret(self, id: str) -> TrueOnSuccess: ...
+    def secrets(self, filters: dict[str, Incomplete] | None = ...) -> JsonList: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/container.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/container.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/api/daemon.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/daemon.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from datetime import datetime
 
 from docker.types import CancellableStream
-
-from .. import auth as auth, types as types, utils as utils
 from _typeshed import Incomplete
+from .. import auth as auth, types as types, utils as utils
 
-from ..types.io import JsonDict
-
+from ..types._io import JsonDict
 
 class DaemonApiMixin:
     def df(self) -> JsonDict: ...
     def events(
         self,
         since: int | datetime | None = ...,
         until: int | datetime | None = ...,
-        filters: dict | None = ...,
+        filters: dict[Incomplete, Incomplete] | None = ...,
         decode: bool | None = ...,
     ) -> CancellableStream: ...
     def info(self) -> JsonDict: ...
     def login(
         self,
         username: str,
         password: str | None = ...,
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/exec_api.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/exec_api.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from .. import errors as errors, utils as utils
 from ..types import CancellableStream as CancellableStream
-from _typeshed import Incomplete
-
-from ..types.io import JsonDict
-from ..types.io import Socket
 
+from ..types._io import JsonDict
+from ..types._io import Socket
 
 class ExecApiMixin:
     def exec_create(
         self,
         container: str,
-        cmd: str | list,
+        cmd: str | list[str] | tuple[str, ...],
         stdout: bool = ...,
         stderr: bool = ...,
         stdin: bool = ...,
         tty: bool = ...,
         privileged: bool = ...,
         user: str = ...,
-        environment: dict | list | None = ...,
+        environment: dict[str, str] | list[str] | tuple[str, ...] | None = ...,
         workdir: str | None = ...,
         detach_keys: str | None = ...,
     ) -> JsonDict: ...
     def exec_inspect(self, exec_id: str) -> JsonDict: ...
     def exec_resize(
         self, exec_id: str, height: int | None = ..., width: int | None = ...
     ) -> None: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/image.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/image.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import Collection
+from typing import BinaryIO, Collection, Iterator
 from typing import Generator
-from typing import IO
 
 from .. import auth as auth, errors as errors, utils as utils
 from ..constants import DEFAULT_DATA_CHUNK_SIZE as DEFAULT_DATA_CHUNK_SIZE
 from _typeshed import Incomplete
 
-from ..types.io import Json
-from ..types.io import JsonDict
-from ..types.io import ResponseResult
+from ..types._io import Json
+from ..types._io import JsonDict
+from ..types._io import ResponseResult
 from ..types.misc_types import TrueOnSuccess
 
-
 class ImageApiMixin:
-    def get_image(self, image: str, chunk_size: int = ...) -> Generator[ResponseResult, None, None]: ...
+    def get_image(
+        self, image: str, chunk_size: int = ...
+    ) -> Iterator[ResponseResult]: ...
     def history(self, image: str) -> str: ...
     def images(
         self,
         name: str | None = ...,
         quiet: bool = ...,
         all: bool = ...,
         filters: dict[str, Incomplete] | None = ...,
-    ) -> dict | list: ...
+    ) -> dict[Incomplete, Incomplete] | list[Incomplete]: ...
     def import_image(
         self,
-        src: str | IO | None = ...,
+        src: str | BinaryIO | None = ...,
         repository: str | None = ...,
         tag: str | None = ...,
         image: str | None = ...,
         changes: Incomplete | None = ...,
         stream_src: bool = ...,
     ) -> ResponseResult: ...
     def import_image_from_data(
@@ -36,62 +36,70 @@
         data: Collection[bytes],
         repository: str | None = ...,
         tag: str | None = ...,
         changes: Incomplete | None = ...,
     ) -> ResponseResult: ...
     def import_image_from_file(
         self,
-        filename,
+        filename: str,
         repository: Incomplete | None = ...,
         tag: Incomplete | None = ...,
         changes: Incomplete | None = ...,
     ) -> ResponseResult: ...
     def import_image_from_stream(
         self,
-        stream,
+        stream: Incomplete,
         repository: Incomplete | None = ...,
         tag: Incomplete | None = ...,
         changes: Incomplete | None = ...,
     ) -> ResponseResult: ...
     def import_image_from_url(
         self,
-        url,
+        url: str,
         repository: Incomplete | None = ...,
         tag: Incomplete | None = ...,
         changes: Incomplete | None = ...,
     ) -> ResponseResult: ...
     def import_image_from_image(
         self,
-        image,
+        image: Incomplete,
         repository: Incomplete | None = ...,
         tag: Incomplete | None = ...,
         changes: Incomplete | None = ...,
     ) -> ResponseResult: ...
     def inspect_image(self, image: str) -> JsonDict: ...
-    def inspect_distribution(self, image: str, auth_config: dict | None = ...) -> JsonDict: ...
-    def load_image(self, data, quiet: bool | None = ...) -> Generator[ResponseResult, None, None]: ...
-    def prune_images(self, filters: dict[str, Incomplete] | None = ...) -> dict[str, Incomplete]: ...
+    def inspect_distribution(
+        self, image: str, auth_config: dict[Incomplete, Incomplete] | None = ...
+    ) -> JsonDict: ...
+    def load_image(
+        self, data: Incomplete, quiet: bool | None = ...
+    ) -> Iterator[ResponseResult]: ...
+    def prune_images(
+        self, filters: dict[str, Incomplete] | None = ...
+    ) -> dict[str, Incomplete]: ...
     def pull(
         self,
         repository: str,
         tag: str | None = ...,
         stream: bool = ...,
         auth_config: dict[str, Incomplete] | None = ...,
         decode: bool = ...,
         platform: str | None = ...,
         all_tags: bool = ...,
-    ) -> str | Generator[ResponseResult, None, None]: ...
+    ) -> str | Iterator[ResponseResult]: ...
     def push(
         self,
         repository: str,
         tag: str | None = ...,
         stream: bool = ...,
         auth_config: dict[str, Incomplete] | None = ...,
         decode: bool = ...,
     ) -> str | Generator[ResponseResult, None, None]: ...
-    def remove_image(self, image: str, force: bool = ..., noprune: bool = ...) -> Json: ...
+    def remove_image(
+        self, image: str, force: bool = ..., noprune: bool = ...
+    ) -> Json: ...
     def search(self, term: str, limit: int | None = ...) -> list[JsonDict]: ...
     def tag(
         self, image: str, repository: str, tag: str | None = ..., force: bool = ...
     ) -> TrueOnSuccess: ...
 
-def is_file(src) -> bool: ...
+def is_file(src: Incomplete) -> bool: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/network.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/network.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-from typing import Literal
-from typing import TypedDict
-
 from docker.types import IPAMConfig
 
 from .. import utils as utils
 from ..errors import InvalidVersion as InvalidVersion
-from ..types.io import Json
-from ..types.io import JsonDict
+from ..types._io import Json, JsonDict
 from ..utils import (
     check_resource as check_resource,
     minimum_version as minimum_version,
     version_lt as version_lt,
 )
 from _typeshed import Incomplete
 
-
 class NetworkApiMixin:
     def networks(
         self,
         names: list[str] | None = ...,
         ids: list[str] | None = ...,
         filters: dict[str, Incomplete] | None = ...,
     ) -> JsonDict: ...
     def create_network(
         self,
         name: str,
         driver: str | None = ...,
-        options: dict | None = ...,
+        options: dict[Incomplete, Incomplete] | None = ...,
         ipam: IPAMConfig | None = ...,
         check_duplicate: bool | None = ...,
         internal: bool = ...,
         labels: dict[str, Incomplete] | None = ...,
         enable_ipv6: bool = ...,
         attachable: bool | None = ...,
         scope: str | None = ...,
         ingress: bool | None = ...,
     ) -> JsonDict: ...
-    def prune_networks(self, filters: FiltersDict | None = ...) -> JsonDict: ...
+    def prune_networks(self, filters: Incomplete | None = ...) -> JsonDict: ...
     def remove_network(self, net_id: str) -> None: ...
     def inspect_network(
         self, net_id: str, verbose: bool | None = ..., scope: str | None = ...
     ) -> Json: ...
     def connect_container_to_network(
         self,
         container: str,
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/plugin.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/plugin.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-from typing import Generator
+from typing import Generator, Iterator
 
 from .. import auth as auth, utils as utils
 from _typeshed import Incomplete
 
-from ..types.io import Json
-from ..types.io import JsonDict
-from ..types.io import ResponseResult
+from ..types._io import Json
+from ..types._io import JsonDict
+from ..types._io import ResponseResult
 from ..types.misc_types import TrueOnSuccess
 
-
 class PluginApiMixin:
-    def configure_plugin(self, name: str, options: dict) -> TrueOnSuccess: ...
-    def create_plugin(self, name: str, plugin_data_dir: str, gzip: bool = ...) -> TrueOnSuccess: ...
+    def configure_plugin(
+        self, name: str, options: dict[Incomplete, Incomplete]
+    ) -> TrueOnSuccess: ...
+    def create_plugin(
+        self, name: str, plugin_data_dir: str, gzip: bool = ...
+    ) -> TrueOnSuccess: ...
     def disable_plugin(self, name: str, force: bool = ...) -> TrueOnSuccess: ...
     def enable_plugin(self, name: str, timeout: int = ...) -> TrueOnSuccess: ...
     def inspect_plugin(self, name: str) -> JsonDict: ...
-    def pull_plugin(self, remote: str, privileges: list, name: str | None = ...) -> Generator[ResponseResult, None, None]: ...
+    def pull_plugin(
+        self, remote: str, privileges: list[Incomplete], name: str | None = ...
+    ) -> Iterator[ResponseResult]: ...
     def plugins(self) -> list[dict[str, Json]]: ...
     def plugin_privileges(self, name: str) -> list[dict[str, Json]]: ...
     def push_plugin(self, name: str) -> Generator[ResponseResult, None, None]: ...
     def remove_plugin(self, name: str, force: bool = ...) -> TrueOnSuccess: ...
-    def upgrade_plugin(self, name: str, remote: str, privileges: list) -> Generator[ResponseResult, None, None]: ...
+    def upgrade_plugin(
+        self, name: str, remote: str, privileges: list[Incomplete]
+    ) -> Iterator[ResponseResult]: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/secret.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/config.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from docker.types import DriverConfig
-
-from .. import errors as errors, utils as utils
-from _typeshed import Incomplete
-
-from ..types.io import JsonDict
-from ..types.io import JsonList
+from .. import utils as utils
+from ..types._io import JsonDict
+from ..types._io import JsonList
 from ..types.misc_types import TrueOnSuccess
+from _typeshed import Incomplete
 
-
-class SecretApiMixin:
-    def create_secret(
+class ConfigApiMixin:
+    def create_config(
         self,
         name: str,
         data: bytes,
-        labels: dict[str, Incomplete] | None = ...,
-        driver: DriverConfig | None = ...,
+        labels: dict[Incomplete, Incomplete] | None = ...,
+        templating: dict[Incomplete, Incomplete] | None = ...,
     ) -> JsonDict: ...
-    def inspect_secret(self, id: str) -> JsonDict: ...
-    def remove_secret(self, id: str) -> TrueOnSuccess: ...
-    def secrets(self, filters: dict[str, Incomplete] | None = ...) -> JsonList: ...
+    def inspect_config(self, id: str) -> JsonDict: ...
+    def remove_config(self, id: str) -> TrueOnSuccess: ...
+    def configs(
+        self, filters: dict[Incomplete, Incomplete] | None = ...
+    ) -> JsonList: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/service.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/service.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generator
+from typing import Generator, Iterator, Literal
 
 from docker.types import RollbackConfig
 
 from docker.types import EndpointConfig
 
 from docker.types import EndpointSpec
 
@@ -10,32 +10,33 @@
 
 from docker.types import TaskTemplate
 
 from .. import auth as auth, errors as errors, utils as utils
 from ..types import ServiceMode as ServiceMode
 from _typeshed import Incomplete
 
-from ..types.io import JsonDict
+from ..types._io import JsonDict
 from ..types.misc_types import TrueOnSuccess
 
-
 class ServiceApiMixin:
     def create_service(
         self,
         task_template: TaskTemplate,
         name: str | None = ...,
         labels: dict[str, Incomplete] | None = ...,
         mode: ServiceMode | None = ...,
         update_config: UpdateConfig | None = ...,
         networks: list[str] | None = ...,
         endpoint_config: EndpointConfig | None = ...,
         endpoint_spec: EndpointSpec | None = ...,
         rollback_config: RollbackConfig | None = ...,
     ) -> JsonDict: ...
-    def inspect_service(self, service: str, insert_defaults: bool | None = ...) -> JsonDict: ...
+    def inspect_service(
+        self, service: str, insert_defaults: bool | None = ...
+    ) -> JsonDict: ...
     def inspect_task(self, task: str) -> JsonDict: ...
     def remove_service(self, service: str) -> TrueOnSuccess: ...
     def services(
         self, filters: dict[str, Incomplete] | None = ..., status: bool | None = ...
     ) -> list[JsonDict]: ...
     def service_logs(
         self,
@@ -44,24 +45,24 @@
         follow: bool = ...,
         stdout: bool = ...,
         stderr: bool = ...,
         since: int = ...,
         timestamps: bool = ...,
         tail: str = ...,
         is_tty: bool | None = ...,
-    ) -> Generator[bytes, None, None]: ...
+    ) -> Iterator[bytes]: ...
     def tasks(self, filters: dict[str, Incomplete] | None = ...) -> list[JsonDict]: ...
     def update_service(
         self,
         service: str,
         version: int,
         task_template: TaskTemplate | None = ...,
         name: str | None = ...,
-        labels: dict | None = ...,
+        labels: dict[Incomplete, Incomplete] | None = ...,
         mode: ServiceMode | None = ...,
         update_config: UpdateConfig | None = ...,
         networks: list[str] | None = ...,
         endpoint_config: EndpointConfig | None = ...,
         endpoint_spec: EndpointSpec | None = ...,
         fetch_current_spec: bool = ...,
         rollback_config: RollbackConfig | None = ...,
-    ): ...
+    ) -> dict[Literal["Warnings"], Incomplete]: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/swarm.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/swarm.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 from .. import errors as errors, types as types, utils as utils
 from ..constants import (
     DEFAULT_SWARM_ADDR_POOL as DEFAULT_SWARM_ADDR_POOL,
     DEFAULT_SWARM_SUBNET_SIZE as DEFAULT_SWARM_SUBNET_SIZE,
 )
 from _typeshed import Incomplete
 
-from ..types.io import JsonDict
+from ..types._io import JsonDict
 from ..types.misc_types import TrueOnSuccess
 
 log: Incomplete
 
 class SwarmApiMixin:
-    def create_swarm_spec(self, *args, **kwargs) -> SwarmSpec: ...
-    def get_unlock_key(self) -> dict: ...
+    def create_swarm_spec(
+        self, *args: Incomplete, **kwargs: Incomplete
+    ) -> SwarmSpec: ...
+    def get_unlock_key(self) -> dict[Incomplete, Incomplete]: ...
     def init_swarm(
         self,
         advertise_addr: str | None = ...,
         listen_addr: str = ...,
         force_new_cluster: bool = ...,
-        swarm_spec: dict | None = ...,
+        swarm_spec: dict[Incomplete, Incomplete] | None = ...,
         default_addr_pool: list[str] | None = ...,
         subnet_size: int | None = ...,
         data_path_addr: str | None = ...,
         data_path_port: int | None = ...,
     ) -> str: ...
     def inspect_swarm(self) -> JsonDict: ...
     def inspect_node(self, node_id: str) -> JsonDict: ...
@@ -33,19 +35,26 @@
         remote_addrs: list[str],
         join_token: str,
         listen_addr: str = ...,
         advertise_addr: str | None = ...,
         data_path_addr: str | None = ...,
     ) -> TrueOnSuccess: ...
     def leave_swarm(self, force: bool = ...) -> TrueOnSuccess: ...
-    def nodes(self, filters: dict | None = ...) -> list[JsonDict]: ...
+    def nodes(
+        self, filters: dict[Incomplete, Incomplete] | None = ...
+    ) -> list[JsonDict]: ...
     def remove_node(self, node_id: str, force: bool = ...) -> TrueOnSuccess: ...
     def unlock_swarm(self, key: str) -> TrueOnSuccess: ...
-    def update_node(self, node_id: str, version: int, node_spec: dict | None = ...) -> TrueOnSuccess: ...
+    def update_node(
+        self,
+        node_id: str,
+        version: int,
+        node_spec: dict[Incomplete, Incomplete] | None = ...,
+    ) -> TrueOnSuccess: ...
     def update_swarm(
         self,
         version: int,
-        swarm_spec: dict | None = ...,
+        swarm_spec: dict[Incomplete, Incomplete] | None = ...,
         rotate_worker_token: bool = ...,
         rotate_manager_token: bool = ...,
         rotate_manager_unlock_key: bool = ...,
     ) -> TrueOnSuccess: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/api/volume.pyi` & `docker_stubs-0.1.1a0/docker-stubs/api/volume.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from .. import errors as errors, utils as utils
 from _typeshed import Incomplete
 
-from ..types.io import JsonDict
-
+from ..types._io import JsonDict
 
 class VolumeApiMixin:
-    def volumes(self, filters: dict | None = ...) -> JsonDict: ...
+    def volumes(
+        self, filters: dict[Incomplete, Incomplete] | None = ...
+    ) -> JsonDict: ...
     def create_volume(
         self,
         name: str | None = ...,
         driver: str | None = ...,
-        driver_opts: dict | None = ...,
-        labels: dict | None = ...,
+        driver_opts: dict[Incomplete, Incomplete] | None = ...,
+        labels: dict[Incomplete, Incomplete] | None = ...,
     ) -> JsonDict: ...
     def inspect_volume(self, name: str) -> JsonDict: ...
-    def prune_volumes(self, filters: dict | None = ...) -> dict: ...
+    def prune_volumes(
+        self, filters: dict[Incomplete, Incomplete] | None = ...
+    ) -> dict[Incomplete, Incomplete]: ...
     def remove_volume(self, name: str, force: bool = ...) -> None: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/auth.pyi` & `docker_stubs-0.1.1a0/docker-stubs/auth.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from . import credentials as credentials, errors as errors
-from .types.io import PathType
-from .types.io import SupportsEncode
+from .types._io import PathType
 from .utils import config as config
 from _typeshed import Incomplete
 
 INDEX_NAME: str
 INDEX_URL: Incomplete
 TOKEN_USERNAME: str
 log: Incomplete
@@ -17,25 +16,30 @@
 
 class AuthConfig(dict):
     def __init__(self, dct: dict, credstore_env: Incomplete | None = ...): ...
     @classmethod
     def parse_auth(cls, entries: dict, raise_on_error: bool = ...) -> dict: ...
     @classmethod
     def load_config(
-        cls, config_path: PathType, config_dict: dict, credstore_env: Incomplete | None = ...
+        cls,
+        config_path: PathType,
+        config_dict: dict,
+        credstore_env: Incomplete | None = ...,
     ) -> AuthConfig: ...
     @property
     def auths(self) -> dict: ...
     @property
     def creds_store(self) -> Incomplete | None: ...
     @property
     def cred_helpers(self) -> dict: ...
     @property
     def is_empty(self) -> bool: ...
-    def resolve_authconfig(self, registry: Incomplete | None = ...) -> Incomplete | None: ...
+    def resolve_authconfig(
+        self, registry: Incomplete | None = ...
+    ) -> Incomplete | None: ...
     def get_credential_store(self, registry: str) -> Incomplete: ...
     def get_all_credentials(self) -> Incomplete: ...
     def add_auth(self, reg, data) -> None: ...
 
 def resolve_authconfig(
     authconfig,
     registry: Incomplete | None = ...,
```

### Comparing `docker_stubs-0.1.0/docker-stubs/client.pyi` & `docker_stubs-0.1.1a0/docker-stubs/client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Callable
-
 from docker.types import CancellableStream
 
 from .api.client import APIClient as APIClient
 from .constants import (
     DEFAULT_MAX_POOL_SIZE as DEFAULT_MAX_POOL_SIZE,
     DEFAULT_TIMEOUT_SECONDS as DEFAULT_TIMEOUT_SECONDS,
 )
@@ -18,17 +16,17 @@
 from .models.swarm import Swarm as Swarm
 from .models.volumes import VolumeCollection as VolumeCollection
 from .utils import kwargs_from_env as kwargs_from_env
 from _typeshed import Incomplete
 
 class DockerClient:
     api: APIClient
-    def __init__(self, *args, **kwargs) -> None: ...
+    def __init__(self, *args: Incomplete, **kwargs: Incomplete) -> None: ...
     @classmethod
-    def from_env(cls, **kwargs) -> DockerClient: ...
+    def from_env(cls, **kwargs: Incomplete) -> DockerClient: ...
     @property
     def configs(self) -> ConfigCollection: ...
     @property
     def containers(self) -> ContainerCollection: ...
     @property
     def images(self) -> ImageCollection: ...
     @property
@@ -41,17 +39,30 @@
     def secrets(self) -> SecretCollection: ...
     @property
     def services(self) -> ServiceCollection: ...
     @property
     def swarm(self) -> Swarm: ...
     @property
     def volumes(self) -> VolumeCollection: ...
-    def events(self, *args, **kwargs) -> CancellableStream: ...
-    def df(self) -> dict: ...
-    def info(self, *args, **kwargs) -> dict: ...
-    def login(self, *args, **kwargs) -> dict: ...
-    def ping(self, *args, **kwargs) -> bool: ...
-    def version(self, *args, **kwargs) -> dict: ...
+    def events(self, *args: Incomplete, **kwargs: Incomplete) -> CancellableStream: ...
+    def df(self) -> dict[Incomplete, Incomplete]: ...
+    def info(
+        self, *args: Incomplete, **kwargs: Incomplete
+    ) -> dict[Incomplete, Incomplete]: ...
+    def login(
+        self, *args: Incomplete, **kwargs: Incomplete
+    ) -> dict[Incomplete, Incomplete]: ...
+    def ping(self, *args: Incomplete, **kwargs: Incomplete) -> bool: ...
+    def version(
+        self, *args: Incomplete, **kwargs: Incomplete
+    ) -> dict[Incomplete, Incomplete]: ...
     def close(self) -> None: ...
-    def __getattr__(self, name) -> None: ...
+    def __getattr__(self, name: str) -> None: ...
 
-from_env: Callable[[], DockerClient]
+def from_env(
+    *,
+    assert_hostname: bool = ...,
+    max_pool_size: int = ...,
+    timeout: int = ...,
+    use_ssh_client: bool = ...,
+    version: str | None = ...
+) -> DockerClient: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/constants.pyi` & `docker_stubs-0.1.1a0/docker-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/context/api.pyi` & `docker_stubs-0.1.1a0/docker-stubs/context/api.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/context/config.pyi` & `docker_stubs-0.1.1a0/docker-stubs/context/config.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/context/context.pyi` & `docker_stubs-0.1.1a0/docker-stubs/context/context.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -6,55 +6,54 @@
     get_meta_dir as get_meta_dir,
     get_meta_file as get_meta_file,
     get_tls_dir as get_tls_dir,
 )
 from docker.errors import ContextException as ContextException
 from docker.tls import TLSConfig as TLSConfig
 
-
-
-
 class Context:
     name: str
     context_type: Incomplete | None
     orchestrator: str | None
-    endpoints: dict
-    tls_cfg: dict
+    endpoints: dict[Incomplete, Incomplete]
+    tls_cfg: dict[Incomplete, Incomplete]
     meta_path: str
     tls_path: str
     def __init__(
         self,
-        name,
+        name: str,
         orchestrator: str | None = ...,
         host: str | None = ...,
-        endpoints: dict | None = ...,
+        endpoints: dict[Incomplete, Incomplete] | None = ...,
         tls: bool = ...,
     ) -> None: ...
     def set_endpoint(
         self,
         name: str = ...,
         host: str | None = ...,
-        tls_cfg: dict | None = ...,
+        tls_cfg: dict[Incomplete, Incomplete] | None = ...,
         skip_tls_verify: bool = ...,
         def_namespace: str | None = ...,
     ) -> None: ...
-    def inspect(self) -> dict: ...
+    def inspect(self) -> dict[Incomplete, Incomplete]: ...
     @classmethod
     def load_context(cls, name: str) -> Context | None: ...
     def save(self) -> None: ...
     def remove(self) -> None: ...
-    def __call__(self) -> dict: ...
+    def __call__(self) -> dict[Incomplete, Incomplete]: ...
     def is_docker_host(self) -> bool: ...
     @property
     def Name(self) -> str: ...
     @property
     def Host(self) -> Incomplete | None: ...
     @property
     def Orchestrator(self) -> str: ...
     @property
-    def Metadata(self) -> dict: ...
+    def Metadata(self) -> dict[Incomplete, Incomplete]: ...
     @property
     def TLSConfig(self) -> Incomplete | None: ...
     @property
-    def TLSMaterial(self) -> dict[Literal["TLSMaterial"], dict]: ...
+    def TLSMaterial(
+        self,
+    ) -> dict[Literal["TLSMaterial"], dict[Incomplete, Incomplete]]: ...
     @property
-    def Storage(self) -> dict[Literal["Storage"], dict]: ...
+    def Storage(self) -> dict[Literal["Storage"], dict[Incomplete, Incomplete]]: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/credentials/store.pyi` & `docker_stubs-0.1.1a0/docker-stubs/credentials/store.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from . import constants as constants, errors as errors
 from .utils import create_environment_dict as create_environment_dict
 from _typeshed import Incomplete
 
-from ..types.io import JsonString
-from ..types.io import SupportsEncode
-
+from ..types._io import JsonString
+from ..types._io import SupportsEncode
 
 class Store:
     program: str
     exe: str
     environment: Incomplete
-    def __init__(self, program, environment: Incomplete | None = ...) -> None: ...
+    def __init__(self, program: str, environment: Incomplete | None = ...) -> None: ...
     def get(self, server: bytes | SupportsEncode) -> JsonString: ...
-    def store(self, server: Incomplete, username: Incomplete, secret: Incomplete) -> Incomplete: ...
+    def store(
+        self, server: Incomplete, username: Incomplete, secret: Incomplete
+    ) -> Incomplete: ...
     def erase(self, server: Incomplete) -> None: ...
     def list(self) -> JsonString: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/errors.pyi` & `docker_stubs-0.1.1a0/docker-stubs/errors.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import requests
 from _typeshed import Incomplete
 
-from docker.types.io import Response
-
+from docker.types._io import Response
 
 class DockerException(Exception): ...
 
 def create_api_error_from_http_exception(e) -> None: ...
 
 class APIError(requests.exceptions.HTTPError, DockerException):
     response: Response
```

### Comparing `docker_stubs-0.1.0/docker-stubs/models/networks.pyi` & `docker_stubs-0.1.1a0/docker-stubs/models/networks.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/models/plugins.pyi` & `docker_stubs-0.1.1a0/docker-stubs/models/plugins.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/models/resource.pyi` & `docker_stubs-0.1.1a0/docker-stubs/models/resource.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from _typeshed import Incomplete
 from typing import Type
 
-
 class Model:
     id_attribute: str
     client: Incomplete
     collection: Incomplete
-    attrs: dict
+    attrs: dict[Incomplete, Incomplete]
     def __init__(
         self,
-        attrs: dict | None = ...,
+        attrs: dict[Incomplete, Incomplete] | None = ...,
         client: Incomplete | None = ...,
         collection: Incomplete | None = ...,
     ) -> None: ...
     def __eq__(self, other: object) -> bool: ...
-    def __hash__(self) -> hash: ...
+    def __hash__(self) -> int: ...
     @property
     def id(self) -> str: ...
     @property
     def short_id(self) -> str: ...
     def reload(self) -> None: ...
 
 class Collection:
     model: Type[Model] | None
     client: Incomplete
     def __init__(self, client: Incomplete | None = ...) -> None: ...
-    def __call__(self, *args, **kwargs) -> None: ...
+    def __call__(self, *args: Incomplete, **kwargs: Incomplete) -> None: ...
     def list(self) -> None: ...
-    def get(self, key) -> None: ...
-    def create(self, attrs) -> None: ...
-    def prepare_model(self, attrs: Model | dict | None = ...) -> Model: ...
+    def get(self, key: str) -> None: ...
+    def create(self, attrs: Incomplete) -> None: ...
+    def prepare_model(
+        self, attrs: Model | dict[Incomplete, Incomplete] | None = ...
+    ) -> Model: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/models/services.pyi` & `docker_stubs-0.1.1a0/docker-stubs/models/services.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generator
+from typing import Iterator
 
 from .resource import Collection as Collection, Model as Model
 from _typeshed import Incomplete
 from docker.errors import (
     InvalidArgument as InvalidArgument,
     create_unexpected_kwargs_error as create_unexpected_kwargs_error,
 )
@@ -10,31 +10,34 @@
     ContainerSpec as ContainerSpec,
     Placement as Placement,
     ServiceMode as ServiceMode,
     TaskTemplate as TaskTemplate,
 )
 from ..types.misc_types import TrueOnSuccess
 
-
 class Service(Model):
     id_attribute: str
     @property
     def name(self) -> str: ...
     @property
     def version(self) -> str: ...
     def remove(self) -> None: ...
-    def tasks(self, filters: dict | None = ...) -> list[dict]: ...
-    def logs(self, **kwargs) -> Generator[bytes, None, None]: ...
-    def update(self, **kwargs) -> None: ...
+    def tasks(
+        self, filters: dict[Incomplete, Incomplete] | None = ...
+    ) -> list[dict[Incomplete, Incomplete]]: ...
+    def logs(self, **kwargs: Incomplete) -> Iterator[bytes]: ...
+    def update(self, **kwargs: Incomplete) -> None: ...
     def scale(self, replicas: int) -> TrueOnSuccess: ...
     def force_update(self) -> TrueOnSuccess: ...
 
 class ServiceCollection(Collection):
     model = Service
-    def create(self, image: str, command: list[str] | str | None = ..., **kwargs) -> Service: ...
-    def get(self, service_id: str, insert_defaults: bool | None = ...) -> Service: ...
-    def list(self, **kwargs) -> list[Service]: ...
+    def create(  # type: ignore[override]
+        self, image: str, command: list[str] | str | None = ..., **kwargs: Incomplete
+    ) -> Service: ...
+    def get(self, service_id: str, insert_defaults: bool | None = ...) -> Service: ...  # type: ignore[override]
+    def list(self, **kwargs: Incomplete) -> list[Service]: ...  # type: ignore[override]
 
 CONTAINER_SPEC_KWARGS: list[str]
 TASK_TEMPLATE_KWARGS: list[str]
 CREATE_SERVICE_KWARGS: list[str]
 PLACEMENT_KWARGS: list[str]
```

### Comparing `docker_stubs-0.1.0/docker-stubs/models/volumes.pyi` & `docker_stubs-0.1.1a0/docker-stubs/models/volumes.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/transport/npipeconn.pyi` & `docker_stubs-0.1.1a0/docker-stubs/transport/npipeconn.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from typing import Any
-from typing import NewType
 
 import urllib3.connection
-from .. import constants as constants
 from .npipesocket import NpipeSocket as NpipeSocket
 from _typeshed import Incomplete
 from docker.transport.basehttpadapter import BaseHTTPAdapter as BaseHTTPAdapter
 
-
-RecentlyUsedContainer = NewType('RecentlyUsedContainer', Any)
-
+RecentlyUsedContainer = Incomplete
 
 class NpipeHTTPConnection(urllib3.connection.HTTPConnection):
     npipe_path: str
     timeout: int
     def __init__(self, npipe_path: str, timeout: int = ...) -> None: ...
     sock: Incomplete
     def connect(self) -> None: ...
 
 class NpipeHTTPConnectionPool(urllib3.connectionpool.HTTPConnectionPool):
     npipe_path: str
     timeout: int
-    def __init__(self, npipe_path: str, timeout: int = ..., maxsize: int = ...) -> None: ...
+    def __init__(
+        self, npipe_path: str, timeout: int = ..., maxsize: int = ...
+    ) -> None: ...
 
 class NpipeHTTPAdapter(BaseHTTPAdapter):
     __attrs__: list[str]
     npipe_path: str
     timeout: int
     max_pool_size: int
     pools: RecentlyUsedContainer
     def __init__(
-        self, base_url: str, timeout: int = ..., pool_connections: int = ..., max_pool_size: int = ...
+        self,
+        base_url: str,
+        timeout: int = ...,
+        pool_connections: int = ...,
+        max_pool_size: int = ...,
     ) -> None: ...
-    def get_connection(self, url: str, proxies: Incomplete | None = ...): ...
-    def request_url(self, request, proxies): ...
+    def get_connection(
+        self, url: str, proxies: Incomplete | None = ...
+    ) -> NpipeHTTPConnectionPool: ...
+    def request_url(self, request: Any, proxies: Any) -> str: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/transport/npipesocket.pyi` & `docker_stubs-0.1.1a0/docker-stubs/transport/npipesocket.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/transport/sshconn.pyi` & `docker_stubs-0.1.1a0/docker-stubs/transport/sshconn.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/transport/unixconn.pyi` & `docker_stubs-0.1.1a0/docker-stubs/transport/unixconn.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/types/__init__.pyi` & `docker_stubs-0.1.1a0/docker-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/types/containers.pyi` & `docker_stubs-0.1.1a0/docker-stubs/types/services.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,160 +1,198 @@
 from .. import errors as errors
-from ..utils.utils import (
-    convert_port_bindings as convert_port_bindings,
-    convert_tmpfs_mounts as convert_tmpfs_mounts,
-    convert_volume_binds as convert_volume_binds,
+from ..constants import IS_WINDOWS_PLATFORM as IS_WINDOWS_PLATFORM
+from ..utils import (
+    check_resource as check_resource,
+    convert_service_networks as convert_service_networks,
     format_environment as format_environment,
     format_extra_hosts as format_extra_hosts,
-    normalize_links as normalize_links,
     parse_bytes as parse_bytes,
-    parse_devices as parse_devices,
     split_command as split_command,
-    version_gte as version_gte,
-    version_lt as version_lt,
 )
-from .base import DictType as DictType
-from .healthcheck import Healthcheck as Healthcheck
 from _typeshed import Incomplete
 
-class LogConfigTypesEnum:
-    JSON: Incomplete
-    SYSLOG: Incomplete
-    JOURNALD: Incomplete
-    GELF: Incomplete
-    FLUENTD: Incomplete
-    NONE: Incomplete
-
-class LogConfig(DictType):
-    types = LogConfigTypesEnum
-    def __init__(self, **kwargs) -> None: ...
-    @property
-    def type(self): ...
-    @property
-    def config(self): ...
-    def set_config_value(self, key, value) -> None: ...
-    def unset_config(self, key) -> None: ...
-
-class Ulimit(DictType):
-    def __init__(self, **kwargs) -> None: ...
-    @property
-    def name(self): ...
-    @property
-    def soft(self): ...
-    @property
-    def hard(self): ...
-
-class DeviceRequest(DictType):
-    def __init__(self, **kwargs) -> None: ...
-    @property
-    def driver(self): ...
+class TaskTemplate(dict):
+    def __init__(
+        self,
+        container_spec,
+        resources: Incomplete | None = ...,
+        restart_policy: Incomplete | None = ...,
+        placement: Incomplete | None = ...,
+        log_driver: Incomplete | None = ...,
+        networks: Incomplete | None = ...,
+        force_update: Incomplete | None = ...,
+    ) -> None: ...
     @property
-    def count(self): ...
+    def container_spec(self): ...
     @property
-    def device_ids(self): ...
+    def resources(self): ...
     @property
-    def capabilities(self): ...
+    def restart_policy(self): ...
     @property
-    def options(self): ...
+    def placement(self): ...
 
-class HostConfig(dict):
+class ContainerSpec(dict):
     def __init__(
         self,
-        version,
-        binds: Incomplete | None = ...,
-        port_bindings: Incomplete | None = ...,
-        lxc_conf: Incomplete | None = ...,
-        publish_all_ports: bool = ...,
-        links: Incomplete | None = ...,
-        privileged: bool = ...,
-        dns: Incomplete | None = ...,
-        dns_search: Incomplete | None = ...,
-        volumes_from: Incomplete | None = ...,
-        network_mode: Incomplete | None = ...,
-        restart_policy: Incomplete | None = ...,
+        image,
+        command: Incomplete | None = ...,
+        args: Incomplete | None = ...,
+        hostname: Incomplete | None = ...,
+        env: Incomplete | None = ...,
+        workdir: Incomplete | None = ...,
+        user: Incomplete | None = ...,
+        labels: Incomplete | None = ...,
+        mounts: Incomplete | None = ...,
+        stop_grace_period: Incomplete | None = ...,
+        secrets: Incomplete | None = ...,
+        tty: Incomplete | None = ...,
+        groups: Incomplete | None = ...,
+        open_stdin: Incomplete | None = ...,
+        read_only: Incomplete | None = ...,
+        stop_signal: Incomplete | None = ...,
+        healthcheck: Incomplete | None = ...,
+        hosts: Incomplete | None = ...,
+        dns_config: Incomplete | None = ...,
+        configs: Incomplete | None = ...,
+        privileges: Incomplete | None = ...,
+        isolation: Incomplete | None = ...,
+        init: Incomplete | None = ...,
         cap_add: Incomplete | None = ...,
         cap_drop: Incomplete | None = ...,
-        devices: Incomplete | None = ...,
-        extra_hosts: Incomplete | None = ...,
-        read_only: Incomplete | None = ...,
-        pid_mode: Incomplete | None = ...,
-        ipc_mode: Incomplete | None = ...,
-        security_opt: Incomplete | None = ...,
-        ulimits: Incomplete | None = ...,
-        log_config: Incomplete | None = ...,
+        sysctls: Incomplete | None = ...,
+    ) -> None: ...
+
+class Mount(dict):
+    def __init__(
+        self,
+        target,
+        source,
+        type: str = ...,
+        read_only: bool = ...,
+        consistency: Incomplete | None = ...,
+        propagation: Incomplete | None = ...,
+        no_copy: bool = ...,
+        labels: Incomplete | None = ...,
+        driver_config: Incomplete | None = ...,
+        tmpfs_size: Incomplete | None = ...,
+        tmpfs_mode: Incomplete | None = ...,
+    ) -> None: ...
+    @classmethod
+    def parse_mount_string(cls, string): ...
+
+class Resources(dict):
+    def __init__(
+        self,
+        cpu_limit: Incomplete | None = ...,
         mem_limit: Incomplete | None = ...,
-        memswap_limit: Incomplete | None = ...,
+        cpu_reservation: Incomplete | None = ...,
         mem_reservation: Incomplete | None = ...,
-        kernel_memory: Incomplete | None = ...,
-        mem_swappiness: Incomplete | None = ...,
-        cgroup_parent: Incomplete | None = ...,
-        group_add: Incomplete | None = ...,
-        cpu_quota: Incomplete | None = ...,
-        cpu_period: Incomplete | None = ...,
-        blkio_weight: Incomplete | None = ...,
-        blkio_weight_device: Incomplete | None = ...,
-        device_read_bps: Incomplete | None = ...,
-        device_write_bps: Incomplete | None = ...,
-        device_read_iops: Incomplete | None = ...,
-        device_write_iops: Incomplete | None = ...,
-        oom_kill_disable: bool = ...,
-        shm_size: Incomplete | None = ...,
-        sysctls: Incomplete | None = ...,
-        tmpfs: Incomplete | None = ...,
-        oom_score_adj: Incomplete | None = ...,
-        dns_opt: Incomplete | None = ...,
-        cpu_shares: Incomplete | None = ...,
-        cpuset_cpus: Incomplete | None = ...,
-        userns_mode: Incomplete | None = ...,
-        uts_mode: Incomplete | None = ...,
-        pids_limit: Incomplete | None = ...,
-        isolation: Incomplete | None = ...,
-        auto_remove: bool = ...,
-        storage_opt: Incomplete | None = ...,
-        init: Incomplete | None = ...,
-        init_path: Incomplete | None = ...,
-        volume_driver: Incomplete | None = ...,
-        cpu_count: Incomplete | None = ...,
-        cpu_percent: Incomplete | None = ...,
-        nano_cpus: Incomplete | None = ...,
-        cpuset_mems: Incomplete | None = ...,
-        runtime: Incomplete | None = ...,
-        mounts: Incomplete | None = ...,
-        cpu_rt_period: Incomplete | None = ...,
-        cpu_rt_runtime: Incomplete | None = ...,
-        device_cgroup_rules: Incomplete | None = ...,
-        device_requests: Incomplete | None = ...,
-        cgroupns: Incomplete | None = ...,
+        generic_resources: Incomplete | None = ...,
+    ) -> None: ...
+
+class UpdateConfig(dict):
+    def __init__(
+        self,
+        parallelism: int = ...,
+        delay: Incomplete | None = ...,
+        failure_action: str = ...,
+        monitor: Incomplete | None = ...,
+        max_failure_ratio: Incomplete | None = ...,
+        order: Incomplete | None = ...,
     ) -> None: ...
 
-def host_config_type_error(param, param_value, expected): ...
-def host_config_version_error(param, version, less_than: bool = ...): ...
-def host_config_value_error(param, param_value): ...
-def host_config_incompatible_error(param, param_value, incompatible_param): ...
+class RollbackConfig(UpdateConfig): ...
+
+class RestartConditionTypesEnum:
+    NONE: Incomplete
+    ON_FAILURE: Incomplete
+    ANY: Incomplete
 
-class ContainerConfig(dict):
+class RestartPolicy(dict):
+    condition_types = RestartConditionTypesEnum
     def __init__(
         self,
-        version,
-        image,
-        command,
-        hostname: Incomplete | None = ...,
-        user: Incomplete | None = ...,
-        detach: bool = ...,
-        stdin_open: bool = ...,
-        tty: bool = ...,
-        ports: Incomplete | None = ...,
-        environment: Incomplete | None = ...,
-        volumes: Incomplete | None = ...,
-        network_disabled: bool = ...,
-        entrypoint: Incomplete | None = ...,
-        working_dir: Incomplete | None = ...,
-        domainname: Incomplete | None = ...,
-        host_config: Incomplete | None = ...,
-        mac_address: Incomplete | None = ...,
-        labels: Incomplete | None = ...,
-        stop_signal: Incomplete | None = ...,
-        networking_config: Incomplete | None = ...,
-        healthcheck: Incomplete | None = ...,
-        stop_timeout: Incomplete | None = ...,
-        runtime: Incomplete | None = ...,
+        condition=...,
+        delay: int = ...,
+        max_attempts: int = ...,
+        window: int = ...,
+    ) -> None: ...
+
+class DriverConfig(dict):
+    def __init__(self, name, options: Incomplete | None = ...) -> None: ...
+
+class EndpointSpec(dict):
+    def __init__(
+        self, mode: Incomplete | None = ..., ports: Incomplete | None = ...
+    ) -> None: ...
+
+def convert_service_ports(ports): ...
+
+class ServiceMode(dict):
+    mode: Incomplete
+    def __init__(
+        self,
+        mode,
+        replicas: Incomplete | None = ...,
+        concurrency: Incomplete | None = ...,
+    ) -> None: ...
+    @property
+    def replicas(self): ...
+
+class SecretReference(dict):
+    def __init__(
+        self,
+        secret_id,
+        secret_name,
+        filename: Incomplete | None = ...,
+        uid: Incomplete | None = ...,
+        gid: Incomplete | None = ...,
+        mode: int = ...,
+    ) -> None: ...
+
+class ConfigReference(dict):
+    def __init__(
+        self,
+        config_id,
+        config_name,
+        filename: Incomplete | None = ...,
+        uid: Incomplete | None = ...,
+        gid: Incomplete | None = ...,
+        mode: int = ...,
+    ) -> None: ...
+
+class Placement(dict):
+    def __init__(
+        self,
+        constraints: Incomplete | None = ...,
+        preferences: Incomplete | None = ...,
+        platforms: Incomplete | None = ...,
+        maxreplicas: Incomplete | None = ...,
+    ) -> None: ...
+
+class PlacementPreference(dict):
+    def __init__(self, strategy, descriptor) -> None: ...
+
+class DNSConfig(dict):
+    def __init__(
+        self,
+        nameservers: Incomplete | None = ...,
+        search: Incomplete | None = ...,
+        options: Incomplete | None = ...,
+    ) -> None: ...
+
+class Privileges(dict):
+    def __init__(
+        self,
+        credentialspec_file: Incomplete | None = ...,
+        credentialspec_registry: Incomplete | None = ...,
+        selinux_disable: Incomplete | None = ...,
+        selinux_user: Incomplete | None = ...,
+        selinux_role: Incomplete | None = ...,
+        selinux_type: Incomplete | None = ...,
+        selinux_level: Incomplete | None = ...,
+    ) -> None: ...
+
+class NetworkAttachmentConfig(dict):
+    def __init__(
+        self, target, aliases: Incomplete | None = ..., options: Incomplete | None = ...
     ) -> None: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/types/networks.pyi` & `docker_stubs-0.1.1a0/docker-stubs/types/networks.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/types/services.pyi` & `docker_stubs-0.1.1a0/docker-stubs/types/containers.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,198 +1,207 @@
+from typing import Literal, overload
 from .. import errors as errors
-from ..constants import IS_WINDOWS_PLATFORM as IS_WINDOWS_PLATFORM
-from ..utils import (
-    check_resource as check_resource,
-    convert_service_networks as convert_service_networks,
+from ..utils.utils import (
+    convert_port_bindings as convert_port_bindings,
+    convert_tmpfs_mounts as convert_tmpfs_mounts,
+    convert_volume_binds as convert_volume_binds,
     format_environment as format_environment,
     format_extra_hosts as format_extra_hosts,
+    normalize_links as normalize_links,
     parse_bytes as parse_bytes,
+    parse_devices as parse_devices,
     split_command as split_command,
+    version_gte as version_gte,
+    version_lt as version_lt,
 )
+from .base import DictType as DictType
+from .healthcheck import Healthcheck as Healthcheck
 from _typeshed import Incomplete
 
-class TaskTemplate(dict):
+class LogConfigTypesEnum:
+    JSON: Incomplete
+    SYSLOG: Incomplete
+    JOURNALD: Incomplete
+    GELF: Incomplete
+    FLUENTD: Incomplete
+    NONE: Incomplete
+
+LogConfigKey = Literal["Type", "Config"]
+LogConfigDict = dict[Incomplete, Incomplete]
+
+class LogConfig(DictType[LogConfigKey, str | LogConfigDict]):
+    types = LogConfigTypesEnum
     def __init__(
         self,
-        container_spec,
-        resources: Incomplete | None = ...,
-        restart_policy: Incomplete | None = ...,
-        placement: Incomplete | None = ...,
-        log_driver: Incomplete | None = ...,
-        networks: Incomplete | None = ...,
-        force_update: Incomplete | None = ...,
+        *,
+        type: str | None = ...,
+        Type: str | None = ...,
+        config: LogConfigDict | None = ...,
+        Config: LogConfigDict | None = ...
     ) -> None: ...
     @property
-    def container_spec(self): ...
+    def type(self) -> str: ...
+    @property
+    def config(self) -> dict[Incomplete, Incomplete]: ...
+    @overload
+    def set_config_value(self, key: Literal["Type"], value: str) -> None: ...
+    @overload
+    def set_config_value(
+        self, key: Literal["Config"], value: LogConfigDict
+    ) -> None: ...
+    def set_config_value(
+        self, key: LogConfigKey, value: str | LogConfigDict
+    ) -> None: ...
+    def unset_config(self, key: str) -> None: ...
+
+UlimitKey = Literal["Name", "Soft", "Hard"]
+
+class Ulimit(DictType[UlimitKey, str | int]):
+    def __init__(
+        self,
+        *,
+        name: str | None = ...,
+        Name: str | None = ...,
+        soft: int | None = ...,
+        Soft: int | None = ...,
+        hard: int | None = ...,
+        Hard: int | None = ...
+    ) -> None: ...
     @property
-    def resources(self): ...
+    def name(self) -> str: ...
     @property
-    def restart_policy(self): ...
+    def soft(self) -> int: ...
     @property
-    def placement(self): ...
+    def hard(self) -> int: ...
 
-class ContainerSpec(dict):
-    def __init__(
-        self,
-        image,
-        command: Incomplete | None = ...,
-        args: Incomplete | None = ...,
-        hostname: Incomplete | None = ...,
-        env: Incomplete | None = ...,
-        workdir: Incomplete | None = ...,
-        user: Incomplete | None = ...,
-        labels: Incomplete | None = ...,
-        mounts: Incomplete | None = ...,
-        stop_grace_period: Incomplete | None = ...,
-        secrets: Incomplete | None = ...,
-        tty: Incomplete | None = ...,
-        groups: Incomplete | None = ...,
-        open_stdin: Incomplete | None = ...,
-        read_only: Incomplete | None = ...,
-        stop_signal: Incomplete | None = ...,
-        healthcheck: Incomplete | None = ...,
-        hosts: Incomplete | None = ...,
-        dns_config: Incomplete | None = ...,
-        configs: Incomplete | None = ...,
-        privileges: Incomplete | None = ...,
-        isolation: Incomplete | None = ...,
-        init: Incomplete | None = ...,
-        cap_add: Incomplete | None = ...,
-        cap_drop: Incomplete | None = ...,
-        sysctls: Incomplete | None = ...,
-    ) -> None: ...
+DeviceRequestKey = Literal["Driver", "Count", "DeviceIDs", "Capabilities", "Options"]
 
-class Mount(dict):
-    def __init__(
-        self,
-        target,
-        source,
-        type: str = ...,
-        read_only: bool = ...,
-        consistency: Incomplete | None = ...,
-        propagation: Incomplete | None = ...,
-        no_copy: bool = ...,
-        labels: Incomplete | None = ...,
-        driver_config: Incomplete | None = ...,
-        tmpfs_size: Incomplete | None = ...,
-        tmpfs_mode: Incomplete | None = ...,
+class DeviceRequest(
+    DictType[DeviceRequestKey, str | int | list[str] | dict[Incomplete, Incomplete]]
+):
+    def __init__(
+        self,
+        *,
+        driver: str | None = ...,
+        Driver: str | None = ...,
+        count: int | None = ...,
+        Count: int | None = ...,
+        device_ids: list[str] | None | None = ...,
+        DeviceIDs: list[str] | None = ...,
+        capabilities: list[str] | None = ...,
+        Capabilities: list[str] | None = ...,
+        options: dict[Incomplete, Incomplete] | None = ...,
+        Options: dict[Incomplete, Incomplete] | None = ...
     ) -> None: ...
-    @classmethod
-    def parse_mount_string(cls, string): ...
+    @property
+    def driver(self) -> str | None: ...
+    @property
+    def count(self) -> int | None: ...
+    @property
+    def device_ids(self) -> list[str]: ...
+    @property
+    def capabilities(self) -> list[str]: ...
+    @property
+    def options(self) -> dict[Incomplete, Incomplete]: ...
 
-class Resources(dict):
+class HostConfig(dict[Incomplete, Incomplete]):
     def __init__(
         self,
-        cpu_limit: Incomplete | None = ...,
+        version,
+        binds: Incomplete | None = ...,
+        port_bindings: Incomplete | None = ...,
+        lxc_conf: Incomplete | None = ...,
+        publish_all_ports: bool = ...,
+        links: Incomplete | None = ...,
+        privileged: bool = ...,
+        dns: Incomplete | None = ...,
+        dns_search: Incomplete | None = ...,
+        volumes_from: Incomplete | None = ...,
+        network_mode: Incomplete | None = ...,
+        restart_policy: Incomplete | None = ...,
+        cap_add: Incomplete | None = ...,
+        cap_drop: Incomplete | None = ...,
+        devices: Incomplete | None = ...,
+        extra_hosts: Incomplete | None = ...,
+        read_only: Incomplete | None = ...,
+        pid_mode: Incomplete | None = ...,
+        ipc_mode: Incomplete | None = ...,
+        security_opt: Incomplete | None = ...,
+        ulimits: Incomplete | None = ...,
+        log_config: Incomplete | None = ...,
         mem_limit: Incomplete | None = ...,
-        cpu_reservation: Incomplete | None = ...,
+        memswap_limit: Incomplete | None = ...,
         mem_reservation: Incomplete | None = ...,
-        generic_resources: Incomplete | None = ...,
-    ) -> None: ...
-
-class UpdateConfig(dict):
-    def __init__(
-        self,
-        parallelism: int = ...,
-        delay: Incomplete | None = ...,
-        failure_action: str = ...,
-        monitor: Incomplete | None = ...,
-        max_failure_ratio: Incomplete | None = ...,
-        order: Incomplete | None = ...,
-    ) -> None: ...
-
-class RollbackConfig(UpdateConfig): ...
-
-class RestartConditionTypesEnum:
-    NONE: Incomplete
-    ON_FAILURE: Incomplete
-    ANY: Incomplete
-
-class RestartPolicy(dict):
-    condition_types = RestartConditionTypesEnum
-    def __init__(
-        self,
-        condition=...,
-        delay: int = ...,
-        max_attempts: int = ...,
-        window: int = ...,
-    ) -> None: ...
-
-class DriverConfig(dict):
-    def __init__(self, name, options: Incomplete | None = ...) -> None: ...
-
-class EndpointSpec(dict):
-    def __init__(
-        self, mode: Incomplete | None = ..., ports: Incomplete | None = ...
-    ) -> None: ...
-
-def convert_service_ports(ports): ...
-
-class ServiceMode(dict):
-    mode: Incomplete
-    def __init__(
-        self,
-        mode,
-        replicas: Incomplete | None = ...,
-        concurrency: Incomplete | None = ...,
-    ) -> None: ...
-    @property
-    def replicas(self): ...
-
-class SecretReference(dict):
-    def __init__(
-        self,
-        secret_id,
-        secret_name,
-        filename: Incomplete | None = ...,
-        uid: Incomplete | None = ...,
-        gid: Incomplete | None = ...,
-        mode: int = ...,
-    ) -> None: ...
-
-class ConfigReference(dict):
-    def __init__(
-        self,
-        config_id,
-        config_name,
-        filename: Incomplete | None = ...,
-        uid: Incomplete | None = ...,
-        gid: Incomplete | None = ...,
-        mode: int = ...,
-    ) -> None: ...
-
-class Placement(dict):
-    def __init__(
-        self,
-        constraints: Incomplete | None = ...,
-        preferences: Incomplete | None = ...,
-        platforms: Incomplete | None = ...,
-        maxreplicas: Incomplete | None = ...,
+        kernel_memory: Incomplete | None = ...,
+        mem_swappiness: Incomplete | None = ...,
+        cgroup_parent: Incomplete | None = ...,
+        group_add: Incomplete | None = ...,
+        cpu_quota: Incomplete | None = ...,
+        cpu_period: Incomplete | None = ...,
+        blkio_weight: Incomplete | None = ...,
+        blkio_weight_device: Incomplete | None = ...,
+        device_read_bps: Incomplete | None = ...,
+        device_write_bps: Incomplete | None = ...,
+        device_read_iops: Incomplete | None = ...,
+        device_write_iops: Incomplete | None = ...,
+        oom_kill_disable: bool = ...,
+        shm_size: Incomplete | None = ...,
+        sysctls: Incomplete | None = ...,
+        tmpfs: Incomplete | None = ...,
+        oom_score_adj: Incomplete | None = ...,
+        dns_opt: Incomplete | None = ...,
+        cpu_shares: Incomplete | None = ...,
+        cpuset_cpus: Incomplete | None = ...,
+        userns_mode: Incomplete | None = ...,
+        uts_mode: Incomplete | None = ...,
+        pids_limit: Incomplete | None = ...,
+        isolation: Incomplete | None = ...,
+        auto_remove: bool = ...,
+        storage_opt: Incomplete | None = ...,
+        init: Incomplete | None = ...,
+        init_path: Incomplete | None = ...,
+        volume_driver: Incomplete | None = ...,
+        cpu_count: Incomplete | None = ...,
+        cpu_percent: Incomplete | None = ...,
+        nano_cpus: Incomplete | None = ...,
+        cpuset_mems: Incomplete | None = ...,
+        runtime: Incomplete | None = ...,
+        mounts: Incomplete | None = ...,
+        cpu_rt_period: Incomplete | None = ...,
+        cpu_rt_runtime: Incomplete | None = ...,
+        device_cgroup_rules: Incomplete | None = ...,
+        device_requests: Incomplete | None = ...,
+        cgroupns: Incomplete | None = ...,
     ) -> None: ...
 
-class PlacementPreference(dict):
-    def __init__(self, strategy, descriptor) -> None: ...
+def host_config_type_error(param, param_value, expected): ...
+def host_config_version_error(param, version, less_than: bool = ...): ...
+def host_config_value_error(param, param_value): ...
+def host_config_incompatible_error(param, param_value, incompatible_param): ...
 
-class DNSConfig(dict):
+class ContainerConfig(dict[Incomplete, Incomplete]):
     def __init__(
         self,
-        nameservers: Incomplete | None = ...,
-        search: Incomplete | None = ...,
-        options: Incomplete | None = ...,
-    ) -> None: ...
-
-class Privileges(dict):
-    def __init__(
-        self,
-        credentialspec_file: Incomplete | None = ...,
-        credentialspec_registry: Incomplete | None = ...,
-        selinux_disable: Incomplete | None = ...,
-        selinux_user: Incomplete | None = ...,
-        selinux_role: Incomplete | None = ...,
-        selinux_type: Incomplete | None = ...,
-        selinux_level: Incomplete | None = ...,
-    ) -> None: ...
-
-class NetworkAttachmentConfig(dict):
-    def __init__(
-        self, target, aliases: Incomplete | None = ..., options: Incomplete | None = ...
+        version,
+        image,
+        command,
+        hostname: Incomplete | None = ...,
+        user: Incomplete | None = ...,
+        detach: bool = ...,
+        stdin_open: bool = ...,
+        tty: bool = ...,
+        ports: Incomplete | None = ...,
+        environment: Incomplete | None = ...,
+        volumes: Incomplete | None = ...,
+        network_disabled: bool = ...,
+        entrypoint: Incomplete | None = ...,
+        working_dir: Incomplete | None = ...,
+        domainname: Incomplete | None = ...,
+        host_config: Incomplete | None = ...,
+        mac_address: Incomplete | None = ...,
+        labels: Incomplete | None = ...,
+        stop_signal: Incomplete | None = ...,
+        networking_config: Incomplete | None = ...,
+        healthcheck: Incomplete | None = ...,
+        stop_timeout: Incomplete | None = ...,
+        runtime: Incomplete | None = ...,
     ) -> None: ...
```

### Comparing `docker_stubs-0.1.0/docker-stubs/types/swarm.pyi` & `docker_stubs-0.1.1a0/docker-stubs/types/swarm.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/utils/__init__.pyi` & `docker_stubs-0.1.1a0/docker-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/utils/build.pyi` & `docker_stubs-0.1.1a0/docker-stubs/utils/build.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/utils/socket.pyi` & `docker_stubs-0.1.1a0/docker-stubs/utils/socket.pyi`

 * *Files identical despite different names*

### Comparing `docker_stubs-0.1.0/docker-stubs/utils/utils.pyi` & `docker_stubs-0.1.1a0/docker-stubs/utils/utils.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -5,27 +5,26 @@
     DEFAULT_NPIPE as DEFAULT_NPIPE,
     DEFAULT_UNIX_SOCKET as DEFAULT_UNIX_SOCKET,
 )
 from ..tls import TLSConfig as TLSConfig
 from _typeshed import Incomplete
 from typing import NamedTuple
 
-from ..types.io import JsonString
-
+from ..types._io import JsonString
 
 class URLComponents(NamedTuple):
     scheme: Incomplete
     netloc: Incomplete
     url: Incomplete
     params: Incomplete
     query: Incomplete
     fragment: Incomplete
 
-def create_ipam_pool(*args, **kwargs) -> None: ...
-def create_ipam_config(*args, **kwargs) -> None: ...
+def create_ipam_pool(*args: Incomplete, **kwargs: Incomplete) -> None: ...
+def create_ipam_config(*args: Incomplete, **kwargs: Incomplete) -> None: ...
 def decode_json_header(header): ...
 def compare_version(v1, v2): ...
 def version_lt(v1, v2): ...
 def version_gte(v1, v2): ...
 def convert_port_bindings(port_bindings): ...
 def convert_volume_binds(binds): ...
 def convert_tmpfs_mounts(tmpfs): ...
```

