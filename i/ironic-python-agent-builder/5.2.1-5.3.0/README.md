# Comparing `tmp/ironic-python-agent-builder-5.2.1.tar.gz` & `tmp/ironic-python-agent-builder-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironic-python-agent-builder-5.2.1.tar", last modified: Fri Mar 29 12:38:18 2024, max compression
+gzip compressed data, was "ironic-python-agent-builder-5.3.0.tar", last modified: Mon Mar  4 10:58:59 2024, max compression
```

## Comparing `ironic-python-agent-builder-5.2.1.tar` & `ironic-python-agent-builder-5.3.0.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.473634 ironic-python-agent-builder-5.2.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10997 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2024-03-29 12:38:18.473634 ironic-python-agent-builder-5.2.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.441634 ironic-python-agent-builder-5.2.1/dib/burn-in/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/burn-in/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/burn-in/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/burn-in/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.441634 ironic-python-agent-builder-5.2.1/dib/extra-hardware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/extra-hardware/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/extra-hardware/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.441634 ironic-python-agent-builder-5.2.1/dib/extra-hardware/environment.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      418 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/extra-hardware/environment.d/10-enable-rdo-deps.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.429634 ironic-python-agent-builder-5.2.1/dib/extra-hardware/install.d/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.441634 ironic-python-agent-builder-5.2.1/dib/extra-hardware/install.d/extra-hardware-package-install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/extra-hardware/install.d/extra-hardware-package-install/package-installs-extra-hardware
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.441634 ironic-python-agent-builder-5.2.1/dib/extra-hardware/install.d/extra-hardware-source-install/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      751 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/extra-hardware/install.d/extra-hardware-source-install/80-extra-hardware-install
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/extra-hardware/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/extra-hardware/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.441634 ironic-python-agent-builder-5.2.1/dib/extra-hardware/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      246 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/extra-hardware/pre-install.d/10-enable-rdo-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.445634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1900 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.445634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/environment.d/01-debian-ipa.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/environment.d/10-defaults.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/environment.d/20-ipa-distro-family.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.445634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      191 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/extra-data.d/15-ssl-ca-copy
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.445634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-package-install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-package-install/package-installs-ironic-python-agent-ramdisk
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.445634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2623 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/60-ironic-python-agent-ramdisk-install
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/ironic-python-agent.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      677 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/ironic-python-agent.init
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/ironic-python-agent.service
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2314 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.445634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1615 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/post-install.d/80-ironic-python-agent-ramdisk
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1364 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/post-install.d/99-remove-extra-packages
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/source-repository-ironic-lib
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/source-repository-ironic-python-agent
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/source-repository-requirements
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.445634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/etc/ironic-python-agent.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/etc/ironic-python-agent.d/README
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/etc/systemd/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/etc/systemd/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/etc/systemd/system/ironic-agent-create-rescue-user.path
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/etc/systemd/system/ironic-agent-create-rescue-user.service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/usr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/usr/local/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/usr/local/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      255 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/static/usr/local/bin/ironic-python-agent-create-rescue-user.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/svc-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-tls/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-tls/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-tls/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-tls/pre-finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1260 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-tls/pre-finalise.d/10-configure-ipa-tls
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1542 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/cleanup.d/98-prepare-resolve-conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3679 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/cleanup.d/99-ramdisk-create
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/environment.d/10-checksum.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/multipath-io/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/multipath-io/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/multipath-io/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/multipath-io/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/multipath-io/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/dib/multipath-io/static/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/dib/multipath-io/static/etc/modules-load.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/dib/multipath-io/static/etc/modules-load.d/iscsi.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.449634 ironic-python-agent-builder-5.2.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.453634 ironic-python-agent-builder-5.2.1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10187 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/doc/source/admin/dib.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/doc/source/admin/tinyipa.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2680 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.453634 ironic-python-agent-builder-5.2.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.453634 ironic-python-agent-builder-5.2.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.453634 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.453634 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7105 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2024-03-29 12:38:18.000000 ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.433634 ironic-python-agent-builder-5.2.1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.457634 ironic-python-agent-builder-5.2.1/playbooks/ironic-python-agent-build-image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/playbooks/ironic-python-agent-build-image/extra-logs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/playbooks/ironic-python-agent-build-image/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/playbooks/ironic-python-agent-build-image/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/playbooks/ironic-python-agent-build-image/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.437634 ironic-python-agent-builder-5.2.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.465634 ironic-python-agent-builder-5.2.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/add-efibootmgr-d2a456de6b999612.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/add-efivar-f83fdf2d797396dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/add-ntpdate-3db2f8565fed761e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/add-nvme-cli-590e42735476a549.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/centos7-python3-185f1d35c37096c7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/centos8-46a95956fd871c90.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/centos8-stream-d9c83190e987e07d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/centos9-0f925822a2ab9e0a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/clean-var-tmp-with-dib-builds-cd31a2cf70a7f935.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/create-ramdisk-random-devices-263f78a2ef40dbe2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/debian-9a4fa6b2d3ef96d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/debian-arm64-fc3cc4949e3100d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/debian-firmware-1927601ebb779bc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/dhcp-predictible-ifnames-b2a1d9e6471b6819.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/drop-python2-534124afa50f62dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/excess-firmware-removal-debian-06c49a8604122b1c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/extra-hardware-73e3c9b5a0143bfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/ironic-lib-6a16f13fc6ec9a50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/ironic-ramdisk-base-3bfb9b90ad416891.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/linux-firmware-9a6f8a9a32c5719d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/lzma-bf4552b98dd5824a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/multipath-0eb6a4f3b2ee22a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/network-manager-auto-dhcp-all-interfaces-rhel-centos-relese-gt-7-0c2054d0067c6e93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/no-fedora-aa65bcc43f9d56fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/no-firmware-e2cb953037a3be8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/no-iscsi-5d132e6468acab0b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/no-sdparm-f77de72b5c0d7859.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/no-suse-e15d8384c423251c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/python2-removal-dee895550b1959af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/remove-PYOPTIMIZE_TINYIPA-ebde63911d140209.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/selinux-permissive-a059f42bb66373a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/tinycore13-caba5a4998bdd628.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/notes/tinyipa-tgt-226f74125238c239.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.465634 ironic-python-agent-builder-5.2.1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.465634 ironic-python-agent-builder-5.2.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.465634 ironic-python-agent-builder-5.2.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9318 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.437634 ironic-python-agent-builder-5.2.1/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.437634 ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.465634 ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.465634 ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/tasks/install.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2109 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.437634 ironic-python-agent-builder-5.2.1/roles/ipa-build-tinyipa-image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.465634 ironic-python-agent-builder-5.2.1/roles/ipa-build-tinyipa-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/roles/ipa-build-tinyipa-image/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.465634 ironic-python-agent-builder-5.2.1/roles/ipa-build-tinyipa-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/roles/ipa-build-tinyipa-image/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2024-03-29 12:38:18.473634 ironic-python-agent-builder-5.2.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.469634 ironic-python-agent-builder-5.2.1/tinyipa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/README.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4487 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/add-ssh-tinyipa.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      974 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build-instance-images.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1086 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build-iso.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9239 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build-tinyipa.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.473634 ironic-python-agent-builder-5.2.1/tinyipa/build_files/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2948 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/bootlocal.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/buildreqs.lst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/buildreqs_python2.lst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/buildreqs_python3.lst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/dhcp.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1332 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/fakeuname
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/finalreqs.lst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/finalreqs_python2.lst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/finalreqs_python3.lst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      193 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/isolinux.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/modprobe.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      110 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/build_files/ntpdate
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2329 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/common.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9241 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/finalise-tinyipa.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2616 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/generate_tox_constraints.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      750 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/install-deps.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/tc-mirror.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1162 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tinyipa/udhcpc.script
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.473634 ironic-python-agent-builder-5.2.1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4120 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tools/iso-image-create
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-29 12:38:18.473634 ironic-python-agent-builder-5.2.1/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4231 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/zuul.d/ironic-python-agent-builder-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1810 2024-03-29 12:37:33.000000 ironic-python-agent-builder-5.2.1/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.585785 ironic-python-agent-builder-5.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11481 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2024-03-04 10:58:59.585785 ironic-python-agent-builder-5.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.557782 ironic-python-agent-builder-5.3.0/dib/burn-in/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/burn-in/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/burn-in/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/burn-in/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.557782 ironic-python-agent-builder-5.3.0/dib/extra-hardware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/extra-hardware/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/extra-hardware/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.557782 ironic-python-agent-builder-5.3.0/dib/extra-hardware/environment.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      418 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/extra-hardware/environment.d/10-enable-rdo-deps.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/extra-hardware/install.d/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.557782 ironic-python-agent-builder-5.3.0/dib/extra-hardware/install.d/extra-hardware-package-install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/extra-hardware/install.d/extra-hardware-package-install/package-installs-extra-hardware
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.557782 ironic-python-agent-builder-5.3.0/dib/extra-hardware/install.d/extra-hardware-source-install/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      751 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/extra-hardware/install.d/extra-hardware-source-install/80-extra-hardware-install
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/extra-hardware/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/extra-hardware/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.557782 ironic-python-agent-builder-5.3.0/dib/extra-hardware/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      246 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/extra-hardware/pre-install.d/10-enable-rdo-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.561782 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1900 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.561782 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/environment.d/01-debian-ipa.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/environment.d/10-defaults.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/environment.d/20-ipa-distro-family.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.561782 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      191 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/extra-data.d/15-ssl-ca-copy
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.561782 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-package-install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-package-install/package-installs-ironic-python-agent-ramdisk
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.561782 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2623 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/60-ironic-python-agent-ramdisk-install
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/ironic-python-agent.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      677 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/ironic-python-agent.init
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/ironic-python-agent.service
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2314 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.561782 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2352 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/post-install.d/80-ironic-python-agent-ramdisk
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1365 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/post-install.d/99-remove-extra-packages
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/source-repository-ironic-lib
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/source-repository-ironic-python-agent
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/source-repository-requirements
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.561782 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/etc/ironic-python-agent.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/etc/ironic-python-agent.d/README
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/etc/systemd/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.561782 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/etc/systemd/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/etc/systemd/system/ironic-agent-create-rescue-user.path
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/etc/systemd/system/ironic-agent-create-rescue-user.service
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/usr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/usr/local/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/usr/local/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      457 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/static/usr/local/bin/ironic-python-agent-create-rescue-user.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/svc-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-tls/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-tls/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-tls/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-tls/pre-finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1260 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-tls/pre-finalise.d/10-configure-ipa-tls
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1542 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/cleanup.d/98-prepare-resolve-conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3680 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/cleanup.d/99-ramdisk-create
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/environment.d/10-checksum.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/dib/multipath-io/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/multipath-io/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/multipath-io/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/multipath-io/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/multipath-io/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/dib/multipath-io/static/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/dib/multipath-io/static/etc/modules-load.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/dib/multipath-io/static/etc/modules-load.d/iscsi.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10222 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/doc/source/admin/dib.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/doc/source/admin/tinyipa.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2680 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.565783 ironic-python-agent-builder-5.3.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.569783 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4342 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.569783 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7104 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2024-03-04 10:58:59.000000 ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.549781 ironic-python-agent-builder-5.3.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.569783 ironic-python-agent-builder-5.3.0/playbooks/ironic-python-agent-build-image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/playbooks/ironic-python-agent-build-image/extra-logs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/playbooks/ironic-python-agent-build-image/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/playbooks/ironic-python-agent-build-image/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/playbooks/ironic-python-agent-build-image/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.553781 ironic-python-agent-builder-5.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.577784 ironic-python-agent-builder-5.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/add-efibootmgr-d2a456de6b999612.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/add-efivar-f83fdf2d797396dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/add-ntpdate-3db2f8565fed761e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/add-nvme-cli-590e42735476a549.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/centos7-python3-185f1d35c37096c7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/centos8-46a95956fd871c90.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/centos8-stream-d9c83190e987e07d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/centos9-0f925822a2ab9e0a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/clean-var-tmp-with-dib-builds-cd31a2cf70a7f935.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/create-ramdisk-random-devices-263f78a2ef40dbe2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/debian-9a4fa6b2d3ef96d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/debian-arm64-fc3cc4949e3100d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/debian-firmware-1927601ebb779bc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/debian-ipa-cb5975e436cba525.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/dhcp-predictible-ifnames-b2a1d9e6471b6819.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/drop-python2-534124afa50f62dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/excess-firmware-removal-debian-06c49a8604122b1c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/extra-hardware-73e3c9b5a0143bfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/ironic-lib-6a16f13fc6ec9a50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/ironic-ramdisk-base-3bfb9b90ad416891.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/linux-firmware-9a6f8a9a32c5719d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/lzma-bf4552b98dd5824a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/multipath-0eb6a4f3b2ee22a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/network-manager-auto-dhcp-all-interfaces-rhel-centos-relese-gt-7-0c2054d0067c6e93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/no-fedora-aa65bcc43f9d56fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/no-firmware-e2cb953037a3be8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/no-iscsi-5d132e6468acab0b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/no-sdparm-f77de72b5c0d7859.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/no-suse-e15d8384c423251c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/python2-removal-dee895550b1959af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/remove-PYOPTIMIZE_TINYIPA-ebde63911d140209.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/selinux-permissive-a059f42bb66373a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/tinycore13-caba5a4998bdd628.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/notes/tinyipa-tgt-226f74125238c239.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.577784 ironic-python-agent-builder-5.3.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.577784 ironic-python-agent-builder-5.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.577784 ironic-python-agent-builder-5.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9318 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.553781 ironic-python-agent-builder-5.3.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.553781 ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.577784 ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.577784 ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/tasks/install.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2109 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.553781 ironic-python-agent-builder-5.3.0/roles/ipa-build-tinyipa-image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.577784 ironic-python-agent-builder-5.3.0/roles/ipa-build-tinyipa-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/roles/ipa-build-tinyipa-image/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.581784 ironic-python-agent-builder-5.3.0/roles/ipa-build-tinyipa-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/roles/ipa-build-tinyipa-image/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2024-03-04 10:58:59.585785 ironic-python-agent-builder-5.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.581784 ironic-python-agent-builder-5.3.0/tinyipa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/README.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4488 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/add-ssh-tinyipa.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      974 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build-instance-images.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1086 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build-iso.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9025 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build-tinyipa.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.585785 ironic-python-agent-builder-5.3.0/tinyipa/build_files/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2949 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/bootlocal.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/buildreqs.lst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/buildreqs_python3.lst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/dhcp.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1332 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/fakeuname
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/finalreqs.lst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/finalreqs_python3.lst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      193 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/isolinux.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/modprobe.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      110 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/build_files/ntpdate
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2297 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/common.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9071 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/finalise-tinyipa.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2616 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/generate_tox_constraints.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      750 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/install-deps.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/tc-mirror.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1162 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tinyipa/udhcpc.script
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.585785 ironic-python-agent-builder-5.3.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4120 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tools/iso-image-create
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1935 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 10:58:59.585785 ironic-python-agent-builder-5.3.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4541 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/zuul.d/ironic-python-agent-builder-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1978 2024-03-04 10:58:31.000000 ironic-python-agent-builder-5.3.0/zuul.d/project.yaml
```

### Comparing `ironic-python-agent-builder-5.2.1/AUTHORS` & `ironic-python-agent-builder-5.3.0/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Andreas Jaeger <aj@suse.com>
 Bernd Mueller <mueller@b1-systems.de>
 Chandan Kumar (raukadah) <chkumar@redhat.com>
