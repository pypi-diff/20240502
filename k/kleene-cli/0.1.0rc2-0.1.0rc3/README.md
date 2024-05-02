# Comparing `tmp/kleene_cli-0.1.0rc2.tar.gz` & `tmp/kleene_cli-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kleene_cli-0.1.0rc2.tar", max compression
+gzip compressed data, was "kleene_cli-0.1.0rc3.tar", max compression
```

## Comparing `kleene_cli-0.1.0rc2.tar` & `kleene_cli-0.1.0rc3.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0     1320 2021-12-21 07:59:05.958536 kleene_cli-0.1.0rc2/LICENSE
--rw-r--r--   0        0        0       13 2024-03-14 16:30:31.980020 kleene_cli-0.1.0rc2/README.md
--rw-r--r--   0        0        0      156 2024-04-15 22:58:40.109975 kleene_cli-0.1.0rc2/klee/client/__init__.py
--rw-r--r--   0        0        0      271 2024-04-15 23:16:20.659132 kleene_cli-0.1.0rc2/klee/client/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    10187 2024-04-15 23:16:20.711132 kleene_cli-0.1.0rc2/klee/client/__pycache__/client.cpython-39.pyc
--rw-r--r--   0        0        0      818 2024-04-15 23:16:21.327138 kleene_cli-0.1.0rc2/klee/client/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     1688 2024-04-15 23:16:21.751141 kleene_cli-0.1.0rc2/klee/client/__pycache__/types.cpython-39.pyc
--rw-r--r--   0        0        0       47 2024-04-15 22:58:32.137900 kleene_cli-0.1.0rc2/klee/client/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-15 23:16:21.179136 kleene_cli-0.1.0rc2/klee/client/api/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2024-04-15 22:58:32.209900 kleene_cli-0.1.0rc2/klee/client/api/default/__init__.py
--rw-r--r--   0        0        0      140 2024-04-15 23:16:21.251137 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3758 2024-04-15 23:16:21.295138 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_create.cpython-39.pyc
--rw-r--r--   0        0        0     3300 2024-04-15 23:16:24.311164 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_inspect.cpython-39.pyc
--rw-r--r--   0        0        0     3775 2024-04-15 23:16:24.063161 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_list.cpython-39.pyc
--rw-r--r--   0        0        0     2994 2024-04-15 23:16:24.175162 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_prune.cpython-39.pyc
--rw-r--r--   0        0        0     3290 2024-04-15 23:16:24.135162 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_remove.cpython-39.pyc
--rw-r--r--   0        0        0     3361 2024-04-15 23:16:24.207163 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_stop.cpython-39.pyc
--rw-r--r--   0        0        0     4238 2024-04-15 23:16:24.347164 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_update.cpython-39.pyc
--rw-r--r--   0        0        0     3743 2024-04-15 23:16:24.271163 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/exec_create.cpython-39.pyc
--rw-r--r--   0        0        0     3179 2024-04-15 23:16:25.219171 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_inspect.cpython-39.pyc
--rw-r--r--   0        0        0     3110 2024-04-15 23:16:25.051170 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_list.cpython-39.pyc
--rw-r--r--   0        0        0     3179 2024-04-15 23:16:25.263172 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_prune.cpython-39.pyc
--rw-r--r--   0        0        0     3402 2024-04-15 23:16:25.095170 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_remove.cpython-39.pyc
--rw-r--r--   0        0        0     3574 2024-04-15 23:16:25.139171 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_tag.cpython-39.pyc
--rw-r--r--   0        0        0     3507 2024-04-15 23:16:24.423164 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_connect.cpython-39.pyc
--rw-r--r--   0        0        0     3347 2024-04-15 23:16:24.495165 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_create.cpython-39.pyc
--rw-r--r--   0        0        0     3512 2024-04-15 23:16:24.579166 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_disconnect.cpython-39.pyc
--rw-r--r--   0        0        0     3270 2024-04-15 23:16:24.655166 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_inspect.cpython-39.pyc
--rw-r--r--   0        0        0     3383 2024-04-15 23:16:24.619166 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_list.cpython-39.pyc
--rw-r--r--   0        0        0     3038 2024-04-15 23:16:24.719167 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_prune.cpython-39.pyc
--rw-r--r--   0        0        0     3302 2024-04-15 23:16:24.679167 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_remove.cpython-39.pyc
--rw-r--r--   0        0        0     3283 2024-04-15 23:16:25.307172 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_create.cpython-39.pyc
--rw-r--r--   0        0        0     3268 2024-04-15 23:16:25.387173 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_inspect.cpython-39.pyc
--rw-r--r--   0        0        0     2884 2024-04-15 23:16:25.347173 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_list.cpython-39.pyc
--rw-r--r--   0        0        0     3054 2024-04-15 23:16:25.515174 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_prune.cpython-39.pyc
--rw-r--r--   0        0        0     3344 2024-04-15 23:16:25.419173 kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_remove.cpython-39.pyc
--rw-r--r--   0        0        0     5464 2024-04-15 22:58:40.509979 kleene_cli-0.1.0rc2/klee/client/api/default/container_create.py
--rw-r--r--   0        0        0     4628 2024-04-15 22:58:40.509979 kleene_cli-0.1.0rc2/klee/client/api/default/container_inspect.py
--rw-r--r--   0        0        0     5075 2024-04-15 22:58:40.541979 kleene_cli-0.1.0rc2/klee/client/api/default/container_list.py
--rw-r--r--   0        0        0     3782 2024-04-15 22:58:40.513979 kleene_cli-0.1.0rc2/klee/client/api/default/container_prune.py
--rw-r--r--   0        0        0     4610 2024-04-15 22:58:40.913982 kleene_cli-0.1.0rc2/klee/client/api/default/container_remove.py
--rw-r--r--   0        0        0     4728 2024-04-15 22:58:40.905982 kleene_cli-0.1.0rc2/klee/client/api/default/container_stop.py
--rw-r--r--   0        0        0     6540 2024-04-15 22:58:40.953983 kleene_cli-0.1.0rc2/klee/client/api/default/container_update.py
--rw-r--r--   0        0        0     5435 2024-04-15 22:58:40.933983 kleene_cli-0.1.0rc2/klee/client/api/default/exec_create.py
--rw-r--r--   0        0        0    15192 2024-04-15 22:58:41.317986 kleene_cli-0.1.0rc2/klee/client/api/default/exec_start_web_socket.py
--rw-r--r--   0        0        0     5424 2024-04-15 22:58:41.453987 kleene_cli-0.1.0rc2/klee/client/api/default/exec_stop.py
--rw-r--r--   0        0        0    15597 2024-04-15 22:58:41.325986 kleene_cli-0.1.0rc2/klee/client/api/default/image_build.py
--rw-r--r--   0        0        0    14812 2024-04-15 22:58:41.369987 kleene_cli-0.1.0rc2/klee/client/api/default/image_create.py
--rw-r--r--   0        0        0     4283 2024-04-15 22:58:41.709990 kleene_cli-0.1.0rc2/klee/client/api/default/image_inspect.py
--rw-r--r--   0        0        0     4080 2024-04-15 22:58:41.737990 kleene_cli-0.1.0rc2/klee/client/api/default/image_list.py
--rw-r--r--   0        0        0     3920 2024-04-15 22:58:41.789991 kleene_cli-0.1.0rc2/klee/client/api/default/image_prune.py
--rw-r--r--   0        0        0     4760 2024-04-15 22:58:41.849991 kleene_cli-0.1.0rc2/klee/client/api/default/image_remove.py
--rw-r--r--   0        0        0     4866 2024-04-15 22:58:42.157994 kleene_cli-0.1.0rc2/klee/client/api/default/image_tag.py
--rw-r--r--   0        0        0     4953 2024-04-15 22:58:42.145994 kleene_cli-0.1.0rc2/klee/client/api/default/network_connect.py
--rw-r--r--   0        0        0     4643 2024-04-15 22:58:42.189994 kleene_cli-0.1.0rc2/klee/client/api/default/network_create.py
--rw-r--r--   0        0        0     5085 2024-04-15 22:58:42.273995 kleene_cli-0.1.0rc2/klee/client/api/default/network_disconnect.py
--rw-r--r--   0        0        0     4527 2024-04-15 22:58:42.545998 kleene_cli-0.1.0rc2/klee/client/api/default/network_inspect.py
--rw-r--r--   0        0        0     4601 2024-04-15 22:58:42.565998 kleene_cli-0.1.0rc2/klee/client/api/default/network_list.py
--rw-r--r--   0        0        0     3876 2024-04-15 22:58:42.569998 kleene_cli-0.1.0rc2/klee/client/api/default/network_prune.py
--rw-r--r--   0        0        0     4578 2024-04-15 22:58:42.677999 kleene_cli-0.1.0rc2/klee/client/api/default/network_remove.py
--rw-r--r--   0        0        0     4490 2024-04-15 22:58:42.946002 kleene_cli-0.1.0rc2/klee/client/api/default/volume_create.py
--rw-r--r--   0        0        0     4533 2024-04-15 22:58:42.966002 kleene_cli-0.1.0rc2/klee/client/api/default/volume_inspect.py
--rw-r--r--   0        0        0     3630 2024-04-15 22:58:42.906001 kleene_cli-0.1.0rc2/klee/client/api/default/volume_list.py
--rw-r--r--   0        0        0     3911 2024-04-15 22:58:43.026002 kleene_cli-0.1.0rc2/klee/client/api/default/volume_prune.py
--rw-r--r--   0        0        0     4677 2024-04-15 22:58:43.354005 kleene_cli-0.1.0rc2/klee/client/api/default/volume_remove.py
--rw-r--r--   0        0        0    12209 2024-04-15 22:58:44.142013 kleene_cli-0.1.0rc2/klee/client/client.py
--rw-r--r--   0        0        0      470 2024-04-15 22:58:43.006002 kleene_cli-0.1.0rc2/klee/client/errors.py
--rw-r--r--   0        0        0     2739 2024-04-15 22:58:32.081899 kleene_cli-0.1.0rc2/klee/client/models/__init__.py
--rw-r--r--   0        0        0     2560 2024-04-15 23:16:21.375138 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6761 2024-04-15 23:16:21.459139 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container.cpython-39.pyc
--rw-r--r--   0        0        0     7915 2024-04-15 23:16:21.827142 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_config.cpython-39.pyc
--rw-r--r--   0        0        0      629 2024-04-15 23:16:21.867142 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_config_network_driver.cpython-39.pyc
--rw-r--r--   0        0        0      591 2024-04-15 23:16:21.915143 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_config_restart_policy.cpython-39.pyc
--rw-r--r--   0        0        0     3588 2024-04-15 23:16:22.035144 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_inspect.cpython-39.pyc
--rw-r--r--   0        0        0      610 2024-04-15 23:16:21.499139 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_network_driver.cpython-39.pyc
--rw-r--r--   0        0        0      572 2024-04-15 23:16:21.591140 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_restart_policy.cpython-39.pyc
--rw-r--r--   0        0        0     7465 2024-04-15 23:16:22.115145 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_summary.cpython-39.pyc
--rw-r--r--   0        0        0     3347 2024-04-15 23:16:22.227146 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/end_point.cpython-39.pyc
--rw-r--r--   0        0        0     3228 2024-04-15 23:16:22.303146 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/end_point_config.cpython-39.pyc
--rw-r--r--   0        0        0     2230 2024-04-15 23:16:22.351147 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/error_response.cpython-39.pyc
--rw-r--r--   0        0        0     3921 2024-04-15 23:16:22.399147 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/exec_config.cpython-39.pyc
--rw-r--r--   0        0        0     2524 2024-04-15 23:16:22.439147 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/exec_start_config.cpython-39.pyc
--rw-r--r--   0        0        0     2148 2024-04-15 23:16:22.471148 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/id_response.cpython-39.pyc
--rw-r--r--   0        0        0     4466 2024-04-15 23:16:22.547148 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image.cpython-39.pyc
--rw-r--r--   0        0        0     4906 2024-04-15 23:16:22.639149 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image_build_config.cpython-39.pyc
--rw-r--r--   0        0        0     2326 2024-04-15 23:16:22.735150 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image_build_config_buildargs.cpython-39.pyc
--rw-r--r--   0        0        0     5220 2024-04-15 23:16:22.779150 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image_create_config.cpython-39.pyc
--rw-r--r--   0        0        0      636 2024-04-15 23:16:22.835151 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image_create_config_method.cpython-39.pyc
--rw-r--r--   0        0        0     3667 2024-04-15 23:16:22.911152 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/mount_point.cpython-39.pyc
--rw-r--r--   0        0        0     3568 2024-04-15 23:16:23.075153 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/mount_point_config.cpython-39.pyc
--rw-r--r--   0        0        0      567 2024-04-15 23:16:23.163154 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/mount_point_config_type.cpython-39.pyc
--rw-r--r--   0        0        0      548 2024-04-15 23:16:22.967152 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/mount_point_type.cpython-39.pyc
--rw-r--r--   0        0        0     4992 2024-04-15 23:16:23.219154 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network.cpython-39.pyc
--rw-r--r--   0        0        0     5373 2024-04-15 23:16:23.359155 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network_config.cpython-39.pyc
--rw-r--r--   0        0        0      583 2024-04-15 23:16:23.427156 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network_config_type.cpython-39.pyc
--rw-r--r--   0        0        0     3020 2024-04-15 23:16:23.503157 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network_inspect.cpython-39.pyc
--rw-r--r--   0        0        0      564 2024-04-15 23:16:23.291155 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network_type.cpython-39.pyc
--rw-r--r--   0        0        0     3786 2024-04-15 23:16:23.603157 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/published_port.cpython-39.pyc
--rw-r--r--   0        0        0     3859 2024-04-15 23:16:23.683158 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/published_port_config.cpython-39.pyc
--rw-r--r--   0        0        0      576 2024-04-15 23:16:23.727159 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/published_port_config_protocol.cpython-39.pyc
--rw-r--r--   0        0        0      557 2024-04-15 23:16:23.639158 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/published_port_protocol.cpython-39.pyc
--rw-r--r--   0        0        0     2769 2024-04-15 23:16:23.759159 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/volume.cpython-39.pyc
--rw-r--r--   0        0        0     2122 2024-04-15 23:16:23.795159 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/volume_config.cpython-39.pyc
--rw-r--r--   0        0        0     3022 2024-04-15 23:16:23.875160 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/volume_inspect.cpython-39.pyc
--rw-r--r--   0        0        0     2830 2024-04-15 23:16:23.919160 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/web_socket_message.cpython-39.pyc
--rw-r--r--   0        0        0      603 2024-04-15 23:16:23.963161 kleene_cli-0.1.0rc2/klee/client/models/__pycache__/web_socket_message_msg_type.cpython-39.pyc
--rw-r--r--   0        0        0     8714 2024-04-15 22:58:44.026012 kleene_cli-0.1.0rc2/klee/client/models/container.py
--rw-r--r--   0        0        0    10371 2024-04-15 22:58:44.110013 kleene_cli-0.1.0rc2/klee/client/models/container_config.py
--rw-r--r--   0        0        0      215 2024-04-15 22:58:37.297948 kleene_cli-0.1.0rc2/klee/client/models/container_config_network_driver.py
--rw-r--r--   0        0        0      177 2024-04-15 22:58:38.693961 kleene_cli-0.1.0rc2/klee/client/models/container_config_restart_policy.py
--rw-r--r--   0        0        0     4462 2024-04-15 22:58:43.930011 kleene_cli-0.1.0rc2/klee/client/models/container_inspect.py
--rw-r--r--   0        0        0      209 2024-04-15 22:58:37.505950 kleene_cli-0.1.0rc2/klee/client/models/container_network_driver.py
--rw-r--r--   0        0        0      171 2024-04-15 22:58:38.829963 kleene_cli-0.1.0rc2/klee/client/models/container_restart_policy.py
--rw-r--r--   0        0        0     9707 2024-04-15 22:58:44.930020 kleene_cli-0.1.0rc2/klee/client/models/container_summary.py
--rw-r--r--   0        0        0     3290 2024-04-15 22:58:44.398015 kleene_cli-0.1.0rc2/klee/client/models/end_point.py
--rw-r--r--   0        0        0     2885 2024-04-15 22:58:44.390015 kleene_cli-0.1.0rc2/klee/client/models/end_point_config.py
--rw-r--r--   0        0        0     1590 2024-04-15 22:58:44.338015 kleene_cli-0.1.0rc2/klee/client/models/error_response.py
--rw-r--r--   0        0        0     3702 2024-04-15 22:58:44.734018 kleene_cli-0.1.0rc2/klee/client/models/exec_config.py
--rw-r--r--   0        0        0     2084 2024-04-15 22:58:44.622017 kleene_cli-0.1.0rc2/klee/client/models/exec_start_config.py
--rw-r--r--   0        0        0     1483 2024-04-15 22:58:44.594017 kleene_cli-0.1.0rc2/klee/client/models/id_response.py
--rw-r--r--   0        0        0     4937 2024-04-15 22:58:45.178023 kleene_cli-0.1.0rc2/klee/client/models/image.py
--rw-r--r--   0        0        0     5646 2024-04-15 22:58:45.186023 kleene_cli-0.1.0rc2/klee/client/models/image_build_config.py
--rw-r--r--   0        0        0     1525 2024-04-15 22:58:44.906020 kleene_cli-0.1.0rc2/klee/client/models/image_build_config_buildargs.py
--rw-r--r--   0        0        0     5294 2024-04-15 22:58:45.378024 kleene_cli-0.1.0rc2/klee/client/models/image_create_config.py
--rw-r--r--   0        0        0      232 2024-04-15 22:58:39.209966 kleene_cli-0.1.0rc2/klee/client/models/image_create_config_method.py
--rw-r--r--   0        0        0     3638 2024-04-15 22:58:45.338024 kleene_cli-0.1.0rc2/klee/client/models/mount_point.py
--rw-r--r--   0        0        0     3376 2024-04-15 22:58:45.530026 kleene_cli-0.1.0rc2/klee/client/models/mount_point_config.py
--rw-r--r--   0        0        0      169 2024-04-15 22:58:37.869954 kleene_cli-0.1.0rc2/klee/client/models/mount_point_config_type.py
--rw-r--r--   0        0        0      163 2024-04-15 22:58:37.229948 kleene_cli-0.1.0rc2/klee/client/models/mount_point_type.py
--rw-r--r--   0        0        0     5383 2024-04-15 22:58:45.850029 kleene_cli-0.1.0rc2/klee/client/models/network.py
--rw-r--r--   0        0        0     5500 2024-04-15 22:58:45.898029 kleene_cli-0.1.0rc2/klee/client/models/network_config.py
--rw-r--r--   0        0        0      192 2024-04-15 22:58:38.513960 kleene_cli-0.1.0rc2/klee/client/models/network_config_type.py
--rw-r--r--   0        0        0     3109 2024-04-15 22:58:45.830029 kleene_cli-0.1.0rc2/klee/client/models/network_inspect.py
--rw-r--r--   0        0        0      186 2024-04-15 22:58:38.625961 kleene_cli-0.1.0rc2/klee/client/models/network_type.py
--rw-r--r--   0        0        0     3687 2024-04-15 22:58:45.922030 kleene_cli-0.1.0rc2/klee/client/models/published_port.py
--rw-r--r--   0        0        0     3729 2024-04-15 22:58:46.162032 kleene_cli-0.1.0rc2/klee/client/models/published_port_config.py
--rw-r--r--   0        0        0      164 2024-04-15 22:58:37.649952 kleene_cli-0.1.0rc2/klee/client/models/published_port_config_protocol.py
--rw-r--r--   0        0        0      158 2024-04-15 22:58:37.773953 kleene_cli-0.1.0rc2/klee/client/models/published_port_protocol.py
--rw-r--r--   0        0        0     2431 2024-04-15 22:58:46.182032 kleene_cli-0.1.0rc2/klee/client/models/volume.py
--rw-r--r--   0        0        0     1463 2024-04-15 22:58:46.106031 kleene_cli-0.1.0rc2/klee/client/models/volume_config.py
--rw-r--r--   0        0        0     2984 2024-04-15 22:58:46.302033 kleene_cli-0.1.0rc2/klee/client/models/volume_inspect.py
--rw-r--r--   0        0        0     2318 2024-04-15 22:58:46.350034 kleene_cli-0.1.0rc2/klee/client/models/web_socket_message.py
--rw-r--r--   0        0        0      198 2024-04-15 22:58:38.437959 kleene_cli-0.1.0rc2/klee/client/models/web_socket_message_msg_type.py
--rw-r--r--   0        0        0      969 2024-04-15 22:58:46.302033 kleene_cli-0.1.0rc2/klee/client/types.py
--rw-r--r--   0        0        0     3679 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc2/klee/config.py
--rw-r--r--   0        0        0     3199 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc2/klee/connection.py
--rw-r--r--   0        0        0    21337 2024-04-22 14:42:55.285287 kleene_cli-0.1.0rc2/klee/container.py
--rw-r--r--   0        0        0     4573 2023-11-01 16:20:47.318593 kleene_cli-0.1.0rc2/klee/custom_client_templates/endpoint_module.py.jinja
--rw-r--r--   0        0        0     5397 2024-04-02 10:04:21.452452 kleene_cli-0.1.0rc2/klee/docs_generator.py
--rw-r--r--   0        0        0    15938 2024-04-23 07:52:47.750640 kleene_cli-0.1.0rc2/klee/image.py
--rw-r--r--   0        0        0      700 2024-04-21 05:50:28.406645 kleene_cli-0.1.0rc2/klee/inspect.py
--rw-r--r--   0        0        0      156 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc2/klee/main.py
--rw-r--r--   0        0        0    50283 2024-04-02 10:04:21.464452 kleene_cli-0.1.0rc2/klee/name_generator.py
--rw-r--r--   0        0        0     8354 2024-04-18 14:11:54.272460 kleene_cli-0.1.0rc2/klee/network.py
--rw-r--r--   0        0        0     3670 2024-04-22 14:42:10.288859 kleene_cli-0.1.0rc2/klee/options.py
--rw-r--r--   0        0        0     9143 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc2/klee/printing.py
--rw-r--r--   0        0        0      688 2024-04-02 10:04:21.452452 kleene_cli-0.1.0rc2/klee/prune.py
--rw-r--r--   0        0        0     4394 2024-04-18 11:43:40.571019 kleene_cli-0.1.0rc2/klee/root.py
--rw-r--r--   0        0        0      433 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc2/klee/shortcuts.py
--rw-r--r--   0        0        0     4942 2024-04-02 10:04:21.452452 kleene_cli-0.1.0rc2/klee/utils.py
--rw-r--r--   0        0        0     3203 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc2/klee/volume.py
--rw-r--r--   0        0        0      936 2024-04-26 07:54:06.006902 kleene_cli-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 kleene_cli-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1320 2021-12-21 07:59:05.958536 kleene_cli-0.1.0rc3/LICENSE
+-rw-r--r--   0        0        0      240 2024-05-02 10:26:15.920787 kleene_cli-0.1.0rc3/README.md
+-rw-r--r--   0        0        0      156 2024-05-01 08:33:10.720631 kleene_cli-0.1.0rc3/klee/client/__init__.py
+-rw-r--r--   0        0        0      271 2024-05-01 08:37:57.007603 kleene_cli-0.1.0rc3/klee/client/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    10187 2024-05-01 08:37:57.035603 kleene_cli-0.1.0rc3/klee/client/__pycache__/client.cpython-39.pyc
+-rw-r--r--   0        0        0      818 2024-05-01 08:37:57.147605 kleene_cli-0.1.0rc3/klee/client/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     1688 2024-05-01 08:37:57.263606 kleene_cli-0.1.0rc3/klee/client/__pycache__/types.cpython-39.pyc
+-rw-r--r--   0        0        0       47 2024-05-01 08:33:04.964571 kleene_cli-0.1.0rc3/klee/client/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-01 08:37:57.079604 kleene_cli-0.1.0rc3/klee/client/api/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2024-05-01 08:33:05.024572 kleene_cli-0.1.0rc3/klee/client/api/default/__init__.py
+-rw-r--r--   0        0        0      140 2024-05-01 08:37:57.103604 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3758 2024-05-01 08:37:59.291627 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_create.cpython-39.pyc
+-rw-r--r--   0        0        0     3300 2024-05-01 08:37:59.463629 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_inspect.cpython-39.pyc
+-rw-r--r--   0        0        0     3775 2024-05-01 08:37:58.191615 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_list.cpython-39.pyc
+-rw-r--r--   0        0        0     2994 2024-05-01 08:37:59.367628 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_prune.cpython-39.pyc
+-rw-r--r--   0        0        0     3290 2024-05-01 08:37:59.347627 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_remove.cpython-39.pyc
+-rw-r--r--   0        0        0     3361 2024-05-01 08:37:59.391628 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_stop.cpython-39.pyc
+-rw-r--r--   0        0        0     4238 2024-05-01 08:37:59.483629 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_update.cpython-39.pyc
+-rw-r--r--   0        0        0     3743 2024-05-01 08:37:59.439628 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/exec_create.cpython-39.pyc
+-rw-r--r--   0        0        0     3179 2024-05-01 08:37:58.347617 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_inspect.cpython-39.pyc
+-rw-r--r--   0        0        0     3110 2024-05-01 08:37:57.127604 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_list.cpython-39.pyc
+-rw-r--r--   0        0        0     3179 2024-05-01 08:37:58.367617 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_prune.cpython-39.pyc
+-rw-r--r--   0        0        0     3402 2024-05-01 08:37:58.287616 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_remove.cpython-39.pyc
+-rw-r--r--   0        0        0     3574 2024-05-01 08:37:58.327617 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_tag.cpython-39.pyc
+-rw-r--r--   0        0        0     3507 2024-05-01 08:37:59.539629 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_connect.cpython-39.pyc
+-rw-r--r--   0        0        0     3347 2024-05-01 08:37:59.507629 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_create.cpython-39.pyc
+-rw-r--r--   0        0        0     3512 2024-05-01 08:37:59.563630 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_disconnect.cpython-39.pyc
+-rw-r--r--   0        0        0     3270 2024-05-01 08:37:59.623630 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_inspect.cpython-39.pyc
+-rw-r--r--   0        0        0     3383 2024-05-01 08:37:59.595630 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_list.cpython-39.pyc
+-rw-r--r--   0        0        0     3038 2024-05-01 08:37:59.667631 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_prune.cpython-39.pyc
+-rw-r--r--   0        0        0     3302 2024-05-01 08:37:59.647631 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_remove.cpython-39.pyc
+-rw-r--r--   0        0        0     3283 2024-05-01 08:37:59.695631 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_create.cpython-39.pyc
+-rw-r--r--   0        0        0     3268 2024-05-01 08:37:59.783632 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_inspect.cpython-39.pyc
+-rw-r--r--   0        0        0     2884 2024-05-01 08:37:59.739632 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_list.cpython-39.pyc
+-rw-r--r--   0        0        0     3054 2024-05-01 08:37:59.827632 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_prune.cpython-39.pyc
+-rw-r--r--   0        0        0     3344 2024-05-01 08:37:59.803632 kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_remove.cpython-39.pyc
+-rw-r--r--   0        0        0     5464 2024-05-01 08:33:11.120635 kleene_cli-0.1.0rc3/klee/client/api/default/container_create.py
+-rw-r--r--   0        0        0     4628 2024-05-01 08:33:11.112635 kleene_cli-0.1.0rc3/klee/client/api/default/container_inspect.py
+-rw-r--r--   0        0        0     5075 2024-05-01 08:33:11.148635 kleene_cli-0.1.0rc3/klee/client/api/default/container_list.py
+-rw-r--r--   0        0        0     3782 2024-05-01 08:33:11.076635 kleene_cli-0.1.0rc3/klee/client/api/default/container_prune.py
+-rw-r--r--   0        0        0     4610 2024-05-01 08:33:11.508639 kleene_cli-0.1.0rc3/klee/client/api/default/container_remove.py
+-rw-r--r--   0        0        0     4728 2024-05-01 08:33:11.520640 kleene_cli-0.1.0rc3/klee/client/api/default/container_stop.py
+-rw-r--r--   0        0        0     6540 2024-05-01 08:33:11.620640 kleene_cli-0.1.0rc3/klee/client/api/default/container_update.py
+-rw-r--r--   0        0        0     5435 2024-05-01 08:33:11.564640 kleene_cli-0.1.0rc3/klee/client/api/default/exec_create.py
+-rw-r--r--   0        0        0    15192 2024-05-01 08:33:11.908643 kleene_cli-0.1.0rc3/klee/client/api/default/exec_start_web_socket.py
+-rw-r--r--   0        0        0     5424 2024-05-01 08:33:12.060645 kleene_cli-0.1.0rc3/klee/client/api/default/exec_stop.py
+-rw-r--r--   0        0        0    15597 2024-05-01 08:33:11.956644 kleene_cli-0.1.0rc3/klee/client/api/default/image_build.py
+-rw-r--r--   0        0        0    14812 2024-05-01 08:33:12.016645 kleene_cli-0.1.0rc3/klee/client/api/default/image_create.py
+-rw-r--r--   0        0        0     4283 2024-05-01 08:33:12.312648 kleene_cli-0.1.0rc3/klee/client/api/default/image_inspect.py
+-rw-r--r--   0        0        0     4080 2024-05-01 08:33:12.300648 kleene_cli-0.1.0rc3/klee/client/api/default/image_list.py
+-rw-r--r--   0        0        0     3920 2024-05-01 08:33:12.412649 kleene_cli-0.1.0rc3/klee/client/api/default/image_prune.py
+-rw-r--r--   0        0        0     4760 2024-05-01 08:33:12.472649 kleene_cli-0.1.0rc3/klee/client/api/default/image_remove.py
+-rw-r--r--   0        0        0     4866 2024-05-01 08:33:12.784653 kleene_cli-0.1.0rc3/klee/client/api/default/image_tag.py
+-rw-r--r--   0        0        0     4953 2024-05-01 08:33:12.748652 kleene_cli-0.1.0rc3/klee/client/api/default/network_connect.py
+-rw-r--r--   0        0        0     4643 2024-05-01 08:33:12.832653 kleene_cli-0.1.0rc3/klee/client/api/default/network_create.py
+-rw-r--r--   0        0        0     5085 2024-05-01 08:33:12.924654 kleene_cli-0.1.0rc3/klee/client/api/default/network_disconnect.py
+-rw-r--r--   0        0        0     4527 2024-05-01 08:33:13.168656 kleene_cli-0.1.0rc3/klee/client/api/default/network_inspect.py
+-rw-r--r--   0        0        0     4601 2024-05-01 08:33:13.176657 kleene_cli-0.1.0rc3/klee/client/api/default/network_list.py
+-rw-r--r--   0        0        0     3876 2024-05-01 08:33:13.192657 kleene_cli-0.1.0rc3/klee/client/api/default/network_prune.py
+-rw-r--r--   0        0        0     4578 2024-05-01 08:33:13.336658 kleene_cli-0.1.0rc3/klee/client/api/default/network_remove.py
+-rw-r--r--   0        0        0     4490 2024-05-01 08:33:13.572661 kleene_cli-0.1.0rc3/klee/client/api/default/volume_create.py
+-rw-r--r--   0        0        0     4533 2024-05-01 08:33:13.596661 kleene_cli-0.1.0rc3/klee/client/api/default/volume_inspect.py
+-rw-r--r--   0        0        0     3630 2024-05-01 08:33:13.544660 kleene_cli-0.1.0rc3/klee/client/api/default/volume_list.py
+-rw-r--r--   0        0        0     3911 2024-05-01 08:33:13.700662 kleene_cli-0.1.0rc3/klee/client/api/default/volume_prune.py
+-rw-r--r--   0        0        0     4677 2024-05-01 08:33:13.964665 kleene_cli-0.1.0rc3/klee/client/api/default/volume_remove.py
+-rw-r--r--   0        0        0    12209 2024-05-01 08:33:14.724673 kleene_cli-0.1.0rc3/klee/client/client.py
+-rw-r--r--   0        0        0      470 2024-05-01 08:33:13.644662 kleene_cli-0.1.0rc3/klee/client/errors.py
+-rw-r--r--   0        0        0     2739 2024-05-01 08:33:04.920571 kleene_cli-0.1.0rc3/klee/client/models/__init__.py
+-rw-r--r--   0        0        0     2560 2024-05-01 08:37:57.175605 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6761 2024-05-01 08:37:57.199605 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container.cpython-39.pyc
+-rw-r--r--   0        0        0     7915 2024-05-01 08:37:57.295606 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_config.cpython-39.pyc
+-rw-r--r--   0        0        0      629 2024-05-01 08:37:57.315606 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_config_network_driver.cpython-39.pyc
+-rw-r--r--   0        0        0      591 2024-05-01 08:37:57.339607 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_config_restart_policy.cpython-39.pyc
+-rw-r--r--   0        0        0     3588 2024-05-01 08:37:57.363607 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_inspect.cpython-39.pyc
+-rw-r--r--   0        0        0      610 2024-05-01 08:37:57.219605 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_network_driver.cpython-39.pyc
+-rw-r--r--   0        0        0      572 2024-05-01 08:37:57.243605 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_restart_policy.cpython-39.pyc
+-rw-r--r--   0        0        0     7465 2024-05-01 08:37:57.391607 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_summary.cpython-39.pyc
+-rw-r--r--   0        0        0     3347 2024-05-01 08:37:57.419607 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/end_point.cpython-39.pyc
+-rw-r--r--   0        0        0     3228 2024-05-01 08:37:57.443608 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/end_point_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2230 2024-05-01 08:37:57.467608 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/error_response.cpython-39.pyc
+-rw-r--r--   0        0        0     3921 2024-05-01 08:37:57.491608 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/exec_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2524 2024-05-01 08:37:57.515608 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/exec_start_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2148 2024-05-01 08:37:57.551609 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/id_response.cpython-39.pyc
+-rw-r--r--   0        0        0     4466 2024-05-01 08:37:57.575609 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image.cpython-39.pyc
+-rw-r--r--   0        0        0     4906 2024-05-01 08:37:57.603609 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image_build_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2326 2024-05-01 08:37:57.627610 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image_build_config_buildargs.cpython-39.pyc
+-rw-r--r--   0        0        0     4954 2024-05-01 08:37:57.683610 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image_create_config.cpython-39.pyc
+-rw-r--r--   0        0        0      636 2024-05-01 08:37:57.703610 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image_create_config_method.cpython-39.pyc
+-rw-r--r--   0        0        0     3667 2024-05-01 08:37:57.739611 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/mount_point.cpython-39.pyc
+-rw-r--r--   0        0        0     3568 2024-05-01 08:37:57.783611 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/mount_point_config.cpython-39.pyc
+-rw-r--r--   0        0        0      567 2024-05-01 08:37:57.807611 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/mount_point_config_type.cpython-39.pyc
+-rw-r--r--   0        0        0      548 2024-05-01 08:37:57.759611 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/mount_point_type.cpython-39.pyc
+-rw-r--r--   0        0        0     4992 2024-05-01 08:37:57.831612 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0        0        0     5373 2024-05-01 08:37:57.879612 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network_config.cpython-39.pyc
+-rw-r--r--   0        0        0      583 2024-05-01 08:37:57.899612 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network_config_type.cpython-39.pyc
+-rw-r--r--   0        0        0     3020 2024-05-01 08:37:57.923613 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network_inspect.cpython-39.pyc
+-rw-r--r--   0        0        0      564 2024-05-01 08:37:57.851612 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network_type.cpython-39.pyc
+-rw-r--r--   0        0        0     3786 2024-05-01 08:37:57.947613 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/published_port.cpython-39.pyc
+-rw-r--r--   0        0        0     3859 2024-05-01 08:37:57.991613 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/published_port_config.cpython-39.pyc
+-rw-r--r--   0        0        0      576 2024-05-01 08:37:58.039614 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/published_port_config_protocol.cpython-39.pyc
+-rw-r--r--   0        0        0      557 2024-05-01 08:37:57.967613 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/published_port_protocol.cpython-39.pyc
+-rw-r--r--   0        0        0     2769 2024-05-01 08:37:58.079614 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/volume.cpython-39.pyc
+-rw-r--r--   0        0        0     2122 2024-05-01 08:37:58.103614 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/volume_config.cpython-39.pyc
+-rw-r--r--   0        0        0     3022 2024-05-01 08:37:58.123615 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/volume_inspect.cpython-39.pyc
+-rw-r--r--   0        0        0     2830 2024-05-01 08:37:58.147615 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/web_socket_message.cpython-39.pyc
+-rw-r--r--   0        0        0      603 2024-05-01 08:37:58.167615 kleene_cli-0.1.0rc3/klee/client/models/__pycache__/web_socket_message_msg_type.cpython-39.pyc
+-rw-r--r--   0        0        0     8714 2024-05-01 08:33:14.660672 kleene_cli-0.1.0rc3/klee/client/models/container.py
+-rw-r--r--   0        0        0    10371 2024-05-01 08:33:14.716673 kleene_cli-0.1.0rc3/klee/client/models/container_config.py
+-rw-r--r--   0        0        0      215 2024-05-01 08:33:08.800611 kleene_cli-0.1.0rc3/klee/client/models/container_config_network_driver.py
+-rw-r--r--   0        0        0      177 2024-05-01 08:33:09.784621 kleene_cli-0.1.0rc3/klee/client/models/container_config_restart_policy.py
+-rw-r--r--   0        0        0     4462 2024-05-01 08:33:14.508670 kleene_cli-0.1.0rc3/klee/client/models/container_inspect.py
+-rw-r--r--   0        0        0      209 2024-05-01 08:33:08.988613 kleene_cli-0.1.0rc3/klee/client/models/container_network_driver.py
+-rw-r--r--   0        0        0      171 2024-05-01 08:33:09.888622 kleene_cli-0.1.0rc3/klee/client/models/container_restart_policy.py
+-rw-r--r--   0        0        0     9707 2024-05-01 08:33:15.560681 kleene_cli-0.1.0rc3/klee/client/models/container_summary.py
+-rw-r--r--   0        0        0     3290 2024-05-01 08:33:15.052676 kleene_cli-0.1.0rc3/klee/client/models/end_point.py
+-rw-r--r--   0        0        0     2885 2024-05-01 08:33:15.020676 kleene_cli-0.1.0rc3/klee/client/models/end_point_config.py
+-rw-r--r--   0        0        0     1590 2024-05-01 08:33:14.932675 kleene_cli-0.1.0rc3/klee/client/models/error_response.py
+-rw-r--r--   0        0        0     3702 2024-05-01 08:33:15.344679 kleene_cli-0.1.0rc3/klee/client/models/exec_config.py
+-rw-r--r--   0        0        0     2084 2024-05-01 08:33:15.276678 kleene_cli-0.1.0rc3/klee/client/models/exec_start_config.py
+-rw-r--r--   0        0        0     1483 2024-05-01 08:33:15.264678 kleene_cli-0.1.0rc3/klee/client/models/id_response.py
+-rw-r--r--   0        0        0     4937 2024-05-01 08:33:15.904685 kleene_cli-0.1.0rc3/klee/client/models/image.py
+-rw-r--r--   0        0        0     5646 2024-05-01 08:33:15.992686 kleene_cli-0.1.0rc3/klee/client/models/image_build_config.py
+-rw-r--r--   0        0        0     1525 2024-05-01 08:33:15.524681 kleene_cli-0.1.0rc3/klee/client/models/image_build_config_buildargs.py
+-rw-r--r--   0        0        0     4939 2024-05-01 08:33:16.028686 kleene_cli-0.1.0rc3/klee/client/models/image_create_config.py
+-rw-r--r--   0        0        0      232 2024-05-01 08:33:10.068624 kleene_cli-0.1.0rc3/klee/client/models/image_create_config_method.py
+-rw-r--r--   0        0        0     3638 2024-05-01 08:33:16.088687 kleene_cli-0.1.0rc3/klee/client/models/mount_point.py
+-rw-r--r--   0        0        0     3376 2024-05-01 08:33:16.288689 kleene_cli-0.1.0rc3/klee/client/models/mount_point_config.py
+-rw-r--r--   0        0        0      169 2024-05-01 08:33:09.152615 kleene_cli-0.1.0rc3/klee/client/models/mount_point_config_type.py
+-rw-r--r--   0        0        0      163 2024-05-01 08:33:08.748611 kleene_cli-0.1.0rc3/klee/client/models/mount_point_type.py
+-rw-r--r--   0        0        0     5383 2024-05-01 08:33:16.684693 kleene_cli-0.1.0rc3/klee/client/models/network.py
+-rw-r--r--   0        0        0     5500 2024-05-01 08:33:16.600692 kleene_cli-0.1.0rc3/klee/client/models/network_config.py
+-rw-r--r--   0        0        0      192 2024-05-01 08:33:09.616620 kleene_cli-0.1.0rc3/klee/client/models/network_config_type.py
+-rw-r--r--   0        0        0     3109 2024-05-01 08:33:16.528691 kleene_cli-0.1.0rc3/klee/client/models/network_inspect.py
+-rw-r--r--   0        0        0      186 2024-05-01 08:33:09.760621 kleene_cli-0.1.0rc3/klee/client/models/network_type.py
+-rw-r--r--   0        0        0     3687 2024-05-01 08:33:16.688693 kleene_cli-0.1.0rc3/klee/client/models/published_port.py
+-rw-r--r--   0        0        0     3729 2024-05-01 08:33:16.884695 kleene_cli-0.1.0rc3/klee/client/models/published_port_config.py
+-rw-r--r--   0        0        0      164 2024-05-01 08:33:09.080614 kleene_cli-0.1.0rc3/klee/client/models/published_port_config_protocol.py
+-rw-r--r--   0        0        0      158 2024-05-01 08:33:09.100614 kleene_cli-0.1.0rc3/klee/client/models/published_port_protocol.py
+-rw-r--r--   0        0        0     2431 2024-05-01 08:33:16.952696 kleene_cli-0.1.0rc3/klee/client/models/volume.py
+-rw-r--r--   0        0        0     1463 2024-05-01 08:33:16.892695 kleene_cli-0.1.0rc3/klee/client/models/volume_config.py
+-rw-r--r--   0        0        0     2984 2024-05-01 08:33:17.076697 kleene_cli-0.1.0rc3/klee/client/models/volume_inspect.py
+-rw-r--r--   0        0        0     2318 2024-05-01 08:33:17.136698 kleene_cli-0.1.0rc3/klee/client/models/web_socket_message.py
+-rw-r--r--   0        0        0      198 2024-05-01 08:33:09.504619 kleene_cli-0.1.0rc3/klee/client/models/web_socket_message_msg_type.py
+-rw-r--r--   0        0        0      969 2024-05-01 08:33:17.040697 kleene_cli-0.1.0rc3/klee/client/types.py
+-rw-r--r--   0        0        0     3679 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc3/klee/config.py
+-rw-r--r--   0        0        0     3199 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc3/klee/connection.py
+-rw-r--r--   0        0        0    21429 2024-04-28 16:30:13.209459 kleene_cli-0.1.0rc3/klee/container.py
+-rw-r--r--   0        0        0     4573 2023-11-01 16:20:47.318593 kleene_cli-0.1.0rc3/klee/custom_client_templates/endpoint_module.py.jinja
+-rw-r--r--   0        0        0     5397 2024-04-29 20:07:48.058814 kleene_cli-0.1.0rc3/klee/docs_generator.py
+-rw-r--r--   0        0        0    15707 2024-05-01 08:28:48.189875 kleene_cli-0.1.0rc3/klee/image.py
+-rw-r--r--   0        0        0      700 2024-04-21 05:50:28.406645 kleene_cli-0.1.0rc3/klee/inspect.py
+-rw-r--r--   0        0        0      156 2024-04-02 10:04:21.448452 kleene_cli-0.1.0rc3/klee/main.py
+-rw-r--r--   0        0        0    50283 2024-04-02 10:04:21.464452 kleene_cli-0.1.0rc3/klee/name_generator.py
+-rw-r--r--   0        0        0     9636 2024-04-29 21:00:38.105601 kleene_cli-0.1.0rc3/klee/network.py
+-rw-r--r--   0        0        0     3670 2024-04-22 14:42:10.288859 kleene_cli-0.1.0rc3/klee/options.py
+-rw-r--r--   0        0        0     9801 2024-04-29 20:09:13.644770 kleene_cli-0.1.0rc3/klee/printing.py
+-rw-r--r--   0        0        0      688 2024-04-02 10:04:21.452452 kleene_cli-0.1.0rc3/klee/prune.py
+-rw-r--r--   0        0        0     5037 2024-04-29 20:19:32.858561 kleene_cli-0.1.0rc3/klee/root.py
+-rw-r--r--   0        0        0      601 2024-04-28 16:17:00.577770 kleene_cli-0.1.0rc3/klee/shortcuts.py
+-rw-r--r--   0        0        0     4942 2024-04-02 10:04:21.452452 kleene_cli-0.1.0rc3/klee/utils.py
+-rw-r--r--   0        0        0     3700 2024-04-29 21:02:01.235003 kleene_cli-0.1.0rc3/klee/volume.py
+-rw-r--r--   0        0        0      936 2024-05-02 10:30:20.619379 kleene_cli-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 kleene_cli-0.1.0rc3/PKG-INFO
```

### Comparing `kleene_cli-0.1.0rc2/LICENSE` & `kleene_cli-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/__pycache__/client.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/__pycache__/client.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 12209 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 b12f 0000  a.......$..f./..
+00000000: 610d 0d0a 0000 0000 4afe 3166 b12f 0000  a.......J.1f./..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6401 6c06 5a06 6400 6403 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6508 4700 6404  m.Z.m.Z...e.G.d.
 00000070: 6405 8400 6405 8302 8301 5a0b 6508 4700  d...d.....Z.e.G.
