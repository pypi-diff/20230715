# Comparing `tmp/panda_python-0.0.0.tar.gz` & `tmp/panda-python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "panda-python-0.5.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `panda_python-0.0.0.tar` & `panda-python-0.5.0.tar`

### file list

```diff
@@ -1,2 +1,71 @@
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 panda_python-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 panda_python-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2135 2022-11-09 12:37:21.000000 panda-python-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 panda-python-0.5.0/.gitignore
+-rw-r--r--   0        0        0    19334 2022-11-09 12:37:21.000000 panda-python-0.5.0/.pylintrc
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 panda-python-0.5.0/.vscode/c_cpp_properties.json
+-rwxr-xr-x   0        0        0      481 2022-11-09 12:37:21.000000 panda-python-0.5.0/.vscode/generate_docs_api.sh
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 panda-python-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 panda-python-0.5.0/.vscode/tasks.json
+-rw-r--r--   0        0        0     1636 2022-11-09 12:37:21.000000 panda-python-0.5.0/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 panda-python-0.5.0/LICENSE
+-rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 panda-python-0.5.0/README.md
+-rwxr-xr-x   0        0        0     1214 2022-11-09 12:37:21.000000 panda-python-0.5.0/bin/before_install.sh
+-rwxr-xr-x   0        0        0     1251 2022-11-09 12:37:21.000000 panda-python-0.5.0/bin/build_all.sh
+-rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.cli.rst
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.constants.rst
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.controllers.rst
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.libfranka.rst
+-rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.motion.rst
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.rst
+-rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/cartesian_impedance.py
+-rw-r--r--   0        0        0     2531 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/communication_test.py
+-rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/mmc.py
+-rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/notebooks/benchmark.ipynb
+-rw-r--r--   0        0        0    31180 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/notebooks/motion.ipynb
+-rw-r--r--   0        0        0    38752 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/notebooks/paper.ipynb
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/constants.h
+-rw-r--r--   0        0        0     1136 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/applied_force.h
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/applied_torque.h
+-rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/cartesian_impedance.h
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/controller.h
+-rw-r--r--   0        0        0     1683 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/force.h
+-rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/integrated_velocity.h
+-rw-r--r--   0        0        0     1337 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/joint_limits/virtual_wall.h
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/joint_limits/virtual_wall_controller.h
+-rw-r--r--   0        0        0     1335 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/joint_position.h
+-rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/trajectory.h
+-rw-r--r--   0        0        0    16534 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/kinematics/fk.h
+-rw-r--r--   0        0        0    14073 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/kinematics/ik.h
+-rw-r--r--   0        0        0     3949 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/motion/generators.h
+-rw-r--r--   0        0        0     3473 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/motion/time_optimal/path.h
+-rw-r--r--   0        0        0     5278 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/motion/time_optimal/trajectory.h
+-rw-r--r--   0        0        0     5819 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/panda.h
+-rw-r--r--   0        0        0     3864 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/utils.h
+-rw-r--r--   0        0        0    51837 2022-11-09 12:37:21.000000 panda-python-0.5.0/logo.jpg
+-rw-r--r--   0        0        0     1673 2022-11-09 12:37:21.000000 panda-python-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    21367 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/_core.cpp
+-rw-r--r--   0        0        0     2284 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/applied_force.cpp
+-rw-r--r--   0        0        0     2080 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/applied_torque.cpp
+-rw-r--r--   0        0        0     6444 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/cartesian_impedance.cpp
+-rw-r--r--   0        0        0     4628 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/force.cpp
+-rw-r--r--   0        0        0     2287 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/integrated_velocity.cpp
+-rw-r--r--   0        0        0     5337 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/joint_limits/virtual_wall.cpp
+-rw-r--r--   0        0        0     3069 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/joint_position.cpp
+-rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/trajectory.cpp
+-rw-r--r--   0        0        0    25036 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/libfranka.cpp
+-rw-r--r--   0        0        0     6824 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/motion/generators.cpp
+-rw-r--r--   0        0        0     9987 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/motion/time_optimal/path.cpp
+-rw-r--r--   0        0        0    23965 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/motion/time_optimal/trajectory.cpp
+-rw-r--r--   0        0        0    14329 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda.cpp
+-rw-r--r--   0        0        0    10245 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/__init__.py
+-rw-r--r--   0        0        0     5211 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/__init__.pyi
+-rw-r--r--   0        0        0    17071 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/_core/__init__.pyi
+-rw-r--r--   0        0        0     2611 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/cli.py
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/constants.py
+-rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/controllers.py
+-rw-r--r--   0        0        0    34215 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/libfranka/__init__.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/motion.py
+-rw-r--r--   0        0        0    14846 2022-11-09 12:37:21.000000 panda-python-0.5.0/PKG-INFO
```