+Damien Rannou <damien.rannou@corp.ovh.com>
 Dmitry Tantsur <divius.inside@gmail.com>
 Dmitry Tantsur <dtantsur@protonmail.com>
 Doug Hellmann <doug@doughellmann.com>
 Fedor Tarasenko <feodor.tarasenko@gmail.com>
 Harald Jensås <hjensas@redhat.com>
 Ian Wienand <iwienand@redhat.com>
 Illia Polliul <ipolliul@juniper.net>
@@ -24,14 +25,15 @@
 Nisha Brahmankar <nisha.ee.iitb@gmail.com>
 Oluwatosin Farai <tosinfarai@gmail.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Pierre Riteau <pierre@stackhpc.com>
 Riccardo Pittau <elfosardo@gmail.com>
 Sagi Shnaidman <sshnaidm@redhat.com>
 Sandeep Yadav <sandyada@redhat.com>
+Sharpz7 <adam.mcarthur62@gmail.com>
 Steve Baker <sbaker@redhat.com>
 Takashi Kajinami <kajinamit@oss.nttdata.com>
 Vasyl Saienko <vsaienko@mirantis.com>
 Xinliang Liu <xinliang.liu@linaro.org>
 XinxinShen <shenxinxin@inspur.com>
 Zygimantas Matonis <zygimantas.matonis@cern.ch>
 huang.zhiping <huang.zhiping@99cloud.net>