@@ -216,17 +216,17 @@
 00000d70: 006a 067c 006a 077c 006a 0864 029c 067c  .j.|.j.|.j.d...|
 00000d80: 006a 09a4 018e 017c 005f 007c 006a 0053  .j.....|._.|.j.S
 00000d90: 0029 03fa 4d47 6574 2074 6865 2075 6e64  .)..MGet the und
 00000da0: 6572 6c79 696e 6720 6874 7470 782e 436c  erlying httpx.Cl
 00000db0: 6965 6e74 2c20 636f 6e73 7472 7563 7469  ient, constructi
 00000dc0: 6e67 2061 206e 6577 206f 6e65 2069 6620  ng a new one if 
 00000dd0: 6e6f 7420 7072 6576 696f 7573 6c79 2073  not previously s
-00000de0: 6574 4ea9 065a 0862 6173 655f 7572 6c72  etN..Z.base_urlr
+00000de0: 6574 4ea9 06da 0862 6173 655f 7572 6c72  etN....base_urlr
 00000df0: 2700 0000 721c 0000 0072 2d00 0000 da06  '...r....r-.....
-00000e00: 7665 7269 6679 5a10 666f 6c6c 6f77 5f72  verifyZ.follow_r
+00000e00: 7665 7269 6679 da10 666f 6c6c 6f77 5f72  verify..follow_r
 00000e10: 6564 6972 6563 7473 290a 7219 0000 00da  edirects).r.....
 00000e20: 0568 7474 7078 7209 0000 0072 0e00 0000  .httpxr....r....
 00000e30: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
 00000e40: 1400 0000 7215 0000 0072 1600 0000 a901  ....r....r......
 00000e50: 7222 0000 0072 2300 0000 7223 0000 0072  r"...r#...r#...r
 00000e60: 2400 0000 da10 6765 745f 6874 7470 785f  $.....get_httpx_
 00000e70: 636c 6965 6e74 5000 0000 7318 0000 0000  clientP...s.....
@@ -237,32 +237,32 @@
 00000ec0: 0002 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
 00000ed0: a000 a100 a001 a100 0100 7c00 5300 a901  ..........|.S...
 00000ee0: 7551 0000 0045 6e74 6572 2061 2063 6f6e  uQ...Enter a con
 00000ef0: 7465 7874 206d 616e 6167 6572 2066 6f72  text manager for
 00000f00: 2073 656c 662e 636c 6965 6e74 e280 9479   self.client...y
 00000f10: 6f75 2063 616e 6e6f 7420 656e 7465 7220  ou cannot enter 
 00000f20: 7477 6963 6520 2873 6565 2068 7474 7078  twice (see httpx
-00000f30: 2064 6f63 7329 a902 723e 0000 00da 095f   docs)..r>....._
-00000f40: 5f65 6e74 6572 5f5f 723d 0000 0072 2300  _enter__r=...r#.
-00000f50: 0000 7223 0000 0072 2400 0000 7241 0000  ..r#...r$...rA..
+00000f30: 2064 6f63 7329 a902 7240 0000 00da 095f   docs)..r@....._
+00000f40: 5f65 6e74 6572 5f5f 723f 0000 0072 2300  _enter__r?...r#.
+00000f50: 0000 7223 0000 0072 2400 0000 7243 0000  ..r#...r$...rC..
 00000f60: 005e 0000 0073 0400 0000 0002 0c01 7a10  .^...s........z.
 00000f70: 436c 6965 6e74 2e5f 5f65 6e74 6572 5f5f  Client.__enter__
 00000f80: a903 da04 6172 6773 da06 6b77 6172 6773  ....args..kwargs
 00000f90: 721d 0000 0063 0100 0000 0000 0000 0000  r....c..........
 00000fa0: 0000 0300 0000 0400 0000 4f00 0000 7318  ..........O...s.
 00000fb0: 0000 007c 00a0 00a1 006a 017c 0169 007c  ...|.....j.|.i.|
 00000fc0: 02a4 018e 0101 0064 0153 00a9 027a 4145  .......d.S...zAE
 00000fd0: 7869 7420 6120 636f 6e74 6578 7420 6d61  xit a context ma
 00000fe0: 6e61 6765 7220 666f 7220 696e 7465 726e  nager for intern
 00000ff0: 616c 2068 7474 7078 2e43 6c69 656e 7420  al httpx.Client 
 00001000: 2873 6565 2068 7474 7078 2064 6f63 7329  (see httpx docs)
-00001010: 4ea9 0272 3e00 0000 da08 5f5f 6578 6974  N..r>.....__exit
-00001020: 5f5f a903 7222 0000 0072 4300 0000 7244  __..r"...rC...rD
+00001010: 4ea9 0272 4000 0000 da08 5f5f 6578 6974  N..r@.....__exit
+00001020: 5f5f a903 7222 0000 0072 4500 0000 7246  __..r"...rE...rF
 00001030: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00001040: 0000 7247 0000 0063 0000 0073 0200 0000  ..rG...c...s....
+00001040: 0000 7249 0000 0063 0000 0073 0200 0000  ..rI...c...s....
 00001050: 0002 7a0f 436c 6965 6e74 2e5f 5f65 7869  ..z.Client.__exi
 00001060: 745f 5fa9 02da 0c61 7379 6e63 5f63 6c69  t__....async_cli
 00001070: 656e 7472 1d00 0000 6302 0000 0000 0000  entr....c.......
 00001080: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00001090: 0073 0a00 0000 7c01 7c00 5f00 7c00 5300  .s....|.|._.|.S.
 000010a0: a901 7aa3 4d61 6e75 616c 6c79 2074 6865  ..z.Manually the
 000010b0: 2075 6e64 6572 6c79 696e 6720 6874 7470   underlying http
@@ -271,15 +271,15 @@
 000010e0: 2054 6869 7320 7769 6c6c 206f 7665 7272   This will overr
 000010f0: 6964 6520 616e 7920 6f74 6865 7220 7365  ide any other se
 00001100: 7474 696e 6773 206f 6e20 7468 6520 636c  ttings on the cl
 00001110: 6965 6e74 2c20 696e 636c 7564 696e 6720  ient, including 
 00001120: 636f 6f6b 6965 732c 2068 6561 6465 7273  cookies, headers
 00001130: 2c20 616e 6420 7469 6d65 6f75 742e 0a20  , and timeout.. 
 00001140: 2020 2020 2020 20a9 0172 1a00 0000 a902         ..r......
-00001150: 7222 0000 0072 4a00 0000 7223 0000 0072  r"...rJ...r#...r
+00001150: 7222 0000 0072 4c00 0000 7223 0000 0072  r"...rL...r#...r
 00001160: 2300 0000 7224 0000 00da 1673 6574 5f61  #...r$.....set_a
 00001170: 7379 6e63 5f68 7474 7078 5f63 6c69 656e  sync_httpx_clien
 00001180: 7467 0000 0073 0400 0000 0005 0601 7a1d  tg...s........z.
 00001190: 436c 6965 6e74 2e73 6574 5f61 7379 6e63  Client.set_async
 000011a0: 5f68 7474 7078 5f63 6c69 656e 7463 0100  _httpx_clientc..
 000011b0: 0000 0000 0000 0000 0000 0100 0000 0900  ................
 000011c0: 0000 4300 0000 733e 0000 007c 006a 0064  ..C...s>...|.j.d
@@ -288,19 +288,19 @@
 000011f0: 006a 0864 029c 067c 006a 09a4 018e 017c  .j.d...|.j.....|
 00001200: 005f 007c 006a 0053 0029 03fa 5247 6574  ._.|.j.S.)..RGet
 00001210: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
 00001220: 6874 7470 782e 4173 796e 6343 6c69 656e  httpx.AsyncClien
 00001230: 742c 2063 6f6e 7374 7275 6374 696e 6720  t, constructing 
 00001240: 6120 6e65 7720 6f6e 6520 6966 206e 6f74  a new one if not
 00001250: 2070 7265 7669 6f75 736c 7920 7365 744e   previously setN
-00001260: 723a 0000 0029 0a72 1a00 0000 723c 0000  r:...).r....r<..
+00001260: 723a 0000 0029 0a72 1a00 0000 723e 0000  r:...).r....r>..
 00001270: 00da 0b41 7379 6e63 436c 6965 6e74 720e  ...AsyncClientr.
 00001280: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
 00001290: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-000012a0: 0072 3d00 0000 7223 0000 0072 2300 0000  .r=...r#...r#...
+000012a0: 0072 3f00 0000 7223 0000 0072 2300 0000  .r?...r#...r#...
 000012b0: 7224 0000 00da 1667 6574 5f61 7379 6e63  r$.....get_async
 000012c0: 5f68 7474 7078 5f63 6c69 656e 746f 0000  _httpx_cliento..
 000012d0: 0073 1800 0000 0002 0a01 0601 0401 0401  .s..............
 000012e0: 0401 0401 0401 04fa 0407 04f9 0809 7a1d  ..............z.
 000012f0: 436c 6965 6e74 2e67 6574 5f61 7379 6e63  Client.get_async
 00001300: 5f68 7474 7078 5f63 6c69 656e 7463 0100  _httpx_clientc..
 00001310: 0000 0000 0000 0000 0000 0100 0000 0200  ................
@@ -308,48 +308,48 @@
 00001330: 00a0 01a1 0049 0064 0148 0001 007c 0053  .....I.d.H...|.S
 00001340: 00a9 0275 6200 0000 456e 7465 7220 6120  ...ub...Enter a 
 00001350: 636f 6e74 6578 7420 6d61 6e61 6765 7220  context manager 
 00001360: 666f 7220 756e 6465 726c 7969 6e67 2068  for underlying h
 00001370: 7474 7078 2e41 7379 6e63 436c 6965 6e74  ttpx.AsyncClient
 00001380: e280 9479 6f75 2063 616e 6e6f 7420 656e  ...you cannot en
 00001390: 7465 7220 7477 6963 6520 2873 6565 2068  ter twice (see h
-000013a0: 7474 7078 2064 6f63 7329 4ea9 0272 5100  ttpx docs)N..rQ.
-000013b0: 0000 da0a 5f5f 6165 6e74 6572 5f5f 723d  ....__aenter__r=
+000013a0: 7474 7078 2064 6f63 7329 4ea9 0272 5300  ttpx docs)N..rS.
+000013b0: 0000 da0a 5f5f 6165 6e74 6572 5f5f 723f  ....__aenter__r?
 000013c0: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-000013d0: 0000 7254 0000 007d 0000 0073 0400 0000  ..rT...}...s....
+000013d0: 0000 7256 0000 007d 0000 0073 0400 0000  ..rV...}...s....
 000013e0: 0002 1201 7a11 436c 6965 6e74 2e5f 5f61  ....z.Client.__a
 000013f0: 656e 7465 725f 5f63 0100 0000 0000 0000  enter__c........
 00001400: 0000 0000 0300 0000 0400 0000 cf00 0000  ................
 00001410: 731e 0000 007c 00a0 00a1 006a 017c 0169  s....|.....j.|.i
 00001420: 007c 02a4 018e 0149 0064 0148 0001 0064  .|.....I.d.H...d
 00001430: 0153 00a9 027a 4845 7869 7420 6120 636f  .S...zHExit a co
 00001440: 6e74 6578 7420 6d61 6e61 6765 7220 666f  ntext manager fo
 00001450: 7220 756e 6465 726c 7969 6e67 2068 7474  r underlying htt
 00001460: 7078 2e41 7379 6e63 436c 6965 6e74 2028  px.AsyncClient (
 00001470: 7365 6520 6874 7470 7820 646f 6373 294e  see httpx docs)N
-00001480: a902 7251 0000 00da 095f 5f61 6578 6974  ..rQ.....__aexit
-00001490: 5f5f 7248 0000 0072 2300 0000 7223 0000  __rH...r#...r#..
-000014a0: 0072 2400 0000 7257 0000 0082 0000 0073  .r$...rW.......s
+00001480: a902 7253 0000 00da 095f 5f61 6578 6974  ..rS.....__aexit
+00001490: 5f5f 724a 0000 0072 2300 0000 7223 0000  __rJ...r#...r#..
+000014a0: 0072 2400 0000 7259 0000 0082 0000 0073  .r$...rY.......s
 000014b0: 0200 0000 0002 7a10 436c 6965 6e74 2e5f  ......z.Client._
 000014c0: 5f61 6578 6974 5f5f 2927 da08 5f5f 6e61  _aexit__)'..__na
 000014d0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 000014e0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 000014f0: 5f5f 646f 635f 5f72 0800 0000 720d 0000  __doc__r....r...
 00001500: 00da 0462 6f6f 6cda 0f5f 5f61 6e6e 6f74  ...bool..__annot
 00001510: 6174 696f 6e73 5f5f da03 7374 72da 0464  ations__..str..d
 00001520: 6963 7472 1100 0000 7203 0000 0072 1200  ictr....r....r..
-00001530: 0000 7213 0000 0072 0400 0000 723c 0000  ..r....r....r<..
+00001530: 0000 7213 0000 0072 0400 0000 723e 0000  ..r....r....r>..
 00001540: 00da 0754 696d 656f 7574 7214 0000 0072  ...Timeoutr....r
 00001550: 0500 0000 da03 7373 6cda 0a53 534c 436f  ......ssl..SSLCo
 00001560: 6e74 6578 7472 1500 0000 7216 0000 0072  ntextr....r....r
 00001570: 0200 0000 7219 0000 0072 0900 0000 721a  ....r....r....r.
-00001580: 0000 0072 5000 0000 7225 0000 0072 2b00  ...rP...r%...r+.
-00001590: 0000 7231 0000 0072 3700 0000 723e 0000  ..r1...r7...r>..
-000015a0: 0072 4100 0000 7247 0000 0072 4e00 0000  .rA...rG...rN...
-000015b0: 7251 0000 0072 5400 0000 7257 0000 0072  rQ...rT...rW...r
+00001580: 0000 0072 5200 0000 7225 0000 0072 2b00  ...rR...r%...r+.
+00001590: 0000 7231 0000 0072 3700 0000 7240 0000  ..r1...r7...r@..
+000015a0: 0072 4300 0000 7249 0000 0072 5000 0000  .rC...rI...rP...
+000015b0: 7253 0000 0072 5600 0000 7259 0000 0072  rS...rV...rY...r
 000015c0: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
 000015d0: 0000 0072 0900 0000 0800 0000 732c 0000  ...r........s,..
 000015e0: 000a 0204 1b14 0108 011c 011c 011a 0120  ............... 
 000015f0: 0114 011c 011a 011a 0218 0818 0812 0812  ................
 00001600: 0810 0e0e 0512 0412 0810 0e0e 0572 0900  .............r..
 00001610: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00001620: 0000 0004 0000 0040 0000 0073 ea01 0000  .......@...s....
@@ -477,15 +477,15 @@
 00001dc0: 7468 6520 4175 7468 6f72 697a 6174 696f  the Authorizatio
 00001dd0: 6e20 6865 6164 6572 0a20 2020 2046 5472  n header.    FTr
 00001de0: 0a00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
 00001df0: 0000 0072 1100 0000 7212 0000 004e 7213  ...r....r....Nr.
 00001e00: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
 00001e10: 0000 7217 0000 0072 1900 0000 721a 0000  ..r....r....r...
 00001e20: 00da 0574 6f6b 656e 5a06 4265 6172 6572  ...tokenZ.Bearer
-00001e30: da06 7072 6566 6978 5a0d 4175 7468 6f72  ..prefixZ.Author
+00001e30: da06 7072 6566 6978 da0d 4175 7468 6f72  ..prefix..Author
 00001e40: 697a 6174 696f 6eda 1061 7574 685f 6865  ization..auth_he
 00001e50: 6164 6572 5f6e 616d 6572 1b00 0000 6302  ader_namer....c.
 00001e60: 0000 0000 0000 0000 0000 0002 0000 0004  ................
 00001e70: 0000 0043 0000 0073 4600 0000 7c00 6a00  ...C...sF...|.j.
 00001e80: 6401 7501 7218 7c00 6a00 6a01 a002 7c01  d.u.r.|.j.j...|.
 00001e90: a101 0100 7c00 6a03 6401 7501 7230 7c00  ....|.j.d.u.r0|.
 00001ea0: 6a03 6a01 a002 7c01 a101 0100 7404 7c00  j.j...|.....t.|.
@@ -532,106 +532,106 @@
 00002130: 6401 7500 725e 7c00 6a01 7222 7c00 6a01  d.u.r^|.j.r"|.j.
 00002140: 9b00 6402 7c00 6a02 9b00 9d03 6e04 7c00  ..d.|.j.....n.|.
 00002150: 6a02 7c00 6a03 7c00 6a04 3c00 7405 6a06  j.|.j.|.j.<.t.j.
 00002160: 6600 7c00 6a07 7c00 6a08 7c00 6a03 7c00  f.|.j.|.j.|.j.|.
 00002170: 6a09 7c00 6a0a 7c00 6a0b 6403 9c06 7c00  j.|.j.|.j.d...|.
 00002180: 6a0c a401 8e01 7c00 5f00 7c00 6a00 5300  j.....|._.|.j.S.
 00002190: 2904 7239 0000 004e fa01 2072 3a00 0000  ).r9...N.. r:...
-000021a0: 290d 7219 0000 0072 6500 0000 7264 0000  ).r....re...rd..
-000021b0: 0072 1200 0000 7266 0000 0072 3c00 0000  .r....rf...r<...
+000021a0: 290d 7219 0000 0072 6700 0000 7266 0000  ).r....rg...rf..
+000021b0: 0072 1200 0000 7269 0000 0072 3e00 0000  .r....ri...r>...
 000021c0: 7209 0000 0072 0e00 0000 7211 0000 0072  r....r....r....r
 000021d0: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
-000021e0: 0000 0072 3d00 0000 7223 0000 0072 2300  ...r=...r#...r#.
-000021f0: 0000 7224 0000 0072 3e00 0000 d600 0000  ..r$...r>.......
+000021e0: 0000 0072 3f00 0000 7223 0000 0072 2300  ...r?...r#...r#.
+000021f0: 0000 7224 0000 0072 4000 0000 d600 0000  ..r$...r@.......
 00002200: 731c 0000 0000 020a 021c ff0a 0306 0104  s...............
 00002210: 0104 0104 0104 0104 0104 fa04 0704 f908  ................
 00002220: 097a 2441 7574 6865 6e74 6963 6174 6564  .z$Authenticated
 00002230: 436c 6965 6e74 2e67 6574 5f68 7474 7078  Client.get_httpx
 00002240: 5f63 6c69 656e 7463 0100 0000 0000 0000  _clientc........
 00002250: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
 00002260: 7310 0000 007c 00a0 00a1 00a0 01a1 0001  s....|..........
-00002270: 007c 0053 0072 3f00 0000 7240 0000 0072  .|.S.r?...r@...r
-00002280: 3d00 0000 7223 0000 0072 2300 0000 7224  =...r#...r#...r$
-00002290: 0000 0072 4100 0000 e700 0000 7304 0000  ...rA.......s...
+00002270: 007c 0053 0072 4100 0000 7242 0000 0072  .|.S.rA...rB...r
+00002280: 3f00 0000 7223 0000 0072 2300 0000 7224  ?...r#...r#...r$
+00002290: 0000 0072 4300 0000 e700 0000 7304 0000  ...rC.......s...
 000022a0: 0000 020c 017a 1d41 7574 6865 6e74 6963  .....z.Authentic
 000022b0: 6174 6564 436c 6965 6e74 2e5f 5f65 6e74  atedClient.__ent
-000022c0: 6572 5f5f 7242 0000 0063 0100 0000 0000  er__rB...c......
+000022c0: 6572 5f5f 7244 0000 0063 0100 0000 0000  er__rD...c......
 000022d0: 0000 0000 0000 0300 0000 0400 0000 4f00  ..............O.
 000022e0: 0000 7318 0000 007c 00a0 00a1 006a 017c  ..s....|.....j.|
 000022f0: 0169 007c 02a4 018e 0101 0064 0153 0072  .i.|.......d.S.r
-00002300: 4500 0000 7246 0000 0072 4800 0000 7223  E...rF...rH...r#
-00002310: 0000 0072 2300 0000 7224 0000 0072 4700  ...r#...r$...rG.
+00002300: 4700 0000 7248 0000 0072 4a00 0000 7223  G...rH...rJ...r#
+00002310: 0000 0072 2300 0000 7224 0000 0072 4900  ...r#...r$...rI.
 00002320: 0000 ec00 0000 7302 0000 0000 027a 1c41  ......s......z.A
 00002330: 7574 6865 6e74 6963 6174 6564 436c 6965  uthenticatedClie
-00002340: 6e74 2e5f 5f65 7869 745f 5f72 4900 0000  nt.__exit__rI...
+00002340: 6e74 2e5f 5f65 7869 745f 5f72 4b00 0000  nt.__exit__rK...
 00002350: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
 00002360: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00002370: 7c00 5f00 7c00 5300 724b 0000 0072 4c00  |._.|.S.rK...rL.
-00002380: 0000 724d 0000 0072 2300 0000 7223 0000  ..rM...r#...r#..
-00002390: 0072 2400 0000 724e 0000 00f0 0000 0073  .r$...rN.......s
+00002370: 7c00 5f00 7c00 5300 724d 0000 0072 4e00  |._.|.S.rM...rN.
+00002380: 0000 724f 0000 0072 2300 0000 7223 0000  ..rO...r#...r#..
+00002390: 0072 2400 0000 7250 0000 00f0 0000 0073  .r$...rP.......s
 000023a0: 0400 0000 0007 0601 7a2a 4175 7468 656e  ........z*Authen
 000023b0: 7469 6361 7465 6443 6c69 656e 742e 7365  ticatedClient.se
 000023c0: 745f 6173 796e 635f 6874 7470 785f 636c  t_async_httpx_cl
 000023d0: 6965 6e74 6301 0000 0000 0000 0000 0000  ientc...........
 000023e0: 0001 0000 0009 0000 0043 0000 0073 6400  .........C...sd.
 000023f0: 0000 7c00 6a00 6401 7500 725e 7c00 6a01  ..|.j.d.u.r^|.j.
 00002400: 7222 7c00 6a01 9b00 6402 7c00 6a02 9b00  r"|.j...d.|.j...
 00002410: 9d03 6e04 7c00 6a02 7c00 6a03 7c00 6a04  ..n.|.j.|.j.|.j.
 00002420: 3c00 7405 6a06 6600 7c00 6a07 7c00 6a08  <.t.j.f.|.j.|.j.
 00002430: 7c00 6a03 7c00 6a09 7c00 6a0a 7c00 6a0b  |.j.|.j.|.j.|.j.
 00002440: 6403 9c06 7c00 6a0c a401 8e01 7c00 5f00  d...|.j.....|._.
