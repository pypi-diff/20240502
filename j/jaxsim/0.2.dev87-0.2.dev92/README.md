# Comparing `tmp/jaxsim-0.2.dev87.tar.gz` & `tmp/jaxsim-0.2.dev92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.2.dev87.tar", last modified: Wed Feb 21 08:04:05 2024, max compression
+gzip compressed data, was "jaxsim-0.2.dev92.tar", last modified: Wed Feb 28 09:34:49 2024, max compression
```

## Comparing `jaxsim-0.2.dev87.tar` & `jaxsim-0.2.dev92.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.657954 jaxsim-0.2.dev87/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.637953 jaxsim-0.2.dev87/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.633953 jaxsim-0.2.dev87/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.641954 jaxsim-0.2.dev87/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.github/workflows/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.github/workflows/read_the_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-02-21 08:04:05.657954 jaxsim-0.2.dev87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.641954 jaxsim-0.2.dev87/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.641954 jaxsim-0.2.dev87/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.641954 jaxsim-0.2.dev87/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/modules/high_level.rst
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/modules/math.rst
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/modules/parsers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/modules/physics.rst
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/modules/simulation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/modules/typing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/docs/modules/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.641954 jaxsim-0.2.dev87/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/examples/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/examples/PD_controller.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/examples/Parallel_computing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.641954 jaxsim-0.2.dev87/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/examples/assets/cartpole.urdf
--rw-r--r--   0 runner    (1001) docker     (127)   241476 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/examples/pixi.lock
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/examples/pixi.toml
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-21 08:04:05.657954 jaxsim-0.2.dev87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.637953 jaxsim-0.2.dev87/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.645954 jaxsim-0.2.dev87/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-21 08:04:05.000000 jaxsim-0.2.dev87/src/jaxsim/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.645954 jaxsim-0.2.dev87/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (127)    57054 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.645954 jaxsim-0.2.dev87/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.645954 jaxsim-0.2.dev87/src/jaxsim/mujoco/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/mujoco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/mujoco/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16047 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/mujoco/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/mujoco/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/mujoco/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.649953 jaxsim-0.2.dev87/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.649953 jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    23610 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.649953 jaxsim-0.2.dev87/src/jaxsim/parsers/rod/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/rod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/rod/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/parsers/rod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.649953 jaxsim-0.2.dev87/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.649953 jaxsim-0.2.dev87/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/aba_motors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/rnea_motors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.653954 jaxsim-0.2.dev87/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.653954 jaxsim-0.2.dev87/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18123 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.653954 jaxsim-0.2.dev87/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.653954 jaxsim-0.2.dev87/src/jaxsim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/utils/jaxsim_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    22616 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/utils/oop.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/utils/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/src/jaxsim/utils/vmappable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.653954 jaxsim-0.2.dev87/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-02-21 08:04:05.000000 jaxsim-0.2.dev87/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-02-21 08:04:05.000000 jaxsim-0.2.dev87/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 08:04:05.000000 jaxsim-0.2.dev87/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 08:04:05.000000 jaxsim-0.2.dev87/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-21 08:04:05.000000 jaxsim-0.2.dev87/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-21 08:04:05.000000 jaxsim-0.2.dev87/src/jaxsim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:04:05.653954 jaxsim-0.2.dev87/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/tests/test_ad_physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/tests/test_eom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/tests/test_forward_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/tests/test_jax_oop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/tests/utils_idyntree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/tests/utils_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-21 08:03:53.000000 jaxsim-0.2.dev87/tests/utils_rng.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.103683 jaxsim-0.2.dev92/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.083683 jaxsim-0.2.dev92/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.079683 jaxsim-0.2.dev92/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.087683 jaxsim-0.2.dev92/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.github/workflows/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.github/workflows/read_the_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-02-28 09:34:49.103683 jaxsim-0.2.dev92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.087683 jaxsim-0.2.dev92/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.087683 jaxsim-0.2.dev92/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.087683 jaxsim-0.2.dev92/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/modules/high_level.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/modules/math.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/modules/parsers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/modules/physics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/modules/simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/modules/typing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/docs/modules/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.087683 jaxsim-0.2.dev92/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/examples/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/examples/PD_controller.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/examples/Parallel_computing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.087683 jaxsim-0.2.dev92/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/examples/assets/cartpole.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)   241476 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/examples/pixi.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/examples/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-02-28 09:34:49.103683 jaxsim-0.2.dev92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.079683 jaxsim-0.2.dev92/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.091683 jaxsim-0.2.dev92/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-28 09:34:49.000000 jaxsim-0.2.dev92/src/jaxsim/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.091683 jaxsim-0.2.dev92/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57054 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.091683 jaxsim-0.2.dev92/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.095683 jaxsim-0.2.dev92/src/jaxsim/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/mujoco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/mujoco/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16047 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/mujoco/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/mujoco/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/mujoco/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.095683 jaxsim-0.2.dev92/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.095683 jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23610 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.095683 jaxsim-0.2.dev92/src/jaxsim/parsers/rod/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/rod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/rod/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/parsers/rod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.095683 jaxsim-0.2.dev92/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.095683 jaxsim-0.2.dev92/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/aba_motors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/rnea_motors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.099683 jaxsim-0.2.dev92/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.099683 jaxsim-0.2.dev92/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18123 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.099683 jaxsim-0.2.dev92/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.099683 jaxsim-0.2.dev92/src/jaxsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/utils/jaxsim_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22616 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/utils/oop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/utils/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/src/jaxsim/utils/vmappable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.103683 jaxsim-0.2.dev92/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-02-28 09:34:49.000000 jaxsim-0.2.dev92/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-02-28 09:34:49.000000 jaxsim-0.2.dev92/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 09:34:49.000000 jaxsim-0.2.dev92/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 09:34:48.000000 jaxsim-0.2.dev92/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-28 09:34:49.000000 jaxsim-0.2.dev92/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-28 09:34:49.000000 jaxsim-0.2.dev92/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:49.099683 jaxsim-0.2.dev92/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/tests/test_ad_physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/tests/test_eom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/tests/test_forward_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/tests/test_jax_oop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/tests/utils_idyntree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/tests/utils_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-28 09:34:37.000000 jaxsim-0.2.dev92/tests/utils_rng.py
```

### Comparing `jaxsim-0.2.dev87/.devcontainer/Dockerfile` & `jaxsim-0.2.dev92/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/.devcontainer/devcontainer.json` & `jaxsim-0.2.dev92/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/.github/workflows/ci_cd.yml` & `jaxsim-0.2.dev92/.github/workflows/ci_cd.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 name: Python CI/CD
 
 on:
+  workflow_dispatch:
   push:
   pull_request:
   release:
     types:
       - published
+  schedule:
+  # * is a special character in YAML so you have to quote this string
+  # Execute a "nightly" build at 2 AM UTC
+  - cron:  '0 2 * * *'
+
 
 jobs:
 
   package:
     name: Package the project
     runs-on: ubuntu-22.04
 
@@ -79,46 +85,33 @@
         run: pip install "$(find dist/ -type f -name '*.whl')[all]"
 
       - name: Install wheel (macos|windows)
         if: contains(matrix.os, 'macos') || contains(matrix.os, 'windows')
         shell: bash
         run: pip install "$(find dist/ -type f -name '*.whl')"
 
+      - name: Document installed pip packages
+        shell: bash
+        run: pip list --verbose
+      
       - name: Import the package
         run: python -c "import jaxsim"
 
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - uses: dorny/paths-filter@v3
-        id: changes
-        with:
-          filters: |
-            src: &src
-              - 'src/**'
-            tests: &tests
-              - 'tests/**'
-            src_and_tests:
-              - *src
-              - *tests
 
       - name: Install Gazebo Classic
-        if: |
-          contains(matrix.os, 'ubuntu') &&
-          (github.event_name != 'pull_request' ||
-           steps.changes.outputs.src_and_tests == 'true')
+        if: contains(matrix.os, 'ubuntu')
         run: |
           sudo apt-get update
           sudo apt-get install gazebo
 
       - name: Run the Python tests
