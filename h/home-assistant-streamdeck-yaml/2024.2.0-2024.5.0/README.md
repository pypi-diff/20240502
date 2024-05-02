# Comparing `tmp/home_assistant_streamdeck_yaml-2024.2.0.tar.gz` & `tmp/home_assistant_streamdeck_yaml-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home_assistant_streamdeck_yaml-2024.2.0.tar", last modified: Sun Feb  4 22:05:21 2024, max compression
+gzip compressed data, was "home_assistant_streamdeck_yaml-2024.5.0.tar", last modified: Thu May  2 19:21:55 2024, max compression
```

## Comparing `home_assistant_streamdeck_yaml-2024.2.0.tar` & `home_assistant_streamdeck_yaml-2024.5.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 22:05:21.704112 home_assistant_streamdeck_yaml-2024.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 22:05:21.696112 home_assistant_streamdeck_yaml-2024.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.github/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 22:05:21.700112 home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/toc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/update-readme.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/Dockerfile.latest
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/Dockerfile.locked
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    45519 2024-02-04 22:05:21.704112 home_assistant_streamdeck_yaml-2024.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    44407 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 22:05:21.700112 home_assistant_streamdeck_yaml-2024.2.0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   158604 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/assets/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    13302 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/assets/fireplace.png
--rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/assets/hogwarts.png
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/assets/netflix.png
--rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/assets/night_sky.png
--rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/assets/space-heater.png
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/assets/spotify.png
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/assets/xbox.png
--rw-r--r--   0 runner    (1001) docker     (127)   127890 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/conda-lock.yml
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 22:05:21.704112 home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45519 2024-02-04 22:05:21.000000 home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-04 22:05:21.000000 home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 22:05:21.000000 home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-04 22:05:21.000000 home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-04 22:05:21.000000 home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-04 22:05:21.000000 home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    64770 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 22:05:21.704112 home_assistant_streamdeck_yaml-2024.2.0/includes/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/anon_all_lights.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/anon_automatic_lights.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/anon_bas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/anon_bedroom_lights.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/anon_living_room_lights.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/anon_sensors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/anon_timers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/home.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/media.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/spotify.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/includes/testing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 22:05:21.704112 home_assistant_streamdeck_yaml-2024.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 22:05:21.704112 home_assistant_streamdeck_yaml-2024.2.0/systemd/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/systemd/home-assistant-streamdeck-yaml.service
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/systemd/restart
--rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/systemd/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/systemd/status
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/systemd/update
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 22:05:21.704112 home_assistant_streamdeck_yaml-2024.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/tests/state.json
--rw-r--r--   0 runner    (1001) docker     (127)    35462 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    39246 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-02-04 22:05:03.000000 home_assistant_streamdeck_yaml-2024.2.0/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:21:55.769159 home_assistant_streamdeck_yaml-2024.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:21:55.761159 home_assistant_streamdeck_yaml-2024.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.github/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:21:55.761159 home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/toc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/update-readme.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/Dockerfile.latest
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/Dockerfile.locked
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    45519 2024-05-02 19:21:55.769159 home_assistant_streamdeck_yaml-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    44407 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:21:55.765159 home_assistant_streamdeck_yaml-2024.5.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   158604 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/assets/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    13302 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/assets/fireplace.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/assets/hogwarts.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/assets/netflix.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/assets/night_sky.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/assets/space-heater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/assets/spotify.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/assets/xbox.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127890 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/conda-lock.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:21:55.769159 home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45519 2024-05-02 19:21:55.000000 home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-02 19:21:55.000000 home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:21:55.000000 home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 19:21:55.000000 home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 19:21:55.000000 home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 19:21:55.000000 home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65461 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:21:55.765159 home_assistant_streamdeck_yaml-2024.5.0/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/anon_all_lights.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/anon_automatic_lights.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/anon_bas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/anon_bedroom_lights.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/anon_living_room_lights.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/anon_sensors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/anon_timers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/home.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/media.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/spotify.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/includes/testing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:21:55.769159 home_assistant_streamdeck_yaml-2024.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:21:55.765159 home_assistant_streamdeck_yaml-2024.5.0/systemd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/systemd/home-assistant-streamdeck-yaml.service
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/systemd/restart
+-rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/systemd/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/systemd/status
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/systemd/update
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:21:55.769159 home_assistant_streamdeck_yaml-2024.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/tests/state.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35463 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39246 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-02 19:21:37.000000 home_assistant_streamdeck_yaml-2024.5.0/tests/test_yaml.py
```

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/.github/release.py` & `home_assistant_streamdeck_yaml-2024.5.0/.github/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create a new release tag with CalVer format."""
+
 import datetime
 import operator
 import os
 from pathlib import Path
 
 import git
 from packaging import version
```

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/automerge.yml` & `home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/automerge.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/docker-build.yml` & `home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/pytest.yml` & `home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/release.yml` & `home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/.github/workflows/update-readme.yml` & `home_assistant_streamdeck_yaml-2024.5.0/.github/workflows/update-readme.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/.gitignore` & `home_assistant_streamdeck_yaml-2024.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/.pre-commit-config.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: mixed-line-ending
   - repo: "https://github.com/ambv/black"