-00002450: 7c00 6a00 5300 2904 724f 0000 004e 7267  |.j.S.).rO...Nrg
+00002450: 7c00 6a00 5300 2904 7251 0000 004e 726a  |.j.S.).rQ...Nrj
 00002460: 0000 0072 3a00 0000 290d 721a 0000 0072  ...r:...).r....r
-00002470: 6500 0000 7264 0000 0072 1200 0000 7266  e...rd...r....rf
-00002480: 0000 0072 3c00 0000 7250 0000 0072 0e00  ...r<...rP...r..
+00002470: 6700 0000 7266 0000 0072 1200 0000 7269  g...rf...r....ri
+00002480: 0000 0072 3e00 0000 7252 0000 0072 0e00  ...r>...rR...r..
 00002490: 0000 7211 0000 0072 1300 0000 7214 0000  ..r....r....r...
-000024a0: 0072 1500 0000 7216 0000 0072 3d00 0000  .r....r....r=...
+000024a0: 0072 1500 0000 7216 0000 0072 3f00 0000  .r....r....r?...
 000024b0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
-000024c0: 5100 0000 fa00 0000 731c 0000 0000 020a  Q.......s.......
+000024c0: 5300 0000 fa00 0000 731c 0000 0000 020a  S.......s.......
 000024d0: 021c ff0a 0306 0104 0104 0104 0104 0104  ................
 000024e0: 0104 fa04 0704 f908 097a 2a41 7574 6865  .........z*Authe
 000024f0: 6e74 6963 6174 6564 436c 6965 6e74 2e67  nticatedClient.g
 00002500: 6574 5f61 7379 6e63 5f68 7474 7078 5f63  et_async_httpx_c
 00002510: 6c69 656e 7463 0100 0000 0000 0000 0000  lientc..........
 00002520: 0000 0100 0000 0200 0000 c300 0000 7316  ..............s.
 00002530: 0000 007c 00a0 00a1 00a0 01a1 0049 0064  ...|.........I.d
-00002540: 0148 0001 007c 0053 0072 5200 0000 7253  .H...|.S.rR...rS
-00002550: 0000 0072 3d00 0000 7223 0000 0072 2300  ...r=...r#...r#.
-00002560: 0000 7224 0000 0072 5400 0000 0b01 0000  ..r$...rT.......
+00002540: 0148 0001 007c 0053 0072 5400 0000 7255  .H...|.S.rT...rU
+00002550: 0000 0072 3f00 0000 7223 0000 0072 2300  ...r?...r#...r#.
+00002560: 0000 7224 0000 0072 5600 0000 0b01 0000  ..r$...rV.......
 00002570: 7304 0000 0000 0212 017a 1e41 7574 6865  s........z.Authe
 00002580: 6e74 6963 6174 6564 436c 6965 6e74 2e5f  nticatedClient._
 00002590: 5f61 656e 7465 725f 5f63 0100 0000 0000  _aenter__c......
 000025a0: 0000 0000 0000 0300 0000 0400 0000 cf00  ................
 000025b0: 0000 731e 0000 007c 00a0 00a1 006a 017c  ..s....|.....j.|
 000025c0: 0169 007c 02a4 018e 0149 0064 0148 0001  .i.|.....I.d.H..
-000025d0: 0064 0153 0072 5500 0000 7256 0000 0072  .d.S.rU...rV...r
-000025e0: 4800 0000 7223 0000 0072 2300 0000 7224  H...r#...r#...r$
-000025f0: 0000 0072 5700 0000 1001 0000 7302 0000  ...rW.......s...
+000025d0: 0064 0153 0072 5700 0000 7258 0000 0072  .d.S.rW...rX...r
+000025e0: 4a00 0000 7223 0000 0072 2300 0000 7224  J...r#...r#...r$
+000025f0: 0000 0072 5900 0000 1001 0000 7302 0000  ...rY.......s...
 00002600: 0000 027a 1d41 7574 6865 6e74 6963 6174  ...z.Authenticat
 00002610: 6564 436c 6965 6e74 2e5f 5f61 6578 6974  edClient.__aexit
-00002620: 5f5f 2929 7258 0000 0072 5900 0000 725a  __))rX...rY...rZ
-00002630: 0000 0072 5b00 0000 7208 0000 0072 0d00  ...r[...r....r..
-00002640: 0000 725c 0000 0072 5d00 0000 725e 0000  ..r\...r]...r^..
-00002650: 0072 5f00 0000 7211 0000 0072 0300 0000  .r_...r....r....
+00002620: 5f5f 2929 725a 0000 0072 5b00 0000 725c  __))rZ...r[...r\
+00002630: 0000 0072 5d00 0000 7208 0000 0072 0d00  ...r]...r....r..
+00002640: 0000 725e 0000 0072 5f00 0000 7260 0000  ..r^...r_...r`..
+00002650: 0072 6100 0000 7211 0000 0072 0300 0000  .ra...r....r....
 00002660: 7212 0000 0072 1300 0000 7204 0000 0072  r....r....r....r
-00002670: 3c00 0000 7260 0000 0072 1400 0000 7205  <...r`...r....r.
-00002680: 0000 0072 6100 0000 7262 0000 0072 1500  ...ra...rb...r..
+00002670: 3e00 0000 7262 0000 0072 1400 0000 7205  >...rb...r....r.
+00002680: 0000 0072 6300 0000 7264 0000 0072 1500  ...rc...rd...r..
 00002690: 0000 7216 0000 0072 0200 0000 7219 0000  ..r....r....r...
-000026a0: 0072 0900 0000 721a 0000 0072 5000 0000  .r....r....rP...
-000026b0: 7265 0000 0072 6600 0000 7225 0000 0072  re...rf...r%...r
-000026c0: 2b00 0000 7231 0000 0072 3700 0000 723e  +...r1...r7...r>
-000026d0: 0000 0072 4100 0000 7247 0000 0072 4e00  ...rA...rG...rN.
-000026e0: 0000 7251 0000 0072 5400 0000 7257 0000  ..rQ...rT...rW..
+000026a0: 0072 0900 0000 721a 0000 0072 5200 0000  .r....r....rR...
+000026b0: 7267 0000 0072 6900 0000 7225 0000 0072  rg...ri...r%...r
+000026c0: 2b00 0000 7231 0000 0072 3700 0000 7240  +...r1...r7...r@
+000026d0: 0000 0072 4300 0000 7249 0000 0072 5000  ...rC...rI...rP.
+000026e0: 0000 7253 0000 0072 5600 0000 7259 0000  ..rS...rV...rY..
 000026f0: 0072 2300 0000 7223 0000 0072 2300 0000  .r#...r#...r#...
-00002700: 7224 0000 0072 6300 0000 8700 0000 7336  r$...rc.......s6
+00002700: 7224 0000 0072 6500 0000 8700 0000 7336  r$...re.......s6
 00002710: 0000 000a 0204 1e14 0108 011c 011c 011a  ................
 00002720: 0120 0114 011c 011a 011a 0208 010c 010c  . ..............
 00002730: 0218 0818 0812 0812 0810 110e 0512 0504  ................
-00002740: 0102 fe0c 0a10 110e 0572 6300 0000 290d  .........rc...).
-00002750: 7261 0000 00da 0674 7970 696e 6772 0200  ra.....typingr..
+00002740: 0102 fe0c 0a10 110e 0572 6500 0000 290d  .........re...).
+00002750: 7263 0000 00da 0674 7970 696e 6772 0200  rc.....typingr..
 00002760: 0000 7203 0000 0072 0400 0000 7205 0000  ..r....r....r...
-00002770: 0072 3c00 0000 da05 6174 7472 7372 0600  .r<.....attrsr..
+00002770: 0072 3e00 0000 da05 6174 7472 7372 0600  .r>.....attrsr..
 00002780: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
-00002790: 0072 6300 0000 7223 0000 0072 2300 0000  .rc...r#...r#...
+00002790: 0072 6500 0000 7223 0000 0072 2300 0000  .re...r#...r#...
 000027a0: 7223 0000 0072 2400 0000 da08 3c6d 6f64  r#...r$.....<mod
 000027b0: 756c 653e 0100 0000 730e 0000 0008 0118  ule>....s.......
 000027c0: 0208 0114 0302 0110 7e02 01              ........~..
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/__pycache__/types.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/__pycache__/types.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:46 2024 UTC, .py size: 969 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 26b1 1d66 c903 0000  a.......&..f....
+00000000: 610d 0d0a 0000 0000 4dfe 3166 c903 0000  a.......M.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 b200 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 6d05 5a05 6d06  d.d.l.m.Z.m.Z.m.
 00000050: 5a06 6d07 5a07 6d08 5a08 6d09 5a09 6d0a  Z.m.Z.m.Z.m.Z.m.
 00000060: 5a0a 0100 6401 6404 6c0b 6d0c 5a0c 0100  Z...d.d.l.m.Z...
 00000070: 4700 6405 6406 8400 6406 8302 5a0d 650d  G.d.d...d...Z.e.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_create.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_create.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:40 2024 UTC, .py size: 5464 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 20b1 1d66 5815 0000  a....... ..fX...
+00000000: 610d 0d0a 0000 0000 47fe 3166 5815 0000  a.......G.1fX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7c01 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -38,23 +38,23 @@
 00000250: 6f6e 5f62 6f64 79da 0672 6574 7572 6e63  on_body..returnc
 00000260: 0000 0000 0000 0000 0100 0000 0200 0000  ................
 00000270: 0400 0000 4300 0000 7314 0000 007c 00a0  ....C...s....|..
 00000280: 00a1 007d 0164 0164 027c 0164 039c 0353  ...}.d.d.|.d...S
 00000290: 0029 044e da04 706f 7374 7a12 2f63 6f6e  .).N..postz./con
 000002a0: 7461 696e 6572 732f 6372 6561 7465 2903  tainers/create).
 000002b0: da06 6d65 7468 6f64 da03 7572 6cda 046a  ..method..url..j
-000002c0: 736f 6e29 015a 0774 6f5f 6469 6374 2902  son).Z.to_dict).
+000002c0: 736f 6e29 01da 0774 6f5f 6469 6374 2902  son)...to_dict).
 000002d0: 720f 0000 005a 0e6a 736f 6e5f 6a73 6f6e  r....Z.json_json
-000002e0: 5f62 6f64 79a9 0072 1500 0000 fa39 2f76  _body..r.....9/v
+000002e0: 5f62 6f64 79a9 0072 1600 0000 fa39 2f76  _body..r.....9/v
 000002f0: 6167 7261 6e74 2f6b 6c65 652f 6b6c 6565  agrant/klee/klee
 00000300: 2f63 6c69 656e 742f 6170 692f 6465 6661  /client/api/defa
 00000310: 756c 742f 636f 6e74 6169 6e65 725f 6372  ult/container_cr
 00000320: 6561 7465 2e70 79da 0b5f 6765 745f 6b77  eate.py.._get_kw
 00000330: 6172 6773 0e00 0000 730a 0000 0000 0708  args....s.......
-00000340: 0302 0102 0102 fd72 1700 0000 2903 da06  .......r....)...
+00000340: 0302 0102 0102 fd72 1800 0000 2903 da06  .......r....)...
 00000350: 636c 6965 6e74 da08 7265 7370 6f6e 7365  client..response
 00000360: 7210 0000 0063 0000 0000 0000 0000 0200  r....c..........
 00000370: 0000 0500 0000 0400 0000 4300 0000 737a  ..........C...sz
 00000380: 0000 007c 016a 0074 016a 026b 0272 1e74  ...|.j.t.j.k.r.t
 00000390: 03a0 047c 01a0 05a1 00a1 017d 027c 0253  ...|.......}.|.S
 000003a0: 007c 016a 0074 016a 066b 0272 3c74 07a0  .|.j.t.j.k.r<t..
 000003b0: 047c 01a0 05a1 00a1 017d 037c 0353 007c  .|.......}.|.S.|
@@ -65,37 +65,37 @@
 00000400: 290d da0b 7374 6174 7573 5f63 6f64 6572  )...status_coder
 00000410: 0200 0000 da07 4352 4541 5445 4472 0d00  ......CREATEDr..
 00000420: 0000 da09 6672 6f6d 5f64 6963 7472 1400  ....from_dictr..
 00000430: 0000 da09 4e4f 545f 464f 554e 4472 0c00  ....NOT_FOUNDr..
 00000440: 0000 da15 494e 5445 524e 414c 5f53 4552  ....INTERNAL_SER
 00000450: 5645 525f 4552 524f 52da 1a72 6169 7365  VER_ERROR..raise
 00000460: 5f6f 6e5f 756e 6578 7065 6374 6564 5f73  _on_unexpected_s
-00000470: 7461 7475 7372 0800 0000 5a10 556e 6578  tatusr....Z.Unex
+00000470: 7461 7475 7372 0800 0000 da10 556e 6578  tatusr......Unex
 00000480: 7065 6374 6564 5374 6174 7573 da07 636f  pectedStatus..co
-00000490: 6e74 656e 7429 0572 1800 0000 7219 0000  ntent).r....r...
-000004a0: 005a 0c72 6573 706f 6e73 655f 3230 315a  .Z.response_201Z
-000004b0: 0c72 6573 706f 6e73 655f 3430 345a 0c72  .response_404Z.r
-000004c0: 6573 706f 6e73 655f 3530 3072 1500 0000  esponse_500r....
-000004d0: 7215 0000 0072 1600 0000 da0f 5f70 6172  r....r......_par
+00000490: 6e74 656e 7429 0572 1900 0000 721a 0000  ntent).r....r...
+000004a0: 005a 0c72 6573 706f 6e73 655f 3230 31da  .Z.response_201.
+000004b0: 0c72 6573 706f 6e73 655f 3430 34da 0c72  .response_404..r
+000004c0: 6573 706f 6e73 655f 3530 3072 1600 0000  esponse_500r....
+000004d0: 7216 0000 0072 1700 0000 da0f 5f70 6172  r....r......_par
 000004e0: 7365 5f72 6573 706f 6e73 651e 0000 0073  se_response....s
 000004f0: 1800 0000 0003 0c01 0e02 0401 0c01 0e02  ................
-00000500: 0401 0c01 0e02 0401 0601 1202 7221 0000  ............r!..
+00000500: 0401 0c01 0e02 0401 0601 1202 7225 0000  ............r%..
 00000510: 0063 0000 0000 0000 0000 0200 0000 0200  .c..............
 00000520: 0000 0800 0000 4300 0000 7322 0000 0074  ......C...s"...t
 00000530: 0074 017c 016a 0283 017c 016a 037c 016a  .t.|.j...|.j.|.j
 00000540: 0474 057c 007c 0164 018d 0264 028d 0453  .t.|.|.d...d...S
-00000550: 0029 034e a902 7218 0000 0072 1900 0000  .).N..r....r....
-00000560: 2904 721a 0000 0072 2000 0000 da07 6865  ).r....r .....he
+00000550: 0029 034e a902 7219 0000 0072 1a00 0000  .).N..r....r....
+00000560: 2904 721b 0000 0072 2200 0000 da07 6865  ).r....r".....he
 00000570: 6164 6572 73da 0670 6172 7365 6429 0672  aders..parsed).r
-00000580: 0e00 0000 7202 0000 0072 1a00 0000 7220  ....r....r....r 
-00000590: 0000 0072 2300 0000 7221 0000 0072 2200  ...r#...r!...r".
-000005a0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000580: 0e00 0000 7202 0000 0072 1b00 0000 7222  ....r....r....r"
+00000590: 0000 0072 2700 0000 7225 0000 0072 2600  ...r'...r%...r&.
+000005a0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
 000005b0: 00da 0f5f 6275 696c 645f 7265 7370 6f6e  ..._build_respon
 000005c0: 7365 3300 0000 730c 0000 0000 0302 0108  se3...s.........
-000005d0: 0104 0104 010a fc72 2500 0000 2903 7218  .......r%...).r.
+000005d0: 0104 0104 010a fc72 2900 0000 2903 7219  .......r)...).r.
 000005e0: 0000 0072 0f00 0000 7210 0000 0063 0100  ...r....r....c..
 000005f0: 0000 0000 0000 0200 0000 0500 0000 0500  ................
 00000600: 0000 4b00 0000 733c 0000 007c 03a0 0074  ..K...s<...|...t
 00000610: 017c 0264 018d 01a1 0101 0074 026a 037c  .|.d.......t.j.|
 00000620: 016a 047c 0064 028d 027d 017c 016a 0566  .j.|.d...}.|.j.f
 00000630: 0069 007c 03a4 018e 017d 0474 067c 017c  .i.|.....}.t.|.|
 00000640: 0464 038d 0253 0029 04e1 5902 0000 636f  .d...S.)..Y...co
@@ -134,24 +134,24 @@
 00000850: 6e20 436c 6965 6e74 2e74 696d 656f 7574  n Client.timeout
 00000860: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
 00000870: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
 00000880: 5b55 6e69 6f6e 5b45 7272 6f72 5265 7370  [Union[ErrorResp
 00000890: 6f6e 7365 2c20 4964 5265 7370 6f6e 7365  onse, IdResponse
 000008a0: 5d5d 0a20 2020 20a9 0172 0f00 0000 2902  ]].    ..r....).
 000008b0: da08 6261 7365 5f75 726c da09 7472 616e  ..base_url..tran
-000008c0: 7370 6f72 7472 2200 0000 2907 da06 7570  sportr"...)...up
-000008d0: 6461 7465 7217 0000 00da 0568 7474 7078  dater......httpx
+000008c0: 7370 6f72 7472 2600 0000 2907 da06 7570  sportr&...)...up
+000008d0: 6461 7465 7218 0000 00da 0568 7474 7078  dater......httpx
 000008e0: 720a 0000 00da 095f 6261 7365 5f75 726c  r......_base_url
-000008f0: da07 7265 7175 6573 7472 2500 0000 2905  ..requestr%...).
-00000900: 7229 0000 0072 1800 0000 720f 0000 00da  r)...r....r.....
-00000910: 066b 7761 7267 7372 1900 0000 7215 0000  .kwargsr....r...
-00000920: 0072 1500 0000 7216 0000 00da 0d73 796e  .r....r......syn
+000008f0: da07 7265 7175 6573 7472 2900 0000 2905  ..requestr)...).
+00000900: 722d 0000 0072 1900 0000 720f 0000 00da  r-...r....r.....
+00000910: 066b 7761 7267 7372 1a00 0000 7216 0000  .kwargsr....r...
+00000920: 0072 1600 0000 7217 0000 00da 0d73 796e  .r....r......syn
 00000930: 635f 6465 7461 696c 6564 3e00 0000 7310  c_detailed>...s.
 00000940: 0000 0000 1a04 0102 0102 ff04 ff04 0610  ................
-00000950: 0110 0272 2f00 0000 6300 0000 0000 0000  ...r/...c.......
+00000950: 0110 0272 3300 0000 6300 0000 0000 0000  ...r3...c.......
 00000960: 0002 0000 0002 0000 0004 0000 0043 0000  .............C..
 00000970: 0073 0e00 0000 7400 7c00 7c01 6401 8d02  .s....t.|.|.d...
 00000980: 6a01 5300 2902 e14f 0200 0063 6f6e 7461  j.S.)..O...conta
 00000990: 696e 6572 2063 7265 6174 650a 0a20 2020  iner create..   
 000009a0: 2020 4372 6561 7465 2061 2063 6f6e 7461    Create a conta
 000009b0: 696e 6572 2e0a 0a20 2020 204e 6f74 6520  iner...    Note 
 000009c0: 7468 6174 2069 7420 6973 206e 6f74 2070  that it is not p
@@ -183,53 +183,53 @@
 00000b60: 6f75 7445 7863 6570 7469 6f6e 3a20 4966  outException: If
 00000b70: 2074 6865 2072 6571 7565 7374 2074 616b   the request tak
 00000b80: 6573 206c 6f6e 6765 7220 7468 616e 2043  es longer than C
 00000b90: 6c69 656e 742e 7469 6d65 6f75 742e 0a0a  lient.timeout...
 00000ba0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
 00000bb0: 2020 2020 2055 6e69 6f6e 5b45 7272 6f72       Union[Error
 00000bc0: 5265 7370 6f6e 7365 2c20 4964 5265 7370  Response, IdResp
-00000bd0: 6f6e 7365 5d0a 2020 2020 a902 7218 0000  onse].    ..r...
-00000be0: 0072 0f00 0000 2902 722f 0000 0072 2400  .r....).r/...r$.
-00000bf0: 0000 7231 0000 0072 1500 0000 7215 0000  ..r1...r....r...
-00000c00: 0072 1600 0000 da04 7379 6e63 6400 0000  .r......syncd...
-00000c10: 7308 0000 0000 1802 0102 0102 fe72 3200  s............r2.
+00000bd0: 6f6e 7365 5d0a 2020 2020 a902 7219 0000  onse].    ..r...
+00000be0: 0072 0f00 0000 2902 7233 0000 0072 2800  .r....).r3...r(.
+00000bf0: 0000 7235 0000 0072 1600 0000 7216 0000  ..r5...r....r...
+00000c00: 0072 1700 0000 da04 7379 6e63 6400 0000  .r......syncd...
+00000c10: 7308 0000 0000 1802 0102 0102 fe72 3600  s............r6.
 00000c20: 0000 6300 0000 0000 0000 0002 0000 0004  ..c.............
 00000c30: 0000 0004 0000 00c3 0000 0073 3000 0000  ...........s0...
 00000c40: 7400 7c01 6401 8d01 7d02 7c00 a001 a100  t.|.d...}.|.....
 00000c50: 6a02 6600 6900 7c02 a401 8e01 4900 6402  j.f.i.|.....I.d.
 00000c60: 4800 7d03 7403 7c00 7c03 6403 8d02 5300  H.}.t.|.|.d...S.
-00000c70: 2904 7226 0000 0072 2700 0000 4e72 2200  ).r&...r'...Nr".
-00000c80: 0000 2904 7217 0000 00da 1667 6574 5f61  ..).r......get_a
+00000c70: 2904 722a 0000 0072 2b00 0000 4e72 2600  ).r*...r+...Nr&.
+00000c80: 0000 2904 7218 0000 00da 1667 6574 5f61  ..).r......get_a
 00000c90: 7379 6e63 5f68 7474 7078 5f63 6c69 656e  sync_httpx_clien
-00000ca0: 7472 2d00 0000 7225 0000 0029 0472 1800  tr-...r%...).r..
-00000cb0: 0000 720f 0000 0072 2e00 0000 7219 0000  ..r....r....r...
-00000cc0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000ca0: 7472 3100 0000 7229 0000 0029 0472 1900  tr1...r)...).r..
+00000cb0: 0000 720f 0000 0072 3200 0000 721a 0000  ..r....r2...r...
+00000cc0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
 00000cd0: da10 6173 796e 6369 6f5f 6465 7461 696c  ..asyncio_detail
 00000ce0: 6564 8200 0000 730a 0000 0000 1802 0102  ed....s.........
-00000cf0: ff06 041a 0272 3400 0000 6300 0000 0000  .....r4...c.....
+00000cf0: ff06 041a 0272 3800 0000 6300 0000 0000  .....r8...c.....
 00000d00: 0000 0002 0000 0002 0000 0004 0000 00c3  ................
 00000d10: 0000 0073 1400 0000 7400 7c00 7c01 6401  ...s....t.|.|.d.
-00000d20: 8d02 4900 6402 4800 6a01 5300 2903 7230  ..I.d.H.j.S.).r0
-00000d30: 0000 0072 3100 0000 4e29 0272 3400 0000  ...r1...N).r4...
-00000d40: 7224 0000 0072 3100 0000 7215 0000 0072  r$...r1...r....r
-00000d50: 1500 0000 7216 0000 00da 0761 7379 6e63  ....r......async
+00000d20: 8d02 4900 6402 4800 6a01 5300 2903 7234  ..I.d.H.j.S.).r4
+00000d30: 0000 0072 3500 0000 4e29 0272 3800 0000  ...r5...N).r8...
+00000d40: 7228 0000 0072 3500 0000 7216 0000 0072  r(...r5...r....r
+00000d50: 1600 0000 7217 0000 00da 0761 7379 6e63  ....r......async
 00000d60: 696f a300 0000 730a 0000 0000 1902 0102  io....s.........
-00000d70: 0102 fe0a ff72 3500 0000 291d da04 6874  .....r5...)...ht
+00000d70: 0102 fe0a ff72 3900 0000 291d da04 6874  .....r9...)...ht
 00000d80: 7470 7202 0000 00da 0674 7970 696e 6772  tpr......typingr
 00000d90: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
-00000da0: 0000 0072 2b00 0000 da00 7208 0000 0072  ...r+.....r....r
-00000db0: 1800 0000 7209 0000 0072 0a00 0000 5a17  ....r....r....Z.
+00000da0: 0000 0072 2f00 0000 da00 7208 0000 0072  ...r/.....r....r
+00000db0: 1900 0000 7209 0000 0072 0a00 0000 da17  ....r....r......
 00000dc0: 6d6f 6465 6c73 2e63 6f6e 7461 696e 6572  models.container
 00000dd0: 5f63 6f6e 6669 6772 0b00 0000 5a15 6d6f  _configr....Z.mo
 00000de0: 6465 6c73 2e65 7272 6f72 5f72 6573 706f  dels.error_respo
 00000df0: 6e73 6572 0c00 0000 5a12 6d6f 6465 6c73  nser....Z.models
 00000e00: 2e69 645f 7265 7370 6f6e 7365 720d 0000  .id_responser...
 00000e10: 00da 0574 7970 6573 720e 0000 00da 0373  ...typesr......s
-00000e20: 7472 7217 0000 0072 2100 0000 7225 0000  trr....r!...r%..
-00000e30: 0072 2f00 0000 7232 0000 0072 3400 0000  .r/...r2...r4...
-00000e40: 7235 0000 0072 1500 0000 7215 0000 0072  r5...r....r....r
-00000e50: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
+00000e20: 7472 7218 0000 0072 2500 0000 7229 0000  trr....r%...r)..
+00000e30: 0072 3300 0000 7236 0000 0072 3800 0000  .r3...r6...r8...
+00000e40: 7239 0000 0072 1600 0000 7216 0000 0072  r9...r....r....r
+00000e50: 1600 0000 7217 0000 00da 083c 6d6f 6475  ....r......<modu
 00000e60: 6c65 3e01 0000 0073 4200 0000 0c01 1802  le>....sB.......
 00000e70: 0802 0c01 1001 0c01 0c01 0c01 0c05 0201  ................
 00000e80: 0afd 0c11 0e01 0efe 0c16 0e01 0efe 0c0e  ................
 00000e90: 0a01 0202 0efa 0c28 0a01 0201 0efc 0c20  .......(....... 
 00000ea0: 0a01 0201 0efc 0c23 0a01 0201 0efc       .......#......
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_inspect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_inspect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:40 2024 UTC, .py size: 4628 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 20b1 1d66 1412 0000  a....... ..f....
+00000000: 610d 0d0a 0000 0000 47fe 3166 1412 0000  a.......G.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_list.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_list.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:40 2024 UTC, .py size: 5075 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 20b1 1d66 d313 0000  a....... ..f....
+00000000: 610d 0d0a 0000 0000 47fe 3166 d313 0000  a.......G.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 5a08 6404  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6404 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6404 6407 6c0e  m.Z.m.Z...d.d.l.
@@ -78,39 +78,39 @@
 000004d0: 4bda 046a 736f 6e72 0c00 0000 da09 6672  K..jsonr......fr
 000004e0: 6f6d 5f64 6963 74da 0661 7070 656e 64da  om_dict..append.
 000004f0: 1a72 6169 7365 5f6f 6e5f 756e 6578 7065  .raise_on_unexpe
 00000500: 6374 6564 5f73 7461 7475 7372 0900 0000  cted_statusr....
 00000510: da10 556e 6578 7065 6374 6564 5374 6174  ..UnexpectedStat
 00000520: 7573 da07 636f 6e74 656e 7429 0672 2200  us..content).r".
 00000530: 0000 7223 0000 00da 0c72 6573 706f 6e73  ..r#.....respons
-00000540: 655f 3230 305a 0d5f 7265 7370 6f6e 7365  e_200Z._response
+00000540: 655f 3230 30da 0d5f 7265 7370 6f6e 7365  e_200.._response
 00000550: 5f32 3030 5a32 636f 6d70 6f6e 656e 7473  _200Z2components
 00000560: 7363 6865 6d61 735f 636f 6e74 6169 6e65  schemas_containe
 00000570: 725f 7375 6d6d 6172 795f 6c69 7374 5f69  r_summary_list_i
 00000580: 7465 6d5f 6461 7461 5a2d 636f 6d70 6f6e  tem_dataZ-compon
 00000590: 656e 7473 7363 6865 6d61 735f 636f 6e74  entsschemas_cont
 000005a0: 6169 6e65 725f 7375 6d6d 6172 795f 6c69  ainer_summary_li
 000005b0: 7374 5f69 7465 6d72 1800 0000 7218 0000  st_itemr....r...
 000005c0: 0072 1900 0000 da0f 5f70 6172 7365 5f72  .r......_parse_r
 000005d0: 6573 706f 6e73 651f 0000 0073 1800 0000  esponse....s....
 000005e0: 0003 0c01 0401 0801 0801 0401 02ff 0404  ................
-000005f0: 0c02 0401 0601 1202 722d 0000 0063 0000  ........r-...c..
+000005f0: 0c02 0401 0601 1202 722e 0000 0063 0000  ........r....c..
 00000600: 0000 0000 0000 0200 0000 0200 0000 0800  ................
 00000610: 0000 4300 0000 7322 0000 0074 0074 017c  ..C...s"...t.t.|
 00000620: 016a 0283 017c 016a 037c 016a 0474 057c  .j...|.j.|.j.t.|
 00000630: 007c 0164 018d 0264 028d 0453 0029 034e  .|.d...d...S.).N
 00000640: a902 7222 0000 0072 2300 0000 2904 7224  ..r"...r#...).r$
 00000650: 0000 0072 2b00 0000 da07 6865 6164 6572  ...r+.....header
 00000660: 73da 0670 6172 7365 6429 0672 0e00 0000  s..parsed).r....
 00000670: 7202 0000 0072 2400 0000 722b 0000 0072  r....r$...r+...r
-00000680: 2f00 0000 722d 0000 0072 2e00 0000 7218  /...r-...r....r.
+00000680: 3000 0000 722e 0000 0072 2f00 0000 7218  0...r....r/...r.
 00000690: 0000 0072 1800 0000 7219 0000 00da 0f5f  ...r....r......_
 000006a0: 6275 696c 645f 7265 7370 6f6e 7365 3300  build_response3.
 000006b0: 0000 730c 0000 0000 0302 0108 0104 0104  ..s.............
-000006c0: 010a fc72 3100 0000 2903 7222 0000 0072  ...r1...).r"...r
+000006c0: 010a fc72 3200 0000 2903 7222 0000 0072  ...r2...).r"...r
 000006d0: 1100 0000 7212 0000 0063 0100 0000 0000  ....r....c......
 000006e0: 0000 0200 0000 0500 0000 0500 0000 4b00  ..............K.
 000006f0: 0000 733c 0000 007c 03a0 0074 017c 0264  ..s<...|...t.|.d
 00000700: 018d 01a1 0101 0074 026a 037c 016a 047c  .......t.j.|.j.|
 00000710: 0064 028d 027d 017c 016a 0566 0069 007c  .d...}.|.j.f.i.|
 00000720: 03a4 018e 017d 0474 067c 017c 0464 038d  .....}.t.|.|.d..
 00000730: 0253 0029 04e1 f401 0000 636f 6e74 6169  .S.)......contai
@@ -142,24 +142,24 @@
 000008d0: 616b 6573 206c 6f6e 6765 7220 7468 616e  akes longer than
 000008e0: 2043 6c69 656e 742e 7469 6d65 6f75 742e   Client.timeout.
 000008f0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
 00000900: 2020 2020 2020 2052 6573 706f 6e73 655b         Response[
 00000910: 4c69 7374 5b27 436f 6e74 6169 6e65 7253  List['ContainerS
 00000920: 756d 6d61 7279 275d 5d0a 2020 2020 7210  ummary']].    r.
 00000930: 0000 0029 02da 0862 6173 655f 7572 6cda  ...)...base_url.
-00000940: 0974 7261 6e73 706f 7274 722e 0000 0029  .transportr....)
+00000940: 0974 7261 6e73 706f 7274 722f 0000 0029  .transportr/...)
 00000950: 07da 0675 7064 6174 6572 2100 0000 da05  ...updater!.....
 00000960: 6874 7470 7872 0b00 0000 da09 5f62 6173  httpxr......_bas
-00000970: 655f 7572 6cda 0772 6571 7565 7374 7231  e_url..requestr1
-00000980: 0000 0029 0572 3400 0000 7222 0000 0072  ...).r4...r"...r
+00000970: 655f 7572 6cda 0772 6571 7565 7374 7232  e_url..requestr2
+00000980: 0000 0029 0572 3500 0000 7222 0000 0072  ...).r5...r"...r
 00000990: 1100 0000 da06 6b77 6172 6773 7223 0000  ......kwargsr#..
 000009a0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
 000009b0: da0d 7379 6e63 5f64 6574 6169 6c65 643e  ..sync_detailed>
 000009c0: 0000 0073 1000 0000 0017 0401 0201 02ff  ...s............