```

### Comparing `ironic-python-agent-builder-5.2.1/CONTRIBUTING.rst` & `ironic-python-agent-builder-5.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/ChangeLog` & `ironic-python-agent-builder-5.3.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 CHANGES
 =======
 
-5.2.1
+5.3.0
 -----
 
+* Update ipmitool version to 1.8.19
+* Update link to ipmitool repository
+* Update tinyipa to tinycore 15.x
+* reno: Update master for unmaintained/yoga
+* Bump hacking to 6.1.0
+* [codespell] Adding CI target for Tox Codespell
+* [codespell] Adding Tox Target for Codespell
+* [codespell] Fixing Spelling Mistakes
 * Drop TripleO job
+* Switch IPA building to Debian Bookworm
 * Fix building images for Bullseye and Bookworm
+* Always generate checksum files on image builds
+* Add link to LP bug tracker
+* Remove USE\_PYTHON3 option
+* Use systemd-networkd for debian
+* 'sudo' group different between RH and Debian
 * CI: Change image-build to use Ubuntu Jammy
-* Update TOX\_CONSTRAINTS\_FILE for stable/2023.2
-* Update .gitreview for stable/2023.2
+* Update master for stable/2023.2
 
 5.2.0
 -----
 
 * Exclude .pyc encoding files
 * Build tinyipa with tinycore 14.x
 * Remove outdated install pyyaml with pip2
```

### Comparing `ironic-python-agent-builder-5.2.1/LICENSE` & `ironic-python-agent-builder-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/PKG-INFO` & `ironic-python-agent-builder-5.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ironic-python-agent-builder
-Version: 5.2.1
+Version: 5.3.0
 Summary: Tools and scripts to build Ironic Python Agent
 Home-page: https://docs.openstack.org/ironic-python-agent-builder/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===========================
         Ironic Python Agent Builder
@@ -12,15 +12,15 @@
         
         Tools and scripts to build a deployment, cleaning or inspection ramdisk
         based on `Ironic Python Agent`_.
         
         * Free software: Apache license
         * Documentation: https://docs.openstack.org/ironic-python-agent-builder
         * Source: https://opendev.org/openstack/ironic-python-agent-builder