-        if: |
-          contains(matrix.os, 'ubuntu') &&
-          (github.event_name != 'pull_request' ||
-           steps.changes.outputs.src_and_tests == 'true')
+        if: contains(matrix.os, 'ubuntu')
         run: pytest
         env:
           JAX_PLATFORM_NAME: cpu
 
   publish:
     name: Publish to PyPI
     needs: test
```

### Comparing `jaxsim-0.2.dev87/.github/workflows/style.yml` & `jaxsim-0.2.dev92/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/.gitignore` & `jaxsim-0.2.dev92/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/CONTRIBUTING.md` & `jaxsim-0.2.dev92/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/LICENSE` & `jaxsim-0.2.dev92/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/PKG-INFO` & `jaxsim-0.2.dev92/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.2.dev87
+Version: 0.2.dev92
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
@@ -27,16 +27,16 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
-Requires-Dist: jax>=0.4.13
-Requires-Dist: jaxlib
+Requires-Dist: jax<0.4.25,>=0.4.13
+Requires-Dist: jaxlib<0.4.25,>=0.4.13
 Requires-Dist: jaxlie>=1.3.0
 Requires-Dist: jax_dataclasses>=1.4.0
 Requires-Dist: pptree
 Requires-Dist: rod
 Provides-Extra: style
 Requires-Dist: black[jupyter]; extra == "style"
 Requires-Dist: isort; extra == "style"
```

### Comparing `jaxsim-0.2.dev87/README.md` & `jaxsim-0.2.dev92/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/docs/conf.py` & `jaxsim-0.2.dev92/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/docs/guide/install.rst` & `jaxsim-0.2.dev92/docs/guide/install.rst`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/docs/index.rst` & `jaxsim-0.2.dev92/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/docs/make.bat` & `jaxsim-0.2.dev92/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/docs/modules/math.rst` & `jaxsim-0.2.dev92/docs/modules/math.rst`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/docs/modules/physics.rst` & `jaxsim-0.2.dev92/docs/modules/physics.rst`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/docs/modules/simulation.rst` & `jaxsim-0.2.dev92/docs/modules/simulation.rst`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/environment.yml` & `jaxsim-0.2.dev92/environment.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/examples/PD_controller.ipynb` & `jaxsim-0.2.dev92/examples/PD_controller.ipynb`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/examples/Parallel_computing.ipynb` & `jaxsim-0.2.dev92/examples/Parallel_computing.ipynb`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/examples/README.md` & `jaxsim-0.2.dev92/examples/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/examples/assets/cartpole.urdf` & `jaxsim-0.2.dev92/examples/assets/cartpole.urdf`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/examples/pixi.lock` & `jaxsim-0.2.dev92/examples/pixi.lock`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/examples/pixi.toml` & `jaxsim-0.2.dev92/examples/pixi.toml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/setup.cfg` & `jaxsim-0.2.dev92/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 zip_safe = False
 packages = find:
 package_dir = 
 	=src
 python_requires = >=3.11
 install_requires = 
 	coloredlogs
-	jax >= 0.4.13
-	jaxlib
+	jax >= 0.4.13,< 0.4.25
+	jaxlib >= 0.4.13,< 0.4.25
 	jaxlie >= 1.3.0
 	jax_dataclasses >= 1.4.0
 	pptree
 	rod
 
 [options.packages.find]
 where = src