-000009d0: 04ff 0406 1001 1002 723a 0000 0063 0000  ........r:...c..
+000009d0: 04ff 0406 1001 1002 723b 0000 0063 0000  ........r;...c..
 000009e0: 0000 0000 0000 0200 0000 0200 0000 0400  ................
 000009f0: 0000 4300 0000 730e 0000 0074 007c 007c  ..C...s....t.|.|
 00000a00: 0164 018d 026a 0153 0029 02e1 ea01 0000  .d...j.S.)......
 00000a10: 636f 6e74 6169 6e65 7220 6c69 7374 0a0a  container list..
 00000a20: 2020 2020 2052 6574 7572 6e73 2061 206c       Returns a l
 00000a30: 6973 7420 6f66 2063 6f6e 7461 696e 6572  ist of container
 00000a40: 2073 756d 6d61 7269 6573 2e20 466f 7220   summaries. For 
@@ -186,51 +186,51 @@
 00000b90: 7469 6f6e 3a20 4966 2074 6865 2072 6571  tion: If the req
 00000ba0: 7565 7374 2074 616b 6573 206c 6f6e 6765  uest takes longe
 00000bb0: 7220 7468 616e 2043 6c69 656e 742e 7469  r than Client.ti
 00000bc0: 6d65 6f75 742e 0a0a 2020 2020 5265 7475  meout...    Retu
 00000bd0: 726e 733a 0a20 2020 2020 2020 204c 6973  rns:.        Lis
 00000be0: 745b 2743 6f6e 7461 696e 6572 5375 6d6d  t['ContainerSumm
 00000bf0: 6172 7927 5d0a 2020 2020 a902 7222 0000  ary'].    ..r"..
-00000c00: 0072 1100 0000 2902 723a 0000 0072 3000  .r....).r:...r0.
-00000c10: 0000 723c 0000 0072 1800 0000 7218 0000  ..r<...r....r...
+00000c00: 0072 1100 0000 2902 723b 0000 0072 3100  .r....).r;...r1.
+00000c10: 0000 723d 0000 0072 1800 0000 7218 0000  ..r=...r....r...
 00000c20: 0072 1900 0000 da04 7379 6e63 6100 0000  .r......synca...
-00000c30: 7308 0000 0000 1502 0102 0102 fe72 3d00  s............r=.
+00000c30: 7308 0000 0000 1502 0102 0102 fe72 3e00  s............r>.
 00000c40: 0000 6300 0000 0000 0000 0002 0000 0004  ..c.............
 00000c50: 0000 0004 0000 00c3 0000 0073 3000 0000  ...........s0...
 00000c60: 7400 7c01 6401 8d01 7d02 7c00 a001 a100  t.|.d...}.|.....
 00000c70: 6a02 6600 6900 7c02 a401 8e01 4900 6402  j.f.i.|.....I.d.
 00000c80: 4800 7d03 7403 7c00 7c03 6403 8d02 5300  H.}.t.|.|.d...S.
-00000c90: 2904 7232 0000 0072 1000 0000 4e72 2e00  ).r2...r....Nr..
+00000c90: 2904 7233 0000 0072 1000 0000 4e72 2f00  ).r3...r....Nr/.
 00000ca0: 0000 2904 7221 0000 00da 1667 6574 5f61  ..).r!.....get_a
 00000cb0: 7379 6e63 5f68 7474 7078 5f63 6c69 656e  sync_httpx_clien
-00000cc0: 7472 3800 0000 7231 0000 0029 0472 2200  tr8...r1...).r".
-00000cd0: 0000 7211 0000 0072 3900 0000 7223 0000  ..r....r9...r#..
+00000cc0: 7472 3900 0000 7232 0000 0029 0472 2200  tr9...r2...).r".
+00000cd0: 0000 7211 0000 0072 3a00 0000 7223 0000  ..r....r:...r#..
 00000ce0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
 00000cf0: da10 6173 796e 6369 6f5f 6465 7461 696c  ..asyncio_detail
 00000d00: 6564 7c00 0000 730a 0000 0000 1502 0102  ed|...s.........
-00000d10: ff06 041a 0272 3f00 0000 6300 0000 0000  .....r?...c.....
+00000d10: ff06 041a 0272 4000 0000 6300 0000 0000  .....r@...c.....
 00000d20: 0000 0002 0000 0002 0000 0004 0000 00c3  ................
 00000d30: 0000 0073 1400 0000 7400 7c00 7c01 6401  ...s....t.|.|.d.
-00000d40: 8d02 4900 6402 4800 6a01 5300 2903 723b  ..I.d.H.j.S.).r;
-00000d50: 0000 0072 3c00 0000 4e29 0272 3f00 0000  ...r<...N).r?...
-00000d60: 7230 0000 0072 3c00 0000 7218 0000 0072  r0...r<...r....r
+00000d40: 8d02 4900 6402 4800 6a01 5300 2903 723c  ..I.d.H.j.S.).r<
+00000d50: 0000 0072 3d00 0000 4e29 0272 4000 0000  ...r=...N).r@...
+00000d60: 7231 0000 0072 3d00 0000 7218 0000 0072  r1...r=...r....r
 00000d70: 1800 0000 7219 0000 00da 0761 7379 6e63  ....r......async
 00000d80: 696f 9a00 0000 730a 0000 0000 1602 0102  io....s.........
-00000d90: 0102 fe0a ff72 4000 0000 291d da04 6874  .....r@...)...ht
+00000d90: 0102 fe0a ff72 4100 0000 291d da04 6874  .....rA...)...ht
 00000da0: 7470 7202 0000 00da 0674 7970 696e 6772  tpr......typingr
 00000db0: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
-00000dc0: 0000 0072 0700 0000 7236 0000 00da 0072  ...r....r6.....r
+00000dc0: 0000 0072 0700 0000 7237 0000 00da 0072  ...r....r7.....r
 00000dd0: 0900 0000 7222 0000 0072 0a00 0000 720b  ....r"...r....r.
 00000de0: 0000 005a 186d 6f64 656c 732e 636f 6e74  ...Z.models.cont
 00000df0: 6169 6e65 725f 7375 6d6d 6172 7972 0c00  ainer_summaryr..
 00000e00: 0000 da05 7479 7065 7372 0d00 0000 720e  ....typesr....r.
 00000e10: 0000 0072 0f00 0000 da04 626f 6f6c da03  ...r......bool..
-00000e20: 7374 7272 2100 0000 722d 0000 0072 3100  strr!...r-...r1.
-00000e30: 0000 723a 0000 0072 3d00 0000 723f 0000  ..r:...r=...r?..
-00000e40: 0072 4000 0000 7218 0000 0072 1800 0000  .r@...r....r....
+00000e20: 7374 7272 2100 0000 722e 0000 0072 3200  strr!...r....r2.
+00000e30: 0000 723b 0000 0072 3e00 0000 7240 0000  ..r;...r>...r@..
+00000e40: 0072 4100 0000 7218 0000 0072 1800 0000  .rA...r....r....
 00000e50: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
 00000e60: 756c 653e 0100 0000 7352 0000 000c 011c  ule>....sR......
 00000e70: 0208 020c 0110 010c 0114 0502 fe04 020c  ................
 00000e80: 010a fd0c 140e 010a fe0c 150e 010a fe0c  ................
 00000e90: 0f02 fc04 030a 010c 020a fa0c 2602 fd04  ............&...
 00000ea0: 020a 010c 010a fc0c 1e02 fd04 020a 010c  ................
 00000eb0: 010a fc0c 2102 fd04 020a 010c 010a fc    ....!..........
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_prune.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_prune.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:40 2024 UTC, .py size: 3782 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 20b1 1d66 c60e 0000  a....... ..f....
+00000000: 610d 0d0a 0000 0000 47fe 3166 c60e 0000  a.......G.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 7a01 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 5a09 6404 6405 6c0a 6d0b 5a0b 0100 6404  Z.d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6404  d.l.m.Z.m.Z...d.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_remove.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_remove.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:40 2024 UTC, .py size: 4610 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 20b1 1d66 0212 0000  a....... ..f....
+00000000: 610d 0d0a 0000 0000 47fe 3166 0212 0000  a.......G.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_stop.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_stop.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:40 2024 UTC, .py size: 4728 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 20b1 1d66 7812 0000  a....... ..fx...
+00000000: 610d 0d0a 0000 0000 47fe 3166 7812 0000  a.......G.1fx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/container_update.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/container_update.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:40 2024 UTC, .py size: 6540 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 20b1 1d66 8c19 0000  a....... ..f....
+00000000: 610d 0d0a 0000 0000 47fe 3166 8c19 0000  a.......G.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 8601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/exec_create.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/exec_create.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:40 2024 UTC, .py size: 5435 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 20b1 1d66 3b15 0000  a....... ..f;...
+00000000: 610d 0d0a 0000 0000 47fe 3166 3b15 0000  a.......G.1f;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7c01 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_inspect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_inspect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:41 2024 UTC, .py size: 4283 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 21b1 1d66 bb10 0000  a.......!..f....
+00000000: 610d 0d0a 0000 0000 48fe 3166 bb10 0000  a.......H.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_list.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_list.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:41 2024 UTC, .py size: 4080 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 21b1 1d66 f00f 0000  a.......!..f....
+00000000: 610d 0d0a 0000 0000 48fe 3166 f00f 0000  a.......H.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4601 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 5a08 6404  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6404 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6404 6407 6c0e  m.Z.m.Z...d.d.l.
@@ -48,44 +48,44 @@
 000002f0: 016a 026b 0272 3a67 007d 027c 01a0 03a1  .j.k.r:g.}.|....
 00000300: 007d 037c 0344 005d 187d 0474 04a0 057c  .}.|.D.].}.t...|
 00000310: 04a1 017d 057c 02a0 067c 05a1 0101 0071  ...}.|...|.....q
 00000320: 1c7c 0253 007c 006a 0772 5274 08a0 097c  .|.S.|.j.rRt...|
 00000330: 016a 007c 016a 0aa1 0282 016e 0464 0053  .j.|.j.....n.d.S
 00000340: 0064 0053 0029 014e 290b da0b 7374 6174  .d.S.).N)...stat
 00000350: 7573 5f63 6f64 6572 0200 0000 da02 4f4b  us_coder......OK
-00000360: da04 6a73 6f6e 720c 0000 00da 0966 726f  ..jsonr......fro
+00000360: da04 6a73 6f6e 720c 0000 005a 0966 726f  ..jsonr....Z.fro
 00000370: 6d5f 6469 6374 da06 6170 7065 6e64 da1a  m_dict..append..
 00000380: 7261 6973 655f 6f6e 5f75 6e65 7870 6563  raise_on_unexpec
-00000390: 7465 645f 7374 6174 7573 7209 0000 00da  ted_statusr.....
+00000390: 7465 645f 7374 6174 7573 7209 0000 005a  ted_statusr....Z
 000003a0: 1055 6e65 7870 6563 7465 6453 7461 7475  .UnexpectedStatu
 000003b0: 73da 0763 6f6e 7465 6e74 2906 7215 0000  s..content).r...
-000003c0: 0072 1600 0000 da0c 7265 7370 6f6e 7365  .r......response
-000003d0: 5f32 3030 da0d 5f72 6573 706f 6e73 655f  _200.._response_
+000003c0: 0072 1600 0000 5a0c 7265 7370 6f6e 7365  .r....Z.response
+000003d0: 5f32 3030 5a0d 5f72 6573 706f 6e73 655f  _200Z._response_
 000003e0: 3230 305a 2663 6f6d 706f 6e65 6e74 7373  200Z&componentss
 000003f0: 6368 656d 6173 5f69 6d61 6765 5f6c 6973  chemas_image_lis
 00000400: 745f 6974 656d 5f64 6174 615a 2163 6f6d  t_item_dataZ!com
 00000410: 706f 6e65 6e74 7373 6368 656d 6173 5f69  ponentsschemas_i
 00000420: 6d61 6765 5f6c 6973 745f 6974 656d 7212  mage_list_itemr.
 00000430: 0000 0072 1200 0000 7213 0000 00da 0f5f  ...r....r......_
 00000440: 7061 7273 655f 7265 7370 6f6e 7365 1600  parse_response..
 00000450: 0000 7318 0000 0000 030c 0104 0108 0108  ..s.............
 00000460: 0104 0102 ff04 040c 0204 0106 0112 0272  ...............r
-00000470: 2100 0000 6300 0000 0000 0000 0002 0000  !...c...........
+00000470: 1d00 0000 6300 0000 0000 0000 0002 0000  ....c...........
 00000480: 0002 0000 0008 0000 0043 0000 0073 2200  .........C...s".
 00000490: 0000 7400 7401 7c01 6a02 8301 7c01 6a03  ..t.t.|.j...|.j.
 000004a0: 7c01 6a04 7405 7c00 7c01 6401 8d02 6402  |.j.t.|.|.d...d.
 000004b0: 8d04 5300 2903 4ea9 0272 1500 0000 7216  ..S.).N..r....r.
-000004c0: 0000 0029 0472 1700 0000 721e 0000 00da  ...).r....r.....
+000004c0: 0000 0029 0472 1700 0000 721c 0000 00da  ...).r....r.....
 000004d0: 0768 6561 6465 7273 da06 7061 7273 6564  .headers..parsed
 000004e0: 2906 720d 0000 0072 0200 0000 7217 0000  ).r....r....r...
-000004f0: 0072 1e00 0000 7223 0000 0072 2100 0000  .r....r#...r!...
-00000500: 7222 0000 0072 1200 0000 7212 0000 0072  r"...r....r....r
+000004f0: 0072 1c00 0000 721f 0000 0072 1d00 0000  .r....r....r....
+00000500: 721e 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
 00000510: 1300 0000 da0f 5f62 7569 6c64 5f72 6573  ......_build_res
 00000520: 706f 6e73 652a 0000 0073 0c00 0000 0003  ponse*...s......
-00000530: 0201 0801 0401 0401 0afc 7225 0000 0029  ..........r%...)
+00000530: 0201 0801 0401 0401 0afc 7221 0000 0029  ..........r!...)
 00000540: 0272 1500 0000 720e 0000 0063 0100 0000  .r....r....c....
 00000550: 0000 0000 0100 0000 0400 0000 0400 0000  ................
 00000560: 4b00 0000 7338 0000 007c 02a0 0074 0183  K...s8...|...t..
 00000570: 00a1 0101 0074 026a 037c 016a 047c 0064  .....t.j.|.j.|.d
 00000580: 018d 027d 017c 016a 0566 0069 007c 02a4  ...}.|.j.f.i.|..
 00000590: 018e 017d 0374 067c 017c 0364 028d 0253  ...}.t.|.|.d...S
 000005a0: 0029 03e1 a701 0000 696d 6167 6520 6c69  .)......image li
@@ -112,23 +112,23 @@
 000006f0: 6865 2072 6571 7565 7374 2074 616b 6573  he request takes
 00000700: 206c 6f6e 6765 7220 7468 616e 2043 6c69   longer than Cli
 00000710: 656e 742e 7469 6d65 6f75 742e 0a0a 2020  ent.timeout...  
 00000720: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
 00000730: 2020 2052 6573 706f 6e73 655b 4c69 7374     Response[List
 00000740: 5b27 496d 6167 6527 5d5d 0a20 2020 2029  ['Image']].    )
 00000750: 02da 0862 6173 655f 7572 6cda 0974 7261  ...base_url..tra
-00000760: 6e73 706f 7274 7222 0000 0029 07da 0675  nsportr"...)...u
+00000760: 6e73 706f 7274 721e 0000 0029 07da 0675  nsportr....)...u
 00000770: 7064 6174 6572 1400 0000 da05 6874 7470  pdater......http
 00000780: 7872 0b00 0000 da09 5f62 6173 655f 7572  xr......_base_ur
-00000790: 6cda 0772 6571 7565 7374 7225 0000 0029  l..requestr%...)
-000007a0: 0472 2800 0000 7215 0000 00da 066b 7761  .r(...r......kwa
+00000790: 6cda 0772 6571 7565 7374 7221 0000 0029  l..requestr!...)
+000007a0: 0472 2400 0000 7215 0000 00da 066b 7761  .r$...r......kwa
 000007b0: 7267 7372 1600 0000 7212 0000 0072 1200  rgsr....r....r..
 000007c0: 0000 7213 0000 00da 0d73 796e 635f 6465  ..r......sync_de
 000007d0: 7461 696c 6564 3500 0000 7308 0000 0000  tailed5...s.....
-000007e0: 100c 0210 0110 0272 2e00 0000 6300 0000  .......r....c...
+000007e0: 100c 0210 0110 0272 2a00 0000 6300 0000  .......r*...c...
 000007f0: 0000 0000 0001 0000 0001 0000 0003 0000  ................
 00000800: 0043 0000 0073 0c00 0000 7400 7c00 6401  .C...s....t.|.d.
 00000810: 8d01 6a01 5300 2902 e19d 0100 0069 6d61  ..j.S.)......ima
 00000820: 6765 206c 6973 740a 0a20 2020 2020 4c69  ge list..     Li
 00000830: 7374 2074 6865 2069 6d61 6765 732e 2055  st the images. U
 00000840: 7365 2074 6865 205b 696d 6167 6520 696e  se the [image in
 00000850: 7370 6563 745d 2823 6f70 6572 6174 696f  spect](#operatio
@@ -150,46 +150,46 @@
 00000950: 696d 656f 7574 4578 6365 7074 696f 6e3a  imeoutException:
 00000960: 2049 6620 7468 6520 7265 7175 6573 7420   If the request 
 00000970: 7461 6b65 7320 6c6f 6e67 6572 2074 6861  takes longer tha
 00000980: 6e20 436c 6965 6e74 2e74 696d 656f 7574  n Client.timeout
 00000990: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
 000009a0: 2020 2020 2020 2020 4c69 7374 5b27 496d          List['Im
 000009b0: 6167 6527 5d0a 2020 2020 a901 7215 0000  age'].    ..r...
-000009c0: 0029 0272 2e00 0000 7224 0000 0072 3000  .).r....r$...r0.
+000009c0: 0029 0272 2a00 0000 7220 0000 0072 2c00  .).r*...r ...r,.
 000009d0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
 000009e0: 00da 0473 796e 634d 0000 0073 0600 0000  ...syncM...s....
-000009f0: 0011 0201 02ff 7231 0000 0063 0000 0000  ......r1...c....
+000009f0: 0011 0201 02ff 722d 0000 0063 0000 0000  ......r-...c....
 00000a00: 0000 0000 0100 0000 0300 0000 0400 0000  ................
 00000a10: c300 0000 732c 0000 0074 0083 007d 017c  ....s,...t...}.|
 00000a20: 00a0 01a1 006a 0266 0069 007c 01a4 018e  .....j.f.i.|....
 00000a30: 0149 0064 0148 007d 0274 037c 007c 0264  .I.d.H.}.t.|.|.d
-00000a40: 028d 0253 0029 0372 2600 0000 4e72 2200  ...S.).r&...Nr".
+00000a40: 028d 0253 0029 0372 2200 0000 4e72 1e00  ...S.).r"...Nr..
 00000a50: 0000 2904 7214 0000 00da 1667 6574 5f61  ..).r......get_a
 00000a60: 7379 6e63 5f68 7474 7078 5f63 6c69 656e  sync_httpx_clien
-00000a70: 7472 2c00 0000 7225 0000 0029 0372 1500  tr,...r%...).r..
-00000a80: 0000 722d 0000 0072 1600 0000 7212 0000  ..r-...r....r...
+00000a70: 7472 2800 0000 7221 0000 0029 0372 1500  tr(...r!...).r..
+00000a80: 0000 7229 0000 0072 1600 0000 7212 0000  ..r)...r....r...
 00000a90: 0072 1200 0000 7213 0000 00da 1061 7379  .r....r......asy
 00000aa0: 6e63 696f 5f64 6574 6169 6c65 6463 0000  ncio_detailedc..
-00000ab0: 0073 0600 0000 0011 0602 1a02 7233 0000  .s..........r3..
+00000ab0: 0073 0600 0000 0011 0602 1a02 722f 0000  .s..........r/..
 00000ac0: 0063 0000 0000 0000 0000 0100 0000 0100  .c..............
 00000ad0: 0000 0300 0000 c300 0000 7312 0000 0074  ..........s....t
 00000ae0: 007c 0064 018d 0149 0064 0248 006a 0153  .|.d...I.d.H.j.S
-00000af0: 0029 0372 2f00 0000 7230 0000 004e 2902  .).r/...r0...N).
-00000b00: 7233 0000 0072 2400 0000 7230 0000 0072  r3...r$...r0...r
+00000af0: 0029 0372 2b00 0000 722c 0000 004e 2902  .).r+...r,...N).
+00000b00: 722f 0000 0072 2000 0000 722c 0000 0072  r/...r ...r,...r
 00000b10: 1200 0000 7212 0000 0072 1300 0000 da07  ....r....r......
 00000b20: 6173 796e 6369 6f7b 0000 0073 0800 0000  asyncio{...s....
-00000b30: 0012 0201 02ff 0aff 7234 0000 0029 1ada  ........r4...)..
+00000b30: 0012 0201 02ff 0aff 7230 0000 0029 1ada  ........r0...)..
 00000b40: 0468 7474 7072 0200 0000 da06 7479 7069  .httpr......typi
 00000b50: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
-00000b60: 0072 0600 0000 7207 0000 0072 2a00 0000  .r....r....r*...
+00000b60: 0072 0600 0000 7207 0000 0072 2600 0000  .r....r....r&...
 00000b70: da00 7209 0000 0072 1500 0000 720a 0000  ..r....r....r...
 00000b80: 0072 0b00 0000 5a0c 6d6f 6465 6c73 2e69  .r....Z.models.i
 00000b90: 6d61 6765 720c 0000 00da 0574 7970 6573  mager......types
 00000ba0: 720d 0000 00da 0373 7472 7214 0000 0072  r......strr....r
-00000bb0: 2100 0000 7225 0000 0072 2e00 0000 7231  !...r%...r....r1
-00000bc0: 0000 0072 3300 0000 7234 0000 0072 1200  ...r3...r4...r..
+00000bb0: 1d00 0000 7221 0000 0072 2a00 0000 722d  ....r!...r*...r-
+00000bc0: 0000 0072 2f00 0000 7230 0000 0072 1200  ...r/...r0...r..
 00000bd0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
 00000be0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
 00000bf0: 3200 0000 0c01 1c02 0802 0c01 1001 0c01  2...............
 00000c00: 0c03 160b 0e01 0afe 0c15 0e01 0afe 0c0c  ................
 00000c10: 0a01 0afe 0c1a 0a01 0afd 0c18 0a01 0afd  ................
 00000c20: 0c1a 0a01 0afd                           ......
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_prune.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_prune.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:41 2024 UTC, .py size: 3920 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 21b1 1d66 500f 0000  a.......!..fP...
+00000000: 610d 0d0a 0000 0000 48fe 3166 500f 0000  a.......H.1fP...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4c01 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 5a09 6404 6405 6c0a 6d0b 5a0b 0100 6404  Z.d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6404  d.l.m.Z.m.Z...d.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_remove.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_remove.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:41 2024 UTC, .py size: 4760 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 21b1 1d66 9812 0000  a.......!..f....
+00000000: 610d 0d0a 0000 0000 48fe 3166 9812 0000  a.......H.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -65,33 +65,33 @@
 00000400: 554e 4472 0b00 0000 da15 494e 5445 524e  UNDr......INTERN
 00000410: 414c 5f53 4552 5645 525f 4552 524f 52da  AL_SERVER_ERROR.
 00000420: 1a72 6169 7365 5f6f 6e5f 756e 6578 7065  .raise_on_unexpe
 00000430: 6374 6564 5f73 7461 7475 7372 0800 0000  cted_statusr....
 00000440: da10 556e 6578 7065 6374 6564 5374 6174  ..UnexpectedStat
 00000450: 7573 da07 636f 6e74 656e 7429 0572 1800  us..content).r..
 00000460: 0000 7219 0000 00da 0c72 6573 706f 6e73  ..r......respons
-00000470: 655f 3230 30da 0c72 6573 706f 6e73 655f  e_200..response_
-00000480: 3430 34da 0c72 6573 706f 6e73 655f 3530  404..response_50
+00000470: 655f 3230 305a 0c72 6573 706f 6e73 655f  e_200Z.response_
+00000480: 3430 345a 0c72 6573 706f 6e73 655f 3530  404Z.response_50
 00000490: 3072 1500 0000 7215 0000 0072 1600 0000  0r....r....r....
 000004a0: da0f 5f70 6172 7365 5f72 6573 706f 6e73  .._parse_respons
 000004b0: 651b 0000 0073 1800 0000 0003 0c01 0e02  e....s..........
 000004c0: 0401 0c01 0e02 0401 0c01 0e02 0401 0601  ................
-000004d0: 1202 7226 0000 0063 0000 0000 0000 0000  ..r&...c........
+000004d0: 1202 7224 0000 0063 0000 0000 0000 0000  ..r$...c........
 000004e0: 0200 0000 0200 0000 0800 0000 4300 0000  ............C...
 000004f0: 7322 0000 0074 0074 017c 016a 0283 017c  s"...t.t.|.j...|
 00000500: 016a 037c 016a 0474 057c 007c 0164 018d  .j.|.j.t.|.|.d..
 00000510: 0264 028d 0453 0029 034e a902 7218 0000  .d...S.).N..r...
 00000520: 0072 1900 0000 2904 721a 0000 0072 2200  .r....).r....r".
 00000530: 0000 da07 6865 6164 6572 73da 0670 6172  ....headers..par
 00000540: 7365 6429 0672 0d00 0000 7202 0000 0072  sed).r....r....r
-00000550: 1a00 0000 7222 0000 0072 2800 0000 7226  ....r"...r(...r&
-00000560: 0000 0072 2700 0000 7215 0000 0072 1500  ...r'...r....r..
+00000550: 1a00 0000 7222 0000 0072 2600 0000 7224  ....r"...r&...r$
+00000560: 0000 0072 2500 0000 7215 0000 0072 1500  ...r%...r....r..
 00000570: 0000 7216 0000 00da 0f5f 6275 696c 645f  ..r......_build_
 00000580: 7265 7370 6f6e 7365 3000 0000 730c 0000  response0...s...
-00000590: 0000 0302 0108 0104 0104 010a fc72 2a00  .............r*.
+00000590: 0000 0302 0108 0104 0104 010a fc72 2800  .............r(.
 000005a0: 0000 2903 720e 0000 0072 1800 0000 720f  ..).r....r....r.
 000005b0: 0000 0063 0200 0000 0000 0000 0100 0000  ...c............
 000005c0: 0500 0000 0500 0000 4b00 0000 733c 0000  ........K...s<..
 000005d0: 007c 03a0 0074 017c 0164 018d 01a1 0101  .|...t.|.d......
 000005e0: 0074 026a 037c 026a 047c 0064 028d 027d  .t.j.|.j.|.d...}
 000005f0: 027c 026a 0566 0069 007c 03a4 018e 017d  .|.j.f.i.|.....}
 00000600: 0474 067c 027c 0464 038d 0253 0029 04e1  .t.|.|.d...S.)..
@@ -122,24 +122,24 @@
 00000790: 7468 616e 2043 6c69 656e 742e 7469 6d65  than Client.time
 000007a0: 6f75 742e 0a0a 2020 2020 5265 7475 726e  out...    Return
 000007b0: 733a 0a20 2020 2020 2020 2052 6573 706f  s:.        Respo
 000007c0: 6e73 655b 556e 696f 6e5b 4572 726f 7252  nse[Union[ErrorR
 000007d0: 6573 706f 6e73 652c 2049 6452 6573 706f  esponse, IdRespo
 000007e0: 6e73 655d 5d0a 2020 2020 7211 0000 0029  nse]].    r....)
 000007f0: 02da 0862 6173 655f 7572 6cda 0974 7261  ...base_url..tra
-00000800: 6e73 706f 7274 7227 0000 0029 07da 0675  nsportr'...)...u
+00000800: 6e73 706f 7274 7225 0000 0029 07da 0675  nsportr%...)...u
 00000810: 7064 6174 6572 1700 0000 da05 6874 7470  pdater......http
 00000820: 7872 0a00 0000 da09 5f62 6173 655f 7572  xr......_base_ur
-00000830: 6cda 0772 6571 7565 7374 722a 0000 0029  l..requestr*...)
-00000840: 0572 2d00 0000 720e 0000 0072 1800 0000  .r-...r....r....
+00000830: 6cda 0772 6571 7565 7374 7228 0000 0029  l..requestr(...)
+00000840: 0572 2b00 0000 720e 0000 0072 1800 0000  .r+...r....r....
 00000850: da06 6b77 6172 6773 7219 0000 0072 1500  ..kwargsr....r..
 00000860: 0000 7215 0000 0072 1600 0000 da0d 7379  ..r....r......sy
 00000870: 6e63 5f64 6574 6169 6c65 643b 0000 0073  nc_detailed;...s
 00000880: 1000 0000 0015 0401 0201 02ff 04ff 0406  ................
-00000890: 1001 1002 7233 0000 0063 0100 0000 0000  ....r3...c......
+00000890: 1001 1002 7231 0000 0063 0100 0000 0000  ....r1...c......
 000008a0: 0000 0100 0000 0200 0000 0400 0000 4300  ..............C.
 000008b0: 0000 730e 0000 0074 007c 007c 0164 018d  ..s....t.|.|.d..
 000008c0: 026a 0153 0029 02e1 cc01 0000 696d 6167  .j.S.)......imag
 000008d0: 6520 7265 6d6f 7665 0a0a 2020 2020 2052  e remove..     R
 000008e0: 656d 6f76 6520 616e 2069 6d61 6765 2e0a  emove an image..
 000008f0: 0a20 2020 2049 6d61 6765 7320 6361 6e27  .    Images can'
 00000900: 7420 6265 2072 656d 6f76 6564 2069 6620  t be removed if 
@@ -164,50 +164,50 @@
 00000a30: 6865 2072 6571 7565 7374 2074 616b 6573  he request takes
 00000a40: 206c 6f6e 6765 7220 7468 616e 2043 6c69   longer than Cli
 00000a50: 656e 742e 7469 6d65 6f75 742e 0a0a 2020  ent.timeout...  
 00000a60: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
 00000a70: 2020 2055 6e69 6f6e 5b45 7272 6f72 5265     Union[ErrorRe
 00000a80: 7370 6f6e 7365 2c20 4964 5265 7370 6f6e  sponse, IdRespon
 00000a90: 7365 5d0a 2020 2020 a902 720e 0000 0072  se].    ..r....r
-00000aa0: 1800 0000 2902 7233 0000 0072 2900 0000  ....).r3...r)...
-00000ab0: 7235 0000 0072 1500 0000 7215 0000 0072  r5...r....r....r
+00000aa0: 1800 0000 2902 7231 0000 0072 2700 0000  ....).r1...r'...
+00000ab0: 7233 0000 0072 1500 0000 7215 0000 0072  r3...r....r....r
 00000ac0: 1600 0000 da04 7379 6e63 5c00 0000 7308  ......sync\...s.
-00000ad0: 0000 0000 1702 0102 0102 fe72 3600 0000  ...........r6...
+00000ad0: 0000 0000 1702 0102 0102 fe72 3400 0000  ...........r4...
 00000ae0: 6301 0000 0000 0000 0001 0000 0004 0000  c...............
 00000af0: 0004 0000 00c3 0000 0073 3000 0000 7400  .........s0...t.
 00000b00: 7c00 6401 8d01 7d02 7c01 a001 a100 6a02  |.d...}.|.....j.
 00000b10: 6600 6900 7c02 a401 8e01 4900 6402 4800  f.i.|.....I.d.H.
 00000b20: 7d03 7403 7c01 7c03 6403 8d02 5300 2904  }.t.|.|.d...S.).
-00000b30: 722b 0000 0072 1100 0000 4e72 2700 0000  r+...r....Nr'...
+00000b30: 7229 0000 0072 1100 0000 4e72 2500 0000  r)...r....Nr%...
 00000b40: 2904 7217 0000 00da 1667 6574 5f61 7379  ).r......get_asy
 00000b50: 6e63 5f68 7474 7078 5f63 6c69 656e 7472  nc_httpx_clientr
-00000b60: 3100 0000 722a 0000 0029 0472 0e00 0000  1...r*...).r....
-00000b70: 7218 0000 0072 3200 0000 7219 0000 0072  r....r2...r....r
+00000b60: 2f00 0000 7228 0000 0029 0472 0e00 0000  /...r(...).r....
+00000b70: 7218 0000 0072 3000 0000 7219 0000 0072  r....r0...r....r
 00000b80: 1500 0000 7215 0000 0072 1600 0000 da10  ....r....r......
 00000b90: 6173 796e 6369 6f5f 6465 7461 696c 6564  asyncio_detailed
 00000ba0: 7900 0000 730a 0000 0000 1702 0102 ff06  y...s...........
-00000bb0: 041a 0272 3800 0000 6301 0000 0000 0000  ...r8...c.......
+00000bb0: 041a 0272 3600 0000 6301 0000 0000 0000  ...r6...c.......
 00000bc0: 0001 0000 0002 0000 0004 0000 00c3 0000  ................
 00000bd0: 0073 1400 0000 7400 7c00 7c01 6401 8d02  .s....t.|.|.d...
-00000be0: 4900 6402 4800 6a01 5300 2903 7234 0000  I.d.H.j.S.).r4..
-00000bf0: 0072 3500 0000 4e29 0272 3800 0000 7229  .r5...N).r8...r)
-00000c00: 0000 0072 3500 0000 7215 0000 0072 1500  ...r5...r....r..
+00000be0: 4900 6402 4800 6a01 5300 2903 7232 0000  I.d.H.j.S.).r2..
+00000bf0: 0072 3300 0000 4e29 0272 3600 0000 7227  .r3...N).r6...r'
+00000c00: 0000 0072 3300 0000 7215 0000 0072 1500  ...r3...r....r..
 00000c10: 0000 7216 0000 00da 0761 7379 6e63 696f  ..r......asyncio
 00000c20: 9900 0000 730a 0000 0000 1802 0102 0102  ....s...........
