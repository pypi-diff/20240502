# Comparing `tmp/tlslib-0.tar.gz` & `tmp/tlslib-0.0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlslib-0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tlslib-0.0.2rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tlslib-0.tar` & `tlslib-0.0.2rc0.tar`

### file list

```diff
@@ -1,3 +1,9 @@
--rw-r--r--   0        0        0      232 2024-04-23 16:25:56.679218 tlslib-0/pyproject.toml
--rw-r--r--   0        0        0       74 2024-04-23 16:26:49.463013 tlslib-0/tlslib.py
--rw-r--r--   0        0        0      147 1970-01-01 00:00:00.000000 tlslib-0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-05-02 15:54:44.029505 tlslib-0.0.2rc0/LICENSE
+-rw-r--r--   0        0        0      593 2024-05-02 15:54:44.029505 tlslib-0.0.2rc0/README.md
+-rw-r--r--   0        0        0     1989 2024-05-02 15:54:44.029505 tlslib-0.0.2rc0/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/__init__.py
+-rw-r--r--   0        0        0     7176 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/insecure/__init__.py
+-rw-r--r--   0        0        0     6146 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/insecure/stdlib_insecure.py
+-rw-r--r--   0        0        0    36106 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/stdlib.py
+-rw-r--r--   0        0        0    32460 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/tlslib.py
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 tlslib-0.0.2rc0/PKG-INFO
```