```

### Comparing `jaxsim-0.2.dev87/src/jaxsim/__init__.py` & `jaxsim-0.2.dev92/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/high_level/joint.py` & `jaxsim-0.2.dev92/src/jaxsim/high_level/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/high_level/link.py` & `jaxsim-0.2.dev92/src/jaxsim/high_level/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/high_level/model.py` & `jaxsim-0.2.dev92/src/jaxsim/high_level/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/logging.py` & `jaxsim-0.2.dev92/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/adjoint.py` & `jaxsim-0.2.dev92/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/conv.py` & `jaxsim-0.2.dev92/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/cross.py` & `jaxsim-0.2.dev92/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/inertia.py` & `jaxsim-0.2.dev92/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/joint.py` & `jaxsim-0.2.dev92/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/plucker.py` & `jaxsim-0.2.dev92/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/quaternion.py` & `jaxsim-0.2.dev92/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/rotation.py` & `jaxsim-0.2.dev92/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/math/skew.py` & `jaxsim-0.2.dev92/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/mujoco/__main__.py` & `jaxsim-0.2.dev92/src/jaxsim/mujoco/__main__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/mujoco/loaders.py` & `jaxsim-0.2.dev92/src/jaxsim/mujoco/loaders.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/mujoco/model.py` & `jaxsim-0.2.dev92/src/jaxsim/mujoco/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/mujoco/visualizer.py` & `jaxsim-0.2.dev92/src/jaxsim/mujoco/visualizer.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.2.dev92/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.2.dev92/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/parsers/rod/parser.py` & `jaxsim-0.2.dev92/src/jaxsim/parsers/rod/parser.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/parsers/rod/utils.py` & `jaxsim-0.2.dev92/src/jaxsim/parsers/rod/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/aba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/aba_motors.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/aba_motors.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/rnea_motors.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/rnea_motors.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/terrain.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/model/physics_model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.2.dev92/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/simulation/integrators.py` & `jaxsim-0.2.dev92/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/simulation/ode.py` & `jaxsim-0.2.dev92/src/jaxsim/simulation/ode.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.2.dev92/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.2.dev92/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/simulation/simulator.py` & `jaxsim-0.2.dev92/src/jaxsim/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.2.dev92/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/typing.py` & `jaxsim-0.2.dev92/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/utils/jaxsim_dataclass.py` & `jaxsim-0.2.dev92/src/jaxsim/utils/jaxsim_dataclass.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/utils/oop.py` & `jaxsim-0.2.dev92/src/jaxsim/utils/oop.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/utils/tracing.py` & `jaxsim-0.2.dev92/src/jaxsim/utils/tracing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim/utils/vmappable.py` & `jaxsim-0.2.dev92/src/jaxsim/utils/vmappable.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.2.dev92/src/jaxsim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.2.dev87
+Version: 0.2.dev92
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
@@ -27,16 +27,16 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
-Requires-Dist: jax>=0.4.13
-Requires-Dist: jaxlib
+Requires-Dist: jax<0.4.25,>=0.4.13
+Requires-Dist: jaxlib<0.4.25,>=0.4.13
 Requires-Dist: jaxlie>=1.3.0
 Requires-Dist: jax_dataclasses>=1.4.0
 Requires-Dist: pptree
 Requires-Dist: rod
 Provides-Extra: style
 Requires-Dist: black[jupyter]; extra == "style"
 Requires-Dist: isort; extra == "style"
```

### Comparing `jaxsim-0.2.dev87/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.2.dev92/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/tests/test_ad_physics.py` & `jaxsim-0.2.dev92/tests/test_ad_physics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/tests/test_eom.py` & `jaxsim-0.2.dev92/tests/test_eom.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/tests/test_forward_dynamics.py` & `jaxsim-0.2.dev92/tests/test_forward_dynamics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/tests/test_jax_oop.py` & `jaxsim-0.2.dev92/tests/test_jax_oop.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/tests/utils_idyntree.py` & `jaxsim-0.2.dev92/tests/utils_idyntree.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/tests/utils_models.py` & `jaxsim-0.2.dev92/tests/utils_models.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.2.dev87/tests/utils_rng.py` & `jaxsim-0.2.dev92/tests/utils_rng.py`

 * *Files identical despite different names*