-00000c30: fe0a ff72 3900 0000 291b da04 6874 7470  ...r9...)...http
+00000c30: fe0a ff72 3700 0000 291b da04 6874 7470  ...r7...)...http
 00000c40: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
 00000c50: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
-00000c60: 0072 2f00 0000 da00 7208 0000 0072 1800  .r/.....r....r..
+00000c60: 0072 2d00 0000 da00 7208 0000 0072 1800  .r-.....r....r..
 00000c70: 0000 7209 0000 0072 0a00 0000 5a15 6d6f  ..r....r....Z.mo
 00000c80: 6465 6c73 2e65 7272 6f72 5f72 6573 706f  dels.error_respo
 00000c90: 6e73 6572 0b00 0000 5a12 6d6f 6465 6c73  nser....Z.models
 00000ca0: 2e69 645f 7265 7370 6f6e 7365 720c 0000  .id_responser...
 00000cb0: 00da 0574 7970 6573 720d 0000 00da 0373  ...typesr......s
-00000cc0: 7472 7217 0000 0072 2600 0000 722a 0000  trr....r&...r*..
-00000cd0: 0072 3300 0000 7236 0000 0072 3800 0000  .r3...r6...r8...
-00000ce0: 7239 0000 0072 1500 0000 7215 0000 0072  r9...r....r....r
+00000cc0: 7472 7217 0000 0072 2400 0000 7228 0000  trr....r$...r(..
+00000cd0: 0072 3100 0000 7234 0000 0072 3600 0000  .r1...r4...r6...
+00000ce0: 7237 0000 0072 1500 0000 7215 0000 0072  r7...r....r....r
 00000cf0: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
 00000d00: 6c65 3e01 0000 0073 3e00 0000 0c01 1802  le>....s>.......
 00000d10: 0802 0c01 1001 0c01 0c01 0c04 0201 0afe  ................
 00000d20: 0c0f 0e01 0efe 0c16 0e01 0efe 0c0c 0c01  ................
 00000d30: 0efe 0c22 0202 0a01 0efc 0c1e 0202 0a01  ..."............
 00000d40: 0efc 0c21 0202 0a01 0efc                 ...!......
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/image_tag.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/image_tag.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 4866 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 0213 0000  a......."..f....
+00000000: 610d 0d0a 0000 0000 48fe 3166 0213 0000  a.......H.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 7e01 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_connect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_connect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 4953 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 5913 0000  a......."..fY...
+00000000: 610d 0d0a 0000 0000 48fe 3166 5913 0000  a.......H.1fY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7401 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 5a08 6404  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6404 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6404 6407 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_create.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_create.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 4643 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 2312 0000  a......."..f#...
+00000000: 610d 0d0a 0000 0000 48fe 3166 2312 0000  a.......H.1f#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7c01 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_disconnect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_disconnect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 5085 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 dd13 0000  a......."..f....
+00000000: 610d 0d0a 0000 0000 48fe 3166 dd13 0000  a.......H.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 7201 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 5a08 6404  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6404 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6404 6407 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_inspect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_inspect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 4527 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 af11 0000  a......."..f....
+00000000: 610d 0d0a 0000 0000 49fe 3166 af11 0000  a.......I.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_list.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_list.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 4601 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 f911 0000  a......."..f....
+00000000: 610d 0d0a 0000 0000 49fe 3166 f911 0000  a.......I.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 8201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 5a08 6404  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6404 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6404 6407 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_prune.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_prune.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 3876 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 240f 0000  a......."..f$...
+00000000: 610d 0d0a 0000 0000 49fe 3166 240f 0000  a.......I.1f$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 7a01 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 5a09 6404 6405 6c0a 6d0b 5a0b 0100 6404  Z.d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6404  d.l.m.Z.m.Z...d.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/network_remove.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/network_remove.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 4578 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 e211 0000  a......."..f....
+00000000: 610d 0d0a 0000 0000 49fe 3166 e211 0000  a.......I.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_create.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_create.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 4490 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 8a11 0000  a......."..f....
+00000000: 610d 0d0a 0000 0000 49fe 3166 8a11 0000  a.......I.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7c01 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_inspect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_inspect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 4533 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 b511 0000  a......."..f....
+00000000: 610d 0d0a 0000 0000 49fe 3166 b511 0000  a.......I.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_list.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_list.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:42 2024 UTC, .py size: 3630 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 22b1 1d66 2e0e 0000  a......."..f....
+00000000: 610d 0d0a 0000 0000 49fe 3166 2e0e 0000  a.......I.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4601 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 5a08 6404  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6404 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6404 6407 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_prune.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_prune.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:43 2024 UTC, .py size: 3911 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 23b1 1d66 470f 0000  a.......#..fG...
+00000000: 610d 0d0a 0000 0000 49fe 3166 470f 0000  a.......I.1fG...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 7a01 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 5a09 6404 6405 6c0a 6d0b 5a0b 0100 6404  Z.d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6404  d.l.m.Z.m.Z...d.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/__pycache__/volume_remove.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/api/default/__pycache__/volume_remove.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:43 2024 UTC, .py size: 4677 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 23b1 1d66 4512 0000  a.......#..fE...
+00000000: 610d 0d0a 0000 0000 49fe 3166 4512 0000  a.......I.1fE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6404 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6404 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6404 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/container_create.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/container_create.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/container_inspect.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/container_inspect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/container_list.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/container_list.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/container_prune.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/container_prune.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/container_remove.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/container_remove.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/container_stop.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/container_stop.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/container_update.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/container_update.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/exec_create.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/exec_create.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/exec_start_web_socket.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/exec_start_web_socket.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/exec_stop.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/exec_stop.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/image_build.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/image_build.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/image_create.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/image_create.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/image_inspect.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/image_inspect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/image_list.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/image_list.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/image_prune.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/image_prune.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/image_remove.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/image_remove.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/image_tag.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/image_tag.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/network_connect.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/network_connect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/network_create.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/network_create.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/network_disconnect.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/network_disconnect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/network_inspect.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/network_inspect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/network_list.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/network_list.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/network_prune.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/network_prune.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/network_remove.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/network_remove.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/volume_create.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/volume_create.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/volume_inspect.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/volume_inspect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/volume_list.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/volume_list.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/volume_prune.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/volume_prune.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/api/default/volume_remove.py` & `kleene_cli-0.1.0rc3/klee/client/api/default/volume_remove.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/client.py` & `kleene_cli-0.1.0rc3/klee/client/client.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__init__.py` & `kleene_cli-0.1.0rc3/klee/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/__init__.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:32 2024 UTC, .py size: 2739 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 18b1 1d66 b30a 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 40fe 3166 b30a 0000  a.......@.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 c801 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
@@ -88,15 +88,15 @@
 00000570: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
 00000580: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
 00000590: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
 000005a0: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
 000005b0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
 000005c0: 0072 2500 0000 7226 0000 004e 294c da07  .r%...r&...N)L..
 000005d0: 5f5f 646f 635f 5fda 0963 6f6e 7461 696e  __doc__..contain
-000005e0: 6572 7202 0000 00da 1063 6f6e 7461 696e  err......contain
+000005e0: 6572 7202 0000 005a 1063 6f6e 7461 696e  err....Z.contain
 000005f0: 6572 5f63 6f6e 6669 6772 0300 0000 5a1f  er_configr....Z.
 00000600: 636f 6e74 6169 6e65 725f 636f 6e66 6967  container_config
 00000610: 5f6e 6574 776f 726b 5f64 7269 7665 7272  _network_driverr
 00000620: 0400 0000 5a1f 636f 6e74 6169 6e65 725f  ....Z.container_
 00000630: 636f 6e66 6967 5f72 6573 7461 7274 5f70  config_restart_p
 00000640: 6f6c 6963 7972 0500 0000 5a11 636f 6e74  olicyr....Z.cont
 00000650: 6169 6e65 725f 696e 7370 6563 7472 0600  ainer_inspectr..
@@ -105,15 +105,15 @@
 00000680: 005a 1863 6f6e 7461 696e 6572 5f72 6573  .Z.container_res
 00000690: 7461 7274 5f70 6f6c 6963 7972 0800 0000  tart_policyr....
 000006a0: 5a11 636f 6e74 6169 6e65 725f 7375 6d6d  Z.container_summ
 000006b0: 6172 7972 0900 0000 5a09 656e 645f 706f  aryr....Z.end_po
 000006c0: 696e 7472 0a00 0000 5a10 656e 645f 706f  intr....Z.end_po
 000006d0: 696e 745f 636f 6e66 6967 720b 0000 005a  int_configr....Z
 000006e0: 0e65 7272 6f72 5f72 6573 706f 6e73 6572  .error_responser
-000006f0: 0c00 0000 da0b 6578 6563 5f63 6f6e 6669  ......exec_confi
+000006f0: 0c00 0000 5a0b 6578 6563 5f63 6f6e 6669  ....Z.exec_confi
 00000700: 6772 0d00 0000 5a11 6578 6563 5f73 7461  gr....Z.exec_sta
 00000710: 7274 5f63 6f6e 6669 6772 0e00 0000 5a0b  rt_configr....Z.
 00000720: 6964 5f72 6573 706f 6e73 6572 0f00 0000  id_responser....
 00000730: da05 696d 6167 6572 1000 0000 5a12 696d  ..imager....Z.im
 00000740: 6167 655f 6275 696c 645f 636f 6e66 6967  age_build_config
 00000750: 7211 0000 005a 1c69 6d61 6765 5f62 7569  r....Z.image_bui
 00000760: 6c64 5f63 6f6e 6669 675f 6275 696c 6461  ld_config_builda
@@ -144,15 +144,15 @@
 000008f0: 6f6c 756d 6572 2200 0000 5a0d 766f 6c75  olumer"...Z.volu
 00000900: 6d65 5f63 6f6e 6669 6772 2300 0000 5a0e  me_configr#...Z.
 00000910: 766f 6c75 6d65 5f69 6e73 7065 6374 7224  volume_inspectr$
 00000920: 0000 005a 1277 6562 5f73 6f63 6b65 745f  ...Z.web_socket_
 00000930: 6d65 7373 6167 6572 2500 0000 5a1b 7765  messager%...Z.we
 00000940: 625f 736f 636b 6574 5f6d 6573 7361 6765  b_socket_message
 00000950: 5f6d 7367 5f74 7970 6572 2600 0000 da07  _msg_typer&.....
-00000960: 5f5f 616c 6c5f 5fa9 0072 2f00 0000 722f  __all__..r/...r/
+00000960: 5f5f 616c 6c5f 5fa9 0072 2d00 0000 722d  __all__..r-...r-
 00000970: 0000 00fa 2c2f 7661 6772 616e 742f 6b6c  ....,/vagrant/kl
 00000980: 6565 2f6b 6c65 652f 636c 6965 6e74 2f6d  ee/klee/client/m
 00000990: 6f64 656c 732f 5f5f 696e 6974 5f5f 2e70  odels/__init__.p
 000009a0: 79da 083c 6d6f 6475 6c65 3e01 0000 0073  y..<module>....s
 000009b0: 4c00 0000 0402 0c01 0c01 0c01 0c01 0c01  L...............
 000009c0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
 000009d0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 8714 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 0a22 0000  a.......$..f."..
+00000000: 610d 0d0a 0000 0000 4afe 3166 0a22 0000  a.......J.1f."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 0100 6400 6402 6c09 6d0a 5a0b  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6403 6c09 6d0c 5a0d 0100 6404  ..d.d.l.m.Z...d.
 00000070: 6405 6c0e 6d0f 5a0f 0100 6404 6406 6c10  d.l.m.Z...d.d.l.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 10371 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 8328 0000  a.......$..f.(..
+00000000: 610d 0d0a 0000 0000 4afe 3166 8328 0000  a.......J.1f.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 0100 6400 6402 6c09 6d0a 5a0b  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6403 6c09 6d0c 5a0d 0100 6404  ..d.d.l.m.Z...d.
 00000070: 6405 6c0e 6d0f 5a0f 0100 6404 6406 6c10  d.l.m.Z...d.d.l.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_config_network_driver.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_config_network_driver.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:37 2024 UTC, .py size: 215 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1db1 1d66 d700 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 44fe 3166 d700 0000  a.......D.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 732a 0000 0065 005a  ....@...s*...e.Z
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_inspect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_inspect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:43 2024 UTC, .py size: 4462 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 23b1 1d66 6e11 0000  a.......#..fn...
+00000000: 610d 0d0a 0000 0000 4afe 3166 6e11 0000  a.......J.1fn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c08 6d0b 5a0c 0100 6404 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 0100 6501 7274 6404  m.Z.m.Z...e.rtd.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_network_driver.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_network_driver.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:37 2024 UTC, .py size: 209 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 610d 0d0a 0000 0000 1db1 1d66 d100 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 44fe 3166 d100 0000  a.......D.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 732a 0000 0065 005a  ....@...s*...e.Z
 00000080: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
 00000090: 0564 045a 0665 0764 059c 0164 0664 0784  .d.Z.e.d...d.d..
 000000a0: 045a 0864 0853 0029 09da 1643 6f6e 7461  .Z.d.S.)...Conta
 000000b0: 696e 6572 4e65 7477 6f72 6b44 7269 7665  inerNetworkDrive
 000000c0: 72da 0864 6973 6162 6c65 64da 0468 6f73  r..disabled..hos
-000000d0: 74da 0569 706e 6574 5a04 766e 6574 2901  t..ipnetZ.vnet).
+000000d0: 745a 0569 706e 6574 da04 766e 6574 2901  tZ.ipnet..vnet).
 000000e0: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
 000000f0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
 00000100: 0073 0a00 0000 7400 7c00 6a01 8301 5300  .s....t.|.j...S.
 00000110: 2901 4e29 02da 0373 7472 da05 7661 6c75  ).N)...str..valu
 00000120: 6529 01da 0473 656c 66a9 0072 0b00 0000  e)...self..r....
 00000130: fa3c 2f76 6167 7261 6e74 2f6b 6c65 652f  .</vagrant/klee/
 00000140: 6b6c 6565 2f63 6c69 656e 742f 6d6f 6465  klee/client/mode
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_restart_policy.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_restart_policy.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:38 2024 UTC, .py size: 171 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1eb1 1d66 ab00 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 45fe 3166 ab00 0000  a.......E.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 7322 0000 0065 005a  ....@...s"...e.Z
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/container_summary.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/container_summary.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 9707 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 eb25 0000  a.......$..f.%..
+00000000: 610d 0d0a 0000 0000 4bfe 3166 eb25 0000  a.......K.1f.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 0100 6400 6402 6c09 6d0a 5a0b  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6403 6c09 6d0c 5a0d 0100 6404  ..d.d.l.m.Z...d.
 00000070: 6405 6c0e 6d0f 5a0f 0100 6404 6406 6c10  d.l.m.Z...d.d.l.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/end_point.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/end_point.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 3290 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 da0c 0000  a.......$..f....
+00000000: 610d 0d0a 0000 0000 4bfe 3166 da0c 0000  a.......K.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 6d0e 5a0e 0100 6505 6406 6407 6408 8d02  m.Z...e.d.d.d...
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/end_point_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/end_point_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 2885 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 450b 0000  a.......$..fE...
+00000000: 610d 0d0a 0000 0000 4bfe 3166 450b 0000  a.......K.1fE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 6d0e 5a0e 0100 6505 6406 6407 6408 8d02  m.Z...e.d.d.d...
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/error_response.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/error_response.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 1590 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 3606 0000  a.......$..f6...
+00000000: 610d 0d0a 0000 0000 4afe 3166 3606 0000  a.......J.1f6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6400 6403 6c06 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6505 6404 6405 6406 8d02 5a0b 6508  ..e.d.d.d...Z.e.
 00000070: 4700 6407 6405 8400 6405 8302 8301 5a0c  G.d.d...d.....Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/exec_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/exec_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 3702 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 760e 0000  a.......$..fv...
+00000000: 610d 0d0a 0000 0000 4bfe 3166 760e 0000  a.......K.1fv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c08 6d0b 5a0c 0100 6404 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 0100 6505 6406 6407  m.Z.m.Z...e.d.d.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/exec_start_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/exec_start_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 2084 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 2408 0000  a.......$..f$...
+00000000: 610d 0d0a 0000 0000 4bfe 3166 2408 0000  a.......K.1f$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6400 6403 6c06 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6505 6404 6405 6406 8d02 5a0b 6508  ..e.d.d.d...Z.e.
 00000070: 4700 6407 6405 8400 6405 8302 8301 5a0c  G.d.d...d.....Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/id_response.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/id_response.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 1483 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 cb05 0000  a.......$..f....
+00000000: 610d 0d0a 0000 0000 4bfe 3166 cb05 0000  a.......K.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6400 6403 6c06 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6505 6404 6405 6406 8d02 5a0b 6508  ..e.d.d.d...Z.e.
 00000070: 4700 6407 6405 8400 6405 8302 8301 5a0c  G.d.d...d.....Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 4937 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 4913 0000  a.......%..fI...
+00000000: 610d 0d0a 0000 0000 4bfe 3166 4913 0000  a.......K.1fI...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c08 6d0b 5a0c 0100 6404 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 0100 6505 6406 6407  m.Z.m.Z...e.d.d.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image_build_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image_build_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 5646 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 0e16 0000  a.......%..f....
+00000000: 610d 0d0a 0000 0000 4bfe 3166 0e16 0000  a.......K.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c08 6d0b 5a0c 0100 6404 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 0100 6501 7274 6404  m.Z.m.Z...e.rtd.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image_build_config_buildargs.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image_build_config_buildargs.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:44 2024 UTC, .py size: 1525 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 24b1 1d66 f505 0000  a.......$..f....
+00000000: 610d 0d0a 0000 0000 4bfe 3166 f505 0000  a.......K.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6400 6403 6c06 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6505 6404 6405 6406 8d02 5a0b 6508  ..e.d.d.d...Z.e.
 00000070: 4700 6407 6405 8400 6405 8302 8301 5a0c  G.d.d...d.....Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image_create_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image_create_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 5294 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 ae14 0000  a.......%..f....
+00000000: 610d 0d0a 0000 0000 4cfe 3166 4b13 0000  a.......L.1fK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6404 6406 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
@@ -15,313 +15,296 @@
 000000e0: da05 6669 656c 64e9 0200 0000 2901 da17  ..field.....)...
 000000f0: 496d 6167 6543 7265 6174 6543 6f6e 6669  ImageCreateConfi
 00000100: 674d 6574 686f 6429 02da 0555 4e53 4554  gMethod)...UNSET
 00000110: da05 556e 7365 74da 0154 da11 496d 6167  ..Unset..T..Imag
 00000120: 6543 7265 6174 6543 6f6e 6669 6729 01da  eCreateConfig)..
 00000130: 0562 6f75 6e64 6300 0000 0000 0000 0000  .boundc.........
 00000140: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
-00000150: 6601 0000 6500 5a01 6400 5a02 5500 6401  f...e.Z.d.Z.U.d.
+00000150: 5201 0000 6500 5a01 6400 5a02 5500 6401  R...e.Z.d.Z.U.d.
 00000160: 5a03 6504 6505 6402 3c00 6403 5a06 6507  Z.e.e.d.<.d.Z.e.
 00000170: 6508 6509 6602 1900 6505 6404 3c00 6405  e.e.f...e.d.<.d.
 00000180: 5a0a 6507 6508 6509 6602 1900 6505 6406  Z.e.e.e.f...e.d.
