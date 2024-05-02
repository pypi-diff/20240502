# Comparing `tmp/libvirt-python-9.8.0.tar.gz` & `tmp/libvirt-python-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvirt-python-9.8.0.tar", last modified: Mon Oct  2 07:33:34 2023, max compression
+gzip compressed data, was "libvirt-python-9.9.0.tar", last modified: Wed Nov  1 09:42:54 2023, max compression
```

## Comparing `libvirt-python-9.8.0.tar` & `libvirt-python-9.9.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.402565 libvirt-python-9.8.0/
--rw-rw-r--   0 jirka      (500) jirka      (500)       27 2014-06-19 09:18:44.000000 libvirt-python-9.8.0/.ctags
--rw-rw-r--   0 jirka      (500) jirka      (500)      171 2014-06-19 09:18:44.000000 libvirt-python-9.8.0/.dir-locals.el
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.392565 libvirt-python-9.8.0/.github/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.395898 libvirt-python-9.8.0/.github/workflows/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1486 2021-12-01 09:53:22.000000 libvirt-python-9.8.0/.github/workflows/lockdown.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      100 2023-01-16 10:59:44.000000 libvirt-python-9.8.0/.gitignore
--rw-rw-r--   0 jirka      (500) jirka      (500)     2795 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/.gitlab-ci.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      554 2016-10-04 07:42:23.000000 libvirt-python-9.8.0/.mailmap
--rw-rw-r--   0 jirka      (500) jirka      (500)     4008 2023-10-02 07:33:34.000000 libvirt-python-9.8.0/AUTHORS
--rw-rw-r--   0 jirka      (500) jirka      (500)      236 2014-06-19 09:18:44.000000 libvirt-python-9.8.0/AUTHORS.in
--rw-rw-r--   0 jirka      (500) jirka      (500)     1023 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 jirka      (500) jirka      (500)    26521 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/COPYING
--rw-rw-r--   0 jirka      (500) jirka      (500)   423335 2023-10-02 07:33:34.000000 libvirt-python-9.8.0/ChangeLog
--rw-rw-r--   0 jirka      (500) jirka      (500)     1491 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/HACKING
--rw-rw-r--   0 jirka      (500) jirka      (500)      326 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/MANIFEST.in
--rw-rw-r--   0 jirka      (500) jirka      (500)      304 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/Makefile
--rw-r--r--   0 jirka      (500) jirka      (500)     2542 2023-10-02 07:33:34.402565 libvirt-python-9.8.0/PKG-INFO
--rw-rw-r--   0 jirka      (500) jirka      (500)     1988 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/README
--rw-rw-r--   0 jirka      (500) jirka      (500)        6 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/VERSION
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.392565 libvirt-python-9.8.0/build/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.402565 libvirt-python-9.8.0/build/libvirt_python.egg-info/
--rw-rw-r--   0 jirka      (500) jirka      (500)     2335 2023-10-02 07:33:34.000000 libvirt-python-9.8.0/build/libvirt_python.egg-info/SOURCES.txt
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.395898 libvirt-python-9.8.0/ci/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.399232 libvirt-python-9.8.0/ci/buildenv/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1463 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/centos-stream-8.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1021 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/centos-stream-9.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/debian-10.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1113 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/debian-sid.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      822 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/fedora-37.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      822 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/fedora-38.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      874 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/fedora-rawhide.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      905 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/opensuse-leap-15.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      911 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/opensuse-tumbleweed.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/ubuntu-2004.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/buildenv/ubuntu-2204.sh
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.399232 libvirt-python-9.8.0/ci/containers/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1556 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/centos-stream-8.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1115 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/centos-stream-9.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1478 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/debian-10.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1446 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/debian-sid.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1312 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/fedora-37.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1312 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/fedora-38.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1374 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/fedora-rawhide.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)      965 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/opensuse-leap-15.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)      979 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/opensuse-tumbleweed.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1476 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/ubuntu-2004.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1476 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/containers/ubuntu-2204.Dockerfile
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.399232 libvirt-python-9.8.0/ci/gitlab/
--rw-rw-r--   0 jirka      (500) jirka      (500)     6071 2023-05-02 11:04:38.000000 libvirt-python-9.8.0/ci/gitlab/build-templates.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     5842 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/gitlab/builds.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1573 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/gitlab/container-templates.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1445 2023-05-17 07:45:20.000000 libvirt-python-9.8.0/ci/gitlab/containers.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      938 2023-05-02 11:04:38.000000 libvirt-python-9.8.0/ci/gitlab/sanity-checks.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     2754 2023-05-02 11:04:38.000000 libvirt-python-9.8.0/ci/gitlab.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1473 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/ci/manifest.yml
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.399232 libvirt-python-9.8.0/examples/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1592 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/README
--rw-rw-r--   0 jirka      (500) jirka      (500)     3300 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/consolecallback.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1663 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/dhcpleases.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     2107 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/dominfo.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1568 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/domipaddrs.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)      690 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/domrestore.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)      762 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/domsave.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1239 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/domstart.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     5066 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/esxlist.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)    36317 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/examples/event-test.py
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.399232 libvirt-python-9.8.0/examples/guest-vcpus/
--rwxrwxr-x   0 jirka      (500) jirka      (500)     3880 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/guest-vcpus/guest-vcpu-daemon.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1588 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/guest-vcpus/guest-vcpu.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     2782 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/nodestats.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     3857 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/sparsestream.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1235 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/examples/topology.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)    70080 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/generator.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      737 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-lxc-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)     3276 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-lxc-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    59229 2022-06-01 07:30:40.000000 libvirt-python-9.8.0/libvirt-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)    31488 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/libvirt-override-virConnect.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     5628 2023-01-16 10:59:44.000000 libvirt-python-9.8.0/libvirt-override-virDomain.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      716 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-override-virDomainCheckpoint.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      702 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-override-virDomainSnapshot.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      381 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-override-virNetwork.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      396 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-override-virStoragePool.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    11453 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-override-virStream.py
--rw-rw-r--   0 jirka      (500) jirka      (500)   331932 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/libvirt-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    10085 2022-05-02 11:37:45.000000 libvirt-python-9.8.0/libvirt-override.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     2725 2023-10-02 07:33:34.000000 libvirt-python-9.8.0/libvirt-python.spec
--rw-rw-r--   0 jirka      (500) jirka      (500)     2732 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/libvirt-python.spec.in
--rw-rw-r--   0 jirka      (500) jirka      (500)     1135 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-qemu-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)    14056 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/libvirt-qemu-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)     3452 2022-05-02 11:37:45.000000 libvirt-python-9.8.0/libvirt-qemu-override.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    16206 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/libvirt-utils.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    13274 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/libvirt-utils.h
--rw-rw-r--   0 jirka      (500) jirka      (500)    16957 2022-07-01 09:27:33.000000 libvirt-python-9.8.0/libvirtaio.py
--rw-rw-r--   0 jirka      (500) jirka      (500)       81 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/pyproject.toml
--rw-rw-r--   0 jirka      (500) jirka      (500)       10 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/requirements-test.txt
--rw-rw-r--   0 jirka      (500) jirka      (500)      639 2023-10-02 07:33:34.402565 libvirt-python-9.8.0/setup.cfg
--rwxrwxr-x   0 jirka      (500) jirka      (500)     8914 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/setup.py
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-10-02 07:33:34.402565 libvirt-python-9.8.0/tests/
--rw-rw-r--   0 jirka      (500) jirka      (500)     2774 2022-07-01 09:27:33.000000 libvirt-python-9.8.0/tests/eventmock.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     6016 2022-07-01 09:27:33.000000 libvirt-python-9.8.0/tests/test_aio.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    16198 2022-05-02 11:37:45.000000 libvirt-python-9.8.0/tests/test_api_coverage.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     2884 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/tests/test_conn.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      758 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/tests/test_domain.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      552 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/tests/test_domain_checkpoint.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      398 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/tests/test_domain_snapshot.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      367 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/tests/test_interface.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      363 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/tests/test_network.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      380 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/tests/test_nodedev.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      600 2022-04-01 10:30:02.000000 libvirt-python-9.8.0/tests/test_storage.py
--rw-rw-r--   0 jirka      (500) jirka      (500)       89 2023-07-03 08:16:56.000000 libvirt-python-9.8.0/tox.ini
--rw-rw-r--   0 jirka      (500) jirka      (500)    10760 2023-10-02 07:33:30.000000 libvirt-python-9.8.0/typewrappers.c
--rw-rw-r--   0 jirka      (500) jirka      (500)     9234 2022-09-20 16:28:07.000000 libvirt-python-9.8.0/typewrappers.h
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.410279 libvirt-python-9.9.0/
+-rw-rw-r--   0 jirka      (500) jirka      (500)       27 2014-06-19 09:18:44.000000 libvirt-python-9.9.0/.ctags
+-rw-rw-r--   0 jirka      (500) jirka      (500)      171 2014-06-19 09:18:44.000000 libvirt-python-9.9.0/.dir-locals.el
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.400279 libvirt-python-9.9.0/.github/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.406946 libvirt-python-9.9.0/.github/workflows/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1486 2021-12-01 09:53:22.000000 libvirt-python-9.9.0/.github/workflows/lockdown.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      100 2023-01-16 10:59:44.000000 libvirt-python-9.9.0/.gitignore
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2795 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/.gitlab-ci.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      554 2016-10-04 07:42:23.000000 libvirt-python-9.9.0/.mailmap
+-rw-rw-r--   0 jirka      (500) jirka      (500)     4008 2023-11-01 09:42:54.000000 libvirt-python-9.9.0/AUTHORS
+-rw-rw-r--   0 jirka      (500) jirka      (500)      236 2014-06-19 09:18:44.000000 libvirt-python-9.9.0/AUTHORS.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1023 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 jirka      (500) jirka      (500)    26521 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/COPYING
+-rw-rw-r--   0 jirka      (500) jirka      (500)   423438 2023-11-01 09:42:54.000000 libvirt-python-9.9.0/ChangeLog
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1491 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/HACKING
+-rw-rw-r--   0 jirka      (500) jirka      (500)      326 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/MANIFEST.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)      304 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/Makefile
+-rw-r--r--   0 jirka      (500) jirka      (500)     2542 2023-11-01 09:42:54.410279 libvirt-python-9.9.0/PKG-INFO
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1988 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/README
+-rw-rw-r--   0 jirka      (500) jirka      (500)        6 2023-11-01 09:42:50.000000 libvirt-python-9.9.0/VERSION
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.400279 libvirt-python-9.9.0/build/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.410279 libvirt-python-9.9.0/build/libvirt_python.egg-info/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2335 2023-11-01 09:42:54.000000 libvirt-python-9.9.0/build/libvirt_python.egg-info/SOURCES.txt
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.406946 libvirt-python-9.9.0/ci/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.406946 libvirt-python-9.9.0/ci/buildenv/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1463 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/centos-stream-8.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1021 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/centos-stream-9.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/debian-10.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1113 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/debian-sid.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      822 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/fedora-37.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      822 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/fedora-38.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      874 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/fedora-rawhide.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      905 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/opensuse-leap-15.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      911 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/opensuse-tumbleweed.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/ubuntu-2004.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1145 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/buildenv/ubuntu-2204.sh
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.406946 libvirt-python-9.9.0/ci/containers/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1556 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/centos-stream-8.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1115 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/centos-stream-9.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1478 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/debian-10.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1446 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/debian-sid.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1312 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/fedora-37.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1312 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/fedora-38.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1374 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/fedora-rawhide.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)      965 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/opensuse-leap-15.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)      979 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/opensuse-tumbleweed.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1476 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/ubuntu-2004.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1476 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/containers/ubuntu-2204.Dockerfile
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.410279 libvirt-python-9.9.0/ci/gitlab/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     6071 2023-05-02 11:04:38.000000 libvirt-python-9.9.0/ci/gitlab/build-templates.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     5842 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/gitlab/builds.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1573 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/gitlab/container-templates.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1445 2023-05-17 07:45:20.000000 libvirt-python-9.9.0/ci/gitlab/containers.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      938 2023-05-02 11:04:38.000000 libvirt-python-9.9.0/ci/gitlab/sanity-checks.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2754 2023-05-02 11:04:38.000000 libvirt-python-9.9.0/ci/gitlab.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1473 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/ci/manifest.yml
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.410279 libvirt-python-9.9.0/examples/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1592 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/README
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3300 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/consolecallback.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1663 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/dhcpleases.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     2107 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/dominfo.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1568 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/domipaddrs.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)      690 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/domrestore.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)      762 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/domsave.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1239 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/domstart.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     5066 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/esxlist.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    36317 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/examples/event-test.py
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.410279 libvirt-python-9.9.0/examples/guest-vcpus/
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     3880 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/guest-vcpus/guest-vcpu-daemon.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1588 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/guest-vcpus/guest-vcpu.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     2782 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/nodestats.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     3857 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/sparsestream.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1235 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/examples/topology.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    70080 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/generator.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      737 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-lxc-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3276 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-lxc-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    59229 2022-06-01 07:30:40.000000 libvirt-python-9.9.0/libvirt-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)    31488 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/libvirt-override-virConnect.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     5628 2023-01-16 10:59:44.000000 libvirt-python-9.9.0/libvirt-override-virDomain.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      716 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-override-virDomainCheckpoint.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      702 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-override-virDomainSnapshot.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      381 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-override-virNetwork.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      396 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-override-virStoragePool.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    11453 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-override-virStream.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)   331932 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/libvirt-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    10085 2022-05-02 11:37:45.000000 libvirt-python-9.9.0/libvirt-override.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2725 2023-11-01 09:42:54.000000 libvirt-python-9.9.0/libvirt-python.spec
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2732 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/libvirt-python.spec.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1135 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-qemu-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)    14056 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/libvirt-qemu-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3452 2022-05-02 11:37:45.000000 libvirt-python-9.9.0/libvirt-qemu-override.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16206 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/libvirt-utils.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    13274 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/libvirt-utils.h
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16957 2022-07-01 09:27:33.000000 libvirt-python-9.9.0/libvirtaio.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)       81 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/pyproject.toml
+-rw-rw-r--   0 jirka      (500) jirka      (500)       10 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/requirements-test.txt
+-rw-rw-r--   0 jirka      (500) jirka      (500)      639 2023-11-01 09:42:54.413612 libvirt-python-9.9.0/setup.cfg
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     8914 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/setup.py
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-11-01 09:42:54.410279 libvirt-python-9.9.0/tests/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2774 2022-07-01 09:27:33.000000 libvirt-python-9.9.0/tests/eventmock.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     6016 2022-07-01 09:27:33.000000 libvirt-python-9.9.0/tests/test_aio.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16198 2022-05-02 11:37:45.000000 libvirt-python-9.9.0/tests/test_api_coverage.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2884 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/tests/test_conn.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      758 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/tests/test_domain.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      552 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/tests/test_domain_checkpoint.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      398 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/tests/test_domain_snapshot.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      367 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/tests/test_interface.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      363 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/tests/test_network.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      380 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/tests/test_nodedev.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      600 2022-04-01 10:30:02.000000 libvirt-python-9.9.0/tests/test_storage.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)       89 2023-07-03 08:16:56.000000 libvirt-python-9.9.0/tox.ini
+-rw-rw-r--   0 jirka      (500) jirka      (500)    10760 2023-10-02 07:33:30.000000 libvirt-python-9.9.0/typewrappers.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)     9234 2022-09-20 16:28:07.000000 libvirt-python-9.9.0/typewrappers.h
```

### Comparing `libvirt-python-9.8.0/.github/workflows/lockdown.yml` & `libvirt-python-9.9.0/.github/workflows/lockdown.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/.gitlab-ci.yml` & `libvirt-python-9.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/.mailmap` & `libvirt-python-9.9.0/.mailmap`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/AUTHORS` & `libvirt-python-9.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/CONTRIBUTING.rst` & `libvirt-python-9.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/COPYING` & `libvirt-python-9.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ChangeLog` & `libvirt-python-9.9.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+ 2023- 10- 2 Jiri Denemark <jdenemar@redhat.com>
+    
+    Post-release version bump to 9.9.0
+    
+    
  2023- 9- 25 Daniel P. Berrangé <berrange@redhat.com>
     
     Request the Python stable API when building
     We have Python 3.6 as a minimum version. If we set Py_LIMITED_API
     to 0x03060000, we'll get the stable python API associated with
     versions >= 3.6. This lets users compile once and have the libvirt
     binary module be loadable by any Python version >= 3.6, as described
```

