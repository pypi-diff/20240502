# Comparing `tmp/bifrost-9.0.1.tar.gz` & `tmp/bifrost-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bifrost-9.0.1.tar", last modified: Thu Nov 26 09:15:18 2020, max compression
+gzip compressed data, was "bifrost-9.1.0.tar", last modified: Thu Feb 17 10:41:05 2022, max compression
```

## Comparing `bifrost-9.0.1.tar` & `bifrost-9.1.0.tar`

### file list

```diff
@@ -1,565 +1,571 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.725288 bifrost-9.0.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2020-11-26 09:14:50.000000 bifrost-9.0.1/.ansible-lint
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2020-11-26 09:14:50.000000 bifrost-9.0.1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2020-11-26 09:14:50.000000 bifrost-9.0.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2020-11-26 09:15:18.000000 bifrost-9.0.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4100 2020-11-26 09:14:50.000000 bifrost-9.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58234 2020-11-26 09:15:18.000000 bifrost-9.0.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2020-11-26 09:14:50.000000 bifrost-9.0.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-11-26 09:14:50.000000 bifrost-9.0.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2020-11-26 09:14:50.000000 bifrost-9.0.1/MISSION.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2020-11-26 09:15:18.725288 bifrost-9.0.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2020-11-26 09:14:50.000000 bifrost-9.0.1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2020-11-26 09:14:51.000000 bifrost-9.0.1/ansible-collections-requirements.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.629289 bifrost-9.0.1/bifrost/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10471 2020-11-26 09:14:51.000000 bifrost-9.0.1/bifrost/cli.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10731 2020-11-26 09:14:51.000000 bifrost-9.0.1/bifrost/inventory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.633288 bifrost-9.0.1/bifrost/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.633288 bifrost-9.0.1/bifrost/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3145 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/tests/functional/test_inventory_functional.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.633288 bifrost-9.0.1/bifrost/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2016 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/tests/unit/test_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5068 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/tests/unit/test_inventory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost/version.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      352 2020-11-26 09:14:50.000000 bifrost-9.0.1/bifrost-cli
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.633288 bifrost-9.0.1/bifrost.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2020-11-26 09:15:18.000000 bifrost-9.0.1/bifrost.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23979 2020-11-26 09:15:18.000000 bifrost-9.0.1/bifrost.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-11-26 09:15:18.000000 bifrost-9.0.1/bifrost.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-11-26 09:15:18.000000 bifrost-9.0.1/bifrost.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-11-26 09:15:18.000000 bifrost-9.0.1/bifrost.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-11-26 09:15:18.000000 bifrost-9.0.1/bifrost.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2020-11-26 09:15:18.000000 bifrost-9.0.1/bifrost.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2020-11-26 09:15:18.000000 bifrost-9.0.1/bifrost.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2020-11-26 09:14:50.000000 bifrost-9.0.1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.633288 bifrost-9.0.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.633288 bifrost-9.0.1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2590 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.637288 bifrost-9.0.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2020-11-26 09:14:51.000000 bifrost-9.0.1/doc/source/contributor/testenv.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2285 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/contributor/vagrant.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2661 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/contributor/virsh.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.637288 bifrost-9.0.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17417 2020-11-26 09:14:51.000000 bifrost-9.0.1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/install/keystone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/install/offline-install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/install/virtualenv.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.637288 bifrost-9.0.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4255 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/user/dhcp.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9148 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/user/howto.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/user/keystone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7592 2020-11-26 09:14:50.000000 bifrost-9.0.1/doc/source/user/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2020-11-26 09:14:50.000000 bifrost-9.0.1/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.641288 bifrost-9.0.1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.641288 bifrost-9.0.1/playbooks/ci/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/ci/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/ci/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1148 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/ci/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/cleanup-deployment-images.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/deploy-dynamic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/enroll-dynamic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/example-deploy-all-available-nodes.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1889 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/install.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.641288 bifrost-9.0.1/playbooks/inventory/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/inventory/baremetal.csv.example
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1926 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/inventory/baremetal.json.example
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/inventory/baremetal.yml.example
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10731 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/inventory/bifrost_inventory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.641288 bifrost-9.0.1/playbooks/inventory/group_vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2607 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/inventory/group_vars/baremetal
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/inventory/group_vars/localhost
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/inventory/group_vars/target
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/inventory/localhost
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/inventory/target
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.641288 bifrost-9.0.1/playbooks/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5402 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/library/network_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6294 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/library/os_ironic_facts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6294 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/library/os_ironic_node_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3105 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/redeploy-dynamic.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.625289 bifrost-9.0.1/playbooks/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2681 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5748 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4291 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1654 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/tasks/ssh_public_key_path.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/tasks/update_facts_from_ironic.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/templates/interfaces.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/templates/network_data.json.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/templates/openstack_meta_data.json.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/vars/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.645288 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3783 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/tasks/create_bootable_image.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4867 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9477 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/vars/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7753 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/dummy-defaults.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_CentOS.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Debian.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Fedora.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_RedHat.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Suse.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Ubuntu_20.04.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.649288 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6511 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/tasks/create_vm.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6722 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/tasks/prepare_libvirt.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.653288 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/net.xml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/pool_dir.xml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/redfish-emulator.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/redfish-emulator.service.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/testvm.xml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/vbmcd.service.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/virtualbmc.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.653288 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6356 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.653288 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.653288 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.653288 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3846 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.653288 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/templates/dhcp-host.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/templates/dns-address.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.653288 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14360 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.657288 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/dummy-defaults.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14492 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Debian_family.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Fedora.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_RedHat_family.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Suse_family.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Ubuntu.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.657288 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/files/boot.ipxe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/files/ironic_policy.te
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/files/tftpboot-map-file
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/files/xinetd.tftp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.657288 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.661288 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14297 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/bootstrap.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4154 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/create_tftpboot.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3548 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/download_ipa_image.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/get_ipxe.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2389 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/hw_types.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5477 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/inspector_bootstrap.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1190 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/inspector_install.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/inspector_start.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3760 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/install.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2082 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/ironic_config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6875 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/keystone_setup.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5967 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/keystone_setup_inspector.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2103 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/migrations.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/prometheus_exporter_install.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/prometheus_exporter_start.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/set_ssh_private_key.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/setup_firewalld.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/staging_install.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/start.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/validate.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/vendor_deps.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/10-rsyslog-remote.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3932 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/dnsmasq.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/inspector-default-boot-ipxe.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2771 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/ironic-inspector.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/ironic-prometheus-exporter.service.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6741 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/ironic.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/nginx.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/static.hosts.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/systemd_template.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2529 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2125 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/tasks/validate.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/templates/clouds.yaml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/templates/openrc.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3760 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/defaults/dummy-defaults.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3119 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/defaults/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/defaults/required_defaults_Debian_family.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/defaults/required_defaults_RedHat_family.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/defaults/required_defaults_Suse_family.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/defaults/required_defaults_Ubuntu.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/files/keystone_policy.te
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.665288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10955 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/bootstrap.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/install.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/start.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4804 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/upgrade.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/keystone-admin.ini.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/keystone-public.ini.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/keystone.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/nginx.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/nginx_conf.d_bifrost-keystone.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/systemd_template.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-pip-install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-pip-install/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-pip-install/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-pip-install/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-pip-install/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2887 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-pip-install/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4179 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5848 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1916 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.669288 bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3180 2020-11-26 09:14:50.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/files/test-dhcp.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1868 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-vm/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-vm/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1875 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-vm/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-test-vm/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1871 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-test-vm/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-tls/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2508 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-tls/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-tls/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-tls/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-tls/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-tls/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2045 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.673288 bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3569 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4391 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1911 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.677288 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/templates/dhcp-host.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/roles/ironic-inspect-node/templates/dns-address.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/test-bifrost-create-vm.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3113 2020-11-26 09:14:51.000000 bifrost-9.0.1/playbooks/test-bifrost.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.625289 bifrost-9.0.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.717288 bifrost-9.0.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/Add-env-var-support-for-mysql-user-password-3ac520eea7ea9807.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/add-bindep-support-8f54b246a1d2bca5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/add-ipe-1f57e04d2881215f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/add-private-key-9788621be14ba324.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/agent-power-0773acb338ae4169.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/allow-create-vm-with-custom-names-0d655bc02e141ec9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/allow-custom-elements-05c9495c8fd840e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/allow-custom-private-endpoints-ip-b4f29647569a15ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/allow-custom-public-endpoints-ip-4662c246f029589e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/allow-install-remote-101eea1ea4009fe1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/always-create-clouds-file-d0b72808155a9344.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ancient-fedora-jessie-773ba251b28f4a94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ansible-2.0-support-81fa15cc27c28ba8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ansible-2.1-4b6b36998287bb11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2252 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ansible-pip-install-2b66bd82ce9ed4f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ansible-virt-0759a857daaacccf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/api-url-a6f79de3cc8b0e3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/auth-59e73f74a2dd507f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/bifrost-cli-extra-19fd989a05b2e4b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/bifrost-inspector-a154561802d8d614.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/bifrost-openstack-ci-prep-172cbb159e0a2b78.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/bifrost-role-auth-support-ea6b5571cd339aa2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/bifrost_node_names-f26ca2eab7e261d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/bionic-centos8-ci-5047b40c6ba51484.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/bump-ansible-version-35c201d1d6d30860.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/centos-keystone-acad21e70153067d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/change-default-vnic-type-a4ba179ea8f9792d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/change-inspector-to-use-mysql-17cb03cabb958ff9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/change-ipa-version-cacaec52a55188cc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ci-testing-faa63db25ebc94df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/cirros-0.5.1-d09a433cbea1a3b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/cleaning-9b4241342320f315.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/cli-validate-474e15ba9631e72f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/client-config-existing-8041abc5db164fd4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/copy_from_local_path-8aff180483e6bced.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/correct-requirements-ci-path-5ced93013d2c9b02.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/create-clouds.yaml-9bbc79c0497dee43.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/create-openrc-9e7f959790f7f409.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/creation-of-ironic-user-5a970c5f73e8ef45.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/custom-partitioning-78d7ac12d80a993f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/debian-buster-dd7cfde9908deb09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/decompose-ironic-install-role-75b9a431bba88bad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/default-ansible2.8-e0000544b2f55b88.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/default-boot-mode-5561325f68224719.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/default-ipa-fe012dfdba580bf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/default-to-use-fasttrack-a526e1d86d2f669d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/deploy-with-selinux-enabled-6c155cfa8f8720c0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/deprecate-classic-drivers-f88c53fa483aa7d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/deprecate_node_network_info-8c5e1bc4df6b8097.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/developer-mode-000e7a125642b9e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/dhcp_ignore_inventory_dhcp-44668e3fe710c134.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/disable_dnsmasq_dns-0d545cdaa81b92a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/dnf-support-413762b0af2887bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/download-ipa-upgrade-91e0fc4beea7419e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/drop-amt-e4bfb6e2ae3c4301.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/drop-python2-f465181d67cccd30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/enable-inspector-discovery-77aa6f5c1f1e42c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/enable_inspector_by_default-828fc1284d6a7c2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/enabled-deploy-interfaces-bf1e25a29ac80680.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/env-vars-f07a4779a881c039.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/explicit-ansible-version-d4052b4900faba99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/f32-suse15.2-44a8189e81b1bfd7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/fast-track-inspection-a28a062e86f06190.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/fedora-core-25-support-b9f8f258a9738a06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/fedora-firewalld-f8e2e15be5fe43fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/firewalld-d53c6396828b91ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/firewalld-services-4c255c02d8d427f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/firewalld-zone-d8c72fb5924a4916.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/fix-deploy-logs-175fb352c5730b58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/fix-inspection-with-inventory-dhcp-cfc236974bf4ed0a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/focal-36208207a571f354.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/focal-e40fdd37d11faac9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/generated-ipa-url-protocol-1a5a2bfc8e20db9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/git-url-root-c81478d395f66e46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/http-basic-40df399ea63956aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/hw-types-17106c0397f34ef1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/images-permissions-2042490e3ca13656.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/initial-release-notes-937001279bbb52cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/inspector-keystone-support-3786a22b49e851e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/inspector-no-longer-powers-off-796801e809184eee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/inspector-processing-hooks-addf80be5f31aa61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/inspector-pxe-args-c65acb610507ab08.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/inspector-ramdisk-logs-0db7c111fd455cec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/install-SUDO_USER-fix-2bf577269008587f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/install-osc-c179e673dc338ab3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/internal-address-c1f9ffb731373ea3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/interpreter-a6cd3a98e9cd239f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/introduce-install-dib-1e53da734a878dac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/introspection-timeout-parameter-8e86afffd2f1d947.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/inventory-functional-tests-998796326c2a92ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/inventory_dhcp_provisioning_ipv4_address-d2779f1abc38324a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/inventory_dns-921195abbc5e65ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ipa-branch-6d1d30876b584cbf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ipa-builder-29d3db174048f1b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ipxe-command-line-ip-argument-8b67a6a3601de1f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ipxe-download-bc1235cbbc87121c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ironic-driver-support-doc-03a4e14ab2adeb85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ironic-extra-packages-e3ad3e4a85e59049.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ironic-inspector-install-from-git-d74a3ce3b1d1c87c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ironic-lib-filters-371185c7a7691106.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ironic-online-migrations-092aef2b4c2ec75f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/jessie-to-stretch-207bbd4f10149b4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/json-rpc-auth-2430cc7432cbfe10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/json-rpc-default-f0cdafc217a1122c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/json-rpc-e5ccd5a13f6d51aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/keystone-installation-3b812d9f673c7bbe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/keystone-lockout-c8a26a09e0f0560b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/kvm-acceleration-support-8be50d32bc34c4b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/list_of_nameservers-cea9e03675bf56bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/log-directories-87b86df40464bb2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/logging-bcc7d552944c94e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/managed-inspection-options-2764b4ae0079f505.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/manual-management-c204a200b0f0e6e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/merge-test-playbooks-aeabc7a614cbce29.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/metalsmith-7044429597a5f137.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/more-clouds-7c0fccf5701918d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/move-to-tinyipa-8c7840b73c40a9e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/mysql-database-separation-d6bf9a4f22cd8bbb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/no-classic-drivers-0b8a346bcab8a004.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/no-clone-cebedc81211dcfa5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/no-csv-b7f149e88aba1b85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/no-osc-b39d14591103b2c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/no-rabbit-95434aaea3bb5528.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/no-shade-b861f699b8a9919f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/no-store-nginx-75bc3f9068fb8f78.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/no-xenial-1c27b7bb2cf165ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/nodes.json-d47a30a22a04c7ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1227 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/nossh-16577ec5c3b82594.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1066 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ocata-summary-040e557460bab2bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/old-network-info-33a853faf6d6c6d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/openstacksdk-addition-efec3878ef988295.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/os_client_config-support-b1073062d842febb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/override-dhcp-boot-6659585b75d58757.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/override_upper_constraints-79f837d8ac58e53d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/passing-no-proxy-32191c148442c57d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/pin-proliantutils-60f1facf44c223ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/populate_dns_servers_dnsmasq-4f30a9957e8de732.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/populate_domain_dnsmasq-5408896247eb39b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/populate_ntp_servers_dnsmasq-249d2a26b94b0bf1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/pxe-acl-26f3be809caa0c88.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/pxe-driver-support-e2d8a769bf910dbc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/random-passwords-b33b8de010ee82b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/redeploy-dynamic-cc8b69f79a6869cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/redfish-92d39daf559d5445.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/releasenote-341a5eebe6168aea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/releasenote-4812959d071329fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/releasenote-94bcb2b0da207f94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/remove-ucs-drivers-37f46fa8500f9ddb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/remove-ucssdk-e61762195a7c8b4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/repo-owner-41db02a4d0406a7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/resource-class-243535c9049cbd73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/sdk-source-1bd77dbd11b08577.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/selinux-lnk_file-527ac51c60f9c2ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/skip-install-bfd642f5065cf304.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/store-data-a14351976eda9842.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/store-introspection-data-bc4f2fef2f5bb543.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/support-custom-ansible-groups-38ad5d3a930b17eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/support-fedora-3b14bffb24097b28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/support-remote-logging-93e159eeef4cc68b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/support-staging-drivers-1c398a56dde9b240.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/suse-ipxe-ce4f1bf07db78860.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/switch_to_openstack_collection-a6eb3e24a68a1a82.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/templated_ironic_conf-bd052f2b2897d37a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/test-redfish-54ed748e2305d8eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/test-with-json-inventory-b05204009f880431.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/test_vm_network_enable_dhcp-78923ef94b44e6d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/tftp-context-6f918743ba9052b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/tls-988e725820bb8aca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/transform_boot_image-16fe26bd1a849aa0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/ubuntu-ports-ce9d1ceaf516adce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/update-ipa-76691dbca92246b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/update-repos-b60563ee51b574fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/update_default_ansible_2.6-82ff11d7b653b946.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/update_default_ansible_2.9-e96335c0ef609642.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/use-tinyipa-31f5343def1c0bf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/use_public_urls_endpoints-1220a7f4164696c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/validate-261b92bc614f5d4a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/validate-path-5c303903900dcd65.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/venv-default-895f7b633803297f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/venv-forever-ba8b85b04a28a293.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/verify-checksum-ipa-a73cf936d0ae2ce1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/vm-host-cpu-type-support-a09768f360372506.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/notes/vm-nic-type-support-0ac47ccd3d56132c.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.721288 bifrost-9.0.1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2733 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2020-11-26 09:14:51.000000 bifrost-9.0.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2020-11-26 09:14:51.000000 bifrost-9.0.1/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.721288 bifrost-9.0.1/scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2020-11-26 09:14:51.000000 bifrost-9.0.1/scripts/README.md
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4009 2020-11-26 09:14:51.000000 bifrost-9.0.1/scripts/collect-test-info.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3036 2020-11-26 09:14:51.000000 bifrost-9.0.1/scripts/env-setup.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4092 2020-11-26 09:14:51.000000 bifrost-9.0.1/scripts/install-deps.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2696 2020-11-26 09:14:51.000000 bifrost-9.0.1/scripts/split_json.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6174 2020-11-26 09:14:51.000000 bifrost-9.0.1/scripts/test-bifrost.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2020-11-26 09:15:18.725288 bifrost-9.0.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2020-11-26 09:14:51.000000 bifrost-9.0.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2020-11-26 09:14:51.000000 bifrost-9.0.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.721288 bifrost-9.0.1/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2020-11-26 09:14:51.000000 bifrost-9.0.1/tools/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2020-11-26 09:14:51.000000 bifrost-9.0.1/tools/ansible-lint.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.721288 bifrost-9.0.1/tools/vagrant_dev_env/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2957 2020-11-26 09:14:51.000000 bifrost-9.0.1/tools/vagrant_dev_env/Vagrantfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2020-11-26 09:14:51.000000 bifrost-9.0.1/tools/vagrant_dev_env/vagrant.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.625289 bifrost-9.0.1/tools/virsh_dev_env/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.721288 bifrost-9.0.1/tools/virsh_dev_env/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2020-11-26 09:14:51.000000 bifrost-9.0.1/tools/virsh_dev_env/network/br_direct.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2020-11-26 09:14:51.000000 bifrost-9.0.1/tools/virsh_dev_env/network/default.xml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.721288 bifrost-9.0.1/tools/virsh_dev_env/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3524 2020-11-26 09:14:51.000000 bifrost-9.0.1/tools/virsh_dev_env/vm/baremetal.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2236 2020-11-26 09:14:51.000000 bifrost-9.0.1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-11-26 09:15:18.721288 bifrost-9.0.1/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3691 2020-11-26 09:14:51.000000 bifrost-9.0.1/zuul.d/bifrost-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2040 2020-11-26 09:14:51.000000 bifrost-9.0.1/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.528663 bifrost-9.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2022-02-17 10:40:35.000000 bifrost-9.1.0/.ansible-lint
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2022-02-17 10:40:35.000000 bifrost-9.1.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2022-02-17 10:40:35.000000 bifrost-9.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2022-02-17 10:41:05.000000 bifrost-9.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4159 2022-02-17 10:40:35.000000 bifrost-9.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59304 2022-02-17 10:41:05.000000 bifrost-9.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-02-17 10:40:35.000000 bifrost-9.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-02-17 10:40:35.000000 bifrost-9.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2022-02-17 10:40:35.000000 bifrost-9.1.0/MISSION.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2022-02-17 10:41:05.528663 bifrost-9.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2022-02-17 10:40:35.000000 bifrost-9.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-02-17 10:40:35.000000 bifrost-9.1.0/ansible-collections-requirements.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.444658 bifrost-9.1.0/bifrost/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10471 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/cli.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10687 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/inventory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.444658 bifrost-9.1.0/bifrost/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.444658 bifrost-9.1.0/bifrost/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3145 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/tests/functional/test_inventory_functional.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.444658 bifrost-9.1.0/bifrost/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2016 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/tests/unit/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5560 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/tests/unit/test_inventory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost/version.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      354 2022-02-17 10:40:35.000000 bifrost-9.1.0/bifrost-cli
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.444658 bifrost-9.1.0/bifrost.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2022-02-17 10:41:05.000000 bifrost-9.1.0/bifrost.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24313 2022-02-17 10:41:05.000000 bifrost-9.1.0/bifrost.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-02-17 10:41:05.000000 bifrost-9.1.0/bifrost.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-02-17 10:41:05.000000 bifrost-9.1.0/bifrost.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-02-17 10:41:05.000000 bifrost-9.1.0/bifrost.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-02-17 10:41:05.000000 bifrost-9.1.0/bifrost.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-02-17 10:41:05.000000 bifrost-9.1.0/bifrost.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2022-02-17 10:41:05.000000 bifrost-9.1.0/bifrost.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2022-02-17 10:40:35.000000 bifrost-9.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.444658 bifrost-9.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.448658 bifrost-9.1.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2590 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.448658 bifrost-9.1.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2386 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/contributor/testenv.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2285 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/contributor/vagrant.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2661 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/contributor/virsh.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.448658 bifrost-9.1.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17943 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/install/keystone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/install/offline-install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/install/virtualenv.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.448658 bifrost-9.1.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4255 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/user/dhcp.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9148 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/user/howto.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/user/keystone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7592 2022-02-17 10:40:35.000000 bifrost-9.1.0/doc/source/user/troubleshooting.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2022-02-17 10:40:35.000000 bifrost-9.1.0/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.452658 bifrost-9.1.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.452658 bifrost-9.1.0/playbooks/ci/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/ci/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/ci/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1148 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/ci/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/cleanup-deployment-images.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/deploy-dynamic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/enroll-dynamic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/example-deploy-all-available-nodes.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1889 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/install.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.452658 bifrost-9.1.0/playbooks/inventory/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/baremetal.csv.example
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1926 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/baremetal.json.example
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/baremetal.yml.example
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10687 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/bifrost_inventory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.452658 bifrost-9.1.0/playbooks/inventory/group_vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2607 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/group_vars/baremetal
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/group_vars/localhost
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/group_vars/target
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/localhost
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/inventory/target
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.452658 bifrost-9.1.0/playbooks/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5402 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/library/network_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6294 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/library/os_ironic_facts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6294 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/library/os_ironic_node_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3105 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/redeploy-dynamic.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.436657 bifrost-9.1.0/playbooks/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.452658 bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.452658 bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2681 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5748 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4291 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1654 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/tasks/ssh_public_key_path.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/tasks/update_facts_from_ironic.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/templates/interfaces.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/templates/network_data.json.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/templates/openstack_meta_data.json.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/vars/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3783 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/tasks/create_bootable_image.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4867 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.456659 bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8998 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.460659 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7753 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.460659 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/dummy-defaults.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2683 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_CentOS.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Debian.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Fedora.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_RedHat.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Suse.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Ubuntu_20.04.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.460659 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.460659 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6511 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/tasks/create_vm.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6722 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/tasks/prepare_libvirt.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.460659 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/net.xml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/pool_dir.xml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/redfish-emulator.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/redfish-emulator.service.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/testvm.xml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/vbmcd.service.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/virtualbmc.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.460659 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6356 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.460659 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.464659 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.464659 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3846 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.464659 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/templates/dhcp-host.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/templates/dns-address.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.464659 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14360 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.464659 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/dummy-defaults.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14617 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Debian_family.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Fedora.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_RedHat_family.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Suse_family.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Ubuntu.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.464659 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/files/boot.ipxe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/files/ironic_policy.te
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/files/tftpboot-map-file
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/files/xinetd.tftp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.464659 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.468659 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14297 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/bootstrap.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4154 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/create_tftpboot.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3548 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/download_ipa_image.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/get_ipxe.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2389 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/hw_types.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5477 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/inspector_bootstrap.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1190 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/inspector_install.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/inspector_start.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3926 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/install.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2082 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/ironic_config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6875 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/keystone_setup.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5967 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/keystone_setup_inspector.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2103 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/migrations.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/prometheus_exporter_install.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/prometheus_exporter_start.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/set_ssh_private_key.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/setup_firewalld.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/staging_install.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/start.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/validate.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/vendor_deps.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.472660 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/10-rsyslog-remote.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3932 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/dnsmasq.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/inspector-default-boot-ipxe.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2772 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/ironic-inspector.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/ironic-prometheus-exporter.service.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6741 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/ironic.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/nginx.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/static.hosts.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/systemd_template.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.472660 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/vars/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.472660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2529 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.472660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.472660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.472660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2125 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/tasks/validate.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.472660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/templates/clouds.yaml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/templates/openrc.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.472660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3760 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/defaults/dummy-defaults.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3119 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/defaults/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/defaults/required_defaults_Debian_family.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/defaults/required_defaults_RedHat_family.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/defaults/required_defaults_Suse_family.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/defaults/required_defaults_Ubuntu.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/files/keystone_policy.te
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10955 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/bootstrap.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/install.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/start.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4804 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/upgrade.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/keystone-admin.ini.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/keystone-public.ini.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/keystone.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/nginx.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/nginx_conf.d_bifrost-keystone.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/systemd_template.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-pip-install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-pip-install/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-pip-install/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-pip-install/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-pip-install/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2887 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-pip-install/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.476660 bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4179 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5856 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1916 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3180 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/files/test-dhcp.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1868 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-vm/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-vm/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1875 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-vm/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-test-vm/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1871 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-test-vm/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-tls/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2508 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-tls/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-tls/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-tls/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-tls/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-tls/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.480660 bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2045 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3569 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4391 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1911 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.484660 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/templates/dhcp-host.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/roles/ironic-inspect-node/templates/dns-address.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/test-bifrost-create-vm.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3113 2022-02-17 10:40:35.000000 bifrost-9.1.0/playbooks/test-bifrost.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.436657 bifrost-9.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.520663 bifrost-9.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/Add-env-var-support-for-mysql-user-password-3ac520eea7ea9807.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/add-bindep-support-8f54b246a1d2bca5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/add-ipe-1f57e04d2881215f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/add-private-key-9788621be14ba324.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/agent-power-0773acb338ae4169.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/allow-create-vm-with-custom-names-0d655bc02e141ec9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/allow-custom-elements-05c9495c8fd840e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/allow-custom-private-endpoints-ip-b4f29647569a15ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/allow-custom-public-endpoints-ip-4662c246f029589e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/allow-install-remote-101eea1ea4009fe1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/always-create-clouds-file-d0b72808155a9344.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ancient-fedora-jessie-773ba251b28f4a94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ansible-2.0-support-81fa15cc27c28ba8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ansible-2.1-4b6b36998287bb11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2252 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ansible-pip-install-2b66bd82ce9ed4f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ansible-virt-0759a857daaacccf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/api-url-a6f79de3cc8b0e3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/auth-59e73f74a2dd507f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/bifrost-cli-extra-19fd989a05b2e4b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/bifrost-inspector-a154561802d8d614.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/bifrost-openstack-ci-prep-172cbb159e0a2b78.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/bifrost-role-auth-support-ea6b5571cd339aa2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/bifrost_node_names-f26ca2eab7e261d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/bionic-centos8-ci-5047b40c6ba51484.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/bump-ansible-version-35c201d1d6d30860.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/centos-keystone-acad21e70153067d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/centos8-stream-0c6d9adb544e36af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/change-default-vnic-type-a4ba179ea8f9792d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/change-inspector-to-use-mysql-17cb03cabb958ff9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/change-ipa-version-cacaec52a55188cc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ci-testing-faa63db25ebc94df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/cirros-0.5.1-d09a433cbea1a3b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/cleaning-9b4241342320f315.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/cli-validate-474e15ba9631e72f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/client-config-existing-8041abc5db164fd4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/copy_from_local_path-8aff180483e6bced.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/correct-requirements-ci-path-5ced93013d2c9b02.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/create-clouds.yaml-9bbc79c0497dee43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/create-openrc-9e7f959790f7f409.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/creation-of-ironic-user-5a970c5f73e8ef45.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/custom-partitioning-78d7ac12d80a993f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/debian-buster-dd7cfde9908deb09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/decompose-ironic-install-role-75b9a431bba88bad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/default-ansible2.8-e0000544b2f55b88.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/default-boot-mode-5561325f68224719.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/default-ipa-fe012dfdba580bf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/default-to-use-fasttrack-a526e1d86d2f669d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/deploy-with-selinux-enabled-6c155cfa8f8720c0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/deprecate-classic-drivers-f88c53fa483aa7d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/deprecate_node_network_info-8c5e1bc4df6b8097.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/developer-mode-000e7a125642b9e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/dhcp_ignore_inventory_dhcp-44668e3fe710c134.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/disable_dnsmasq_dns-0d545cdaa81b92a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/dnf-support-413762b0af2887bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/download-ipa-upgrade-91e0fc4beea7419e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/drop-amt-e4bfb6e2ae3c4301.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/drop-python2-f465181d67cccd30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/enable-inspector-discovery-77aa6f5c1f1e42c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/enable_inspector_by_default-828fc1284d6a7c2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/enabled-deploy-interfaces-bf1e25a29ac80680.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/env-vars-f07a4779a881c039.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/explicit-ansible-version-d4052b4900faba99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/f32-suse15.2-44a8189e81b1bfd7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/fast-track-inspection-a28a062e86f06190.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/fedora-core-25-support-b9f8f258a9738a06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/fedora-firewalld-f8e2e15be5fe43fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/firewalld-d53c6396828b91ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/firewalld-services-4c255c02d8d427f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/firewalld-zone-d8c72fb5924a4916.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/fix-deploy-logs-175fb352c5730b58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/fix-inspection-with-inventory-dhcp-cfc236974bf4ed0a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/fix-story-2008394-9a77486a838a1f2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/focal-36208207a571f354.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/focal-e40fdd37d11faac9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/generated-ipa-url-protocol-1a5a2bfc8e20db9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/git-url-root-c81478d395f66e46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/http-basic-40df399ea63956aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/hw-types-17106c0397f34ef1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/images-permissions-2042490e3ca13656.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/initial-release-notes-937001279bbb52cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inspect-fast-track-36007cc32bdf7e5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inspector-keystone-support-3786a22b49e851e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inspector-no-longer-powers-off-796801e809184eee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inspector-processing-hooks-addf80be5f31aa61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inspector-pxe-args-c65acb610507ab08.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inspector-ramdisk-logs-0db7c111fd455cec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/install-SUDO_USER-fix-2bf577269008587f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/install-osc-c179e673dc338ab3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/internal-address-c1f9ffb731373ea3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/interpreter-a6cd3a98e9cd239f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/introduce-install-dib-1e53da734a878dac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/introspection-timeout-parameter-8e86afffd2f1d947.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inventory-functional-tests-998796326c2a92ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inventory_dhcp_provisioning_ipv4_address-d2779f1abc38324a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/inventory_dns-921195abbc5e65ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ipa-branch-6d1d30876b584cbf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ipa-builder-29d3db174048f1b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ipxe-command-line-ip-argument-8b67a6a3601de1f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ipxe-download-bc1235cbbc87121c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ironic-driver-support-doc-03a4e14ab2adeb85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ironic-extra-packages-e3ad3e4a85e59049.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ironic-inspector-install-from-git-d74a3ce3b1d1c87c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ironic-lib-filters-371185c7a7691106.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ironic-online-migrations-092aef2b4c2ec75f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/jessie-to-stretch-207bbd4f10149b4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/json-rpc-auth-2430cc7432cbfe10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/json-rpc-default-f0cdafc217a1122c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/json-rpc-e5ccd5a13f6d51aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/keystone-installation-3b812d9f673c7bbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/keystone-lockout-c8a26a09e0f0560b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/kvm-acceleration-support-8be50d32bc34c4b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/list_of_nameservers-cea9e03675bf56bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/log-directories-87b86df40464bb2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/logging-bcc7d552944c94e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/managed-inspection-options-2764b4ae0079f505.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/manual-management-c204a200b0f0e6e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/merge-test-playbooks-aeabc7a614cbce29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/metalsmith-7044429597a5f137.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/more-clouds-7c0fccf5701918d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/move-dib-deps-install-8a8aafc060461dc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/move-to-tinyipa-8c7840b73c40a9e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/mysql-database-separation-d6bf9a4f22cd8bbb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/no-classic-drivers-0b8a346bcab8a004.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/no-clone-cebedc81211dcfa5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/no-csv-b7f149e88aba1b85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/no-osc-b39d14591103b2c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/no-rabbit-95434aaea3bb5528.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/no-shade-b861f699b8a9919f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/no-store-nginx-75bc3f9068fb8f78.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/no-xenial-1c27b7bb2cf165ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/nodes.json-d47a30a22a04c7ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1227 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/nossh-16577ec5c3b82594.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1066 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ocata-summary-040e557460bab2bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/old-network-info-33a853faf6d6c6d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/openstacksdk-addition-efec3878ef988295.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/os_client_config-support-b1073062d842febb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/override-dhcp-boot-6659585b75d58757.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/override_upper_constraints-79f837d8ac58e53d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/params-ab98e0ac242d119a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/passing-no-proxy-32191c148442c57d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/pin-proliantutils-60f1facf44c223ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/populate_dns_servers_dnsmasq-4f30a9957e8de732.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/populate_domain_dnsmasq-5408896247eb39b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/populate_ntp_servers_dnsmasq-249d2a26b94b0bf1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/pxe-acl-26f3be809caa0c88.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/pxe-driver-support-e2d8a769bf910dbc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/random-passwords-b33b8de010ee82b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/redeploy-dynamic-cc8b69f79a6869cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/redfish-92d39daf559d5445.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/releasenote-341a5eebe6168aea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/releasenote-4812959d071329fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/releasenote-94bcb2b0da207f94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/remove-ucs-drivers-37f46fa8500f9ddb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/remove-ucssdk-e61762195a7c8b4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/repo-owner-41db02a4d0406a7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/resource-class-243535c9049cbd73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/sdk-source-1bd77dbd11b08577.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/selinux-lnk_file-527ac51c60f9c2ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/skip-install-bfd642f5065cf304.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/squashfs-ddbbbac856e8f9fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/store-data-a14351976eda9842.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/store-introspection-data-bc4f2fef2f5bb543.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/support-custom-ansible-groups-38ad5d3a930b17eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/support-fedora-3b14bffb24097b28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/support-remote-logging-93e159eeef4cc68b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/support-staging-drivers-1c398a56dde9b240.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/suse-ipxe-ce4f1bf07db78860.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/switch_to_openstack_collection-a6eb3e24a68a1a82.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/templated_ironic_conf-bd052f2b2897d37a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/test-redfish-54ed748e2305d8eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/test-with-json-inventory-b05204009f880431.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/test_vm_network_enable_dhcp-78923ef94b44e6d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/tftp-context-6f918743ba9052b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/tls-988e725820bb8aca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/transform_boot_image-16fe26bd1a849aa0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/ubuntu-ports-ce9d1ceaf516adce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/update-ipa-76691dbca92246b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/update-repos-b60563ee51b574fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/update_default_ansible_2.6-82ff11d7b653b946.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/update_default_ansible_2.9-e96335c0ef609642.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/use-tinyipa-31f5343def1c0bf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/use_public_urls_endpoints-1220a7f4164696c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/validate-261b92bc614f5d4a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/validate-path-5c303903900dcd65.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/venv-default-895f7b633803297f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/venv-forever-ba8b85b04a28a293.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/verify-checksum-ipa-a73cf936d0ae2ce1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/vm-host-cpu-type-support-a09768f360372506.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/notes/vm-nic-type-support-0ac47ccd3d56132c.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.524663 bifrost-9.1.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2733 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-02-17 10:40:35.000000 bifrost-9.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2022-02-17 10:40:35.000000 bifrost-9.1.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.524663 bifrost-9.1.0/scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2022-02-17 10:40:35.000000 bifrost-9.1.0/scripts/README.md
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4138 2022-02-17 10:40:35.000000 bifrost-9.1.0/scripts/collect-test-info.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3047 2022-02-17 10:40:35.000000 bifrost-9.1.0/scripts/env-setup.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4612 2022-02-17 10:40:35.000000 bifrost-9.1.0/scripts/install-deps.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2696 2022-02-17 10:40:35.000000 bifrost-9.1.0/scripts/split_json.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6170 2022-02-17 10:40:35.000000 bifrost-9.1.0/scripts/test-bifrost.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2022-02-17 10:41:05.528663 bifrost-9.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-02-17 10:40:35.000000 bifrost-9.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2022-02-17 10:40:35.000000 bifrost-9.1.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.524663 bifrost-9.1.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2022-02-17 10:40:35.000000 bifrost-9.1.0/tools/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2022-02-17 10:40:35.000000 bifrost-9.1.0/tools/ansible-lint.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.528663 bifrost-9.1.0/tools/vagrant_dev_env/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2957 2022-02-17 10:40:35.000000 bifrost-9.1.0/tools/vagrant_dev_env/Vagrantfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2022-02-17 10:40:35.000000 bifrost-9.1.0/tools/vagrant_dev_env/vagrant.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.436657 bifrost-9.1.0/tools/virsh_dev_env/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.528663 bifrost-9.1.0/tools/virsh_dev_env/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2022-02-17 10:40:35.000000 bifrost-9.1.0/tools/virsh_dev_env/network/br_direct.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2022-02-17 10:40:35.000000 bifrost-9.1.0/tools/virsh_dev_env/network/default.xml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.528663 bifrost-9.1.0/tools/virsh_dev_env/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3524 2022-02-17 10:40:35.000000 bifrost-9.1.0/tools/virsh_dev_env/vm/baremetal.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2422 2022-02-17 10:40:35.000000 bifrost-9.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-17 10:41:05.528663 bifrost-9.1.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2022-02-17 10:40:35.000000 bifrost-9.1.0/zuul.d/bifrost-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2000 2022-02-17 10:40:35.000000 bifrost-9.1.0/zuul.d/project.yaml
```

### Comparing `bifrost-9.0.1/.ansible-lint` & `bifrost-9.1.0/.ansible-lint`

 * *Files 11% similar despite different names*

```diff
@@ -3,8 +3,9 @@
   - '208'  # File permissions not mentioned
   - '301'  # Commands should not change things if nothing needs doing
   - '502'  # All tasks should be named
   - '701'  # meta/main.yml should contain relevant info
   - '702'  # Tags must contain lowercase letters and digits only
   # NOTE(dtantsur): the following rules should likely stay excluded:
   - '106'  # Role name {} does not match ``^[a-z][a-z0-9_]+$`` pattern'