-00000190: 3c00 6403 5a0b 6507 6508 6509 6602 1900  <.d.Z.e.e.e.f...
-000001a0: 6505 6407 3c00 6405 5a0c 6507 6508 6509  e.d.<.d.Z.e.e.e.
-000001b0: 6602 1900 6505 6408 3c00 6409 5a0d 6507  f...e.d.<.d.Z.e.
-000001c0: 6508 650e 6602 1900 6505 640a 3c00 6405  e.e.f...e.d.<.d.
-000001d0: 5a0f 6507 6508 6509 6602 1900 6505 640b  Z.e.e.e.f...e.d.
-000001e0: 3c00 6409 5a10 6507 6508 650e 6602 1900  <.d.Z.e.e.e.f...
-000001f0: 6505 640c 3c00 6409 5a11 6507 6508 650e  e.d.<.d.Z.e.e.e.
-00000200: 6602 1900 6505 640d 3c00 6512 6403 6513  f...e.d.<.e.d.e.
-00000210: 640e 8d02 5a14 6515 650e 6516 6602 1900  d...Z.e.e.e.f...
-00000220: 6505 640f 3c00 6515 650e 6516 6602 1900  e.d.<.e.e.e.f...
-00000230: 6410 9c01 6411 6412 8404 5a17 6518 6519  d...d.d...Z.e.e.
-00000240: 651a 1900 6515 650e 6516 6602 1900 651a  e...e.e.e.f...e.
-00000250: 6413 9c03 6414 6415 8404 8301 5a1b 651c  d...d.d.....Z.e.
-00000260: 651d 650e 1900 6410 9c01 6416 6417 8404  e.e...d...d.d...
-00000270: 8301 5a1e 650e 6516 6418 9c02 6419 641a  ..Z.e.e.d...d.d.
-00000280: 8404 5a1f 650e 6516 641b 641c 9c03 641d  ..Z.e.e.d.d...d.
-00000290: 641e 8404 5a20 650e 641b 6418 9c02 641f  d...Z e.d.d...d.
-000002a0: 6420 8404 5a21 650e 6509 6418 9c02 6421  d ..Z!e.e.d...d!
-000002b0: 6422 8404 5a22 641b 5300 2923 720f 0000  d"..Z"d.S.)#r...
-000002c0: 0061 ff07 0000 436f 6e66 6967 7572 6174  .a....Configurat
-000002d0: 696f 6e20 666f 7220 7468 6520 6372 6561  ion for the crea
-000002e0: 7469 6f6e 206f 6620 6261 7365 2069 6d61  tion of base ima
-000002f0: 6765 732e 0a0a 2020 2020 4174 7472 6962  ges...    Attrib
-00000300: 7574 6573 3a0a 2020 2020 2020 2020 6d65  utes:.        me
-00000310: 7468 6f64 2028 496d 6167 6543 7265 6174  thod (ImageCreat
-00000320: 6543 6f6e 6669 674d 6574 686f 6429 3a20  eConfigMethod): 
-00000330: 5468 6572 6520 6172 6520 666f 7572 206d  There are four m
-00000340: 6574 686f 6473 2066 6f72 2063 7265 6174  ethods for creat
-00000350: 696e 6720 6120 6e65 7720 6261 7365 2069  ing a new base i
-00000360: 6d61 6765 3a0a 0a20 2020 2020 2020 2020  mage:..         
-00000370: 2020 202d 2060 6665 7463 6860 3a20 4665     - `fetch`: Fe
-00000380: 7463 6820 6120 7265 6c65 6173 652f 736e  tch a release/sn
-00000390: 6170 7368 6f74 206f 6620 7468 6520 6261  apshot of the ba
-000003a0: 7365 2073 7973 7465 6d20 6672 6f6d 2060  se system from `
-000003b0: 7572 6c60 2061 6e64 2075 7365 2069 7420  url` and use it 
-000003c0: 666f 7220 696d 6167 6520 6372 6561 7469  for image creati
-000003d0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-000003e0: 2d20 6066 6574 6368 2d61 7574 6f60 3a20  - `fetch-auto`: 
-000003f0: 4175 746f 6d61 7469 6361 6c6c 7920 6665  Automatically fe
-00000400: 7463 6820 6120 7265 6c65 6173 652f 736e  tch a release/sn
-00000410: 6170 7368 6f74 2066 726f 6d20 7468 6520  apshot from the 
-00000420: 6f66 6669 6361 6c20 4672 6565 4253 4420  offical FreeBSD 
-00000430: 6d69 7272 6f72 732c 2062 6173 6564 206f  mirrors, based o
-00000440: 6e20 696e 666f 726d 6174 696f 6e0a 2020  n information.  
-00000450: 2020 2020 2020 2020 2020 6672 6f6d 2060            from `
-00000460: 756e 616d 6528 3129 602e 0a20 2020 2020  uname(1)`..     
-00000470: 2020 2020 2020 202d 2060 7a66 732d 636f         - `zfs-co
-00000480: 7079 603a 2043 7265 6174 6520 7468 6520  py`: Create the 
-00000490: 6261 7365 2069 6d61 6765 2062 6173 6564  base image based
-000004a0: 206f 6e20 6120 636f 7079 206f 6620 607a   on a copy of `z
-000004b0: 6673 5f64 6174 6173 6574 602e 0a20 2020  fs_dataset`..   
-000004c0: 2020 2020 2020 2020 202d 2060 7a66 732d           - `zfs-
-000004d0: 636c 6f6e 6560 3a20 4372 6561 7465 2074  clone`: Create t
-000004e0: 6865 2062 6173 6520 696d 6167 6520 6261  he base image ba
-000004f0: 7365 6420 6f6e 2061 2063 6c6f 6e65 206f  sed on a clone o
-00000500: 6620 607a 6673 5f64 6174 6173 6574 602e  f `zfs_dataset`.
-00000510: 0a20 2020 2020 2020 2061 7574 6f74 6167  .        autotag
-00000520: 2028 556e 696f 6e5b 556e 7365 742c 2062   (Union[Unset, b
-00000530: 6f6f 6c5d 293a 202a 2a60 6665 7463 682d  ool]): **`fetch-
-00000540: 6175 746f 6020 6d65 7468 6f64 206f 6e6c  auto` method onl
-00000550: 792a 2a0a 0a20 2020 2020 2020 2020 2020  y**..           
-00000560: 2057 6865 7468 6572 206f 7220 6e6f 7420   Whether or not 
-00000570: 746f 2061 7574 6f2d 6765 6e65 7265 6174  to auto-genereat
-00000580: 6520 6120 6e61 6d65 7461 6720 6046 7265  e a nametag `Fre
-00000590: 6542 5344 2d3c 7665 7273 696f 6e3e 3a6c  eBSD-<version>:l
-000005a0: 6174 6573 7460 2062 6173 6564 206f 6e20  atest` based on 
-000005b0: 6075 6e61 6d65 2831 2960 2e0a 2020 2020  `uname(1)`..    
-000005c0: 2020 2020 2020 2020 4f76 6572 7269 6465          Override
-000005d0: 7320 6074 6167 6020 6966 2073 6574 2074  s `tag` if set t
-000005e0: 6f20 6074 7275 6560 2e0a 2020 2020 2020  o `true`..      
-000005f0: 2020 646e 7320 2855 6e69 6f6e 5b55 6e73    dns (Union[Uns
-00000600: 6574 2c20 626f 6f6c 5d29 3a20 5768 6574  et, bool]): Whet
-00000610: 6865 7220 6f72 206e 6f74 2074 6f20 636f  her or not to co
-00000620: 7079 2060 2f65 7463 2f72 6573 6f6c 762e  py `/etc/resolv.
-00000630: 636f 6e66 6020 6672 6f6d 2074 6865 2068  conf` from the h
-00000640: 6f73 7420 746f 2074 6865 206e 6577 2069  ost to the new i
-00000650: 6d61 6765 2e20 4465 6661 756c 743a 0a20  mage. Default:. 
-00000660: 2020 2020 2020 2020 2020 2054 7275 652e             True.
-00000670: 0a20 2020 2020 2020 2066 6f72 6365 2028  .        force (
-00000680: 556e 696f 6e5b 556e 7365 742c 2062 6f6f  Union[Unset, boo
-00000690: 6c5d 293a 202a 2a60 6665 7463 682d 6175  l]): **`fetch-au
-000006a0: 746f 6020 6d65 7468 6f64 206f 6e6c 792a  to` method only*
-000006b0: 2a0a 0a20 2020 2020 2020 2020 2020 2049  *..            I
-000006c0: 676e 6f72 6520 616e 7920 6469 7363 7265  gnore any discre
-000006d0: 7061 6e63 6965 7320 696e 2074 6865 206f  pancies in the o
-000006e0: 7574 7075 7420 6f66 2060 756e 616d 6528  utput of `uname(
-000006f0: 3129 6020 7768 656e 2064 6574 6572 6d69  1)` when determi
-00000700: 6e69 6e67 2074 6865 2046 7265 6542 5344  ning the FreeBSD
-00000710: 2076 6572 7369 6f6e 2e0a 2020 2020 2020   version..      
-00000720: 2020 6c6f 6361 6c74 696d 6520 2855 6e69    localtime (Uni
-00000730: 6f6e 5b55 6e73 6574 2c20 626f 6f6c 5d29  on[Unset, bool])
-00000740: 3a20 5768 6574 6865 7220 6f72 206e 6f74  : Whether or not
-00000750: 2074 6f20 636f 7079 2060 2f65 7463 2f6c   to copy `/etc/l
-00000760: 6f63 616c 7469 6d65 6020 6672 6f6d 2074  ocaltime` from t
-00000770: 6865 2068 6f73 7420 746f 2074 6865 206e  he host to the n
-00000780: 6577 2069 6d61 6765 2e20 4465 6661 756c  ew image. Defaul
-00000790: 743a 0a20 2020 2020 2020 2020 2020 2054  t:.            T
-000007a0: 7275 652e 0a20 2020 2020 2020 2074 6167  rue..        tag
-000007b0: 2028 556e 696f 6e5b 556e 7365 742c 2073   (Union[Unset, s
-000007c0: 7472 5d29 3a20 4e61 6d65 2061 6e64 206f  tr]): Name and o
-000007d0: 7074 696f 6e61 6c6c 7920 6120 7461 6720  ptionally a tag 
-000007e0: 696e 2074 6865 2060 6e61 6d65 3a74 6167  in the `name:tag
-000007f0: 6020 666f 726d 6174 2e20 4966 2060 7461  ` format. If `ta
-00000800: 6760 2069 7320 6f6d 6974 7465 642c 2074  g` is omitted, t
-00000810: 6865 2064 6566 6175 6c74 0a20 2020 2020  he default.     
-00000820: 2020 2020 2020 2076 616c 7565 2060 6c61         value `la
-00000830: 7465 7374 6020 6973 2075 7365 642e 0a20  test` is used.. 
-00000840: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00000850: 756c 743a 2027 272e 0a20 2020 2020 2020  ult: ''..       
-00000860: 2075 7064 6174 6520 2855 6e69 6f6e 5b55   update (Union[U
-00000870: 6e73 6574 2c20 626f 6f6c 5d29 3a20 5570  nset, bool]): Up
-00000880: 6461 7465 2074 6865 2062 6173 6520 696d  date the base im
-00000890: 6167 6520 7573 696e 6720 6066 7265 6562  age using `freeb
-000008a0: 7364 2d75 7064 6174 6528 3829 602e 0a20  sd-update(8)`.. 
-000008b0: 2020 2020 2020 2020 2020 2053 6565 2074             See t
-000008c0: 6865 205b 6d61 6e2d 7061 6765 735d 2868  he [man-pages](h
-000008d0: 7474 7073 3a2f 2f6d 616e 2e66 7265 6562  ttps://man.freeb
-000008e0: 7364 2e6f 7267 2f63 6769 2f6d 616e 2e63  sd.org/cgi/man.c
-000008f0: 6769 3f71 7565 7279 3d66 7265 6562 7364  gi?query=freebsd
-00000900: 2d75 7064 6174 6529 2066 6f72 2064 6574  -update) for det
-00000910: 6169 6c73 2061 626f 7574 2077 6869 6368  ails about which
-00000920: 2046 7265 6542 5344 0a20 2020 2020 2020   FreeBSD.       
-00000930: 2020 2020 2076 6572 7369 6f6e 7320 6361       versions ca
-00000940: 6e20 6265 2075 7064 6174 6564 2e22 2c0a  n be updated.",.
-00000950: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00000960: 6175 6c74 3a20 5472 7565 2e0a 2020 2020  ault: True..    
-00000970: 2020 2020 7572 6c20 2855 6e69 6f6e 5b55      url (Union[U
-00000980: 6e73 6574 2c20 7374 725d 293a 202a 2a60  nset, str]): **`
-00000990: 6665 7463 6860 206d 6574 686f 6420 6f6e  fetch` method on
-000009a0: 6c79 2a2a 0a0a 2020 2020 2020 2020 2020  ly**..          
-000009b0: 2020 5552 4c20 746f 2074 6865 2062 6173    URL to the bas
-000009c0: 6520 7379 7374 656d 2028 6120 6062 6173  e system (a `bas
-000009d0: 652e 7478 7a60 2066 696c 6529 2074 6861  e.txz` file) tha
-000009e0: 7420 4b6c 6565 6e65 6420 7368 6f75 6c64  t Kleened should
-000009f0: 2075 7365 2074 6f20 6372 6561 7465 2074   use to create t
-00000a00: 6865 2062 6173 6520 696d 6167 652e 0a20  he base image.. 
-00000a10: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00000a20: 756c 743a 2027 272e 0a20 2020 2020 2020  ult: ''..       
-00000a30: 207a 6673 5f64 6174 6173 6574 2028 556e   zfs_dataset (Un
-00000a40: 696f 6e5b 556e 7365 742c 2073 7472 5d29  ion[Unset, str])
-00000a50: 3a20 2a2a 607a 6673 2d2a 6020 6d65 7468  : **`zfs-*` meth
-00000a60: 6f64 7320 6f6e 6c79 2a2a 0a0a 2020 2020  ods only**..    
-00000a70: 2020 2020 2020 2020 5a46 5320 6461 7461          ZFS data
-00000a80: 7365 7420 7468 6174 2074 6865 2069 6d61  set that the ima
-00000a90: 6765 2073 686f 756c 6420 6265 2062 6173  ge should be bas
-00000aa0: 6564 206f 6e2e 0a20 2020 2020 2020 2020  ed on..         
-00000ab0: 2020 2020 4465 6661 756c 743a 2027 272e      Default: ''.
-00000ac0: 0a20 2020 20da 066d 6574 686f 6446 da07  .    ..methodF..
-00000ad0: 6175 746f 7461 6754 da03 646e 73da 0566  autotagT..dns..f
-00000ae0: 6f72 6365 da09 6c6f 6361 6c74 696d 65da  orce..localtime.
-00000af0: 00da 0374 6167 da06 7570 6461 7465 da03  ...tag..update..
-00000b00: 7572 6cda 0b7a 6673 5f64 6174 6173 6574  url..zfs_dataset
-00000b10: 2902 da04 696e 6974 da07 6661 6374 6f72  )...init..factor
-00000b20: 79da 1561 6464 6974 696f 6e61 6c5f 7072  y..additional_pr
-00000b30: 6f70 6572 7469 6573 2901 da06 7265 7475  operties)...retu
-00000b40: 726e 6301 0000 0000 0000 0000 0000 000b  rnc.............
-00000b50: 0000 0004 0000 0043 0000 0073 da00 0000  .......C...s....
-00000b60: 7c00 6a00 6a01 7d01 7c00 6a02 7d02 7c00  |.j.j.}.|.j.}.|.
-00000b70: 6a03 7d03 7c00 6a04 7d04 7c00 6a05 7d05  j.}.|.j.}.|.j.}.
-00000b80: 7c00 6a06 7d06 7c00 6a07 7d07 7c00 6a08  |.j.}.|.j.}.|.j.
-00000b90: 7d08 7c00 6a09 7d09 6900 7d0a 7c0a a007  }.|.j.}.i.}.|...
-00000ba0: 7c00 6a0a a101 0100 7c0a a007 6401 7c01  |.j.....|...d.|.
-00000bb0: 6901 a101 0100 7c02 740b 7501 7266 7c02  i.....|.t.u.rf|.
-00000bc0: 7c0a 6402 3c00 7c03 740b 7501 7276 7c03  |.d.<.|.t.u.rv|.
-00000bd0: 7c0a 6403 3c00 7c04 740b 7501 7286 7c04  |.d.<.|.t.u.r.|.
-00000be0: 7c0a 6404 3c00 7c05 740b 7501 7296 7c05  |.d.<.|.t.u.r.|.
-00000bf0: 7c0a 6405 3c00 7c06 740b 7501 72a6 7c06  |.d.<.|.t.u.r.|.
-00000c00: 7c0a 6406 3c00 7c07 740b 7501 72b6 7c07  |.d.<.|.t.u.r.|.
-00000c10: 7c0a 6407 3c00 7c08 740b 7501 72c6 7c08  |.d.<.|.t.u.r.|.
-00000c20: 7c0a 6408 3c00 7c09 740b 7501 72d6 7c09  |.d.<.|.t.u.r.|.
-00000c30: 7c0a 6409 3c00 7c0a 5300 290a 4e72 1100  |.d.<.|.S.).Nr..
-00000c40: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00000c50: 0072 1500 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000c60: 7219 0000 0072 1a00 0000 290c 7211 0000  r....r....).r...
-00000c70: 00da 0576 616c 7565 7212 0000 0072 1300  ...valuer....r..
-00000c80: 0000 7214 0000 0072 1500 0000 7217 0000  ..r....r....r...
-00000c90: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000ca0: 721d 0000 0072 0c00 0000 290b da04 7365  r....r....)...se
-00000cb0: 6c66 7211 0000 0072 1200 0000 7213 0000  lfr....r....r...
-00000cc0: 0072 1400 0000 7215 0000 0072 1700 0000  .r....r....r....
-00000cd0: 7218 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00000ce0: 0a66 6965 6c64 5f64 6963 74a9 0072 2200  .field_dict..r".
-00000cf0: 0000 fa37 2f76 6167 7261 6e74 2f6b 6c65  ...7/vagrant/kle
-00000d00: 652f 6b6c 6565 2f63 6c69 656e 742f 6d6f  e/klee/client/mo
-00000d10: 6465 6c73 2f69 6d61 6765 5f63 7265 6174  dels/image_creat
-00000d20: 655f 636f 6e66 6967 2e70 79da 0774 6f5f  e_config.py..to_
-00000d30: 6469 6374 3f00 0000 7340 0000 0000 0108  dict?...s@......
-00000d40: 0206 0106 0106 0106 0106 0106 0106 0106  ................
-00000d50: 0204 010c 0104 0204 ff02 ff04 0508 0108  ................
-00000d60: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00000d70: 0108 0108 0108 0108 0108 0108 027a 1949  .............z.I
-00000d80: 6d61 6765 4372 6561 7465 436f 6e66 6967  mageCreateConfig
-00000d90: 2e74 6f5f 6469 6374 2903 da03 636c 73da  .to_dict)...cls.
-00000da0: 0873 7263 5f64 6963 7472 1e00 0000 6302  .src_dictr....c.
-00000db0: 0000 0000 0000 0000 0000 000d 0000 000b  ................
-00000dc0: 0000 0043 0000 0073 9a00 0000 7c01 a000  ...C...s....|...
-00000dd0: a100 7d02 7401 7c02 a002 6401 a101 8301  ..}.t.|...d.....
-00000de0: 7d03 7c02 a002 6402 7403 a102 7d04 7c02  }.|...d.t...}.|.
-00000df0: a002 6403 7403 a102 7d05 7c02 a002 6404  ..d.t...}.|...d.
-00000e00: 7403 a102 7d06 7c02 a002 6405 7403 a102  t...}.|...d.t...
-00000e10: 7d07 7c02 a002 6406 7403 a102 7d08 7c02  }.|...d.t...}.|.
-00000e20: a002 6407 7403 a102 7d09 7c02 a002 6408  ..d.t...}.|...d.
-00000e30: 7403 a102 7d0a 7c02 a002 6409 7403 a102  t...}.|...d.t...
-00000e40: 7d0b 7c00 7c03 7c04 7c05 7c06 7c07 7c08  }.|.|.|.|.|.|.|.
-00000e50: 7c09 7c0a 7c0b 640a 8d09 7d0c 7c02 7c0c  |.|.|.d...}.|.|.
-00000e60: 5f04 7c0c 5300 290b 4e72 1100 0000 7212  _.|.S.).Nr....r.
-00000e70: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
-00000e80: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000e90: 0072 1a00 0000 2909 7211 0000 0072 1200  .r....).r....r..
-00000ea0: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000eb0: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000ec0: 721a 0000 0029 05da 0463 6f70 7972 0b00  r....)...copyr..
-00000ed0: 0000 da03 706f 7072 0c00 0000 721d 0000  ....popr....r...
-00000ee0: 0029 0d72 2500 0000 7226 0000 00da 0164  .).r%...r&.....d
-00000ef0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00000f00: 1400 0000 7215 0000 0072 1700 0000 7218  ....r....r....r.
-00000f10: 0000 0072 1900 0000 721a 0000 00da 1369  ...r....r......i
-00000f20: 6d61 6765 5f63 7265 6174 655f 636f 6e66  mage_create_conf
-00000f30: 6967 7222 0000 0072 2200 0000 7223 0000  igr"...r"...r#..
-00000f40: 00da 0966 726f 6d5f 6469 6374 6500 0000  ...from_dicte...
-00000f50: 732e 0000 0000 0208 010e 020c 020c 020c  s...............
-00000f60: 020c 020c 020c 020c 020c 0202 0102 0102  ................
-00000f70: 0102 0102 0102 0102 0102 0102 0102 f706  ................
-00000f80: 0c06 017a 1b49 6d61 6765 4372 6561 7465  ...z.ImageCreate
-00000f90: 436f 6e66 6967 2e66 726f 6d5f 6469 6374  Config.from_dict
-00000fa0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000fb0: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-00000fc0: 7c00 6a01 a002 a100 8301 5300 a901 4e29  |.j.......S...N)
-00000fd0: 03da 046c 6973 7472 1d00 0000 da04 6b65  ...listr......ke
-00000fe0: 7973 2901 7220 0000 0072 2200 0000 7222  ys).r ...r"...r"
-00000ff0: 0000 0072 2300 0000 da0f 6164 6469 7469  ...r#.....additi
-00001000: 6f6e 616c 5f6b 6579 7389 0000 0073 0200  onal_keys....s..
-00001010: 0000 0002 7a21 496d 6167 6543 7265 6174  ....z!ImageCreat
-00001020: 6543 6f6e 6669 672e 6164 6469 7469 6f6e  eConfig.addition
-00001030: 616c 5f6b 6579 7329 02da 036b 6579 721e  al_keys)...keyr.
-00001040: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00001050: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-00001060: 007c 006a 007c 0119 0053 0072 2c00 0000  .|.j.|...S.r,...
-00001070: a901 721d 0000 00a9 0272 2000 0000 7230  ..r......r ...r0
-00001080: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00001090: 0000 da0b 5f5f 6765 7469 7465 6d5f 5f8d  ....__getitem__.
-000010a0: 0000 0073 0200 0000 0001 7a1d 496d 6167  ...s......z.Imag
-000010b0: 6543 7265 6174 6543 6f6e 6669 672e 5f5f  eCreateConfig.__
-000010c0: 6765 7469 7465 6d5f 5f4e 2903 7230 0000  getitem__N).r0..
-000010d0: 0072 1f00 0000 721e 0000 0063 0300 0000  .r....r....c....
-000010e0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-000010f0: 4300 0000 730e 0000 007c 027c 006a 007c  C...s....|.|.j.|
-00001100: 013c 0064 0053 0072 2c00 0000 7231 0000  .<.d.S.r,...r1..
-00001110: 0029 0372 2000 0000 7230 0000 0072 1f00  .).r ...r0...r..
-00001120: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00001130: 00da 0b5f 5f73 6574 6974 656d 5f5f 9000  ...__setitem__..
-00001140: 0000 7302 0000 0000 017a 1d49 6d61 6765  ..s......z.Image
-00001150: 4372 6561 7465 436f 6e66 6967 2e5f 5f73  CreateConfig.__s
-00001160: 6574 6974 656d 5f5f 6302 0000 0000 0000  etitem__c.......
-00001170: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00001180: 0073 0c00 0000 7c00 6a00 7c01 3d00 6400  .s....|.j.|.=.d.
-00001190: 5300 722c 0000 0072 3100 0000 7232 0000  S.r,...r1...r2..
-000011a0: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
-000011b0: da0b 5f5f 6465 6c69 7465 6d5f 5f93 0000  ..__delitem__...
-000011c0: 0073 0200 0000 0001 7a1d 496d 6167 6543  .s......z.ImageC
-000011d0: 7265 6174 6543 6f6e 6669 672e 5f5f 6465  reateConfig.__de
-000011e0: 6c69 7465 6d5f 5f63 0200 0000 0000 0000  litem__c........
-000011f0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00001200: 730a 0000 007c 017c 006a 0076 0053 0072  s....|.|.j.v.S.r
-00001210: 2c00 0000 7231 0000 0072 3200 0000 7222  ,...r1...r2...r"
-00001220: 0000 0072 2200 0000 7223 0000 00da 0c5f  ...r"...r#....._
-00001230: 5f63 6f6e 7461 696e 735f 5f96 0000 0073  _contains__....s
-00001240: 0200 0000 0001 7a1e 496d 6167 6543 7265  ......z.ImageCre
-00001250: 6174 6543 6f6e 6669 672e 5f5f 636f 6e74  ateConfig.__cont
-00001260: 6169 6e73 5f5f 2923 da08 5f5f 6e61 6d65  ains__)#..__name
-00001270: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001280: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00001290: 646f 635f 5f72 0b00 0000 da0f 5f5f 616e  doc__r......__an
-000012a0: 6e6f 7461 7469 6f6e 735f 5f72 1200 0000  notations__r....
-000012b0: 7207 0000 0072 0d00 0000 da04 626f 6f6c  r....r......bool
-000012c0: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-000012d0: 1700 0000 da03 7374 7272 1800 0000 7219  ......strr....r.
-000012e0: 0000 0072 1a00 0000 da0c 5f61 7474 7273  ...r......_attrs
-000012f0: 5f66 6965 6c64 da04 6469 6374 721d 0000  _field..dictr...
-00001300: 0072 0300 0000 7202 0000 0072 2400 0000  .r....r....r$...
-00001310: da0b 636c 6173 736d 6574 686f 6472 0500  ..classmethodr..
-00001320: 0000 720e 0000 0072 2b00 0000 da08 7072  ..r....r+.....pr
-00001330: 6f70 6572 7479 7204 0000 0072 2f00 0000  opertyr....r/...
-00001340: 7233 0000 0072 3400 0000 7235 0000 0072  r3...r4...r5...r
-00001350: 3600 0000 7222 0000 0072 2200 0000 7222  6...r"...r"...r"
-00001360: 0000 0072 2300 0000 720f 0000 000c 0000  ...r#...r.......
-00001370: 0073 2800 0000 0a02 0426 0801 1401 1401  .s(......&......
-00001380: 1401 1401 1401 1401 1401 1401 1c02 1626  ...............&
-00001390: 0201 2023 0201 1403 1003 1203 1003 4e29  .. #..........N)
-000013a0: 13da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
-000013b0: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
-000013c0: 0000 7207 0000 00da 0561 7474 7273 7208  ..r......attrsr.
-000013d0: 0000 00da 0d5f 6174 7472 735f 6465 6669  ....._attrs_defi
-000013e0: 6e65 7209 0000 0072 3e00 0000 5a21 6d6f  ner....r>...Z!mo
-000013f0: 6465 6c73 2e69 6d61 6765 5f63 7265 6174  dels.image_creat
-00001400: 655f 636f 6e66 6967 5f6d 6574 686f 6472  e_config_methodr
-00001410: 0b00 0000 da05 7479 7065 7372 0c00 0000  ......typesr....
-00001420: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00001430: 2200 0000 7222 0000 0072 2200 0000 7223  "...r"...r"...r#
-00001440: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001450: 0073 0e00 0000 2002 0c01 0c02 0c01 1002  .s.... .........
-00001460: 0c03 0201                                ....
+00000190: 3c00 6405 5a0b 6507 6508 6509 6602 1900  <.d.Z.e.e.e.f...
+000001a0: 6505 6407 3c00 6408 5a0c 6507 6508 650d  e.d.<.d.Z.e.e.e.
+000001b0: 6602 1900 6505 6409 3c00 6403 5a0e 6507  f...e.d.<.d.Z.e.
+000001c0: 6508 6509 6602 1900 6505 640a 3c00 6408  e.e.f...e.d.<.d.
+000001d0: 5a0f 6507 6508 650d 6602 1900 6505 640b  Z.e.e.e.f...e.d.
+000001e0: 3c00 6408 5a10 6507 6508 650d 6602 1900  <.d.Z.e.e.e.f...
+000001f0: 6505 640c 3c00 6511 6403 6512 640d 8d02  e.d.<.e.d.e.d...
+00000200: 5a13 6514 650d 6515 6602 1900 6505 640e  Z.e.e.e.f...e.d.
+00000210: 3c00 6514 650d 6515 6602 1900 640f 9c01  <.e.e.e.f...d...
+00000220: 6410 6411 8404 5a16 6517 6518 6519 1900  d.d...Z.e.e.e...
+00000230: 6514 650d 6515 6602 1900 6519 6412 9c03  e.e.e.f...e.d...
+00000240: 6413 6414 8404 8301 5a1a 651b 651c 650d  d.d.....Z.e.e.e.
+00000250: 1900 640f 9c01 6415 6416 8404 8301 5a1d  ..d...d.d.....Z.
+00000260: 650d 6515 6417 9c02 6418 6419 8404 5a1e  e.e.d...d.d...Z.
+00000270: 650d 6515 641a 641b 9c03 641c 641d 8404  e.e.d.d...d.d...
+00000280: 5a1f 650d 641a 6417 9c02 641e 641f 8404  Z.e.d.d...d.d...
+00000290: 5a20 650d 6509 6417 9c02 6420 6421 8404  Z e.e.d...d d!..
+000002a0: 5a21 641a 5300 2922 720f 0000 0061 6307  Z!d.S.)"r....ac.
+000002b0: 0000 436f 6e66 6967 7572 6174 696f 6e20  ..Configuration 
+000002c0: 666f 7220 7468 6520 6372 6561 7469 6f6e  for the creation
+000002d0: 206f 6620 6261 7365 2069 6d61 6765 732e   of base images.
+000002e0: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+000002f0: 3a0a 2020 2020 2020 2020 6d65 7468 6f64  :.        method
+00000300: 2028 496d 6167 6543 7265 6174 6543 6f6e   (ImageCreateCon
+00000310: 6669 674d 6574 686f 6429 3a20 5468 6572  figMethod): Ther
+00000320: 6520 6172 6520 666f 7572 206d 6574 686f  e are four metho
+00000330: 6473 2066 6f72 2063 7265 6174 696e 6720  ds for creating 
+00000340: 6120 6e65 7720 6261 7365 2069 6d61 6765  a new base image
+00000350: 3a0a 0a20 2020 2020 2020 2020 2020 202d  :..            -
+00000360: 2060 6665 7463 6860 3a20 4665 7463 6820   `fetch`: Fetch 
+00000370: 6120 7265 6c65 6173 652f 736e 6170 7368  a release/snapsh
+00000380: 6f74 206f 6620 7468 6520 6261 7365 2073  ot of the base s
+00000390: 7973 7465 6d20 6672 6f6d 2060 7572 6c60  ystem from `url`
+000003a0: 2061 6e64 2075 7365 2069 7420 666f 7220   and use it for 
+000003b0: 696d 6167 6520 6372 6561 7469 6f6e 2e0a  image creation..
+000003c0: 2020 2020 2020 2020 2020 2020 2d20 6066              - `f
+000003d0: 6574 6368 2d61 7574 6f60 3a20 4175 746f  etch-auto`: Auto
+000003e0: 6d61 7469 6361 6c6c 7920 6665 7463 6820  matically fetch 
+000003f0: 6120 7265 6c65 6173 652f 736e 6170 7368  a release/snapsh
+00000400: 6f74 2066 726f 6d20 7468 6520 6f66 6669  ot from the offi
+00000410: 6361 6c20 4672 6565 4253 4420 6d69 7272  cal FreeBSD mirr
+00000420: 6f72 732c 2062 6173 6564 206f 6e20 696e  ors, based on in
+00000430: 666f 726d 6174 696f 6e0a 2020 2020 2020  formation.      
+00000440: 2020 2020 2020 6672 6f6d 2060 756e 616d        from `unam
+00000450: 6528 3129 602e 0a20 2020 2020 2020 2020  e(1)`..         
+00000460: 2020 202d 2060 7a66 732d 636f 7079 603a     - `zfs-copy`:
+00000470: 2043 7265 6174 6520 7468 6520 6261 7365   Create the base
+00000480: 2069 6d61 6765 2062 6173 6564 206f 6e20   image based on 
+00000490: 6120 636f 7079 206f 6620 607a 6673 5f64  a copy of `zfs_d
+000004a0: 6174 6173 6574 602e 0a20 2020 2020 2020  ataset`..       
+000004b0: 2020 2020 202d 2060 7a66 732d 636c 6f6e       - `zfs-clon
+000004c0: 6560 3a20 4372 6561 7465 2074 6865 2062  e`: Create the b
+000004d0: 6173 6520 696d 6167 6520 6261 7365 6420  ase image based 
+000004e0: 6f6e 2061 2063 6c6f 6e65 206f 6620 607a  on a clone of `z
+000004f0: 6673 5f64 6174 6173 6574 602e 0a20 2020  fs_dataset`..   
+00000500: 2020 2020 2061 7574 6f74 6167 2028 556e       autotag (Un
+00000510: 696f 6e5b 556e 7365 742c 2062 6f6f 6c5d  ion[Unset, bool]
+00000520: 293a 202a 2a60 6665 7463 682d 6175 746f  ): **`fetch-auto
+00000530: 6020 6d65 7468 6f64 206f 6e6c 792a 2a0a  ` method only**.
+00000540: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+00000550: 7468 6572 206f 7220 6e6f 7420 746f 2061  ther or not to a
+00000560: 7574 6f2d 6765 6e65 7265 6174 6520 6120  uto-genereate a 
+00000570: 6e61 6d65 7461 6720 6046 7265 6542 5344  nametag `FreeBSD
+00000580: 2d3c 7665 7273 696f 6e3e 3a6c 6174 6573  -<version>:lates
+00000590: 7460 2062 6173 6564 206f 6e20 6075 6e61  t` based on `una
+000005a0: 6d65 2831 2960 2e0a 2020 2020 2020 2020  me(1)`..        
+000005b0: 2020 2020 4f76 6572 7269 6465 7320 6074      Overrides `t
+000005c0: 6167 6020 6966 2073 6574 2074 6f20 6074  ag` if set to `t
+000005d0: 7275 6560 2e0a 2020 2020 2020 2020 646e  rue`..        dn
+000005e0: 7320 2855 6e69 6f6e 5b55 6e73 6574 2c20  s (Union[Unset, 
+000005f0: 626f 6f6c 5d29 3a20 5768 6574 6865 7220  bool]): Whether 
+00000600: 6f72 206e 6f74 2074 6f20 636f 7079 2060  or not to copy `
+00000610: 2f65 7463 2f72 6573 6f6c 762e 636f 6e66  /etc/resolv.conf
+00000620: 6020 6672 6f6d 2074 6865 2068 6f73 7420  ` from the host 
+00000630: 746f 2074 6865 206e 6577 2069 6d61 6765  to the new image
+00000640: 2e20 4465 6661 756c 743a 0a20 2020 2020  . Default:.     
+00000650: 2020 2020 2020 2054 7275 652e 0a20 2020         True..   
+00000660: 2020 2020 206c 6f63 616c 7469 6d65 2028       localtime (
+00000670: 556e 696f 6e5b 556e 7365 742c 2062 6f6f  Union[Unset, boo
+00000680: 6c5d 293a 2057 6865 7468 6572 206f 7220  l]): Whether or 
+00000690: 6e6f 7420 746f 2063 6f70 7920 602f 6574  not to copy `/et
+000006a0: 632f 6c6f 6361 6c74 696d 6560 2066 726f  c/localtime` fro
+000006b0: 6d20 7468 6520 686f 7374 2074 6f20 7468  m the host to th
+000006c0: 6520 6e65 7720 696d 6167 652c 2069 6620  e new image, if 
+000006d0: 6974 0a20 2020 2020 2020 2020 2020 2065  it.            e
+000006e0: 7869 7374 732e 2044 6566 6175 6c74 3a20  xists. Default: 
+000006f0: 5472 7565 2e0a 2020 2020 2020 2020 7461  True..        ta
+00000700: 6720 2855 6e69 6f6e 5b55 6e73 6574 2c20  g (Union[Unset, 
+00000710: 7374 725d 293a 204e 616d 6520 616e 6420  str]): Name and 
+00000720: 6f70 7469 6f6e 616c 6c79 2061 2074 6167  optionally a tag
+00000730: 2069 6e20 7468 6520 606e 616d 653a 7461   in the `name:ta
+00000740: 6760 2066 6f72 6d61 742e 2049 6620 6074  g` format. If `t
+00000750: 6167 6020 6973 206f 6d69 7474 6564 2c20  ag` is omitted, 
+00000760: 7468 6520 6465 6661 756c 740a 2020 2020  the default.    
+00000770: 2020 2020 2020 2020 7661 6c75 6520 606c          value `l
+00000780: 6174 6573 7460 2069 7320 7573 6564 2e0a  atest` is used..
+00000790: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+000007a0: 6175 6c74 3a20 2727 2e0a 2020 2020 2020  ault: ''..      
+000007b0: 2020 7570 6461 7465 2028 556e 696f 6e5b    update (Union[
+000007c0: 556e 7365 742c 2062 6f6f 6c5d 293a 2055  Unset, bool]): U
+000007d0: 7064 6174 6520 7468 6520 6261 7365 2069  pdate the base i
+000007e0: 6d61 6765 2074 6f20 7468 6520 6c61 7374  mage to the last
+000007f0: 6573 7420 7061 7463 682d 6c65 7665 6c20  est patch-level 
+00000800: 7573 696e 6720 6066 7265 6562 7364 2d75  using `freebsd-u
+00000810: 7064 6174 6528 3829 602e 0a20 2020 2020  pdate(8)`..     
+00000820: 2020 2020 2020 2053 6565 2074 6865 205b         See the [
+00000830: 6d61 6e2d 7061 6765 735d 2868 7474 7073  man-pages](https
+00000840: 3a2f 2f6d 616e 2e66 7265 6562 7364 2e6f  ://man.freebsd.o
+00000850: 7267 2f63 6769 2f6d 616e 2e63 6769 3f71  rg/cgi/man.cgi?q
+00000860: 7565 7279 3d66 7265 6562 7364 2d75 7064  uery=freebsd-upd
+00000870: 6174 6529 2066 6f72 2064 6574 6169 6c73  ate) for details
+00000880: 2061 626f 7574 2077 6869 6368 2046 7265   about which Fre
+00000890: 6542 5344 0a20 2020 2020 2020 2020 2020  eBSD.           
+000008a0: 2076 6572 7369 6f6e 7320 6361 6e20 6265   versions can be
+000008b0: 2075 7064 6174 6564 2e22 2c0a 2020 2020   updated.",.    
+000008c0: 2020 2020 7572 6c20 2855 6e69 6f6e 5b55      url (Union[U
+000008d0: 6e73 6574 2c20 7374 725d 293a 202a 2a60  nset, str]): **`
+000008e0: 6665 7463 6860 206d 6574 686f 6420 6f6e  fetch` method on
+000008f0: 6c79 2a2a 0a0a 2020 2020 2020 2020 2020  ly**..          
+00000900: 2020 5552 4c20 746f 2074 6865 2062 6173    URL to the bas
+00000910: 6520 7379 7374 656d 2028 6120 6062 6173  e system (a `bas
+00000920: 652e 7478 7a60 2066 696c 6529 2074 6861  e.txz` file) tha
+00000930: 7420 4b6c 6565 6e65 6420 7368 6f75 6c64  t Kleened should
+00000940: 2075 7365 2074 6f20 6372 6561 7465 2074   use to create t
+00000950: 6865 2062 6173 6520 696d 6167 652e 0a20  he base image.. 
+00000960: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00000970: 756c 743a 2027 272e 0a20 2020 2020 2020  ult: ''..       
+00000980: 207a 6673 5f64 6174 6173 6574 2028 556e   zfs_dataset (Un
+00000990: 696f 6e5b 556e 7365 742c 2073 7472 5d29  ion[Unset, str])
+000009a0: 3a20 2a2a 607a 6673 2d2a 6020 6d65 7468  : **`zfs-*` meth
+000009b0: 6f64 7320 6f6e 6c79 2a2a 0a0a 2020 2020  ods only**..    
+000009c0: 2020 2020 2020 2020 5a46 5320 6461 7461          ZFS data
+000009d0: 7365 7420 7468 6174 2074 6865 2069 6d61  set that the ima
+000009e0: 6765 2073 686f 756c 6420 6265 2062 6173  ge should be bas
+000009f0: 6564 206f 6e2e 0a20 2020 2020 2020 2020  ed on..         
+00000a00: 2020 2020 4465 6661 756c 743a 2027 272e      Default: ''.
+00000a10: 0a20 2020 20da 066d 6574 686f 6446 da07  .    ..methodF..
+00000a20: 6175 746f 7461 6754 da03 646e 73da 096c  autotagT..dns..l
+00000a30: 6f63 616c 7469 6d65 da00 da03 7461 67da  ocaltime....tag.
+00000a40: 0675 7064 6174 65da 0375 726c da0b 7a66  .update..url..zf
+00000a50: 735f 6461 7461 7365 7429 02da 0469 6e69  s_dataset)...ini
+00000a60: 74da 0766 6163 746f 7279 da15 6164 6469  t..factory..addi
+00000a70: 7469 6f6e 616c 5f70 726f 7065 7274 6965  tional_propertie
+00000a80: 7329 01da 0672 6574 7572 6e63 0100 0000  s)...returnc....
+00000a90: 0000 0000 0000 0000 0a00 0000 0400 0000  ................
+00000aa0: 4300 0000 73c4 0000 007c 006a 006a 017d  C...s....|.j.j.}
+00000ab0: 017c 006a 027d 027c 006a 037d 037c 006a  .|.j.}.|.j.}.|.j
+00000ac0: 047d 047c 006a 057d 057c 006a 067d 067c  .}.|.j.}.|.j.}.|
+00000ad0: 006a 077d 077c 006a 087d 0869 007d 097c  .j.}.|.j.}.i.}.|
+00000ae0: 09a0 067c 006a 09a1 0101 007c 09a0 0664  ...|.j.....|...d
+00000af0: 017c 0169 01a1 0101 007c 0274 0a75 0172  .|.i.....|.t.u.r
+00000b00: 607c 027c 0964 023c 007c 0374 0a75 0172  `|.|.d.<.|.t.u.r
+00000b10: 707c 037c 0964 033c 007c 0474 0a75 0172  p|.|.d.<.|.t.u.r
+00000b20: 807c 047c 0964 043c 007c 0574 0a75 0172  .|.|.d.<.|.t.u.r
+00000b30: 907c 057c 0964 053c 007c 0674 0a75 0172  .|.|.d.<.|.t.u.r
+00000b40: a07c 067c 0964 063c 007c 0774 0a75 0172  .|.|.d.<.|.t.u.r
+00000b50: b07c 077c 0964 073c 007c 0874 0a75 0172  .|.|.d.<.|.t.u.r
+00000b60: c07c 087c 0964 083c 007c 0953 0029 094e  .|.|.d.<.|.S.).N
+00000b70: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000b80: 1400 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00000b90: 0000 0072 1900 0000 290b 7211 0000 00da  ...r....).r.....
+00000ba0: 0576 616c 7565 7212 0000 0072 1300 0000  .valuer....r....
+00000bb0: 7214 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000bc0: 1800 0000 7219 0000 0072 1c00 0000 720c  ....r....r....r.
+00000bd0: 0000 0029 0ada 0473 656c 6672 1100 0000  ...)...selfr....
+00000be0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000bf0: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
+00000c00: 0000 00da 0a66 6965 6c64 5f64 6963 74a9  .....field_dict.
+00000c10: 0072 2100 0000 fa37 2f76 6167 7261 6e74  .r!....7/vagrant
+00000c20: 2f6b 6c65 652f 6b6c 6565 2f63 6c69 656e  /klee/klee/clien
+00000c30: 742f 6d6f 6465 6c73 2f69 6d61 6765 5f63  t/models/image_c
+00000c40: 7265 6174 655f 636f 6e66 6967 2e70 79da  reate_config.py.
+00000c50: 0774 6f5f 6469 6374 3a00 0000 733a 0000  .to_dict:...s:..
+00000c60: 0000 0108 0206 0106 0106 0106 0106 0106  ................
+00000c70: 0106 0204 010c 0104 0204 ff02 ff04 0508  ................
+00000c80: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00000c90: 0108 0108 0108 0108 0108 027a 1949 6d61  ...........z.Ima
+00000ca0: 6765 4372 6561 7465 436f 6e66 6967 2e74  geCreateConfig.t
+00000cb0: 6f5f 6469 6374 2903 da03 636c 73da 0873  o_dict)...cls..s
+00000cc0: 7263 5f64 6963 7472 1d00 0000 6302 0000  rc_dictr....c...
+00000cd0: 0000 0000 0000 0000 000c 0000 000a 0000  ................
+00000ce0: 0043 0000 0073 8c00 0000 7c01 a000 a100  .C...s....|.....
+00000cf0: 7d02 7401 7c02 a002 6401 a101 8301 7d03  }.t.|...d.....}.
+00000d00: 7c02 a002 6402 7403 a102 7d04 7c02 a002  |...d.t...}.|...
+00000d10: 6403 7403 a102 7d05 7c02 a002 6404 7403  d.t...}.|...d.t.
+00000d20: a102 7d06 7c02 a002 6405 7403 a102 7d07  ..}.|...d.t...}.
+00000d30: 7c02 a002 6406 7403 a102 7d08 7c02 a002  |...d.t...}.|...
+00000d40: 6407 7403 a102 7d09 7c02 a002 6408 7403  d.t...}.|...d.t.
+00000d50: a102 7d0a 7c00 7c03 7c04 7c05 7c06 7c07  ..}.|.|.|.|.|.|.
+00000d60: 7c08 7c09 7c0a 6409 8d08 7d0b 7c02 7c0b  |.|.|.d...}.|.|.
+00000d70: 5f04 7c0b 5300 290a 4e72 1100 0000 7212  _.|.S.).Nr....r.
+00000d80: 0000 0072 1300 0000 7214 0000 0072 1600  ...r....r....r..
+00000d90: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000da0: 0029 0872 1100 0000 7212 0000 0072 1300  .).r....r....r..
+00000db0: 0000 7214 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000dc0: 0072 1800 0000 7219 0000 0029 05da 0463  .r....r....)...c
+00000dd0: 6f70 7972 0b00 0000 da03 706f 7072 0c00  opyr......popr..
+00000de0: 0000 721c 0000 0029 0c72 2400 0000 7225  ..r....).r$...r%
+00000df0: 0000 00da 0164 7211 0000 0072 1200 0000  .....dr....r....
+00000e00: 7213 0000 0072 1400 0000 7216 0000 0072  r....r....r....r
+00000e10: 1700 0000 7218 0000 0072 1900 0000 da13  ....r....r......
+00000e20: 696d 6167 655f 6372 6561 7465 5f63 6f6e  image_create_con
+00000e30: 6669 6772 2100 0000 7221 0000 0072 2200  figr!...r!...r".
+00000e40: 0000 da09 6672 6f6d 5f64 6963 745d 0000  ....from_dict]..
+00000e50: 0073 2a00 0000 0002 0801 0e02 0c02 0c02  .s*.............
+00000e60: 0c02 0c02 0c02 0c02 0c02 0201 0201 0201  ................
+00000e70: 0201 0201 0201 0201 0201 02f8 060b 0601  ................
+00000e80: 7a1b 496d 6167 6543 7265 6174 6543 6f6e  z.ImageCreateCon
+00000e90: 6669 672e 6672 6f6d 5f64 6963 7463 0100  fig.from_dictc..
+00000ea0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000eb0: 0000 4300 0000 730e 0000 0074 007c 006a  ..C...s....t.|.j
+00000ec0: 01a0 02a1 0083 0153 00a9 014e 2903 da04  .......S...N)...
+00000ed0: 6c69 7374 721c 0000 00da 046b 6579 7329  listr......keys)
+00000ee0: 0172 1f00 0000 7221 0000 0072 2100 0000  .r....r!...r!...
+00000ef0: 7222 0000 00da 0f61 6464 6974 696f 6e61  r".....additiona
+00000f00: 6c5f 6b65 7973 7e00 0000 7302 0000 0000  l_keys~...s.....
+00000f10: 027a 2149 6d61 6765 4372 6561 7465 436f  .z!ImageCreateCo
+00000f20: 6e66 6967 2e61 6464 6974 696f 6e61 6c5f  nfig.additional_
+00000f30: 6b65 7973 2902 da03 6b65 7972 1d00 0000  keys)...keyr....
+00000f40: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000f50: 0002 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
+00000f60: 6a00 7c01 1900 5300 722b 0000 00a9 0172  j.|...S.r+.....r
+00000f70: 1c00 0000 a902 721f 0000 0072 2f00 0000  ......r....r/...
+00000f80: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
+00000f90: 0b5f 5f67 6574 6974 656d 5f5f 8200 0000  .__getitem__....
+00000fa0: 7302 0000 0000 017a 1d49 6d61 6765 4372  s......z.ImageCr
+00000fb0: 6561 7465 436f 6e66 6967 2e5f 5f67 6574  eateConfig.__get
+00000fc0: 6974 656d 5f5f 4e29 0372 2f00 0000 721e  item__N).r/...r.
+00000fd0: 0000 0072 1d00 0000 6303 0000 0000 0000  ...r....c.......
+00000fe0: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+00000ff0: 0073 0e00 0000 7c02 7c00 6a00 7c01 3c00  .s....|.|.j.|.<.
+00001000: 6400 5300 722b 0000 0072 3000 0000 2903  d.S.r+...r0...).
+00001010: 721f 0000 0072 2f00 0000 721e 0000 0072  r....r/...r....r
+00001020: 2100 0000 7221 0000 0072 2200 0000 da0b  !...r!...r".....
+00001030: 5f5f 7365 7469 7465 6d5f 5f85 0000 0073  __setitem__....s
+00001040: 0200 0000 0001 7a1d 496d 6167 6543 7265  ......z.ImageCre
+00001050: 6174 6543 6f6e 6669 672e 5f5f 7365 7469  ateConfig.__seti
+00001060: 7465 6d5f 5f63 0200 0000 0000 0000 0000  tem__c..........
+00001070: 0000 0200 0000 0200 0000 4300 0000 730c  ..........C...s.
+00001080: 0000 007c 006a 007c 013d 0064 0053 0072  ...|.j.|.=.d.S.r
+00001090: 2b00 0000 7230 0000 0072 3100 0000 7221  +...r0...r1...r!
+000010a0: 0000 0072 2100 0000 7222 0000 00da 0b5f  ...r!...r"....._
+000010b0: 5f64 656c 6974 656d 5f5f 8800 0000 7302  _delitem__....s.
+000010c0: 0000 0000 017a 1d49 6d61 6765 4372 6561  .....z.ImageCrea
+000010d0: 7465 436f 6e66 6967 2e5f 5f64 656c 6974  teConfig.__delit
+000010e0: 656d 5f5f 6302 0000 0000 0000 0000 0000  em__c...........
+000010f0: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00001100: 0000 7c01 7c00 6a00 7600 5300 722b 0000  ..|.|.j.v.S.r+..
+00001110: 0072 3000 0000 7231 0000 0072 2100 0000  .r0...r1...r!...
+00001120: 7221 0000 0072 2200 0000 da0c 5f5f 636f  r!...r".....__co
+00001130: 6e74 6169 6e73 5f5f 8b00 0000 7302 0000  ntains__....s...
+00001140: 0000 017a 1e49 6d61 6765 4372 6561 7465  ...z.ImageCreate
+00001150: 436f 6e66 6967 2e5f 5f63 6f6e 7461 696e  Config.__contain
+00001160: 735f 5f29 22da 085f 5f6e 616d 655f 5fda  s__)"..__name__.
+00001170: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00001180: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00001190: 5f5f 720b 0000 00da 0f5f 5f61 6e6e 6f74  __r......__annot
+000011a0: 6174 696f 6e73 5f5f 7212 0000 0072 0700  ations__r....r..
+000011b0: 0000 720d 0000 00da 0462 6f6f 6c72 1300  ..r......boolr..
+000011c0: 0000 7214 0000 0072 1600 0000 da03 7374  ..r....r......st
+000011d0: 7272 1700 0000 7218 0000 0072 1900 0000  rr....r....r....
+000011e0: da0c 5f61 7474 7273 5f66 6965 6c64 da04  .._attrs_field..
+000011f0: 6469 6374 721c 0000 0072 0300 0000 7202  dictr....r....r.
+00001200: 0000 0072 2300 0000 da0b 636c 6173 736d  ...r#.....classm
+00001210: 6574 686f 6472 0500 0000 720e 0000 0072  ethodr....r....r
+00001220: 2a00 0000 da08 7072 6f70 6572 7479 7204  *.....propertyr.
+00001230: 0000 0072 2e00 0000 7232 0000 0072 3300  ...r....r2...r3.
+00001240: 0000 7234 0000 0072 3500 0000 7221 0000  ..r4...r5...r!..
+00001250: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00001260: 720f 0000 000c 0000 0073 2600 0000 0a02  r........s&.....
+00001270: 0422 0801 1401 1401 1401 1401 1401 1401  ."..............
+00001280: 1401 1c02 1623 0201 2020 0201 1403 1003  .....#..  ......
+00001290: 1203 1003 4e29 13da 0674 7970 696e 6772  ....N)...typingr
+000012a0: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
+000012b0: 0000 0072 0600 0000 7207 0000 00da 0561  ...r....r......a
+000012c0: 7474 7273 7208 0000 00da 0d5f 6174 7472  ttrsr......_attr
+000012d0: 735f 6465 6669 6e65 7209 0000 0072 3d00  s_definer....r=.
+000012e0: 0000 5a21 6d6f 6465 6c73 2e69 6d61 6765  ..Z!models.image
+000012f0: 5f63 7265 6174 655f 636f 6e66 6967 5f6d  _create_config_m
+00001300: 6574 686f 6472 0b00 0000 da05 7479 7065  ethodr......type
+00001310: 7372 0c00 0000 720d 0000 0072 0e00 0000  sr....r....r....
+00001320: 720f 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+00001330: 2100 0000 7222 0000 00da 083c 6d6f 6475  !...r".....<modu
+00001340: 6c65 3e01 0000 0073 0e00 0000 2002 0c01  le>....s.... ...
+00001350: 0c02 0c01 1002 0c03 0201                 ..........
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/image_create_config_method.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/image_create_config_method.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:39 2024 UTC, .py size: 232 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1fb1 1d66 e800 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 46fe 3166 e800 0000  a.......F.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 732a 0000 0065 005a  ....@...s*...e.Z
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/mount_point.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/mount_point.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 3638 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 360e 0000  a.......%..f6...
+00000000: 610d 0d0a 0000 0000 4cfe 3166 360e 0000  a.......L.1f6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6404 6406 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/mount_point_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/mount_point_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 3376 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 300d 0000  a.......%..f0...
+00000000: 610d 0d0a 0000 0000 4cfe 3166 300d 0000  a.......L.1f0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6404 6406 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/mount_point_config_type.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/mount_point_config_type.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:37 2024 UTC, .py size: 169 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1db1 1d66 a900 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 45fe 3166 a900 0000  a.......E.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 7322 0000 0065 005a  ....@...s"...e.Z
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/mount_point_type.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/published_port_config_protocol.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:37 2024 UTC, .py size: 163 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-00000000: 610d 0d0a 0000 0000 1db1 1d66 a300 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 45fe 3166 a400 0000  a.......E.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 7322 0000 0065 005a  ....@...s"...e.Z
 00000080: 0164 005a 0264 015a 0364 025a 0465 0564  .d.Z.d.Z.d.Z.e.d
 00000090: 039c 0164 0464 0584 045a 0664 0653 0029  ...d.d...Z.d.S.)
-000000a0: 07da 0e4d 6f75 6e74 506f 696e 7454 7970  ...MountPointTyp
-000000b0: 655a 066e 756c 6c66 73da 0676 6f6c 756d  eZ.nullfs..volum
-000000c0: 6529 01da 0672 6574 7572 6e63 0100 0000  e)...returnc....
-000000d0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000000e0: 4300 0000 730a 0000 0074 007c 006a 0183  C...s....t.|.j..
-000000f0: 0153 0029 014e 2902 da03 7374 72da 0576  .S.).N)...str..v
-00000100: 616c 7565 2901 da04 7365 6c66 a900 7209  alue)...self..r.
-00000110: 0000 00fa 342f 7661 6772 616e 742f 6b6c  ....4/vagrant/kl
-00000120: 6565 2f6b 6c65 652f 636c 6965 6e74 2f6d  ee/klee/client/m
-00000130: 6f64 656c 732f 6d6f 756e 745f 706f 696e  odels/mount_poin
-00000140: 745f 7479 7065 2e70 79da 075f 5f73 7472  t_type.py..__str
-00000150: 5f5f 0800 0000 7302 0000 0000 017a 164d  __....s......z.M
-00000160: 6f75 6e74 506f 696e 7454 7970 652e 5f5f  ountPointType.__
-00000170: 7374 725f 5f4e 2907 da08 5f5f 6e61 6d65  str__N)...__name
-00000180: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000190: 5f5f 7175 616c 6e61 6d65 5f5f 5a06 4e55  __qualname__Z.NU
-000001a0: 4c4c 4653 5a06 564f 4c55 4d45 7206 0000  LLFSZ.VOLUMEr...
-000001b0: 0072 0b00 0000 7209 0000 0072 0900 0000  .r....r....r....
-000001c0: 7209 0000 0072 0a00 0000 7203 0000 0004  r....r....r.....
-000001d0: 0000 0073 0600 0000 0801 0401 0402 7203  ...s..........r.
-000001e0: 0000 004e 2904 da04 656e 756d 7202 0000  ...N)...enumr...
-000001f0: 0072 0600 0000 7203 0000 0072 0900 0000  .r....r....r....
-00000200: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
-00000210: 083c 6d6f 6475 6c65 3e01 0000 0073 0200  .<module>....s..
-00000220: 0000 0c03                                ....
+000000a0: 07da 1b50 7562 6c69 7368 6564 506f 7274  ...PublishedPort
+000000b0: 436f 6e66 6967 5072 6f74 6f63 6f6c da03  ConfigProtocol..
+000000c0: 7463 70da 0375 6470 2901 da06 7265 7475  tcp..udp)...retu
+000000d0: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
+000000e0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+000000f0: 7400 7c00 6a01 8301 5300 2901 4e29 02da  t.|.j...S.).N)..
+00000100: 0373 7472 da05 7661 6c75 6529 01da 0473  .str..value)...s
+00000110: 656c 66a9 0072 0a00 0000 fa42 2f76 6167  elf..r.....B/vag
+00000120: 7261 6e74 2f6b 6c65 652f 6b6c 6565 2f63  rant/klee/klee/c
+00000130: 6c69 656e 742f 6d6f 6465 6c73 2f70 7562  lient/models/pub
+00000140: 6c69 7368 6564 5f70 6f72 745f 636f 6e66  lished_port_conf
+00000150: 6967 5f70 726f 746f 636f 6c2e 7079 da07  ig_protocol.py..
+00000160: 5f5f 7374 725f 5f08 0000 0073 0200 0000  __str__....s....
+00000170: 0001 7a23 5075 626c 6973 6865 6450 6f72  ..z#PublishedPor
+00000180: 7443 6f6e 6669 6750 726f 746f 636f 6c2e  tConfigProtocol.
+00000190: 5f5f 7374 725f 5f4e 2907 da08 5f5f 6e61  __str__N)...__na
+000001a0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000001b0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da03  ..__qualname__..
+000001c0: 5443 50da 0355 4450 7207 0000 0072 0c00  TCP..UDPr....r..
+000001d0: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+000001e0: 0072 0b00 0000 7203 0000 0004 0000 0073  .r....r........s
+000001f0: 0600 0000 0801 0401 0402 7203 0000 004e  ..........r....N
+00000200: 2904 da04 656e 756d 7202 0000 0072 0700  )...enumr....r..
+00000210: 0000 7203 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+00000220: 0072 0a00 0000 720b 0000 00da 083c 6d6f  .r....r......<mo
+00000230: 6475 6c65 3e01 0000 0073 0200 0000 0c03  dule>....s......
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 5383 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 0715 0000  a.......%..f....
+00000000: 610d 0d0a 0000 0000 4cfe 3166 0715 0000  a.......L.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6404 6406 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 5500 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 7c15 0000  a.......%..f|...
+00000000: 610d 0d0a 0000 0000 4cfe 3166 7c15 0000  a.......L.1f|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6404 6406 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network_config_type.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network_config_type.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:38 2024 UTC, .py size: 192 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1eb1 1d66 c000 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 45fe 3166 c000 0000  a.......E.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 7326 0000 0065 005a  ....@...s&...e.Z
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network_inspect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network_inspect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 3109 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 250c 0000  a.......%..f%...
+00000000: 610d 0d0a 0000 0000 4cfe 3166 250c 0000  a.......L.1f%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c08 6d0b 5a0c 0100 6404 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 0100 6501 7268 6404  m.Z.m.Z...e.rhd.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/network_type.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/network_type.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:38 2024 UTC, .py size: 186 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-00000000: 610d 0d0a 0000 0000 1eb1 1d66 ba00 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 45fe 3166 ba00 0000  a.......E.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 7326 0000 0065 005a  ....@...s&...e.Z
 00000080: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
 00000090: 0565 0664 049c 0164 0564 0684 045a 0764  .e.d...d.d...Z.d
 000000a0: 0753 0029 08da 0b4e 6574 776f 726b 5479  .S.)...NetworkTy
-000000b0: 7065 5a06 6272 6964 6765 5a06 6375 7374  peZ.bridgeZ.cust
-000000c0: 6f6d 5a08 6c6f 6f70 6261 636b 2901 da06  omZ.loopback)...
+000000b0: 7065 5a06 6272 6964 6765 da06 6375 7374  peZ.bridge..cust
+000000c0: 6f6d da08 6c6f 6f70 6261 636b 2901 da06  om..loopback)...
 000000d0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
 000000e0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
 000000f0: 0a00 0000 7400 7c00 6a01 8301 5300 2901  ....t.|.j...S.).
 00000100: 4e29 02da 0373 7472 da05 7661 6c75 6529  N)...str..value)
-00000110: 01da 0473 656c 66a9 0072 0800 0000 fa30  ...self..r.....0
+00000110: 01da 0473 656c 66a9 0072 0a00 0000 fa30  ...self..r.....0
 00000120: 2f76 6167 7261 6e74 2f6b 6c65 652f 6b6c  /vagrant/klee/kl
 00000130: 6565 2f63 6c69 656e 742f 6d6f 6465 6c73  ee/client/models
 00000140: 2f6e 6574 776f 726b 5f74 7970 652e 7079  /network_type.py
 00000150: da07 5f5f 7374 725f 5f09 0000 0073 0200  ..__str__....s..
 00000160: 0000 0001 7a13 4e65 7477 6f72 6b54 7970  ....z.NetworkTyp
 00000170: 652e 5f5f 7374 725f 5f4e 2908 da08 5f5f  e.__str__N)...__
 00000180: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000190: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 000001a0: 5a06 4252 4944 4745 5a06 4355 5354 4f4d  Z.BRIDGEZ.CUSTOM
-000001b0: 5a08 4c4f 4f50 4241 434b 7205 0000 0072  Z.LOOPBACKr....r
-000001c0: 0a00 0000 7208 0000 0072 0800 0000 7208  ....r....r....r.
-000001d0: 0000 0072 0900 0000 7203 0000 0004 0000  ...r....r.......
+000001b0: 5a08 4c4f 4f50 4241 434b 7207 0000 0072  Z.LOOPBACKr....r
+000001c0: 0c00 0000 720a 0000 0072 0a00 0000 720a  ....r....r....r.
+000001d0: 0000 0072 0b00 0000 7203 0000 0004 0000  ...r....r.......
 000001e0: 0073 0800 0000 0801 0401 0401 0402 7203  .s............r.
 000001f0: 0000 004e 2904 da04 656e 756d 7202 0000  ...N)...enumr...
-00000200: 0072 0500 0000 7203 0000 0072 0800 0000  .r....r....r....
-00000210: 7208 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
+00000200: 0072 0700 0000 7203 0000 0072 0a00 0000  .r....r....r....
+00000210: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
 00000220: 083c 6d6f 6475 6c65 3e01 0000 0073 0200  .<module>....s..
 00000230: 0000 0c03                                ....
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/published_port.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/published_port.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:45 2024 UTC, .py size: 3687 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 25b1 1d66 670e 0000  a.......%..fg...
+00000000: 610d 0d0a 0000 0000 4cfe 3166 670e 0000  a.......L.1fg...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6505 6406 6407 6408 8d02 5a0e 6509  ..e.d.d.d...Z.e.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/published_port_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/published_port_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:46 2024 UTC, .py size: 3729 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 26b1 1d66 910e 0000  a.......&..f....
+00000000: 610d 0d0a 0000 0000 4cfe 3166 910e 0000  a.......L.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c08 6d0b 5a0c 0100 6404 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0e 0100 6404 6406 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
@@ -151,15 +151,15 @@
 00000960: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
 00000970: 2904 7212 0000 0072 1300 0000 7214 0000  ).r....r....r...
 00000980: 0072 1500 0000 290a da04 636f 7079 da03  .r....)...copy..
 00000990: 706f 7072 0800 0000 7204 0000 00da 0373  popr....r......s
 000009a0: 7472 720d 0000 0072 1a00 0000 720e 0000  trr....r....r...
 000009b0: 0072 0c00 0000 7218 0000 0029 0972 2200  .r....r....).r".
 000009c0: 0000 7223 0000 00da 0164 7212 0000 0072  ..r#.....dr....r
-000009d0: 1300 0000 7214 0000 00da 095f 7072 6f74  ....r......_prot
+000009d0: 1300 0000 7214 0000 005a 095f 7072 6f74  ....r....Z._prot
 000009e0: 6f63 6f6c 7215 0000 00da 1570 7562 6c69  ocolr......publi
 000009f0: 7368 6564 5f70 6f72 745f 636f 6e66 6967  shed_port_config
 00000a00: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
 00000a10: 0966 726f 6d5f 6469 6374 4100 0000 7320  .from_dictA...s 
 00000a20: 0000 0000 0208 010a 020a 0214 020c 020a  ................
 00000a30: 0106 0208 0202 0102 0102 0102 0102 fc06  ................
 00000a40: 0706 017a 1d50 7562 6c69 7368 6564 506f  ...z.PublishedPo
@@ -173,69 +173,69 @@
 00000ac0: 7469 6f6e 616c 5f6b 6579 735b 0000 0073  tional_keys[...s
 00000ad0: 0200 0000 0002 7a23 5075 626c 6973 6865  ......z#Publishe
 00000ae0: 6450 6f72 7443 6f6e 6669 672e 6164 6469  dPortConfig.addi
 00000af0: 7469 6f6e 616c 5f6b 6579 7329 02da 036b  tional_keys)...k
 00000b00: 6579 7219 0000 0063 0200 0000 0000 0000  eyr....c........
 00000b10: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
 00000b20: 730a 0000 007c 006a 007c 0119 0053 0072  s....|.j.|...S.r
-00000b30: 2b00 0000 a901 7218 0000 00a9 0272 1d00  +.....r......r..
-00000b40: 0000 722f 0000 0072 1f00 0000 721f 0000  ..r/...r....r...
+00000b30: 2a00 0000 a901 7218 0000 00a9 0272 1d00  *.....r......r..
+00000b40: 0000 722e 0000 0072 1f00 0000 721f 0000  ..r....r....r...
 00000b50: 0072 2000 0000 da0b 5f5f 6765 7469 7465  .r .....__getite
 00000b60: 6d5f 5f5f 0000 0073 0200 0000 0001 7a1f  m___...s......z.
 00000b70: 5075 626c 6973 6865 6450 6f72 7443 6f6e  PublishedPortCon
 00000b80: 6669 672e 5f5f 6765 7469 7465 6d5f 5f4e  fig.__getitem__N
-00000b90: 2903 722f 0000 0072 1b00 0000 7219 0000  ).r/...r....r...
+00000b90: 2903 722e 0000 0072 1b00 0000 7219 0000  ).r....r....r...
 00000ba0: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
 00000bb0: 0000 0300 0000 4300 0000 730e 0000 007c  ......C...s....|
-00000bc0: 027c 006a 007c 013c 0064 0053 0072 2b00  .|.j.|.<.d.S.r+.
-00000bd0: 0000 7230 0000 0029 0372 1d00 0000 722f  ..r0...).r....r/
+00000bc0: 027c 006a 007c 013c 0064 0053 0072 2a00  .|.j.|.<.d.S.r*.
+00000bd0: 0000 722f 0000 0029 0372 1d00 0000 722e  ..r/...).r....r.
 00000be0: 0000 0072 1b00 0000 721f 0000 0072 1f00  ...r....r....r..
 00000bf0: 0000 7220 0000 00da 0b5f 5f73 6574 6974  ..r .....__setit
 00000c00: 656d 5f5f 6200 0000 7302 0000 0000 017a  em__b...s......z
 00000c10: 1f50 7562 6c69 7368 6564 506f 7274 436f  .PublishedPortCo
 00000c20: 6e66 6967 2e5f 5f73 6574 6974 656d 5f5f  nfig.__setitem__
 00000c30: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
 00000c40: 0002 0000 0043 0000 0073 0c00 0000 7c00  .....C...s....|.
-00000c50: 6a00 7c01 3d00 6400 5300 722b 0000 0072  j.|.=.d.S.r+...r
-00000c60: 3000 0000 7231 0000 0072 1f00 0000 721f  0...r1...r....r.
+00000c50: 6a00 7c01 3d00 6400 5300 722a 0000 0072  j.|.=.d.S.r*...r
+00000c60: 2f00 0000 7230 0000 0072 1f00 0000 721f  /...r0...r....r.
 00000c70: 0000 0072 2000 0000 da0b 5f5f 6465 6c69  ...r .....__deli
 00000c80: 7465 6d5f 5f65 0000 0073 0200 0000 0001  tem__e...s......
 00000c90: 7a1f 5075 626c 6973 6865 6450 6f72 7443  z.PublishedPortC
 00000ca0: 6f6e 6669 672e 5f5f 6465 6c69 7465 6d5f  onfig.__delitem_
 00000cb0: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
 00000cc0: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00000cd0: 017c 006a 0076 0053 0072 2b00 0000 7230  .|.j.v.S.r+...r0
-00000ce0: 0000 0072 3100 0000 721f 0000 0072 1f00  ...r1...r....r..
+00000cd0: 017c 006a 0076 0053 0072 2a00 0000 722f  .|.j.v.S.r*...r/
+00000ce0: 0000 0072 3000 0000 721f 0000 0072 1f00  ...r0...r....r..
 00000cf0: 0000 7220 0000 00da 0c5f 5f63 6f6e 7461  ..r .....__conta
 00000d00: 696e 735f 5f68 0000 0073 0200 0000 0001  ins__h...s......
 00000d10: 7a20 5075 626c 6973 6865 6450 6f72 7443  z PublishedPortC
 00000d20: 6f6e 6669 672e 5f5f 636f 6e74 6169 6e73  onfig.__contains
 00000d30: 5f5f 291d da08 5f5f 6e61 6d65 5f5f da0a  __)...__name__..
 00000d40: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000d50: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
 00000d60: 5f72 2600 0000 da0f 5f5f 616e 6e6f 7461  _r&.....__annota
 00000d70: 7469 6f6e 735f 5f72 0400 0000 720c 0000  tions__r....r...
 00000d80: 00da 0354 4350 7215 0000 0072 0700 0000  ...TCPr....r....
 00000d90: 720e 0000 00da 0c5f 6174 7472 735f 6669  r......_attrs_fi
 00000da0: 656c 64da 0464 6963 7472 1800 0000 7203  eld..dictr....r.
 00000db0: 0000 0072 0200 0000 7221 0000 00da 0b63  ...r....r!.....c
 00000dc0: 6c61 7373 6d65 7468 6f64 7205 0000 0072  lassmethodr....r
-00000dd0: 0f00 0000 722a 0000 00da 0870 726f 7065  ....r*.....prope
-00000de0: 7274 7972 2e00 0000 7232 0000 0072 3300  rtyr....r2...r3.
-00000df0: 0000 7234 0000 00da 0462 6f6f 6c72 3500  ..r4.....boolr5.
+00000dd0: 0f00 0000 7229 0000 00da 0870 726f 7065  ....r).....prope
+00000de0: 7274 7972 2d00 0000 7231 0000 0072 3200  rtyr-...r1...r2.
+00000df0: 0000 7233 0000 00da 0462 6f6f 6c72 3400  ..r3.....boolr4.
 00000e00: 0000 721f 0000 0072 1f00 0000 721f 0000  ..r....r....r...
 00000e10: 0072 2000 0000 7210 0000 000c 0000 0073  .r ...r........s
 00000e20: 2000 0000 0a02 0414 0801 0801 0c02 04ff   ...............
 00000e30: 1203 1c02 1617 0201 2019 0201 1403 1003  ........ .......
 00000e40: 1203 1003 4e29 14da 0674 7970 696e 6772  ....N)...typingr
 00000e50: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
 00000e60: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
 00000e70: 0000 da05 6174 7472 7372 0900 0000 da0d  ....attrsr......
 00000e80: 5f61 7474 7273 5f64 6566 696e 6572 0a00  _attrs_definer..
-00000e90: 0000 723c 0000 005a 256d 6f64 656c 732e  ..r<...Z%models.
+00000e90: 0000 723b 0000 005a 256d 6f64 656c 732e  ..r;...Z%models.
 00000ea0: 7075 626c 6973 6865 645f 706f 7274 5f63  published_port_c
 00000eb0: 6f6e 6669 675f 7072 6f74 6f63 6f6c 720c  onfig_protocolr.
 00000ec0: 0000 00da 0574 7970 6573 720d 0000 0072  .....typesr....r
 00000ed0: 0e00 0000 720f 0000 0072 1000 0000 721f  ....r....r....r.
 00000ee0: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
 00000ef0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
 00000f00: 730e 0000 0024 020c 010c 020c 0110 020c  s....$..........
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/published_port_protocol.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/published_port_protocol.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:37 2024 UTC, .py size: 158 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1db1 1d66 9e00 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 45fe 3166 9e00 0000  a.......E.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 7322 0000 0065 005a  ....@...s"...e.Z
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/volume.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/volume.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:46 2024 UTC, .py size: 2431 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 26b1 1d66 7f09 0000  a.......&..f....
+00000000: 610d 0d0a 0000 0000 4cfe 3166 7f09 0000  a.......L.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 6d0e 5a0e 0100 6505 6406 6407 6408 8d02  m.Z...e.d.d.d...
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/volume_config.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/volume_config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:46 2024 UTC, .py size: 1463 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 26b1 1d66 b705 0000  a.......&..f....
+00000000: 610d 0d0a 0000 0000 4cfe 3166 b705 0000  a.......L.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6400 6403 6c06 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6505 6404 6405 6406 8d02 5a0b 6508  ..e.d.d.d...Z.e.
 00000070: 4700 6407 6405 8400 6405 8302 8301 5a0c  G.d.d...d.....Z.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/volume_inspect.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/volume_inspect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:46 2024 UTC, .py size: 2984 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 26b1 1d66 a80b 0000  a.......&..f....
+00000000: 610d 0d0a 0000 0000 4dfe 3166 a80b 0000  a.......M.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6403 6c08 6d0b 5a0c 0100 6404 6405 6c0d  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 0100 6501 7268 6404  m.Z.m.Z...e.rhd.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/web_socket_message.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/web_socket_message.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:46 2024 UTC, .py size: 2318 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 26b1 1d66 0e09 0000  a.......&..f....
+00000000: 610d 0d0a 0000 0000 4dfe 3166 0e09 0000  a.......M.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6400 6403 6c06 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6405 6c0b 6d0c 5a0c 0100 6505  ..d.d.l.m.Z...e.
 00000070: 6406 6407 6408 8d02 5a0d 6508 4700 6409  d.d.d...Z.e.G.d.
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/__pycache__/web_socket_message_msg_type.cpython-39.pyc` & `kleene_cli-0.1.0rc3/klee/client/models/__pycache__/web_socket_message_msg_type.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 15 22:58:38 2024 UTC, .py size: 198 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-00000000: 610d 0d0a 0000 0000 1eb1 1d66 c600 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 45fe 3166 c600 0000  a.......E.1f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 6501 8304 5a03 6404 5300  ..d.e.e...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0445 6e75 6d63  )......)...Enumc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0300 0000 4000 0000 7326 0000 0065 005a  ....@...s&...e.Z
 00000080: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
 00000090: 0565 0664 049c 0164 0564 0684 045a 0764  .e.d...d.d...Z.d
 000000a0: 0753 0029 08da 1757 6562 536f 636b 6574  .S.)...WebSocket
 000000b0: 4d65 7373 6167 654d 7367 5479 7065 da07  MessageMsgType..
-000000c0: 636c 6f73 696e 67da 0565 7272 6f72 da08  closing..error..
+000000c0: 636c 6f73 696e 67da 0565 7272 6f72 5a08  closing..errorZ.
 000000d0: 7374 6172 7469 6e67 2901 da06 7265 7475  starting)...retu
 000000e0: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
 000000f0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
 00000100: 7400 7c00 6a01 8301 5300 2901 4e29 02da  t.|.j...S.).N)..
 00000110: 0373 7472 da05 7661 6c75 6529 01da 0473  .str..value)...s
-00000120: 656c 66a9 0072 0b00 0000 fa3f 2f76 6167  elf..r.....?/vag
+00000120: 656c 66a9 0072 0a00 0000 fa3f 2f76 6167  elf..r.....?/vag
 00000130: 7261 6e74 2f6b 6c65 652f 6b6c 6565 2f63  rant/klee/klee/c
 00000140: 6c69 656e 742f 6d6f 6465 6c73 2f77 6562  lient/models/web
 00000150: 5f73 6f63 6b65 745f 6d65 7373 6167 655f  _socket_message_
 00000160: 6d73 675f 7479 7065 2e70 79da 075f 5f73  msg_type.py..__s
 00000170: 7472 5f5f 0900 0000 7302 0000 0000 017a  tr__....s......z
 00000180: 1f57 6562 536f 636b 6574 4d65 7373 6167  .WebSocketMessag
 00000190: 654d 7367 5479 7065 2e5f 5f73 7472 5f5f  eMsgType.__str__
 000001a0: 4e29 08da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
 000001b0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 000001c0: 6c6e 616d 655f 5f5a 0743 4c4f 5349 4e47  lname__Z.CLOSING
 000001d0: da05 4552 524f 525a 0853 5441 5254 494e  ..ERRORZ.STARTIN
-000001e0: 4772 0800 0000 720d 0000 0072 0b00 0000  Gr....r....r....
-000001f0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+000001e0: 4772 0700 0000 720c 0000 0072 0a00 0000  Gr....r....r....
+000001f0: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
 00000200: 0300 0000 0400 0000 7308 0000 0008 0104  ........s.......
 00000210: 0104 0104 0272 0300 0000 4e29 04da 0465  .....r....N)...e
-00000220: 6e75 6d72 0200 0000 7208 0000 0072 0300  numr....r....r..
-00000230: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00000240: 0072 0c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000220: 6e75 6d72 0200 0000 7207 0000 0072 0300  numr....r....r..
+00000230: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+00000240: 0072 0b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 00000250: 0100 0000 7302 0000 000c 03              ....s......
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/container.py` & `kleene_cli-0.1.0rc3/klee/client/models/container.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/container_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/container_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/container_inspect.py` & `kleene_cli-0.1.0rc3/klee/client/models/container_inspect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/container_summary.py` & `kleene_cli-0.1.0rc3/klee/client/models/container_summary.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/end_point.py` & `kleene_cli-0.1.0rc3/klee/client/models/end_point.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/end_point_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/end_point_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/error_response.py` & `kleene_cli-0.1.0rc3/klee/client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/exec_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/exec_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/exec_start_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/exec_start_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/id_response.py` & `kleene_cli-0.1.0rc3/klee/client/models/id_response.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/image.py` & `kleene_cli-0.1.0rc3/klee/client/models/image.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/image_build_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/image_build_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/image_build_config_buildargs.py` & `kleene_cli-0.1.0rc3/klee/client/models/image_build_config_buildargs.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/image_create_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/image_create_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,53 +23,47 @@
             - `zfs-clone`: Create the base image based on a clone of `zfs_dataset`.
         autotag (Union[Unset, bool]): **`fetch-auto` method only**
 
             Whether or not to auto-genereate a nametag `FreeBSD-<version>:latest` based on `uname(1)`.
             Overrides `tag` if set to `true`.
         dns (Union[Unset, bool]): Whether or not to copy `/etc/resolv.conf` from the host to the new image. Default:
             True.
-        force (Union[Unset, bool]): **`fetch-auto` method only**
-
-            Ignore any discrepancies in the output of `uname(1)` when determining the FreeBSD version.
-        localtime (Union[Unset, bool]): Whether or not to copy `/etc/localtime` from the host to the new image. Default:
-            True.
+        localtime (Union[Unset, bool]): Whether or not to copy `/etc/localtime` from the host to the new image, if it
+            exists. Default: True.
         tag (Union[Unset, str]): Name and optionally a tag in the `name:tag` format. If `tag` is omitted, the default
             value `latest` is used.
              Default: ''.
-        update (Union[Unset, bool]): Update the base image using `freebsd-update(8)`.
+        update (Union[Unset, bool]): Update the base image to the lastest patch-level using `freebsd-update(8)`.
             See the [man-pages](https://man.freebsd.org/cgi/man.cgi?query=freebsd-update) for details about which FreeBSD
             versions can be updated.",
-             Default: True.
         url (Union[Unset, str]): **`fetch` method only**
 
             URL to the base system (a `base.txz` file) that Kleened should use to create the base image.
              Default: ''.
         zfs_dataset (Union[Unset, str]): **`zfs-*` methods only**
 
             ZFS dataset that the image should be based on.
              Default: ''.
     """
 
     method: ImageCreateConfigMethod
     autotag: Union[Unset, bool] = False
     dns: Union[Unset, bool] = True
-    force: Union[Unset, bool] = False
     localtime: Union[Unset, bool] = True
     tag: Union[Unset, str] = ""
-    update: Union[Unset, bool] = True
+    update: Union[Unset, bool] = False
     url: Union[Unset, str] = ""
     zfs_dataset: Union[Unset, str] = ""
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         method = self.method.value
 
         autotag = self.autotag
         dns = self.dns
-        force = self.force
         localtime = self.localtime
         tag = self.tag
         update = self.update
         url = self.url
         zfs_dataset = self.zfs_dataset
 
         field_dict: Dict[str, Any] = {}
@@ -79,16 +73,14 @@
                 "method": method,
             }
         )
         if autotag is not UNSET:
             field_dict["autotag"] = autotag
         if dns is not UNSET:
             field_dict["dns"] = dns
-        if force is not UNSET:
-            field_dict["force"] = force
         if localtime is not UNSET:
             field_dict["localtime"] = localtime
         if tag is not UNSET:
             field_dict["tag"] = tag
         if update is not UNSET:
             field_dict["update"] = update
         if url is not UNSET:
@@ -103,31 +95,28 @@
         d = src_dict.copy()
         method = ImageCreateConfigMethod(d.pop("method"))
 
         autotag = d.pop("autotag", UNSET)
 
         dns = d.pop("dns", UNSET)
 
-        force = d.pop("force", UNSET)
-
         localtime = d.pop("localtime", UNSET)
 
         tag = d.pop("tag", UNSET)
 
         update = d.pop("update", UNSET)
 
         url = d.pop("url", UNSET)
 
         zfs_dataset = d.pop("zfs_dataset", UNSET)
 
         image_create_config = cls(
             method=method,
             autotag=autotag,
             dns=dns,
-            force=force,
             localtime=localtime,
             tag=tag,
             update=update,
             url=url,
             zfs_dataset=zfs_dataset,
         )
```

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/mount_point.py` & `kleene_cli-0.1.0rc3/klee/client/models/mount_point.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/mount_point_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/mount_point_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/network.py` & `kleene_cli-0.1.0rc3/klee/client/models/network.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/network_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/network_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/network_inspect.py` & `kleene_cli-0.1.0rc3/klee/client/models/network_inspect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/published_port.py` & `kleene_cli-0.1.0rc3/klee/client/models/published_port.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/published_port_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/published_port_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/volume.py` & `kleene_cli-0.1.0rc3/klee/client/models/volume.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/volume_config.py` & `kleene_cli-0.1.0rc3/klee/client/models/volume_config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/volume_inspect.py` & `kleene_cli-0.1.0rc3/klee/client/models/volume_inspect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/models/web_socket_message.py` & `kleene_cli-0.1.0rc3/klee/client/models/web_socket_message.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/client/types.py` & `kleene_cli-0.1.0rc3/klee/client/types.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/config.py` & `kleene_cli-0.1.0rc3/klee/config.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/connection.py` & `kleene_cli-0.1.0rc3/klee/connection.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/container.py` & `kleene_cli-0.1.0rc3/klee/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,26 +406,28 @@
         click.Argument(["image"], nargs=1),
         click.Argument(["command"], nargs=-1),
     ]
     run.params.extend(opts_args)
     return run
 
 