### Comparing `libvirt-python-9.8.0/HACKING` & `libvirt-python-9.9.0/HACKING`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/PKG-INFO` & `libvirt-python-9.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libvirt-python
-Version: 9.8.0
+Version: 9.9.0
 Summary: The libvirt virtualization API python binding
 Home-page: http://www.libvirt.org
 Maintainer: Libvirt Maintainers
 Maintainer-email: libvir-list@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `libvirt-python-9.8.0/README` & `libvirt-python-9.9.0/README`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/build/libvirt_python.egg-info/SOURCES.txt` & `libvirt-python-9.9.0/build/libvirt_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/centos-stream-8.sh` & `libvirt-python-9.9.0/ci/buildenv/centos-stream-8.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/centos-stream-9.sh` & `libvirt-python-9.9.0/ci/buildenv/centos-stream-9.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/debian-10.sh` & `libvirt-python-9.9.0/ci/buildenv/debian-10.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/debian-sid.sh` & `libvirt-python-9.9.0/ci/buildenv/debian-sid.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/fedora-37.sh` & `libvirt-python-9.9.0/ci/buildenv/fedora-37.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/fedora-38.sh` & `libvirt-python-9.9.0/ci/buildenv/fedora-38.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/fedora-rawhide.sh` & `libvirt-python-9.9.0/ci/buildenv/fedora-rawhide.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/opensuse-leap-15.sh` & `libvirt-python-9.9.0/ci/buildenv/opensuse-leap-15.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/opensuse-tumbleweed.sh` & `libvirt-python-9.9.0/ci/buildenv/opensuse-tumbleweed.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/ubuntu-2004.sh` & `libvirt-python-9.9.0/ci/buildenv/ubuntu-2004.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/buildenv/ubuntu-2204.sh` & `libvirt-python-9.9.0/ci/buildenv/ubuntu-2204.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/centos-stream-8.Dockerfile` & `libvirt-python-9.9.0/ci/containers/centos-stream-8.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/centos-stream-9.Dockerfile` & `libvirt-python-9.9.0/ci/containers/centos-stream-9.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/debian-10.Dockerfile` & `libvirt-python-9.9.0/ci/containers/debian-10.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/debian-sid.Dockerfile` & `libvirt-python-9.9.0/ci/containers/debian-sid.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/fedora-37.Dockerfile` & `libvirt-python-9.9.0/ci/containers/fedora-37.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/fedora-38.Dockerfile` & `libvirt-python-9.9.0/ci/containers/fedora-38.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/fedora-rawhide.Dockerfile` & `libvirt-python-9.9.0/ci/containers/fedora-rawhide.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/opensuse-leap-15.Dockerfile` & `libvirt-python-9.9.0/ci/containers/opensuse-leap-15.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/opensuse-tumbleweed.Dockerfile` & `libvirt-python-9.9.0/ci/containers/opensuse-tumbleweed.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/ubuntu-2004.Dockerfile` & `libvirt-python-9.9.0/ci/containers/ubuntu-2004.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/containers/ubuntu-2204.Dockerfile` & `libvirt-python-9.9.0/ci/containers/ubuntu-2204.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/gitlab/build-templates.yml` & `libvirt-python-9.9.0/ci/gitlab/build-templates.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/gitlab/builds.yml` & `libvirt-python-9.9.0/ci/gitlab/builds.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/gitlab/container-templates.yml` & `libvirt-python-9.9.0/ci/gitlab/container-templates.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/gitlab/containers.yml` & `libvirt-python-9.9.0/ci/gitlab/containers.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/gitlab/sanity-checks.yml` & `libvirt-python-9.9.0/ci/gitlab/sanity-checks.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/gitlab.yml` & `libvirt-python-9.9.0/ci/gitlab.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/ci/manifest.yml` & `libvirt-python-9.9.0/ci/manifest.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/README` & `libvirt-python-9.9.0/examples/README`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/consolecallback.py` & `libvirt-python-9.9.0/examples/consolecallback.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/dhcpleases.py` & `libvirt-python-9.9.0/examples/dhcpleases.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/dominfo.py` & `libvirt-python-9.9.0/examples/dominfo.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/domipaddrs.py` & `libvirt-python-9.9.0/examples/domipaddrs.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/domrestore.py` & `libvirt-python-9.9.0/examples/domrestore.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/domsave.py` & `libvirt-python-9.9.0/examples/domsave.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/domstart.py` & `libvirt-python-9.9.0/examples/domstart.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/esxlist.py` & `libvirt-python-9.9.0/examples/esxlist.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/event-test.py` & `libvirt-python-9.9.0/examples/event-test.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/guest-vcpus/guest-vcpu-daemon.py` & `libvirt-python-9.9.0/examples/guest-vcpus/guest-vcpu-daemon.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/guest-vcpus/guest-vcpu.py` & `libvirt-python-9.9.0/examples/guest-vcpus/guest-vcpu.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/nodestats.py` & `libvirt-python-9.9.0/examples/nodestats.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/sparsestream.py` & `libvirt-python-9.9.0/examples/sparsestream.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/examples/topology.py` & `libvirt-python-9.9.0/examples/topology.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/generator.py` & `libvirt-python-9.9.0/generator.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-lxc-override-api.xml` & `libvirt-python-9.9.0/libvirt-lxc-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-lxc-override.c` & `libvirt-python-9.9.0/libvirt-lxc-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-override-api.xml` & `libvirt-python-9.9.0/libvirt-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-override-virConnect.py` & `libvirt-python-9.9.0/libvirt-override-virConnect.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-override-virDomain.py` & `libvirt-python-9.9.0/libvirt-override-virDomain.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-override-virDomainCheckpoint.py` & `libvirt-python-9.9.0/libvirt-override-virDomainCheckpoint.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-override-virDomainSnapshot.py` & `libvirt-python-9.9.0/libvirt-override-virDomainSnapshot.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-override-virStream.py` & `libvirt-python-9.9.0/libvirt-override-virStream.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-override.c` & `libvirt-python-9.9.0/libvirt-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-override.py` & `libvirt-python-9.9.0/libvirt-override.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-python.spec` & `libvirt-python-9.9.0/libvirt-python.spec`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     %define supported_platform 1
 %else
     %define supported_platform 0
 %endif
 
 Summary: The libvirt virtualization API python3 binding
 Name: libvirt-python