+  - '403'  # Package installs should not use latest
   - '503'  # Tasks that run when changed should likely be handlers
```

### Comparing `bifrost-9.0.1/AUTHORS` & `bifrost-9.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/CONTRIBUTING.rst` & `bifrost-9.1.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 For a highly abridged version, read on.
 
 -------------
 Communicating
 -------------
 
 Before you file a bug or new review set, it's often helpful to chat with other
-developers. The #openstack-ironic channel is a good place to start, and if
+developers. The #openstack-ironic channel on OFTC IRC network
+(irc://irc.oftc.net/#openstack-ironic) is a good place to start, and if
 you don't have IRC (or would prefer email),
 openstack-discuss@lists.openstack.org is the mailing list for all OpenStack
 projects. As the name implies, that mailing list is for all OpenStack
 development, so it's often harder to get attention on your particular issue.
 
 -----------
 Filing Bugs
```

### Comparing `bifrost-9.0.1/ChangeLog` & `bifrost-9.1.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,37 @@
 CHANGES
 =======
 
+9.1.0
+-----
+
+* [CI] Move Kolla testing to CentOS Stream
+* Revert "libvirt: pin edk2-ovmf for CentOS Stream"
+* Recognize TOX\_CONSTRAINTS\_FILE as a valid constraints variable
+* Install DIB dependencies in bifrost-ironic-install role
+* Add OFTC network channel to contributor docs
+* libvirt: pin edk2-ovmf for CentOS Stream
+* Point ipa-builder to stable/wallaby
+* Install squashfs-tools for Ubuntu image builds
+* Use explicit path for which
+* Increase memory of vm to adjust for new tinyipa
+* Upgrade pip version to fix pep-517 enforcing
+* Fix the Debian Buster version number
+* Restore the conditional verbosity in bash scripts
+* Misplaced variable preventing fast-track after inspection
+* Exit on all errors in bash scripts when possible
+* Install at least pip version 19.1.1
+* Collect firewalld info if present
+* docs: explain OS support in terms of two tiers
+* Fix passing parameters with spaces to bifrost-cli
+* Remove lower-constraints job
+* Switch to CentOS 8 Stream for testing
+* Fix two CI issues
+* Fix missing node facts with BIFROST\_INVENTORY\_SOURCE=ironic
+
 9.0.1
 -----
 
 * Fix handling rootwrap.d filters
 * Ensure PATH contains the virtual environment when validating CLI
 * Specify mandatory name parameter for virt\_net
 * Explicitly open ports 68 and 69 on Ubuntu
```

### Comparing `bifrost-9.0.1/LICENSE` & `bifrost-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/PKG-INFO` & `bifrost-9.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bifrost
-Version: 9.0.1
+Version: 9.1.0
 Summary: Deployment of physical machines using OpenStack Ironic and Ansible
 Home-page: https://docs.openstack.org/bifrost/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Bifrost
         -------
```

### Comparing `bifrost-9.0.1/README.rst` & `bifrost-9.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/bifrost/__init__.py` & `bifrost-9.1.0/bifrost/__init__.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/bifrost/cli.py` & `bifrost-9.1.0/bifrost/cli.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/bifrost/inventory.py` & `bifrost-9.1.0/bifrost/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,16 +227,15 @@
     machines = cloud.list_machines()
 
     node_names = os.environ.get('BIFROST_NODE_NAMES', None)
     if node_names:
         node_names = node_names.split(',')
 
     for machine in machines:
-        if 'properties' not in machine:
-            machine = cloud.get_machine(machine['uuid'])
+        machine = cloud.get_machine(machine['uuid'])
         if machine['name'] is None:
             name = machine['uuid']
         else:
             name = machine['name']
 
         if node_names and name not in node_names:
             continue
```

### Comparing `bifrost-9.0.1/bifrost/tests/base.py` & `bifrost-9.1.0/bifrost/tests/base.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/bifrost/tests/functional/test_inventory_functional.py` & `bifrost-9.1.0/bifrost/tests/functional/test_inventory_functional.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/bifrost/tests/unit/test_cli.py` & `bifrost-9.1.0/bifrost/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/bifrost/tests/unit/test_inventory.py` & `bifrost-9.1.0/bifrost/tests/unit/test_inventory.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,26 +40,34 @@
 
     @mock.patch.object(openstack, 'connect', autospec=True)
     def test__process_sdk(self, mock_sdk):
         (groups, hostvars) = inventory._prepare_inventory()
         mock_cloud = mock_sdk.return_value
         mock_cloud.list_machines.return_value = [
             {
-                'driver_info': {
-                    'ipmi_address': '1.2.3.4',
-                },
+                'driver_info': None,
                 'links': [],
                 'name': 'node1',
                 'ports': [],
-                'properties': {
-                    'cpus': 42,
-                },
+                'properties': None,
                 'uuid': 'f3fbf7c6-b4e9-4dd2-8ca0-c74a50f8be45',
             },
         ]
+        mock_cloud.get_machine.return_value = {
+            'driver_info': {
+                'ipmi_address': '1.2.3.4',
+            },
+            'links': [],
+            'name': 'node1',
+            'ports': [],
+            'properties': {
+                'cpus': 42,
+            },
+            'uuid': 'f3fbf7c6-b4e9-4dd2-8ca0-c74a50f8be45',
+        }
         mock_cloud.list_nics_for_machine.return_value = [
             {
                 'address': '00:11:22:33:44:55',
                 'uuid': 'e2be93b5-a8f6-46a2-bec7-571b8ecf2938',
             },
         ]
         (groups, hostvars) = inventory._process_sdk(groups, hostvars)
@@ -90,26 +98,34 @@
 
     @mock.patch.object(openstack, 'connect', autospec=True)
     def test__process_sdk_multiple_nics(self, mock_sdk):
         (groups, hostvars) = inventory._prepare_inventory()
         mock_cloud = mock_sdk.return_value
         mock_cloud.list_machines.return_value = [
             {
-                'driver_info': {
-                    'ipmi_address': '1.2.3.4',
-                },
+                'driver_info': None,
                 'links': [],
                 'name': 'node1',
                 'ports': [],
-                'properties': {
-                    'cpus': 42,
-                },
+                'properties': None,
                 'uuid': 'f3fbf7c6-b4e9-4dd2-8ca0-c74a50f8be45',
             },
         ]
+        mock_cloud.get_machine.return_value = {
+            'driver_info': {
+                'ipmi_address': '1.2.3.4',
+            },
+            'links': [],
+            'name': 'node1',
+            'ports': [],
+            'properties': {
+                'cpus': 42,
+            },
+            'uuid': 'f3fbf7c6-b4e9-4dd2-8ca0-c74a50f8be45',
+        }
         mock_cloud.list_nics_for_machine.return_value = [
             {
                 'address': '00:11:22:33:44:55',
                 'uuid': 'e2be93b5-a8f6-46a2-bec7-571b8ecf2938',
             },
             {
                 'address': '00:11:22:33:44:56',
```

### Comparing `bifrost-9.0.1/bifrost/tests/utils.py` & `bifrost-9.1.0/bifrost/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/bifrost/version.py` & `bifrost-9.1.0/bifrost/version.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/bifrost.egg-info/PKG-INFO` & `bifrost-9.1.0/bifrost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bifrost
-Version: 9.0.1
+Version: 9.1.0
 Summary: Deployment of physical machines using OpenStack Ironic and Ansible
 Home-page: https://docs.openstack.org/bifrost/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Bifrost
         -------
```

### Comparing `bifrost-9.0.1/bifrost.egg-info/SOURCES.txt` & `bifrost-9.1.0/bifrost.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,14 @@
 playbooks/roles/bifrost-create-bootable-image/meta/main.yml
 playbooks/roles/bifrost-create-bootable-image/tasks/create_bootable_image.yml
 playbooks/roles/bifrost-create-bootable-image/tasks/main.yml
 playbooks/roles/bifrost-create-dib-image/README.md
 playbooks/roles/bifrost-create-dib-image/defaults/main.yml
 playbooks/roles/bifrost-create-dib-image/meta/main.yml
 playbooks/roles/bifrost-create-dib-image/tasks/main.yml
-playbooks/roles/bifrost-create-dib-image/vars/main.yml
 playbooks/roles/bifrost-create-vm-nodes/README.md
 playbooks/roles/bifrost-create-vm-nodes/defaults/dummy-defaults.yml
 playbooks/roles/bifrost-create-vm-nodes/defaults/main.yml
 playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_CentOS.yml
 playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Debian.yml
 playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_Fedora.yml
 playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_RedHat.yml
@@ -166,14 +165,15 @@
 playbooks/roles/bifrost-ironic-install/templates/inspector-default-boot-ipxe.j2
 playbooks/roles/bifrost-ironic-install/templates/ironic-inspector.conf.j2
 playbooks/roles/bifrost-ironic-install/templates/ironic-prometheus-exporter.service.j2
 playbooks/roles/bifrost-ironic-install/templates/ironic.conf.j2
 playbooks/roles/bifrost-ironic-install/templates/nginx.conf.j2
 playbooks/roles/bifrost-ironic-install/templates/static.hosts.j2
 playbooks/roles/bifrost-ironic-install/templates/systemd_template.j2
+playbooks/roles/bifrost-ironic-install/vars/main.yml
 playbooks/roles/bifrost-keystone-client-config/README.md
 playbooks/roles/bifrost-keystone-client-config/defaults/main.yml
 playbooks/roles/bifrost-keystone-client-config/meta/main.yml
 playbooks/roles/bifrost-keystone-client-config/tasks/main.yml
 playbooks/roles/bifrost-keystone-client-config/tasks/validate.yml
 playbooks/roles/bifrost-keystone-client-config/templates/clouds.yaml.j2
 playbooks/roles/bifrost-keystone-client-config/templates/openrc.j2
@@ -261,14 +261,15 @@
 releasenotes/notes/bifrost-inspector-a154561802d8d614.yaml
 releasenotes/notes/bifrost-openstack-ci-prep-172cbb159e0a2b78.yaml
 releasenotes/notes/bifrost-role-auth-support-ea6b5571cd339aa2.yaml
 releasenotes/notes/bifrost_node_names-f26ca2eab7e261d6.yaml
 releasenotes/notes/bionic-centos8-ci-5047b40c6ba51484.yaml
 releasenotes/notes/bump-ansible-version-35c201d1d6d30860.yaml
 releasenotes/notes/centos-keystone-acad21e70153067d.yaml
+releasenotes/notes/centos8-stream-0c6d9adb544e36af.yaml
 releasenotes/notes/change-default-vnic-type-a4ba179ea8f9792d.yaml
 releasenotes/notes/change-inspector-to-use-mysql-17cb03cabb958ff9.yaml
 releasenotes/notes/change-ipa-version-cacaec52a55188cc.yaml
 releasenotes/notes/ci-testing-faa63db25ebc94df.yaml
 releasenotes/notes/cirros-0.5.1-d09a433cbea1a3b9.yaml
 releasenotes/notes/cleaning-9b4241342320f315.yaml
 releasenotes/notes/cli-validate-474e15ba9631e72f.yaml
@@ -305,22 +306,24 @@
 releasenotes/notes/fedora-core-25-support-b9f8f258a9738a06.yaml
 releasenotes/notes/fedora-firewalld-f8e2e15be5fe43fd.yaml
 releasenotes/notes/firewalld-d53c6396828b91ee.yaml
 releasenotes/notes/firewalld-services-4c255c02d8d427f8.yaml
 releasenotes/notes/firewalld-zone-d8c72fb5924a4916.yaml
 releasenotes/notes/fix-deploy-logs-175fb352c5730b58.yaml
 releasenotes/notes/fix-inspection-with-inventory-dhcp-cfc236974bf4ed0a.yaml
+releasenotes/notes/fix-story-2008394-9a77486a838a1f2c.yaml
 releasenotes/notes/focal-36208207a571f354.yaml
 releasenotes/notes/focal-e40fdd37d11faac9.yaml
 releasenotes/notes/generated-ipa-url-protocol-1a5a2bfc8e20db9b.yaml
 releasenotes/notes/git-url-root-c81478d395f66e46.yaml
 releasenotes/notes/http-basic-40df399ea63956aa.yaml
 releasenotes/notes/hw-types-17106c0397f34ef1.yaml
 releasenotes/notes/images-permissions-2042490e3ca13656.yaml
 releasenotes/notes/initial-release-notes-937001279bbb52cd.yaml
+releasenotes/notes/inspect-fast-track-36007cc32bdf7e5c.yaml
 releasenotes/notes/inspector-keystone-support-3786a22b49e851e5.yaml
 releasenotes/notes/inspector-no-longer-powers-off-796801e809184eee.yaml
 releasenotes/notes/inspector-processing-hooks-addf80be5f31aa61.yaml
 releasenotes/notes/inspector-pxe-args-c65acb610507ab08.yaml
 releasenotes/notes/inspector-ramdisk-logs-0db7c111fd455cec.yaml
 releasenotes/notes/install-SUDO_USER-fix-2bf577269008587f.yaml
 releasenotes/notes/install-osc-c179e673dc338ab3.yaml
@@ -351,14 +354,15 @@
 releasenotes/notes/log-directories-87b86df40464bb2d.yaml
 releasenotes/notes/logging-bcc7d552944c94e4.yaml
 releasenotes/notes/managed-inspection-options-2764b4ae0079f505.yaml
 releasenotes/notes/manual-management-c204a200b0f0e6e0.yaml
 releasenotes/notes/merge-test-playbooks-aeabc7a614cbce29.yaml
 releasenotes/notes/metalsmith-7044429597a5f137.yaml
 releasenotes/notes/more-clouds-7c0fccf5701918d7.yaml
+releasenotes/notes/move-dib-deps-install-8a8aafc060461dc0.yaml
 releasenotes/notes/move-to-tinyipa-8c7840b73c40a9e8.yaml
 releasenotes/notes/mysql-database-separation-d6bf9a4f22cd8bbb.yaml
 releasenotes/notes/no-classic-drivers-0b8a346bcab8a004.yaml
 releasenotes/notes/no-clone-cebedc81211dcfa5.yaml
 releasenotes/notes/no-csv-b7f149e88aba1b85.yaml
 releasenotes/notes/no-osc-b39d14591103b2c3.yaml
 releasenotes/notes/no-rabbit-95434aaea3bb5528.yaml
@@ -369,14 +373,15 @@
 releasenotes/notes/nossh-16577ec5c3b82594.yaml
 releasenotes/notes/ocata-summary-040e557460bab2bc.yaml
 releasenotes/notes/old-network-info-33a853faf6d6c6d0.yaml
 releasenotes/notes/openstacksdk-addition-efec3878ef988295.yaml
 releasenotes/notes/os_client_config-support-b1073062d842febb.yaml
 releasenotes/notes/override-dhcp-boot-6659585b75d58757.yaml
 releasenotes/notes/override_upper_constraints-79f837d8ac58e53d.yaml
+releasenotes/notes/params-ab98e0ac242d119a.yaml
 releasenotes/notes/passing-no-proxy-32191c148442c57d.yaml
 releasenotes/notes/pin-proliantutils-60f1facf44c223ca.yaml
 releasenotes/notes/populate_dns_servers_dnsmasq-4f30a9957e8de732.yaml
 releasenotes/notes/populate_domain_dnsmasq-5408896247eb39b4.yaml
 releasenotes/notes/populate_ntp_servers_dnsmasq-249d2a26b94b0bf1.yaml
 releasenotes/notes/pxe-acl-26f3be809caa0c88.yaml
 releasenotes/notes/pxe-driver-support-e2d8a769bf910dbc.yaml
@@ -389,14 +394,15 @@
 releasenotes/notes/remove-ucs-drivers-37f46fa8500f9ddb.yaml
 releasenotes/notes/remove-ucssdk-e61762195a7c8b4d.yaml
 releasenotes/notes/repo-owner-41db02a4d0406a7a.yaml
 releasenotes/notes/resource-class-243535c9049cbd73.yaml
 releasenotes/notes/sdk-source-1bd77dbd11b08577.yaml
 releasenotes/notes/selinux-lnk_file-527ac51c60f9c2ad.yaml
 releasenotes/notes/skip-install-bfd642f5065cf304.yaml
+releasenotes/notes/squashfs-ddbbbac856e8f9fc.yaml
 releasenotes/notes/store-data-a14351976eda9842.yaml
 releasenotes/notes/store-introspection-data-bc4f2fef2f5bb543.yaml
 releasenotes/notes/support-custom-ansible-groups-38ad5d3a930b17eb.yaml
 releasenotes/notes/support-fedora-3b14bffb24097b28.yaml
 releasenotes/notes/support-remote-logging-93e159eeef4cc68b.yaml
 releasenotes/notes/support-staging-drivers-1c398a56dde9b240.yaml
 releasenotes/notes/suse-ipxe-ce4f1bf07db78860.yaml
```

### Comparing `bifrost-9.0.1/bindep.txt` & `bifrost-9.1.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/conf.py` & `bifrost-9.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/contributor/testenv.rst` & `bifrost-9.1.0/doc/source/contributor/testenv.rst`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 Command::
 
   scripts/test-bifrost.sh
 
 Note:
 
 - In order to cap requirements for installation, an ``upper_constraints_file``
-  setting is defined. This is consuming the ``UPPER_CONSTRAINTS_FILE`` env
-  var by default, to properly integrate with CI systems, and will default
-  to ``/opt/stack/requirements/upper-constraints.txt`` file if not present.
+  setting is defined. This is consuming the ``UPPER_CONSTRAINTS_FILE`` or
+  ``TOX_CONSTRAINTS_FILE`` env var by default, to properly integrate with CI
+  systems, and will default to
+  ``/opt/stack/requirements/upper-constraints.txt`` file if not present.
 
 Manually test with Virtual Machines
 ===================================
 
 Bifrost supports using virtual machines to emulate the hardware.
 
 The VirtualBMC_ project is used as an IPMI proxy, so that the same ``ipmi``
```

### Comparing `bifrost-9.0.1/doc/source/contributor/vagrant.rst` & `bifrost-9.1.0/doc/source/contributor/vagrant.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/contributor/virsh.rst` & `bifrost-9.1.0/doc/source/contributor/virsh.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/install/index.rst` & `bifrost-9.1.0/doc/source/install/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,45 @@
 ============
 Introduction
 ============
 
 This document will guide you through installing the Bare Metal Service (ironic)
 using Bifrost.
 
-Requirements
-============
+Supported operating systems
+===========================
+
+1st tier support (fully tested in the CI, no known or potential issues):
+
+* CentOS Stream 8
+* Ubuntu 20.04 "Focal"
+* Debian 10 "Buster"
+
+2nd tier support (limited testing or known issues):
+
+* Ubuntu 18.04 "Bionic"
+
+  Tested in the Bifrost CI, but no longer tested in the ironic upstream CI.
 
-Supported operating systems:
+* RHEL 8 and regular CentOS 8
+
+  Only tested indirectly via CentOS Stream 8.
+
+* openSUSE Leap 15.2
+
+  Tested in the CI but has frequent issues.
 
-* Ubuntu 18.04, 20.04
-* Red Hat Enterprise Linux (RHEL) 8
-* CentOS 8
-* openSUSE Leap 15.2 (15.1 is supported but not recommended)
 * Fedora 32 (30 is supported but not recommended)
-* Debian Buster
+
+  Only the latest Fedora is tested in the CI.
+
+.. note::
+   Operating systems evolve and so does the support for them, even on stable
+   branches. This especially concerns Fedora, which is evolving faster than
+   other distributions.
 
 Bifrost structure
 =================
 
 Installation and use of Bifrost is split into roughly three steps:
 
 - **install**:
```

### Comparing `bifrost-9.0.1/doc/source/install/keystone.rst` & `bifrost-9.1.0/doc/source/install/keystone.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/install/offline-install.rst` & `bifrost-9.1.0/doc/source/install/offline-install.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/user/dhcp.rst` & `bifrost-9.1.0/doc/source/user/dhcp.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/user/howto.rst` & `bifrost-9.1.0/doc/source/user/howto.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/user/keystone.rst` & `bifrost-9.1.0/doc/source/user/keystone.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/doc/source/user/troubleshooting.rst` & `bifrost-9.1.0/doc/source/user/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/lower-constraints.txt` & `bifrost-9.1.0/lower-constraints.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 cffi==1.13.0
 chardet==3.0.4
 cliff==3.1.0
 cmd2==0.8.9
 coverage==4.0
 cryptography==2.2.1
 debtcollector==1.19.0
-doc8==0.6.0
 docutils==0.14
 extras==1.0.0
 fixtures==3.0.0
 future==0.18.2
 idna==2.6
 iso8601==0.1.12
-keystoneauth1==3.4.0
+keystoneauth1==3.18.0
 linecache2==1.0.0
 monotonic==1.4
 mox3==0.25.0
 msgpack==0.5.6
 netaddr==0.7.19
 netifaces==0.10.6
 openstacksdk==0.37.0
@@ -32,15 +31,14 @@
 oslo.serialization==2.25.0
 oslo.utils==3.36.0
 passlib==1.7.2
 pbr==2.0.0
 prettytable==0.7.2
 pyasn1==0.4.2
 pycparser==2.18
-Pygments==2.2.0
 pyinotify==0.9.6
 pyOpenSSL==18.0.0
 pyparsing==2.2.0
 pyperclip==1.8.0
 python-dateutil==2.7.0
 python-mimeparse==1.6.0
 python-subunit==1.2.0
```

### Comparing `bifrost-9.0.1/playbooks/ci/run.yaml` & `bifrost-9.1.0/playbooks/ci/run.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/enroll-dynamic.yaml` & `bifrost-9.1.0/playbooks/enroll-dynamic.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/example-deploy-all-available-nodes.yaml` & `bifrost-9.1.0/playbooks/example-deploy-all-available-nodes.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/install.yaml` & `bifrost-9.1.0/playbooks/install.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/inventory/baremetal.csv.example` & `bifrost-9.1.0/playbooks/inventory/baremetal.csv.example`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/inventory/baremetal.json.example` & `bifrost-9.1.0/playbooks/inventory/baremetal.json.example`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/inventory/baremetal.yml.example` & `bifrost-9.1.0/playbooks/inventory/baremetal.yml.example`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/inventory/bifrost_inventory.py` & `bifrost-9.1.0/playbooks/inventory/bifrost_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,16 +227,15 @@
     machines = cloud.list_machines()
 
     node_names = os.environ.get('BIFROST_NODE_NAMES', None)
     if node_names:
         node_names = node_names.split(',')
 
     for machine in machines:
-        if 'properties' not in machine:
-            machine = cloud.get_machine(machine['uuid'])
+        machine = cloud.get_machine(machine['uuid'])
         if machine['name'] is None:
             name = machine['uuid']
         else:
             name = machine['name']
 
         if node_names and name not in node_names:
             continue
```

### Comparing `bifrost-9.0.1/playbooks/inventory/group_vars/baremetal` & `bifrost-9.1.0/playbooks/inventory/group_vars/baremetal`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/inventory/group_vars/localhost` & `bifrost-9.1.0/playbooks/inventory/group_vars/localhost`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # to both the baremetal and localhost groups.  If the file is already on
 # disk, then the image generation will not take place, otherwise an image
 # will be generated using diskimage-builder.
 # deploy_image_filename: "deployment_image.qcow2"
 # deploy_image: "{{http_boot_folder}}/{{deploy_image_filename}}"
 
 # Setting to utilize diskimage-builder to create a bootable image.
-create_image_via_dib: true
+create_image_via_dib: "{{ not use_cirros | default(false) | bool }}"
 dib_image_type: vm
 
 # Create IPA image instead of downloading an pre-made IPA image.
 create_ipa_image: false
 
 # Dnsmasq default route for clients. If not defined, dnsmasq will push to
 # clients as default route the same IP of the dnsmasq server.
```

### Comparing `bifrost-9.0.1/playbooks/inventory/group_vars/target` & `bifrost-9.1.0/playbooks/inventory/group_vars/target`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # to both the baremetal and localhost groups.  If the file is already on
 # disk, then the image generation will not take place, otherwise an image
 # will be generated using diskimage-builder.
 # deploy_image_filename: "deployment_image.qcow2"
 # deploy_image: "{{http_boot_folder}}/{{deploy_image_filename}}"
 
 # Setting to utilize diskimage-builder to create a bootable image.
-create_image_via_dib: true
+create_image_via_dib: "{{ not use_cirros | default(false) | bool }}"
 dib_image_type: vm
 
 # Create IPA image instead of downloading an pre-made IPA image.
 create_ipa_image: false
 
 # Dnsmasq default route for clients. If not defined, dnsmasq will push to
 # clients as default route the same IP of the dnsmasq server.
```

### Comparing `bifrost-9.0.1/playbooks/library/network_metadata.py` & `bifrost-9.1.0/playbooks/library/network_metadata.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/library/os_ironic_facts.py` & `bifrost-9.1.0/playbooks/library/os_ironic_facts.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/library/os_ironic_node_info.py` & `bifrost-9.1.0/playbooks/library/os_ironic_node_info.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/redeploy-dynamic.yaml` & `bifrost-9.1.0/playbooks/redeploy-dynamic.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-cloud-config/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-cloud-config/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/tasks/ssh_public_key_path.yaml` & `bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/tasks/ssh_public_key_path.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-configdrives-dynamic/tasks/update_facts_from_ironic.yaml` & `bifrost-9.1.0/playbooks/roles/bifrost-configdrives-dynamic/tasks/update_facts_from_ironic.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/tasks/create_bootable_image.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/tasks/create_bootable_image.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-bootable-image/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-bootable-image/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-dib-image/tasks/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ---
-- name: Ensure required packages are installed
-  package:
-    name: "{{ dib_host_required_packages }}"
-    state: present
-  when: not skip_package_install | bool
 # If attempting to utilize a base Ubuntu image, diskimage-builder
 # is the recommended, and default path.
 - name: "Test if image is present"
   stat: path={{ dib_imagename }}
   register: test_image_present
 - name: "Test if image is present - {{ dib_imagename }}.{{ dib_imagetype | default('qcow2') }}"
   stat: path={{ dib_imagename }}.{{ dib_imagetype | default('qcow2') }}
@@ -182,23 +177,14 @@
       {{ dib_qemuopts_arg|default('') }}
       {{ dib_rootlabel_arg|default('') }}
       {{ dib_rdelement_arg|default('') }}
       {{ dib_installtype_arg|default('') }}
       {{ dib_packages_arg|default('') }}
       {{ dib_os_element }}
       {{ dib_elements|default('') }}
-- name: Install debootstrap if building a Debian image
-  package:
-    name: debootstrap
-    state: present
-  when:
-    - not test_image_present.stat.exists
-    - not test_image_dib_present.stat.exists
-    - not test_image_initramfs_present.stat.exists
-    - ("debian" in dib_os_element or "ubuntu" in dib_os_element)
 - name: "Initiate image build"
   command: disk-image-create {{ dib_arglist }}
   environment: "{{ dib_env_vars_final | combine(bifrost_venv_env) }}"
   when:
     - not build_ramdisk | bool
     - not test_image_present.stat.exists
     - not test_image_dib_present.stat.exists
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-dib-image/vars/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/tasks/main.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright (c) 2017 SUSE Linux GmbH.
+# Copyright (c) 2016 Hewlett-Packard Development Company, L.P.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-# implied.
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-dib_host_required_packages:
-  - dosfstools
-  - e2fsprogs
-  - gdisk
-  - xfsprogs
+---
+- name: Execute python dhcp check file
+  become: true
+  script: test-dhcp.py "{{ inventory_dhcp }}" "{{ inventory_dhcp_static_ip }}"
+  args:
+    executable: "{{ ansible_python.executable }}"
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -45,13 +45,17 @@
 
 git_branch: master
 git_root: "/opt/stack"
 git_url_root: https://opendev.org
 reqs_git_url: "{{ git_url_root }}/openstack/requirements"
 reqs_git_folder: "{{ git_root }}/requirements"
 reqs_git_branch: "{{ git_branch }}"
-upper_constraints_file: "{{ lookup('env', 'UPPER_CONSTRAINTS_FILE') | default(reqs_git_folder + '/upper-constraints.txt', True) }}"
+upper_constraints_file: >-
+  {{ lookup('env', 'UPPER_CONSTRAINTS_FILE')
+     | default(lookup('env', 'TOX_CONSTRAINTS_FILE'), True)
+     | default(reqs_git_folder + '/upper-constraints.txt', True) }}
+
 update_repos: true
 force_update_repos: true
 
 # Conditional variables utilized based on CI or manual testing options.
 copy_from_local_path: false
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_CentOS.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/defaults/required_defaults_CentOS.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/tasks/create_vm.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/tasks/create_vm.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/tasks/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,21 @@
     - "../defaults/dummy-defaults.yml"
 
 - name: "Install required packages"
   package:
     name: "{{ required_packages }}"
     state: present
 
+# NOTE(dtantsur): workaround for https://bugzilla.redhat.com/show_bug.cgi?id=1840485
+- name: "Work around libgrypt issue on RHEL/CentOS 8.3"
+  package:
+    name: libgcrypt
+    state: latest
+  when: ansible_distribution in ['RedHat', 'CentOS']
+
 - name: ensure installation root folder exists
   become: yes
   file:
     state: directory
     dest: "{{ git_root }}"
     owner: "{{ ansible_user_id }}"
     group: "{{ ansible_user_gid }}"
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/tasks/prepare_libvirt.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/tasks/prepare_libvirt.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-create-vm-nodes/templates/testvm.xml.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-create-vm-nodes/templates/testvm.xml.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-deploy-nodes-dynamic/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-deploy-nodes-dynamic/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 openstacksdk_source_install: false
 ironicinspector_source_install: true
 ironicinspectorclient_source_install: false
 sushy_source_install: false
 staging_drivers_source_install: true
 prometheus_exporter_source_install: true
 # Setting to utilize diskimage-builder to create a bootable image.
-create_image_via_dib: true
+create_image_via_dib: "{{ not use_cirros | default(false) | bool }}"
+create_ipa_image: false
 dib_image_type: vm
+dib_os_element: "debian"
 # Setting to install diskimage-builder
-install_dib: "{{ create_image_via_dib }}"
+install_dib: "{{ create_image_via_dib | bool or create_ipa_image | bool }}"
 # If testing is true, then the environment is setup for using libvirt
 # virtual machines for the hardware instead of real hardware.
 testing: false
 
 # set to true to skip installation completely
 skip_install: False
 # set to true to skip installing ironic dependencies
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Debian_family.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Debian_family.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Fedora.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Fedora.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_RedHat_family.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_RedHat_family.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Suse_family.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Suse_family.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Ubuntu.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/defaults/required_defaults_Ubuntu.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/bootstrap.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/create_tftpboot.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/create_tftpboot.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/download_ipa_image.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/download_ipa_image.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/get_ipxe.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/get_ipxe.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/hw_types.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/hw_types.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/inspector_bootstrap.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/inspector_bootstrap.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/inspector_install.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/inspector_install.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/inspector_start.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/inspector_start.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/install.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/install.yml`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,20 @@
     name: bifrost-pip-install
   vars:
     package: diskimage-builder
     sourcedir: "{{ dib_git_folder }}"
     source_install: true
   when: install_dib | bool
 
+- name: Ensure required packages are installed
+  package:
+    name: "{{ dib_host_required_packages | select | list }}"
+    state: present
+  when: install_dib | bool
+
 - name: "sushy - Install"
   include_role:
     name: bifrost-pip-install
   vars:
     package: sushy
     sourcedir: "{{ sushy_git_folder }}"
     source_install: "{{ sushy_source_install }}"
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/ironic_config.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/ironic_config.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/keystone_setup.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/keystone_setup.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/keystone_setup_inspector.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/keystone_setup_inspector.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/migrations.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/migrations.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/prometheus_exporter_install.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/prometheus_exporter_install.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/prometheus_exporter_start.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/prometheus_exporter_start.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/set_ssh_private_key.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/set_ssh_private_key.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/setup_firewalld.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/setup_firewalld.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/staging_install.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/staging_install.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/start.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/start.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/validate.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/validate.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/tasks/vendor_deps.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/tasks/vendor_deps.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/dnsmasq.conf.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/dnsmasq.conf.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/ironic-inspector.conf.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/ironic-inspector.conf.j2`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 ramdisk_logs_dir = {{ inspector_ramdisk_logs_local_path }}
 {% endif %}
 always_store_ramdisk_logs = {{ inspector_store_ramdisk_logs | default('true') | bool }}
 {% if inspector_processing_hooks is defined %}
 processing_hooks = {{ inspector_processing_hooks }}
 {% endif %}
 store_data = database
+power_off = {{ power_off_after_inspection }}
+
 {% if inspector.discovery.enabled == true %}
 node_not_found_hook = enroll
-power_off = {{ power_off_after_inspection }}
 
 [discovery]
 enroll_node_driver = {{ inspector.discovery.default_node_driver }}
 {% endif %}
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/ironic.conf.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/ironic.conf.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-ironic-install/templates/nginx.conf.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-ironic-install/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/tasks/validate.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/tasks/validate.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/templates/clouds.yaml.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/templates/clouds.yaml.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-client-config/templates/openrc.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-client-config/templates/openrc.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/bootstrap.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/install.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/install.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/start.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/start.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/tasks/upgrade.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/tasks/upgrade.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/keystone.conf.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/keystone.conf.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/nginx.conf.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-keystone-install/templates/nginx_conf.d_bifrost-keystone.conf.j2` & `bifrost-9.1.0/playbooks/roles/bifrost-keystone-install/templates/nginx_conf.d_bifrost-keystone.conf.j2`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-pip-install/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-pip-install/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-pip-install/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-pip-install/defaults/main.yml`

 * *Files 26% similar despite different names*

```diff
@@ -12,8 +12,11 @@
 developer_mode: false
 extra_args:
 pip_install_retries: 5
 pip_install_delay: 10
 reqs_git_folder: /opt/stack/requirements
 state: present
 version:
-upper_constraints_file: "{{ lookup('env', 'UPPER_CONSTRAINTS_FILE') | default(reqs_git_folder + '/upper-constraints.txt', True) }}"
+upper_constraints_file: >-
+  {{ lookup('env', 'UPPER_CONSTRAINTS_FILE')
+     | default(lookup('env', 'TOX_CONSTRAINTS_FILE'), True)
+     | default(reqs_git_folder + '/upper-constraints.txt', True) }}
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-pip-install/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-pip-install/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/defaults/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ironicinspector_git_branch: "{{ git_branch }}"
 ironicinspectorclient_git_branch: "{{ git_branch }}"
 reqs_git_branch: "{{ git_branch }}"
 staging_drivers_git_branch: "{{ git_branch }}"
 keystone_git_branch: "{{ git_branch }}"
 sushy_git_branch: "{{ git_branch }}"
 ipa_git_branch: "{{ git_branch }}"
-ipa_builder_git_branch: master
+ipa_builder_git_branch: stable/wallaby
 prometheus_exporter_git_branch: "{{ git_branch }}"
 # disable source install to prevent cloning
 ironicclient_source_install: false
 openstacksdk_source_install: false
 ironicinspector_source_install: true
 ironicinspectorclient_source_install: false
 sushy_source_install: false
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-prep-for-install/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-prep-for-install/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-prepare-for-test-dynamic/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-prepare-for-test-dynamic/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/files/test-dhcp.py` & `bifrost-9.1.0/playbooks/roles/bifrost-test-dhcp/files/test-dhcp.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-dhcp/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/tasks/main.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-# Copyright (c) 2016 Hewlett-Packard Development Company, L.P.
+# Copyright (c) 2015 Hewlett-Packard Development Company, L.P.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ---
-- name: Execute python dhcp check file
-  become: true
-  script: test-dhcp.py "{{ inventory_dhcp }}" "{{ inventory_dhcp_static_ip }}"
-  args:
-    executable: "{{ ansible_python.executable }}"
+- import_role:
+    name: bifrost-cloud-config
+
+- name: "Delete hardware"
+  openstack.cloud.baremetal_node:
+    cloud: "{{ cloud_name | default(omit) }}"
+    auth_type: "{{ auth_type | default(omit) }}"
+    auth: "{{ auth | default(omit) }}"
+    ca_cert: "{{ tls_certificate_path | default(omit) }}"
+    ironic_url: "{{ ironic_url | default(omit) }}"
+    driver: ""
+    uuid: "{{ uuid | default() }}"
+    name: "{{ name | default() }}"
+    state: absent
+    nics: "{{ nics }}"
+    driver_info: "{}"
```

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/meta/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/meta/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-inspection/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-test-inspection/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-vm/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-test-vm/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-vm/meta/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-test-vm/meta/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-test-vm/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-test-vm/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-tls/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-tls/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-tls/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-tls/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-tls/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-tls/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/README.md` & `bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/bifrost-unprovision-node-dynamic/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/bifrost-unprovision-node-dynamic/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/ironic-delete-dynamic/README.md` & `bifrost-9.1.0/playbooks/roles/ironic-delete-dynamic/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/README.md` & `bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/ironic-enroll-dynamic/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/ironic-enroll-dynamic/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/ironic-inspect-node/README.md` & `bifrost-9.1.0/playbooks/roles/ironic-inspect-node/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/ironic-inspect-node/defaults/main.yml` & `bifrost-9.1.0/playbooks/roles/ironic-inspect-node/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/roles/ironic-inspect-node/tasks/main.yml` & `bifrost-9.1.0/playbooks/roles/ironic-inspect-node/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/test-bifrost-create-vm.yaml` & `bifrost-9.1.0/playbooks/test-bifrost-create-vm.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/playbooks/test-bifrost.yaml` & `bifrost-9.1.0/playbooks/test-bifrost.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/add-bindep-support-8f54b246a1d2bca5.yaml` & `bifrost-9.1.0/releasenotes/notes/add-bindep-support-8f54b246a1d2bca5.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/allow-custom-public-endpoints-ip-4662c246f029589e.yaml` & `bifrost-9.1.0/releasenotes/notes/allow-custom-public-endpoints-ip-4662c246f029589e.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/ansible-2.0-support-81fa15cc27c28ba8.yaml` & `bifrost-9.1.0/releasenotes/notes/ansible-2.0-support-81fa15cc27c28ba8.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/ansible-pip-install-2b66bd82ce9ed4f6.yaml` & `bifrost-9.1.0/releasenotes/notes/ansible-pip-install-2b66bd82ce9ed4f6.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/ansible-virt-0759a857daaacccf.yaml` & `bifrost-9.1.0/releasenotes/notes/ansible-virt-0759a857daaacccf.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/bifrost-role-auth-support-ea6b5571cd339aa2.yaml` & `bifrost-9.1.0/releasenotes/notes/bifrost-role-auth-support-ea6b5571cd339aa2.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/change-ipa-version-cacaec52a55188cc.yaml` & `bifrost-9.1.0/releasenotes/notes/change-ipa-version-cacaec52a55188cc.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/custom-partitioning-78d7ac12d80a993f.yaml` & `bifrost-9.1.0/releasenotes/notes/custom-partitioning-78d7ac12d80a993f.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/deprecate-classic-drivers-f88c53fa483aa7d5.yaml` & `bifrost-9.1.0/releasenotes/notes/deprecate-classic-drivers-f88c53fa483aa7d5.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/deprecate_node_network_info-8c5e1bc4df6b8097.yaml` & `bifrost-9.1.0/releasenotes/notes/deprecate_node_network_info-8c5e1bc4df6b8097.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/fedora-core-25-support-b9f8f258a9738a06.yaml` & `bifrost-9.1.0/releasenotes/notes/fedora-core-25-support-b9f8f258a9738a06.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/http-basic-40df399ea63956aa.yaml` & `bifrost-9.1.0/releasenotes/notes/http-basic-40df399ea63956aa.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/inspector-keystone-support-3786a22b49e851e5.yaml` & `bifrost-9.1.0/releasenotes/notes/inspector-keystone-support-3786a22b49e851e5.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/inspector-no-longer-powers-off-796801e809184eee.yaml` & `bifrost-9.1.0/releasenotes/notes/inspector-no-longer-powers-off-796801e809184eee.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/inventory_dhcp_provisioning_ipv4_address-d2779f1abc38324a.yaml` & `bifrost-9.1.0/releasenotes/notes/inventory_dhcp_provisioning_ipv4_address-d2779f1abc38324a.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/logging-bcc7d552944c94e4.yaml` & `bifrost-9.1.0/releasenotes/notes/logging-bcc7d552944c94e4.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/more-clouds-7c0fccf5701918d7.yaml` & `bifrost-9.1.0/releasenotes/notes/more-clouds-7c0fccf5701918d7.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/move-to-tinyipa-8c7840b73c40a9e8.yaml` & `bifrost-9.1.0/releasenotes/notes/move-to-tinyipa-8c7840b73c40a9e8.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/mysql-database-separation-d6bf9a4f22cd8bbb.yaml` & `bifrost-9.1.0/releasenotes/notes/mysql-database-separation-d6bf9a4f22cd8bbb.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/nossh-16577ec5c3b82594.yaml` & `bifrost-9.1.0/releasenotes/notes/nossh-16577ec5c3b82594.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/ocata-summary-040e557460bab2bc.yaml` & `bifrost-9.1.0/releasenotes/notes/ocata-summary-040e557460bab2bc.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/os_client_config-support-b1073062d842febb.yaml` & `bifrost-9.1.0/releasenotes/notes/os_client_config-support-b1073062d842febb.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/override-dhcp-boot-6659585b75d58757.yaml` & `bifrost-9.1.0/releasenotes/notes/override-dhcp-boot-6659585b75d58757.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/populate_domain_dnsmasq-5408896247eb39b4.yaml` & `bifrost-9.1.0/releasenotes/notes/populate_domain_dnsmasq-5408896247eb39b4.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/pxe-driver-support-e2d8a769bf910dbc.yaml` & `bifrost-9.1.0/releasenotes/notes/pxe-driver-support-e2d8a769bf910dbc.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/random-passwords-b33b8de010ee82b6.yaml` & `bifrost-9.1.0/releasenotes/notes/random-passwords-b33b8de010ee82b6.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/releasenote-341a5eebe6168aea.yaml` & `bifrost-9.1.0/releasenotes/notes/releasenote-341a5eebe6168aea.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/store-data-a14351976eda9842.yaml` & `bifrost-9.1.0/releasenotes/notes/store-data-a14351976eda9842.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/support-custom-ansible-groups-38ad5d3a930b17eb.yaml` & `bifrost-9.1.0/releasenotes/notes/support-custom-ansible-groups-38ad5d3a930b17eb.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/templated_ironic_conf-bd052f2b2897d37a.yaml` & `bifrost-9.1.0/releasenotes/notes/templated_ironic_conf-bd052f2b2897d37a.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/test-with-json-inventory-b05204009f880431.yaml` & `bifrost-9.1.0/releasenotes/notes/test-with-json-inventory-b05204009f880431.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/tls-988e725820bb8aca.yaml` & `bifrost-9.1.0/releasenotes/notes/tls-988e725820bb8aca.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/use_public_urls_endpoints-1220a7f4164696c3.yaml` & `bifrost-9.1.0/releasenotes/notes/use_public_urls_endpoints-1220a7f4164696c3.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/notes/verify-checksum-ipa-a73cf936d0ae2ce1.yaml` & `bifrost-9.1.0/releasenotes/notes/verify-checksum-ipa-a73cf936d0ae2ce1.yaml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/releasenotes/source/conf.py` & `bifrost-9.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/requirements.txt` & `bifrost-9.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/scripts/README.md` & `bifrost-9.1.0/scripts/README.md`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/scripts/collect-test-info.sh` & `bifrost-9.1.0/scripts/collect-test-info.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/bin/bash
 
 # Note(TheJulia): We should proceed with attempting to collect information
 # even if a command fails, and as such set -e should not be present.
-set -ux
-set -o pipefail
+set -uxo pipefail
 
 # Note(TheJulia): If there is a workspace variable, we want to utilize that as
 # the preference of where to put logs
 SCRIPT_HOME="$(cd "$(dirname "$0")" && pwd)"
 LOG_LOCATION="${LOG_LOCATION:-${SCRIPT_HOME}/../logs}"
 
 VERBOSE_LOGS="${VERBOSE_LOGS:-False}"
@@ -44,14 +43,19 @@
     sudo iptables -S &> ${iptables_dir}/iptables_all_saved_rules.txt
     if [[ "$VERBOSE_LOGS" == "True" ]]; then
         for table in filter raw security mangle nat; do
             sudo iptables -L -v -n -t ${table} &> ${iptables_dir}/iptables_${table}.log
         done
     fi
 fi
+
+if $(sudo firewall-cmd --version &>/dev/null); then
+    sudo firewall-cmd --list-all-zones &> ${LOG_LOCATION}/firewalld-zones.log
+fi
+
 if $(ip link &>/dev/null); then
     ip -s link &> ${LOG_LOCATION}/interface_counters.log
 fi
 
 mkdir -p ${LOG_LOCATION}/all
 sudo cp -a /var/log/* ${LOG_LOCATION}/all/.
 sudo chown -R $USER ${LOG_LOCATION}/all
```

### Comparing `bifrost-9.0.1/scripts/env-setup.sh` & `bifrost-9.1.0/scripts/env-setup.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/bin/bash
-set -eu
+
+set -euo pipefail
 
 . $(dirname $0)/install-deps.sh
 # NOTE(pas-ha) the above exports some useful variables like
 # $PYTHON , $PIP and $VENV depending on venv install or not
 
 DEFAULT_PIP_ANSIBLE='>=2.9,<2.10'
```

### Comparing `bifrost-9.0.1/scripts/install-deps.sh` & `bifrost-9.1.0/scripts/install-deps.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 #!/bin/bash
 
-set -eu
+set -euo pipefail
 
 if [[ "${BIFROST_TRACE:-}" == true ]]; then
     set -x
 fi
 
 declare -A PKG_MAP
 
+# NOTE(rpittau): we need a stable recent version of pip to avoid issues with
+# the cryptography package.
+PIP_MIN_REQ="20.0.1"
+PIP_TUPLE="(20, 0, 1)"
+
 # workaround: for latest bindep to work, it needs to use en_US local
 export LANG=en_US.UTF-8
 
 export VENV=${VENV:-/opt/stack/bifrost}
 
+# NOTE(dtantsur): change this when creating a stable branch
+BRANCH=${ZUUL_BRANCH:-victoria}
+CONSTRAINTS_FILE=${UPPER_CONSTRAINTS_FILE:-${TOX_CONSTRAINTS_FILE:-https://releases.openstack.org/constraints/upper/$BRANCH}}
+
 CHECK_CMD_PKGS=(
     python3-devel
     python3
     python3-pip
 )
 
 echo Detecting package manager
@@ -60,15 +69,15 @@
     if $(${CHECK_CMD} python3-cryptography &> /dev/null); then
         sudo -E apt-get remove -y python3-cryptography
     fi
     ;;
 
     rhel|fedora|centos)
     OS_FAMILY="RedHat"
-    PKG_MANAGER=$(which dnf || which yum)
+    PKG_MANAGER=$(/usr/bin/which dnf || /usr/bin/which yum)
     if [[ "${BIFROST_TRACE:-}" != true ]]; then
         PKG_MANAGER="$PKG_MANAGER --quiet"
     fi
     INSTALLER_CMD="sudo -H -E ${PKG_MANAGER} -y install"
     CHECK_CMD="rpm -q"
     PKG_MAP=(
         [python3]=python3
@@ -78,15 +87,15 @@
     EXTRA_PKG_DEPS=()
     sudo -E ${PKG_MANAGER} updateinfo
     ;;
 
     *) echo "ERROR: Supported package manager not found.  Supported: apt, dnf, yum, zypper"; exit 1;;
 esac
 
-echo Installing Python and PIP
+echo "Installing Python and PIP"
 
 for pkg in ${CHECK_CMD_PKGS[@]}; do
     if ! $(${CHECK_CMD} ${PKG_MAP[$pkg]} &>/dev/null); then
         ${INSTALLER_CMD} ${PKG_MAP[$pkg]}
     fi
 done
 
@@ -125,26 +134,27 @@
 # keeping the path even with -E.
 PYTHON="python3"
 PIP="${PYTHON} -m pip"
 if [[ "${BIFROST_TRACE:-}" != true ]]; then
     PIP="$PIP --quiet"
 fi
 
-$PYTHON << EOF
-import pip
-version = tuple(map(int, pip.__version__.split('.')))
-assert version >= (7, 1)
-EOF
+# NOTE(rpittau): we need a stable recent version of pip to avoid issues with
+# the cryptography package.
+PIP_REQUIRED=$($PYTHON -c "import pip; print(tuple(map(int, pip.__version__.split('.'))) >= $PIP_TUPLE)")
+if [[ $PIP_REQUIRED == "False" ]]; then
+    ${PIP} install "pip==$PIP_MIN_REQ"
+fi
 
 export PIP_OPTS="--upgrade-strategy only-if-needed"
 
 echo "Installing bindep"
 ${PIP} install bindep
 
 echo "Using Bindep to install binary dependencies"
 # bindep returns 1 if packages are missing
 bindep -b &> /dev/null || ${INSTALLER_CMD} $(bindep -b)
 
 echo "Installing Python requirements"
-${PIP} install -r "$(dirname $0)/../requirements.txt" -c ${UPPER_CONSTRAINTS_FILE:-https://releases.openstack.org/constraints/upper/victoria}
+${PIP} install -r "$(dirname $0)/../requirements.txt" -c "${CONSTRAINTS_FILE}"
 
 echo "Completed installation of basic dependencies."
```

### Comparing `bifrost-9.0.1/scripts/split_json.py` & `bifrost-9.1.0/scripts/split_json.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/scripts/test-bifrost.sh` & `bifrost-9.1.0/scripts/test-bifrost.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 
-set -eux
-set -o pipefail
+set -euxo pipefail
+
 export PYTHONUNBUFFERED=1
 SCRIPT_HOME="$(cd "$(dirname "$0")" && pwd)"
 BIFROST_HOME=$SCRIPT_HOME/..
 ANSIBLE_INSTALL_ROOT=${ANSIBLE_INSTALL_ROOT:-/opt/stack}
 USE_DHCP="${USE_DHCP:-false}"
 BUILD_IMAGE="${BUILD_IMAGE:-false}"
 BAREMETAL_DATA_FILE=${BAREMETAL_DATA_FILE:-'/tmp/baremetal.json'}
@@ -126,15 +126,15 @@
            --${task} \
            -e testing_user=${TESTING_USER}
 done
 
 # Create the test VMs
 ../bifrost-cli --debug testenv \
     --count ${TEST_VM_NUM_NODES} \
-    --memory ${VM_MEMORY_SIZE:-512} \
+    --memory ${VM_MEMORY_SIZE:-1024} \
     --disk ${VM_DISK:-5} \
     --inventory "${BAREMETAL_DATA_FILE}" \
     --driver ${TEST_VM_NODE_DRIVER:-ipmi} \
     --extra-vars git_url_root="${WORKSPACE:-https://opendev.org}" \
     ${VM_SETUP_EXTRA:-} \
     ${BIFROST_CLI_EXTRA:-}
```

### Comparing `bifrost-9.0.1/setup.cfg` & `bifrost-9.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/setup.py` & `bifrost-9.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/tools/ansible-lint.sh` & `bifrost-9.1.0/tools/ansible-lint.sh`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/tools/vagrant_dev_env/Vagrantfile` & `bifrost-9.1.0/tools/vagrant_dev_env/Vagrantfile`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/tools/vagrant_dev_env/vagrant.yml` & `bifrost-9.1.0/tools/vagrant_dev_env/vagrant.yml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/tools/virsh_dev_env/vm/baremetal.xml` & `bifrost-9.1.0/tools/virsh_dev_env/vm/baremetal.xml`

 * *Files identical despite different names*

### Comparing `bifrost-9.0.1/tox.ini` & `bifrost-9.1.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,20 @@
     -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/victoria}
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/test-requirements.txt
 commands = stestr run --slowest {posargs}
 passenv = http_proxy HTTP_PROXY https_proxy HTTPS_PROXY no_proxy NO_PROXY
 
 [testenv:pep8]
+deps =
+    Pygments>=2.2.0 # BSD license
+    doc8>=0.6.0 # Apache-2.0
+    flake8-import-order>=0.17.1 # LGPLv3
+    hacking>=3.1.0,<4.0.0 # Apache-2.0
+    pycodestyle>=2.0.0,<2.7.0 # MIT
 commands =
     flake8 {posargs}
     doc8 doc/source releasenotes/source README.rst CONTRIBUTING.rst MISSION.rst HACKING.rst
 
 [testenv:venv]
 commands = {posargs}
```

### Comparing `bifrost-9.0.1/zuul.d/bifrost-jobs.yaml` & `bifrost-9.1.0/zuul.d/bifrost-jobs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     post-run: playbooks/ci/post.yaml
     required-projects:
       - openstack/bifrost
       - openstack/diskimage-builder
       - openstack/ironic
       - openstack/ironic-inspector
       - openstack/ironic-python-agent
-      - openstack/ironic-python-agent-builder
+      - name: openstack/ironic-python-agent-builder
+        override-checkout: stable/wallaby
       - openstack/requirements
       - x/ironic-staging-drivers
 
 - job:
     name: bifrost-integration
     parent: bifrost-base
 
@@ -40,15 +41,15 @@
     name: bifrost-integration-dhcp-ubuntu-focal
     parent: bifrost-integration-dhcp
     nodeset: ubuntu-focal
 
 - job:
     name: bifrost-integration-dhcp-centos-8
     parent: bifrost-integration-dhcp
-    nodeset: centos-8
+    nodeset: centos-8-stream
 
 - job:
     name: bifrost-integration-dibipa-debian
     parent: bifrost-integration
     timeout: 7200
     vars:
       build_image: true
@@ -57,15 +58,15 @@
     name: bifrost-integration-dibipa-debian-ubuntu-focal
     parent: bifrost-integration-dibipa-debian
     nodeset: ubuntu-focal
 
 - job:
     name: bifrost-integration-dibipa-debian-centos-8
     parent: bifrost-integration-dibipa-debian
-    nodeset: centos-8
+    nodeset: centos-8-stream
 
 - job:
     name: bifrost-integration-tinyipa
     parent: bifrost-base
     timeout: 3600
     vars:
       noauth_mode: false
@@ -110,20 +111,20 @@
     parent: bifrost-integration-tinyipa-ubuntu-focal
     vars:
       cli_test: true
 
 - job:
     name: bifrost-integration-tinyipa-centos-8
     parent: bifrost-integration-tinyipa
-    nodeset: centos-8
+    nodeset: centos-8-stream
 
 - job:
     name: bifrost-integration-tinyipa-keystone-centos-8
     parent: bifrost-integration-tinyipa
-    nodeset: centos-8
+    nodeset: centos-8-stream
     required-projects:
       - openstack/keystone
       - openstack/ironic-prometheus-exporter
     vars:
       enable_keystone: true
       enable_tls: true
       test_driver: redfish
```

### Comparing `bifrost-9.0.1/zuul.d/project.yaml` & `bifrost-9.1.0/zuul.d/project.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 - project:
     templates:
       - openstack-python3-victoria-jobs
-      - openstack-lower-constraints-jobs
       - check-requirements
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - bifrost-tox-linters
         - bifrost-integration-tinyipa-ubuntu-focal
@@ -31,15 +30,15 @@
             voting: false
         - bifrost-cli-ubuntu-focal:
             voting: false
         - bifrost-collections-src:
             voting: false
         - bifrost-keystone-collections-src:
             voting: false
-        - kolla-ansible-centos8-source-bifrost:
+        - kolla-ansible-centos8s-source-bifrost:
             voting: false
             # NOTE(yoctozepto): to override from job definition
             files: .*
             irrelevant-files:
               - ^.*\.rst$
               - ^bifrost/tests/.*$
               - ^api-ref/.*$
```