-root.add_command(container_create("create"), name="create")
-root.add_command(container_list("ls"), name="ls")
-root.add_command(
-    inspect_command(
-        name="inspect",
+def container_inspect(name, hidden=False):
+    return inspect_command(
+        name=name,
+        hidden=hidden,
         argument="container",
         id_var="container_id",
         docs="Display detailed information on a container.",
         endpoint=container_inspect_endpoint,
-    ),
-    name="inspect",
-)
+    )
+
+
+root.add_command(container_create("create"), name="create")
+root.add_command(container_list("ls"), name="ls")
+root.add_command(container_inspect("inspect"), name="inspect")
 root.add_command(container_remove("rm"), name="rm")
 root.add_command(
     prune_command(
         name="prune",
         docs="Remove all stopped containers.",
         warning="WARNING! This will remove all stopped containers.",
         endpoint=container_prune_endpoint,
```

### Comparing `kleene_cli-0.1.0rc2/klee/custom_client_templates/endpoint_module.py.jinja` & `kleene_cli-0.1.0rc3/klee/custom_client_templates/endpoint_module.py.jinja`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/docs_generator.py` & `kleene_cli-0.1.0rc3/klee/docs_generator.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/image.py` & `kleene_cli-0.1.0rc3/klee/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,46 +93,38 @@
         "--update/--no-update",
         default=False,
         show_default=True,
         metavar="bool",
         help="Update the userland using freebsd-update(8). See the freebsd-update man-page for details on which FreeBSD versions can be updated.",
     )
     @click.option(
-        "--force",
-        "-f",
-        is_flag=True,
-        default=False,
-        metavar="flag",
-        help="Proceed using a userland from a FreeBSD mirror even if a customized build is detected on the host. Method **fetch-auto** only.",
-    )
-    @click.option(
         "--autotag/--no-autotag",
         "-a",
         is_flag=True,
         default=True,
         show_default=True,
         metavar="bool",
         help="Autogenerate a nametag 'FreeBSD-\<version\>:latest'. If `tag` is set this is ignored. Method **fetch-auto** only.",
     )
     @click.argument("method", nargs=1)
     @click.argument("source", nargs=-1)
-    def create(tag, dns, localtime, update, force, autotag, method, source):
+    def create(tag, dns, localtime, update, autotag, method, source):
         """
         Create a base image from a tar-archive or a ZFS dataset.
 
         **METHOD** can be one of the following:
 
         - **fetch-auto**: Automatically fetch a release/snapshot from the offical FreeBSD
           mirrors, based on host information from uname(1). **SOURCE** is not used.
         - **fetch**: Fetch a custom version of the base system and use it for image creation.
           **SOURCE** is a valid url for fetch(1), pointing to a base.txz file locally or remote.
         - **zfs-copy**: Create a base image from a copy of an existing ZFS dataset. **SOURCE** is the dataset.
         - **zfs-clone**: Create a base image from a clone of an existing ZFS dataset. **SOURCE** is the dataset.
         """
-        _create(tag, dns, localtime, update, force, autotag, method, source)
+        _create(tag, dns, localtime, update, autotag, method, source)
 
     return create
 
 
 def image_build(name, hidden=False):
     @click.command(
         cls=command_cls(),
@@ -292,33 +284,35 @@
                 500: print_backend_error,
             },
         )
 
     return tag
 
 
-root.add_command(image_create("create"), name="create")
-root.add_command(image_build("build"), name="build")
-root.add_command(image_list("ls"), name="ls")
-root.add_command(
-    inspect_command(
-        name="inspect",
+def image_inspect(name, hidden=False):
+    return inspect_command(
+        name=name,
+        hidden=hidden,
         argument="image",
         id_var="image_id",
         docs="Display detailed information on an image",
         endpoint=image_inspect_endpoint,
-    ),
-    name="inspect",
-)
+    )
+
+
+root.add_command(image_create("create"), name="create")
+root.add_command(image_build("build"), name="build")
+root.add_command(image_list("ls"), name="ls")
+root.add_command(image_inspect("inspect"), name="inspect")
 root.add_command(image_remove("rm"), name="rm")
 root.add_command(image_prune("prune"), name="prune")
 root.add_command(image_tag("tag"), name="tag")
 
 
-def _create(tag, dns, localtime, update, force, autotag, method, source):
+def _create(tag, dns, localtime, update, autotag, method, source):
     dataset = ""
     url = ""
 
     if len(source) > 1:
         additional_arguments = " ".join(source[1:])
         echo_error(f"too many arguments: {additional_arguments}")
         return
@@ -338,15 +332,14 @@
         "method": method,
         "url": url,
         "zfs_dataset": dataset,
         "tag": tag,
         "dns": dns,
         "localtime": localtime,
         "update": update,
-        "force": force,
         "autotag": autotag,
     }
     config_json = json.dumps(config)
     asyncio.run(_create_image_and_listen_for_messages(config_json))
 
 
 async def _create_image_and_listen_for_messages(config_json):
```

### Comparing `kleene_cli-0.1.0rc2/klee/inspect.py` & `kleene_cli-0.1.0rc3/klee/inspect.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/name_generator.py` & `kleene_cli-0.1.0rc3/klee/name_generator.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/network.py` & `kleene_cli-0.1.0rc3/klee/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import click
 
-from .client.api.default.network_connect import sync_detailed as network_connect
-from .client.api.default.network_create import sync_detailed as network_create
-from .client.api.default.network_disconnect import sync_detailed as network_disconnect
+from .client.api.default.network_create import sync_detailed as network_create_endpoint
+from .client.api.default.network_connect import (
+    sync_detailed as network_connect_endpoint,
+)
+from .client.api.default.network_disconnect import (
+    sync_detailed as network_disconnect_endpoint,
+)
 from .client.api.default.network_list import sync_detailed as network_list_endpoint
 from .client.api.default.network_inspect import (
     sync_detailed as network_inspect_endpoint,
 )
-from .client.api.default.network_remove import sync_detailed as network_remove
+from .client.api.default.network_remove import sync_detailed as network_remove_endpoint
 from .client.api.default.network_prune import sync_detailed as network_prune_endpoint
 
 from .client.models.end_point_config import EndPointConfig
 from .client.models.network_config import NetworkConfig
 
 from .printing import (
     print_table,
@@ -35,191 +39,209 @@
 
 # pylint: disable=unused-argument
 @click.group(cls=group_cls(), add_help_option=True, short_help="Manage networks")
 def root(name="network"):
     """Manage networks"""
 
 
-@root.command(cls=command_cls(), name="create", no_args_is_help=True)
-@click.option(
-    "--type",
-    "-t",
-    default="loopback",
-    show_default=True,
-    help="What kind of network should be created. Possible values are 'bridge', 'loopback', and 'custom'.",
-)
-@click.option(
-    "--interface",
-    "-i",
-    default="",
-    help="""
-    Name of the interface used on the host for the network.
-    If not set the interface name is set to 'kleened' postfixed with an integer.
-    If `type` is set to 'custom' the value of `interface` must be the name of an existing interface.
-  """,
-)
-@click.option("--subnet", default="", help="Subnet in CIDR format for the network")
-@click.option(
-    "--subnet6", default="", help="IPv6 subnet in CIDR format for the network"
-)
-@click.option(
-    "--gw",
-    default="auto",
-    help="""VNET+bridge only. The default IPv4 router that is added to 'vnet' containers on startup, if `subnet` is set.
-    If set to 'auto' the first IP of `subnet` is added to the bridge and used as a gateway (default).
-    Setting `--gw=\"\"` disables adding a gateway.
-    """,
-)
-@click.option(
-    "--gw6",
-    default="auto",
-    help="""VNET+bridge only. The default IPv6 router that is added to 'vnet' containers, if `subnet6` is set.
-    See `gw` for details.
-    """,
-)
-@click.option(
-    "--nat",
-    default=True,
-    metavar="bool",
-    help="Whether or not to use NAT for the network's outgoing traffic. Default is to use NAT, use `--no-nat` to disable it.",
-)
-@click.option(
-    "--nat-if",
-    default=None,
-    metavar="string",
-    help="""
-    Specify which interface to NAT the IPv4 network traffic to.
-    Defaults to the host's gateway interface. Ignored if `no-nat` is set.
-    """,
-)
-@click.option(
-    "--icc",
-    default=True,
-    metavar="bool",
-    show_default=True,
-    help="Whether or not to enable connectivity between containers within the same network.",
-)
-@click.option(
-    "--internal",
-    default=False,
-    is_flag=True,
-    metavar="flag",
-    help="Whether or not the network is internal, i.e., not allowing outgoing upstream traffic",
-)
-@click.argument("name", nargs=1)
-def create(**config):
-    """Create a new network."""
-    config["gateway"] = config.pop("gw")
-    config["gateway6"] = config.pop("gw6")
-    for gw in ["gateway", "gateway6"]:
-        config[gw] = "<auto>" if config[gw] == "auto" else config[gw]
-
-    nat = config.pop("nat")
-    nat_interface = config.pop("nat_if")
-    if nat:
-        config["nat"] = "<host-gateway>" if nat_interface is None else nat_interface
-    else:
-        config["nat"] = ""
-
-    network_config = NetworkConfig.from_dict(config)
-
-    request_and_print_response(
-        network_create,
-        kwargs={"json_body": network_config},
-        statuscode2printer={
-            201: print_response_id,
-            409: print_response_msg,
-            500: print_backend_error,
-        },
+def network_create(name, hidden=False):
+    @root.command(cls=command_cls(), name=name, hidden=hidden, no_args_is_help=True)
+    @click.option(
+        "--type",
+        "-t",
+        default="loopback",
+        show_default=True,
+        help="What kind of network should be created. Possible values are 'bridge', 'loopback', and 'custom'.",
     )
+    @click.option(
+        "--interface",
+        "-i",
+        default="",
+        help="""
+        Name of the interface used on the host for the network.
+        If not set the interface name is set to 'kleened' postfixed with an integer.
+        If `type` is set to 'custom' the value of `interface` must be the name of an existing interface.
+      """,
+    )
+    @click.option("--subnet", default="", help="Subnet in CIDR format for the network")
+    @click.option(
+        "--subnet6", default="", help="IPv6 subnet in CIDR format for the network"
+    )
+    @click.option(
+        "--gw",
+        default="auto",
+        help="""VNET+bridge only. The default IPv4 router that is added to 'vnet' containers on startup, if `subnet` is set.
+        If set to 'auto' the first IP of `subnet` is added to the bridge and used as a gateway (default).
+        Setting `--gw=\"\"` disables adding a gateway.
+        """,
+    )
+    @click.option(
+        "--gw6",
+        default="auto",
+        help="""VNET+bridge only. The default IPv6 router that is added to 'vnet' containers, if `subnet6` is set.
+        See `gw` for details.
+        """,
+    )
+    @click.option(
+        "--nat",
+        default=True,
+        metavar="bool",
+        help="Whether or not to use NAT for the network's outgoing traffic. Default is to use NAT, use `--no-nat` to disable it.",
+    )
+    @click.option(
+        "--nat-if",
+        default=None,
+        metavar="string",
+        help="""
+        Specify which interface to NAT the IPv4 network traffic to.
+        Defaults to the host's gateway interface. Ignored if `no-nat` is set.
+        """,
+    )
+    @click.option(
+        "--icc",
+        default=True,
+        metavar="bool",
+        show_default=True,
+        help="Whether or not to enable connectivity between containers within the same network.",
+    )
+    @click.option(
+        "--internal",
+        default=False,
+        is_flag=True,
+        metavar="flag",
+        help="Whether or not the network is internal, i.e., not allowing outgoing upstream traffic",
+    )
+    @click.argument("name", nargs=1)
+    def create(**config):
+        """Create a new network."""
+        config["gateway"] = config.pop("gw")
+        config["gateway6"] = config.pop("gw6")
+        for gw in ["gateway", "gateway6"]:
+            config[gw] = "<auto>" if config[gw] == "auto" else config[gw]
+
+        nat = config.pop("nat")
+        nat_interface = config.pop("nat_if")
+        if nat:
+            config["nat"] = "<host-gateway>" if nat_interface is None else nat_interface
+        else:
+            config["nat"] = ""
 
+        network_config = NetworkConfig.from_dict(config)
 
-@root.command(cls=command_cls(), name="rm", no_args_is_help=True)
-@click.argument("networks", required=True, nargs=-1)
-def remove(networks):
-    """
-    Remove one or more networks. Any connected containers will be disconnected.
-    """
-    for network_id in networks:
-        response = request_and_print_response(
-            network_remove,
-            kwargs={"network_id": network_id},
+        request_and_print_response(
+            network_create_endpoint,
+            kwargs={"json_body": network_config},
             statuscode2printer={
-                200: print_response_id,
-                404: print_response_msg,
+                201: print_response_id,
+                409: print_response_msg,
                 500: print_backend_error,
             },
         )
-        if response is None or response.status_code != 200:
-            break
 
+    return create
 
-root.add_command(
-    prune_command(
-        name="prune",
-        docs="Remove all unused networks, i.e., networks without connected containers.",
-        warning="WARNING! This will remove all unused networks.",
-        endpoint=network_prune_endpoint,
-    )
-)
+
+def network_remove(name, hidden=False):
+    @click.command(cls=command_cls(), name=name, hidden=hidden, no_args_is_help=True)
+    @click.argument("networks", required=True, nargs=-1)
+    def remove(networks):
+        """
+        Remove one or more networks. Any connected containers will be disconnected.
+        """
+        for network_id in networks:
+            response = request_and_print_response(
+                network_remove_endpoint,
+                kwargs={"network_id": network_id},
+                statuscode2printer={
+                    200: print_response_id,
+                    404: print_response_msg,
+                    500: print_backend_error,
+                },
+            )
+            if response is None or response.status_code != 200:
+                break
+
+    return remove
 
 
 def network_list(name, hidden=False):
     def _print_networks(response):
         networks = [[nw.id, nw.name, nw.type, nw.subnet] for nw in response.parsed]
         print_table(networks, NETWORK_LIST_COLUMNS)
 
-    @root.command(cls=command_cls(), name=name, hidden=hidden)
+    @click.command(cls=command_cls(), name=name, hidden=hidden)
     def listing():
         """List networks"""
         request_and_print_response(
             network_list_endpoint,
             kwargs={},
             statuscode2printer={200: _print_networks, 500: print_backend_error},
         )
 
     return listing
 
 
-root.add_command(network_list("ls"), name="ls")
-
-
-root.add_command(
-    inspect_command(
-        name="inspect",
+def network_inspect(name, hidden=False):
+    return inspect_command(
+        name=name,
+        hidden=hidden,
         argument="network",
         id_var="network_id",
         docs="Display detailed information on a network.",
         endpoint=network_inspect_endpoint,
-    ),
-    name="inspect",
-)
+    )
 
 
-@root.command(cls=command_cls(), name="connect", no_args_is_help=True)
-@click.option(
-    "--ip",
-    default=None,
-    help="IPv4 address used for the container. If omitted and a ipv4 subnet exists for **NETWORK**, an unused ip is allocated. Otherwise it is ignored.",
-)
-@click.option(
-    "--ip6",
-    default=None,
-    help="IPv6 address used for the container. If omitted and a ipv6 subnet exists for **NETWORK**, an unused ip is allocated. Otherwise it is ignored.",
-)
-@click.argument("network", required=True, nargs=1)
-@click.argument("container", required=True, nargs=1)
-def connect(ip, ip6, network, container):
-    """
-    Connect a container to a network.
-
-    **NETWORK** and **CONTAINER** are network and container identifiers, respectively.
-    Once connected, the container can communicate with other containers in the same network.
-    """
-    _connect(ip, ip6, network, container)
+def network_connect(name, hidden=False):
+    @click.command(cls=command_cls(), name=name, hidden=hidden, no_args_is_help=True)
+    @click.option(
+        "--ip",
+        default=None,
+        help="IPv4 address used for the container. If omitted and a ipv4 subnet exists for **NETWORK**, an unused ip is allocated. Otherwise it is ignored.",
+    )
+    @click.option(
+        "--ip6",
+        default=None,
+        help="IPv6 address used for the container. If omitted and a ipv6 subnet exists for **NETWORK**, an unused ip is allocated. Otherwise it is ignored.",
+    )
+    @click.argument("network", required=True, nargs=1)
+    @click.argument("container", required=True, nargs=1)
+    def connect(ip, ip6, network, container):
+        """
+        Connect a container to a network.
+
+        **NETWORK** and **CONTAINER** are network and container identifiers, respectively.
+        Once connected, the container can communicate with other containers in the same network.
+        """
+        _connect(ip, ip6, network, container)
+
+    return connect
+
+
+def network_disconnect(name, hidden=False):
+    @click.command(cls=command_cls(), name=name, hidden=hidden, no_args_is_help=True)
+    @click.argument("network", required=True, nargs=1)
+    @click.argument("container", required=True, nargs=1)
+    def disconnect(network, container):
+        """
+        Disconnect a container from a network.
+
+        Running containers can also be disconnected from a network.
+        """
+        request_and_print_response(
+            network_disconnect_endpoint,
+            kwargs={"network_id": network, "container_id": container},
+            statuscode2printer={
+                204: print_nothing,
+                404: print_response_msg,
+                500: print_backend_error,
+            },
+        )
+
+    return disconnect
 
 
 def _connect(ip, ip6, network, container):
     ip = "<auto>" if ip is None else ip
     ip6 = "<auto>" if ip6 is None else ip6
 
     if ip is not None:
@@ -233,36 +255,32 @@
         )
     else:
         endpoint_config = EndPointConfig.from_dict(
             {"network": network, "container": container}
         )
 
     return request_and_print_response(
-        network_connect,
+        network_connect_endpoint,
         kwargs={"json_body": endpoint_config},
         statuscode2printer={
             204: print_nothing,
             404: print_response_msg,
             409: print_response_msg,
             500: print_backend_error,
         },
     )
 
 
-@root.command(cls=command_cls(), name="disconnect", no_args_is_help=True)
-@click.argument("network", required=True, nargs=1)
-@click.argument("container", required=True, nargs=1)
-def disconnect(network, container):
-    """
-    Disconnect a container from a network.
-
-    Running containers can also be disconnected from a network.
-    """
-    request_and_print_response(
-        network_disconnect,
-        kwargs={"network_id": network, "container_id": container},
-        statuscode2printer={
-            204: print_nothing,
-            404: print_response_msg,
-            500: print_backend_error,
-        },
+root.add_command(network_create("create"), name="create")
+root.add_command(network_list("ls"), name="ls")
+root.add_command(network_inspect("inspect"), name="inspect")
+root.add_command(network_remove("rm"), name="rm")
+root.add_command(
+    prune_command(
+        name="prune",
+        docs="Remove all unused networks, i.e., networks without connected containers.",
+        warning="WARNING! This will remove all unused networks.",
+        endpoint=network_prune_endpoint,
     )
+)
+root.add_command(network_disconnect("disconnect"), name="disconnect")
+root.add_command(network_connect("connect"), name="connect")
```

### Comparing `kleene_cli-0.1.0rc2/klee/options.py` & `kleene_cli-0.1.0rc3/klee/options.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/printing.py` & `kleene_cli-0.1.0rc3/klee/printing.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,16 +145,16 @@
 
     console.print(table, soft_wrap=True)
 
 
 class RootGroup(click.Group):
     def format_options(self, ctx: Context, formatter: HelpFormatter) -> None:
         click.Command.format_options(self, ctx, formatter)
-        self.format_shortcuts(ctx, formatter)
         self.format_commands(ctx, formatter)
+        self.format_shortcuts(ctx, formatter)
 
     def format_shortcuts(self, ctx: Context, formatter: HelpFormatter) -> None:
         """Extra format methods for multi methods that adds all the commands
         after the options.
         """
         commands = []
         for subcommand in self.list_commands(ctx):
@@ -234,38 +234,50 @@
 
     if config.theme == THEME_DOCSGENERATOR:
         return DocsGroup
 
     raise Exception(f"cli theme '{config.theme}' not known")
 
 
+SINGLE_SHORTCUTS = {"build", "create", "exec", "restart", "start", "stop", "run"}
+
+
 def print_shortcuts_section(self):
     commands_table = Table(highlight=True, box=None, show_header=False)
 
     # commands = []
     for name, command in self.commands.items():
         # Hidden commands are the shortcuts
-        if command.hidden:
+        if command.hidden and command.name in SINGLE_SHORTCUTS:
             cmd_help = command.get_short_help_str(limit=200)
             commands_table.add_row(Text(name, style="bold yellow"), Markdown(cmd_help))
 
+    is_help = (
+        "Inspect an object, where X is [c]ontainer, [i]mage, [n]etwork, or [v]olume."
+    )
+    rm_help = "Remove one or more objects, where X is [c]ontainer, [i]mage, [n]etwork, or [v]olume."
+    ls_help = "List objects, where X is [c]ontainer, [i]mage, [n]etwork, or [v]olume."
+    commands_table.add_row(Text("isX", style="bold yellow"), Markdown(is_help))
+    commands_table.add_row(Text("rmX", style="bold yellow"), Markdown(rm_help))
+    commands_table.add_row(Text("lsX", style="bold yellow"), Markdown(ls_help))
     console.print(
         Panel(commands_table, border_style="dim", title="Shortcuts", title_align="left")
     )
 
 
 def print_commands_section(self, ctx):
     commands_table = Table(highlight=True, box=None, show_header=False)
 
     commands = []
     for subcommand in self.list_commands(ctx):
         cmd = self.get_command(ctx, subcommand)
         # What is this, the tool lied about a command.  Ignore it
         if cmd is None:
             continue
+
         if cmd.hidden:
             continue
 
         commands.append((subcommand, cmd))
 
     for subcommand, cmd in commands:
         cmd_help = Markdown(cmd.get_short_help_str(limit=200))
```

### Comparing `kleene_cli-0.1.0rc2/klee/prune.py` & `kleene_cli-0.1.0rc3/klee/prune.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/root.py` & `kleene_cli-0.1.0rc3/klee/root.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,43 +29,63 @@
     config.update_bootstrap_options(config_file, theme)
     config.load_config_file()
 
     from .container import (
         root as container_root,
         container_create,
         container_remove,
+        container_inspect,
         container_exec,
         container_list,
         container_start,
         container_stop,
         container_restart,
         container_run,
     )
 
     from .printing import root_cls
-    from .image import root as image_root, image_list, image_build, image_remove
-    from .network import root as network_root, network_list
-    from .volume import root as volume_root, volume_list
+    from .image import (
+        root as image_root,
+        image_list,
+        image_build,
+        image_remove,
+        image_inspect,
+    )
+    from .network import (
+        root as network_root,
+        network_list,
+        network_remove,
+        network_inspect,
+    )
+    from .volume import root as volume_root, volume_list, volume_remove, volume_inspect
     from .shortcuts import SHORTCUTS
 
     shortcuts2command_obj = {
+        # This is all the actual shortcuts.
+        # The 'Shortcuts' help section prints a compacted list. See 'printing.py' for details.
         # Format: <shortcut name>: <actual click command object>
         "build": image_build("build", hidden=True),
         "create": container_create("create", hidden=True),
         "exec": container_exec("exec", hidden=True),
+        "restart": container_restart("restart", hidden=True),
+        "start": container_start("start", hidden=True),
+        "stop": container_stop("stop", hidden=True),
+        "run": container_run("run", hidden=True),
+        "isc": container_inspect("isc", hidden=True),
+        "isi": image_inspect("isi", hidden=True),
+        "isn": network_inspect("isn", hidden=True),
+        "isv": volume_inspect("isv", hidden=True),
         "lsc": container_list("lsc", hidden=True),
         "lsi": image_list(name="lsi", hidden=True),
         "lsn": network_list(name="lsn", hidden=True),
         "lsv": volume_list(name="lsv", hidden=True),
-        "restart": container_restart("restart", hidden=True),
         "rmc": container_remove("rmc", hidden=True),
         "rmi": image_remove("rmi", hidden=True),
-        "run": container_run("run", hidden=True),
-        "start": container_start("start", hidden=True),
-        "stop": container_stop("stop", hidden=True),
+        "rmn": network_remove("rmn", hidden=True),
+        "rmv": volume_remove("rmv", hidden=True),
     }
 
     @click.group(cls=root_cls(), name="klee")
     @click.version_option(version="0.0.1")
     @click.option("--config", default=None, help="Location of Klee config file.")
     @click.option(
         "--theme",
```

### Comparing `kleene_cli-0.1.0rc2/klee/utils.py` & `kleene_cli-0.1.0rc3/klee/utils.py`

 * *Files identical despite different names*

### Comparing `kleene_cli-0.1.0rc2/klee/volume.py` & `kleene_cli-0.1.0rc3/klee/volume.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 
-from .client.api.default.volume_create import sync_detailed as volume_create
+from .client.api.default.volume_create import sync_detailed as volume_create_endpoint
 from .client.api.default.volume_list import sync_detailed as volume_list_endpoint
 from .client.api.default.volume_inspect import sync_detailed as volume_inspect_endpoint
-from .client.api.default.volume_remove import sync_detailed as volume_remove
+from .client.api.default.volume_remove import sync_detailed as volume_remove_endpoint
 from .client.api.default.volume_prune import sync_detailed as volume_prune_endpoint
 
 from .client.models.volume_config import VolumeConfig
 from .printing import (
     print_table,
     command_cls,
     group_cls,
@@ -21,30 +21,33 @@
 
 # pylint: disable=unused-argument
 @click.group(cls=group_cls())
 def root(name="volume"):
     """Manage volumes"""
 
 
-@root.command(cls=command_cls(), no_args_is_help=True)
-@click.argument("volume_name", nargs=1)
-def create(volume_name):
-    """
-    Create a new volume. If the volume name already exists nothing happens.
-    """
-    config = VolumeConfig.from_dict({"name": volume_name})
-    request_and_print_response(
-        volume_create,
-        kwargs={"json_body": config},
-        statuscode2printer={201: print_response_id, 500: print_backend_error},
-    )
+def volume_create(name, hidden=False):
+    @click.command(cls=command_cls(), name=name, hidden=hidden, no_args_is_help=True)
+    @click.argument("volume_name", nargs=1)
+    def create(volume_name):
+        """
+        Create a new volume. If the volume name already exists nothing happens.
+        """
+        config = VolumeConfig.from_dict({"name": volume_name})
+        request_and_print_response(
+            volume_create_endpoint,
+            kwargs={"json_body": config},
+            statuscode2printer={201: print_response_id, 500: print_backend_error},
+        )
+
+    return create
 
 
 def volume_list(name, hidden=False):
-    @root.command(cls=command_cls(), name=name, hidden=hidden)
+    @click.command(cls=command_cls(), name=name, hidden=hidden)
     def listing():
         """List volumes"""
         request_and_print_response(
             volume_list_endpoint,
             kwargs={},
             statuscode2printer={200: _print_volumes, 500: print_backend_error},
         )
@@ -59,46 +62,50 @@
     ]
     volumes = [
         [vol.name, human_duration(vol.created) + " ago"] for vol in response.parsed
     ]
     print_table(volumes, VOLUME_LIST_COLUMNS)
 
 
-root.add_command(volume_list("ls"), name="ls")
-
-root.add_command(
-    inspect_command(
-        name="inspect",
+def volume_inspect(name, hidden=False):
+    return inspect_command(
+        name=name,
+        hidden=hidden,
         argument="volume",
         id_var="volume_name",
         docs="Display detailed information on an volume.",
         endpoint=volume_inspect_endpoint,
-    ),
-    name="inspect",
-)
+    )
 
 
-@root.command(cls=command_cls(), name="rm", no_args_is_help=True)
-@click.argument("volumes", required=True, nargs=-1)
-def remove(volumes):
-    """Remove one or more volumes. You cannot remove a volume that is in use by a container."""
-    for volume_name in volumes:
-        response = request_and_print_response(
-            volume_remove,
-            kwargs={"volume_name": volume_name},
-            statuscode2printer={
-                200: print_response_id,
-                404: print_response_msg,
-                500: print_backend_error,
-            },
-        )
-        if response is None or response.status_code != 200:
-            break
+def volume_remove(name, hidden=False):
+    @click.command(cls=command_cls(), name=name, hidden=hidden, no_args_is_help=True)
+    @click.argument("volumes", required=True, nargs=-1)
+    def remove(volumes):
+        """Remove one or more volumes. You cannot remove a volume that is in use by a container."""
+        for volume_name in volumes:
+            response = request_and_print_response(
+                volume_remove_endpoint,
+                kwargs={"volume_name": volume_name},
+                statuscode2printer={
+                    200: print_response_id,
+                    404: print_response_msg,
+                    500: print_backend_error,
+                },
+            )
+            if response is None or response.status_code != 200:
+                break
+
+    return remove
 
 
+root.add_command(volume_create("create"), name="create")
+root.add_command(volume_list("ls"), name="ls")
+root.add_command(volume_inspect("inspect"), name="inspect")
+root.add_command(volume_remove("rm"), name="rm")
 root.add_command(
     prune_command(
         name="prune",
         docs="Remove all volumes that are not being mounted into any containers.",
         warning="WARNING! This will remove all unused volumes.",
         endpoint=volume_prune_endpoint,
     )
```

### Comparing `kleene_cli-0.1.0rc2/pyproject.toml` & `kleene_cli-0.1.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kleene-cli"
-version = "0.1.0rc2"
+version = "0.1.0rc3"
 description = "Klee - Kleene's CLI tool."
 authors = ["Lasse Grinderslev Andersen <lasse@philomath.dk>"]
 maintainers = [
     "Lasse Grinderslev Andersen <lasse@philomath.dk>",
 ]
 license = "BSD-2-Clause"
 readme = "README.md"
```