-        * Bugs: https://storyboard.openstack.org/#!/project/948
+        * Bugs: https://bugs.launchpad.net/ironic-python-agent-builder
         * Release Notes: https://docs.openstack.org/releasenotes/ironic-python-agent-builder/
         
         .. _Ironic Python Agent: https://docs.openstack.org/ironic-python-agent
         
         
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
```

### Comparing `ironic-python-agent-builder-5.2.1/README.rst` & `ironic-python-agent-builder-5.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 
 Tools and scripts to build a deployment, cleaning or inspection ramdisk
 based on `Ironic Python Agent`_.
 
 * Free software: Apache license
 * Documentation: https://docs.openstack.org/ironic-python-agent-builder
 * Source: https://opendev.org/openstack/ironic-python-agent-builder
-* Bugs: https://storyboard.openstack.org/#!/project/948
+* Bugs: https://bugs.launchpad.net/ironic-python-agent-builder
 * Release Notes: https://docs.openstack.org/releasenotes/ironic-python-agent-builder/
 
 .. _Ironic Python Agent: https://docs.openstack.org/ironic-python-agent
```

### Comparing `ironic-python-agent-builder-5.2.1/dib/extra-hardware/README.rst` & `ironic-python-agent-builder-5.3.0/dib/extra-hardware/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/extra-hardware/install.d/extra-hardware-source-install/80-extra-hardware-install` & `ironic-python-agent-builder-5.3.0/dib/extra-hardware/install.d/extra-hardware-source-install/80-extra-hardware-install`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/README.rst` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/environment.d/10-defaults.bash` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/environment.d/10-defaults.bash`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/60-ironic-python-agent-ramdisk-install` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/60-ironic-python-agent-ramdisk-install`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/ironic-python-agent.init` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/install.d/ironic-python-agent-ramdisk-source-install/ironic-python-agent.init`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/package-installs.yaml` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/package-installs.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/pkg-map` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/pkg-map`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-ramdisk/post-install.d/99-remove-extra-packages` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-ramdisk/post-install.d/99-remove-extra-packages`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     done
 done
 
 # TODO(dtantsur): implement the same for debian-based systems
 case "$DISTRO_NAME" in
     fedora|centos|rhel)
         ${YUM:-yum} remove -y postfix gcc make
-        # Remove webkit... Save ~26MB. This is a ramdisk, not a web brower.
+        # Remove webkit... Save ~26MB. This is a ramdisk, not a web browser.
         ${YUM:-yum} remove -y webkit2gtk3-jsc libproxy-webkitgtk4 || true
         # Remove polkit... Save ~23 MB. This is a ramdisk, not a desktop.
         ${YUM:-yum} remove -y polkit polkit-libs PackageKit polkit-pkla-compat || true
 
         ${YUM:-yum} clean all
         # Rebuilding the rpm database after removing packages will reduce
         # its size
```

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-tls/README.rst` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-tls/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 =======================
 Adds TLS support to ironic-python-agent-ramdisk.
 
 If enabled without any environment variables set to modify configuration,
 this element will enable TLS API support in IPA with a self-signed certificate
 and key created at build time.
 
-Optionally, you can provide your own SSL certifiate and key, and optionally
+Optionally, you can provide your own SSL certificate and key, and optionally
 ca, via the following environment variables. They should be set to an
 accessible path on the build systems filesystem. If set, they will be copied
 into the built ramdisk, and IPA will be configured to use them.
 
 The environment variables are:
  - ``DIB_IPA_CERT_FILE`` should point to the TLS certificate for ramdisk use.
  - ``DIB_IPA_KEY_FILE`` should point to the private key matching
```

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-python-agent-tls/pre-finalise.d/10-configure-ipa-tls` & `ironic-python-agent-builder-5.3.0/dib/ironic-python-agent-tls/pre-finalise.d/10-configure-ipa-tls`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/README.rst` & `ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/cleanup.d/98-prepare-resolve-conf` & `ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/cleanup.d/98-prepare-resolve-conf`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/dib/ironic-ramdisk-base/cleanup.d/99-ramdisk-create` & `ironic-python-agent-builder-5.3.0/dib/ironic-ramdisk-base/cleanup.d/99-ramdisk-create`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 sudo mv ./tmp/fstab.new ./etc/fstab
 sudo ln -s ./sbin/init ./
 
 # NOTE(TheJulia): Make a random and urandom entry to handle
 # long standing systemd bug cases where it may, depending on
 # underlying OS config/version, try to open the random number
 # generator before initializing.
-# This class of issue has appeared frquently with systemd,
+# This class of issue has appeared frequently with systemd,
 # https://github.com/systemd/systemd/issues/4167 is a commonly
 # referenced example of this behavior.
 if ! [ -a ./dev/random ]; then
     sudo mknod ./dev/random c 1 8
 fi
 if ! [ -a ./dev/urandom ]; then
     sudo mknod ./dev/urandom c 1 9
```

### Comparing `ironic-python-agent-builder-5.2.1/doc/source/admin/dib.rst` & `ironic-python-agent-builder-5.3.0/doc/source/admin/dib.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 diskimage-builder images
 ========================
 
 Images built using diskimage-builder_ are recommended for production use on
 real hardware. The recommended distributions are:
 
 * CentOS Stream 9
-* Debian Bullseye and Bookworm (``debian-minimal`` element)
+* Debian Bookworm (``debian-minimal`` element)
 
 The following should work but receive only limited testing and support:
 
 * Ubuntu 20.04 Focal
+* Debian Bullseye (``debian-minimal`` element)
 
 Building
 --------
 
 ... with the helper script
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -181,15 +182,15 @@
 The list can be found below this paragraph. The majority of these firmware
 images are used by SoCs, WI-FI chips, some GPUs and Smartnics which are
 unlikely to be encountered. If you want to override this, change the
 ``IPA_REMOVE_FIRMWARE`` environment variable to a comma-separated list
 of directories or files under ``/usr/lib/firmware``.
 Set it to an empty string to disable firmware removal.
 
-Fimrware removed:
+Firmware removed:
 
 * ``amdgpu``
 * ``netronome``
 * ``qcom``
 * ``ti-communication``
 * ``ti-keystone``
 * ``ueagle-atm``
@@ -270,15 +271,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 Adds TLS support to ironic-python-agent-ramdisk.
 
 By default this element will enable TLS API support in IPA with a self-signed
 certificate and key created at build time.
 
-Optionally, you can provide your own SSL certifiate and key, and optionally
+Optionally, you can provide your own SSL certificate and key, and optionally
 CA, via the following environment variables. They should be set to an
 accessible path on the build systems filesystem. If set, they will be copied
 into the built ramdisk, and IPA will be configured to use them.
 
 The environment variables are:
 
 * ``DIB_IPA_CERT_FILE`` should point to the TLS certificate for ramdisk use.
