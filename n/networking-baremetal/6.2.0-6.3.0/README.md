# Comparing `tmp/networking-baremetal-6.2.0.tar.gz` & `tmp/networking-baremetal-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networking-baremetal-6.2.0.tar", last modified: Thu Aug 31 10:15:41 2023, max compression
+gzip compressed data, was "networking-baremetal-6.3.0.tar", last modified: Thu Mar 14 12:04:29 2024, max compression
```

## Comparing `networking-baremetal-6.2.0.tar` & `networking-baremetal-6.3.0.tar`

### file list

```diff
@@ -1,168 +1,171 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.216807 networking-baremetal-6.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6159 2023-08-31 10:15:40.000000 networking-baremetal-6.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2023-08-31 10:15:41.216807 networking-baremetal-6.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.188805 networking-baremetal-6.2.0/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.188805 networking-baremetal-6.2.0/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1751 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/devstack/lib/networking-baremetal
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.188805 networking-baremetal-6.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.188805 networking-baremetal-6.2.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4043 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.188805 networking-baremetal-6.2.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.188805 networking-baremetal-6.2.0/doc/source/configuration/ironic-neutron-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/configuration/ironic-neutron-agent/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/configuration/ironic-neutron-agent/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/configuration/ironic-neutron-agent/sample-config.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.192805 networking-baremetal-6.2.0/doc/source/configuration/ml2/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.192805 networking-baremetal-6.2.0/doc/source/configuration/ml2/device_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/configuration/ml2/device_drivers/common_config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/configuration/ml2/device_drivers/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/configuration/ml2/device_drivers/netconf-openconfig.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1082 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/configuration/ml2/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.192805 networking-baremetal-6.2.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2294 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4784 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/contributor/quickstart-multitenant.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/contributor/quickstart-netconf-openconfig.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3544 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/contributor/quickstart.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.192805 networking-baremetal-6.2.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4523 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.192805 networking-baremetal-6.2.0/networking_baremetal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.196806 networking-baremetal-6.2.0/networking_baremetal/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11277 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/agent/ironic_neutron_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3292 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4977 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.196806 networking-baremetal-6.2.0/networking_baremetal/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3581 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/drivers/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.196806 networking-baremetal-6.2.0/networking_baremetal/drivers/netconf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41328 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/drivers/netconf/openconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/ironic_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.196806 networking-baremetal-6.2.0/networking_baremetal/openconfig/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4618 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/aggregate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4533 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/ethernet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11381 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/interfaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/openconfig/lacp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/lacp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8855 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/lacp/lacp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/lacp/types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/openconfig/network_instance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/network_instance/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3675 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/network_instance/network_instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/openconfig/vlan/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/vlan/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/vlan/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13697 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/openconfig/vlan/vlan.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/plugins/ml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/plugins/ml2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27486 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/plugins/ml2/baremetal_mech.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/tests/unit/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.200806 networking-baremetal-6.2.0/networking_baremetal/tests/unit/drivers/netconf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/drivers/netconf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57311 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/drivers/netconf/test_openconfig.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.204806 networking-baremetal-6.2.0/networking_baremetal/tests/unit/ironic_agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/ironic_agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3597 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/ironic_agent/test_hashring_member_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15078 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/ironic_agent/test_ironic_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.204806 networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9357 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/test_interfaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4963 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/test_lacp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/test_network_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7172 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/test_vlan.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.204806 networking-baremetal-6.2.0/networking_baremetal/tests/unit/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.204806 networking-baremetal-6.2.0/networking_baremetal/tests/unit/plugins/ml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/plugins/ml2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26798 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/plugins/ml2/test_baremetal_mech.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5215 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/networking_baremetal/tests/unit/plugins/ml2/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.196806 networking-baremetal-6.2.0/networking_baremetal.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/networking_baremetal.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5653 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/networking_baremetal.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/networking_baremetal.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/networking_baremetal.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/networking_baremetal.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/networking_baremetal.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/networking_baremetal.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2023-08-31 10:15:41.000000 networking-baremetal-6.2.0/networking_baremetal.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.184805 networking-baremetal-6.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.208806 networking-baremetal-6.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/add-initial-note-8f08fd95b0149b2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/agent-notification-auto-delete-queues-a3782fbeea2b57b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/device-manager-driver-interface-741703fbfc063780.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/distributed-agent-hashring-6b623a7a9caf0425.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/drop-py-2-7-2249129e616bb1e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/fix-exception-handling-openstacksdk-d3eff6f9fe9ea42f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/fix-member-manager-notification-queue-not-consumed-449738d4fd799634.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/ironic-neutron-agent-291f8aad7d53f06c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/mech-agent-driver-ffc361e528668f8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/netconf-openconfig-device-driver-8fc15c9c2dc4bf17.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/netconf-openconfig-device-driver-lacp-support-ed9e1bc0eb784c9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/netconf-openconfig-device-driver-pre-configured-link-aggregates-2dcba8f96500d159.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/openconfig-library-5ecd1f158666c6c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/replace-ironicclient-with-openstacksdk-75d1edd705571f94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/sighup-service-reloads-configs-11cd374cc33aac83.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/notes/vlan-type-support-mech-driver-31f907c76dc44923.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.212806 networking-baremetal-6.2.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.212806 networking-baremetal-6.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.212806 networking-baremetal-6.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9105 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2023-08-31 10:15:41.216807 networking-baremetal-6.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.212806 networking-baremetal-6.2.0/tools/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.212806 networking-baremetal-6.2.0/tools/config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/tools/config/networking-baremetal-common-device-driver-opts.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/tools/config/networking-baremetal-ironic-neutron-agent.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/tools/config/networking-baremetal-netconf-openconfig-driver-opts.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      477 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/tools/flake8wrap.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1296 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/tools/run_bashate.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3477 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-31 10:15:41.216807 networking-baremetal-6.2.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2438 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/zuul.d/networking-baremetal-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-08-31 10:15:11.000000 networking-baremetal-6.2.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6532 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.941134 networking-baremetal-6.3.0/devstack/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.941134 networking-baremetal-6.3.0/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1751 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/devstack/lib/networking-baremetal
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.941134 networking-baremetal-6.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.941134 networking-baremetal-6.3.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4043 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.941134 networking-baremetal-6.3.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/doc/source/configuration/ironic-neutron-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/configuration/ironic-neutron-agent/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/configuration/ironic-neutron-agent/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/configuration/ironic-neutron-agent/sample-config.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/doc/source/configuration/ml2/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/doc/source/configuration/ml2/device_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/configuration/ml2/device_drivers/common_config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/configuration/ml2/device_drivers/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/configuration/ml2/device_drivers/netconf-openconfig.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1082 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/configuration/ml2/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2294 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4784 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/contributor/quickstart-multitenant.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/contributor/quickstart-netconf-openconfig.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3544 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/contributor/quickstart.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4523 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/networking_baremetal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/networking_baremetal/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11393 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/agent/ironic_neutron_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3292 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4977 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/networking_baremetal/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3581 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/drivers/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/networking_baremetal/drivers/netconf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41328 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/drivers/netconf/openconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/ironic_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/networking_baremetal/openconfig/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4618 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/aggregate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4533 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/ethernet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11381 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/interfaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/openconfig/lacp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/lacp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8855 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/lacp/lacp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/lacp/types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/openconfig/network_instance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/network_instance/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3675 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/network_instance/network_instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/openconfig/vlan/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/vlan/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/vlan/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13697 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/openconfig/vlan/vlan.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/plugins/ml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/plugins/ml2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27747 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/plugins/ml2/baremetal_mech.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/tests/unit/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/tests/unit/drivers/netconf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/drivers/netconf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57311 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/drivers/netconf/test_openconfig.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/tests/unit/ironic_agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/ironic_agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3597 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/ironic_agent/test_hashring_member_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15078 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/ironic_agent/test_ironic_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9357 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/test_interfaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4963 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/test_lacp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/test_network_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7172 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/test_vlan.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.949133 networking-baremetal-6.3.0/networking_baremetal/tests/unit/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.953133 networking-baremetal-6.3.0/networking_baremetal/tests/unit/plugins/ml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/plugins/ml2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26378 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/plugins/ml2/test_baremetal_mech.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5215 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/networking_baremetal/tests/unit/plugins/ml2/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.945134 networking-baremetal-6.3.0/networking_baremetal.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/networking_baremetal.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5821 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/networking_baremetal.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/networking_baremetal.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/networking_baremetal.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/networking_baremetal.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/networking_baremetal.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/networking_baremetal.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-03-14 12:04:29.000000 networking-baremetal-6.3.0/networking_baremetal.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.941134 networking-baremetal-6.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.953133 networking-baremetal-6.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/add-initial-note-8f08fd95b0149b2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/agent-notification-auto-delete-queues-a3782fbeea2b57b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/device-manager-driver-interface-741703fbfc063780.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/distributed-agent-hashring-6b623a7a9caf0425.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/drop-py-2-7-2249129e616bb1e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/fix-conflict-with-ngs-41a862c292718c3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/fix-exception-handling-openstacksdk-d3eff6f9fe9ea42f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/fix-member-manager-notification-queue-not-consumed-449738d4fd799634.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/fix_autodelete_for_quorum_queues-e001f2d8d8ae780b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/ironic-neutron-agent-291f8aad7d53f06c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/mech-agent-driver-ffc361e528668f8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/netconf-openconfig-device-driver-8fc15c9c2dc4bf17.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/netconf-openconfig-device-driver-lacp-support-ed9e1bc0eb784c9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/netconf-openconfig-device-driver-pre-configured-link-aggregates-2dcba8f96500d159.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/openconfig-library-5ecd1f158666c6c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/replace-ironicclient-with-openstacksdk-75d1edd705571f94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/sighup-service-reloads-configs-11cd374cc33aac83.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/notes/vlan-type-support-mech-driver-31f907c76dc44923.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9105 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/tools/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/tools/config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/tools/config/networking-baremetal-common-device-driver-opts.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/tools/config/networking-baremetal-ironic-neutron-agent.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/tools/config/networking-baremetal-netconf-openconfig-driver-opts.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      477 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/tools/flake8wrap.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1296 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/tools/run_bashate.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3740 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:04:29.957134 networking-baremetal-6.3.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2572 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/zuul.d/networking-baremetal-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-03-14 12:04:02.000000 networking-baremetal-6.3.0/zuul.d/project.yaml
```

### Comparing `networking-baremetal-6.2.0/AUTHORS` & `networking-baremetal-6.3.0/AUTHORS`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 Le Hou <houl7@chinaunicom.cn>
 Mark Goddard <mark@stackhpc.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Pavlo Shchelokovskyy <shchelokovskyy@gmail.com>
 Riccardo Pittau <elfosardo@gmail.com>
 Sam Betts <sam@code-smash.net>
 Sean McGinnis <sean.mcginnis@gmail.com>
+Sharpz7 <adam.mcarthur62@gmail.com>
+Sven Kieske <kieske@osism.tech>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Tuan Do Anh <tuanda@vn.fujitsu.com>
 Vasyl Saienko <vsaienko@mirantis.com>
 Vieri <15050873171@163.com>
 Vladyslav Drok <vdrok@mirantis.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 YuehuiLei <leiyuehui@inspur.com>
 huang.zhiping <huang.zhiping@99cloud.net>
```