-Version: 9.8.0
+Version: 9.9.0
 Release: 1%{?dist}
 Source0: https://libvirt.org/sources/python/%{name}-%{version}.tar.gz
 Url: https://libvirt.org
 License: LGPL-2.1-or-later
 BuildRequires: libvirt-devel == %{version}
 BuildRequires: python3-devel
 BuildRequires: python3-pytest
```

### Comparing `libvirt-python-9.8.0/libvirt-python.spec.in` & `libvirt-python-9.9.0/libvirt-python.spec.in`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-qemu-override-api.xml` & `libvirt-python-9.9.0/libvirt-qemu-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-qemu-override.c` & `libvirt-python-9.9.0/libvirt-qemu-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-qemu-override.py` & `libvirt-python-9.9.0/libvirt-qemu-override.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-utils.c` & `libvirt-python-9.9.0/libvirt-utils.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirt-utils.h` & `libvirt-python-9.9.0/libvirt-utils.h`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/libvirtaio.py` & `libvirt-python-9.9.0/libvirtaio.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/setup.cfg` & `libvirt-python-9.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/setup.py` & `libvirt-python-9.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/tests/eventmock.py` & `libvirt-python-9.9.0/tests/eventmock.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/tests/test_aio.py` & `libvirt-python-9.9.0/tests/test_aio.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/tests/test_api_coverage.py` & `libvirt-python-9.9.0/tests/test_api_coverage.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/tests/test_conn.py` & `libvirt-python-9.9.0/tests/test_conn.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/tests/test_domain.py` & `libvirt-python-9.9.0/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/tests/test_domain_checkpoint.py` & `libvirt-python-9.9.0/tests/test_domain_checkpoint.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/tests/test_storage.py` & `libvirt-python-9.9.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/typewrappers.c` & `libvirt-python-9.9.0/typewrappers.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.8.0/typewrappers.h` & `libvirt-python-9.9.0/typewrappers.h`

 * *Files identical despite different names*