```

### Comparing `ironic-python-agent-builder-5.2.1/doc/source/admin/tinyipa.rst` & `ironic-python-agent-builder-5.3.0/doc/source/admin/tinyipa.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/doc/source/conf.py` & `ironic-python-agent-builder-5.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/doc/source/contributor/index.rst` & `ironic-python-agent-builder-5.3.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/doc/source/install/index.rst` & `ironic-python-agent-builder-5.3.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/ironic_python_agent_builder/__init__.py` & `ironic-python-agent-builder-5.3.0/ironic_python_agent_builder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,18 @@
         os.environ['DIB_RELEASE'] = args.release
     if args.branch:
         os.environ['DIB_REPOREF_ironic_python_agent'] = args.branch
         os.environ['DIB_REPOREF_requirements'] = args.branch
     if args.lzma:
         os.environ['DIB_IPA_COMPRESS_CMD'] = \
             'xz --format=lzma --compress --stdout'
+    # Enable checksum generation by default
+    if 'DIB_CHECKSUM' not in os.environ:
+        os.environ['DIB_CHECKSUM'] = 'sha256'
+
     extra_args = shlex.split(args.extra_args) if args.extra_args else []
     if args.verbose:
         extra_args.append("-x")
     try:
         subprocess.check_call(['disk-image-create', '-o', args.output,
                                'ironic-python-agent-ramdisk',
                                args.distribution] + args.element + extra_args)
```

### Comparing `ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/PKG-INFO` & `ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ironic-python-agent-builder
-Version: 5.2.1
+Version: 5.3.0
 Summary: Tools and scripts to build Ironic Python Agent
 Home-page: https://docs.openstack.org/ironic-python-agent-builder/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===========================
         Ironic Python Agent Builder
@@ -12,15 +12,15 @@
         
         Tools and scripts to build a deployment, cleaning or inspection ramdisk
         based on `Ironic Python Agent`_.
         
         * Free software: Apache license
         * Documentation: https://docs.openstack.org/ironic-python-agent-builder
         * Source: https://opendev.org/openstack/ironic-python-agent-builder
-        * Bugs: https://storyboard.openstack.org/#!/project/948
+        * Bugs: https://bugs.launchpad.net/ironic-python-agent-builder
         * Release Notes: https://docs.openstack.org/releasenotes/ironic-python-agent-builder/
         
         .. _Ironic Python Agent: https://docs.openstack.org/ironic-python-agent
         
         
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
```

### Comparing `ironic-python-agent-builder-5.2.1/ironic_python_agent_builder.egg-info/SOURCES.txt` & `ironic-python-agent-builder-5.3.0/ironic_python_agent_builder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 releasenotes/notes/centos8-stream-d9c83190e987e07d.yaml
 releasenotes/notes/centos9-0f925822a2ab9e0a.yaml
 releasenotes/notes/clean-var-tmp-with-dib-builds-cd31a2cf70a7f935.yaml
 releasenotes/notes/create-ramdisk-random-devices-263f78a2ef40dbe2.yaml
 releasenotes/notes/debian-9a4fa6b2d3ef96d0.yaml
 releasenotes/notes/debian-arm64-fc3cc4949e3100d9.yaml
 releasenotes/notes/debian-firmware-1927601ebb779bc4.yaml
+releasenotes/notes/debian-ipa-cb5975e436cba525.yaml
 releasenotes/notes/dhcp-predictible-ifnames-b2a1d9e6471b6819.yaml
 releasenotes/notes/drop-python2-534124afa50f62dd.yaml
 releasenotes/notes/excess-firmware-removal-debian-06c49a8604122b1c.yaml
 releasenotes/notes/extra-hardware-73e3c9b5a0143bfa.yaml
 releasenotes/notes/ironic-lib-6a16f13fc6ec9a50.yaml
 releasenotes/notes/ironic-ramdisk-base-3bfb9b90ad416891.yaml
 releasenotes/notes/linux-firmware-9a6f8a9a32c5719d.yaml
@@ -106,14 +107,15 @@
 releasenotes/notes/no-suse-e15d8384c423251c.yaml
 releasenotes/notes/python2-removal-dee895550b1959af.yaml
 releasenotes/notes/remove-PYOPTIMIZE_TINYIPA-ebde63911d140209.yaml
 releasenotes/notes/selinux-permissive-a059f42bb66373a1.yaml
 releasenotes/notes/tinycore13-caba5a4998bdd628.yaml
 releasenotes/notes/tinyipa-tgt-226f74125238c239.yaml
 releasenotes/source/2023.1.rst
+releasenotes/source/2023.2.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/wallaby.rst
 releasenotes/source/xena.rst
 releasenotes/source/yoga.rst
 releasenotes/source/zed.rst
@@ -135,20 +137,18 @@
 tinyipa/finalise-tinyipa.sh
 tinyipa/generate_tox_constraints.sh
 tinyipa/install-deps.sh
 tinyipa/tc-mirror.sh
 tinyipa/udhcpc.script
 tinyipa/build_files/bootlocal.sh
 tinyipa/build_files/buildreqs.lst
-tinyipa/build_files/buildreqs_python2.lst
 tinyipa/build_files/buildreqs_python3.lst
 tinyipa/build_files/dhcp.sh
 tinyipa/build_files/fakeuname
 tinyipa/build_files/finalreqs.lst
-tinyipa/build_files/finalreqs_python2.lst
 tinyipa/build_files/finalreqs_python3.lst
 tinyipa/build_files/isolinux.cfg
 tinyipa/build_files/modprobe.conf
 tinyipa/build_files/ntpdate
 tools/iso-image-create
 zuul.d/ironic-python-agent-builder-jobs.yaml
 zuul.d/project.yaml