### Comparing `networking-baremetal-6.2.0/CONTRIBUTING.rst` & `networking-baremetal-6.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/ChangeLog` & `networking-baremetal-6.3.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 CHANGES
 =======
 
+6.3.0
+-----
+
+* don't force amqp\_auto\_delete for quorum queues
+* [codespell] Adding CI target for Tox Codespell
+* [codespell] Adding Tox Target for Codespell
+* [codespell] Fixing Spelling Mistakes
+* Bump hacking to 6.1.0
+* reno: Update master for unmaintained/yoga
+* Remove deprecated pbr options
+* Do not try to bind port when we can't
+* Update master for stable/2023.2
+
 6.2.0
 -----
 
 * Bugs are now in launchpad, doc fixes
 * Update to hacking v6
 * Update master for stable/2023.1
 * [CI] Explicitly disable port security
```

### Comparing `networking-baremetal-6.2.0/LICENSE` & `networking-baremetal-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/PKG-INFO` & `networking-baremetal-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: networking-baremetal
-Version: 6.2.0
+Version: 6.3.0
 Summary: Neutron plugin that provides deep Ironic/Neutron integration.
 Home-page: https://docs.openstack.org/networking-baremetal/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: networking-baremetal plugin
         ---------------------------
```

### Comparing `networking-baremetal-6.2.0/README.rst` & `networking-baremetal-6.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/devstack/lib/networking-baremetal` & `networking-baremetal-6.3.0/devstack/lib/networking-baremetal`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/devstack/plugin.sh` & `networking-baremetal-6.3.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/conf.py` & `networking-baremetal-6.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/configuration/ironic-neutron-agent/sample-config.rst` & `networking-baremetal-6.3.0/doc/source/configuration/ironic-neutron-agent/sample-config.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/configuration/ml2/device_drivers/common_config.rst` & `networking-baremetal-6.3.0/doc/source/configuration/ml2/device_drivers/common_config.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/configuration/ml2/device_drivers/index.rst` & `networking-baremetal-6.3.0/doc/source/configuration/ml2/device_drivers/index.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/configuration/ml2/device_drivers/netconf-openconfig.rst` & `networking-baremetal-6.3.0/doc/source/configuration/ml2/device_drivers/netconf-openconfig.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/configuration/ml2/index.rst` & `networking-baremetal-6.3.0/doc/source/configuration/ml2/index.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/contributor/index.rst` & `networking-baremetal-6.3.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/contributor/quickstart-multitenant.rst` & `networking-baremetal-6.3.0/doc/source/contributor/quickstart-multitenant.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/contributor/quickstart.rst` & `networking-baremetal-6.3.0/doc/source/contributor/quickstart.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/index.rst` & `networking-baremetal-6.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/doc/source/install/index.rst` & `networking-baremetal-6.3.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/__init__.py` & `networking-baremetal-6.3.0/networking_baremetal/__init__.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/_i18n.py` & `networking-baremetal-6.3.0/networking_baremetal/_i18n.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/agent/ironic_neutron_agent.py` & `networking-baremetal-6.3.0/networking_baremetal/agent/ironic_neutron_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 
 def list_opts():
     return [('agent', agent_config.AGENT_STATE_OPTS)]
 
 
 def _get_notification_transport_url():
     url = urlparse.urlparse(CONF.transport_url)
-    if CONF.oslo_messaging_rabbit.amqp_auto_delete is False:
+    if (CONF.oslo_messaging_rabbit.amqp_auto_delete is False
+            and not getattr(CONF.oslo_messaging_rabbit, 'rabbit_quorum_queue',
+                            None)):
         q = urlparse.parse_qs(url.query)
         q.update({'amqp_auto_delete': ['true']})
         query = urlparse.urlencode({k: v[0] for k, v in q.items()})
         url = url._replace(query=query)
     return urlparse.urlunparse(url)
 
 
@@ -186,15 +188,15 @@
             self.notifier.info({
                 'ironic-neutron-agent': 'heartbeat'},
                 'ironic-neutron-agent-member-manager',
                 {'id': self.agent_id,
                  'host': self.agent_host,
                  'timestamp': timeutils.utcnow_ts()})
         except Exception:
-            LOG.exception('Failed to send hash ring membership hearbeat!')
+            LOG.exception('Failed to send hash ring membership heartbeat!')
 
     def get_template_node_state(self, node_uuid):
         return {
             'binary': constants.BAREMETAL_BINARY,
             'host': node_uuid,
             'topic': n_const.L2_AGENT_TOPIC,
             'configurations': {
```