-    rev: 23.11.0
+    rev: 24.3.0
     hooks:
       - id: black-jupyter
         language_version: python3
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.1.6"
+    rev: "v0.3.5"
     hooks:
       - id: ruff
         args: ["--fix"]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.7.1"
+    rev: "v1.9.0"
     hooks:
       - id: mypy
         additional_dependencies: ["types-PyYAML", "types-requests", "types-setuptools"]
```

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/Dockerfile.latest` & `home_assistant_streamdeck_yaml-2024.5.0/Dockerfile.latest`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/Dockerfile.locked` & `home_assistant_streamdeck_yaml-2024.5.0/Dockerfile.locked`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/LICENSE` & `home_assistant_streamdeck_yaml-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/PKG-INFO` & `home_assistant_streamdeck_yaml-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home_assistant_streamdeck_yaml
-Version: 2024.2.0
+Version: 2024.5.0
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cairosvg
```

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/README.md` & `home_assistant_streamdeck_yaml-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/assets/Roboto-Regular.ttf` & `home_assistant_streamdeck_yaml-2024.5.0/assets/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/assets/fireplace.png` & `home_assistant_streamdeck_yaml-2024.5.0/assets/fireplace.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/assets/hogwarts.png` & `home_assistant_streamdeck_yaml-2024.5.0/assets/hogwarts.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/assets/netflix.png` & `home_assistant_streamdeck_yaml-2024.5.0/assets/netflix.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/assets/night_sky.png` & `home_assistant_streamdeck_yaml-2024.5.0/assets/night_sky.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/assets/space-heater.png` & `home_assistant_streamdeck_yaml-2024.5.0/assets/space-heater.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/assets/spotify.png` & `home_assistant_streamdeck_yaml-2024.5.0/assets/spotify.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/assets/xbox.png` & `home_assistant_streamdeck_yaml-2024.5.0/assets/xbox.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/conda-lock.yml` & `home_assistant_streamdeck_yaml-2024.5.0/conda-lock.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/configuration.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/configuration.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/docker-compose.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO` & `home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home_assistant_streamdeck_yaml
-Version: 2024.2.0
+Version: 2024.5.0
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cairosvg
```

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt` & `home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/home_assistant_streamdeck_yaml.py` & `home_assistant_streamdeck_yaml-2024.5.0/home_assistant_streamdeck_yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 """Home Assistant Stream Deck integration."""
+
 from __future__ import annotations
 
 import asyncio
 import colorsys
 import functools as ft
 import hashlib
 import io
@@ -162,23 +163,26 @@
         allow_template=True,
         description="The delay (in seconds) before the `service` is called."
         " This is useful if you want to wait before calling the `service`."
         " Counts down from the time the button is pressed."
         " If while counting the button is pressed again, the timer is cancelled."
         " Should be a float or template string that evaluates to a float.",
     )
-    special_type: Literal[
-        "next-page",
-        "previous-page",
-        "empty",
-        "go-to-page",
-        "turn-off",
-        "light-control",
-        "reload",
-    ] | None = Field(
+    special_type: (
+        Literal[
+            "next-page",
+            "previous-page",
+            "empty",
+            "go-to-page",
+            "turn-off",
+            "light-control",
+            "reload",
+        ]
+        | None
+    ) = Field(
         default=None,
         allow_template=False,
         description="Special type of button."
         " If no specified, the button is a normal button."
         " If `next-page`, the button will go to the next page."
         " If `previous-page`, the button will go to the previous page."
         " If `turn-off`, the button will turn off the SteamDeck until any button is pressed."
@@ -702,14 +706,15 @@
 
     Parameters
     ----------
     delay
         The delay in seconds after which the callback will be called.
     callback
         The function or coroutine to be called after the delay.
+
     """
 
     def __init__(
         self,
         delay: float,
         callback: Callable[[], None | Coroutine] | None = None,
     ) -> None:
@@ -900,14 +905,15 @@
     list[str]
         A list of `n_colors` hex colors, represented as strings.
 
     Examples
     --------
     >>> _generate_uniform_hex_colors(3)
     ['#0000ff', '#00ff00', '#ff0000']
+
     """
 
     def generate_hues(n_hues: int) -> list[float]:
         """Generate `n_hues` hues that are uniformly spaced around the color wheel."""
         return _linspace(0, 1, n_hues)
 
     def generate_saturations(n_saturations: int) -> list[float]:
@@ -1511,24 +1517,41 @@
     # This resets all buttons except the turn-off button that
     # was just pressed, however, this doesn't matter with the
     # 0 brightness. Unless no button was pressed.
     deck.reset()
     deck.set_brightness(0)
 
 
+async def _sync_input_boolean(
+    state_entity_id: str | None,
+    websocket: websockets.WebSocketClientProtocol,
+    state: Literal["on", "off"],
+) -> None:
+    """Sync the input boolean state with the Stream Deck."""
+    if (state_entity_id is not None) and (
+        state_entity_id.split(".")[0] == "input_boolean"
+    ):
+        await call_service(
+            websocket,
+            f"input_boolean.turn_{state}",
+            {},
+            {"entity_id": state_entity_id},
+        )
+
+
 async def _handle_key_press(
     websocket: websockets.WebSocketClientProtocol,
     complete_state: StateDict,
     config: Config,
     button: Button,
     deck: StreamDeck,
 ) -> None:
     if not config._is_on:
         turn_on(config, deck, complete_state)
-        return
+        await _sync_input_boolean(config.state_entity_id, websocket, "on")
 
     def update_all() -> None:
         deck.reset()
         update_all_key_images(deck, config, complete_state)
 
     if button.special_type == "next-page":
         config.next_page()
@@ -1539,14 +1562,15 @@
     elif button.special_type == "go-to-page":
         assert isinstance(button.special_type_data, (str, int))
         config.to_page(button.special_type_data)  # type: ignore[arg-type]
         update_all()
         return  # to skip the _detached_page reset below
     elif button.special_type == "turn-off":
         turn_off(config, deck)
+        await _sync_input_boolean(config.state_entity_id, websocket, "off")
     elif button.special_type == "light-control":
         assert isinstance(button.special_type_data, dict)
         page = _light_page(
             entity_id=button.entity_id,
             n_colors=10,
             colormap=button.special_type_data.get("colormap", None),
             colors=button.special_type_data.get("colors", None),
@@ -1636,14 +1660,15 @@
     hash_len
         The length of the hash to include in the filename, by default 8.
 
     Returns
     -------
     Path
         The filename with the hash included, if specified.
+
     """
     domain, path = re.findall(r"(?<=://)([a-zA-Z\.]+).*?(/.*)", url)[0]
     h = hashlib.sha256(f"{domain}{path}".encode()).hexdigest()[:hash_len]
     extension = Path(path).suffix
     filename = f"{domain.replace('.', '_')}-{h}{extension}"
     return ASSETS_PATH / Path(filename)
 
@@ -1659,14 +1684,15 @@
         A HEX color in the format "#RRGGBB".
     scale
         A scaling factor between 0 and 1.
 
     Returns
     -------
     A scaled HEX color in the format "#RRGGBB".
+
     """
     scale = max(0, min(1, scale))
     # Convert HEX color to RGB values
     r = int(hex_color[1:3], 16)
     g = int(hex_color[3:5], 16)
     b = int(hex_color[5:7], 16)
 
@@ -1711,14 +1737,15 @@
         The opacity of the icon. 0 is black, 1 is full color.
     margin
         The margin to add around the icon.
     filename_png
         The name of the file to save the PNG content to.
     size
         The size of the resulting PNG image.
+
     """
     import cairosvg  # importing here because it requires a non Python dep
 
     with filename_svg.open() as f:
         svg_content = f.read()
 
     fill_color = _scale_hex_color(color, opacity)
```

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/anon_all_lights.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/anon_all_lights.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/anon_automatic_lights.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/anon_automatic_lights.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/anon_bas.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/anon_bas.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/anon_living_room_lights.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/anon_living_room_lights.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/anon_sensors.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/anon_sensors.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/anon_timers.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/anon_timers.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/home.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/home.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/media.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/media.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/spotify.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/spotify.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/includes/testing.yaml` & `home_assistant_streamdeck_yaml-2024.5.0/includes/testing.yaml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/pyproject.toml` & `home_assistant_streamdeck_yaml-2024.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/systemd/home-assistant-streamdeck-yaml.service` & `home_assistant_streamdeck_yaml-2024.5.0/systemd/home-assistant-streamdeck-yaml.service`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/tests/state.json` & `home_assistant_streamdeck_yaml-2024.5.0/tests/state.json`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/tests/test_app.py` & `home_assistant_streamdeck_yaml-2024.5.0/tests/test_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test Home Assistant Stream Deck YAML."""
+
 from __future__ import annotations
 
 import asyncio
 import json
 import sys
 import textwrap
 from pathlib import Path
```

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/tests/test_examples.py` & `home_assistant_streamdeck_yaml-2024.5.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2024.2.0/tests/test_yaml.py` & `home_assistant_streamdeck_yaml-2024.5.0/tests/test_yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the yaml loading."""
+
 from io import StringIO
 from pathlib import Path
 
 import pytest
 import yaml
 
 from home_assistant_streamdeck_yaml import safe_load_yaml
```