```

### Comparing `ironic-python-agent-builder-5.2.1/playbooks/ironic-python-agent-build-image/post.yaml` & `ironic-python-agent-builder-5.3.0/playbooks/ironic-python-agent-build-image/post.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/releasenotes/notes/network-manager-auto-dhcp-all-interfaces-rhel-centos-relese-gt-7-0c2054d0067c6e93.yaml` & `ironic-python-agent-builder-5.3.0/releasenotes/notes/network-manager-auto-dhcp-all-interfaces-rhel-centos-relese-gt-7-0c2054d0067c6e93.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/releasenotes/source/conf.py` & `ironic-python-agent-builder-5.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/defaults/main.yaml` & `ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/tasks/install.yaml` & `ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/tasks/install.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/roles/ipa-build-dib-image/tasks/main.yaml` & `ironic-python-agent-builder-5.3.0/roles/ipa-build-dib-image/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/roles/ipa-build-tinyipa-image/tasks/main.yaml` & `ironic-python-agent-builder-5.3.0/roles/ipa-build-tinyipa-image/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/setup.cfg` & `ironic-python-agent-builder-5.3.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -19,11 +19,14 @@
 
 [files]
 packages = 
 	ironic_python_agent_builder
 data_files = 
 	share/ironic-python-agent-builder/dib = dib/*
 
+[codespell]
+quiet-level = 4
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ironic-python-agent-builder-5.2.1/setup.py` & `ironic-python-agent-builder-5.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/Makefile` & `ironic-python-agent-builder-5.3.0/tinyipa/Makefile`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/add-ssh-tinyipa.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/add-ssh-tinyipa.sh`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # During rebuild this script installs and configures OpenSSH server if needed
 # and makes required changes for Ansible + Python to work in compiled/optimized
 # Python environment.
 #
 # By default, id_rsa or id_dsa keys  of the user performing the build
 # are baked into the image as authorized_keys for 'tc' user.
-# To supply different public ssh key, befor running this script set
+# To supply different public ssh key, before running this script set
 # SSH_PUBLIC_KEY environment variable to point to absolute path to the key.
 #
 # This script produces "ansible-<tinyipa-ramdisk-name>" ramdisk that can serve
 # as ramdisk for both ansible-deploy driver and agent-based Ironic drivers,
 
 set -ex
 WORKDIR=$(readlink -f $0 | xargs dirname)
```

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/build-instance-images.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/build-instance-images.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/build-iso.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/build-iso.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/build-tinyipa.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/build-tinyipa.sh`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 set -ex
 WORKDIR=$(readlink -f $0 | xargs dirname)
 source ${WORKDIR}/common.sh
 
 IRONIC_LIB_SOURCE=${IRONIC_LIB_SOURCE:-}
 
-TC_RELEASE="14.x"
+TC_RELEASE="15.x"
 QEMU_RELEASE="v5.2.0"
 LSHW_RELEASE="B.02.18"
 BIOSDEVNAME_RELEASE="0.7.2"
-IPMITOOL_GIT_HASH="710888479332a46bad78f3d736eff0cbdefd2d1b"
+IPMITOOL_GIT_HASH="19d78782d795d0cf4ceefe655f616210c9143e62"
 
 CHROOT_CMD="sudo chroot $BUILDDIR /usr/bin/env -i PATH=$CHROOT_PATH http_proxy=$http_proxy https_proxy=$https_proxy no_proxy=$no_proxy"
 
 function clone_single_branch {
     git clone --branch $3 --depth=1 $1 $2
 }
 
@@ -38,15 +38,15 @@
 
 cd $WORKDIR/build_files
 wget -N $TINYCORE_MIRROR_URL/$TC_RELEASE/x86_64/release/distribution_files/corepure64.gz
 wget -N $TINYCORE_MIRROR_URL/$TC_RELEASE/x86_64/release/distribution_files/vmlinuz64
 cd $WORKDIR
 
 ########################################################
-# Build Required Python Dependecies in a Build Directory
+# Build Required Python Dependencies in a Build Directory
 ########################################################
 
 # Make directory for building in
 mkdir "$BUILDDIR"
 
 # Extract rootfs from .gz file
 ( cd "$BUILDDIR" && zcat $WORKDIR/build_files/corepure64.gz | sudo cpio -i -H newc -d )
@@ -57,33 +57,30 @@
 # Download Qemu-utils, Biosdevname and IPMItool source
 clone_single_branch "https://github.com/qemu/qemu.git" "${BUILDDIR}/tmp/qemu" "$QEMU_RELEASE"
 clone_single_branch "https://github.com/lyonel/lshw.git" "${BUILDDIR}/tmp/lshw" "$LSHW_RELEASE"
 if $TINYIPA_REQUIRE_BIOSDEVNAME; then
     wget -N -O - https://linux.dell.com/biosdevname/biosdevname-${BIOSDEVNAME_RELEASE}/biosdevname-${BIOSDEVNAME_RELEASE}.tar.gz | tar -xz -C "${BUILDDIR}/tmp" -f -
 fi
 if $TINYIPA_REQUIRE_IPMITOOL; then
-    git clone https://github.com/ipmitool/ipmitool.git "${BUILDDIR}/tmp/ipmitool-src"
+    git clone https://codeberg.org/IPMITool/ipmitool.git "${BUILDDIR}/tmp/ipmitool-src"
     cd "${BUILDDIR}/tmp/ipmitool-src"
     git reset $IPMITOOL_GIT_HASH --hard
     cd -
 fi
 
 # Create directory for python local mirror
 mkdir -p "$BUILDDIR/tmp/localpip"
 
 # Download IPA and requirements
 IPA_SOURCE_DIR=${IPA_SOURCE_DIR:-/opt/stack/ironic-python-agent}
 cd $IPA_SOURCE_DIR
 rm -rf *.egg-info
 pwd
 
-PYTHON_COMMAND="python"
-if [[ $USE_PYTHON3 == "True" ]]; then
-    PYTHON_COMMAND="python3"
-fi
+PYTHON_COMMAND="python3"
 $PYTHON_COMMAND setup.py sdist --dist-dir "$BUILDDIR/tmp/localpip" --quiet
 
 ls $BUILDDIR/tmp/localpip || true
 cp requirements.txt $BUILDDIR/tmp/ipa-requirements.txt
 
 if [ -n "$IRONIC_LIB_SOURCE" ]; then
     pushd $IRONIC_LIB_SOURCE
@@ -141,35 +138,29 @@
     done
 fi
 
 $CHROOT_CMD mkdir -m777 /etc/sysconfig/tcedir
 $CHROOT_CMD touch /etc/sysconfig/tcuser
 $CHROOT_CMD chmod a+rwx /etc/sysconfig/tcuser
 
-mkdir $BUILDDIR/tmp/overides
-cp $WORKDIR/build_files/fakeuname $BUILDDIR/tmp/overides/uname
+mkdir $BUILDDIR/tmp/overrides
+cp $WORKDIR/build_files/fakeuname $BUILDDIR/tmp/overrides/uname
 
 sudo cp $WORKDIR/build_files/ntpdate $BUILDDIR/bin/ntpdate
 
-PY_REQS="buildreqs_python2.lst"
-if [[ $USE_PYTHON3 == "True" ]]; then
-    PY_REQS="buildreqs_python3.lst"
-fi
+PY_REQS="buildreqs_python3.lst"
 
 # NOTE(rpittau) change ownership of the tce info dir to prevent writing issues
 sudo chown $TC:$STAFF $BUILDDIR/usr/local/tce.installed
 
 while read line; do
     sudo chroot --userspec=$TC:$STAFF $BUILDDIR /usr/bin/env -i PATH=$CHROOT_PATH http_proxy=$http_proxy https_proxy=$https_proxy no_proxy=$no_proxy tce-load -wci $line
 done < <(paste $WORKDIR/build_files/$PY_REQS $WORKDIR/build_files/buildreqs.lst)
 
-TINYIPA_PYTHON_EXE="python"
-if [[ $USE_PYTHON3 == "True" ]]; then
-    TINYIPA_PYTHON_EXE="python3.9"
-fi
+TINYIPA_PYTHON_EXE="python3.9"
 
 PIP_COMMAND="$TINYIPA_PYTHON_EXE -m pip"
 
 # Build python wheels
 $CHROOT_CMD ${TINYIPA_PYTHON_EXE} -m ensurepip
 $CHROOT_CMD ${PIP_COMMAND} install --upgrade pip==${PIP_VERSION} wheel
 $CHROOT_CMD ${PIP_COMMAND} install pbr
```

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/build_files/bootlocal.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/build_files/bootlocal.sh`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     echo "Starting haveged entropy daemon:"
     /usr/local/sbin/haveged
 fi
 
 # Maybe save some RAM?
 #rm -rf /tmp/builtin
 
-# Install IPA and dependecies
+# Install IPA and dependencies
 if ! type "ironic-python-agent" > /dev/null ; then
     PIP_COMMAND="pip"
     if hash pip3 2>/dev/null; then
         PIP_COMMAND="pip3"
     fi
     $PIP_COMMAND install --no-index --find-links=file:///tmp/wheelhouse ironic_python_agent
 fi
```

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/build_files/dhcp.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/build_files/dhcp.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/build_files/fakeuname` & `ironic-python-agent-builder-5.3.0/tinyipa/build_files/fakeuname`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/bin/sh
 
 S="Linux"
 N="box"
-R="6.1.2-tinycore64"
+R="6.6.8-tinycore64"
 P="unknown"
 V="#2017 SMP"
 M="x86_64"
 I="unknown"
 O="GNU/Linux"
 
 OPT_A=false
```

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/common.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/common.sh`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 BUILDDIR="$WORKDIR/tinyipabuild"
 
 PIP_VERSION="21.3.1"
 
 TINYIPA_REQUIRE_BIOSDEVNAME=${TINYIPA_REQUIRE_BIOSDEVNAME:-false}
 TINYIPA_REQUIRE_IPMITOOL=${TINYIPA_REQUIRE_IPMITOOL:-true}
-USE_PYTHON3=${USE_PYTHON3:-True}
 
 # PYTHON_EXTRA_SOURCES_DIR_LIST is a csv list of python package dirs to include
 PYTHON_EXTRA_SOURCES_DIR_LIST=${PYTHON_EXTRA_SOURCES_DIR_LIST:-}
 
 # Allow an extension to be added to the generated files by specifying
 # $BRANCH_PATH e.g. export BRANCH_PATH=master results in tinyipa-master.gz etc
 BRANCH_EXT=''
@@ -21,15 +20,15 @@
     BRANCH_EXT="-$BRANCH_PATH"
 fi
 export BRANCH_EXT
 
 TC=1001
 STAFF=50
 
-CHROOT_PATH="/tmp/overides:/usr/local/sbin:/usr/local/bin:/apps/bin:/usr/sbin:/usr/bin:/sbin:/bin"
+CHROOT_PATH="/tmp/overrides:/usr/local/sbin:/usr/local/bin:/apps/bin:/usr/sbin:/usr/bin:/sbin:/bin"
 CHROOT_CMD="sudo chroot $DST_DIR /usr/bin/env -i PATH=$CHROOT_PATH http_proxy=$http_proxy https_proxy=$https_proxy no_proxy=$no_proxy"
 TC_CHROOT_CMD="sudo chroot --userspec=$TC:$STAFF $DST_DIR /usr/bin/env -i PATH=$CHROOT_PATH http_proxy=$http_proxy https_proxy=$https_proxy no_proxy=$no_proxy"
 
 function setup_tce {
     # Setup resolv.conf, add mirrors, mount proc
     local dst_dir="$1"
```

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/finalise-tinyipa.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/finalise-tinyipa.sh`

 * *Files 1% similar despite different names*

```diff
@@ -81,23 +81,20 @@
 if $TINYIPA_REQUIRE_BIOSDEVNAME; then
     cp $WORKDIR/build_files/biosdevname.* $FINALDIR/tmp/builtin/optional
 fi
 if $TINYIPA_REQUIRE_IPMITOOL; then
     cp $WORKDIR/build_files/ipmitool.* $FINALDIR/tmp/builtin/optional
 fi
 
-mkdir $FINALDIR/tmp/overides
-cp $WORKDIR/build_files/fakeuname $FINALDIR/tmp/overides/uname
+mkdir $FINALDIR/tmp/overrides
+cp $WORKDIR/build_files/fakeuname $FINALDIR/tmp/overrides/uname
 
 sudo cp $WORKDIR/build_files/ntpdate $FINALDIR/bin/ntpdate
 sudo chmod 755 $FINALDIR/bin/ntpdate
-PY_REQS="finalreqs_python2.lst"
-if [[ $USE_PYTHON3 == "True" ]]; then
-    PY_REQS="finalreqs_python3.lst"
-fi
+PY_REQS="finalreqs_python3.lst"
 
 # NOTE(rpittau) change ownership of the tce info dir to prevent writing issues
 sudo chown $TC:$STAFF $FINALDIR/usr/local/tce.installed
 
 while read line; do
     $TC_CHROOT_CMD tce-load -wic $line
 done < <(paste $WORKDIR/build_files/finalreqs.lst $WORKDIR/build_files/$PY_REQS)
@@ -136,20 +133,16 @@
 if $TINYIPA_REQUIRE_IPMITOOL; then
     $TC_CHROOT_CMD tce-load -ic /tmp/builtin/optional/ipmitool.tcz
 fi
 
 # Ensure tinyipa picks up installed kernel modules
 $CHROOT_CMD depmod -a `$WORKDIR/build_files/fakeuname -r`
 
-PIP_COMMAND="pip"
-TINYIPA_PYTHON_EXE="python"
-if [[ $USE_PYTHON3 == "True" ]]; then
-    PIP_COMMAND="pip3"
-    TINYIPA_PYTHON_EXE="python3"
-fi
+PIP_COMMAND="pip3"
+TINYIPA_PYTHON_EXE="python3"
 
 # Install pip
 # NOTE(rpittau): pip MUST be the same version used in the build script or
 # dragons will appear and put everything on fire
 $CHROOT_CMD ${TINYIPA_PYTHON_EXE} -m ensurepip
 $CHROOT_CMD ${PIP_COMMAND} install --upgrade pip==${PIP_VERSION} wheel
 
@@ -184,15 +177,15 @@
 # Disable ZSwap
 sudo sed -i '/# Main/a NOZSWAP=1' "$FINALDIR/etc/init.d/tc-config"
 # sudo cp $WORKDIR/build_files/tc-config $FINALDIR/etc/init.d/tc-config
 
 # Place ipv6 modprobe config so the kernel support loads.
 sudo cp "$WORKDIR/build_files/modprobe.conf" "$FINALDIR/etc/modproble.conf"
 
-# NOTE(rpittau): workaorund for hwclock
+# NOTE(rpittau): workaround for hwclock
 # The adjtime file used by hwclock in tinycore is /var/lib/hwclock/adjtime
 # but for some reason (bug?) the file is not created when hwclock is
 # invoked, causing hwclock to fail when using certain options, for example
 # --systohc.
 # We create the dir and the file to prevent that.
 $CHROOT_CMD mkdir -p /var/lib/hwclock
 $CHROOT_CMD touch /var/lib/hwclock/adjtime
```

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/generate_tox_constraints.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/generate_tox_constraints.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/install-deps.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/install-deps.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/tc-mirror.sh` & `ironic-python-agent-builder-5.3.0/tinyipa/tc-mirror.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tinyipa/udhcpc.script` & `ironic-python-agent-builder-5.3.0/tinyipa/udhcpc.script`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tools/iso-image-create` & `ironic-python-agent-builder-5.3.0/tools/iso-image-create`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-builder-5.2.1/tox.ini` & `ironic-python-agent-builder-5.3.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 [testenv]
 usedevelop = True
 basepython = python3
 setenv =
    VIRTUAL_ENV={envdir}
    PYTHONWARNINGS=default::DeprecationWarning
 deps =
-  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.2}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/doc/requirements.txt
 
 [testenv:pep8]
 deps =
-    hacking~=6.0.0 # Apache-2.0
+    hacking~=6.1.0 # Apache-2.0
     flake8-import-order>=0.17.1 # LGPLv3
     doc8>=0.6.0 # Apache-2.0
     pycodestyle>=2.0.0,<3.0.0 # MIT
 commands =
     flake8 ironic_python_agent_builder
     doc8 doc/source README.rst CONTRIBUTING.rst
 
@@ -48,7 +48,17 @@
 # [H106] Don't put vim configuration in source files.
 # [H203] Use assertIs(Not)None to check for None.
 # [H204] Use assert(Not)Equal to check for equality.
 # [H205] Use assert(Greater|Less)(Equal) for comparison.
 # [H210] Require 'autospec', 'spec', or 'spec_set' in mock.patch/mock.patch.object calls
 # [H904] Delay string interpolations at logging calls.
 enable-extensions=H106,H203,H204,H205,H210,H904
+
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

### Comparing `ironic-python-agent-builder-5.2.1/zuul.d/ironic-python-agent-builder-jobs.yaml` & `ironic-python-agent-builder-5.3.0/zuul.d/ironic-python-agent-builder-jobs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     name: ironic-python-agent-build-image-dib-debian
     parent: ironic-python-agent-build-image-base
     required-projects:
       - openstack/diskimage-builder
     vars:
       image_type: 'dib'
       image_distro: 'debian-minimal'
-      image_release: 'bullseye'
+      image_release: 'bookworm'
 
 - job:
     name: ironic-python-agent-check-image-base
     parent: base
     nodeset: ubuntu-jammy
     pre-run: playbooks/ironic-python-agent-build-image/pre.yaml
     run: playbooks/ironic-python-agent-build-image/run.yaml
@@ -93,14 +93,20 @@
     name: ironic-python-agent-check-image-dib-debian
     parent: ironic-python-agent-check-image-base
     required-projects:
       - openstack/diskimage-builder
     vars:
       image_type: 'dib'
       image_distro: 'debian-minimal'
+      image_release: 'bookworm'
+
+- job:
+    name: ironic-python-agent-check-image-dib-debian-bullseye
+    parent: ironic-python-agent-check-image-dib-debian
+    vars:
       image_release: 'bullseye'
 
 - job:
     name: ironic-python-agent-check-image-dib-debian-arm64
     parent: ironic-python-agent-check-image-dib-debian
     nodeset: debian-bullseye-arm64
     vars:
@@ -132,7 +138,15 @@
 
 - job:
     name: ironic-python-agent-check-image-dib-ubuntu-arm64
     parent: ironic-python-agent-check-image-dib-ubuntu
     nodeset: ubuntu-jammy-arm64
     vars:
       image_target_name: ubuntu-arm64
+
+
+- job:
+    name: ironic-python-agent-builder-tox-codespell
+    parent: openstack-tox
+    timeout: 7200
+    vars:
+      tox_envlist: codespell
```

### Comparing `ironic-python-agent-builder-5.2.1/zuul.d/project.yaml` & `ironic-python-agent-builder-5.3.0/zuul.d/project.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,26 @@
         - ironic-python-agent-check-image-tinyipa
         - ironic-python-agent-check-image-dib-centos9
         - ironic-python-agent-check-image-dib-centos9-extra
         - ironic-python-agent-check-image-dib-debian
         - ironic-python-agent-check-image-dib-debian-arm64
         - ironic-python-agent-check-image-dib-debian-extra
         # Non-voting jobs
+        - ironic-python-agent-check-image-dib-debian-bullseye:
+            voting: false
         - ironic-python-agent-check-image-dib-ubuntu:
             voting: false
         - ironic-python-agent-check-image-dib-ubuntu-arm64:
             voting: false
         - ipa-tempest-bios-ipmi-direct-src:
             voting: false
         - ipa-tempest-ironic-inspector-src:
             voting: false
+        - ironic-python-agent-builder-tox-codespell:
+            voting: false
     gate:
       jobs:
         - openstack-tox-pep8
         - ironic-standalone-ipa-src
         - ipa-tempest-bios-ipmi-direct-tinyipa-src
         - ironic-python-agent-check-image-tinyipa
         - ironic-python-agent-check-image-dib-centos9
```