### Comparing `networking-baremetal-6.2.0/networking_baremetal/common.py` & `networking-baremetal-6.3.0/networking_baremetal/common.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/config.py` & `networking-baremetal-6.3.0/networking_baremetal/config.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/constants.py` & `networking-baremetal-6.3.0/networking_baremetal/constants.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/drivers/base.py` & `networking-baremetal-6.3.0/networking_baremetal/drivers/base.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/drivers/netconf/openconfig.py` & `networking-baremetal-6.3.0/networking_baremetal/drivers/netconf/openconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
         aggregate_ids = {f'{prefix}{x}'
                          for x in range(int(aggregate_id_range[0]),
                                         int(aggregate_id_range[1]) + 1)}
         return aggregate_ids
 
     @staticmethod
     def allocate_deferred(aggregate_id, config):
-        """Set aggregation id where it was deffered
+        """Set aggregation id where it was deferred
 
         :param aggregate_id: Aggregation ID for the link aggregate,
             for example 'po123'
         :param config: Configuration objects to update
         """
         for conf in config:
             if isinstance(conf, interfaces.Interfaces):
```

### Comparing `networking-baremetal-6.2.0/networking_baremetal/exceptions.py` & `networking-baremetal-6.3.0/networking_baremetal/exceptions.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/ironic_client.py` & `networking-baremetal-6.3.0/networking_baremetal/ironic_client.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/aggregate.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/aggregate.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/ethernet.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/ethernet.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/interfaces.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/interfaces.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/interfaces/types.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/interfaces/types.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/lacp/lacp.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/lacp/lacp.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/lacp/types.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/lacp/types.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/network_instance/network_instance.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/network_instance/network_instance.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/vlan/types.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/vlan/types.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/openconfig/vlan/vlan.py` & `networking-baremetal-6.3.0/networking_baremetal/openconfig/vlan/vlan.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/plugins/ml2/baremetal_mech.py` & `networking-baremetal-6.3.0/networking_baremetal/plugins/ml2/baremetal_mech.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,14 +483,20 @@
                                 {'link': link, 'port': port[api.ID],
                                  'device': device})
                     LOG.debug(e.message)
                     return False
 
             by_device[device]['links'].append(link)
 
+        if not by_device:
+            # NOTE(vsaienko): we can call set_binding ONLY when we complete
+            # binding for the port in the segment. We do not handle the port
+            # and want to let other drivers to bind it.
+            return False
+
         # Check driver(s) support the bond_mode - if not fail port binding
         if (bond_mode and by_device
                 and not self._is_bond_mode_supported(bond_mode, by_device)):
             LOG.warning('Cannot bind port %(port)s, unsupported '
                         'bond_mode %(bond_mode)s',
                         {'port': port[api.ID], 'bond_mode': bond_mode})
             return False
```

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/base.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/base.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/drivers/netconf/test_openconfig.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/drivers/netconf/test_openconfig.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/ironic_agent/test_hashring_member_manager.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/ironic_agent/test_hashring_member_manager.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/ironic_agent/test_ironic_agent.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/ironic_agent/test_ironic_agent.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/test_interfaces.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/test_lacp.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/test_lacp.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/test_network_instance.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/test_network_instance.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/openconfig/test_vlan.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/openconfig/test_vlan.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/plugins/ml2/test_baremetal_mech.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/plugins/ml2/test_baremetal_mech.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,23 +68,14 @@
                                     vnic_type=self.VNIC_TYPE)
 
     def test_initialize(self):
         self.assertEqual([portbindings.VNIC_BAREMETAL],
                          self.driver.supported_vnic_types)
         self.assertEqual(portbindings.VIF_TYPE_OTHER, self.driver.vif_type)
 
-    @mock.patch.object(provisioning_blocks, 'add_provisioning_component',
-                       autospec=True)
-    def test_bind_port(self, mpb_pc):
-        port_context = self._make_port_ctx(self.AGENTS)
-        port_context._plugin_context = 'plugin_context'
-        self.assertIsNone(port_context._bound_vif_type)
-        self.driver.bind_port(port_context)
-        self.assertEqual(port_context._bound_vif_type, self.driver.vif_type)
-
     def test_get_allowed_network_types(self):
         agent_mock = mock.Mock()
         allowed_network_types = self.driver.get_allowed_network_types(
             agent_mock)
         self.assertEqual(allowed_network_types,
                          [n_const.TYPE_FLAT, n_const.TYPE_VLAN])
 
@@ -334,15 +325,15 @@
             network_type=n_const.TYPE_VLAN)
         m_nc.original = ml2_utils.get_test_network(
             network_type=n_const.TYPE_VLAN)
         self.driver.update_network_postcommit(m_nc)
         self.mock_manager.assert_not_called()
         self.mock_driver.assert_not_called()
 
-        # Whith physical network
+        # With physical network
         self.mock_manager.reset_mock()
         self.mock_driver.reset_mock()
         m_nc.current = ml2_utils.get_test_network(
             network_type=n_const.TYPE_VLAN,
             segmentation_id=10,
             physical_network='fake_physical_network')
         self.driver.update_network_postcommit(m_nc)
@@ -443,15 +434,16 @@
                     'switch_info': 'not-such-device'})
         context = self._make_port_ctx(self.AGENTS, binding_profile)
         context._plugin_context = 'plugin_context'
         self.assertIsNone(context._bound_vif_type)
         self.driver.bind_port(context)
         self.mock_manager.assert_not_called()
         self.mock_driver.create_port.assert_not_called()
-        self.assertEqual(context._bound_vif_type, self.driver.vif_type)
+        self.assertIsNone(context._bound_vif_type)
+        mock_p_blocks.assert_not_called()
 
     @mock.patch.object(provisioning_blocks, 'add_provisioning_component',
                        autospec=True)
     def test_driver_load_error_does_not_bind_port(self, mock_p_blocks):
         binding_profile = {}
         lli = binding_profile['local_link_information'] = []
         lli.append({'port_id': 'test1/1', 'switch_id': 'aa:bb:cc:dd:ee:ff',
```

### Comparing `networking-baremetal-6.2.0/networking_baremetal/tests/unit/plugins/ml2/utils.py` & `networking-baremetal-6.3.0/networking_baremetal/tests/unit/plugins/ml2/utils.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/networking_baremetal.egg-info/PKG-INFO` & `networking-baremetal-6.3.0/networking_baremetal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: networking-baremetal
-Version: 6.2.0
+Version: 6.3.0
 Summary: Neutron plugin that provides deep Ironic/Neutron integration.
 Home-page: https://docs.openstack.org/networking-baremetal/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: networking-baremetal plugin
         ---------------------------
```

### Comparing `networking-baremetal-6.2.0/networking_baremetal.egg-info/SOURCES.txt` & `networking-baremetal-6.3.0/networking_baremetal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -87,26 +87,29 @@
 networking_baremetal/tests/unit/plugins/ml2/utils.py
 releasenotes/notes/.placeholder
 releasenotes/notes/add-initial-note-8f08fd95b0149b2c.yaml
 releasenotes/notes/agent-notification-auto-delete-queues-a3782fbeea2b57b1.yaml
 releasenotes/notes/device-manager-driver-interface-741703fbfc063780.yaml
 releasenotes/notes/distributed-agent-hashring-6b623a7a9caf0425.yaml
 releasenotes/notes/drop-py-2-7-2249129e616bb1e5.yaml
+releasenotes/notes/fix-conflict-with-ngs-41a862c292718c3b.yaml
 releasenotes/notes/fix-exception-handling-openstacksdk-d3eff6f9fe9ea42f.yaml
 releasenotes/notes/fix-member-manager-notification-queue-not-consumed-449738d4fd799634.yaml
+releasenotes/notes/fix_autodelete_for_quorum_queues-e001f2d8d8ae780b.yaml
 releasenotes/notes/ironic-neutron-agent-291f8aad7d53f06c.yaml
 releasenotes/notes/mech-agent-driver-ffc361e528668f8e.yaml
 releasenotes/notes/netconf-openconfig-device-driver-8fc15c9c2dc4bf17.yaml
 releasenotes/notes/netconf-openconfig-device-driver-lacp-support-ed9e1bc0eb784c9b.yaml
 releasenotes/notes/netconf-openconfig-device-driver-pre-configured-link-aggregates-2dcba8f96500d159.yaml
 releasenotes/notes/openconfig-library-5ecd1f158666c6c5.yaml
 releasenotes/notes/replace-ironicclient-with-openstacksdk-75d1edd705571f94.yaml
 releasenotes/notes/sighup-service-reloads-configs-11cd374cc33aac83.yaml
 releasenotes/notes/vlan-type-support-mech-driver-31f907c76dc44923.yaml
 releasenotes/source/2023.1.rst
+releasenotes/source/2023.2.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
```

### Comparing `networking-baremetal-6.2.0/networking_baremetal.egg-info/entry_points.txt` & `networking-baremetal-6.3.0/networking_baremetal.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/releasenotes/notes/agent-notification-auto-delete-queues-a3782fbeea2b57b1.yaml` & `networking-baremetal-6.3.0/releasenotes/notes/agent-notification-auto-delete-queues-a3782fbeea2b57b1.yaml`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/releasenotes/notes/fix-member-manager-notification-queue-not-consumed-449738d4fd799634.yaml` & `networking-baremetal-6.3.0/releasenotes/notes/fix-member-manager-notification-queue-not-consumed-449738d4fd799634.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
 fixes:
   - |
     Fixes an issue causing heavy RAM (and/or-storage) usage on the message
     broker back-end. The ``ironic-neutron-agent`` uses oslo.messaging
     notifications, with all notification listeners using pools. Since all
-    listeneres are using pools the default notification queue in messaging is
+    listeners are using pools the default notification queue in messaging is
     not consumed (only the pool queues are consumed). The default notification
-    queue was continously growing, consuming more and more resources on the
+    queue was continuously growing, consuming more and more resources on the
     messaging back-end. See `oslo.messaging bug: 1814544
     <https://bugs.launchpad.net/oslo.messaging/+bug/1814544>`_ and `bug:
     2004938 <https://storyboard.openstack.org/#!/story/2004938>`_ for more
     details.
```

### Comparing `networking-baremetal-6.2.0/releasenotes/notes/ironic-neutron-agent-291f8aad7d53f06c.yaml` & `networking-baremetal-6.3.0/releasenotes/notes/ironic-neutron-agent-291f8aad7d53f06c.yaml`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/releasenotes/notes/openconfig-library-5ecd1f158666c6c5.yaml` & `networking-baremetal-6.3.0/releasenotes/notes/openconfig-library-5ecd1f158666c6c5.yaml`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/releasenotes/notes/replace-ironicclient-with-openstacksdk-75d1edd705571f94.yaml` & `networking-baremetal-6.3.0/releasenotes/notes/replace-ironicclient-with-openstacksdk-75d1edd705571f94.yaml`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/releasenotes/notes/sighup-service-reloads-configs-11cd374cc33aac83.yaml` & `networking-baremetal-6.3.0/releasenotes/notes/sighup-service-reloads-configs-11cd374cc33aac83.yaml`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/releasenotes/notes/vlan-type-support-mech-driver-31f907c76dc44923.yaml` & `networking-baremetal-6.3.0/releasenotes/notes/vlan-type-support-mech-driver-31f907c76dc44923.yaml`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/releasenotes/source/conf.py` & `networking-baremetal-6.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/requirements.txt` & `networking-baremetal-6.3.0/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 # Requirements lower bounds listed here are our best effort to keep them up to
 # date but we do not test them so no guarantee of having them all correct. If
 # you find any incorrect lower bounds, let us know or propose a fix.
-
-# The order of packages is significant, because pip processes them in the order
-# of appearance. Changing the order has an impact on the overall integration
-# process, which may cause wedges in the gate later.
-
 ncclient>=0.6.9 # Apache-2.0
 neutron-lib>=1.28.0 # Apache-2.0
 oslo.config>=5.2.0 # Apache-2.0
 oslo.i18n>=3.15.3 # Apache-2.0
 oslo.log>=3.36.0 # Apache-2.0
 oslo.utils>=3.40.2 # Apache-2.0
 oslo.messaging>=5.29.0 # Apache-2.0
```

### Comparing `networking-baremetal-6.2.0/setup.cfg` & `networking-baremetal-6.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 console_scripts = 
 	ironic-neutron-agent = networking_baremetal.agent.ironic_neutron_agent:main
 neutron.ml2.mechanism_drivers = 
 	baremetal = networking_baremetal.plugins.ml2.baremetal_mech:BaremetalMechanismDriver
 networking_baremetal.drivers = 
 	netconf-openconfig = networking_baremetal.drivers.netconf.openconfig:NetconfOpenConfigDriver
 
-[pbr]
-autodoc_index_modules = True
-api_doc_dir = contributor/api
+[codespell]
+quiet-level = 4
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `networking-baremetal-6.2.0/setup.py` & `networking-baremetal-6.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/tools/run_bashate.sh` & `networking-baremetal-6.3.0/tools/run_bashate.sh`

 * *Files identical despite different names*

### Comparing `networking-baremetal-6.2.0/tox.ini` & `networking-baremetal-6.3.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     no_proxy
     NO_PROXY
 
 [testenv:pep8]
 deps =
     bashate>=0.5.1 # Apache-2.0
     flake8-import-order>=0.17.1 # LGPLv3
-    hacking~=6.0.0 # Apache-2.0
+    hacking~=6.1.0 # Apache-2.0
     pycodestyle>=2.0.0,<3.0.0 # MIT
 allowlist_externals = bash
                       {toxinidir}/tools/run_bashate.sh
 commands =
   bash tools/flake8wrap.sh {posargs}
   # Run bashate during pep8 runs to ensure violations are caught by
   # the check and gate queues.
@@ -102,7 +102,16 @@
 builtins = _
 exclude=.venv,.git,.tox,dist,doc,*lib/python*,*egg,build
 import-order-style = pep8
 application-import-names = networking_baremetal
 filename = *.py
 per-file-ignores =
     networking_baremetal/agent/ironic_neutron_agent.py:E402
+
+[testenv:codespell]
+description =
+  Run codespell to check spelling
+deps = codespell
+# note(JayF): {posargs} lets us run `tox -ecodespell -- -w` to get codespell
+#             to correct spelling issues in our code it's aware of.
+commands =
+  codespell {posargs}
```

### Comparing `networking-baremetal-6.2.0/zuul.d/networking-baremetal-jobs.yaml` & `networking-baremetal-6.3.0/zuul.d/networking-baremetal-jobs.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -65,7 +65,13 @@
         q-agt: True
         q-dhcp: True
         q-l3: True
         q-meta: True
         q-metering: True
         q-svc: True
 
+- job:
+    name: networking-baremetal-tox-codespell
+    parent: openstack-tox
+    timeout: 7200
+    vars:
+      tox_envlist: codespell
```

