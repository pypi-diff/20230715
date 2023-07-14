# Comparing `tmp/gymnasium-0.28.1.tar.gz` & `tmp/gymnasium-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium-0.28.1.tar", last modified: Sat Mar 25 12:01:02 2023, max compression
+gzip compressed data, was "gymnasium-0.29.0.tar", last modified: Fri Jul 14 22:47:35 2023, max compression
```

## Comparing `gymnasium-0.28.1.tar` & `gymnasium-0.29.0.tar`

### file list

```diff
@@ -1,280 +1,292 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.921148 gymnasium-0.28.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-25 12:00:48.000000 gymnasium-0.28.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-03-25 12:01:02.921148 gymnasium-0.28.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-03-25 12:00:48.000000 gymnasium-0.28.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.849148 gymnasium-0.28.1/gymnasium/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25983 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.853148 gymnasium-0.28.1/gymnasium/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.853148 gymnasium-0.28.1/gymnasium/envs/box2d/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/box2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31316 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/box2d/bipedal_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/box2d/car_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29145 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/box2d/car_racing.py
--rw-r--r--   0 runner    (1001) docker     (123)    32769 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/box2d/lunar_lander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.857148 gymnasium-0.28.1/gymnasium/envs/classic_control/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/classic_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/classic_control/acrobot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.857148 gymnasium-0.28.1/gymnasium/envs/classic_control/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/classic_control/assets/clockwise.png
--rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/classic_control/cartpole.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/classic_control/continuous_mountain_car.py
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/classic_control/mountain_car.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/classic_control/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/classic_control/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.865148 gymnasium-0.28.1/gymnasium/envs/mujoco/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/ant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/ant_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    20964 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/ant_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.869148 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/ant.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/half_cheetah.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/hopper.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/humanoid.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/humanoidstandup.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/inverted_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/point.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/pusher.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/reacher.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/swimmer.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/assets/walker2d.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/half_cheetah.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/half_cheetah_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/half_cheetah_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/hopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/hopper_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/hopper_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/humanoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/humanoid_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    27871 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/humanoid_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/humanoidstandup.py
--rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/humanoidstandup_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/inverted_double_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/inverted_double_pendulum_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/inverted_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/inverted_pendulum_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/mujoco_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25367 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/mujoco_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/pusher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/pusher_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/reacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/reacher_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/swimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/swimmer_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/swimmer_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/walker2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/walker2d_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/mujoco/walker2d_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.869148 gymnasium-0.28.1/gymnasium/envs/phys2d/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/phys2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/phys2d/cartpole.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/phys2d/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)    42757 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.869148 gymnasium-0.28.1/gymnasium/envs/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17236 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/tabular/blackjack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.873148 gymnasium-0.28.1/gymnasium/envs/toy_text/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/blackjack.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/cliffwalking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.873148 gymnasium-0.28.1/gymnasium/envs/toy_text/font/
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/font/Minecraft.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/frozen_lake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.897148 gymnasium-0.28.1/gymnasium/envs/toy_text/img/
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/C2.png
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/C3.png
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/C4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/C5.png
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/C6.png
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/C7.png
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/C8.png
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/C9.png
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/CA.png
--rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/CJ.png
--rw-r--r--   0 runner    (1001) docker     (123)    19498 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/CK.png
--rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/CQ.png
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/CT.png
--rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/Card.png
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/D2.png
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/D3.png
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/D4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/D5.png
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/D6.png
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/D7.png
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/D8.png
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/D9.png
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/DA.png
--rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/DJ.png
--rw-r--r--   0 runner    (1001) docker     (123)    19118 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/DK.png
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/DQ.png
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/DT.png
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/H2.png
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/H3.png
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/H4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/H5.png
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/H6.png
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/H7.png
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/H8.png
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/H9.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/HA.png
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/HJ.png
--rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/HK.png
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/HQ.png
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/HT.png
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/S2.png
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/S3.png
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/S4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/S5.png
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/S6.png
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/S7.png
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/S8.png
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/S9.png
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/SA.png
--rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/SJ.png
--rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/SK.png
--rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/SQ.png
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/ST.png
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/cab_front.png
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/cab_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/cab_rear.png
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/cab_right.png
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/cookie.png
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/cracked_hole.png
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/elf_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/elf_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/elf_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/elf_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/goal.png
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_horiz.png
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_left.png
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_right.png
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_top.png
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/hole.png
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/hotel.png
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/ice.png
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_bg1.png
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_bg2.png
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_cliff.png
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_near-cliff1.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_near-cliff2.png
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/passenger.png
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/stool.png
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/img/taxi_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/taxi.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/envs/toy_text/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.897148 gymnasium-0.28.1/gymnasium/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/functional_jax_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.897148 gymnasium-0.28.1/gymnasium/experimental/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26849 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/vector/async_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/vector/sync_vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.897148 gymnasium-0.28.1/gymnasium/experimental/vector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/vector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/vector/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/vector/utils/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/vector/utils/space_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/vector/vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.901148 gymnasium-0.28.1/gymnasium/experimental/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/atari_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/jax_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/jax_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/lambda_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    25038 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/lambda_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/lambda_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/numpy_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/stateful_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/stateful_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.901148 gymnasium-0.28.1/gymnasium/experimental/wrappers/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/vector/record_episode_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/experimental/wrappers/vector/vector_list_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.905148 gymnasium-0.28.1/gymnasium/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/multi_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/multi_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    18860 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/spaces/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.909148 gymnasium-0.28.1/gymnasium/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/ezpickle.py
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/passive_env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/play.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/record_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/save_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/seeding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/utils/step_api_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.909148 gymnasium-0.28.1/gymnasium/vector/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/async_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/sync_vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.909148 gymnasium-0.28.1/gymnasium/vector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/utils/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/utils/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/vector/vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.917148 gymnasium-0.28.1/gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/atari_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/autoreset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/clip_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/filter_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/flatten_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/gray_scale_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/human_rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.921148 gymnasium-0.28.1/gymnasium/wrappers/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/monitoring/video_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/order_enforcing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/pixel_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/record_episode_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/record_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/render_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/rescale_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/resize_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/step_api_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/time_aware_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/transform_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/transform_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-25 12:00:49.000000 gymnasium-0.28.1/gymnasium/wrappers/vector_list_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.849148 gymnasium-0.28.1/gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-03-25 12:01:02.000000 gymnasium-0.28.1/gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-03-25 12:01:02.000000 gymnasium-0.28.1/gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 12:01:02.000000 gymnasium-0.28.1/gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-25 12:01:02.000000 gymnasium-0.28.1/gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-25 12:01:02.000000 gymnasium-0.28.1/gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-25 12:00:49.000000 gymnasium-0.28.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 12:01:02.921148 gymnasium-0.28.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-25 12:00:49.000000 gymnasium-0.28.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:01:02.921148 gymnasium-0.28.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-03-25 12:00:49.000000 gymnasium-0.28.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-25 12:00:49.000000 gymnasium-0.28.1/tests/testing_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.326094 gymnasium-0.29.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-14 22:47:24.000000 gymnasium-0.29.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-14 22:47:35.326094 gymnasium-0.29.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-07-14 22:47:24.000000 gymnasium-0.29.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.298094 gymnasium-0.29.0/gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27533 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.298094 gymnasium-0.29.0/gymnasium/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.298094 gymnasium-0.29.0/gymnasium/envs/box2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/box2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31316 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/box2d/bipedal_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/box2d/car_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29145 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/box2d/car_racing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32721 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/box2d/lunar_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.298094 gymnasium-0.29.0/gymnasium/envs/classic_control/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/classic_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/classic_control/acrobot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.298094 gymnasium-0.29.0/gymnasium/envs/classic_control/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/classic_control/assets/clockwise.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/classic_control/cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/classic_control/continuous_mountain_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/classic_control/mountain_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/classic_control/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/classic_control/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.302094 gymnasium-0.29.0/gymnasium/envs/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/ant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/ant_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/ant_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.302094 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/ant.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/half_cheetah.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/hopper.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/humanoid.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/humanoidstandup.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/inverted_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/point.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/pusher.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/reacher.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/swimmer.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/assets/walker2d.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/half_cheetah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/half_cheetah_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/half_cheetah_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/hopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/hopper_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/hopper_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/humanoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/humanoid_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/humanoid_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/humanoidstandup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23799 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/humanoidstandup_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/inverted_double_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/inverted_double_pendulum_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/inverted_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/inverted_pendulum_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/mujoco_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25376 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/mujoco_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/pusher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/pusher_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/reacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/reacher_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/swimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/swimmer_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/swimmer_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/walker2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/walker2d_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/mujoco/walker2d_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.302094 gymnasium-0.29.0/gymnasium/envs/phys2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/phys2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.302094 gymnasium-0.29.0/gymnasium/envs/phys2d/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/phys2d/assets/clockwise.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/phys2d/cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/phys2d/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43653 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.306094 gymnasium-0.29.0/gymnasium/envs/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17206 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/tabular/blackjack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/tabular/cliffwalking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.306094 gymnasium-0.29.0/gymnasium/envs/toy_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/blackjack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/cliffwalking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.306094 gymnasium-0.29.0/gymnasium/envs/toy_text/font/
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/font/Minecraft.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/frozen_lake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.314094 gymnasium-0.29.0/gymnasium/envs/toy_text/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/C2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/C3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/C4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/C5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/C6.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/C7.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/C8.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/C9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/CA.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/CJ.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19498 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/CK.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/CQ.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/CT.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/Card.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/D2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/D3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/D4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/D5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/D6.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/D7.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/D8.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/D9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/DA.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/DJ.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19118 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/DK.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/DQ.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/DT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/H2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/H3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/H4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/H5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/H6.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/H7.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/H8.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/H9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/HA.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/HJ.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/HK.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/HQ.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/HT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/S2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/S3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/S4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/S5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/S6.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/S7.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/S8.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/S9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/SA.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/SJ.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/SK.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/SQ.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/ST.png
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/cab_front.png
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/cab_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/cab_rear.png
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/cab_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/cookie.png
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/cracked_hole.png
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/elf_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/elf_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/elf_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/elf_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/goal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_horiz.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_top.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/hole.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/hotel.png
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/ice.png
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_bg1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_bg2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_cliff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_near-cliff1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_near-cliff2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/passenger.png
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/stool.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/img/taxi_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/taxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/envs/toy_text/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.314094 gymnasium-0.29.0/gymnasium/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/functional_jax_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.314094 gymnasium-0.29.0/gymnasium/experimental/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26861 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/vector/async_vector_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/vector/sync_vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.314094 gymnasium-0.29.0/gymnasium/experimental/vector/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/vector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/vector/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/vector/utils/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/vector/utils/space_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/vector/vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.318094 gymnasium-0.29.0/gymnasium/experimental/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/atari_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/jax_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/jax_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/lambda_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/lambda_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/lambda_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/numpy_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/stateful_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/stateful_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/stateful_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.318094 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/dict_info_to_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/jax_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/jax_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/numpy_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/record_episode_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/vectorize_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/vectorize_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/vectorize_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.318094 gymnasium-0.29.0/gymnasium/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/multi_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/multi_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/spaces/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.322094 gymnasium-0.29.0/gymnasium/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/env_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/ezpickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/passive_env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/record_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/save_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/seeding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/utils/step_api_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.322094 gymnasium-0.29.0/gymnasium/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27833 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/async_vector_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/sync_vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.322094 gymnasium-0.29.0/gymnasium/vector/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/utils/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/utils/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/vector/vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.326094 gymnasium-0.29.0/gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/atari_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/autoreset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/clip_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/filter_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/flatten_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/frame_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/gray_scale_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/human_rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.326094 gymnasium-0.29.0/gymnasium/wrappers/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/monitoring/video_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/order_enforcing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/pixel_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/record_episode_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/record_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/render_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/rescale_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/resize_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/step_api_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/time_aware_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/transform_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/transform_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-14 22:47:25.000000 gymnasium-0.29.0/gymnasium/wrappers/vector_list_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.298094 gymnasium-0.29.0/gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-14 22:47:35.000000 gymnasium-0.29.0/gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-14 22:47:35.000000 gymnasium-0.29.0/gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:47:35.000000 gymnasium-0.29.0/gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-14 22:47:35.000000 gymnasium-0.29.0/gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 22:47:35.000000 gymnasium-0.29.0/gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-14 22:47:25.000000 gymnasium-0.29.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:47:35.326094 gymnasium-0.29.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-14 22:47:25.000000 gymnasium-0.29.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:47:35.326094 gymnasium-0.29.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-07-14 22:47:25.000000 gymnasium-0.29.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-14 22:47:25.000000 gymnasium-0.29.0/tests/testing_env.py
```

### Comparing `gymnasium-0.28.1/LICENSE` & `gymnasium-0.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/PKG-INFO` & `gymnasium-0.29.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gymnasium
-Version: 0.28.1
+Version: 0.29.0
 Summary: A standard API for reinforcement learning and a diverse set of reference environments (formerly Gym).
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://farama.org
 Project-URL: Repository, https://github.com/Farama-Foundation/Gymnasium
 Project-URL: Documentation, https://gymnasium.farama.org
 Project-URL: Bug Report, https://github.com/Farama-Foundation/Gymnasium/issues
 Keywords: Reinforcement Learning,game,RL,AI,gymnasium
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: atari
 Provides-Extra: accept-rom-license
 Provides-Extra: box2d
 Provides-Extra: classic-control
 Provides-Extra: classic_control
 Provides-Extra: mujoco-py
@@ -33,15 +32,16 @@
 Provides-Extra: toy_text
 Provides-Extra: jax
 Provides-Extra: other
 Provides-Extra: all
 Provides-Extra: testing
 License-File: LICENSE
 
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8127025.svg)](https://doi.org/10.5281/zenodo.8127025)
+
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/Gymnasium/main/gymnasium-text.png" width="500px"/>
 </p>
 
 Gymnasium is an open source Python library for developing and comparing reinforcement learning algorithms by providing a standard API to communicate between learning algorithms and environments, as well as a standard set of environments compliant with that API. This is a fork of OpenAI's [Gym](https://github.com/openai/gym) library by it's maintainers (OpenAI handed over maintenance a few years ago to an outside team), and is where future maintenance will occur going forward.
 
@@ -59,15 +59,15 @@
 
 ## Installation
 
 To install the base Gymnasium library, use `pip install gymnasium`
 
 This does not include dependencies for all families of environments (there's a massive number, and some can be problematic to install on certain systems). You can install these dependencies for one family like `pip install "gymnasium[atari]"` or use `pip install "gymnasium[all]"` to install all dependencies.
 
-We support and test for Python 3.7, 3.8, 3.9, 3.10, 3.11 on Linux and macOS. We will accept PRs related to Windows, but do not officially support it.
+We support and test for Python 3.8, 3.9, 3.10, 3.11 on Linux and macOS. We will accept PRs related to Windows, but do not officially support it.
 
 ## API
 
 The Gymnasium API models environments as simple Python `env` classes. Creating environment instances and interacting with them is very simple- here's an example using the "CartPole-v1" environment:
 
 ```python
 import gymnasium as gym
@@ -86,20 +86,40 @@
 ## Notable Related Libraries
 
 Please note that this is an incomplete list, and just includes libraries that the maintainers most commonly point newcommers to when asked for recommendations.
 
 * [CleanRL](https://github.com/vwxyzjn/cleanrl) is a learning library based on the Gymnasium API. It is designed to cater to newer people in the field and provides very good reference implementations.
 * [PettingZoo](https://github.com/Farama-Foundation/PettingZoo) is a multi-agent version of Gymnasium with a number of implemented environments, i.e. multi-agent Atari environments.
 * The Farama Foundation also has a collection of many other [environments](https://farama.org/projects) that are maintained by the same team as Gymnasium and use the Gymnasium API.
-* If you're looking to track your rewards, hyperparameters, random seeds and more you can use [Comet](https://www.comet.com/site/?utm_source=gymnasium&utm_medium=partner&utm_campaign=partner_gymnasium_2023&utm_content=github) which has a built-in integration for Gymnasium. [Here's tutorial on how to use them together](https://bit.ly/CometGymnasiumIntegration). Comet is a sponsor of the Farama Foundation.
+* [Comet](https://www.comet.com/site/?utm_source=gymnasium&utm_medium=partner&utm_campaign=partner_gymnasium_2023&utm_content=github) is a free ML-Ops tool that tracks rewards, metrics, hyperparameters, and code for ML training runs. Comet has an easy-to use integration with Gymnasium, here's a [tutorial](https://bit.ly/CometGymnasiumIntegration) on how to use them together! Comet is a sponsor of the Farama Foundation!
+
+
 
 ## Environment Versioning
 
 Gymnasium keeps strict versioning for reproducibility reasons. All environments end in a suffix like "-v0".  When changes are made to environments that might impact learning results, the number is increased by one to prevent potential confusion. These inherent from Gym.
 
 ## Development Roadmap
 
 We have a roadmap for future development work for Gymnasium available here: https://github.com/Farama-Foundation/Gymnasium/issues/12
 
 ## Support Gymnasium's Development
 
 If you are financially able to do so and would like to support the development of Gymnasium, please join others in the community in [donating to us](https://github.com/sponsors/Farama-Foundation).
+
+## Citation
+
+You can cite Gymnasium as:
+
+```
+@misc{towers_gymnasium_2023,
+        title = {Gymnasium},
+        url = {https://zenodo.org/record/8127025},
+        abstract = {An API standard for single-agent reinforcement learning environments, with popular reference environments and related utilities (formerly Gym)},
+        urldate = {2023-07-08},
+        publisher = {Zenodo},
+        author = {Towers, Mark and Terry, Jordan K. and Kwiatkowski, Ariel and Balis, John U. and Cola, Gianluca de and Deleu, Tristan and Goulão, Manuel and Kallinteris, Andreas and KG, Arjun and Krimmel, Markus and Perez-Vicente, Rodrigo and Pierré, Andrea and Schulhoff, Sander and Tai, Jun Jet and Shen, Andrew Tan Jin and Younis, Omar G.},
+        month = mar,
+        year = {2023},
+        doi = {10.5281/zenodo.8127026},
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gymnasium-0.28.1/README.md` & `gymnasium-0.29.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8127025.svg)](https://doi.org/10.5281/zenodo.8127025)
+
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/Gymnasium/main/gymnasium-text.png" width="500px"/>
 </p>
 
 Gymnasium is an open source Python library for developing and comparing reinforcement learning algorithms by providing a standard API to communicate between learning algorithms and environments, as well as a standard set of environments compliant with that API. This is a fork of OpenAI's [Gym](https://github.com/openai/gym) library by it's maintainers (OpenAI handed over maintenance a few years ago to an outside team), and is where future maintenance will occur going forward.
 
@@ -20,15 +21,15 @@
 
 ## Installation
 
 To install the base Gymnasium library, use `pip install gymnasium`
 
 This does not include dependencies for all families of environments (there's a massive number, and some can be problematic to install on certain systems). You can install these dependencies for one family like `pip install "gymnasium[atari]"` or use `pip install "gymnasium[all]"` to install all dependencies.
 
-We support and test for Python 3.7, 3.8, 3.9, 3.10, 3.11 on Linux and macOS. We will accept PRs related to Windows, but do not officially support it.
+We support and test for Python 3.8, 3.9, 3.10, 3.11 on Linux and macOS. We will accept PRs related to Windows, but do not officially support it.
 
 ## API
 
 The Gymnasium API models environments as simple Python `env` classes. Creating environment instances and interacting with them is very simple- here's an example using the "CartPole-v1" environment:
 
 ```python
 import gymnasium as gym
@@ -47,20 +48,40 @@
 ## Notable Related Libraries
 
 Please note that this is an incomplete list, and just includes libraries that the maintainers most commonly point newcommers to when asked for recommendations.
 
 * [CleanRL](https://github.com/vwxyzjn/cleanrl) is a learning library based on the Gymnasium API. It is designed to cater to newer people in the field and provides very good reference implementations.
 * [PettingZoo](https://github.com/Farama-Foundation/PettingZoo) is a multi-agent version of Gymnasium with a number of implemented environments, i.e. multi-agent Atari environments.
 * The Farama Foundation also has a collection of many other [environments](https://farama.org/projects) that are maintained by the same team as Gymnasium and use the Gymnasium API.
-* If you're looking to track your rewards, hyperparameters, random seeds and more you can use [Comet](https://www.comet.com/site/?utm_source=gymnasium&utm_medium=partner&utm_campaign=partner_gymnasium_2023&utm_content=github) which has a built-in integration for Gymnasium. [Here's tutorial on how to use them together](https://bit.ly/CometGymnasiumIntegration). Comet is a sponsor of the Farama Foundation.
+* [Comet](https://www.comet.com/site/?utm_source=gymnasium&utm_medium=partner&utm_campaign=partner_gymnasium_2023&utm_content=github) is a free ML-Ops tool that tracks rewards, metrics, hyperparameters, and code for ML training runs. Comet has an easy-to use integration with Gymnasium, here's a [tutorial](https://bit.ly/CometGymnasiumIntegration) on how to use them together! Comet is a sponsor of the Farama Foundation!
+
+
 
 ## Environment Versioning
 
 Gymnasium keeps strict versioning for reproducibility reasons. All environments end in a suffix like "-v0".  When changes are made to environments that might impact learning results, the number is increased by one to prevent potential confusion. These inherent from Gym.
 
 ## Development Roadmap
 
 We have a roadmap for future development work for Gymnasium available here: https://github.com/Farama-Foundation/Gymnasium/issues/12
 
 ## Support Gymnasium's Development
 
 If you are financially able to do so and would like to support the development of Gymnasium, please join others in the community in [donating to us](https://github.com/sponsors/Farama-Foundation).
+
+## Citation
+
+You can cite Gymnasium as:
+
+```
+@misc{towers_gymnasium_2023,
+        title = {Gymnasium},
+        url = {https://zenodo.org/record/8127025},
+        abstract = {An API standard for single-agent reinforcement learning environments, with popular reference environments and related utilities (formerly Gym)},
+        urldate = {2023-07-08},
+        publisher = {Zenodo},
+        author = {Towers, Mark and Terry, Jordan K. and Kwiatkowski, Ariel and Balis, John U. and Cola, Gianluca de and Deleu, Tristan and Goulão, Manuel and Kallinteris, Andreas and KG, Arjun and Krimmel, Markus and Perez-Vicente, Rodrigo and Pierré, Andrea and Schulhoff, Sander and Tai, Jun Jet and Shen, Andrew Tan Jin and Younis, Omar G.},
+        month = mar,
+        year = {2023},
+        doi = {10.5281/zenodo.8127026},
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gymnasium-0.28.1/gymnasium/__init__.py` & `gymnasium-0.29.0/gymnasium/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 from gymnasium.envs.registration import (
     make,
     spec,
     register,
     registry,
     pprint_registry,
     make_vec,
+    register_envs,
 )
 
 # necessary for `envs.__init__` which registers all gymnasium environments and loads plugins
 from gymnasium import envs
-from gymnasium import experimental, spaces, utils, vector, wrappers, error, logger
+from gymnasium import spaces, utils, vector, wrappers, error, logger
+from gymnasium import experimental
 
 
 __all__ = [
     # core classes
     "Env",
     "Wrapper",
     "ObservationWrapper",
@@ -34,25 +36,26 @@
     # registration
     "make",
     "make_vec",
     "spec",
     "register",
     "registry",
     "pprint_registry",
+    "register_envs",
     # module folders
     "envs",
     "experimental",
     "spaces",
     "utils",
     "vector",
     "wrappers",
     "error",
     "logger",
 ]
-__version__ = "0.28.1"
+__version__ = "0.29.0"
 
 
 # Initializing pygame initializes audio connections through SDL. SDL uses alsa by default on all Linux systems
 # SDL connecting to alsa frequently create these giant lists of warnings every time you import an environment using
 #   pygame
 # DSP is far more benign (and should probably be the default in SDL anyways)
```

### Comparing `gymnasium-0.28.1/gymnasium/core.py` & `gymnasium-0.29.0/gymnasium/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import TYPE_CHECKING, Any, Generic, SupportsFloat, TypeVar
 
 import numpy as np
 
-from gymnasium import spaces
+from gymnasium import logger, spaces
 from gymnasium.utils import RecordConstructorArgs, seeding
 
 
 if TYPE_CHECKING:
     from gymnasium.envs.registration import EnvSpec, WrapperSpec
 
 ObsType = TypeVar("ObsType")
@@ -181,14 +181,15 @@
         """
         raise NotImplementedError
 
     def close(self):
         """After the user has finished using the environment, close contains the code necessary to "clean up" the environment.
 
         This is critical for closing rendering windows, database or HTTP connections.
+        Calling ``close`` on an already closed environment has no effect and won't raise an error.
         """
         pass
 
     @property
     def unwrapped(self) -> Env[ObsType, ActType]:
         """Returns the base non-wrapped environment.
 
@@ -229,14 +230,18 @@
 
     def __exit__(self, *args: Any):
         """Support with-statement for the environment and closes the environment."""
         self.close()
         # propagate exception
         return False
 
+    def get_wrapper_attr(self, name: str) -> Any:
+        """Gets the attribute `name` from the environment."""
+        return getattr(self, name)
+
 
 WrapperObsType = TypeVar("WrapperObsType")
 WrapperActType = TypeVar("WrapperActType")
 
 
 class Wrapper(
     Env[WrapperObsType, WrapperActType],
@@ -268,23 +273,56 @@
         self._observation_space: spaces.Space[WrapperObsType] | None = None
         self._reward_range: tuple[SupportsFloat, SupportsFloat] | None = None
         self._metadata: dict[str, Any] | None = None
 
         self._cached_spec: EnvSpec | None = None
 
     def __getattr__(self, name: str) -> Any:
-        """Returns an attribute with ``name``, unless ``name`` starts with an underscore."""
+        """Returns an attribute with ``name``, unless ``name`` starts with an underscore.
+
+        Args:
+            name: The variable name
+
+        Returns:
+            The value of the variable in the wrapper stack
+
+        Warnings:
+            This feature is deprecated and removed in v1.0 and replaced with `env.get_attr(name})`
+        """
         if name == "_np_random":
             raise AttributeError(
                 "Can't access `_np_random` of a wrapper, use `self.unwrapped._np_random` or `self.np_random`."
             )
         elif name.startswith("_"):
             raise AttributeError(f"accessing private attribute '{name}' is prohibited")
+        logger.warn(
+            f"env.{name} to get variables from other wrappers is deprecated and will be removed in v1.0, "
+            f"to get this variable you can do `env.unwrapped.{name}` for environment variables or `env.get_attr('{name}')` that will search the reminding wrappers."
+        )
         return getattr(self.env, name)
 
+    def get_wrapper_attr(self, name: str) -> Any:
+        """Gets an attribute from the wrapper and lower environments if `name` doesn't exist in this object.
+
+        Args:
+            name: The variable name to get
+
+        Returns:
+            The variable with name in wrapper or lower environments
+        """
+        if hasattr(self, name):
+            return getattr(self, name)
+        else:
+            try:
+                return self.env.get_wrapper_attr(name)
+            except AttributeError as e:
+                raise AttributeError(
+                    f"wrapper {self.class_name()} has no attribute {name!r}"
+                ) from e
+
     @property
     def spec(self) -> EnvSpec | None:
         """Returns the :attr:`Env` :attr:`spec` attribute with the `WrapperSpec` if the wrapper inherits from `EzPickle`."""
         if self._cached_spec is not None:
             return self._cached_spec
 
         env_spec = self.env.spec
@@ -356,14 +394,15 @@
         self._observation_space = space
 
     @property
     def reward_range(self) -> tuple[SupportsFloat, SupportsFloat]:
         """Return the :attr:`Env` :attr:`reward_range` unless overwritten then the wrapper :attr:`reward_range` is used."""
         if self._reward_range is None:
             return self.env.reward_range
+        logger.warn("The `reward_range` is deprecated and will be removed in v1.0")
         return self._reward_range
 
     @reward_range.setter
     def reward_range(self, value: tuple[SupportsFloat, SupportsFloat]):
         self._reward_range = value
 
     @property
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/__init__.py` & `gymnasium-0.29.0/gymnasium/envs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,31 +58,31 @@
 )
 
 
 # Phys2d (jax classic control)
 # ----------------------------------------
 
 register(
-    id="CartPoleJax-v0",
+    id="phys2d/CartPole-v0",
     entry_point="gymnasium.envs.phys2d.cartpole:CartPoleJaxEnv",
     vector_entry_point="gymnasium.envs.phys2d.cartpole:CartPoleJaxVectorEnv",
     max_episode_steps=200,
     reward_threshold=195.0,
 )
 
 register(
-    id="CartPoleJax-v1",
+    id="phys2d/CartPole-v1",
     entry_point="gymnasium.envs.phys2d.cartpole:CartPoleJaxEnv",
     vector_entry_point="gymnasium.envs.phys2d.cartpole:CartPoleJaxVectorEnv",
     max_episode_steps=500,
     reward_threshold=475.0,
 )
 
 register(
-    id="PendulumJax-v0",
+    id="phys2d/Pendulum-v0",
     entry_point="gymnasium.envs.phys2d.pendulum:PendulumJaxEnv",
     vector_entry_point="gymnasium.envs.phys2d.pendulum:PendulumJaxVectorEnv",
     max_episode_steps=200,
 )
 
 # Box2d
 # ----------------------------------------
@@ -162,19 +162,24 @@
 )
 
 
 # Tabular
 # ----------------------------------------
 
 register(
-    id="Jax-Blackjack-v0",
+    id="tabular/Blackjack-v0",
     entry_point="gymnasium.envs.tabular.blackjack:BlackJackJaxEnv",
     kwargs={"sutton_and_barto": True, "natural": False},
 )
 
+register(
+    id="tabular/CliffWalking-v0",
+    entry_point="gymnasium.envs.tabular.cliffwalking:CliffWalkingJaxEnv",
+)
+
 
 # Mujoco
 # ----------------------------------------
 
 # 2D
 
 register(
@@ -365,15 +370,15 @@
     max_episode_steps=1000,
 )
 
 
 # --- For shimmy compatibility
 def _raise_shimmy_error(*args: Any, **kwargs: Any):
     raise ImportError(
-        "To use the gym compatibility environments, run `pip install shimmy[gym]`"
+        "To use the gym compatibility environments, run `pip install shimmy[gym-v21]` or `pip install shimmy[gym-v26]`"
     )
 
 
 # When installed, shimmy will re-register these environments with the correct entry_point
 register(id="GymV21Environment-v0", entry_point=_raise_shimmy_error)
 register(id="GymV26Environment-v0", entry_point=_raise_shimmy_error)
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/box2d/bipedal_walker.py` & `gymnasium-0.29.0/gymnasium/envs/box2d/bipedal_walker.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/box2d/car_dynamics.py` & `gymnasium-0.29.0/gymnasium/envs/box2d/car_dynamics.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/box2d/car_racing.py` & `gymnasium-0.29.0/gymnasium/envs/box2d/car_racing.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/box2d/lunar_lander.py` & `gymnasium-0.29.0/gymnasium/envs/box2d/lunar_lander.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,32 +284,32 @@
         self.continuous = continuous
 
         low = np.array(
             [
                 # these are bounds for position
                 # realistically the environment should have ended
                 # long before we reach more than 50% outside
-                -1.5 * SCALE * 2,
-                -1.5 * SCALE * 2,
+                -1.5,
+                -1.5,
                 # velocity bounds is 5x rated speed
                 -5.0,
                 -5.0,
                 -math.pi,
                 -5.0,
                 -0.0,
                 -0.0,
             ]
         ).astype(np.float32)
         high = np.array(
             [
                 # these are bounds for position
                 # realistically the environment should have ended
                 # long before we reach more than 50% outside
-                1.5 * SCALE * 2,
-                1.5 * SCALE * 2,
+                1.5,
+                1.5,
                 # velocity bounds is 5x rated speed
                 5.0,
                 5.0,
                 math.pi,
                 5.0,
                 1.0,
                 1.0,
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/classic_control/acrobot.py` & `gymnasium-0.29.0/gymnasium/envs/classic_control/acrobot.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/classic_control/assets/clockwise.png` & `gymnasium-0.29.0/gymnasium/envs/classic_control/assets/clockwise.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/classic_control/cartpole.py` & `gymnasium-0.29.0/gymnasium/envs/classic_control/cartpole.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
        if the cart leaves the `(-2.4, 2.4)` range.
     -  The pole angle can be observed between  `(-.418, .418)` radians (or **±24°**), but the episode terminates
        if the pole angle is not in the range `(-.2095, .2095)` (or **±12°**)
 
     ## Rewards
 
     Since the goal is to keep the pole upright for as long as possible, a reward of `+1` for every step taken,
-    including the termination step, is allotted. The threshold for rewards is 475 for v1.
+    including the termination step, is allotted. The threshold for rewards is 500 for v1 and 200 for v0.
 
     ## Starting State
 
     All observations are assigned a uniformly random value in `(-0.05, 0.05)`
 
     ## Episode End
 
@@ -358,18 +358,18 @@
             ],
             dtype=np.float32,
         )
 
         self.low = -0.05
         self.high = 0.05
 
-        self.action_space = batch_space(spaces.Discrete(2), num_envs)
-        self.observation_space = batch_space(
-            spaces.Box(-high, high, dtype=np.float32), num_envs
-        )
+        self.single_action_space = spaces.Discrete(2)
+        self.action_space = batch_space(self.single_action_space, num_envs)
+        self.single_observation_space = spaces.Box(-high, high, dtype=np.float32)
+        self.observation_space = batch_space(self.single_observation_space, num_envs)
 
         self.render_mode = render_mode
 
         self.screen_width = 600
         self.screen_height = 400
         self.screens = None
         self.clocks = None
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/classic_control/continuous_mountain_car.py` & `gymnasium-0.29.0/gymnasium/envs/classic_control/continuous_mountain_car.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/classic_control/mountain_car.py` & `gymnasium-0.29.0/gymnasium/envs/classic_control/mountain_car.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/classic_control/pendulum.py` & `gymnasium-0.29.0/gymnasium/envs/classic_control/pendulum.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     ## Rewards
 
     The reward function is defined as:
 
     *r = -(theta<sup>2</sup> + 0.1 * theta_dt<sup>2</sup> + 0.001 * torque<sup>2</sup>)*
 
-    where `$\theta$` is the pendulum's angle normalized between *[-pi, pi]* (with 0 being in the upright position).
+    where `theta` is the pendulum's angle normalized between *[-pi, pi]* (with 0 being in the upright position).
     Based on the above equation, the minimum reward that can be obtained is
     *-(pi<sup>2</sup> + 0.1 * 8<sup>2</sup> + 0.001 * 2<sup>2</sup>) = -16.2736044*,
     while the maximum reward is zero (pendulum is upright with zero velocity and no torque applied).
 
     ## Starting State
 
     The starting state is a random angle in *[-pi, pi]* and a random angular velocity in *[-1,1]*.
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/classic_control/utils.py` & `gymnasium-0.29.0/gymnasium/envs/classic_control/utils.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/__init__.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/ant.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/ant.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/ant_v3.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/ant_v3.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/ant_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/ant_v4.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     """
     ## Description
 
     This environment is based on the environment introduced by Schulman,
     Moritz, Levine, Jordan and Abbeel in ["High-Dimensional Continuous Control
     Using Generalized Advantage Estimation"](https://arxiv.org/abs/1506.02438).
     The ant is a 3D robot consisting of one torso (free rotational body) with
-    four legs attached to it with each leg having two links. The goal is to
+    four legs attached to it with each leg having two body parts. The goal is to
     coordinate the four legs to move in the forward (right) direction by applying
-    torques on the eight hinges connecting the two links of each leg and the torso
-    (nine parts and eight hinges).
+    torques on the eight hinges connecting the two body parts of each leg and the torso
+    (nine body parts and eight hinges).
 
     ## Action Space
     The action space is a `Box(-1, 1, (8,), float32)`. An action represents the torques applied at the hinge joints.
 
     | Num | Action                                                            | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
     | --- | ----------------------------------------------------------------- | ----------- | ----------- | -------------------------------- | ----- | ------------ |
     | 0   | Torque applied on the rotor between the torso and back right hip  | -1          | 1           | hip_4 (right_back_leg)           | hinge | torque (N m) |
@@ -34,28 +34,26 @@
     | 3   | Torque applied on the rotor between the front left two links      | -1          | 1           | angle_1 (front_left_leg)         | hinge | torque (N m) |
     | 4   | Torque applied on the rotor between the torso and front right hip | -1          | 1           | hip_2 (front_right_leg)          | hinge | torque (N m) |
     | 5   | Torque applied on the rotor between the front right two links     | -1          | 1           | angle_2 (front_right_leg)        | hinge | torque (N m) |
     | 6   | Torque applied on the rotor between the torso and back left hip   | -1          | 1           | hip_3 (back_leg)                 | hinge | torque (N m) |
     | 7   | Torque applied on the rotor between the back left two links       | -1          | 1           | angle_3 (back_leg)               | hinge | torque (N m) |
 
     ## Observation Space
-
     Observations consist of positional values of different body parts of the ant,
     followed by the velocities of those individual parts (their derivatives) with all
     the positions ordered before all the velocities.
 
     By default, observations do not include the x- and y-coordinates of the ant's torso. These may
     be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will have 29 dimensions where the first two dimensions
+    In that case, the observation space will be a `Box(-Inf, Inf, (29,), float64)` where the first two observations
     represent the x- and y- coordinates of the ant's torso.
     Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x- and y-coordinates
     of the torso will be returned in `info` with keys `"x_position"` and `"y_position"`, respectively.
 
-    However, by default, an observation is a `ndarray` with shape `(27,)`
-    where the elements correspond to the following:
+    However, by default, observation Space is a `Box(-Inf, Inf, (27,), float64)` where the elements correspond to the following:
 
     | Num | Observation                                                  | Min    | Max    | Name (in corresponding XML file)       | Joint | Unit                     |
     |-----|--------------------------------------------------------------|--------|--------|----------------------------------------|-------|--------------------------|
     | 0   | z-coordinate of the torso (centre)                           | -Inf   | Inf    | torso                                  | free  | position (m)             |
     | 1   | x-orientation of the torso (centre)                          | -Inf   | Inf    | torso                                  | free  | angle (rad)              |
     | 2   | y-orientation of the torso (centre)                          | -Inf   | Inf    | torso                                  | free  | angle (rad)              |
     | 3   | z-orientation of the torso (centre)                          | -Inf   | Inf    | torso                                  | free  | angle (rad)              |
@@ -78,33 +76,34 @@
     | 20  | angular velocity of the angle between front left links       | -Inf   | Inf    | ankle_1 (front_left_leg)               | hinge | angle (rad)              |
     | 21  | angular velocity of angle between torso and front right link | -Inf   | Inf    | hip_2 (front_right_leg)                | hinge | angle (rad)              |
     | 22  | angular velocity of the angle between front right links      | -Inf   | Inf    | ankle_2 (front_right_leg)              | hinge | angle (rad)              |
     | 23  | angular velocity of angle between torso and back left link   | -Inf   | Inf    | hip_3 (back_leg)                       | hinge | angle (rad)              |
     | 24  | angular velocity of the angle between back left links        | -Inf   | Inf    | ankle_3 (back_leg)                     | hinge | angle (rad)              |
     | 25  | angular velocity of angle between torso and back right link  | -Inf   | Inf    | hip_4 (right_back_leg)                 | hinge | angle (rad)              |
     | 26  | angular velocity of the angle between back right links       | -Inf   | Inf    | ankle_4 (right_back_leg)               | hinge | angle (rad)              |
+    | excluded | x-coordinate of the torso (centre)                      | -Inf   | Inf    | torso                                  | free  | position (m)             |
+    | excluded | y-coordinate of the torso (centre)                      | -Inf   | Inf    | torso                                  | free  | position (m)             |
 
 
     If version < `v4` or `use_contact_forces` is `True` then the observation space is extended by 14*6 = 84 elements, which are contact forces
     (external forces - force x, y, z and torque x, y, z) applied to the
-    center of mass of each of the objects. The 14 object are:
+    center of mass of each of the body parts. The 14 body parts are:
 
-    in `v4` or earlier:
-    | id | object |
+    | id (for `v2`, `v3`, `v4)` | body parts |
     |  ---  |  ------------  |
-    | 0 | worldObject (note: forces are always full of zeros) |
-    | 1 | torso |
-    | 2 | front_left_leg |
-    | 3 | aux_1 (front left leg) |
-    | 4 | ankle_1 (front left leg) |
-    | 5 | front_right_leg |
-    | 6 | aux_2 (front right leg) |
-    | 7 | ankle_2 (front right leg) |
-    | 8 | back_leg (back left leg) |
-    | 9 | aux_3 (back left leg) |
+    | 0  | worldbody (note: forces are always full of zeros) |
+    | 1  | torso |
+    | 2  | front_left_leg |
+    | 3  | aux_1 (front left leg) |
+    | 4  | ankle_1 (front left leg) |
+    | 5  | front_right_leg |
+    | 6  | aux_2 (front right leg) |
+    | 7  | ankle_2 (front right leg) |
+    | 8  | back_leg (back left leg) |
+    | 9  | aux_3 (back left leg) |
     | 10 | ankle_3 (back left leg) |
     | 11 | right_back_leg |
     | 12 | aux_4 (back right leg) |
     | 13 | ankle_4 (back right leg) |
 
 
     The (x,y,z) coordinates are translational DOFs while the orientations are rotational
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/ant.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/ant.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/half_cheetah.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/half_cheetah.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/hopper.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/hopper.xml`

 * *Files 10% similar despite different names*

#### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/hopper.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/hopper.xml`

```diff
@@ -1,37 +1,42 @@
 <?xml version="1.0" encoding="utf-8"?>
+<!--
+Hopper model for `Hopper-v5`, based on openai/gym/Walker2d
+modified by @saran_t
+  - To not require `coordinate="global"`
+-->
 <mujoco model="hopper">
-  <compiler angle="degree" coordinate="global" inertiafromgeom="true"/>
+  <compiler angle="degree" inertiafromgeom="true"/>
   <default>
     <joint armature="1" damping="1" limited="true"/>
     <geom conaffinity="1" condim="1" contype="1" margin="0.001" material="geom" rgba="0.8 0.6 .4 1" solimp=".8 .8 .01" solref=".02 1"/>
     <motor ctrllimited="true" ctrlrange="-.4 .4"/>
   </default>
   <option integrator="RK4" timestep="0.002"/>
   <visual>
     <map znear="0.02"/>
   </visual>
   <worldbody>
     <light cutoff="100" diffuse="1 1 1" dir="-0 0 -1.3" directional="true" exponent="1" pos="0 0 1.3" specular=".1 .1 .1"/>
     <geom conaffinity="1" condim="3" name="floor" pos="0 0 0" rgba="0.8 0.9 0.8 1" size="20 20 .125" type="plane" material="MatPlane"/>
     <body name="torso" pos="0 0 1.25">
-      <camera name="track" mode="trackcom" pos="0 -3 1" xyaxes="1 0 0 0 0 1"/>
-      <joint armature="0" axis="1 0 0" damping="0" limited="false" name="rootx" pos="0 0 0" stiffness="0" type="slide"/>
-      <joint armature="0" axis="0 0 1" damping="0" limited="false" name="rootz" pos="0 0 0" ref="1.25" stiffness="0" type="slide"/>
-      <joint armature="0" axis="0 1 0" damping="0" limited="false" name="rooty" pos="0 0 1.25" stiffness="0" type="hinge"/>
-      <geom friction="0.9" fromto="0 0 1.45 0 0 1.05" name="torso_geom" size="0.05" type="capsule"/>
-      <body name="thigh" pos="0 0 1.05">
-        <joint axis="0 -1 0" name="thigh_joint" pos="0 0 1.05" range="-150 0" type="hinge"/>
-        <geom friction="0.9" fromto="0 0 1.05 0 0 0.6" name="thigh_geom" size="0.05" type="capsule"/>
-        <body name="leg" pos="0 0 0.35">
-          <joint axis="0 -1 0" name="leg_joint" pos="0 0 0.6" range="-150 0" type="hinge"/>
-          <geom friction="0.9" fromto="0 0 0.6 0 0 0.1" name="leg_geom" size="0.04" type="capsule"/>
-          <body name="foot" pos="0.13 0 0">
-            <joint axis="0 -1 0" name="foot_joint" pos="0 0 0.1" range="-45 45" type="hinge"/>
-            <geom friction="2.0" fromto="-0.13 0 0.1 0.26 0 0.1" name="foot_geom" size="0.06" type="capsule"/>
+      <camera name="track" mode="trackcom" pos="0 -3 -0.25" xyaxes="1 0 0 0 0 1"/>
+      <joint armature="0" axis="1 0 0" damping="0" limited="false" name="rootx" pos="0 0 -1.25" stiffness="0" type="slide"/>
+      <joint armature="0" axis="0 0 1" damping="0" limited="false" name="rootz" pos="0 0 -1.25" ref="1.25" stiffness="0" type="slide"/>
+      <joint armature="0" axis="0 1 0" damping="0" limited="false" name="rooty" pos="0 0 0" stiffness="0" type="hinge"/>
+      <geom friction="0.9" name="torso_geom" size="0.05 0.19999999999999996" type="capsule"/>
+      <body name="thigh" pos="0 0 -0.19999999999999996">
+        <joint axis="0 -1 0" name="thigh_joint" pos="0 0 0" range="-150 0" type="hinge"/>
+        <geom friction="0.9" pos="0 0 -0.22500000000000009" name="thigh_geom" size="0.05 0.22500000000000003" type="capsule"/>
+        <body name="leg" pos="0 0 -0.70000000000000007">
+          <joint axis="0 -1 0" name="leg_joint" pos="0 0 0.25" range="-150 0" type="hinge"/>
+          <geom friction="0.9" name="leg_geom" size="0.04 0.25" type="capsule"/>
+          <body name="foot" pos="0.13 0 -0.35">
+            <joint axis="0 -1 0" name="foot_joint" pos="-0.13 0 0.1" range="-45 45" type="hinge"/>
+            <geom friction="2.0" pos="-0.065 0 0.1" quat="0.70710678118654757 0 -0.70710678118654746 0" name="foot_geom" size="0.06 0.195" type="capsule"/>
           </body>
         </body>
       </body>
     </body>
   </worldbody>
   <actuator>
     <motor ctrllimited="true" ctrlrange="-1.0 1.0" gear="200.0" joint="thigh_joint"/>
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/humanoid.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/humanoid.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/humanoidstandup.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/humanoidstandup.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/inverted_pendulum.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/inverted_pendulum.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/point.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/point.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/pusher.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/pusher.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/reacher.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/reacher.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/swimmer.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/swimmer.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/walker2d.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/walker2d.xml`

 * *Files 14% similar despite different names*

#### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/assets/walker2d.xml` & `gymnasium-0.29.0/gymnasium/envs/mujoco/assets/walker2d.xml`

```diff
@@ -1,46 +1,52 @@
 <?xml version="1.0" encoding="utf-8"?>
+<!--
+Walker2D model for `Walker2d-v5`, based on openai/gym/Walker2d
+modified by @kallinteris-Andreas
+  - To not require `coordinate="global"`
+  - keep feet friction to 0.9/1.9
+-->
 <mujoco model="walker2d">
-  <compiler angle="degree" coordinate="global" inertiafromgeom="true"/>
+  <compiler angle="degree" inertiafromgeom="true"/>
   <default>
     <joint armature="0.01" damping=".1" limited="true"/>
     <geom conaffinity="0" condim="3" contype="1" density="1000" friction=".7 .1 .1" rgba="0.8 0.6 .4 1"/>
   </default>
   <option integrator="RK4" timestep="0.002"/>
   <worldbody>
     <light cutoff="100" diffuse="1 1 1" dir="-0 0 -1.3" directional="true" exponent="1" pos="0 0 1.3" specular=".1 .1 .1"/>
     <geom conaffinity="1" condim="3" name="floor" pos="0 0 0" rgba="0.8 0.9 0.8 1" size="40 40 40" type="plane" material="MatPlane"/>
     <body name="torso" pos="0 0 1.25">
-      <camera name="track" mode="trackcom" pos="0 -3 1" xyaxes="1 0 0 0 0 1"/>
-      <joint armature="0" axis="1 0 0" damping="0" limited="false" name="rootx" pos="0 0 0" stiffness="0" type="slide"/>
-      <joint armature="0" axis="0 0 1" damping="0" limited="false" name="rootz" pos="0 0 0" ref="1.25" stiffness="0" type="slide"/>
-      <joint armature="0" axis="0 1 0" damping="0" limited="false" name="rooty" pos="0 0 1.25" stiffness="0" type="hinge"/>
-      <geom friction="0.9" fromto="0 0 1.45 0 0 1.05" name="torso_geom" size="0.05" type="capsule"/>
-      <body name="thigh" pos="0 0 1.05">
-        <joint axis="0 -1 0" name="thigh_joint" pos="0 0 1.05" range="-150 0" type="hinge"/>
-        <geom friction="0.9" fromto="0 0 1.05 0 0 0.6" name="thigh_geom" size="0.05" type="capsule"/>
-        <body name="leg" pos="0 0 0.35">
-          <joint axis="0 -1 0" name="leg_joint" pos="0 0 0.6" range="-150 0" type="hinge"/>
-          <geom friction="0.9" fromto="0 0 0.6 0 0 0.1" name="leg_geom" size="0.04" type="capsule"/>
-          <body name="foot" pos="0.2 0 0">
-            <joint axis="0 -1 0" name="foot_joint" pos="0 0 0.1" range="-45 45" type="hinge"/>
-            <geom friction="0.9" fromto="-0.0 0 0.1 0.2 0 0.1" name="foot_geom" size="0.06" type="capsule"/>
+      <camera name="track" mode="trackcom" pos="0 -3 -0.25" xyaxes="1 0 0 0 0 1"/>
+      <joint armature="0" axis="1 0 0" damping="0" limited="false" name="rootx" pos="0 0 -1.25" stiffness="0" type="slide"/>
+      <joint armature="0" axis="0 0 1" damping="0" limited="false" name="rootz" pos="0 0 -1.25" ref="1.25" stiffness="0" type="slide"/>
+      <joint armature="0" axis="0 1 0" damping="0" limited="false" name="rooty" pos="0 0 0" stiffness="0" type="hinge"/>
+      <geom friction="0.9" name="torso_geom" size="0.050000000000000003 0.19999999999999996" type="capsule"/>
+      <body name="thigh" pos="0 0 -0.19999999999999996">
+        <joint axis="0 -1 0" name="thigh_joint" pos="0 0 0" range="-150 0" type="hinge"/>
+        <geom friction="0.9" pos="0 0 -0.22500000000000009" name="thigh_geom" size="0.050000000000000003 0.22500000000000003" type="capsule"/>
+        <body name="leg" pos="0 0 -0.70000000000000007">
+          <joint axis="0 -1 0" name="leg_joint" pos="0 0 0.25" range="-150 0" type="hinge"/>
+          <geom friction="0.9" name="leg_geom" size="0.040000000000000001 0.25" type="capsule"/>
+          <body name="foot" pos="0.20000000000000001 0 -0.34999999999999998">
+            <joint axis="0 -1 0" name="foot_joint" pos="-0.20000000000000001 0 0.10000000000000001" range="-45 45" type="hinge"/>
+            <geom friction="0.9" pos="-0.10000000000000001 0 0.10000000000000001" quat="0.70710678118654757 0 -0.70710678118654746 0" name="foot_geom" size="0.059999999999999998 0.10000000000000001" type="capsule"/>
           </body>
         </body>
       </body>
       <!-- copied and then replace thigh->thigh_left, leg->leg_left, foot->foot_right -->
-      <body name="thigh_left" pos="0 0 1.05">
-        <joint axis="0 -1 0" name="thigh_left_joint" pos="0 0 1.05" range="-150 0" type="hinge"/>
-        <geom friction="0.9" fromto="0 0 1.05 0 0 0.6" name="thigh_left_geom" rgba=".7 .3 .6 1" size="0.05" type="capsule"/>
-        <body name="leg_left" pos="0 0 0.35">
-          <joint axis="0 -1 0" name="leg_left_joint" pos="0 0 0.6" range="-150 0" type="hinge"/>
-          <geom friction="0.9" fromto="0 0 0.6 0 0 0.1" name="leg_left_geom" rgba=".7 .3 .6 1" size="0.04" type="capsule"/>
-          <body name="foot_left" pos="0.2 0 0">
-            <joint axis="0 -1 0" name="foot_left_joint" pos="0 0 0.1" range="-45 45" type="hinge"/>
-            <geom friction="1.9" fromto="-0.0 0 0.1 0.2 0 0.1" name="foot_left_geom" rgba=".7 .3 .6 1" size="0.06" type="capsule"/>
+      <body name="thigh_left" pos="0 0 -0.19999999999999996">
+        <joint axis="0 -1 0" name="thigh_left_joint" pos="0 0 0" range="-150 0" type="hinge"/>
+        <geom friction="0.9" name="thigh_left_geom" rgba=".7 .3 .6 1" size="0.050000000000000003 0.22500000000000003" pos="0 0 -0.22500000000000009" type="capsule"/>
+        <body name="leg_left" pos="0 0 -0.70000000000000007">
+          <joint axis="0 -1 0" name="leg_left_joint" pos="0 0 0.25" range="-150 0" type="hinge"/>
+          <geom friction="0.9" name="leg_left_geom" rgba=".7 .3 .6 1" size="0.040000000000000001 0.25" type="capsule"/>
+          <body name="foot_left" pos="0.20000000000000001 0 -0.34999999999999998">
+            <joint axis="0 -1 0" name="foot_left_joint" pos="-0.20000000000000001 0 0.10000000000000001" range="-45 45" type="hinge"/>
+            <geom friction="1.9" name="foot_left_geom" rgba=".7 .3 .6 1" size="0.059999999999999998 0.10000000000000001" pos="-0.10000000000000001 0 0.10000000000000001" type="capsule" quat="0.70710678118654757 0 -0.70710678118654746 0"/>
           </body>
         </body>
       </body>
     </body>
   </worldbody>
   <actuator>
     <!-- <motor joint="torso_joint" ctrlrange="-100.0 100.0" isctrllimited="true"/>-->
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/half_cheetah.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/half_cheetah.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/half_cheetah_v3.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/half_cheetah_v3.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/half_cheetah_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/half_cheetah_v4.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,50 +14,48 @@
 
 class HalfCheetahEnv(MujocoEnv, utils.EzPickle):
     """
     ## Description
 
     This environment is based on the work by P. Wawrzyński in
     ["A Cat-Like Robot Real-Time Learning to Run"](http://staff.elka.pw.edu.pl/~pwawrzyn/pub-s/0812_LSCLRR.pdf).
-    The HalfCheetah is a 2-dimensional robot consisting of 9 links and 8
+    The HalfCheetah is a 2-dimensional robot consisting of 9 body parts and 8
     joints connecting them (including two paws). The goal is to apply a torque
     on the joints to make the cheetah run forward (right) as fast as possible,
     with a positive reward allocated based on the distance moved forward and a
     negative reward allocated for moving backward. The torso and head of the
     cheetah are fixed, and the torque can only be applied on the other 6 joints
     over the front and back thighs (connecting to the torso), shins
     (connecting to the thighs) and feet (connecting to the shins).
 
     ## Action Space
-    The action space is a `Box(-1, 1, (6,), float32)`. An action represents the torques applied between *links*.
+    The action space is a `Box(-1, 1, (6,), float32)`. An action represents the torques applied at the hinge joints.
 
     | Num | Action                                  | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
     | --- | --------------------------------------- | ----------- | ----------- | -------------------------------- | ----- | ------------ |
     | 0   | Torque applied on the back thigh rotor  | -1          | 1           | bthigh                           | hinge | torque (N m) |
     | 1   | Torque applied on the back shin rotor   | -1          | 1           | bshin                            | hinge | torque (N m) |
     | 2   | Torque applied on the back foot rotor   | -1          | 1           | bfoot                            | hinge | torque (N m) |
     | 3   | Torque applied on the front thigh rotor | -1          | 1           | fthigh                           | hinge | torque (N m) |
     | 4   | Torque applied on the front shin rotor  | -1          | 1           | fshin                            | hinge | torque (N m) |
     | 5   | Torque applied on the front foot rotor  | -1          | 1           | ffoot                            | hinge | torque (N m) |
 
 
     ## Observation Space
-
     Observations consist of positional values of different body parts of the
     cheetah, followed by the velocities of those individual parts (their derivatives) with all the positions ordered before all the velocities.
 
-    By default, observations do not include the x-coordinate of the cheetah's center of mass. It may
+    By default, observations do not include the cheetah's `rootx`. It may
     be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will have 18 dimensions where the first dimension
-    represents the x-coordinate of the cheetah's center of mass.
-    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x-coordinate
+    In that case, the observation space will be a `Box(-Inf, Inf, (18,), float64)` where the first element
+    represents the `rootx`.
+    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the
     will be returned in `info` with key `"x_position"`.
 
-    However, by default, the observation is a `ndarray` with shape `(17,)` where the elements correspond to the following:
-
+    However, by default, the observation is a `Box(-Inf, Inf, (17,), float64)` where the elements correspond to the following:
 
     | Num | Observation                          | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
     | --- | ------------------------------------ | ---- | --- | -------------------------------- | ----- | ------------------------ |
     | 0   | z-coordinate of the front tip        | -Inf | Inf | rootz                            | slide | position (m)             |
     | 1   | angle of the front tip               | -Inf | Inf | rooty                            | hinge | angle (rad)              |
     | 2   | angle of the second rotor            | -Inf | Inf | bthigh                           | hinge | angle (rad)              |
     | 3   | angle of the second rotor            | -Inf | Inf | bshin                            | hinge | angle (rad)              |
@@ -70,14 +68,15 @@
     | 10  | angle of the front tip               | -Inf | Inf | rooty                            | hinge | angular velocity (rad/s) |
     | 11  | angle of the second rotor            | -Inf | Inf | bthigh                           | hinge | angular velocity (rad/s) |
     | 12  | angle of the second rotor            | -Inf | Inf | bshin                            | hinge | angular velocity (rad/s) |
     | 13  | velocity of the tip along the x-axis | -Inf | Inf | bfoot                            | hinge | angular velocity (rad/s) |
     | 14  | velocity of the tip along the y-axis | -Inf | Inf | fthigh                           | hinge | angular velocity (rad/s) |
     | 15  | angular velocity of front tip        | -Inf | Inf | fshin                            | hinge | angular velocity (rad/s) |
     | 16  | angular velocity of second rotor     | -Inf | Inf | ffoot                            | hinge | angular velocity (rad/s) |
+    | excluded |  x-coordinate of the front tip  | -Inf | Inf | rootx                            | slide | position (m)             |
 
     ## Rewards
     The reward consists of two parts:
     - *forward_reward*: A reward of moving forward which is measured
     as *`forward_reward_weight` * (x-coordinate before action - x-coordinate after action)/dt*. *dt* is
     the time between actions and is dependent on the frame_skip parameter
     (fixed to 5), where the frametime is 0.01 - making the
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/hopper.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/hopper.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/hopper_v3.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/hopper_v3.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/hopper_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/hopper_v4.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,51 +24,51 @@
     one-legged figure that consist of four main body parts - the torso at the
     top, the thigh in the middle, the leg in the bottom, and a single foot on
     which the entire body rests. The goal is to make hops that move in the
     forward (right) direction by applying torques on the three hinges
     connecting the four body parts.
 
     ## Action Space
-    The action space is a `Box(-1, 1, (3,), float32)`. An action represents the torques applied between *links*
+    The action space is a `Box(-1, 1, (3,), float32)`. An action represents the torques applied at the hinge joints.
 
     | Num | Action                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
     |-----|------------------------------------|-------------|-------------|----------------------------------|-------|--------------|
     | 0   | Torque applied on the thigh rotor  | -1          | 1           | thigh_joint                      | hinge | torque (N m) |
     | 1   | Torque applied on the leg rotor    | -1          | 1           | leg_joint                        | hinge | torque (N m) |
     | 2   | Torque applied on the foot rotor   | -1          | 1           | foot_joint                       | hinge | torque (N m) |
 
     ## Observation Space
-
     Observations consist of positional values of different body parts of the
     hopper, followed by the velocities of those individual parts
     (their derivatives) with all the positions ordered before all the velocities.
 
     By default, observations do not include the x-coordinate of the hopper. It may
     be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will have 12 dimensions where the first dimension
+    In that case, the observation space will be `Box(-Inf, Inf, (12,), float64)` where the first observation
     represents the x-coordinate of the hopper.
     Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x-coordinate
     will be returned in `info` with key `"x_position"`.
 
-    However, by default, the observation is a `ndarray` with shape `(11,)` where the elements
+    However, by default, the observation is a `Box(-Inf, Inf, (11,), float64)` where the elements
     correspond to the following:
 
-    | Num | Observation                                      | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
-    | --- | ------------------------------------------------ | ---- | --- | -------------------------------- | ----- | ------------------------ |
-    | 0   | z-coordinate of the top (height of hopper)       | -Inf | Inf | rootz                            | slide | position (m)             |
-    | 1   | angle of the top                                 | -Inf | Inf | rooty                            | hinge | angle (rad)              |
-    | 2   | angle of the thigh joint                         | -Inf | Inf | thigh_joint                      | hinge | angle (rad)              |
-    | 3   | angle of the leg joint                           | -Inf | Inf | leg_joint                        | hinge | angle (rad)              |
-    | 4   | angle of the foot joint                          | -Inf | Inf | foot_joint                       | hinge | angle (rad)              |
-    | 5   | velocity of the x-coordinate of the top          | -Inf | Inf | rootx                            | slide | velocity (m/s)           |
-    | 6   | velocity of the z-coordinate (height) of the top | -Inf | Inf | rootz                            | slide | velocity (m/s)           |
-    | 7   | angular velocity of the angle of the top         | -Inf | Inf | rooty                            | hinge | angular velocity (rad/s) |
-    | 8   | angular velocity of the thigh hinge              | -Inf | Inf | thigh_joint                      | hinge | angular velocity (rad/s) |
-    | 9   | angular velocity of the leg hinge                | -Inf | Inf | leg_joint                        | hinge | angular velocity (rad/s) |
-    | 10  | angular velocity of the foot hinge               | -Inf | Inf | foot_joint                       | hinge | angular velocity (rad/s) |
+    | Num | Observation                                        | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
+    | --- | -------------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------ |
+    | 0   | z-coordinate of the torso (height of hopper)       | -Inf | Inf | rootz                            | slide | position (m)             |
+    | 1   | angle of the torso                                 | -Inf | Inf | rooty                            | hinge | angle (rad)              |
+    | 2   | angle of the thigh joint                           | -Inf | Inf | thigh_joint                      | hinge | angle (rad)              |
+    | 3   | angle of the leg joint                             | -Inf | Inf | leg_joint                        | hinge | angle (rad)              |
+    | 4   | angle of the foot joint                            | -Inf | Inf | foot_joint                       | hinge | angle (rad)              |
+    | 5   | velocity of the x-coordinate of the torso          | -Inf | Inf | rootx                          | slide | velocity (m/s)           |
+    | 6   | velocity of the z-coordinate (height) of the torso | -Inf | Inf | rootz                          | slide | velocity (m/s)           |
+    | 7   | angular velocity of the angle of the torso         | -Inf | Inf | rooty                          | hinge | angular velocity (rad/s) |
+    | 8   | angular velocity of the thigh hinge                | -Inf | Inf | thigh_joint                      | hinge | angular velocity (rad/s) |
+    | 9   | angular velocity of the leg hinge                  | -Inf | Inf | leg_joint                        | hinge | angular velocity (rad/s) |
+    | 10  | angular velocity of the foot hinge                 | -Inf | Inf | foot_joint                       | hinge | angular velocity (rad/s) |
+    | excluded | x-coordinate of the torso                     | -Inf | Inf | rootx                            | slide | position (m)             |
 
 
     ## Rewards
     The reward consists of three parts:
     - *healthy_reward*: Every timestep that the hopper is healthy (see definition in section "Episode Termination"), it gets a reward of fixed value `healthy_reward`.
     - *forward_reward*: A reward of hopping forward which is measured
     as *`forward_reward_weight` * (x-coordinate before action - x-coordinate after action)/dt*. *dt* is
@@ -292,15 +292,7 @@
             low=noise_low, high=noise_high, size=self.model.nv
         )
 
         self.set_state(qpos, qvel)
 
         observation = self._get_obs()
         return observation
-
-    def viewer_setup(self):
-        assert self.viewer is not None
-        for key, value in DEFAULT_CAMERA_CONFIG.items():
-            if isinstance(value, np.ndarray):
-                getattr(self.viewer.cam, key)[:] = value
-            else:
-                setattr(self.viewer.cam, key, value)
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/humanoid.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/humanoid.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/humanoid_v3.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/humanoid_v3.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/humanoid_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/humanoid_v4.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class HumanoidEnv(MujocoEnv, utils.EzPickle):
     """
     ## Description
 
     This environment is based on the environment introduced by Tassa, Erez and Todorov
     in ["Synthesis and stabilization of complex behaviors through online trajectory optimization"](https://ieeexplore.ieee.org/document/6386025).
     The 3D bipedal robot is designed to simulate a human. It has a torso (abdomen) with a pair of
-    legs and arms. The legs each consist of two links, and so the arms (representing the knees and
+    legs and arms. The legs each consist of three body parts, and the arms 2 body parts (representing the knees and
     elbows respectively). The goal of the environment is to walk forward as fast as possible without falling over.
 
     ## Action Space
     The action space is a `Box(-1, 1, (17,), float32)`. An action represents the torques applied at the hinge joints.
 
     | Num | Action                    | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit |
     |-----|----------------------|---------------|----------------|---------------------------------------|-------|------|
@@ -40,50 +40,49 @@
     | 3   | Torque applied on the rotor between torso/abdomen and the right hip (x-coordinate) | -0.4 | 0.4 | right_hip_x (right_thigh)   | hinge | torque (N m) |
     | 4   | Torque applied on the rotor between torso/abdomen and the right hip (z-coordinate) | -0.4 | 0.4 | right_hip_z (right_thigh)   | hinge | torque (N m) |
     | 5   | Torque applied on the rotor between torso/abdomen and the right hip (y-coordinate) | -0.4 | 0.4 | right_hip_y (right_thigh)   | hinge | torque (N m) |
     | 6   | Torque applied on the rotor between the right hip/thigh and the right shin         | -0.4 | 0.4 | right_knee                  | hinge | torque (N m) |
     | 7   | Torque applied on the rotor between torso/abdomen and the left hip (x-coordinate)  | -0.4 | 0.4 | left_hip_x (left_thigh)     | hinge | torque (N m) |
     | 8   | Torque applied on the rotor between torso/abdomen and the left hip (z-coordinate)  | -0.4 | 0.4 | left_hip_z (left_thigh)     | hinge | torque (N m) |
     | 9   | Torque applied on the rotor between torso/abdomen and the left hip (y-coordinate)  | -0.4 | 0.4 | left_hip_y (left_thigh)     | hinge | torque (N m) |
-    | 10   | Torque applied on the rotor between the left hip/thigh and the left shin          | -0.4 | 0.4 | left_knee                   | hinge | torque (N m) |
-    | 11   | Torque applied on the rotor between the torso and right upper arm (coordinate -1) | -0.4 | 0.4 | right_shoulder1             | hinge | torque (N m) |
-    | 12   | Torque applied on the rotor between the torso and right upper arm (coordinate -2) | -0.4 | 0.4 | right_shoulder2             | hinge | torque (N m) |
-    | 13   | Torque applied on the rotor between the right upper arm and right lower arm       | -0.4 | 0.4 | right_elbow                 | hinge | torque (N m) |
-    | 14   | Torque applied on the rotor between the torso and left upper arm (coordinate -1)  | -0.4 | 0.4 | left_shoulder1              | hinge | torque (N m) |
-    | 15   | Torque applied on the rotor between the torso and left upper arm (coordinate -2)  | -0.4 | 0.4 | left_shoulder2              | hinge | torque (N m) |
-    | 16   | Torque applied on the rotor between the left upper arm and left lower arm         | -0.4 | 0.4 | left_elbow                  | hinge | torque (N m) |
+    | 10  | Torque applied on the rotor between the left hip/thigh and the left shin           | -0.4 | 0.4 | left_knee                   | hinge | torque (N m) |
+    | 11  | Torque applied on the rotor between the torso and right upper arm (coordinate -1)  | -0.4 | 0.4 | right_shoulder1             | hinge | torque (N m) |
+    | 12  | Torque applied on the rotor between the torso and right upper arm (coordinate -2)  | -0.4 | 0.4 | right_shoulder2             | hinge | torque (N m) |
+    | 13  | Torque applied on the rotor between the right upper arm and right lower arm        | -0.4 | 0.4 | right_elbow                 | hinge | torque (N m) |
+    | 14  | Torque applied on the rotor between the torso and left upper arm (coordinate -1)   | -0.4 | 0.4 | left_shoulder1              | hinge | torque (N m) |
+    | 15  | Torque applied on the rotor between the torso and left upper arm (coordinate -2)   | -0.4 | 0.4 | left_shoulder2              | hinge | torque (N m) |
+    | 16  | Torque applied on the rotor between the left upper arm and left lower arm          | -0.4 | 0.4 | left_elbow                  | hinge | torque (N m) |
 
     ## Observation Space
-
     Observations consist of positional values of different body parts of the Humanoid,
-     followed by the velocities of those individual parts (their derivatives) with all the
-     positions ordered before all the velocities.
+    followed by the velocities of those individual parts (their derivatives) with all the
+    positions ordered before all the velocities.
 
     By default, observations do not include the x- and y-coordinates of the torso. These may
     be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will have 378 dimensions where the first two dimensions
+    In that case, the observation space will be a `Box(-Inf, Inf, (378,), float64)` where the first two observations
     represent the x- and y-coordinates of the torso.
     Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x- and y-coordinates
     will be returned in `info` with keys `"x_position"` and `"y_position"`, respectively.
 
-    However, by default, the observation is a `ndarray` with shape `(376,)` where the elements correspond to the following:
+    However, by default, the observation is a `Box(-Inf, Inf, (376,), float64)`. The elements correspond to the following:
 
     | Num | Observation                                                                                                     | Min  | Max | Name (in corresponding XML file) | Joint | Unit                       |
     | --- | --------------------------------------------------------------------------------------------------------------- | ---- | --- | -------------------------------- | ----- | -------------------------- |
     | 0   | z-coordinate of the torso (centre)                                                                              | -Inf | Inf | root                             | free  | position (m)               |
     | 1   | x-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 2   | y-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 3   | z-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 4   | w-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 5   | z-angle of the abdomen (in lower_waist)                                                                         | -Inf | Inf | abdomen_z                        | hinge | angle (rad)                |
     | 6   | y-angle of the abdomen (in lower_waist)                                                                         | -Inf | Inf | abdomen_y                        | hinge | angle (rad)                |
     | 7   | x-angle of the abdomen (in pelvis)                                                                              | -Inf | Inf | abdomen_x                        | hinge | angle (rad)                |
     | 8   | x-coordinate of angle between pelvis and right hip (in right_thigh)                                             | -Inf | Inf | right_hip_x                      | hinge | angle (rad)                |
     | 9   | z-coordinate of angle between pelvis and right hip (in right_thigh)                                             | -Inf | Inf | right_hip_z                      | hinge | angle (rad)                |
-    | 19  | y-coordinate of angle between pelvis and right hip (in right_thigh)                                             | -Inf | Inf | right_hip_y                      | hinge | angle (rad)                |
+    | 10  | y-coordinate of angle between pelvis and right hip (in right_thigh)                                             | -Inf | Inf | right_hip_y                      | hinge | angle (rad)                |
     | 11  | angle between right hip and the right shin (in right_knee)                                                      | -Inf | Inf | right_knee                       | hinge | angle (rad)                |
     | 12  | x-coordinate of angle between pelvis and left hip (in left_thigh)                                               | -Inf | Inf | left_hip_x                       | hinge | angle (rad)                |
     | 13  | z-coordinate of angle between pelvis and left hip (in left_thigh)                                               | -Inf | Inf | left_hip_z                       | hinge | angle (rad)                |
     | 14  | y-coordinate of angle between pelvis and left hip (in left_thigh)                                               | -Inf | Inf | left_hip_y                       | hinge | angle (rad)                |
     | 15  | angle between left hip and the left shin (in left_knee)                                                         | -Inf | Inf | left_knee                        | hinge | angle (rad)                |
     | 16  | coordinate-1 (multi-axis) angle between torso and right arm (in right_upper_arm)                                | -Inf | Inf | right_shoulder1                  | hinge | angle (rad)                |
     | 17  | coordinate-2 (multi-axis) angle between torso and right arm (in right_upper_arm)                                | -Inf | Inf | right_shoulder2                  | hinge | angle (rad)                |
@@ -109,15 +108,17 @@
     | 37  | y-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_y                       | hinge | anglular velocity (rad/s)  |
     | 38  | angular velocity of the angle between left hip and the left shin (in left_knee)                                 | -Inf | Inf | left_knee                        | hinge | anglular velocity (rad/s)  |
     | 39  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder1                  | hinge | anglular velocity (rad/s)  |
     | 40  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder2                  | hinge | anglular velocity (rad/s)  |
     | 41  | angular velocity of the angle between right upper arm and right_lower_arm                                       | -Inf | Inf | right_elbow                      | hinge | anglular velocity (rad/s)  |
     | 42  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder1                   | hinge | anglular velocity (rad/s)  |
     | 43  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder2                   | hinge | anglular velocity (rad/s)  |
-    | 44  | angular velocitty of the angle between left upper arm and left_lower_arm                                        | -Inf | Inf | left_elbow                       | hinge | anglular velocity (rad/s)  |
+    | 44  | angular velocity of the angle between left upper arm and left_lower_arm                                         | -Inf | Inf | left_elbow                       | hinge | anglular velocity (rad/s)  |
+    | excluded | x-coordinate of the torso (centre)                                                                         | -Inf | Inf | root                             | free  | position (m)               |
+    | excluded | y-coordinate of the torso (centre)                                                                         | -Inf | Inf | root                             | free  | position (m)               |
 
     Additionally, after all the positional and velocity based values in the table,
     the observation contains (in order):
     - *cinert:* Mass and inertia of a single rigid body relative to the center of mass
     (this is an intermediate result of transition). It has shape 14*10 (*nbody * 10*)
     and hence adds to another 140 elements in the state space.
     - *cvel:* Center of mass based velocity. It has shape 14 * 6 (*nbody * 6*) and hence
@@ -125,14 +126,61 @@
     - *qfrc_actuator:* Constraint force generated as the actuator force. This has shape
     `(23,)`  *(nv * 1)* and hence adds another 23 elements to the state space.
     - *cfrc_ext:* This is the center of mass based external force on the body.  It has shape
     14 * 6 (*nbody * 6*) and hence adds to another 84 elements in the state space.
     where *nbody* stands for the number of bodies in the robot and *nv* stands for the
     number of degrees of freedom (*= dim(qvel)*)
 
+    The body parts are:
+
+    | id (for `v2`,`v3`,`v4`) | body part |
+    | --- |  ------------  |
+    | 0   | worldBody (note: all values are constant 0) |
+    | 1   | torso |
+    | 2   | lwaist |
+    | 3   | pelvis |
+    | 4   | right_thigh |
+    | 5   | right_sin |
+    | 6   | right_foot |
+    | 7   | left_thigh |
+    | 8   | left_sin |
+    | 9   | left_foot |
+    | 10  | right_upper_arm |
+    | 11  | right_lower_arm |
+    | 12  | left_upper_arm |
+    | 13  | left_lower_arm |
+
+    The joints are:
+
+    | id (for `v2`,`v3`,`v4`) | joint |
+    | --- |  ------------  |
+    | 0   | root |
+    | 1   | root |
+    | 2   | root |
+    | 3   | root |
+    | 4   | root |
+    | 5   | root |
+    | 6   | abdomen_z |
+    | 7   | abdomen_y |
+    | 8   | abdomen_x |
+    | 9   | right_hip_x |
+    | 10  | right_hip_z |
+    | 11  | right_hip_y |
+    | 12  | right_knee |
+    | 13  | left_hip_x |
+    | 14  | left_hiz_z |
+    | 15  | left_hip_y |
+    | 16  | left_knee |
+    | 17  | right_shoulder1 |
+    | 18  | right_shoulder2 |
+    | 19  | right_elbow|
+    | 20  | left_shoulder1 |
+    | 21  | left_shoulder2 |
+    | 22  | left_elfbow |
+
     The (x,y,z) coordinates are translational DOFs while the orientations are rotational
     DOFs expressed as quaternions. One can read more about free joints on the
     [Mujoco Documentation](https://mujoco.readthedocs.io/en/latest/XMLreference.html).
 
     **Note:** Humanoid-v4 environment no longer has the following contact forces issue.
     If using previous Humanoid versions from v4, there have been reported issues that using a Mujoco-Py version > 2.0
     results in the contact forces always being 0. As such we recommend to use a Mujoco-Py
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/humanoidstandup.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/humanoidstandup.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/humanoidstandup_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/humanoidstandup_v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,21 +48,26 @@
     | 12  | Torque applied on the rotor between the torso and right upper arm (coordinate -2)  | -0.4        | 0.4         | right_shoulder2                  | hinge | torque (N m) |
     | 13  | Torque applied on the rotor between the right upper arm and right lower arm        | -0.4        | 0.4         | right_elbow                      | hinge | torque (N m) |
     | 14  | Torque applied on the rotor between the torso and left upper arm (coordinate -1)   | -0.4        | 0.4         | left_shoulder1                   | hinge | torque (N m) |
     | 15  | Torque applied on the rotor between the torso and left upper arm (coordinate -2)   | -0.4        | 0.4         | left_shoulder2                   | hinge | torque (N m) |
     | 16  | Torque applied on the rotor between the left upper arm and left lower arm          | -0.4        | 0.4         | left_elbow                       | hinge | torque (N m) |
 
     ## Observation Space
+    Observations consist of positional values of different body parts of the Humanoid,
+    followed by the velocities of those individual parts (their derivatives) with all the
+    positions ordered before all the velocities.
+
+    By default, observations do not include the x- and y-coordinates of the torso. These may
+    be included by passing `exclude_current_positions_from_observation=False` during construction.
+    In that case, the observation space will be a `Box(-Inf, Inf, (378,), float64)` where the first two observations
+    represent the x- and y-coordinates of the torso.
+    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x- and y-coordinates
+    will be returned in `info` with keys `"x_position"` and `"y_position"`, respectively.
 
-    The state space consists of positional values of different body parts of the Humanoid,
-    followed by the velocities of those individual parts (their derivatives) with all the positions ordered before all the velocities.
-
-    **Note:** The x- and y-coordinates of the torso are being omitted to produce position-agnostic behavior in policies
-
-    The observation is a `ndarray` with shape `(376,)` where the elements correspond to the following:
+    However, by default, the observation is a `Box(-Inf, Inf, (376,), float64)`. The elements correspond to the following:
 
     | Num | Observation                                                                                                     | Min  | Max | Name (in corresponding XML file) | Joint | Unit                       |
     | --- | --------------------------------------------------------------------------------------------------------------- | ---- | --- | -------------------------------- | ----- | -------------------------- |
     | 0   | z-coordinate of the torso (centre)                                                                              | -Inf | Inf | root                             | free  | position (m)               |
     | 1   | x-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 2   | y-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 3   | z-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
@@ -92,40 +97,88 @@
     | 27  | z-coordinate angular velocity of the torso (centre)                                                             | -Inf | Inf | root                             | free  | anglular velocity (rad/s)  |
     | 28  | z-coordinate of angular velocity of the abdomen (in lower_waist)                                                | -Inf | Inf | abdomen_z                        | hinge | anglular velocity (rad/s)  |
     | 29  | y-coordinate of angular velocity of the abdomen (in lower_waist)                                                | -Inf | Inf | abdomen_y                        | hinge | anglular velocity (rad/s)  |
     | 30  | x-coordinate of angular velocity of the abdomen (in pelvis)                                                     | -Inf | Inf | abdomen_x                        | hinge | aanglular velocity (rad/s) |
     | 31  | x-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_x                      | hinge | anglular velocity (rad/s)  |
     | 32  | z-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_z                      | hinge | anglular velocity (rad/s)  |
     | 33  | y-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_y                      | hinge | anglular velocity (rad/s)  |
-    | 35  | angular velocity of the angle between right hip and the right shin (in right_knee)                              | -Inf | Inf | right_knee                       | hinge | anglular velocity (rad/s)  |
-    | 36  | x-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_x                       | hinge | anglular velocity (rad/s)  |
-    | 37  | z-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_z                       | hinge | anglular velocity (rad/s)  |
-    | 38  | y-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_y                       | hinge | anglular velocity (rad/s)  |
-    | 39  | angular velocity of the angle between left hip and the left shin (in left_knee)                                 | -Inf | Inf | left_knee                        | hinge | anglular velocity (rad/s)  |
-    | 40  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder1                  | hinge | anglular velocity (rad/s)  |
-    | 41  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder2                  | hinge | anglular velocity (rad/s)  |
-    | 42  | angular velocity of the angle between right upper arm and right_lower_arm                                       | -Inf | Inf | right_elbow                      | hinge | anglular velocity (rad/s)  |
-    | 43  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder1                   | hinge | anglular velocity (rad/s)  |
-    | 44  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder2                   | hinge | anglular velocity (rad/s)  |
-    | 45  | angular velocity of the angle between left upper arm and left_lower_arm                                        | -Inf | Inf | left_elbow                       | hinge | anglular velocity (rad/s)  |
-
+    | 34  | angular velocity of the angle between right hip and the right shin (in right_knee)                              | -Inf | Inf | right_knee                       | hinge | anglular velocity (rad/s)  |
+    | 35  | x-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_x                       | hinge | anglular velocity (rad/s)  |
+    | 36  | z-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_z                       | hinge | anglular velocity (rad/s)  |
+    | 37  | y-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_y                       | hinge | anglular velocity (rad/s)  |
+    | 38  | angular velocity of the angle between left hip and the left shin (in left_knee)                                 | -Inf | Inf | left_knee                        | hinge | anglular velocity (rad/s)  |
+    | 39  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder1                  | hinge | anglular velocity (rad/s)  |
+    | 40  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder2                  | hinge | anglular velocity (rad/s)  |
+    | 41  | angular velocity of the angle between right upper arm and right_lower_arm                                       | -Inf | Inf | right_elbow                      | hinge | anglular velocity (rad/s)  |
+    | 42  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder1                   | hinge | anglular velocity (rad/s)  |
+    | 43  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder2                   | hinge | anglular velocity (rad/s)  |
+    | 44  | angular velocity of the angle between left upper arm and left_lower_arm                                         | -Inf | Inf | left_elbow                       | hinge | anglular velocity (rad/s)  |
+    | excluded | x-coordinate of the torso (centre)                                                                         | -Inf | Inf | root                             | free  | position (m)               |
+    | excluded | y-coordinate of the torso (centre)                                                                         | -Inf | Inf | root                             | free  | position (m)               |
 
     Additionally, after all the positional and velocity based values in the table,
-    the state_space consists of (in order):
+    the observation contains (in order):
     - *cinert:* Mass and inertia of a single rigid body relative to the center of mass
     (this is an intermediate result of transition). It has shape 14*10 (*nbody * 10*)
     and hence adds to another 140 elements in the state space.
     - *cvel:* Center of mass based velocity. It has shape 14 * 6 (*nbody * 6*) and hence
     adds another 84 elements in the state space
     - *qfrc_actuator:* Constraint force generated as the actuator force. This has shape
     `(23,)`  *(nv * 1)* and hence adds another 23 elements to the state space.
     - *cfrc_ext:* This is the center of mass based external force on the body.  It has shape
     14 * 6 (*nbody * 6*) and hence adds to another 84 elements in the state space.
-    where *nbody* stands for the number of bodies in the robot and *nv* stands for the number
-    of degrees of freedom (*= dim(qvel)*)
+    where *nbody* stands for the number of bodies in the robot and *nv* stands for the
+    number of degrees of freedom (*= dim(qvel)*)
+
+    The body parts are:
+
+    | id (for `v2`,`v3`,`v4`) | body part |
+    | --- |  ------------  |
+    | 0   | worldBody (note: all values are constant 0) |
+    | 1   | torso |
+    | 2   | lwaist |
+    | 3   | pelvis |
+    | 4   | right_thigh |
+    | 5   | right_sin |
+    | 6   | right_foot |
+    | 7   | left_thigh |
+    | 8   | left_sin |
+    | 9   | left_foot |
+    | 10  | right_upper_arm |
+    | 11  | right_lower_arm |
+    | 12  | left_upper_arm |
+    | 13  | left_lower_arm |
+
+    The joints are:
+
+    | id (for `v2`,`v3`,`v4`) | joint |
+    | --- |  ------------  |
+    | 0   | root |
+    | 1   | root |
+    | 2   | root |
+    | 3   | root |
+    | 4   | root |
+    | 5   | root |
+    | 6   | abdomen_z |
+    | 7   | abdomen_y |
+    | 8   | abdomen_x |
+    | 9   | right_hip_x |
+    | 10  | right_hip_z |
+    | 11  | right_hip_y |
+    | 12  | right_knee |
+    | 13  | left_hip_x |
+    | 14  | left_hiz_z |
+    | 15  | left_hip_y |
+    | 16  | left_knee |
+    | 17  | right_shoulder1 |
+    | 18  | right_shoulder2 |
+    | 19  | right_elbow|
+    | 20  | left_shoulder1 |
+    | 21  | left_shoulder2 |
+    | 22  | left_elfbow |
 
     The (x,y,z) coordinates are translational DOFs while the orientations are rotational
     DOFs expressed as quaternions. One can read more about free joints on the
     [Mujoco Documentation](https://mujoco.readthedocs.io/en/latest/XMLreference.html).
 
     **Note:** HumanoidStandup-v4 environment no longer has the following contact forces issue.
     If using previous HumanoidStandup versions from v4, there have been reported issues that using a Mujoco-Py version > 2.0 results
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/inverted_double_pendulum.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/inverted_double_pendulum.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/inverted_double_pendulum_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/inverted_double_pendulum_v4.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/inverted_pendulum.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/inverted_pendulum.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/inverted_pendulum_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/inverted_pendulum_v4.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/mujoco_env.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/mujoco_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from os import path
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
+from numpy.typing import NDArray
 
 import gymnasium as gym
 from gymnasium import error, logger, spaces
 from gymnasium.spaces import Space
 
 
 try:
@@ -22,52 +23,72 @@
 else:
     MUJOCO_IMPORT_ERROR = None
 
 
 DEFAULT_SIZE = 480
 
 
-class BaseMujocoEnv(gym.Env):
+class BaseMujocoEnv(gym.Env[np.float64, np.float32]):
     """Superclass for all MuJoCo environments."""
 
     def __init__(
         self,
         model_path,
         frame_skip,
         observation_space: Space,
         render_mode: Optional[str] = None,
         width: int = DEFAULT_SIZE,
         height: int = DEFAULT_SIZE,
         camera_id: Optional[int] = None,
         camera_name: Optional[str] = None,
     ):
-        if model_path.startswith("/"):
+        """Base abstract class for mujoco based environments.
+
+        Args:
+            model_path: Path to the MuJoCo Model.
+            frame_skip: Number of MuJoCo simulation steps per gym `step()`.
+            observation_space: The observation space of the environment.
+            render_mode: The `render_mode` used.
+            width: The width of the render window.
+            height: The height of the render window.
+            camera_id: The camera ID used.
+            camera_name: The name of the camera used (can not be used in conjunction with `camera_id`).
+
+        Raises:
+            OSError: when the `model_path` does not exist.
+            error.DependencyNotInstalled: When `mujoco` is not installed.
+        """
+        if model_path.startswith(".") or model_path.startswith("/"):
             self.fullpath = model_path
+        elif model_path.startswith("~"):
+            self.fullpath = path.expanduser(model_path)
         else:
             self.fullpath = path.join(path.dirname(__file__), "assets", model_path)
         if not path.exists(self.fullpath):
             raise OSError(f"File {self.fullpath} does not exist")
 
         self.width = width
         self.height = height
-        self._initialize_simulation()  # may use width and height
+        # may use width and height
+        self.model, self.data = self._initialize_simulation()
 
         self.init_qpos = self.data.qpos.ravel().copy()
         self.init_qvel = self.data.qvel.ravel().copy()
 
         self.frame_skip = frame_skip
 
         assert self.metadata["render_modes"] == [
             "human",
             "rgb_array",
             "depth_array",
         ], self.metadata["render_modes"]
-        assert (
-            int(np.round(1.0 / self.dt)) == self.metadata["render_fps"]
-        ), f'Expected value: {int(np.round(1.0 / self.dt))}, Actual value: {self.metadata["render_fps"]}'
+        if "render_fps" in self.metadata:
+            assert (
+                int(np.round(1.0 / self.dt)) == self.metadata["render_fps"]
+            ), f'Expected value: {int(np.round(1.0 / self.dt))}, Actual value: {self.metadata["render_fps"]}'
 
         self.observation_space = observation_space
         self._set_action_space()
 
         self.render_mode = render_mode
         self.camera_name = camera_name
         self.camera_id = camera_id
@@ -77,92 +98,97 @@
         low, high = bounds.T
         self.action_space = spaces.Box(low=low, high=high, dtype=np.float32)
         return self.action_space
 
     # methods to override:
     # ----------------------------
 
-    def reset_model(self):
+    def reset_model(self) -> NDArray[np.float64]:
         """
         Reset the robot degrees of freedom (qpos and qvel).
         Implement this in each subclass.
         """
         raise NotImplementedError
 
-    def _initialize_simulation(self):
+    def _initialize_simulation(self) -> Tuple[Any, Any]:
         """
         Initialize MuJoCo simulation data structures mjModel and mjData.
         """
         raise NotImplementedError
 
-    def _reset_simulation(self):
+    def _reset_simulation(self) -> None:
         """
         Reset MuJoCo simulation data structures, mjModel and mjData.
         """
         raise NotImplementedError
 
-    def _step_mujoco_simulation(self, ctrl, n_frames):
+    def _step_mujoco_simulation(self, ctrl, n_frames) -> None:
         """
         Step over the MuJoCo simulation.
         """
         raise NotImplementedError
 
-    def render(self):
+    def render(self) -> Union[NDArray[np.float64], None]:
         """
         Render a frame from the MuJoCo simulation as specified by the render_mode.
         """
         raise NotImplementedError
 
     # -----------------------------
+    def _get_reset_info(self) -> Dict[str, float]:
+        """Function that generates the `info` that is returned during a `reset()`."""
+        return {}
 
     def reset(
         self,
         *,
         seed: Optional[int] = None,
         options: Optional[dict] = None,
     ):
         super().reset(seed=seed)
 
         self._reset_simulation()
 
         ob = self.reset_model()
+        info = self._get_reset_info()
+
         if self.render_mode == "human":
             self.render()
-        return ob, {}
+        return ob, info
 
-    def set_state(self, qpos, qvel):
+    def set_state(self, qpos, qvel) -> None:
         """
         Set the joints position qpos and velocity qvel of the model. Override this method depending on the MuJoCo bindings used.
         """
         assert qpos.shape == (self.model.nq,) and qvel.shape == (self.model.nv,)
 
     @property
-    def dt(self):
+    def dt(self) -> float:
         return self.model.opt.timestep * self.frame_skip
 
-    def do_simulation(self, ctrl, n_frames):
+    def do_simulation(self, ctrl, n_frames) -> None:
         """
         Step the simulation n number of frames and applying a control action.
         """
         # Check control input is contained in the action space
-        if np.array(ctrl).shape != self.action_space.shape:
+        if np.array(ctrl).shape != (self.model.nu,):
             raise ValueError(
-                f"Action dimension mismatch. Expected {self.action_space.shape}, found {np.array(ctrl).shape}"
+                f"Action dimension mismatch. Expected {(self.model.nu,)}, found {np.array(ctrl).shape}"
             )
         self._step_mujoco_simulation(ctrl, n_frames)
 
     def close(self):
         """Close all processes like rendering contexts"""
         raise NotImplementedError
 
-    def get_body_com(self, body_name):
+    def get_body_com(self, body_name) -> NDArray[np.float64]:
         """Return the cartesian position of a body frame"""
         raise NotImplementedError
 
-    def state_vector(self):
+    def state_vector(self) -> NDArray[np.float64]:
         """Return the position and velocity joint states of the model"""
         return np.concatenate([self.data.qpos.flat, self.data.qvel.flat])
 
 
 class MuJocoPyEnv(BaseMujocoEnv):
     def __init__(
         self,
@@ -201,17 +227,18 @@
             width,
             height,
             camera_id,
             camera_name,
         )
 
     def _initialize_simulation(self):
-        self.model = mujoco_py.load_model_from_path(self.fullpath)
-        self.sim = mujoco_py.MjSim(self.model)
-        self.data = self.sim.data
+        model = mujoco_py.load_model_from_path(self.fullpath)
+        self.sim = mujoco_py.MjSim(model)
+        data = self.sim.data
+        return model, data
 
     def _reset_simulation(self):
         self.sim.reset()
 
     def set_state(self, qpos, qvel):
         super().set_state(qpos, qvel)
         state = self.sim.get_state()
@@ -343,20 +370,23 @@
 
         from gymnasium.envs.mujoco.mujoco_rendering import MujocoRenderer
 
         self.mujoco_renderer = MujocoRenderer(
             self.model, self.data, default_camera_config
         )
 
-    def _initialize_simulation(self):
-        self.model = mujoco.MjModel.from_xml_path(self.fullpath)
+    def _initialize_simulation(
+        self,
+    ):
+        model = mujoco.MjModel.from_xml_path(self.fullpath)
         # MjrContext will copy model.vis.global_.off* to con.off*
-        self.model.vis.global_.offwidth = self.width
-        self.model.vis.global_.offheight = self.height
-        self.data = mujoco.MjData(self.model)
+        model.vis.global_.offwidth = self.width
+        model.vis.global_.offheight = self.height
+        data = mujoco.MjData(model)
+        return model, data
 
     def _reset_simulation(self):
         mujoco.mj_resetData(self.model, self.data)
 
     def set_state(self, qpos, qvel):
         super().set_state(qpos, qvel)
         self.data.qpos[:] = np.copy(qpos)
@@ -364,15 +394,15 @@
         if self.model.na == 0:
             self.data.act[:] = None
         mujoco.mj_forward(self.model, self.data)
 
     def _step_mujoco_simulation(self, ctrl, n_frames):
         self.data.ctrl[:] = ctrl
 
-        mujoco.mj_step(self.model, self.data, nstep=self.frame_skip)
+        mujoco.mj_step(self.model, self.data, nstep=n_frames)
 
         # As of MuJoCo 2.0, force-related quantities like cacc are not computed
         # unless there's a force sensor in the model.
         # See https://github.com/openai/gym/issues/1541
         mujoco.mj_rnePostConstraint(self.model, self.data)
 
     def render(self):
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/mujoco_rendering.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/mujoco_rendering.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,16 +323,16 @@
     def make_context_current(self):
         glfw.make_context_current(self.window)
 
     def free(self):
         if self.window:
             if glfw.get_current_context() == self.window:
                 glfw.make_context_current(None)
-        glfw.destroy_window(self.window)
-        self.window = None
+            glfw.destroy_window(self.window)
+            self.window = None
 
     def __del__(self):
         """Eliminate all of the OpenGL glfw contexts and windows"""
         self.free()
 
     def render(self):
         """
@@ -599,15 +599,15 @@
 
 
 class MujocoRenderer:
     """This is the MuJoCo renderer manager class for every MuJoCo environment.
 
     The class has two main public methods available:
     - :meth:`render` - Renders the environment in three possible modes: "human", "rgb_array", or "depth_array"
-    - :meth:`close` - Closes all contexts initialized with the rendere
+    - :meth:`close` - Closes all contexts initialized with the renderer
 
     """
 
     def __init__(
         self,
         model: "mujoco.MjModel",
         data: "mujoco.MjData",
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/pusher.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/pusher.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/pusher_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/pusher_v4.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     - Angle of rotational joints on the pusher
     - Angular velocities of rotational joints on the pusher
     - The coordinates of the fingertip of the pusher
     - The coordinates of the object to be moved
     - The coordinates of the goal position
 
-    The observation is a `ndarray` with shape `(23,)` where the elements correspond to the table below.
+    The observation is a `Box(-Inf, Inf, (23,), float64)` where the elements correspond to the table below.
     An analogy can be drawn to a human arm in order to help understand the state space, with the words flex and roll meaning the
     same as human joints.
 
     | Num | Observation                                              | Min  | Max | Name (in corresponding XML file) | Joint    | Unit                     |
     | --- | -------------------------------------------------------- | ---- | --- | -------------------------------- | -------- | ------------------------ |
     | 0   | Rotation of the panning the shoulder                     | -Inf | Inf | r_shoulder_pan_joint             | hinge    | angle (rad)              |
     | 1   | Rotation of the shoulder lifting joint                   | -Inf | Inf | r_shoulder_lift_joint            | hinge    | angle (rad)              |
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/reacher.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/reacher.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/reacher_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/reacher_v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,33 +19,32 @@
 
     | Num | Action                                                                          | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit |
     |-----|---------------------------------------------------------------------------------|-------------|-------------|--------------------------|-------|------|
     | 0   | Torque applied at the first hinge (connecting the link to the point of fixture) | -1 | 1 | joint0  | hinge | torque (N m) |
     | 1   |  Torque applied at the second hinge (connecting the two links)                  | -1 | 1 | joint1  | hinge | torque (N m) |
 
     ## Observation Space
-
     Observations consist of
 
     - The cosine of the angles of the two arms
     - The sine of the angles of the two arms
     - The coordinates of the target
     - The angular velocities of the arms
     - The vector between the target and the reacher's fingertip (3 dimensional with the last element being 0)
 
-    The observation is a `ndarray` with shape `(11,)` where the elements correspond to the following:
+    The observation is a `Box(-Inf, Inf, (11,), float64)` where the elements correspond to the following:
 
     | Num | Observation                                                                                    | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
     | --- | ---------------------------------------------------------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------ |
     | 0   | cosine of the angle of the first arm                                                           | -Inf | Inf | cos(joint0)                      | hinge | unitless                 |
     | 1   | cosine of the angle of the second arm                                                          | -Inf | Inf | cos(joint1)                      | hinge | unitless                 |
     | 2   | sine of the angle of the first arm                                                             | -Inf | Inf | sin(joint0)                      | hinge | unitless                 |
     | 3   | sine of the angle of the second arm                                                            | -Inf | Inf | sin(joint1)                      | hinge | unitless                 |
-    | 4   | x-coordinate of the target                                                                    | -Inf | Inf | target_x                         | slide | position (m)             |
-    | 5   | y-coordinate of the target                                                                    | -Inf | Inf | target_y                         | slide | position (m)             |
+    | 4   | x-coordinate of the target                                                                     | -Inf | Inf | target_x                         | slide | position (m)             |
+    | 5   | y-coordinate of the target                                                                     | -Inf | Inf | target_y                         | slide | position (m)             |
     | 6   | angular velocity of the first arm                                                              | -Inf | Inf | joint0                           | hinge | angular velocity (rad/s) |
     | 7   | angular velocity of the second arm                                                             | -Inf | Inf | joint1                           | hinge | angular velocity (rad/s) |
     | 8   | x-value of position_fingertip - position_target                                                | -Inf | Inf | NA                               | slide | position (m)             |
     | 9   | y-value of position_fingertip - position_target                                                | -Inf | Inf | NA                               | slide | position (m)             |
     | 10  | z-value of position_fingertip - position_target (constantly 0 since reacher is 2d and z is same for both) | -Inf | Inf | NA                               | slide | position (m)             |
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/swimmer.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/swimmer.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/swimmer_v3.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/swimmer_v3.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/swimmer_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/swimmer_v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,38 +40,39 @@
 
     | Num | Action                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
     |-----|------------------------------------|-------------|-------------|----------------------------------|-------|--------------|
     | 0   | Torque applied on the first rotor  | -1          | 1           | motor1_rot                       | hinge | torque (N m) |
     | 1   | Torque applied on the second rotor | -1          | 1           | motor2_rot                       | hinge | torque (N m) |
 
     ## Observation Space
-
     By default, observations consists of:
     * θ<sub>i</sub>: angle of part *i* with respect to the *x* axis
     * θ<sub>i</sub>': its derivative with respect to time (angular velocity)
 
     In the default case, observations do not include the x- and y-coordinates of the front tip. These may
     be included by passing `exclude_current_positions_from_observation=False` during construction.
-    Then, the observation space will have 10 dimensions where the first two dimensions
+    Then, the observation space will be `Box(-Inf, Inf, (10,), float64)` where the first two observations
     represent the x- and y-coordinates of the front tip.
     Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x- and y-coordinates
     will be returned in `info` with keys `"x_position"` and `"y_position"`, respectively.
 
-    By default, the observation is a `ndarray` with shape `(8,)` where the elements correspond to the following:
+    By default, the observation is a `Box(-Inf, Inf, (8,), float64)` where the elements correspond to the following:
 
     | Num | Observation                          | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
     | --- | ------------------------------------ | ---- | --- | -------------------------------- | ----- | ------------------------ |
     | 0   | angle of the front tip               | -Inf | Inf | free_body_rot                    | hinge | angle (rad)              |
     | 1   | angle of the first rotor             | -Inf | Inf | motor1_rot                       | hinge | angle (rad)              |
     | 2   | angle of the second rotor            | -Inf | Inf | motor2_rot                       | hinge | angle (rad)              |
     | 3   | velocity of the tip along the x-axis | -Inf | Inf | slider1                          | slide | velocity (m/s)           |
     | 4   | velocity of the tip along the y-axis | -Inf | Inf | slider2                          | slide | velocity (m/s)           |
     | 5   | angular velocity of front tip        | -Inf | Inf | free_body_rot                    | hinge | angular velocity (rad/s) |
     | 6   | angular velocity of first rotor      | -Inf | Inf | motor1_rot                       | hinge | angular velocity (rad/s) |
-    | 7   | angular velocity of second rotor     | -Inf | Inf | motor2_rot                             | hinge | angular velocity (rad/s) |
+    | 7   | angular velocity of second rotor     | -Inf | Inf | motor2_rot                       | hinge | angular velocity (rad/s) |
+    | excluded | position of the tip along the x-axis | -Inf | Inf | slider1                          | slide | position (m)           |
+    | excluded | position of the tip along the y-axis | -Inf | Inf | slider2                          | slide | position (m)           |
 
     ## Rewards
     The reward consists of two parts:
     - *forward_reward*: A reward of moving forward which is measured
     as *`forward_reward_weight` * (x-coordinate before action - x-coordinate after action)/dt*. *dt* is
     the time between actions and is dependent on the frame_skip parameter
     (default is 4), where the frametime is 0.01 - making the
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/walker2d.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/walker2d.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/walker2d_v3.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/walker2d_v3.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/mujoco/walker2d_v4.py` & `gymnasium-0.29.0/gymnasium/envs/mujoco/walker2d_v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,78 +13,78 @@
 }
 
 
 class Walker2dEnv(MujocoEnv, utils.EzPickle):
     """
     ## Description
 
-    This environment builds on the hopper environment based on the work done by Erez, Tassa, and Todorov
-    in ["Infinite Horizon Model Predictive Control for Nonlinear Periodic Tasks"](http://www.roboticsproceedings.org/rss07/p10.pdf)
-    by adding another set of legs making it possible for the robot to walker forward instead of
+    This environment builds on the [hopper](https://gymnasium.farama.org/environments/mujoco/hopper/) environment
+    by adding another set of legs making it possible for the robot to walk forward instead of
     hop. Like other Mujoco environments, this environment aims to increase the number of independent state
     and control variables as compared to the classic control environments. The walker is a
-    two-dimensional two-legged figure that consist of four main body parts - a single torso at the top
+    two-dimensional two-legged figure that consist of seven main body parts - a single torso at the top
     (with the two legs splitting after the torso), two thighs in the middle below the torso, two legs
     in the bottom below the thighs, and two feet attached to the legs on which the entire body rests.
-    The goal is to make coordinate both sets of feet, legs, and thighs to move in the forward (right)
-    direction by applying torques on the six hinges connecting the six body parts.
+    The goal is to walk in the in the forward (right)
+    direction by applying torques on the six hinges connecting the seven body parts.
 
     ## Action Space
     The action space is a `Box(-1, 1, (6,), float32)`. An action represents the torques applied at the hinge joints.
 
     | Num | Action                                 | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
     |-----|----------------------------------------|-------------|-------------|----------------------------------|-------|--------------|
     | 0   | Torque applied on the thigh rotor      | -1          | 1           | thigh_joint                      | hinge | torque (N m) |
     | 1   | Torque applied on the leg rotor        | -1          | 1           | leg_joint                        | hinge | torque (N m) |
     | 2   | Torque applied on the foot rotor       | -1          | 1           | foot_joint                       | hinge | torque (N m) |
     | 3   | Torque applied on the left thigh rotor | -1          | 1           | thigh_left_joint                 | hinge | torque (N m) |
     | 4   | Torque applied on the left leg rotor   | -1          | 1           | leg_left_joint                   | hinge | torque (N m) |
     | 5   | Torque applied on the left foot rotor  | -1          | 1           | foot_left_joint                  | hinge | torque (N m) |
 
     ## Observation Space
-
     Observations consist of positional values of different body parts of the walker,
     followed by the velocities of those individual parts (their derivatives) with all the positions ordered before all the velocities.
 
-    By default, observations do not include the x-coordinate of the top. It may
+    By default, observations do not include the x-coordinate of the torso. It may
     be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will have 18 dimensions where the first dimension
-    represent the x-coordinates of the top of the walker.
+    In that case, the observation space will be `Box(-Inf, Inf, (18,), float64)` where the first observation
+    represent the x-coordinates of the torso of the walker.
     Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x-coordinate
-    of the top will be returned in `info` with key `"x_position"`.
+    of the torso will be returned in `info` with key `"x_position"`.
+
+    By default, observation is a `Box(-Inf, Inf, (17,), float64)` where the elements correspond to the following:
 
-    By default, observation is a `ndarray` with shape `(17,)` where the elements correspond to the following:
+    | Num | Observation                                        | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
+    | --- | -------------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------ |
+    | excluded | x-coordinate of the torso                     | -Inf | Inf | rootx                            | slide | position (m)             |
+    | 0   | z-coordinate of the torso (height of Walker2d)     | -Inf | Inf | rootz                            | slide | position (m)             |
+    | 1   | angle of the torso                                 | -Inf | Inf | rooty                            | hinge | angle (rad)              |
+    | 2   | angle of the thigh joint                           | -Inf | Inf | thigh_joint                      | hinge | angle (rad)              |
+    | 3   | angle of the leg joint                             | -Inf | Inf | leg_joint                        | hinge | angle (rad)              |
+    | 4   | angle of the foot joint                            | -Inf | Inf | foot_joint                       | hinge | angle (rad)              |
+    | 5   | angle of the left thigh joint                      | -Inf | Inf | thigh_left_joint                 | hinge | angle (rad)              |
+    | 6   | angle of the left leg joint                        | -Inf | Inf | leg_left_joint                   | hinge | angle (rad)              |
+    | 7   | angle of the left foot joint                       | -Inf | Inf | foot_left_joint                  | hinge | angle (rad)              |
+    | 8   | velocity of the x-coordinate of the torso          | -Inf | Inf | rootx                            | slide | velocity (m/s)           |
+    | 9   | velocity of the z-coordinate (height) of the torso | -Inf | Inf | rootz                            | slide | velocity (m/s)           |
+    | 10  | angular velocity of the angle of the torso         | -Inf | Inf | rooty                            | hinge | angular velocity (rad/s) |
+    | 11  | angular velocity of the thigh hinge                | -Inf | Inf | thigh_joint                      | hinge | angular velocity (rad/s) |
+    | 12  | angular velocity of the leg hinge                  | -Inf | Inf | leg_joint                        | hinge | angular velocity (rad/s) |
+    | 13  | angular velocity of the foot hinge                 | -Inf | Inf | foot_joint                       | hinge | angular velocity (rad/s) |
+    | 14  | angular velocity of the thigh hinge                | -Inf | Inf | thigh_left_joint                 | hinge | angular velocity (rad/s) |
+    | 15  | angular velocity of the leg hinge                  | -Inf | Inf | leg_left_joint                   | hinge | angular velocity (rad/s) |
+    | 16  | angular velocity of the foot hinge                 | -Inf | Inf | foot_left_joint                  | hinge | angular velocity (rad/s) |
 
-    | Num | Observation                                      | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
-    | --- | ------------------------------------------------ | ---- | --- | -------------------------------- | ----- | ------------------------ |
-    | 0   | z-coordinate of the top (height of hopper)       | -Inf | Inf | rootz (torso)                    | slide | position (m)             |
-    | 1   | angle of the top                                 | -Inf | Inf | rooty (torso)                    | hinge | angle (rad)              |
-    | 2   | angle of the thigh joint                         | -Inf | Inf | thigh_joint                      | hinge | angle (rad)              |
-    | 3   | angle of the leg joint                           | -Inf | Inf | leg_joint                        | hinge | angle (rad)              |
-    | 4   | angle of the foot joint                          | -Inf | Inf | foot_joint                       | hinge | angle (rad)              |
-    | 5   | angle of the left thigh joint                    | -Inf | Inf | thigh_left_joint                 | hinge | angle (rad)              |
-    | 6   | angle of the left leg joint                      | -Inf | Inf | leg_left_joint                   | hinge | angle (rad)              |
-    | 7   | angle of the left foot joint                     | -Inf | Inf | foot_left_joint                  | hinge | angle (rad)              |
-    | 8   | velocity of the x-coordinate of the top          | -Inf | Inf | rootx                            | slide | velocity (m/s)           |
-    | 9   | velocity of the z-coordinate (height) of the top | -Inf | Inf | rootz                            | slide | velocity (m/s)           |
-    | 10  | angular velocity of the angle of the top         | -Inf | Inf | rooty                            | hinge | angular velocity (rad/s) |
-    | 11  | angular velocity of the thigh hinge              | -Inf | Inf | thigh_joint                      | hinge | angular velocity (rad/s) |
-    | 12  | angular velocity of the leg hinge                | -Inf | Inf | leg_joint                        | hinge | angular velocity (rad/s) |
-    | 13  | angular velocity of the foot hinge               | -Inf | Inf | foot_joint                       | hinge | angular velocity (rad/s) |
-    | 14  | angular velocity of the thigh hinge              | -Inf | Inf | thigh_left_joint                 | hinge | angular velocity (rad/s) |
-    | 15  | angular velocity of the leg hinge                | -Inf | Inf | leg_left_joint                   | hinge | angular velocity (rad/s) |
-    | 16  | angular velocity of the foot hinge               | -Inf | Inf | foot_left_joint                  | hinge | angular velocity (rad/s) |
     ## Rewards
     The reward consists of three parts:
     - *healthy_reward*: Every timestep that the walker is alive, it receives a fixed reward of value `healthy_reward`,
     - *forward_reward*: A reward of walking forward which is measured as
     *`forward_reward_weight` * (x-coordinate before action - x-coordinate after action)/dt*.
     *dt* is the time between actions and is dependeent on the frame_skip parameter
     (default is 4), where the frametime is 0.002 - making the default
-    *dt = 4 * 0.002 = 0.008*. This reward would be positive if the walker walks forward (right) desired.
+    *dt = 4 * 0.002 = 0.008*. This reward would be positive if the walker walks forward (positive x direction).
     - *ctrl_cost*: A cost for penalising the walker if it
     takes actions that are too large. It is measured as
     *`ctrl_cost_weight` * sum(action<sup>2</sup>)* where *`ctrl_cost_weight`* is
     a parameter set for the control and has a default value of 0.001
 
     The total reward returned is ***reward*** *=* *healthy_reward bonus + forward_reward - ctrl_cost* and `info` will also contain the individual reward terms
 
@@ -127,15 +127,15 @@
     | Parameter                                    | Type      | Default          | Description                                                                                                                                                       |
     | -------------------------------------------- | --------- | ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
     | `xml_file`                                   | **str**   | `"walker2d.xml"` | Path to a MuJoCo model                                                                                                                                            |
     | `forward_reward_weight`                      | **float** | `1.0`            | Weight for _forward_reward_ term (see section on reward)                                                                                                          |
     | `ctrl_cost_weight`                           | **float** | `1e-3`           | Weight for _ctr_cost_ term (see section on reward)                                                                                                                |
     | `healthy_reward`                             | **float** | `1.0`            | Constant reward given if the ant is "healthy" after timestep                                                                                                      |
     | `terminate_when_unhealthy`                   | **bool**  | `True`           | If true, issue a done signal if the z-coordinate of the walker is no longer healthy                                                                               |
-    | `healthy_z_range`                            | **tuple** | `(0.8, 2)`       | The z-coordinate of the top of the walker must be in this range to be considered healthy                                                                          |
+    | `healthy_z_range`                            | **tuple** | `(0.8, 2)`       | The z-coordinate of the torso of the walker must be in this range to be considered healthy                                                                        |
     | `healthy_angle_range`                        | **tuple** | `(-1, 1)`        | The angle must be in this range to be considered healthy                                                                                                          |
     | `reset_noise_scale`                          | **float** | `5e-3`           | Scale of random perturbations of initial position and velocity (see section on Starting State)                                                                    |
     | `exclude_current_positions_from_observation` | **bool**  | `True`           | Whether or not to omit the x-coordinate from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies |
 
 
     ## Version History
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/phys2d/cartpole.py` & `gymnasium-0.29.0/gymnasium/envs/phys2d/cartpole.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from gymnasium.utils import EzPickle
 
 
 RenderStateType = Tuple["pygame.Surface", "pygame.time.Clock"]  # type: ignore  # noqa: F821
 
 
 class CartPoleFunctional(
-    FuncEnv[jnp.ndarray, jnp.ndarray, int, float, bool, RenderStateType]
+    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType]
 ):
     """Cartpole but in jax and functional.
 
     Example:
         >>> import jax
         >>> import jax.numpy as jnp
         >>> from gymnasium.envs.phys2d.cartpole import CartPoleFunctional
@@ -91,15 +91,15 @@
     def initial(self, rng: PRNGKey):
         """Initial state generation."""
         return jax.random.uniform(
             key=rng, minval=-self.x_init, maxval=self.x_init, shape=(4,)
         )
 
     def transition(
-        self, state: jnp.ndarray, action: int | jnp.ndarray, rng: None = None
+        self, state: jax.Array, action: int | jax.Array, rng: None = None
     ) -> StateType:
         """Cartpole transition."""
         x, x_dot, theta, theta_dot = state
         force = jnp.sign(action - 0.5) * self.force_mag
         costheta = jnp.cos(theta)
         sintheta = jnp.sin(theta)
 
@@ -118,34 +118,34 @@
         theta = theta + self.tau * theta_dot
         theta_dot = theta_dot + self.tau * thetaacc
 
         state = jnp.array((x, x_dot, theta, theta_dot), dtype=jnp.float32)
 
         return state
 
-    def observation(self, state: jnp.ndarray) -> jnp.ndarray:
+    def observation(self, state: jax.Array) -> jax.Array:
         """Cartpole observation."""
         return state
 
-    def terminal(self, state: jnp.ndarray) -> jnp.ndarray:
+    def terminal(self, state: jax.Array) -> jax.Array:
         """Checks if the state is terminal."""
         x, _, theta, _ = state
 
         terminated = (
             (x < -self.x_threshold)
             | (x > self.x_threshold)
             | (theta < -self.theta_threshold_radians)
             | (theta > self.theta_threshold_radians)
         )
 
         return terminated
 
     def reward(
         self, state: StateType, action: ActType, next_state: StateType
-    ) -> jnp.ndarray:
+    ) -> jax.Array:
         """Computes the reward for the state transition using the action."""
         x, _, theta, _ = state
 
         terminated = (
             (x < -self.x_threshold)
             | (x > self.x_threshold)
             | (theta < -self.theta_threshold_radians)
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/phys2d/pendulum.py` & `gymnasium-0.29.0/gymnasium/envs/phys2d/pendulum.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gymnasium.utils import EzPickle
 
 
 RenderStateType = Tuple["pygame.Surface", "pygame.time.Clock", Optional[float]]  # type: ignore  # noqa: F821
 
 
 class PendulumFunctional(
-    FuncEnv[jnp.ndarray, jnp.ndarray, int, float, bool, RenderStateType]
+    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType]
 ):
     """Pendulum but in jax and functional structure."""
 
     max_speed = 8
     max_torque = 2.0
     dt = 0.05
     g = 10.0
@@ -43,16 +43,16 @@
 
     def initial(self, rng: PRNGKey):
         """Initial state generation."""
         high = jnp.array([self.high_x, self.high_y])
         return jax.random.uniform(key=rng, minval=-high, maxval=high, shape=high.shape)
 
     def transition(
-        self, state: jnp.ndarray, action: int | jnp.ndarray, rng: None = None
-    ) -> jnp.ndarray:
+        self, state: jax.Array, action: int | jax.Array, rng: None = None
+    ) -> jax.Array:
         """Pendulum transition."""
         th, thdot = state  # th := theta
         u = action
 
         g = self.g
         m = self.m
         l = self.l
@@ -63,15 +63,15 @@
         newthdot = thdot + (3 * g / (2 * l) * jnp.sin(th) + 3.0 / (m * l**2) * u) * dt
         newthdot = jnp.clip(newthdot, -self.max_speed, self.max_speed)
         newth = th + newthdot * dt
 
         new_state = jnp.array([newth, newthdot])
         return new_state
 
-    def observation(self, state: jnp.ndarray) -> jnp.ndarray:
+    def observation(self, state: jax.Array) -> jax.Array:
         """Generates an observation based on the state."""
         theta, thetadot = state
         return jnp.array([jnp.cos(theta), jnp.sin(theta), thetadot])
 
     def reward(self, state: StateType, action: ActType, next_state: StateType) -> float:
         """Generates the reward based on the state, action and next state."""
         th, thdot = state  # th := theta
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/registration.py` & `gymnasium-0.29.0/gymnasium/envs/registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,38 +9,27 @@
 import importlib.util
 import json
 import re
 import sys
 import traceback
 from collections import defaultdict
 from dataclasses import dataclass, field
+from types import ModuleType
 from typing import Any, Callable, Iterable, Sequence
 
+import gymnasium as gym
 from gymnasium import Env, Wrapper, error, logger
-from gymnasium.experimental.vector import AsyncVectorEnv, SyncVectorEnv, VectorEnv
-from gymnasium.wrappers import (
-    AutoResetWrapper,
-    EnvCompatibility,
-    HumanRendering,
-    OrderEnforcing,
-    PassiveEnvChecker,
-    RenderCollection,
-    TimeLimit,
-)
 
 
 if sys.version_info < (3, 10):
     import importlib_metadata as metadata  # type: ignore
 else:
     import importlib.metadata as metadata
 
-if sys.version_info < (3, 8):
-    from typing_extensions import Protocol
-else:
-    from typing import Protocol
+from typing import Protocol
 
 
 ENV_ID_RE = re.compile(
     r"^(?:(?P<namespace>[\w:-]+)\/)?(?:(?P<name>[\w:.-]+?))(?:-v(?P<version>\d+))?$"
 )
 
 
@@ -51,28 +40,29 @@
     "WrapperSpec",
     # Functions
     "register",
     "make",
     "make_vec",
     "spec",
     "pprint_registry",
+    "register_envs",
 ]
 
 
 class EnvCreator(Protocol):
     """Function type expected for an environment."""
 
     def __call__(self, **kwargs: Any) -> Env:
         ...
 
 
 class VectorEnvCreator(Protocol):
     """Function type expected for an environment."""
 
-    def __call__(self, **kwargs: Any) -> VectorEnv:
+    def __call__(self, **kwargs: Any) -> gym.experimental.vector.VectorEnv:
         ...
 
 
 @dataclass
 class WrapperSpec:
     """A specification for recording wrapper configs.
 
@@ -531,15 +521,17 @@
         logger.warn(
             f"Using the latest versioned environment `{new_env_id}` "
             f"instead of the unversioned environment `{env_name}`."
         )
 
     if env_spec is None:
         _check_version_exists(ns, name, version)
-        raise error.Error(f"No registered env with id: {env_name}")
+        raise error.Error(
+            f"No registered env with id: {env_name}. Did you register it, or import the package that registers it? Use `gymnasium.pprint_registry()` to see all of the registered environments."
+        )
 
     return env_spec
 
 
 def load_env_creator(name: str) -> EnvCreator | VectorEnvCreator:
     """Loads an environment with name of style ``"(import path):(environment name)"`` and returns the environment creation function, normally the environment class type.
 
@@ -600,14 +592,19 @@
             fn = plugin.load()
             try:
                 fn()
             except Exception:
                 logger.warn(f"plugin: {plugin.value} raised {traceback.format_exc()}")
 
 
+def register_envs(env_module: ModuleType):
+    """A No-op function such that it can appear to IDEs that a module is used."""
+    pass
+
+
 @contextlib.contextmanager
 def namespace(ns: str):
     """Context manager for modifying the current namespace."""
     global current_namespace
     old_namespace = current_namespace
     current_namespace = ns
     yield
@@ -666,17 +663,21 @@
                 f"Custom namespace `{kwargs.get('namespace')}` is being overridden by namespace `{current_namespace}`. "
                 f"If you are developing a plugin you shouldn't specify a namespace in `register` calls. "
                 "The namespace is specified through the entry point package metadata."
             )
         ns_id = current_namespace
     else:
         ns_id = ns
-
     full_env_id = get_env_id(ns_id, name, version)
 
+    if autoreset is True:
+        logger.warn(
+            "`gymnasium.register(..., autoreset=True)` is deprecated and will be removed in v1.0. If users wish to use it then add the auto reset wrapper in the `addition_wrappers` argument."
+        )
+
     new_spec = EnvSpec(
         id=full_env_id,
         entry_point=entry_point,
         reward_threshold=reward_threshold,
         nondeterministic=nondeterministic,
         max_episode_steps=max_episode_steps,
         order_enforce=order_enforce,
@@ -806,15 +807,17 @@
         ):
             raise error.Error(
                 f"You passed render_mode='human' although {env_spec.id} doesn't implement human-rendering natively. "
                 "Gym tried to apply the HumanRendering wrapper but it looks like your environment is using the old "
                 "rendering API, which is not supported by the HumanRendering wrapper."
             ) from e
         else:
-            raise e
+            raise type(e)(
+                f"{e} was raised from the environment creator for {env_spec.id} with kwargs ({env_spec_kwargs})"
+            )
 
     # Set the minimal env spec for the environment.
     env.unwrapped.spec = EnvSpec(
         id=env_spec.id,
         entry_point=env_spec.entry_point,
         reward_threshold=env_spec.reward_threshold,
         nondeterministic=env_spec.nondeterministic,
@@ -842,73 +845,79 @@
                 f"The environment's wrapper spec {recreated_wrapper_spec} is different from the saved `EnvSpec` additional wrapper {env_spec_wrapper_spec}"
             )
 
     # Add step API wrapper
     if apply_api_compatibility is True or (
         apply_api_compatibility is None and env_spec.apply_api_compatibility is True
     ):
-        env = EnvCompatibility(env, render_mode)
+        logger.warn(
+            "`gymnasium.make(..., apply_api_compatibility=True)` and `env_spec.apply_api_compatibility` is deprecated and will be removed in v1.0"
+        )
+        env = gym.wrappers.EnvCompatibility(env, render_mode)
 
     # Run the environment checker as the lowest level wrapper
     if disable_env_checker is False or (
         disable_env_checker is None and env_spec.disable_env_checker is False
     ):
-        env = PassiveEnvChecker(env)
+        env = gym.wrappers.PassiveEnvChecker(env)
 
     # Add the order enforcing wrapper
     if env_spec.order_enforce:
-        env = OrderEnforcing(env)
+        env = gym.wrappers.OrderEnforcing(env)
 
     # Add the time limit wrapper
     if max_episode_steps is not None:
-        env = TimeLimit(env, max_episode_steps)
+        env = gym.wrappers.TimeLimit(env, max_episode_steps)
     elif env_spec.max_episode_steps is not None:
-        env = TimeLimit(env, env_spec.max_episode_steps)
+        env = gym.wrappers.TimeLimit(env, env_spec.max_episode_steps)
 
     # Add the auto-reset wrapper
     if autoreset is True or (autoreset is None and env_spec.autoreset is True):
-        env = AutoResetWrapper(env)
+        env = gym.wrappers.AutoResetWrapper(env)
+
+        logger.warn(
+            "`gymnasium.make(..., autoreset=True)` is deprecated and will be removed in v1.0"
+        )
 
     for wrapper_spec in env_spec.additional_wrappers[num_prior_wrappers:]:
         if wrapper_spec.kwargs is None:
             raise ValueError(
                 f"{wrapper_spec.name} wrapper does not inherit from `gymnasium.utils.RecordConstructorArgs`, therefore, the wrapper cannot be recreated."
             )
 
         env = load_env_creator(wrapper_spec.entry_point)(env=env, **wrapper_spec.kwargs)
 
     # Add human rendering wrapper
     if apply_human_rendering:
-        env = HumanRendering(env)
+        env = gym.wrappers.HumanRendering(env)
     elif apply_render_collection:
-        env = RenderCollection(env)
+        env = gym.wrappers.RenderCollection(env)
 
     return env
 
 
 def make_vec(
     id: str | EnvSpec,
     num_envs: int = 1,
     vectorization_mode: str = "async",
     vector_kwargs: dict[str, Any] | None = None,
     wrappers: Sequence[Callable[[Env], Wrapper]] | None = None,
     **kwargs,
-) -> VectorEnv:
+) -> gym.experimental.vector.VectorEnv:
     """Create a vector environment according to the given ID.
 
     Note:
         This feature is experimental, and is likely to change in future releases.
 
     To find all available environments use `gymnasium.envs.registry.keys()` for all valid ids.
 
     Args:
         id: Name of the environment. Optionally, a module to import can be included, eg. 'module:Env-v0'
         num_envs: Number of environments to create
         vectorization_mode: How to vectorize the environment. Can be either "async", "sync" or "custom"
-        kwargs: Additional arguments to pass to the environment constructor.
         vector_kwargs: Additional arguments to pass to the vectorized environment constructor.
         wrappers: A sequence of wrapper functions to apply to the environment. Can only be used in "sync" or "async" mode.
         **kwargs: Additional arguments to pass to the environment constructor.
 
     Returns:
         An instance of the environment.
 
@@ -949,42 +958,44 @@
         env_creator = entry_point
     else:
         # Assume it's a string
         env_creator = load_env_creator(entry_point)
 
     def _create_env():
         # Env creator for use with sync and async modes
-        render_mode = _kwargs.get("render_mode", None)
-        inner_render_mode = (
-            render_mode[: -len("_list")]
-            if render_mode is not None and render_mode.endswith("_list")
-            else render_mode
-        )
         _kwargs_copy = _kwargs.copy()
-        _kwargs_copy["render_mode"] = inner_render_mode
+
+        render_mode = _kwargs.get("render_mode", None)
+        if render_mode is not None:
+            inner_render_mode = (
+                render_mode[: -len("_list")]
+                if render_mode.endswith("_list")
+                else render_mode
+            )
+            _kwargs_copy["render_mode"] = inner_render_mode
 
         _env = env_creator(**_kwargs_copy)
         _env.spec = spec_
         if spec_.max_episode_steps is not None:
-            _env = TimeLimit(_env, spec_.max_episode_steps)
+            _env = gym.wrappers.TimeLimit(_env, spec_.max_episode_steps)
 
         if render_mode is not None and render_mode.endswith("_list"):
-            _env = RenderCollection(_env)
+            _env = gym.wrappers.RenderCollection(_env)
 
         for wrapper in wrappers:
             _env = wrapper(_env)
         return _env
 
     if vectorization_mode == "sync":
-        env = SyncVectorEnv(
+        env = gym.experimental.vector.SyncVectorEnv(
             env_fns=[_create_env for _ in range(num_envs)],
             **vector_kwargs,
         )
     elif vectorization_mode == "async":
-        env = AsyncVectorEnv(
+        env = gym.experimental.vector.AsyncVectorEnv(
             env_fns=[_create_env for _ in range(num_envs)],
             **vector_kwargs,
         )
     elif vectorization_mode == "custom":
         if len(wrappers) > 0:
             raise error.Error("Cannot use custom vectorization mode with wrappers.")
         vector_kwargs["max_episode_steps"] = spec_.max_episode_steps
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/tabular/blackjack.py` & `gymnasium-0.29.0/gymnasium/envs/tabular/blackjack.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 deck = jnp.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10])
 
 
 class EnvState(NamedTuple):
     """A named tuple which contains the full state of the blackjack game."""
 
-    dealer_hand: jnp.ndarray
-    player_hand: jnp.ndarray
+    dealer_hand: jax.Array
+    player_hand: jax.Array
     dealer_cards: int
     player_cards: int
     done: int
 
 
 def cmp(a, b):
     """Returns 1 if a > b, otherwise returns -1."""
@@ -155,15 +155,15 @@
             jnp.count_nonzero(hand) == 2, (jnp.count_nonzero(hand == 1) > 0)
         ),
         (jnp.count_nonzero(hand == 10) > 0),
     )
 
 
 class BlackjackFunctional(
-    FuncEnv[jnp.ndarray, jnp.ndarray, int, float, bool, RenderStateType]
+    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType]
 ):
     """Blackjack is a card game where the goal is to beat the dealer by obtaining cards that sum to closer to 21 (without going over 21) than the dealers cards.
 
     ### Description
     Card Values:
 
     - Face cards (Jack, Queen, King) have a point value of 10.
@@ -237,17 +237,15 @@
         """Initializes Blackjack functional env."""
         # Flag to payout 1.5 on a "natural" blackjack win, like casino rules
         # Ref: http://www.bicyclecards.com/how-to-play/blackjack/
         self.natural = natural
         # Flag for full agreement with the (Sutton and Barto, 2018) definition. Overrides self.natural
         self.sutton_and_barto = sutton_and_barto
 
-    def transition(
-        self, state: EnvState, action: Union[int, jnp.ndarray], key: PRNGKey
-    ):
+    def transition(self, state: EnvState, action: Union[int, jax.Array], key: PRNGKey):
         """The blackjack environment's state transition function."""
         env_state = jax.lax.cond(action, take, notake, (state, key))
 
         hand_state, key = env_state
         dealer_hand = hand_state.dealer_hand
         player_hand = hand_state.player_hand
         dealer_cards = hand_state.dealer_cards
@@ -282,32 +280,32 @@
             dealer_cards=dealer_cards,
             player_cards=player_cards,
             done=0,
         )
 
         return state
 
-    def observation(self, state: EnvState) -> jnp.ndarray:
+    def observation(self, state: EnvState) -> jax.Array:
         """Blackjack observation."""
         return jnp.array(
             [
                 sum_hand(state.player_hand),
                 state.dealer_hand[0],
                 usable_ace(state.player_hand) * 1.0,
             ],
             dtype=np.int32,
         )
 
-    def terminal(self, state: EnvState) -> jnp.ndarray:
+    def terminal(self, state: EnvState) -> jax.Array:
         """Determines if a particular Blackjack observation is terminal."""
         return (state.done) > 0
 
     def reward(
         self, state: EnvState, action: ActType, next_state: StateType
-    ) -> jnp.ndarray:
+    ) -> jax.Array:
         """Calculates reward from a state."""
         state = next_state
 
         dealer_hand = state.dealer_hand
         player_hand = state.player_hand
 
         # -1 reward if the player busts, otherwise +1 if better than dealer, 0 if tie, -1 if loss.
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/blackjack.py` & `gymnasium-0.29.0/gymnasium/envs/toy_text/blackjack.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/cliffwalking.py` & `gymnasium-0.29.0/gymnasium/envs/toy_text/cliffwalking.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/font/Minecraft.ttf` & `gymnasium-0.29.0/gymnasium/envs/toy_text/font/Minecraft.ttf`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/frozen_lake.py` & `gymnasium-0.29.0/gymnasium/envs/toy_text/frozen_lake.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     The episode ends if the following happens:
 
     - Termination:
         1. The player moves into a hole.
         2. The player reaches the goal at `max(nrow) * max(ncol) - 1` (location `[max(nrow)-1, max(ncol)-1]`).
 
     - Truncation (when using the time_limit wrapper):
-        1. The length of the episode is 100 for 4x4 environment, 200 for 8x8 environment.
+        1. The length of the episode is 100 for 4x4 environment, 200 for FrozenLake8x8-v1 environment.
 
     ## Information
 
     `step()` and `reset()` return a dict with the following keys:
     - p - transition probability for the state.
 
     See <a href="#is_slippy">`is_slippery`</a> for transition probability information.
```

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/C2.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/C2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/C3.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/C3.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/C4.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/C4.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/C5.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/C5.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/C6.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/C6.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/C7.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/C7.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/C8.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/C8.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/C9.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/C9.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/CA.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/CA.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/CJ.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/CJ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/CK.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/CK.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/CQ.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/CQ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/CT.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/CT.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/Card.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/Card.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/D2.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/D2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/D3.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/D3.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/D4.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/D4.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/D5.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/D5.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/D6.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/D6.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/D7.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/D7.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/D8.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/D8.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/D9.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/D9.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/DA.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/DA.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/DJ.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/DJ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/DK.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/DK.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/DQ.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/DQ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/DT.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/DT.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/H2.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/H2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/H3.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/H3.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/H4.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/H4.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/H5.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/H5.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/H6.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/H6.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/H7.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/H7.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/H8.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/H8.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/H9.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/H9.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/HA.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/HA.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/HJ.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/HJ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/HK.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/HK.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/HQ.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/HQ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/HT.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/HT.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/S2.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/S2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/S3.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/S3.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/S4.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/S4.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/S5.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/S5.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/S6.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/S6.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/S7.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/S7.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/S8.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/S8.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/S9.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/S9.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/SA.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/SA.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/SJ.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/SJ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/SK.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/SK.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/SQ.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/SQ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/ST.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/ST.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/cab_front.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/cab_front.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/cab_left.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/cab_left.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/cab_rear.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/cab_rear.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/cab_right.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/cab_right.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/cookie.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/cookie.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/cracked_hole.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/cracked_hole.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/elf_down.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/elf_down.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/elf_left.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/elf_left.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/elf_right.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/elf_right.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/elf_up.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/elf_up.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/goal.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/goal.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_bottom.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_bottom.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_horiz.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_horiz.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_left.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_left.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_right.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_right.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_top.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_top.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/gridworld_median_vert.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/gridworld_median_vert.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/hole.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/hole.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/hotel.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/hotel.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_bg1.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_bg1.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_bg2.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_bg2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_near-cliff1.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_near-cliff1.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/mountain_near-cliff2.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/mountain_near-cliff2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/passenger.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/passenger.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/stool.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/stool.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/img/taxi_background.png` & `gymnasium-0.29.0/gymnasium/envs/toy_text/img/taxi_background.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/envs/toy_text/taxi.py` & `gymnasium-0.29.0/gymnasium/envs/toy_text/taxi.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/error.py` & `gymnasium-0.29.0/gymnasium/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,14 +177,18 @@
     """Error message for using wrap after configure."""
 
 
 class RetriesExceededError(Error):
     """Error message for retries exceeding set number."""
 
 
+class DeprecatedWrapper(ImportError):
+    """Error message for importing an old version of a wrapper."""
+
+
 # Vectorized environments errors
 
 
 class AlreadyPendingCallError(Exception):
     """Raised when `reset`, or `step` is called asynchronously (e.g. with `reset_async`, or `step_async` respectively), and `reset_async`, or `step_async` (respectively) is called again (without a complete call to `reset_wait`, or `step_wait` respectively)."""
 
     def __init__(self, message: str, name: str):
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/__init__.py` & `gymnasium-0.29.0/gymnasium/experimental/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Root __init__ of the gym experimental wrappers."""
 
 
-from gymnasium.experimental import functional, wrappers
-from gymnasium.experimental.functional import FuncEnv
-from gymnasium.experimental.vector.async_vector_env import AsyncVectorEnv
-from gymnasium.experimental.vector.sync_vector_env import SyncVectorEnv
-from gymnasium.experimental.vector.vector_env import VectorEnv, VectorWrapper
+from gymnasium.experimental import functional, vector, wrappers
+
+
+# from gymnasium.experimental.functional import FuncEnv
+# from gymnasium.experimental.vector.async_vector_env import AsyncVectorEnv
+# from gymnasium.experimental.vector.sync_vector_env import SyncVectorEnv
+# from gymnasium.experimental.vector.vector_env import VectorEnv, VectorWrapper
 
 
 __all__ = [
     # Functional
-    "FuncEnv",
+    # "FuncEnv",
     "functional",
     # Vector
-    "VectorEnv",
-    "VectorWrapper",
-    "SyncVectorEnv",
-    "AsyncVectorEnv",
+    # "VectorEnv",
+    # "VectorWrapper",
+    # "SyncVectorEnv",
+    # "AsyncVectorEnv",
     # wrappers
     "wrappers",
+    "vector",
 ]
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/functional.py` & `gymnasium-0.29.0/gymnasium/experimental/functional.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/experimental/functional_jax_env.py` & `gymnasium-0.29.0/gymnasium/experimental/functional_jax_env.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -131,17 +131,17 @@
     ):
         """Initialize the environment from a FuncEnv."""
         super().__init__()
         if metadata is None:
             metadata = {}
         self.func_env = func_env
         self.num_envs = num_envs
+
         self.single_observation_space = func_env.observation_space
         self.single_action_space = func_env.action_space
-
         self.observation_space = batch_space(
             self.single_observation_space, self.num_envs
         )
         self.action_space = batch_space(self.single_action_space, self.num_envs)
 
         self.metadata = metadata
         self.render_mode = render_mode
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/vector/__init__.py` & `gymnasium-0.29.0/gymnasium/experimental/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/experimental/vector/async_vector_env.py` & `gymnasium-0.29.0/gymnasium/experimental/vector/async_vector_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,16 @@
             context: Context for `multiprocessing`_. If ``None``, then the default context is used.
             daemon: If ``True``, then subprocesses have ``daemon`` flag turned on; that is, they will quit if
                 the head process quits. However, ``daemon=True`` prevents subprocesses to spawn children,
                 so for some environments you may want to have it set to ``False``.
             worker: If set, then use that worker in a subprocess instead of a default one.
                 Can be useful to override some inner vector env logic, for instance, how resets on termination or truncation are handled.
 
-        Warnings: worker is an advanced mode option. It provides a high degree of flexibility and a high chance
+        Warnings:
+            worker is an advanced mode option. It provides a high degree of flexibility and a high chance
             to shoot yourself in the foot; thus, if you are writing your own worker, it is recommended to start
             from the code for ``_worker`` (or ``_worker_shared_memory``) method, and add changes.
 
         Raises:
             RuntimeError: If the observation space of some sub-environment does not match observation_space
                 (or, by default, the observation space of the first sub-environment).
             ValueError: If observation_space is a custom space (i.e. not a default space in Gym,
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/vector/sync_vector_env.py` & `gymnasium-0.29.0/gymnasium/experimental/vector/sync_vector_env.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/experimental/vector/utils/__init__.py` & `gymnasium-0.29.0/gymnasium/experimental/vector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/experimental/vector/utils/misc.py` & `gymnasium-0.29.0/gymnasium/experimental/vector/utils/misc.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/experimental/vector/utils/shared_memory.py` & `gymnasium-0.29.0/gymnasium/experimental/vector/utils/shared_memory.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/experimental/vector/utils/space_utils.py` & `gymnasium-0.29.0/gymnasium/experimental/vector/utils/space_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,36 +69,29 @@
     repeats = tuple([n] + [1] * space.low.ndim)
     low, high = np.tile(space.low, repeats), np.tile(space.high, repeats)
     return Box(low=low, high=high, dtype=space.dtype, seed=deepcopy(space.np_random))
 
 
 @batch_space.register(Discrete)
 def _batch_space_discrete(space: Discrete, n: int = 1):
-    if space.start == 0:
-        return MultiDiscrete(
-            np.full((n,), space.n, dtype=space.dtype),
-            dtype=space.dtype,
-            seed=deepcopy(space.np_random),
-        )
-    else:
-        return Box(
-            low=space.start,
-            high=space.start + space.n - 1,
-            shape=(n,),
-            dtype=space.dtype,
-            seed=deepcopy(space.np_random),
-        )
+    return MultiDiscrete(
+        np.full((n,), space.n, dtype=space.dtype),
+        dtype=space.dtype,
+        seed=deepcopy(space.np_random),
+        start=np.full((n,), space.start, dtype=space.dtype),
+    )
 
 
 @batch_space.register(MultiDiscrete)
 def _batch_space_multidiscrete(space: MultiDiscrete, n: int = 1):
     repeats = tuple([n] + [1] * space.nvec.ndim)
-    high = np.tile(space.nvec, repeats) - 1
+    low = np.tile(space.start, repeats)
+    high = low + np.tile(space.nvec, repeats) - 1
     return Box(
-        low=np.zeros_like(high),
+        low=low,
         high=high,
         dtype=space.dtype,
         seed=deepcopy(space.np_random),
     )
 
 
 @batch_space.register(MultiBinary)
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/vector/vector_env.py` & `gymnasium-0.29.0/gymnasium/vector/vector_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,21 @@
 """Base class for vectorized environments."""
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
+from typing import Any, List, Optional, Tuple, Union
 
 import numpy as np
+from numpy.typing import NDArray
 
 import gymnasium as gym
-from gymnasium.core import ActType, ObsType
-from gymnasium.utils import seeding
-
-
-if TYPE_CHECKING:
-    from gymnasium.envs.registration import EnvSpec
+from gymnasium.vector.utils.spaces import batch_space
 
-ArrayType = TypeVar("ArrayType")
 
+__all__ = ["VectorEnv"]
 
-__all__ = [
-    "VectorEnv",
-    "VectorWrapper",
-    "VectorObservationWrapper",
-    "VectorActionWrapper",
-    "VectorRewardWrapper",
-    "ArrayType",
-]
 
-
-class VectorEnv(Generic[ObsType, ActType, ArrayType]):
+class VectorEnv(gym.Env):
     """Base class for vectorized environments to run multiple independent copies of the same environment in parallel.
 
     Vector environments can provide a linear speed-up in the steps taken per second through sampling multiple
     sub-environments at the same time. To prevent terminated environments waiting until all sub-environments have
     terminated or truncated, the vector environments autoreset sub-environments after they terminate or truncated.
     As a result, the final step's observation and info are overwritten by the reset's observation and info.
     Therefore, the observation and info for the final step of a sub-environment is stored in the info parameter,
@@ -59,31 +44,83 @@
         for all the sub-environments during initialization.
 
     Note:
         All parallel environments should share the identical observation and action spaces.
         In other words, a vector of multiple different environments is not supported.
     """
 
-    spec: EnvSpec
+    def __init__(
+        self,
+        num_envs: int,
+        observation_space: gym.Space,
+        action_space: gym.Space,
+    ):
+        """Base class for vectorized environments.
+
+        Args:
+            num_envs: Number of environments in the vectorized environment.
+            observation_space: Observation space of a single environment.
+            action_space: Action space of a single environment.
+        """
+        self.num_envs = num_envs
+        self.is_vector_env = True
+        self.observation_space = batch_space(observation_space, n=num_envs)
+        self.action_space = batch_space(action_space, n=num_envs)
+
+        self.closed = False
+        self.viewer = None
+
+        # The observation and action spaces of a single environment are
+        # kept in separate properties
+        self.single_observation_space = observation_space
+        self.single_action_space = action_space
+
+    def reset_async(
+        self,
+        seed: Optional[Union[int, List[int]]] = None,
+        options: Optional[dict] = None,
+    ):
+        """Reset the sub-environments asynchronously.
+
+        This method will return ``None``. A call to :meth:`reset_async` should be followed
+        by a call to :meth:`reset_wait` to retrieve the results.
+
+        Args:
+            seed: The reset seed
+            options: Reset options
+        """
+        pass
 
-    observation_space: gym.Space
-    action_space: gym.Space
+    def reset_wait(
+        self,
+        seed: Optional[Union[int, List[int]]] = None,
+        options: Optional[dict] = None,
+    ):
+        """Retrieves the results of a :meth:`reset_async` call.
+
+        A call to this method must always be preceded by a call to :meth:`reset_async`.
 
-    num_envs: int
+        Args:
+            seed: The reset seed
+            options: Reset options
 
-    closed = False
+        Returns:
+            The results from :meth:`reset_async`
 
-    _np_random: np.random.Generator | None = None
+        Raises:
+            NotImplementedError: VectorEnv does not implement function
+        """
+        raise NotImplementedError("VectorEnv does not implement function")
 
     def reset(
         self,
         *,
-        seed: int | list[int] | None = None,
-        options: dict[str, Any] | None = None,
-    ) -> tuple[ObsType, dict[str, Any]]:  # type: ignore
+        seed: Optional[Union[int, List[int]]] = None,
+        options: Optional[dict] = None,
+    ):
         """Reset all parallel environments and return a batch of initial observations and info.
 
         Args:
             seed: The environment reset seeds
             options: If to return the options
 
         Returns:
@@ -94,20 +131,44 @@
             >>> envs = gym.vector.make("CartPole-v1", num_envs=3)
             >>> envs.reset(seed=42)
             (array([[ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ],
                    [ 0.01522993, -0.04562247, -0.04799704,  0.03392126],
                    [-0.03774345, -0.02418869, -0.00942293,  0.0469184 ]],
                   dtype=float32), {})
         """
-        if seed is not None:
-            self._np_random, seed = seeding.np_random(seed)
+        self.reset_async(seed=seed, options=options)
+        return self.reset_wait(seed=seed, options=options)
+
+    def step_async(self, actions):
+        """Asynchronously performs steps in the sub-environments.
+
+        The results can be retrieved via a call to :meth:`step_wait`.
+
+        Args:
+            actions: The actions to take asynchronously
+        """
+
+    def step_wait(
+        self, **kwargs
+    ) -> Tuple[Any, NDArray[Any], NDArray[Any], NDArray[Any], dict]:
+        """Retrieves the results of a :meth:`step_async` call.
+
+        A call to this method must always be preceded by a call to :meth:`step_async`.
+
+        Args:
+            **kwargs: Additional keywords for vector implementation
+
+        Returns:
+            The results from the :meth:`step_async` call
+        """
+        raise NotImplementedError()
 
     def step(
-        self, actions: ActType
-    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
+        self, actions
+    ) -> Tuple[Any, NDArray[Any], NDArray[Any], NDArray[Any], dict]:
         """Take an action for each parallel environment.
 
         Args:
             actions: element of :attr:`action_space` Batch of actions.
 
         Returns:
             Batch of (observations, rewards, terminations, truncations, infos)
@@ -129,20 +190,62 @@
                    [ 0.01431748, -0.24002443, -0.04731862,  0.3110827 ],
                    [-0.03822722,  0.1710671 , -0.00848456, -0.2487226 ]],
                   dtype=float32)
             >>> rewards
             array([1., 1., 1.])
             >>> termination
             array([False, False, False])
-            >>> termination
+            >>> truncation
             array([False, False, False])
             >>> infos
             {}
         """
-        pass
+        self.step_async(actions)
+        return self.step_wait()
+
+    def call_async(self, name, *args, **kwargs):
+        """Calls a method name for each parallel environment asynchronously."""
+
+    def call_wait(self, **kwargs) -> List[Any]:  # type: ignore
+        """After calling a method in :meth:`call_async`, this function collects the results."""
+
+    def call(self, name: str, *args, **kwargs) -> List[Any]:
+        """Call a method, or get a property, from each parallel environment.
+
+        Args:
+            name (str): Name of the method or property to call.
+            *args: Arguments to apply to the method call.
+            **kwargs: Keyword arguments to apply to the method call.
+
+        Returns:
+            List of the results of the individual calls to the method or property for each environment.
+        """
+        self.call_async(name, *args, **kwargs)
+        return self.call_wait()
+
+    def get_attr(self, name: str):
+        """Get a property from each parallel environment.
+
+        Args:
+            name (str): Name of the property to be get from each individual environment.
+
+        Returns:
+            The property with name
+        """
+        return self.call(name)
+
+    def set_attr(self, name: str, values: Union[list, tuple, object]):
+        """Set a property in each sub-environment.
+
+        Args:
+            name (str): Name of the property to be set in each individual environment.
+            values (list, tuple, or object): Values of the property to be set to. If `values` is a list or
+                tuple, then it corresponds to the values for each individual environment, otherwise a single value
+                is set for all environments.
+        """
 
     def close_extras(self, **kwargs):
         """Clean up the extra resources e.g. beyond what's in this base class."""
         pass
 
     def close(self, **kwargs):
         """Close all parallel environments and release resources.
@@ -159,38 +262,19 @@
             This will be automatically called when garbage collected or program exited.
 
         Args:
             **kwargs: Keyword arguments passed to :meth:`close_extras`
         """
         if self.closed:
             return
-
+        if self.viewer is not None:
+            self.viewer.close()
         self.close_extras(**kwargs)
         self.closed = True
 
-    @property
-    def np_random(self) -> np.random.Generator:
-        """Returns the environment's internal :attr:`_np_random` that if not set will initialise with a random seed.
-
-        Returns:
-            Instances of `np.random.Generator`
-        """
-        if self._np_random is None:
-            self._np_random, seed = seeding.np_random()
-        return self._np_random
-
-    @np_random.setter
-    def np_random(self, value: np.random.Generator):
-        self._np_random = value
-
-    @property
-    def unwrapped(self):
-        """Return the base environment."""
-        return self
-
     def _add_info(self, infos: dict, info: dict, env_num: int) -> dict:
         """Add env info to the info dictionary of the vectorized environment.
 
         Given the `info` of a single environment add it to the `infos` dictionary
         which represents all the infos of the vectorized environment.
         Every `key` of `info` is paired with a boolean mask `_key` representing
         whether or not the i-indexed environment has this `info`.
@@ -210,15 +294,15 @@
             else:
                 info_array, array_mask = infos[k], infos[f"_{k}"]
 
             info_array[env_num], array_mask[env_num] = info[k], True
             infos[k], infos[f"_{k}"] = info_array, array_mask
         return infos
 
-    def _init_info_arrays(self, dtype: type) -> tuple[np.ndarray, np.ndarray]:
+    def _init_info_arrays(self, dtype: type) -> Tuple[np.ndarray, np.ndarray]:
         """Initialize the info array.
 
         Initialize the info array. If the dtype is numeric
         the info array will have the same dtype, otherwise
         will be an array of `None`. Also, a boolean array
         of the same length is returned. It will be used for
         assessing which environment has info data.
@@ -246,140 +330,69 @@
 
     def __repr__(self) -> str:
         """Returns a string representation of the vector environment.
 
         Returns:
             A string containing the class name, number of environments and environment spec id
         """
-        if getattr(self, "spec", None) is None:
+        if self.spec is None:
             return f"{self.__class__.__name__}({self.num_envs})"
         else:
             return f"{self.__class__.__name__}({self.spec.id}, {self.num_envs})"
 
 
-class VectorWrapper(VectorEnv):
+class VectorEnvWrapper(VectorEnv):
     """Wraps the vectorized environment to allow a modular transformation.
 
     This class is the base class for all wrappers for vectorized environments. The subclass
     could override some methods to change the behavior of the original vectorized environment
     without touching the original code.
 
     Note:
         Don't forget to call ``super().__init__(env)`` if the subclass overrides :meth:`__init__`.
     """
 
     def __init__(self, env: VectorEnv):
-        """Initialize the vectorized environment wrapper."""
-        super().__init__()
-
         assert isinstance(env, VectorEnv)
         self.env = env
 
     # explicitly forward the methods defined in VectorEnv
     # to self.env (instead of the base class)
+    def reset_async(self, **kwargs):
+        return self.env.reset_async(**kwargs)
 
-    def reset(self, **kwargs):
-        """Reset all environments."""
-        return self.env.reset(**kwargs)
-
-    def step(self, actions):
-        """Step all environments."""
-        return self.env.step(actions)
+    def reset_wait(self, **kwargs):
+        return self.env.reset_wait(**kwargs)
+
+    def step_async(self, actions):
+        return self.env.step_async(actions)
+
+    def step_wait(self):
+        return self.env.step_wait()
 
     def close(self, **kwargs):
-        """Close all environments."""
         return self.env.close(**kwargs)
 
     def close_extras(self, **kwargs):
-        """Close all extra resources."""
         return self.env.close_extras(**kwargs)
 
+    def call(self, name, *args, **kwargs):
+        return self.env.call(name, *args, **kwargs)
+
+    def set_attr(self, name, values):
+        return self.env.set_attr(name, values)
+
     # implicitly forward all other methods and attributes to self.env
     def __getattr__(self, name):
-        """Forward all other attributes to the base environment."""
         if name.startswith("_"):
             raise AttributeError(f"attempted to get missing private attribute '{name}'")
         return getattr(self.env, name)
 
     @property
     def unwrapped(self):
-        """Return the base non-wrapped environment."""
         return self.env.unwrapped
 
     def __repr__(self):
-        """Return the string representation of the vectorized environment."""
         return f"<{self.__class__.__name__}, {self.env}>"
 
     def __del__(self):
-        """Close the vectorized environment."""
         self.env.__del__()
-
-
-class VectorObservationWrapper(VectorWrapper):
-    """Wraps the vectorized environment to allow a modular transformation of the observation. Equivalent to :class:`gym.ObservationWrapper` for vectorized environments."""
-
-    def reset(self, **kwargs):
-        """Modifies the observation returned from the environment ``reset`` using the :meth:`observation`."""
-        observation = self.env.reset(**kwargs)
-        return self.observation(observation)
-
-    def step(self, actions):
-        """Modifies the observation returned from the environment ``step`` using the :meth:`observation`."""
-        observation, reward, termination, truncation, info = self.env.step(actions)
-        return (
-            self.observation(observation),
-            observation,
-            reward,
-            termination,
-            truncation,
-            info,
-        )
-
-    def observation(self, observation: ObsType) -> ObsType:
-        """Defines the observation transformation.
-
-        Args:
-            observation (object): the observation from the environment
-
-        Returns:
-            observation (object): the transformed observation
-        """
-        raise NotImplementedError
-
-
-class VectorActionWrapper(VectorWrapper):
-    """Wraps the vectorized environment to allow a modular transformation of the actions. Equivalent of :class:`~gym.ActionWrapper` for vectorized environments."""
-
-    def step(self, actions: ActType):
-        """Steps through the environment using a modified action by :meth:`action`."""
-        return self.env.step(self.action(actions))
-
-    def actions(self, actions: ActType) -> ActType:
-        """Transform the actions before sending them to the environment.
-
-        Args:
-            actions (ActType): the actions to transform
-
-        Returns:
-            ActType: the transformed actions
-        """
-        raise NotImplementedError
-
-
-class VectorRewardWrapper(VectorWrapper):
-    """Wraps the vectorized environment to allow a modular transformation of the reward. Equivalent of :class:`~gym.RewardWrapper` for vectorized environments."""
-
-    def step(self, actions):
-        """Steps through the environment returning a reward modified by :meth:`reward`."""
-        observation, reward, termination, truncation, info = self.env.step(actions)
-        return observation, self.reward(reward), termination, truncation, info
-
-    def reward(self, reward: ArrayType) -> ArrayType:
-        """Transform the reward before returning it.
-
-        Args:
-            reward (array): the reward to transform
-
-        Returns:
-            array: the transformed reward
-        """
-        raise NotImplementedError
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/atari_preprocessing.py` & `gymnasium-0.29.0/gymnasium/wrappers/atari_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 import gymnasium as gym
 from gymnasium.spaces import Box
 
 
 try:
     import cv2
 except ImportError:
-    raise gym.error.DependencyNotInstalled(
-        "opencv-python package not installed, run `pip install gymnasium[other]` to get dependencies for atari"
-    )
+    cv2 = None
 
 
-class AtariPreprocessingV0(gym.Wrapper, gym.utils.RecordConstructorArgs):
+class AtariPreprocessing(gym.Wrapper, gym.utils.RecordConstructorArgs):
     """Atari 2600 preprocessing wrapper.
 
     This class follows the guidelines in Machado et al. (2018),
     "Revisiting the Arcade Learning Environment: Evaluation Protocols and Open Problems for General Agents".
 
     Specifically, the following preprocess stages applies to the atari environment:
 
@@ -70,14 +68,18 @@
             terminal_on_life_loss=terminal_on_life_loss,
             grayscale_obs=grayscale_obs,
             grayscale_newaxis=grayscale_newaxis,
             scale_obs=scale_obs,
         )
         gym.Wrapper.__init__(self, env)
 
+        if cv2 is None:
+            raise gym.error.DependencyNotInstalled(
+                "opencv-python package not installed, run `pip install gymnasium[other]` to get dependencies for atari"
+            )
         assert frame_skip > 0
         assert screen_size > 0
         assert noop_max >= 0
         if frame_skip > 1:
             if (
                 env.spec is not None
                 and "NoFrameskip" not in env.spec.id
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/common.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     check_observation_space,
     env_render_passive_checker,
     env_reset_passive_checker,
     env_step_passive_checker,
 )
 
 
+__all__ = [
+    "AutoresetV0",
+    "PassiveEnvCheckerV0",
+    "OrderEnforcingV0",
+    "RecordEpisodeStatisticsV0",
+]
+
+
 class AutoresetV0(
     gym.Wrapper[ObsType, ActType, ObsType, ActType], gym.utils.RecordConstructorArgs
 ):
     """A class for providing an automatic reset functionality for gymnasium environments when calling :meth:`self.step`."""
 
     def __init__(self, env: gym.Env[ObsType, ActType]):
         """A class for providing an automatic reset functionality for gymnasium environments when calling :meth:`self.step`.
@@ -79,19 +87,19 @@
     def __init__(self, env: gym.Env[ObsType, ActType]):
         """Initialises the wrapper with the environments, run the observation and action space tests."""
         gym.utils.RecordConstructorArgs.__init__(self)
         gym.Wrapper.__init__(self, env)
 
         assert hasattr(
             env, "action_space"
-        ), "The environment must specify an action space. https://gymnasium.farama.org/content/environment_creation/"
+        ), "The environment must specify an action space. https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/"
         check_action_space(env.action_space)
         assert hasattr(
             env, "observation_space"
-        ), "The environment must specify an observation space. https://gymnasium.farama.org/content/environment_creation/"
+        ), "The environment must specify an observation space. https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/"
         check_observation_space(env.observation_space)
 
         self._checked_reset: bool = False
         self._checked_step: bool = False
         self._checked_render: bool = False
 
     def step(
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/jax_to_numpy.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/jax_to_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,82 +10,89 @@
 
 import gymnasium as gym
 from gymnasium.core import ActType, ObsType, RenderFrame, WrapperActType, WrapperObsType
 from gymnasium.error import DependencyNotInstalled
 
 
 try:
+    import jax
     import jax.numpy as jnp
 except ImportError:
     raise DependencyNotInstalled(
         "Jax is not installed therefore cannot call `numpy_to_jax`, run `pip install gymnasium[jax]`"
     )
 
-__all__ = ["jax_to_numpy", "numpy_to_jax", "JaxToNumpyV0"]
+__all__ = ["JaxToNumpyV0", "jax_to_numpy", "numpy_to_jax"]
 
 
 @functools.singledispatch
 def numpy_to_jax(value: Any) -> Any:
-    """Converts a value to a Jax DeviceArray."""
+    """Converts a value to a Jax Array."""
     raise Exception(
         f"No known conversion for Numpy type ({type(value)}) to Jax registered. Report as issue on github."
     )
 
 
 @numpy_to_jax.register(numbers.Number)
-@numpy_to_jax.register(np.ndarray)
-def _number_ndarray_numpy_to_jax(
-    value: np.ndarray | numbers.Number,
-) -> jnp.DeviceArray:
-    """Converts a numpy array or  number (int, float, etc.) to a Jax DeviceArray."""
+def _number_to_jax(
+    value: numbers.Number,
+) -> jax.Array:
+    """Converts a number (int, float, etc.) to a Jax Array."""
     assert jnp is not None
     return jnp.array(value)
 
 
+@numpy_to_jax.register(np.ndarray)
+def _numpy_array_to_jax(value: np.ndarray) -> jax.Array:
+    """Converts a NumPy Array to a Jax Array with the same dtype (excluding float64 without being enabled)."""
+    assert jnp is not None
+    return jnp.array(value, dtype=value.dtype)
+
+
 @numpy_to_jax.register(abc.Mapping)
 def _mapping_numpy_to_jax(value: Mapping[str, Any]) -> Mapping[str, Any]:
-    """Converts a dictionary of numpy arrays to a mapping of Jax DeviceArrays."""
+    """Converts a dictionary of numpy arrays to a mapping of Jax Array."""
     return type(value)(**{k: numpy_to_jax(v) for k, v in value.items()})
 
 
 @numpy_to_jax.register(abc.Iterable)
 def _iterable_numpy_to_jax(
     value: Iterable[np.ndarray | Any],
-) -> Iterable[jnp.DeviceArray | Any]:
-    """Converts an Iterable from Numpy Arrays to an iterable of Jax DeviceArrays."""
+) -> Iterable[jax.Array | Any]:
+    """Converts an Iterable from Numpy Arrays to an iterable of Jax Array."""
     return type(value)(numpy_to_jax(v) for v in value)
 
 
 @functools.singledispatch
 def jax_to_numpy(value: Any) -> Any:
     """Converts a value to a numpy array."""
     raise Exception(
         f"No known conversion for Jax type ({type(value)}) to NumPy registered. Report as issue on github."
     )
 
 
-@jax_to_numpy.register(jnp.DeviceArray)
-def _devicearray_jax_to_numpy(value: jnp.DeviceArray) -> np.ndarray:
-    """Converts a Jax DeviceArray to a numpy array."""
+@jax_to_numpy.register(jax.Array)
+def _devicearray_jax_to_numpy(value: jax.Array) -> np.ndarray:
+    """Converts a Jax Array to a numpy array."""
     return np.array(value)
 
 
 @jax_to_numpy.register(abc.Mapping)
 def _mapping_jax_to_numpy(
-    value: Mapping[str, jnp.DeviceArray | Any]
+    value: Mapping[str, jax.Array | Any]
 ) -> Mapping[str, np.ndarray | Any]:
-    """Converts a dictionary of Jax DeviceArrays to a mapping of numpy arrays."""
+    """Converts a dictionary of Jax Array to a mapping of numpy arrays."""
     return type(value)(**{k: jax_to_numpy(v) for k, v in value.items()})
 
 
 @jax_to_numpy.register(abc.Iterable)
 def _iterable_jax_to_numpy(
     value: Iterable[np.ndarray | Any],
-) -> Iterable[jnp.DeviceArray | Any]:
-    """Converts an Iterable from Numpy arrays to an iterable of Jax DeviceArrays."""
+) -> Iterable[jax.Array | Any]:
+    """Converts an Iterable from Numpy arrays to an iterable of Jax Array."""
     return type(value)(jax_to_numpy(v) for v in value)
 
 
 class JaxToNumpyV0(
     gym.Wrapper[WrapperObsType, WrapperActType, ObsType, ActType],
     gym.utils.RecordConstructorArgs,
 ):
@@ -95,18 +102,18 @@
 
     Notes:
         The Jax To Numpy and Numpy to Jax conversion does not guarantee a roundtrip (jax -> numpy -> jax) and vice versa.
         The reason for this is jax does not support non-array values, therefore numpy ``int_32(5) -> DeviceArray([5], dtype=jnp.int23)``
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType]):
-        """Wraps an environment such that the input and outputs are numpy arrays.
+        """Wraps a jax environment such that the input and outputs are numpy arrays.
 
         Args:
-            env: the environment to wrap
+            env: the jax environment to wrap
         """
         if jnp is None:
             raise DependencyNotInstalled(
                 "jax is not installed, run `pip install gymnasium[jax]`"
             )
         gym.utils.RecordConstructorArgs.__init__(self)
         gym.Wrapper.__init__(self, env)
@@ -116,15 +123,15 @@
     ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict]:
         """Transforms the action to a jax array .
 
         Args:
             action: the action to perform as a numpy array
 
         Returns:
-            A tuple containing the next observation, reward, termination, truncation, and extra info.
+            A tuple containing numpy versions of the next observation, reward, termination, truncation, and extra info.
         """
         jax_action = numpy_to_jax(action)
         obs, reward, terminated, truncated, info = self.env.step(jax_action)
 
         return (
             jax_to_numpy(obs),
             float(reward),
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/jax_to_torch.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/jax_to_torch.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import gymnasium as gym
 from gymnasium.core import RenderFrame, WrapperActType, WrapperObsType
 from gymnasium.error import DependencyNotInstalled
 from gymnasium.experimental.wrappers.jax_to_numpy import jax_to_numpy
 
 
 try:
+    import jax
     import jax.numpy as jnp
     from jax import dlpack as jax_dlpack
 except ImportError:
     raise DependencyNotInstalled(
         "Jax is not installed therefore cannot call `torch_to_jax`, run `pip install gymnasium[jax]`"
     )
 
@@ -35,90 +36,90 @@
     Device = Union[str, torch.device]
 except ImportError:
     raise DependencyNotInstalled(
         "Torch is not installed therefore cannot call `torch_to_jax`, run `pip install torch`"
     )
 
 
-__all__ = ["jax_to_torch", "torch_to_jax", "JaxToTorchV0"]
+__all__ = ["JaxToTorchV0", "jax_to_torch", "torch_to_jax", "Device"]
 
 
 @functools.singledispatch
 def torch_to_jax(value: Any) -> Any:
-    """Converts a PyTorch Tensor into a Jax DeviceArray."""
+    """Converts a PyTorch Tensor into a Jax Array."""
     raise Exception(
         f"No known conversion for Torch type ({type(value)}) to Jax registered. Report as issue on github."
     )
 
 
 @torch_to_jax.register(numbers.Number)
 def _number_torch_to_jax(value: numbers.Number) -> Any:
     """Convert a python number (int, float, complex) to a jax array."""
     return jnp.array(value)
 
 
 @torch_to_jax.register(torch.Tensor)
-def _tensor_torch_to_jax(value: torch.Tensor) -> jnp.DeviceArray:
-    """Converts a PyTorch Tensor into a Jax DeviceArray."""
+def _tensor_torch_to_jax(value: torch.Tensor) -> jax.Array:
+    """Converts a PyTorch Tensor into a Jax Array."""
     tensor = torch_dlpack.to_dlpack(value)  # pyright: ignore[reportPrivateImportUsage]
     tensor = jax_dlpack.from_dlpack(tensor)  # pyright: ignore[reportPrivateImportUsage]
     return tensor
 
 
 @torch_to_jax.register(abc.Mapping)
 def _mapping_torch_to_jax(value: Mapping[str, Any]) -> Mapping[str, Any]:
-    """Converts a mapping of PyTorch Tensors into a Dictionary of Jax DeviceArrays."""
+    """Converts a mapping of PyTorch Tensors into a Dictionary of Jax Array."""
     return type(value)(**{k: torch_to_jax(v) for k, v in value.items()})
 
 
 @torch_to_jax.register(abc.Iterable)
 def _iterable_torch_to_jax(value: Iterable[Any]) -> Iterable[Any]:
-    """Converts an Iterable from PyTorch Tensors to an iterable of Jax DeviceArrays."""
+    """Converts an Iterable from PyTorch Tensors to an iterable of Jax Array."""
     return type(value)(torch_to_jax(v) for v in value)
 
 
 @functools.singledispatch
 def jax_to_torch(value: Any, device: Device | None = None) -> Any:
-    """Converts a Jax DeviceArray into a PyTorch Tensor."""
+    """Converts a Jax Array into a PyTorch Tensor."""
     raise Exception(
         f"No known conversion for Jax type ({type(value)}) to PyTorch registered. Report as issue on github."
     )
 
 
-@jax_to_torch.register(jnp.DeviceArray)
+@jax_to_torch.register(jax.Array)
 def _devicearray_jax_to_torch(
-    value: jnp.DeviceArray, device: Device | None = None
+    value: jax.Array, device: Device | None = None
 ) -> torch.Tensor:
-    """Converts a Jax DeviceArray into a PyTorch Tensor."""
+    """Converts a Jax Array into a PyTorch Tensor."""
     assert jax_dlpack is not None and torch_dlpack is not None
     dlpack = jax_dlpack.to_dlpack(value)  # pyright: ignore[reportPrivateImportUsage]
     tensor = torch_dlpack.from_dlpack(dlpack)
     if device:
         return tensor.to(device=device)
     return tensor
 
 
 @jax_to_torch.register(abc.Mapping)
 def _jax_mapping_to_torch(
     value: Mapping[str, Any], device: Device | None = None
 ) -> Mapping[str, Any]:
-    """Converts a mapping of Jax DeviceArrays into a Dictionary of PyTorch Tensors."""
+    """Converts a mapping of Jax Array into a Dictionary of PyTorch Tensors."""
     return type(value)(**{k: jax_to_torch(v, device) for k, v in value.items()})
 
 
 @jax_to_torch.register(abc.Iterable)
 def _jax_iterable_to_torch(
     value: Iterable[Any], device: Device | None = None
 ) -> Iterable[Any]:
-    """Converts an Iterable from Jax DeviceArrays to an iterable of PyTorch Tensors."""
+    """Converts an Iterable from Jax Array to an iterable of PyTorch Tensors."""
     return type(value)(jax_to_torch(v, device) for v in value)
 
 
 class JaxToTorchV0(gym.Wrapper, gym.utils.RecordConstructorArgs):
-    """Wraps a jax-based environment so that it can be interacted with through PyTorch Tensors.
+    """Wraps a Jax-based environment so that it can be interacted with through PyTorch Tensors.
 
     Actions must be provided as PyTorch Tensors and observations will be returned as PyTorch Tensors.
 
     Note:
         For ``rendered`` this is returned as a NumPy array not a pytorch Tensor.
     """
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/lambda_action.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/lambda_action.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 """A collection of wrappers that all use the LambdaAction class.
 
-* ``LambdaAction`` - Transforms the actions based on a function
-* ``ClipAction`` - Clips the action within a bounds
-* ``RescaleAction`` - Rescales the action within a minimum and maximum actions
+* ``LambdaActionV0`` - Transforms the actions based on a function
+* ``ClipActionV0`` - Clips the action within a bounds
+* ``RescaleActionV0`` - Rescales the action within a minimum and maximum actions
 """
 from __future__ import annotations
 
 from typing import Callable
 
-
-try:
-    import jumpy.numpy as jp
-except ImportError as e:
-    raise ImportError("Jumpy is not installed, run `pip install jax-jumpy`") from e
 import numpy as np
 
 import gymnasium as gym
 from gymnasium.core import ActType, ObsType, WrapperActType
 from gymnasium.spaces import Box, Space
 
 
+__all__ = ["LambdaActionV0", "ClipActionV0", "RescaleActionV0"]
+
+
 class LambdaActionV0(
     gym.ActionWrapper[ObsType, WrapperActType, ActType], gym.utils.RecordConstructorArgs
 ):
     """A wrapper that provides a function to modify the action passed to :meth:`step`."""
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         func: Callable[[WrapperActType], ActType],
         action_space: Space[WrapperActType] | None,
     ):
         """Initialize LambdaAction.
 
         Args:
-            env: The gymnasium environment
-            func: Function to apply to ``step`` ``action``
+            env: The environment to wrap
+            func: Function to apply to the :meth:`step`'s ``action``
             action_space: The updated action space of the wrapper given the function.
         """
         gym.utils.RecordConstructorArgs.__init__(
             self, func=func, action_space=action_space
         )
         gym.Wrapper.__init__(self, env)
 
@@ -71,23 +69,23 @@
         ... # Executes the action np.array([1.0, -1.0, 0]) in the base environment
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType]):
         """A wrapper for clipping continuous actions within the valid bound.
 
         Args:
-            env: The environment to apply the wrapper
+            env: The environment to wrap
         """
         assert isinstance(env.action_space, Box)
 
         gym.utils.RecordConstructorArgs.__init__(self)
         LambdaActionV0.__init__(
             self,
             env=env,
-            func=lambda action: jp.clip(
+            func=lambda action: np.clip(
                 action, env.action_space.low, env.action_space.high
             ),
             action_space=Box(
                 -np.inf,
                 np.inf,
                 shape=env.action_space.shape,
                 dtype=env.action_space.dtype,
@@ -121,18 +119,18 @@
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         min_action: float | int | np.ndarray,
         max_action: float | int | np.ndarray,
     ):
-        """Initializes the :class:`RescaleAction` wrapper.
+        """Constructor for the Rescale Action wrapper.
 
         Args:
-            env (Env): The environment to apply the wrapper
+            env (Env): The environment to wrap
             min_action (float, int or np.ndarray): The min values for each action. This may be a numpy array or a scalar.
             max_action (float, int or np.ndarray): The max values for each action. This may be a numpy array or a scalar.
         """
         gym.utils.RecordConstructorArgs.__init__(
             self, min_action=min_action, max_action=max_action
         )
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/lambda_observations.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/lambda_observation.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,48 @@
 * ``FlattenObservationV0`` - Flattens the observations
 * ``GrayscaleObservationV0`` - Converts a RGB observation to a grayscale observation
 * ``ResizeObservationV0`` - Resizes an array-based observation (normally a RGB observation)
 * ``ReshapeObservationV0`` - Reshapes an array-based observation
 * ``RescaleObservationV0`` - Rescales an observation to between a minimum and maximum value
 * ``DtypeObservationV0`` - Convert an observation to a dtype
 * ``PixelObservationV0`` - Allows the observation to the rendered frame
-* ``NormalizeObservationV0`` - Normalized the observations to a mean and
 """
 from __future__ import annotations
 
-from typing import Any, Callable, Sequence
-from typing_extensions import Final
+from typing import Any, Callable, Final, Sequence
 
-
-try:
-    import jumpy.numpy as jp
-except ImportError as e:
-    raise ImportError("Jumpy is not installed, run `pip install jax-jumpy`") from e
 import numpy as np
 
 import gymnasium as gym
 from gymnasium import spaces
 from gymnasium.core import ActType, ObsType, WrapperObsType
 from gymnasium.error import DependencyNotInstalled
-from gymnasium.experimental.wrappers.utils import RunningMeanStd
+
+
+__all__ = [
+    "LambdaObservationV0",
+    "FilterObservationV0",
+    "FlattenObservationV0",
+    "GrayscaleObservationV0",
+    "ResizeObservationV0",
+    "ReshapeObservationV0",
+    "RescaleObservationV0",
+    "DtypeObservationV0",
+    "PixelObservationV0",
+]
 
 
 class LambdaObservationV0(
     gym.ObservationWrapper[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
     """Transforms an observation via a function provided to the wrapper.
 
     The function :attr:`func` will be applied to all observations.
-    If the observations from :attr:`func` are outside the bounds of the `env` spaces, provide a :attr:`observation_space`.
+    If the observations from :attr:`func` are outside the bounds of the ``env``'s observation space, provide an :attr:`observation_space`.
 
     Example:
         >>> import gymnasium as gym
         >>> from gymnasium.experimental.wrappers import LambdaObservationV0
         >>> import numpy as np
         >>> np.random.seed(0)
         >>> env = gym.make("CartPole-v1")
@@ -56,16 +61,16 @@
         func: Callable[[ObsType], Any],
         observation_space: gym.Space[WrapperObsType] | None,
     ):
         """Constructor for the lambda observation wrapper.
 
         Args:
             env: The environment to wrap
-            func: A function that will transform an observation. If this transformed observation is outside the observation space of `env.observation_space` then provide an `observation_space`.
-            observation_space: The observation spaces of the wrapper, if None, then it is assumed the same as `env.observation_space`.
+            func: A function that will transform an observation. If this transformed observation is outside the observation space of ``env.observation_space`` then provide an `observation_space`.
+            observation_space: The observation spaces of the wrapper, if None, then it is assumed the same as ``env.observation_space``.
         """
         gym.utils.RecordConstructorArgs.__init__(
             self, func=func, observation_space=observation_space
         )
         gym.ObservationWrapper.__init__(self, env)
 
         if observation_space is not None:
@@ -78,15 +83,15 @@
         return self.func(observation)
 
 
 class FilterObservationV0(
     LambdaObservationV0[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Filter Dict observation space by the keys.
+    """Filters Dict or Tuple observation space by the keys or indexes.
 
     Example:
         >>> import gymnasium as gym
         >>> from gymnasium.wrappers import TransformObservation
         >>> from gymnasium.experimental.wrappers import FilterObservationV0
         >>> env = gym.make("CartPole-v1")
         >>> env = gym.wrappers.TransformObservation(env, lambda obs: {'obs': obs, 'time': 0})
@@ -99,15 +104,20 @@
         >>> env.step(0)
         ({'time': 0}, 1.0, False, False, {})
     """
 
     def __init__(
         self, env: gym.Env[ObsType, ActType], filter_keys: Sequence[str | int]
     ):
-        """Constructor for an environment with a dictionary observation space where all :attr:`filter_keys` are in the observation space keys."""
+        """Constructor for the filter observation wrapper.
+
+        Args:
+            env: The environment to wrap
+            filter_keys: The subspaces to be included, use a list of strings or integers for ``Dict`` and ``Tuple`` spaces respectivesly
+        """
         assert isinstance(filter_keys, Sequence)
         gym.utils.RecordConstructorArgs.__init__(self, filter_keys=filter_keys)
 
         # Filters for dictionary space
         if isinstance(env.observation_space, spaces.Dict):
             assert all(isinstance(key, str) for key in filter_keys)
 
@@ -173,15 +183,15 @@
                 self,
                 env=env,
                 func=lambda obs: tuple(obs[key] for key in filter_keys),
                 observation_space=new_observation_spaces,
             )
         else:
             raise ValueError(
-                f"FilterObservation wrapper is only usable with ``Dict`` and ``Tuple`` observations, actual type: {type(env.observation_space)}"
+                f"FilterObservation wrapper is only usable with `Dict` and `Tuple` observations, actual type: {type(env.observation_space)}"
             )
 
         self.filter_keys: Final[Sequence[str | int]] = filter_keys
 
 
 class FlattenObservationV0(
     LambdaObservationV0[WrapperObsType, ActType, ObsType],
@@ -200,15 +210,19 @@
         (27648,)
         >>> obs, _ = env.reset()
         >>> obs.shape
         (27648,)
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType]):
-        """Constructor for any environment's observation space that implements ``spaces.utils.flatten_space`` and ``spaces.utils.flatten``."""
+        """Constructor for any environment's observation space that implements ``spaces.utils.flatten_space`` and ``spaces.utils.flatten``.
+
+        Args:
+            env:  The environment to wrap
+        """
         gym.utils.RecordConstructorArgs.__init__(self)
         LambdaObservationV0.__init__(
             self,
             env=env,
             func=lambda obs: spaces.utils.flatten(env.observation_space, obs),
             observation_space=spaces.utils.flatten_space(env.observation_space),
         )
@@ -233,15 +247,20 @@
         (96, 96)
         >>> grayscale_env = GrayscaleObservationV0(env, keep_dim=True)
         >>> grayscale_env.observation_space.shape
         (96, 96, 1)
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], keep_dim: bool = False):
-        """Constructor for an RGB image based environments to make the image grayscale."""
+        """Constructor for an RGB image based environments to make the image grayscale.
+
+        Args:
+            env: The environment to wrap
+            keep_dim: If to keep the channel in the observation, if ``True``, ``obs.shape == 3`` else ``obs.shape == 2``
+        """
         assert isinstance(env.observation_space, spaces.Box)
         assert (
             len(env.observation_space.shape) == 3
             and env.observation_space.shape[-1] == 3
         )
         assert (
             np.all(env.observation_space.low == 0)
@@ -257,31 +276,31 @@
                 high=255,
                 shape=env.observation_space.shape[:2] + (1,),
                 dtype=np.uint8,
             )
             LambdaObservationV0.__init__(
                 self,
                 env=env,
-                func=lambda obs: jp.expand_dims(
-                    jp.sum(
-                        jp.multiply(obs, jp.array([0.2125, 0.7154, 0.0721])), axis=-1
+                func=lambda obs: np.expand_dims(
+                    np.sum(
+                        np.multiply(obs, np.array([0.2125, 0.7154, 0.0721])), axis=-1
                     ).astype(np.uint8),
                     axis=-1,
                 ),
                 observation_space=new_observation_space,
             )
         else:
             new_observation_space = spaces.Box(
                 low=0, high=255, shape=env.observation_space.shape[:2], dtype=np.uint8
             )
             LambdaObservationV0.__init__(
                 self,
                 env=env,
-                func=lambda obs: jp.sum(
-                    jp.multiply(obs, jp.array([0.2125, 0.7154, 0.0721])), axis=-1
+                func=lambda obs: np.sum(
+                    np.multiply(obs, np.array([0.2125, 0.7154, 0.0721])), axis=-1
                 ).astype(np.uint8),
                 observation_space=new_observation_space,
             )
 
 
 class ResizeObservationV0(
     LambdaObservationV0[WrapperObsType, ActType, ObsType],
@@ -297,15 +316,20 @@
         (96, 96, 3)
         >>> resized_env = ResizeObservationV0(env, (32, 32))
         >>> resized_env.observation_space.shape
         (32, 32, 3)
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], shape: tuple[int, ...]):
-        """Constructor that requires an image environment observation space with a shape."""
+        """Constructor that requires an image environment observation space with a shape.
+
+        Args:
+            env: The environment to wrap
+            shape: The resized observation shape
+        """
         assert isinstance(env.observation_space, spaces.Box)
         assert len(env.observation_space.shape) in [2, 3]
         assert np.all(env.observation_space.low == 0) and np.all(
             env.observation_space.high == 255
         )
         assert env.observation_space.dtype == np.uint8
 
@@ -319,15 +343,18 @@
             raise DependencyNotInstalled(
                 "opencv (cv2) is not installed, run `pip install gymnasium[other]`"
             ) from e
 
         self.shape: Final[tuple[int, ...]] = tuple(shape)
 
         new_observation_space = spaces.Box(
-            low=0, high=255, shape=self.shape + env.observation_space.shape[2:]
+            low=0,
+            high=255,
+            shape=self.shape + env.observation_space.shape[2:],
+            dtype=np.uint8,
         )
 
         gym.utils.RecordConstructorArgs.__init__(self, shape=shape)
         LambdaObservationV0.__init__(
             self,
             env=env,
             func=lambda obs: cv2.resize(obs, self.shape, interpolation=cv2.INTER_AREA),
@@ -349,15 +376,20 @@
         (96, 96, 3)
         >>> reshape_env = ReshapeObservationV0(env, (24, 4, 96, 1, 3))
         >>> reshape_env.observation_space.shape
         (24, 4, 96, 1, 3)
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], shape: int | tuple[int, ...]):
-        """Constructor for env with Box observation space that has a shape product equal to the new shape product."""
+        """Constructor for env with ``Box`` observation space that has a shape product equal to the new shape product.
+
+        Args:
+            env: The environment to wrap
+            shape: The reshaped observation space
+        """
         assert isinstance(env.observation_space, spaces.Box)
         assert np.product(shape) == np.product(env.observation_space.shape)
 
         assert isinstance(shape, tuple)
         assert all(np.issubdtype(type(elem), np.integer) for elem in shape)
         assert all(x > 0 or x == -1 for x in shape)
 
@@ -369,15 +401,15 @@
         )
         self.shape = shape
 
         gym.utils.RecordConstructorArgs.__init__(self, shape=shape)
         LambdaObservationV0.__init__(
             self,
             env=env,
-            func=lambda obs: jp.reshape(obs, shape),
+            func=lambda obs: np.reshape(obs, shape),
             observation_space=new_observation_space,
         )
 
 
 class RescaleObservationV0(
     LambdaObservationV0[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
@@ -397,15 +429,21 @@
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         min_obs: np.floating | np.integer | np.ndarray,
         max_obs: np.floating | np.integer | np.ndarray,
     ):
-        """Constructor that requires the env observation spaces to be a :class:`Box`."""
+        """Constructor that requires the env observation spaces to be a :class:`Box`.
+
+        Args:
+            env: The environment to wrap
+            min_obs: The new minimum observation bound
+            max_obs: The new maximum observation bound
+        """
         assert isinstance(env.observation_space, spaces.Box)
         assert not np.any(env.observation_space.low == np.inf) and not np.any(
             env.observation_space.high == np.inf
         )
 
         if not isinstance(min_obs, np.ndarray):
             assert np.issubdtype(type(min_obs), np.integer) or np.issubdtype(
@@ -448,18 +486,27 @@
         )
 
 
 class DtypeObservationV0(
     LambdaObservationV0[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Observation wrapper for transforming the dtype of an observation."""
+    """Observation wrapper for transforming the dtype of an observation.
+
+    Note:
+        This is only compatible with :class:`Box`, :class:`Discrete`, :class:`MultiDiscrete` and :class:`MultiBinary` observation spaces
+    """
 
     def __init__(self, env: gym.Env[ObsType, ActType], dtype: Any):
-        """Constructor for Dtype, this is only valid with :class:`Box`, :class:`Discrete`, :class:`MultiDiscrete` and :class:`MultiBinary` observation spaces."""
+        """Constructor for Dtype observation wrapper.
+
+        Args:
+            env: The environment to wrap
+            dtype: The new dtype of the observation
+        """
         assert isinstance(
             env.observation_space,
             (spaces.Box, spaces.Discrete, spaces.MultiDiscrete, spaces.MultiBinary),
         )
 
         self.dtype = dtype
         if isinstance(env.observation_space, spaces.Box):
@@ -501,15 +548,15 @@
         )
 
 
 class PixelObservationV0(
     LambdaObservationV0[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Augment observations by pixel values.
+    """Includes the rendered observations to the environment's observations.
 
     Observations of this wrapper will be dictionaries of images.
     You can also choose to add the observation of the base environment to this dictionary.
     In that case, if the base environment has an observation space of type :class:`Dict`, the dictionary
     of rendered images will be updated with the base environment's observation. If, however, the observation
     space is of type :class:`Box`, the base environment's observation (which will be an element of the :class:`Box`
     space) will be added to the dictionary under the key "state".
@@ -518,21 +565,21 @@
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         pixels_only: bool = True,
         pixels_key: str = "pixels",
         obs_key: str = "state",
     ):
-        """Initializes a new pixel Wrapper.
+        """Constructor of the pixel observation wrapper.
 
         Args:
             env: The environment to wrap.
-            pixels_only (bool): If `True` (default), the original observation returned
+            pixels_only (bool): If ``True`` (default), the original observation returned
                 by the wrapped environment will be discarded, and a dictionary
-                observation will only include pixels. If `False`, the
+                observation will only include pixels. If ``False``, the
                 observation dictionary will contain both the original
                 observations and the pixel observations.
             pixels_key: Optional custom string specifying the pixel key. Defaults to "pixels"
             obs_key: Optional custom string specifying the obs key. Defaults to "state"
         """
         gym.utils.RecordConstructorArgs.__init__(
             self, pixels_only=pixels_only, pixels_key=pixels_key, obs_key=obs_key
@@ -567,55 +614,7 @@
             )
             LambdaObservationV0.__init__(
                 self,
                 env=env,
                 func=lambda obs: {obs_key: obs, pixels_key: self.render()},
                 observation_space=obs_space,
             )
-
-
-class NormalizeObservationV0(
-    gym.ObservationWrapper[WrapperObsType, ActType, ObsType],
-    gym.utils.RecordConstructorArgs,
-):
-    """This wrapper will normalize observations s.t. each coordinate is centered with unit variance.
-
-    The property `_update_running_mean` allows to freeze/continue the running mean calculation of the observation
-    statistics. If `True` (default), the `RunningMeanStd` will get updated every time `self.observation()` is called.
-    If `False`, the calculated statistics are used but not updated anymore; this may be used during evaluation.
-
-    Note:
-        The normalization depends on past trajectories and observations will not be normalized correctly if the wrapper was
-        newly instantiated or the policy was changed recently.
-    """
-
-    def __init__(self, env: gym.Env[ObsType, ActType], epsilon: float = 1e-8):
-        """This wrapper will normalize observations s.t. each coordinate is centered with unit variance.
-
-        Args:
-            env (Env): The environment to apply the wrapper
-            epsilon: A stability parameter that is used when scaling the observations.
-        """
-        gym.utils.RecordConstructorArgs.__init__(self, epsilon=epsilon)
-        gym.ObservationWrapper.__init__(self, env)
-
-        self.obs_rms = RunningMeanStd(shape=self.observation_space.shape)
-        self.epsilon = epsilon
-        self._update_running_mean = True
-
-    @property
-    def update_running_mean(self) -> bool:
-        """Property to freeze/continue the running mean calculation of the observation statistics."""
-        return self._update_running_mean
-
-    @update_running_mean.setter
-    def update_running_mean(self, setting: bool):
-        """Sets the property to freeze/continue the running mean calculation of the observation statistics."""
-        self._update_running_mean = setting
-
-    def observation(self, observation: ObsType) -> WrapperObsType:
-        """Normalises the observation using the running mean and variance of the observations."""
-        if self._update_running_mean:
-            self.obs_rms.update(observation)
-        return (observation - self.obs_rms.mean) / np.sqrt(
-            self.obs_rms.var + self.epsilon
-        )
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/numpy_to_torch.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/numpy_to_torch.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Device = Union[str, torch.device]
 except ImportError:
     raise DependencyNotInstalled(
         "Torch is not installed therefore cannot call `torch_to_numpy`, run `pip install torch`"
     )
 
 
-__all__ = ["torch_to_numpy", "numpy_to_torch", "NumpyToTorchV0"]
+__all__ = ["NumpyToTorchV0", "torch_to_numpy", "numpy_to_torch"]
 
 
 @functools.singledispatch
 def torch_to_numpy(value: Any) -> Any:
     """Converts a PyTorch Tensor into a NumPy Array."""
     raise Exception(
         f"No known conversion for Torch type ({type(value)}) to NumPy registered. Report as issue on github."
@@ -39,55 +39,55 @@
 def _number_torch_to_numpy(value: numbers.Number | torch.Tensor) -> Any:
     """Convert a python number (int, float, complex) and torch.Tensor to a numpy array."""
     return np.array(value)
 
 
 @torch_to_numpy.register(abc.Mapping)
 def _mapping_torch_to_numpy(value: Mapping[str, Any]) -> Mapping[str, Any]:
-    """Converts a mapping of PyTorch Tensors into a Dictionary of Jax DeviceArrays."""
+    """Converts a mapping of PyTorch Tensors into a Dictionary of Jax Array."""
     return type(value)(**{k: torch_to_numpy(v) for k, v in value.items()})
 
 
 @torch_to_numpy.register(abc.Iterable)
 def _iterable_torch_to_numpy(value: Iterable[Any]) -> Iterable[Any]:
-    """Converts an Iterable from PyTorch Tensors to an iterable of Jax DeviceArrays."""
+    """Converts an Iterable from PyTorch Tensors to an iterable of Jax Array."""
     return type(value)(torch_to_numpy(v) for v in value)
 
 
 @functools.singledispatch
 def numpy_to_torch(value: Any, device: Device | None = None) -> Any:
-    """Converts a Jax DeviceArray into a PyTorch Tensor."""
+    """Converts a Jax Array into a PyTorch Tensor."""
     raise Exception(
         f"No known conversion for NumPy type ({type(value)}) to PyTorch registered. Report as issue on github."
     )
 
 
 @numpy_to_torch.register(np.ndarray)
 def _numpy_to_torch(value: np.ndarray, device: Device | None = None) -> torch.Tensor:
-    """Converts a Jax DeviceArray into a PyTorch Tensor."""
+    """Converts a Jax Array into a PyTorch Tensor."""
     assert torch is not None
     tensor = torch.tensor(value)
     if device:
         return tensor.to(device=device)
     return tensor
 
 
 @numpy_to_torch.register(abc.Mapping)
 def _numpy_mapping_to_torch(
     value: Mapping[str, Any], device: Device | None = None
 ) -> Mapping[str, Any]:
-    """Converts a mapping of Jax DeviceArrays into a Dictionary of PyTorch Tensors."""
+    """Converts a mapping of Jax Array into a Dictionary of PyTorch Tensors."""
     return type(value)(**{k: numpy_to_torch(v, device) for k, v in value.items()})
 
 
 @numpy_to_torch.register(abc.Iterable)
 def _numpy_iterable_to_torch(
     value: Iterable[Any], device: Device | None = None
 ) -> Iterable[Any]:
-    """Converts an Iterable from Jax DeviceArrays to an iterable of PyTorch Tensors."""
+    """Converts an Iterable from Jax Array to an iterable of PyTorch Tensors."""
     return type(value)(numpy_to_torch(v, device) for v in value)
 
 
 class NumpyToTorchV0(gym.Wrapper, gym.utils.RecordConstructorArgs):
     """Wraps a numpy-based environment so that it can be interacted with through PyTorch Tensors.
 
     Actions must be provided as PyTorch Tensors and observations will be returned as PyTorch Tensors.
@@ -107,21 +107,21 @@
         gym.Wrapper.__init__(self, env)
 
         self.device: Device | None = device
 
     def step(
         self, action: WrapperActType
     ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict]:
-        """Performs the given action within the environment.
+        """Using a PyTorch based action that is converted to NumPy to be used by the environment.
 
         Args:
-            action: The action to perform as a PyTorch Tensor
+            action: A PyTorch-based action
 
         Returns:
-            The next observation, reward, termination, truncation, and extra info
+            The PyTorch-based Tensor next observation, reward, termination, truncation, and extra info
         """
         jax_action = torch_to_numpy(action)
         obs, reward, terminated, truncated, info = self.env.step(jax_action)
 
         return (
             numpy_to_torch(obs, self.device),
             float(reward),
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/rendering.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 import gymnasium as gym
 from gymnasium import error, logger
 from gymnasium.core import ActType, ObsType, RenderFrame
 from gymnasium.error import DependencyNotInstalled
 
 
+__all__ = ["RenderCollectionV0", "RecordVideoV0", "HumanRenderingV0"]
+
+
 class RenderCollectionV0(
     gym.Wrapper[ObsType, ActType, ObsType, ActType], gym.utils.RecordConstructorArgs
 ):
     """Collect rendered frames of an environment such ``render`` returns a ``list[RenderedFrame]``."""
 
     def __init__(
         self,
@@ -96,58 +99,52 @@
     They should be functions returning a boolean that indicates whether a recording should be started at the
     current episode or step, respectively.
     If neither :attr:`episode_trigger` nor ``step_trigger`` is passed, a default ``episode_trigger`` will be employed,
     i.e. capped_cubic_video_schedule. This function starts a video at every episode that is a power of 3 until 1000 and
     then every 1000 episodes.
     By default, the recording will be stopped once reset is called. However, you can also create recordings of fixed
     length (possibly spanning several episodes) by passing a strictly positive value for ``video_length``.
-    This wrapper uses the value `fps` from metadata as the number of frames per second;
-    if `fps` is not defined in metadata, the default value 30 is used.
     """
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         video_folder: str,
         episode_trigger: Callable[[int], bool] | None = None,
         step_trigger: Callable[[int], bool] | None = None,
         video_length: int = 0,
         name_prefix: str = "rl-video",
+        fps: int | None = None,
         disable_logger: bool = False,
     ):
         """Wrapper records videos of rollouts.
 
         Args:
             env: The environment that will be wrapped
             video_folder (str): The folder where the recordings will be stored
             episode_trigger: Function that accepts an integer and returns ``True`` iff a recording should be started at this episode
             step_trigger: Function that accepts an integer and returns ``True`` iff a recording should be started at this step
             video_length (int): The length of recorded episodes. If 0, entire episodes are recorded.
                 Otherwise, snippets of the specified length are captured
             name_prefix (str): Will be prepended to the filename of the recordings
+            fps (int): The frame per second in the video. The default value is the one specified in the environment metadata.
+                If the environment metadata doesn't specify `render_fps`, the value 30 is used.
             disable_logger (bool): Whether to disable moviepy logger or not
         """
         gym.utils.RecordConstructorArgs.__init__(
             self,
             video_folder=video_folder,
             episode_trigger=episode_trigger,
             step_trigger=step_trigger,
             video_length=video_length,
             name_prefix=name_prefix,
             disable_logger=disable_logger,
         )
         gym.Wrapper.__init__(self, env)
 
-        try:
-            import moviepy  # noqa: F401
-        except ImportError as e:
-            raise error.DependencyNotInstalled(
-                "MoviePy is not installed, run `pip install moviepy`"
-            ) from e
-
         if env.render_mode in {None, "human", "ansi"}:
             raise ValueError(
                 f"Render mode is {env.render_mode}, which is incompatible with RecordVideo.",
                 "Initialize your environment with a render_mode that returns an image, such as rgb_array.",
             )
 
         if episode_trigger is None and step_trigger is None:
@@ -168,25 +165,34 @@
         if os.path.isdir(self.video_folder):
             logger.warn(
                 f"Overwriting existing videos at {self.video_folder} folder "
                 f"(try specifying a different `video_folder` for the `RecordVideo` wrapper if this is not desired)"
             )
         os.makedirs(self.video_folder, exist_ok=True)
 
+        if fps is None:
+            fps = self.metadata.get("render_fps", 30)
+        self.frames_per_sec: int = fps
         self.name_prefix: str = name_prefix
         self._video_name: str | None = None
-        self.frames_per_sec: int = self.metadata.get("render_fps", 30)
         self.video_length: int = video_length if video_length != 0 else float("inf")
         self.recording: bool = False
         self.recorded_frames: list[RenderFrame] = []
         self.render_history: list[RenderFrame] = []
 
         self.step_id = -1
         self.episode_id = -1
 
+        try:
+            import moviepy  # noqa: F401
+        except ImportError as e:
+            raise error.DependencyNotInstalled(
+                "MoviePy is not installed, run `pip install moviepy`"
+            ) from e
+
     def _capture_frame(self):
         assert self.recording, "Cannot capture a frame, recording wasn't started."
 
         frame = self.env.render()
         if isinstance(frame, List):
             if len(frame) == 0:  # render was called
                 return
@@ -313,15 +319,15 @@
         >>> wrapped = HumanRenderingV0(env)
         >>> obs, _ = wrapped.reset()     # This will start rendering to the screen
 
         The wrapper can also be applied directly when the environment is instantiated, simply by passing
         ``render_mode="human"`` to ``make``. The wrapper will only be applied if the environment does not
         implement human-rendering natively (i.e. ``render_mode`` does not contain ``"human"``).
 
-        >>> env = gym.make("CartPoleJax-v1", render_mode="human")      # CartPoleJax-v1 doesn't implement human-rendering natively
+        >>> env = gym.make("phys2d/CartPole-v1", render_mode="human")      # CartPoleJax-v1 doesn't implement human-rendering natively
         >>> obs, _ = env.reset()     # This will start rendering to the screen
 
         Warning: If the base environment uses ``render_mode="rgb_array_list"``, its (i.e. the *base environment's*) render method
         will always return an empty list:
 
         >>> env = gym.make("LunarLander-v2", render_mode="rgb_array_list")
         >>> wrapped = HumanRenderingV0(env)
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/stateful_action.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/stateful_action.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from typing import Any
 
 import gymnasium as gym
 from gymnasium.core import ActType, ObsType
 from gymnasium.error import InvalidProbability
 
 
+__all__ = ["StickyActionV0"]
+
+
 class StickyActionV0(
     gym.ActionWrapper[ObsType, ActType, ActType], gym.utils.RecordConstructorArgs
 ):
     """Wrapper which adds a probability of repeating the previous action.
 
     This wrapper follows the implementation proposed by `Machado et al., 2018 <https://arxiv.org/pdf/1709.06009.pdf>`_
     in Section 5.2 on page 12.
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/stateful_observation.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/stateful_observation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """A collection of stateful observation wrappers.
 
 * ``DelayObservationV0`` - A wrapper for delaying the returned observation
 * ``TimeAwareObservationV0`` - A wrapper for adding time aware observations to environment observation
 * ``FrameStackObservationV0`` - Frame stack the observations
+* ``NormalizeObservationV0`` - Normalized the observations to a mean and
+* ``MaxAndSkipObservationV0`` - Return only every ``skip``-th frame (frameskipping) and return the max between the two last frames.
 """
 from __future__ import annotations
 
 from collections import deque
 from copy import deepcopy
-from typing import Any, SupportsFloat
-from typing_extensions import Final
+from typing import Any, Final, SupportsFloat
 
 import numpy as np
 
 import gymnasium as gym
 import gymnasium.spaces as spaces
 from gymnasium.core import ActType, ObsType, WrapperActType, WrapperObsType
 from gymnasium.experimental.vector.utils import (
     batch_space,
     concatenate,
     create_empty_array,
 )
-from gymnasium.experimental.wrappers.utils import create_zero_array
+from gymnasium.experimental.wrappers.utils import RunningMeanStd, create_zero_array
 from gymnasium.spaces import Box, Dict, Tuple
 
 
+__all__ = [
+    "DelayObservationV0",
+    "TimeAwareObservationV0",
+    "FrameStackObservationV0",
+    "NormalizeObservationV0",
+]
+
+
 class DelayObservationV0(
     gym.ObservationWrapper[ObsType, ActType, ObsType], gym.utils.RecordConstructorArgs
 ):
     """Wrapper which adds a delay to the returned observation.
 
     Before reaching the :attr:`delay` number of timesteps, returned observations is an array of zeros with
     the same shape as the observation space.
@@ -172,17 +181,16 @@
             dict_time_key=dict_time_key,
         )
         gym.ObservationWrapper.__init__(self, env)
 
         self.flatten: Final[bool] = flatten
         self.normalize_time: Final[bool] = normalize_time
 
-        if hasattr(env, "_max_episode_steps"):
-            self.max_timesteps = getattr(env, "_max_episode_steps")
-        elif env.spec is not None and env.spec.max_episode_steps is not None:
+        # We don't need to keep if a TimeLimit wrapper exists as `spec` will do that work for us now
+        if env.spec is not None and env.spec.max_episode_steps is not None:
             self.max_timesteps = env.spec.max_episode_steps
         else:
             raise ValueError(
                 "The environment must be wrapped by a TimeLimit wrapper or the spec specify a `max_episode_steps`."
             )
 
         self._timesteps: int = 0
@@ -378,7 +386,120 @@
 
         updated_obs = deepcopy(
             concatenate(
                 self.env.observation_space, self._stacked_obs, self._stacked_array
             )
         )
         return updated_obs, info
+
+
+class NormalizeObservationV0(
+    gym.ObservationWrapper[WrapperObsType, ActType, ObsType],
+    gym.utils.RecordConstructorArgs,
+):
+    """This wrapper will normalize observations s.t. each coordinate is centered with unit variance.
+
+    The property `_update_running_mean` allows to freeze/continue the running mean calculation of the observation
+    statistics. If `True` (default), the `RunningMeanStd` will get updated every time `self.observation()` is called.
+    If `False`, the calculated statistics are used but not updated anymore; this may be used during evaluation.
+
+    Note:
+        The normalization depends on past trajectories and observations will not be normalized correctly if the wrapper was
+        newly instantiated or the policy was changed recently.
+    """
+
+    def __init__(self, env: gym.Env[ObsType, ActType], epsilon: float = 1e-8):
+        """This wrapper will normalize observations s.t. each coordinate is centered with unit variance.
+
+        Args:
+            env (Env): The environment to apply the wrapper
+            epsilon: A stability parameter that is used when scaling the observations.
+        """
+        gym.utils.RecordConstructorArgs.__init__(self, epsilon=epsilon)
+        gym.ObservationWrapper.__init__(self, env)
+
+        self.obs_rms = RunningMeanStd(shape=self.observation_space.shape)
+        self.epsilon = epsilon
+        self._update_running_mean = True
+
+    @property
+    def update_running_mean(self) -> bool:
+        """Property to freeze/continue the running mean calculation of the observation statistics."""
+        return self._update_running_mean
+
+    @update_running_mean.setter
+    def update_running_mean(self, setting: bool):
+        """Sets the property to freeze/continue the running mean calculation of the observation statistics."""
+        self._update_running_mean = setting
+
+    def observation(self, observation: ObsType) -> WrapperObsType:
+        """Normalises the observation using the running mean and variance of the observations."""
+        if self._update_running_mean:
+            self.obs_rms.update(observation)
+        return (observation - self.obs_rms.mean) / np.sqrt(
+            self.obs_rms.var + self.epsilon
+        )
+
+
+class MaxAndSkipObservationV0(
+    gym.Wrapper[WrapperObsType, ActType, ObsType, ActType],
+    gym.utils.RecordConstructorArgs,
+):
+    """This wrapper will return only every ``skip``-th frame (frameskipping) and return the max between the two last observations.
+
+    Note: This wrapper is based on the wrapper from stable-baselines3: https://stable-baselines3.readthedocs.io/en/master/_modules/stable_baselines3/common/atari_wrappers.html#MaxAndSkipEnv
+    """
+
+    def __init__(self, env: gym.Env[ObsType, ActType], skip: int = 4):
+        """This wrapper will return only every ``skip``-th frame (frameskipping) and return the max between the two last frames.
+
+        Args:
+            env (Env): The environment to apply the wrapper
+            skip: The number of frames to skip
+        """
+        gym.utils.RecordConstructorArgs.__init__(self, skip=skip)
+        gym.Wrapper.__init__(self, env)
+
+        if not np.issubdtype(type(skip), np.integer):
+            raise TypeError(
+                f"The skip is expected to be an integer, actual type: {type(skip)}"
+            )
+        if skip < 2:
+            raise ValueError(
+                f"The skip value needs to be equal or greater than two, actual value: {skip}"
+            )
+        if env.observation_space.shape is None:
+            raise ValueError("The observation space must have the shape attribute.")
+
+        self._skip = skip
+        self._obs_buffer = np.zeros(
+            (2, *env.observation_space.shape), dtype=env.observation_space.dtype
+        )
+
+    def step(
+        self, action: WrapperActType
+    ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict[str, Any]]:
+        """Step the environment with the given action for ``skip`` steps.
+
+        Repeat action, sum reward, and max over last observations.
+
+        Args:
+            action: The action to step through the environment with
+        Returns:
+            Max of the last two observations, reward, terminated, truncated, and info from the environment
+        """
+        total_reward = 0.0
+        terminated = truncated = False
+        info = {}
+        for i in range(self._skip):
+            obs, reward, terminated, truncated, info = self.env.step(action)
+            done = terminated or truncated
+            if i == self._skip - 2:
+                self._obs_buffer[0] = obs
+            if i == self._skip - 1:
+                self._obs_buffer[1] = obs
+            total_reward += float(reward)
+            if done:
+                break
+        max_frame = self._obs_buffer.max(axis=0)
+
+        return max_frame, total_reward, terminated, truncated, info
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/utils.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     Sequence,
     Text,
     Tuple,
 )
 from gymnasium.spaces.space import T_cov
 
 
+__all__ = ["RunningMeanStd", "update_mean_var_count_from_moments", "create_zero_array"]
+
+
 class RunningMeanStd:
     """Tracks the mean, variance and count of values."""
 
     # https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Parallel_algorithm
     def __init__(self, epsilon=1e-4, shape=()):
         """Tracks the mean, variance and count of values."""
         self.mean = np.zeros(shape, "float64")
@@ -95,16 +98,20 @@
 
 @create_zero_array.register(Discrete)
 def _create_discrete_zero_array(space: Discrete):
     return space.start
 
 
 @create_zero_array.register(MultiDiscrete)
+def _create_multidiscrete_zero_array(space: MultiDiscrete):
+    return np.array(space.start, copy=True, dtype=space.dtype)
+
+
 @create_zero_array.register(MultiBinary)
-def _create_array_zero_array(space: Discrete):
+def _create_array_zero_array(space: MultiBinary):
     return np.zeros(space.shape, dtype=space.dtype)
 
 
 @create_zero_array.register(Tuple)
 def _create_tuple_zero_array(space: Tuple):
     return tuple(create_zero_array(subspace) for subspace in space.spaces)
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/vector/record_episode_statistics.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/vector/record_episode_statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Wrapper that tracks the cumulative rewards and episode lengths."""
+from __future__ import annotations
+
 import time
 from collections import deque
-from typing import List, Optional, Union
 
 import numpy as np
 
-from gymnasium.experimental.vector.vector_env import VectorEnv, VectorWrapper
+from gymnasium.core import ActType, ObsType
+from gymnasium.experimental.vector.vector_env import ArrayType, VectorEnv, VectorWrapper
+
 
+__all__ = ["RecordEpisodeStatisticsV0"]
 
-class VectorRecordEpisodeStatistics(VectorWrapper):
+
+class RecordEpisodeStatisticsV0(VectorWrapper):
     """This wrapper will keep track of cumulative rewards and episode lengths.
 
     At the end of an episode, the statistics of the episode will be added to ``info``
     using the key ``episode``. If using a vectorized environment also the key
     ``_episode`` is used which indicates whether the env at the respective index has
     the episode statistics.
 
@@ -28,17 +33,17 @@
         ... }
 
     For a vectorized environments the output will be in the form of::
 
         >>> infos = {  # doctest: +SKIP
         ...     ...
         ...     "episode": {
-        ...         "r": "<array of cumulative reward>",
-        ...         "l": "<array of episode length>",
-        ...         "t": "<array of elapsed time since beginning of episode>"
+        ...         "r": "<array of cumulative reward for each done sub-environment>",
+        ...         "l": "<array of episode length for each done sub-environment>",
+        ...         "t": "<array of elapsed time since beginning of episode for each done sub-environment>"
         ...     },
         ...     "_episode": "<boolean array of length num-envs>"
         ... }
 
     Moreover, the most recent rewards and episode lengths are stored in buffers that can be accessed via
     :attr:`wrapped_env.return_queue` and :attr:`wrapped_env.length_queue` respectively.
 
@@ -51,53 +56,62 @@
         """This wrapper will keep track of cumulative rewards and episode lengths.
 
         Args:
             env (Env): The environment to apply the wrapper
             deque_size: The size of the buffers :attr:`return_queue` and :attr:`length_queue`
         """
         super().__init__(env)
-        self.num_envs = getattr(env, "num_envs", 1)
+
         self.episode_count = 0
-        self.episode_start_times: np.ndarray = None
-        self.episode_returns: Optional[np.ndarray] = None
-        self.episode_lengths: Optional[np.ndarray] = None
+
+        self.episode_start_times: np.ndarray = np.zeros(())
+        self.episode_returns: np.ndarray = np.zeros(())
+        self.episode_lengths: np.ndarray = np.zeros(())
+
         self.return_queue = deque(maxlen=deque_size)
         self.length_queue = deque(maxlen=deque_size)
-        self.is_vector_env = True
 
     def reset(
         self,
-        seed: Optional[Union[int, List[int]]] = None,
-        options: Optional[dict] = None,
+        seed: int | list[int] | None = None,
+        options: dict | None = None,
     ):
         """Resets the environment using kwargs and resets the episode returns and lengths."""
         obs, info = super().reset(seed=seed, options=options)
+
         self.episode_start_times = np.full(
             self.num_envs, time.perf_counter(), dtype=np.float32
         )
         self.episode_returns = np.zeros(self.num_envs, dtype=np.float32)
         self.episode_lengths = np.zeros(self.num_envs, dtype=np.int32)
+
         return obs, info
 
-    def step(self, action):
+    def step(
+        self, actions: ActType
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
         """Steps through the environment, recording the episode statistics."""
         (
             observations,
             rewards,
             terminations,
             truncations,
             infos,
-        ) = self.env.step(action)
+        ) = self.env.step(actions)
+
         assert isinstance(
             infos, dict
         ), f"`info` dtype is {type(infos)} while supported dtype is `dict`. This may be due to usage of other wrappers in the wrong order."
+
         self.episode_returns += rewards
         self.episode_lengths += 1
+
         dones = np.logical_or(terminations, truncations)
         num_dones = np.sum(dones)
+
         if num_dones:
             if "episode" in infos or "_episode" in infos:
                 raise ValueError(
                     "Attempted to add episode stats when they already exist"
                 )
             else:
                 infos["episode"] = {
@@ -105,22 +119,26 @@
                     "l": np.where(dones, self.episode_lengths, 0),
                     "t": np.where(
                         dones,
                         np.round(time.perf_counter() - self.episode_start_times, 6),
                         0.0,
                     ),
                 }
-                if self.is_vector_env:
-                    infos["_episode"] = np.where(dones, True, False)
-            self.return_queue.extend(self.episode_returns[dones])
-            self.length_queue.extend(self.episode_lengths[dones])
+                infos["_episode"] = dones
+
             self.episode_count += num_dones
+
+            for i in np.where(dones):
+                self.return_queue.extend(self.episode_returns[i])
+                self.length_queue.extend(self.episode_lengths[i])
+
             self.episode_lengths[dones] = 0
             self.episode_returns[dones] = 0
             self.episode_start_times[dones] = time.perf_counter()
+
         return (
             observations,
             rewards,
             terminations,
             truncations,
             infos,
         )
```

### Comparing `gymnasium-0.28.1/gymnasium/experimental/wrappers/vector/vector_list_info.py` & `gymnasium-0.29.0/gymnasium/wrappers/vector_list_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,63 @@
 """Wrapper that converts the info format for vec envs into the list format."""
 
 from typing import List
 
-from gymnasium.experimental.vector.vector_env import VectorEnv, VectorWrapper
+import gymnasium as gym
 
 
-class VectorListInfo(VectorWrapper):
+class VectorListInfo(gym.Wrapper, gym.utils.RecordConstructorArgs):
     """Converts infos of vectorized environments from dict to List[dict].
 
     This wrapper converts the info format of a
     vector environment from a dictionary to a list of dictionaries.
     This wrapper is intended to be used around vectorized
     environments. If using other wrappers that perform
     operation on info like `RecordEpisodeStatistics` this
     need to be the outermost wrapper.
 
     i.e. `VectorListInfo(RecordEpisodeStatistics(envs))`
 
-    Example::
-
-        >>> # actual
-        >>> {  # doctest: +SKIP
-        ...      "k": np.array([0., 0., 0.5, 0.3]),
-        ...      "_k": np.array([False, False, True, True])
-        ...  }
-        >>> # classic
-        >>> [{}, {}, {k: 0.5}, {k: 0.3}]  # doctest: +SKIP
+    Example:
+        >>> # As dict:
+        >>> infos = {
+        ...     "final_observation": "<array of length num-envs>",
+        ...     "_final_observation": "<boolean array of length num-envs>",
+        ...     "final_info": "<array of length num-envs>",
+        ...     "_final_info": "<boolean array of length num-envs>",
+        ...     "episode": {
+        ...         "r": "<array of cumulative reward>",
+        ...         "l": "<array of episode length>",
+        ...         "t": "<array of elapsed time since beginning of episode>"
+        ...     },
+        ...     "_episode": "<boolean array of length num-envs>"
+        ... }
+        >>> # As list:
+        >>> infos = [
+        ...     {
+        ...         "episode": {"r": "<cumulative reward>", "l": "<episode length>", "t": "<elapsed time since beginning of episode>"},
+        ...         "final_observation": "<observation>",
+        ...         "final_info": {},
+        ...     },
+        ...     ...,
+        ... ]
     """
 
-    def __init__(self, env: VectorEnv):
+    def __init__(self, env):
         """This wrapper will convert the info into the list format.
 
         Args:
             env (Env): The environment to apply the wrapper
         """
-        super().__init__(env)
+        gym.utils.RecordConstructorArgs.__init__(self)
+        gym.Wrapper.__init__(self, env)
+        try:
+            self.get_wrapper_attr("is_vector_env")
+        except AttributeError:
+            assert False, "This wrapper can only be used in vectorized environments."
 
     def step(self, action):
         """Steps through the environment, convert dict info to list."""
         observation, reward, terminated, truncated, infos = self.env.step(action)
         list_info = self._convert_info_to_list(infos)
 
         return observation, reward, terminated, truncated, list_info
```

### Comparing `gymnasium-0.28.1/gymnasium/logger.py` & `gymnasium-0.29.0/gymnasium/logger.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/spaces/__init__.py` & `gymnasium-0.29.0/gymnasium/spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/spaces/box.py` & `gymnasium-0.29.0/gymnasium/spaces/box.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,46 +85,56 @@
         ), "Box dtype must be explicitly provided, cannot be None."
         self.dtype = np.dtype(dtype)
 
         # determine shape if it isn't provided directly
         if shape is not None:
             assert all(
                 np.issubdtype(type(dim), np.integer) for dim in shape
-            ), f"Expect all shape elements to be an integer, actual type: {tuple(type(dim) for dim in shape)}"
+            ), f"Expected all shape elements to be an integer, actual type: {tuple(type(dim) for dim in shape)}"
             shape = tuple(int(dim) for dim in shape)  # This changes any np types to int
         elif isinstance(low, np.ndarray):
             shape = low.shape
         elif isinstance(high, np.ndarray):
             shape = high.shape
         elif is_float_integer(low) and is_float_integer(high):
             shape = (1,)
         else:
             raise ValueError(
-                f"Box shape is inferred from low and high, expect their types to be np.ndarray, an integer or a float, actual type low: {type(low)}, high: {type(high)}"
+                f"Box shape is inferred from low and high, expected their types to be np.ndarray, an integer or a float, actual type low: {type(low)}, high: {type(high)}"
             )
 
         # Capture the boundedness information before replacing np.inf with get_inf
         _low = np.full(shape, low, dtype=float) if is_float_integer(low) else low
         self.bounded_below: NDArray[np.bool_] = -np.inf < _low
 
         _high = np.full(shape, high, dtype=float) if is_float_integer(high) else high
         self.bounded_above: NDArray[np.bool_] = np.inf > _high
 
-        low = _broadcast(low, self.dtype, shape, inf_sign="-")
-        high = _broadcast(high, self.dtype, shape, inf_sign="+")
+        low = _broadcast(low, self.dtype, shape)
+        high = _broadcast(high, self.dtype, shape)
 
         assert isinstance(low, np.ndarray)
         assert (
             low.shape == shape
         ), f"low.shape doesn't match provided shape, low.shape: {low.shape}, shape: {shape}"
         assert isinstance(high, np.ndarray)
         assert (
             high.shape == shape
         ), f"high.shape doesn't match provided shape, high.shape: {high.shape}, shape: {shape}"
 
+        # check that we don't have invalid low or high
+        if np.any(low > high):
+            raise ValueError(
+                f"Some low values are greater than high, low={low}, high={high}"
+            )
+        if np.any(np.isposinf(low)):
+            raise ValueError(f"No low value can be equal to `np.inf`, low={low}")
+        if np.any(np.isneginf(high)):
+            raise ValueError(f"No high value can be equal to `-np.inf`, high={high}")
+
         self._shape: tuple[int, ...] = shape
 
         low_precision = get_precision(low.dtype)
         high_precision = get_precision(high.dtype)
         dtype_precision = get_precision(self.dtype)
         if min(low_precision, high_precision) > dtype_precision:
             gym.logger.warn(f"Box bound precision lowered by casting to {self.dtype}")
@@ -242,15 +252,15 @@
 
     def to_jsonable(self, sample_n: Sequence[NDArray[Any]]) -> list[list]:
         """Convert a batch of samples from this space to a JSONable data type."""
         return [sample.tolist() for sample in sample_n]
 
     def from_jsonable(self, sample_n: Sequence[float | int]) -> list[NDArray[Any]]:
         """Convert a JSONable data type to a batch of samples from this space."""
-        return [np.asarray(sample) for sample in sample_n]
+        return [np.asarray(sample, dtype=self.dtype) for sample in sample_n]
 
     def __repr__(self) -> str:
         """A string representation of this space.
 
         The representation will include bounds, shape and dtype.
         If a bound is uniform, only the corresponding scalar will be given to avoid redundant and ugly strings.
 
@@ -277,65 +287,51 @@
         if not hasattr(self, "low_repr"):
             self.low_repr = _short_repr(self.low)
 
         if not hasattr(self, "high_repr"):
             self.high_repr = _short_repr(self.high)
 
 
-def get_inf(dtype: np.dtype, sign: str) -> int | float:
-    """Returns an infinite that doesn't break things.
-
-    Args:
-        dtype: An `np.dtype`
-        sign (str): must be either `"+"` or `"-"`
-
-    Returns:
-        Gets an infinite value with the sign and dtype
-
-    Raises:
-        TypeError: Unknown sign, use either '+' or '-'
-        ValueError: Unknown dtype for infinite bounds
-    """
-    if np.dtype(dtype).kind == "f":
-        if sign == "+":
-            return np.inf
-        elif sign == "-":
-            return -np.inf
-        else:
-            raise TypeError(f"Unknown sign {sign}, use either '+' or '-'")
-    elif np.dtype(dtype).kind == "i":
-        if sign == "+":
-            return np.iinfo(dtype).max - 2
-        elif sign == "-":
-            return np.iinfo(dtype).min + 2
-        else:
-            raise TypeError(f"Unknown sign {sign}, use either '+' or '-'")
-    else:
-        raise ValueError(f"Unknown dtype {dtype} for infinite bounds")
-
-
 def get_precision(dtype: np.dtype) -> SupportsFloat:
     """Get precision of a data type."""
     if np.issubdtype(dtype, np.floating):
         return np.finfo(dtype).precision
     else:
         return np.inf
 
 
 def _broadcast(
     value: SupportsFloat | NDArray[Any],
     dtype: np.dtype,
     shape: tuple[int, ...],
-    inf_sign: str,
 ) -> NDArray[Any]:
-    """Handle infinite bounds and broadcast at the same time if needed."""
+    """Handle infinite bounds and broadcast at the same time if needed.
+
+    This is needed primarily because:
+        >>> import numpy as np
+        >>> np.full((2,), np.inf, dtype=np.int32)
+        array([-2147483648, -2147483648], dtype=int32)
+    """
     if is_float_integer(value):
-        value = get_inf(dtype, inf_sign) if np.isinf(value) else value
-        value = np.full(shape, value, dtype=dtype)
+        if np.isneginf(value) and np.dtype(dtype).kind == "i":
+            value = np.iinfo(dtype).min + 2
+        elif np.isposinf(value) and np.dtype(dtype).kind == "i":
+            value = np.iinfo(dtype).max - 2
+
+        return np.full(shape, value, dtype=dtype)
+
+    elif isinstance(value, np.ndarray):
+        # this is needed because we can't stuff np.iinfo(int).min into an array of dtype float
+        casted_value = value.astype(dtype)
+
+        # change bounds only if values are negative or positive infinite
+        if np.dtype(dtype).kind == "i":
+            casted_value[np.isneginf(value)] = np.iinfo(dtype).min + 2
+            casted_value[np.isposinf(value)] = np.iinfo(dtype).max - 2
+
+        return casted_value
+
     else:
-        assert isinstance(value, np.ndarray)
-        if np.any(np.isinf(value)):
-            # create new array with dtype, but maintain old one to preserve np.inf
-            temp = value.astype(dtype)
-            temp[np.isinf(value)] = get_inf(dtype, inf_sign)
-            value = temp
-    return value
+        # only np.ndarray allowed beyond this point
+        raise TypeError(
+            f"Unknown dtype for `value`, expected `np.ndarray` or float/integer, got {type(value)}"
+        )
```

### Comparing `gymnasium-0.28.1/gymnasium/spaces/dict.py` & `gymnasium-0.29.0/gymnasium/spaces/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Implementation of a space that represents the cartesian product of other spaces as a dictionary."""
 from __future__ import annotations
 
 import collections.abc
 import typing
 from collections import OrderedDict
-from typing import Any, Sequence
+from typing import Any, KeysView, Sequence
 
 import numpy as np
 
 from gymnasium.spaces.space import Space
 
 
 class Dict(Space[typing.Dict[str, Any]], typing.Mapping[str, Space[Any]]):
@@ -176,14 +176,18 @@
             return all(x[key] in self.spaces[key] for key in self.spaces.keys())
         return False
 
     def __getitem__(self, key: str) -> Space[Any]:
         """Get the space that is associated to `key`."""
         return self.spaces[key]
 
+    def keys(self) -> KeysView:
+        """Returns the keys of the Dict."""
+        return KeysView(self.spaces)
+
     def __setitem__(self, key: str, value: Space[Any]):
         """Set the space that is associated to `key`."""
         assert isinstance(
             value, Space
         ), f"Trying to set {key} to Dict space with value that is not a gymnasium space, actual type: {type(value)}"
         self.spaces[key] = value
```

### Comparing `gymnasium-0.28.1/gymnasium/spaces/discrete.py` & `gymnasium-0.29.0/gymnasium/spaces/discrete.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/spaces/graph.py` & `gymnasium-0.29.0/gymnasium/spaces/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,15 @@
                [-69.142105 ,  36.60979  ,  48.95243  ]], dtype=float32), edges=array([2, 0, 1, 1, 0, 0, 1, 0]), edge_links=array([[7, 5],
                [6, 9],
                [4, 1],
                [8, 6],
                [7, 0],
                [3, 7],
                [8, 4],
-               [8, 8]]))
-
+               [8, 8]], dtype=int32))
     """
 
     def __init__(
         self,
         node_space: Box | Discrete,
         edge_space: None | Box | Discrete,
         seed: int | np.random.Generator | None = None,
@@ -65,15 +64,15 @@
         This argument must be either a Box or Discrete instance.
 
         The argument ``edge_space`` specifies the base space that each edge feature will use.
         This argument must be either a None, Box or Discrete instance.
 
         Args:
             node_space (Union[Box, Discrete]): space of the node features.
-            edge_space (Union[None, Box, Discrete]): space of the node features.
+            edge_space (Union[None, Box, Discrete]): space of the edge features.
             seed: Optionally, you can use this argument to seed the RNG that is used to sample from the space.
         """
         assert isinstance(
             node_space, (Box, Discrete)
         ), f"Values of the node_space should be instances of Box or Discrete, got {type(node_space)}"
         if edge_space is not None:
             assert isinstance(
@@ -174,15 +173,15 @@
             if sampled_edge_space is not None
             else None
         )
 
         sampled_edge_links = None
         if sampled_edges is not None and num_edges > 0:
             sampled_edge_links = self.np_random.integers(
-                low=0, high=num_nodes, size=(num_edges, 2)
+                low=0, high=num_nodes, size=(num_edges, 2), dtype=np.int32
             )
 
         return GraphInstance(sampled_nodes, sampled_edges, sampled_edge_links)
 
     def contains(self, x: GraphInstance) -> bool:
         """Return boolean specifying if x is a valid member of this space."""
         if isinstance(x, GraphInstance):
@@ -244,20 +243,21 @@
     def from_jsonable(
         self, sample_n: Sequence[dict[str, list[list[int] | list[float]]]]
     ) -> list[GraphInstance]:
         """Convert a JSONable data type to a batch of samples from this space."""
         ret: list[GraphInstance] = []
         for sample in sample_n:
             if "edges" in sample:
+                assert self.edge_space is not None
                 ret_n = GraphInstance(
-                    np.asarray(sample["nodes"]),
-                    np.asarray(sample["edges"]),
-                    np.asarray(sample["edge_links"]),
+                    np.asarray(sample["nodes"], dtype=self.node_space.dtype),
+                    np.asarray(sample["edges"], dtype=self.edge_space.dtype),
+                    np.asarray(sample["edge_links"], dtype=np.int32),
                 )
             else:
                 ret_n = GraphInstance(
-                    np.asarray(sample["nodes"]),
+                    np.asarray(sample["nodes"], dtype=self.node_space.dtype),
                     None,
                     None,
                 )
             ret.append(ret_n)
         return ret
```

### Comparing `gymnasium-0.28.1/gymnasium/spaces/multi_binary.py` & `gymnasium-0.29.0/gymnasium/spaces/multi_binary.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/spaces/multi_discrete.py` & `gymnasium-0.29.0/gymnasium/spaces/multi_discrete.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Implementation of a space that represents the cartesian product of `Discrete` spaces."""
 from __future__ import annotations
 
-from typing import Any, Sequence
+from typing import Any, Iterable, Mapping, Sequence
 
 import numpy as np
 from numpy.typing import NDArray
 
 import gymnasium as gym
 from gymnasium.spaces.discrete import Discrete
 from gymnasium.spaces.space import MaskNDArray, Space
@@ -40,26 +40,37 @@
     """
 
     def __init__(
         self,
         nvec: NDArray[np.integer[Any]] | list[int],
         dtype: str | type[np.integer[Any]] = np.int64,
         seed: int | np.random.Generator | None = None,
+        start: NDArray[np.integer[Any]] | list[int] | None = None,
     ):
         """Constructor of :class:`MultiDiscrete` space.
 
-        The argument ``nvec`` will determine the number of values each categorical variable can take.
+        The argument ``nvec`` will determine the number of values each categorical variable can take. If
+        ``start`` is provided, it will define the minimal values corresponding to each categorical variable.
 
         Args:
             nvec: vector of counts of each categorical variable. This will usually be a list of integers. However,
                 you may also pass a more complicated numpy array if you'd like the space to have several axes.
             dtype: This should be some kind of integer type.
             seed: Optionally, you can use this argument to seed the RNG that is used to sample from the space.
+            start: Optionally, the starting value the element of each class will take (defaults to 0).
         """
         self.nvec = np.array(nvec, dtype=dtype, copy=True)
+        if start is not None:
+            self.start = np.array(start, dtype=dtype, copy=True)
+        else:
+            self.start = np.zeros(self.nvec.shape, dtype=dtype)
+
+        assert (
+            self.start.shape == self.nvec.shape
+        ), "start and nvec (counts) should have the same shape"
         assert (self.nvec > 0).all(), "nvec (counts) have to be positive"
 
         super().__init__(self.nvec.shape, dtype, seed)
 
     @property
     def shape(self) -> tuple[int, ...]:
         """Has stricter type than :class:`gym.Space` - never None."""
@@ -74,35 +85,38 @@
         self, mask: tuple[MaskNDArray, ...] | None = None
     ) -> NDArray[np.integer[Any]]:
         """Generates a single random sample this space.
 
         Args:
             mask: An optional mask for multi-discrete, expects tuples with a `np.ndarray` mask in the position of each
                 action with shape `(n,)` where `n` is the number of actions and `dtype=np.int8`.
-                Only mask values == 1 are possible to sample unless all mask values for an action are 0 then the default action 0 is sampled.
+                Only mask values == 1 are possible to sample unless all mask values for an action are 0 then the default action `self.start` (the smallest element) is sampled.
 
         Returns:
             An `np.ndarray` of shape `space.shape`
         """
         if mask is not None:
 
             def _apply_mask(
                 sub_mask: MaskNDArray | tuple[MaskNDArray, ...],
                 sub_nvec: MaskNDArray | np.integer[Any],
+                sub_start: MaskNDArray | np.integer[Any],
             ) -> int | list[Any]:
                 if isinstance(sub_nvec, np.ndarray):
                     assert isinstance(
                         sub_mask, tuple
                     ), f"Expects the mask to be a tuple for sub_nvec ({sub_nvec}), actual type: {type(sub_mask)}"
                     assert len(sub_mask) == len(
                         sub_nvec
                     ), f"Expects the mask length to be equal to the number of actions, mask length: {len(sub_mask)}, nvec length: {len(sub_nvec)}"
                     return [
-                        _apply_mask(new_mask, new_nvec)
-                        for new_mask, new_nvec in zip(sub_mask, sub_nvec)
+                        _apply_mask(new_mask, new_nvec, new_start)
+                        for new_mask, new_nvec, new_start in zip(
+                            sub_mask, sub_nvec, sub_start
+                        )
                     ]
                 else:
                     assert np.issubdtype(
                         type(sub_nvec), np.integer
                     ), f"Expects the sub_nvec to be an action, actually: {sub_nvec}, {type(sub_nvec)}"
                     assert isinstance(
                         sub_mask, np.ndarray
@@ -116,35 +130,40 @@
 
                     valid_action_mask = sub_mask == 1
                     assert np.all(
                         np.logical_or(sub_mask == 0, valid_action_mask)
                     ), f"Expects all masks values to 0 or 1, actual values: {sub_mask}"
 
                     if np.any(valid_action_mask):
-                        return self.np_random.choice(np.where(valid_action_mask)[0])
+                        return (
+                            self.np_random.choice(np.where(valid_action_mask)[0])
+                            + sub_start
+                        )
                     else:
-                        return 0
+                        return sub_start
 
-            return np.array(_apply_mask(mask, self.nvec), dtype=self.dtype)
+            return np.array(_apply_mask(mask, self.nvec, self.start), dtype=self.dtype)
 
-        return (self.np_random.random(self.nvec.shape) * self.nvec).astype(self.dtype)
+        return (self.np_random.random(self.nvec.shape) * self.nvec).astype(
+            self.dtype
+        ) + self.start
 
     def contains(self, x: Any) -> bool:
         """Return boolean specifying if x is a valid member of this space."""
         if isinstance(x, Sequence):
             x = np.array(x)  # Promote list to array for contains check
 
         # if nvec is uint32 and space dtype is uint32, then 0 <= x < self.nvec guarantees that x
         # is within correct bounds for space dtype (even though x does not have to be unsigned)
         return bool(
             isinstance(x, np.ndarray)
             and x.shape == self.shape
             and x.dtype != object
-            and np.all(0 <= x)
-            and np.all(x < self.nvec)
+            and np.all(self.start <= x)
+            and np.all(x - self.start < self.nvec)
         )
 
     def to_jsonable(
         self, sample_n: Sequence[NDArray[np.integer[Any]]]
     ) -> list[Sequence[int]]:
         """Convert a batch of samples from this space to a JSONable data type."""
         return [sample.tolist() for sample in sample_n]
@@ -153,23 +172,26 @@
         self, sample_n: list[Sequence[int]]
     ) -> list[NDArray[np.integer[Any]]]:
         """Convert a JSONable data type to a batch of samples from this space."""
         return [np.array(sample) for sample in sample_n]
 
     def __repr__(self):
         """Gives a string representation of this space."""
+        if np.any(self.start != 0):
+            return f"MultiDiscrete({self.nvec}, start={self.start})"
         return f"MultiDiscrete({self.nvec})"
 
-    def __getitem__(self, index: int):
+    def __getitem__(self, index: int | tuple[int, ...]):
         """Extract a subspace from this ``MultiDiscrete`` space."""
         nvec = self.nvec[index]
+        start = self.start[index]
         if nvec.ndim == 0:
-            subspace = Discrete(nvec)
+            subspace = Discrete(nvec, start=start)
         else:
-            subspace = MultiDiscrete(nvec, self.dtype)  # type: ignore
+            subspace = MultiDiscrete(nvec, self.dtype, start=start)
 
         # you don't need to deepcopy as np random generator call replaces the state not the data
         subspace.np_random.bit_generator.state = self.np_random.bit_generator.state
 
         return subspace
 
     def __len__(self):
@@ -179,9 +201,26 @@
                 "Getting the length of a multi-dimensional MultiDiscrete space."
             )
         return len(self.nvec)
 
     def __eq__(self, other: Any) -> bool:
         """Check whether ``other`` is equivalent to this instance."""
         return bool(
-            isinstance(other, MultiDiscrete) and np.all(self.nvec == other.nvec)
+            isinstance(other, MultiDiscrete)
+            and np.all(self.nvec == other.nvec)
+            and np.all(self.start == other.start)
         )
+
+    def __setstate__(self, state: Iterable[tuple[str, Any]] | Mapping[str, Any]):
+        """Used when loading a pickled space.
+
+        This method has to be implemented explicitly to allow for loading of legacy states.
+
+        Args:
+            state: The new state
+        """
+        state = dict(state)
+
+        if "start" not in state:
+            state["start"] = np.zeros(state["_shape"], dtype=state["dtype"])
+
+        super().__setstate__(state)
```

### Comparing `gymnasium-0.28.1/gymnasium/spaces/sequence.py` & `gymnasium-0.29.0/gymnasium/spaces/sequence.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/spaces/space.py` & `gymnasium-0.29.0/gymnasium/spaces/space.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/spaces/text.py` & `gymnasium-0.29.0/gymnasium/spaces/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 class Text(Space[str]):
     r"""A space representing a string comprised of characters from a given charset.
 
     Example:
         >>> from gymnasium.spaces import Text
         >>> # {"", "B5", "hello", ...}
         >>> Text(5)
-        Text(1, 5, characters=0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz)
+        Text(1, 5, charset=0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz)
         >>> # {"0", "42", "0123456789", ...}
         >>> import string
         >>> Text(min_length = 1,
         ...      max_length = 10,
         ...      charset = string.digits)
-        Text(1, 10, characters=0123456789)
+        Text(1, 10, charset=0123456789)
     """
 
     def __init__(
         self,
         max_length: int,
         *,
         min_length: int = 1,
@@ -151,17 +151,15 @@
         if isinstance(x, str):
             if self.min_length <= len(x) <= self.max_length:
                 return all(c in self.character_set for c in x)
         return False
 
     def __repr__(self) -> str:
         """Gives a string representation of this space."""
-        return (
-            f"Text({self.min_length}, {self.max_length}, characters={self.characters})"
-        )
+        return f"Text({self.min_length}, {self.max_length}, charset={self.characters})"
 
     def __eq__(self, other: Any) -> bool:
         """Check whether ``other`` is equivalent to this instance."""
         return (
             isinstance(other, Text)
             and self.min_length == other.min_length
             and self.max_length == other.max_length
```

### Comparing `gymnasium-0.28.1/gymnasium/spaces/tuple.py` & `gymnasium-0.29.0/gymnasium/spaces/tuple.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/spaces/utils.py` & `gymnasium-0.29.0/gymnasium/spaces/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 def _flatten_multidiscrete(
     space: MultiDiscrete, x: NDArray[np.int64]
 ) -> NDArray[np.int64]:
     offsets = np.zeros((space.nvec.size + 1,), dtype=np.int32)
     offsets[1:] = np.cumsum(space.nvec.flatten())
 
     onehot = np.zeros((offsets[-1],), dtype=space.dtype)
-    onehot[offsets[:-1] + x.flatten()] = 1
+    onehot[offsets[:-1] + (x - space.start).flatten()] = 1
     return onehot
 
 
 @flatten.register(Tuple)
 def _flatten_tuple(space: Tuple, x: tuple[Any, ...]) -> tuple[Any, ...] | NDArray[Any]:
     if space.is_np_flattenable:
         return np.concatenate(
@@ -304,15 +304,18 @@
     nonzero = np.nonzero(x)
     if len(nonzero[0]) == 0:
         raise ValueError(
             f"{x} is not a concatenation of one-hot encoded vectors and can not be unflattened to space {space}. "
             "Not all valid samples in a flattened space can be unflattened."
         )
     (indices,) = cast(type(offsets[:-1]), nonzero)
-    return np.asarray(indices - offsets[:-1], dtype=space.dtype).reshape(space.shape)
+    return (
+        np.asarray(indices - offsets[:-1], dtype=space.dtype).reshape(space.shape)
+        + space.start
+    )
 
 
 @unflatten.register(Tuple)
 def _unflatten_tuple(
     space: Tuple, x: NDArray[Any] | tuple[Any, ...]
 ) -> tuple[Any, ...]:
     if space.is_np_flattenable:
```

### Comparing `gymnasium-0.28.1/gymnasium/utils/__init__.py` & `gymnasium-0.29.0/gymnasium/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/utils/colorize.py` & `gymnasium-0.29.0/gymnasium/utils/colorize.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/utils/env_checker.py` & `gymnasium-0.29.0/gymnasium/utils/env_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,17 +46,21 @@
                 data_equivalence(data_1[k], data_2[k]) for k in data_1.keys()
             )
         elif isinstance(data_1, (tuple, list)):
             return len(data_1) == len(data_2) and all(
                 data_equivalence(o_1, o_2) for o_1, o_2 in zip(data_1, data_2)
             )
         elif isinstance(data_1, np.ndarray):
-            return data_1.shape == data_2.shape and np.allclose(
-                data_1, data_2, atol=0.00001
-            )
+            if data_1.shape == data_2.shape and data_1.dtype == data_2.dtype:
+                if data_1.dtype == object:
+                    return all(data_equivalence(a, b) for a, b in zip(data_1, data_2))
+                else:
+                    return np.allclose(data_1, data_2, atol=0.00001)
+            else:
+                return False
         else:
             return data_1 == data_2
     else:
         return False
 
 
 def check_reset_seed(env: gym.Env):
@@ -254,44 +258,44 @@
 
 def check_env(env: gym.Env, warn: bool = None, skip_render_check: bool = False):
     """Check that an environment follows Gym API.
 
     This is an invasive function that calls the environment's reset and step.
 
     This is particularly useful when using a custom environment.
-    Please take a look at https://gymnasium.farama.org/content/environment_creation/
+    Please take a look at https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/
     for more information about the API.
 
     Args:
         env: The Gym environment that will be checked
         warn: Ignored
         skip_render_check: Whether to skip the checks for the render method. True by default (useful for the CI)
     """
     if warn is not None:
         logger.warn("`check_env(warn=...)` parameter is now ignored.")
 
     assert isinstance(
         env, gym.Env
-    ), "The environment must inherit from the gymnasium.Env class. See https://gymnasium.farama.org/content/environment_creation/ for more info."
+    ), "The environment must inherit from the gymnasium.Env class. See https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/ for more info."
 
     if env.unwrapped is not env:
         logger.warn(
             f"The environment ({env}) is different from the unwrapped version ({env.unwrapped}). This could effect the environment checker as the environment most likely has a wrapper applied to it. We recommend using the raw environment for `check_env` using `env.unwrapped`."
         )
 
     # ============= Check the spaces (observation and action) ================
     assert hasattr(
         env, "action_space"
-    ), "The environment must specify an action space. See https://gymnasium.farama.org/content/environment_creation/ for more info."
+    ), "The environment must specify an action space. See https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/ for more info."
     check_action_space(env.action_space)
     check_space_limit(env.action_space, "action")
 
     assert hasattr(
         env, "observation_space"
-    ), "The environment must specify an observation space. See https://gymnasium.farama.org/content/environment_creation/ for more info."
+    ), "The environment must specify an observation space. See https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/ for more info."
     check_observation_space(env.observation_space)
     check_space_limit(env.observation_space, "observation")
 
     # ==== Check the reset method ====
     check_seed_deprecation(env)
     check_reset_return_info_deprecation(env)
     check_reset_return_type(env)
@@ -313,7 +317,17 @@
                 new_env.reset()
                 env_render_passive_checker(new_env)
                 new_env.close()
         else:
             logger.warn(
                 "Not able to test alternative render modes due to the environment not having a spec. Try instantialising the environment through gymnasium.make"
             )
+
+    if env.spec is not None:
+        new_env = env.spec.make()
+        new_env.close()
+        try:
+            new_env.close()
+        except Exception as e:
+            logger.warn(
+                f"Calling `env.close()` on the closed environment should be allowed, but it raised an exception: {e}"
+            )
```

### Comparing `gymnasium-0.28.1/gymnasium/utils/ezpickle.py` & `gymnasium-0.29.0/gymnasium/utils/ezpickle.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/utils/passive_env_checker.py` & `gymnasium-0.29.0/gymnasium/utils/passive_env_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,38 +17,14 @@
 
 def _check_box_observation_space(observation_space: spaces.Box):
     """Checks that a :class:`Box` observation space is defined in a sensible way.
 
     Args:
         observation_space: A box observation space
     """
-    # Check if the box is an image
-    if (len(observation_space.shape) == 3 and observation_space.shape[0] != 1) or (
-        len(observation_space.shape) == 4 and observation_space.shape[0] == 1
-    ):
-        if observation_space.dtype != np.uint8:
-            logger.warn(
-                f"It seems a Box observation space is an image but the `dtype` is not `np.uint8`, actual type: {observation_space.dtype}. "
-                "If the Box observation space is not an image, we recommend flattening the observation to have only a 1D vector."
-            )
-        if np.any(observation_space.low != 0) or np.any(observation_space.high != 255):
-            logger.warn(
-                "It seems a Box observation space is an image but the lower and upper bounds are not [0, 255]. "
-                f"Actual lower bound: {np.min(observation_space.low)}, upper bound: {np.max(observation_space.high)}. "
-                "Generally, CNN policies assume observations are within that range, so you may encounter an issue if the observation values are not."
-            )
-
-    if len(observation_space.shape) not in [1, 3]:
-        if not (len(observation_space.shape) == 2 and observation_space.shape[0] == 1):
-            logger.warn(
-                "A Box observation space has an unconventional shape (neither an image, nor a 1D vector). "
-                "We recommend flattening the observation to have only a 1D vector or use a custom policy to properly process the data. "
-                f"Actual observation shape: {observation_space.shape}"
-            )
-
     assert (
         observation_space.low.shape == observation_space.shape
     ), f"The Box observation space shape and low shape have different shapes, low shape: {observation_space.low.shape}, box shape: {observation_space.shape}"
     assert (
         observation_space.high.shape == observation_space.shape
     ), f"The Box observation space shape and high shape have have different shapes, high shape: {observation_space.high.shape}, box shape: {observation_space.shape}"
 
@@ -78,19 +54,14 @@
     ), f"The Box action space shape and high shape have different shapes, high shape: {action_space.high.shape}, box shape: {action_space.shape}"
 
     if np.any(action_space.low == action_space.high):
         logger.warn(
             "A Box action space maximum and minimum values are equal. "
             f"Actual equal coordinates: {[x for x in zip(*np.where(action_space.low == action_space.high))]}"
         )
-    elif np.any(action_space.high < action_space.low):
-        logger.warn(
-            "A Box action space low value is greater than a high value. "
-            f"Actual less than coordinates: {[x for x in zip(*np.where(action_space.high < action_space.low))]}"
-        )
 
 
 def check_space(
     space: Space, space_type: str, check_box_space_fn: Callable[[spaces.Box], None]
 ):
     """A passive check of the environment action space that should not affect the environment."""
     if not isinstance(space, spaces.Space):
```

### Comparing `gymnasium-0.28.1/gymnasium/utils/play.py` & `gymnasium-0.29.0/gymnasium/utils/play.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/utils/record_constructor.py` & `gymnasium-0.29.0/gymnasium/utils/record_constructor.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/utils/save_video.py` & `gymnasium-0.29.0/gymnasium/utils/save_video.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/utils/seeding.py` & `gymnasium-0.29.0/gymnasium/utils/seeding.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/utils/step_api_compatibility.py` & `gymnasium-0.29.0/gymnasium/utils/step_api_compatibility.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/vector/__init__.py` & `gymnasium-0.29.0/gymnasium/vector/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         >>> env = gym.vector.make('CartPole-v1', num_envs=3)
         >>> env.reset(seed=42)
         (array([[ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ],
                [ 0.01522993, -0.04562247, -0.04799704,  0.03392126],
                [-0.03774345, -0.02418869, -0.00942293,  0.0469184 ]],
               dtype=float32), {})
     """
+    gym.logger.warn(
+        "`gymnasium.vector.make(...)` is deprecated and will be replaced by `gymnasium.make_vec(...)` in v1.0"
+    )
 
     def create_env(env_num: int) -> Callable[[], Env]:
         """Creates an environment that can enable or disable the environment checker."""
         # If the env_num > 0 then disable the environment checker otherwise use the parameter
         _disable_env_checker = True if env_num > 0 else disable_env_checker
 
         def _make_env() -> Env:
```

### Comparing `gymnasium-0.28.1/gymnasium/vector/async_vector_env.py` & `gymnasium-0.29.0/gymnasium/vector/async_vector_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,16 @@
             context: Context for `multiprocessing`_. If ``None``, then the default context is used.
             daemon: If ``True``, then subprocesses have ``daemon`` flag turned on; that is, they will quit if
                 the head process quits. However, ``daemon=True`` prevents subprocesses to spawn children,
                 so for some environments you may want to have it set to ``False``.
             worker: If set, then use that worker in a subprocess instead of a default one.
                 Can be useful to override some inner vector env logic, for instance, how resets on termination or truncation are handled.
 
-        Warnings: worker is an advanced mode option. It provides a high degree of flexibility and a high chance
+        Warnings:
+            worker is an advanced mode option. It provides a high degree of flexibility and a high chance
             to shoot yourself in the foot; thus, if you are writing your own worker, it is recommended to start
             from the code for ``_worker`` (or ``_worker_shared_memory``) method, and add changes.
 
         Raises:
             RuntimeError: If the observation space of some sub-environment does not match observation_space
                 (or, by default, the observation space of the first sub-environment).
             ValueError: If observation_space is a custom space (i.e. not a default space in Gym,
```

### Comparing `gymnasium-0.28.1/gymnasium/vector/sync_vector_env.py` & `gymnasium-0.29.0/gymnasium/vector/sync_vector_env.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/vector/utils/__init__.py` & `gymnasium-0.29.0/gymnasium/vector/utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 from gymnasium.vector.utils.misc import CloudpickleWrapper, clear_mpi_env_vars
 from gymnasium.vector.utils.numpy_utils import concatenate, create_empty_array
 from gymnasium.vector.utils.shared_memory import (
     create_shared_memory,
     read_from_shared_memory,
     write_to_shared_memory,
 )
-from gymnasium.vector.utils.spaces import (  # pyright: reportPrivateUsage=false
-    BaseGymSpaces,
-    _BaseGymSpaces,
-    batch_space,
-    iterate,
+from gymnasium.vector.utils.spaces import (
+    _BaseGymSpaces,  # pyright: ignore[reportPrivateUsage]
 )
+from gymnasium.vector.utils.spaces import BaseGymSpaces, batch_space, iterate
 
 
 __all__ = [
     "CloudpickleWrapper",
     "clear_mpi_env_vars",
     "concatenate",
     "create_empty_array",
```

### Comparing `gymnasium-0.28.1/gymnasium/vector/utils/misc.py` & `gymnasium-0.29.0/gymnasium/vector/utils/misc.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/vector/utils/numpy_utils.py` & `gymnasium-0.29.0/gymnasium/vector/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/vector/utils/shared_memory.py` & `gymnasium-0.29.0/gymnasium/vector/utils/shared_memory.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/vector/utils/spaces.py` & `gymnasium-0.29.0/gymnasium/vector/utils/spaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,36 +57,29 @@
     repeats = tuple([n] + [1] * space.low.ndim)
     low, high = np.tile(space.low, repeats), np.tile(space.high, repeats)
     return Box(low=low, high=high, dtype=space.dtype, seed=deepcopy(space.np_random))
 
 
 @batch_space.register(Discrete)
 def _batch_space_discrete(space, n=1):
-    if space.start == 0:
-        return MultiDiscrete(
-            np.full((n,), space.n, dtype=space.dtype),
-            dtype=space.dtype,
-            seed=deepcopy(space.np_random),
-        )
-    else:
-        return Box(
-            low=space.start,
-            high=space.start + space.n - 1,
-            shape=(n,),
-            dtype=space.dtype,
-            seed=deepcopy(space.np_random),
-        )
+    return MultiDiscrete(
+        np.full((n,), space.n, dtype=space.dtype),
+        dtype=space.dtype,
+        seed=deepcopy(space.np_random),
+        start=np.full((n,), space.start, dtype=space.dtype),
+    )
 
 
 @batch_space.register(MultiDiscrete)
 def _batch_space_multidiscrete(space, n=1):
     repeats = tuple([n] + [1] * space.nvec.ndim)
-    high = np.tile(space.nvec, repeats) - 1
+    low = np.tile(space.start, repeats)
+    high = low + np.tile(space.nvec, repeats) - 1
     return Box(
-        low=np.zeros_like(high),
+        low=low,
         high=high,
         dtype=space.dtype,
         seed=deepcopy(space.np_random),
     )
 
 
 @batch_space.register(MultiBinary)
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/__init__.py` & `gymnasium-0.29.0/gymnasium/wrappers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     >>> import gymnasium as gym
     >>> from gymnasium.wrappers import RescaleAction
     >>> base_env = gym.make("Hopper-v4")
     >>> base_env.action_space
     Box(-1.0, 1.0, (3,), float32)
     >>> wrapped_env = RescaleAction(base_env, min_action=0, max_action=1)
     >>> wrapped_env.action_space
-    Box(-1.0, 1.0, (3,), float32)
+    Box(0.0, 1.0, (3,), float32)
 
 You can access the environment underneath the **first** wrapper by using the :attr:`gymnasium.Wrapper.env` attribute.
 As the :class:`gymnasium.Wrapper` class inherits from :class:`gymnasium.Env` then :attr:`gymnasium.Wrapper.env` can be another wrapper.
 
     >>> wrapped_env
     <RescaleAction<TimeLimit<OrderEnforcing<PassiveEnvChecker<HopperEnv<Hopper-v4>>>>>>
     >>> wrapped_env.env
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/atari_preprocessing.py` & `gymnasium-0.29.0/gymnasium/experimental/wrappers/atari_preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Implementation of Atari 2600 Preprocessing following the guidelines of Machado et al., 2018."""
 import numpy as np
 
 import gymnasium as gym
 from gymnasium.spaces import Box
 
 
-try:
-    import cv2
-except ImportError:
-    cv2 = None
+__all__ = ["AtariPreprocessingV0"]
 
 
-class AtariPreprocessing(gym.Wrapper, gym.utils.RecordConstructorArgs):
+class AtariPreprocessingV0(gym.Wrapper, gym.utils.RecordConstructorArgs):
     """Atari 2600 preprocessing wrapper.
 
     This class follows the guidelines in Machado et al. (2018),
     "Revisiting the Arcade Learning Environment: Evaluation Protocols and Open Problems for General Agents".
 
     Specifically, the following preprocess stages applies to the atari environment:
 
@@ -68,18 +65,21 @@
             terminal_on_life_loss=terminal_on_life_loss,
             grayscale_obs=grayscale_obs,
             grayscale_newaxis=grayscale_newaxis,
             scale_obs=scale_obs,
         )
         gym.Wrapper.__init__(self, env)
 
-        if cv2 is None:
+        try:
+            import cv2  # noqa: F401
+        except ImportError:
             raise gym.error.DependencyNotInstalled(
                 "opencv-python package not installed, run `pip install gymnasium[other]` to get dependencies for atari"
             )
+
         assert frame_skip > 0
         assert screen_size > 0
         assert noop_max >= 0
         if frame_skip > 1:
             if (
                 env.spec is not None
                 and "NoFrameskip" not in env.spec.id
@@ -183,15 +183,17 @@
         self.obs_buffer[1].fill(0)
 
         return self._get_obs(), reset_info
 
     def _get_obs(self):
         if self.frame_skip > 1:  # more efficient in-place pooling
             np.maximum(self.obs_buffer[0], self.obs_buffer[1], out=self.obs_buffer[0])
-        assert cv2 is not None
+
+        import cv2
+
         obs = cv2.resize(
             self.obs_buffer[0],
             (self.screen_size, self.screen_size),
             interpolation=cv2.INTER_AREA,
         )
 
         if self.scale_obs:
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/autoreset.py` & `gymnasium-0.29.0/gymnasium/wrappers/autoreset.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
      - ``final_reward`` is the reward after calling :meth:`self.env.step`, prior to calling :meth:`self.env.reset`.
      - ``final_terminated`` is the terminated value before calling :meth:`self.env.reset`.
      - ``final_truncated`` is the truncated value before calling :meth:`self.env.reset`. Both `final_terminated` and `final_truncated` cannot be False.
      - ``info`` is a dict containing all the keys from the info dict returned by the call to :meth:`self.env.reset`,
        with an additional key "final_observation" containing the observation returned by the last call to :meth:`self.env.step`
        and "final_info" containing the info dict returned by the last call to :meth:`self.env.step`.
 
-    Warning: When using this wrapper to collect rollouts, note that when :meth:`Env.step` returns `terminated` or `truncated`, a
+    Warning:
+        When using this wrapper to collect rollouts, note that when :meth:`Env.step` returns `terminated` or `truncated`, a
         new observation from after calling :meth:`Env.reset` is returned by :meth:`Env.step` alongside the
         final reward, terminated and truncated state from the previous episode.
         If you need the final state from the previous episode, you need to retrieve it via the
         "final_observation" key in the info dict.
         Make sure you know what you're doing if you use this wrapper!
     """
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/clip_action.py` & `gymnasium-0.29.0/gymnasium/wrappers/clip_action.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/compatibility.py` & `gymnasium-0.29.0/gymnasium/wrappers/compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 """A compatibility wrapper converting an old-style environment into a valid environment."""
-import sys
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, Optional, Protocol, Tuple, runtime_checkable
 
 import gymnasium as gym
 from gymnasium import logger
 from gymnasium.core import ObsType
 from gymnasium.utils.step_api_compatibility import (
     convert_to_terminated_truncated_step_api,
 )
 
 
-if sys.version_info >= (3, 8):
-    from typing import Protocol, runtime_checkable
-else:
-    from typing_extensions import Protocol, runtime_checkable
-
-
 @runtime_checkable
 class LegacyEnv(Protocol):
     """A protocol for environments using the old step API."""
 
     observation_space: gym.Space
     action_space: gym.Space
 
@@ -61,16 +54,16 @@
         Some information may be lost in the conversion, so we recommend updating your environment.
 
         Args:
             old_env (LegacyEnv): the env to wrap, implemented with the old API
             render_mode (str): the render mode to use when rendering the environment, passed automatically to env.render
         """
         logger.deprecation(
-            "The `gymnasium.make(..., apply_api_compatibility=...)` parameter is deprecated and will be removed in v0.29. "
-            "Instead use `gym.make('GymV21Environment-v0', env_name=...)` or `from shimmy import GymV21CompatibilityV0`"
+            "The `gymnasium.make(..., apply_api_compatibility=...)` parameter is deprecated and will be removed in v1.0. "
+            "Instead use `gymnasium.make('GymV21Environment-v0', env_name=...)` or `from shimmy import GymV21CompatibilityV0`"
         )
 
         self.env = old_env
         self.metadata = getattr(old_env, "metadata", {"render_modes": []})
         self.render_mode = render_mode
         self.reward_range = getattr(old_env, "reward_range", None)
         self.spec = getattr(old_env, "spec", None)
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/env_checker.py` & `gymnasium-0.29.0/gymnasium/wrappers/env_checker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """A passive environment checker wrapper for an environment's observation and action space along with the reset, step and render functions."""
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import TYPE_CHECKING
 
 import gymnasium as gym
+from gymnasium import logger
 from gymnasium.core import ActType
 from gymnasium.utils.passive_env_checker import (
     check_action_space,
     check_observation_space,
     env_render_passive_checker,
     env_reset_passive_checker,
     env_step_passive_checker,
@@ -25,44 +26,45 @@
     def __init__(self, env):
         """Initialises the wrapper with the environments, run the observation and action space tests."""
         gym.utils.RecordConstructorArgs.__init__(self)
         gym.Wrapper.__init__(self, env)
 
         assert hasattr(
             env, "action_space"
-        ), "The environment must specify an action space. https://gymnasium.farama.org/content/environment_creation/"
+        ), "The environment must specify an action space. https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/"
         check_action_space(env.action_space)
         assert hasattr(
             env, "observation_space"
-        ), "The environment must specify an observation space. https://gymnasium.farama.org/content/environment_creation/"
+        ), "The environment must specify an observation space. https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/"
         check_observation_space(env.observation_space)
 
         self.checked_reset = False
         self.checked_step = False
         self.checked_render = False
+        self.close_called = False
 
     def step(self, action: ActType):
         """Steps through the environment that on the first call will run the `passive_env_step_check`."""
-        if self.checked_step is False:
+        if not self.checked_step:
             self.checked_step = True
             return env_step_passive_checker(self.env, action)
         else:
             return self.env.step(action)
 
     def reset(self, **kwargs):
         """Resets the environment that on the first call will run the `passive_env_reset_check`."""
-        if self.checked_reset is False:
+        if not self.checked_reset:
             self.checked_reset = True
             return env_reset_passive_checker(self.env, **kwargs)
         else:
             return self.env.reset(**kwargs)
 
     def render(self, *args, **kwargs):
         """Renders the environment that on the first call will run the `passive_env_render_check`."""
-        if self.checked_render is False:
+        if not self.checked_render:
             self.checked_render = True
             return env_render_passive_checker(self.env, *args, **kwargs)
         else:
             return self.env.render(*args, **kwargs)
 
     @property
     def spec(self) -> EnvSpec | None:
@@ -73,7 +75,21 @@
         env_spec = self.env.spec
         if env_spec is not None:
             env_spec = deepcopy(env_spec)
             env_spec.disable_env_checker = False
 
         self._cached_spec = env_spec
         return env_spec
+
+    def close(self):
+        """Warns if calling close on a closed environment fails."""
+        if not self.close_called:
+            self.close_called = True
+            return self.env.close()
+        else:
+            try:
+                return self.env.close()
+            except Exception as e:
+                logger.warn(
+                    "Calling `env.close()` on the closed environment should be allowed, but it raised the following exception."
+                )
+                raise e
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/filter_observation.py` & `gymnasium-0.29.0/gymnasium/wrappers/filter_observation.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/flatten_observation.py` & `gymnasium-0.29.0/gymnasium/wrappers/flatten_observation.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/frame_stack.py` & `gymnasium-0.29.0/gymnasium/wrappers/frame_stack.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/gray_scale_observation.py` & `gymnasium-0.29.0/gymnasium/wrappers/gray_scale_observation.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/human_rendering.py` & `gymnasium-0.29.0/gymnasium/wrappers/human_rendering.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         >>> wrapped = HumanRendering(env)
         >>> obs, _ = wrapped.reset()     # This will start rendering to the screen
 
         The wrapper can also be applied directly when the environment is instantiated, simply by passing
         ``render_mode="human"`` to ``make``. The wrapper will only be applied if the environment does not
         implement human-rendering natively (i.e. ``render_mode`` does not contain ``"human"``).
 
-        >>> env = gym.make("CartPoleJax-v1", render_mode="human")      # CartPoleJax-v1 doesn't implement human-rendering natively
+        >>> env = gym.make("phys2d/CartPole-v1", render_mode="human")      # phys2d/CartPole-v1 doesn't implement human-rendering natively
         >>> obs, _ = env.reset()     # This will start rendering to the screen
 
         Warning: If the base environment uses ``render_mode="rgb_array_list"``, its (i.e. the *base environment's*) render method
         will always return an empty list:
 
         >>> env = gym.make("LunarLander-v2", render_mode="rgb_array_list")
         >>> wrapped = HumanRendering(env)
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/monitoring/video_recorder.py` & `gymnasium-0.29.0/gymnasium/wrappers/monitoring/video_recorder.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,39 +36,38 @@
             base_path (Optional[str]): Alternatively, path to the video file without extension, which will be added.
             disable_logger (bool): Whether to disable moviepy logger or not.
 
         Raises:
             Error: You can pass at most one of `path` or `base_path`
             Error: Invalid path given that must have a particular file extension
         """
-        try:
-            # check that moviepy is now installed
-            import moviepy  # noqa: F401
-        except ImportError as e:
-            raise error.DependencyNotInstalled(
-                "moviepy is not installed, run `pip install moviepy`"
-            ) from e
-
         self._async = env.metadata.get("semantics.async")
         self.enabled = enabled
         self.disable_logger = disable_logger
         self._closed = False
 
         self.render_history = []
         self.env = env
 
         self.render_mode = env.render_mode
 
-        if "rgb_array_list" != self.render_mode and "rgb_array" != self.render_mode:
-            logger.warn(
-                f"Disabling video recorder because environment {env} was not initialized with any compatible video "
-                "mode between `rgb_array` and `rgb_array_list`"
+        try:
+            # check that moviepy is now installed
+            import moviepy  # noqa: F401
+        except ImportError as e:
+            raise error.DependencyNotInstalled(
+                "moviepy is not installed, run `pip install moviepy`"
+            ) from e
+
+        if self.render_mode in {None, "human", "ansi", "ansi_list"}:
+            raise ValueError(
+                f"Render mode is {self.render_mode}, which is incompatible with"
+                f" RecordVideo. Initialize your environment with a render_mode"
+                f" that returns an image, such as rgb_array."
             )
-            # Disable since the environment has not been initialized with a compatible `render_mode`
-            self.enabled = False
 
         # Don't bother setting anything else if not enabled
         if not self.enabled:
             return
 
         if path is not None and base_path is not None:
             raise error.Error("You can pass at most one of `path` or `base_path`.")
@@ -140,17 +139,14 @@
             self.recorded_frames.append(frame)
 
     def close(self):
         """Flush all data to disk and close any open frame encoders."""
         if not self.enabled or self._closed:
             return
 
-        # First close the environment
-        self.env.close()
-
         # Close the encoder
         if len(self.recorded_frames) > 0:
             try:
                 from moviepy.video.io.ImageSequenceClip import ImageSequenceClip
             except ImportError as e:
                 raise error.DependencyNotInstalled(
                     "moviepy is not installed, run `pip install moviepy`"
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/normalize.py` & `gymnasium-0.29.0/gymnasium/wrappers/normalize.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,16 +59,21 @@
         Args:
             env (Env): The environment to apply the wrapper
             epsilon: A stability parameter that is used when scaling the observations.
         """
         gym.utils.RecordConstructorArgs.__init__(self, epsilon=epsilon)
         gym.Wrapper.__init__(self, env)
 
-        self.num_envs = getattr(env, "num_envs", 1)
-        self.is_vector_env = getattr(env, "is_vector_env", False)
+        try:
+            self.num_envs = self.get_wrapper_attr("num_envs")
+            self.is_vector_env = self.get_wrapper_attr("is_vector_env")
+        except AttributeError:
+            self.num_envs = 1
+            self.is_vector_env = False
+
         if self.is_vector_env:
             self.obs_rms = RunningMeanStd(shape=self.single_observation_space.shape)
         else:
             self.obs_rms = RunningMeanStd(shape=self.observation_space.shape)
         self.epsilon = epsilon
 
     def step(self, action):
@@ -117,16 +122,21 @@
             env (env): The environment to apply the wrapper
             epsilon (float): A stability parameter
             gamma (float): The discount factor that is used in the exponential moving average.
         """
         gym.utils.RecordConstructorArgs.__init__(self, gamma=gamma, epsilon=epsilon)
         gym.Wrapper.__init__(self, env)
 
-        self.num_envs = getattr(env, "num_envs", 1)
-        self.is_vector_env = getattr(env, "is_vector_env", False)
+        try:
+            self.num_envs = self.get_wrapper_attr("num_envs")
+            self.is_vector_env = self.get_wrapper_attr("is_vector_env")
+        except AttributeError:
+            self.num_envs = 1
+            self.is_vector_env = False
+
         self.return_rms = RunningMeanStd(shape=())
         self.returns = np.zeros(self.num_envs)
         self.gamma = gamma
         self.epsilon = epsilon
 
     def step(self, action):
         """Steps through the environment, normalizing the rewards returned."""
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/order_enforcing.py` & `gymnasium-0.29.0/gymnasium/wrappers/order_enforcing.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/pixel_observation.py` & `gymnasium-0.29.0/gymnasium/wrappers/pixel_observation.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/record_episode_statistics.py` & `gymnasium-0.29.0/gymnasium/wrappers/record_episode_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,22 +55,27 @@
         Args:
             env (Env): The environment to apply the wrapper
             deque_size: The size of the buffers :attr:`return_queue` and :attr:`length_queue`
         """
         gym.utils.RecordConstructorArgs.__init__(self, deque_size=deque_size)
         gym.Wrapper.__init__(self, env)
 
-        self.num_envs = getattr(env, "num_envs", 1)
+        try:
+            self.num_envs = self.get_wrapper_attr("num_envs")
+            self.is_vector_env = self.get_wrapper_attr("is_vector_env")
+        except AttributeError:
+            self.num_envs = 1
+            self.is_vector_env = False
+
         self.episode_count = 0
         self.episode_start_times: np.ndarray = None
         self.episode_returns: Optional[np.ndarray] = None
         self.episode_lengths: Optional[np.ndarray] = None
         self.return_queue = deque(maxlen=deque_size)
         self.length_queue = deque(maxlen=deque_size)
-        self.is_vector_env = getattr(env, "is_vector_env", False)
 
     def reset(self, **kwargs):
         """Resets the environment using kwargs and resets the episode returns and lengths."""
         obs, info = super().reset(**kwargs)
         self.episode_start_times = np.full(
             self.num_envs, time.perf_counter(), dtype=np.float32
         )
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/record_video.py` & `gymnasium-0.29.0/gymnasium/wrappers/record_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,21 @@
             step_trigger=step_trigger,
             video_length=video_length,
             name_prefix=name_prefix,
             disable_logger=disable_logger,
         )
         gym.Wrapper.__init__(self, env)
 
+        if env.render_mode in {None, "human", "ansi", "ansi_list"}:
+            raise ValueError(
+                f"Render mode is {env.render_mode}, which is incompatible with"
+                f" RecordVideo. Initialize your environment with a render_mode"
+                f" that returns an image, such as rgb_array."
+            )
+
         if episode_trigger is None and step_trigger is None:
             episode_trigger = capped_cubic_video_schedule
 
         trigger_count = sum(x is not None for x in [episode_trigger, step_trigger])
         assert trigger_count == 1, "Must specify exactly one trigger"
 
         self.episode_trigger = episode_trigger
@@ -94,25 +101,29 @@
         self.step_id = 0
         self.video_length = video_length
 
         self.recording = False
         self.terminated = False
         self.truncated = False
         self.recorded_frames = 0
-        self.is_vector_env = getattr(env, "is_vector_env", False)
         self.episode_id = 0
 
+        try:
+            self.is_vector_env = self.get_wrapper_attr("is_vector_env")
+        except AttributeError:
+            self.is_vector_env = False
+
     def reset(self, **kwargs):
         """Reset the environment using kwargs and then starts recording if video enabled."""
         observations = super().reset(**kwargs)
         self.terminated = False
         self.truncated = False
         if self.recording:
             assert self.video_recorder is not None
-            self.video_recorder.frames = []
+            self.video_recorder.recorded_frames = []
             self.video_recorder.capture_frame()
             self.recorded_frames += 1
             if self.video_length > 0:
                 if self.recorded_frames > self.video_length:
                     self.close_video_recorder()
         elif self._video_enabled():
             self.start_video_recorder()
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/render_collection.py` & `gymnasium-0.29.0/gymnasium/wrappers/render_collection.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/rescale_action.py` & `gymnasium-0.29.0/gymnasium/wrappers/rescale_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,21 @@
         self.min_action = (
             np.zeros(env.action_space.shape, dtype=env.action_space.dtype) + min_action
         )
         self.max_action = (
             np.zeros(env.action_space.shape, dtype=env.action_space.dtype) + max_action
         )
 
+        self.action_space = Box(
+            low=min_action,
+            high=max_action,
+            shape=env.action_space.shape,
+            dtype=env.action_space.dtype,
+        )
+
     def action(self, action):
         """Rescales the action affinely from  [:attr:`min_action`, :attr:`max_action`] to the action space of the base environment, :attr:`env`.
 
         Args:
             action: The action to rescale
 
         Returns:
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/resize_observation.py` & `gymnasium-0.29.0/gymnasium/wrappers/resize_observation.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/step_api_compatibility.py` & `gymnasium-0.29.0/gymnasium/wrappers/step_api_compatibility.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/time_aware_observation.py` & `gymnasium-0.29.0/gymnasium/wrappers/time_aware_observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,19 @@
         gym.ObservationWrapper.__init__(self, env)
 
         assert isinstance(env.observation_space, Box)
         assert env.observation_space.dtype == np.float32
         low = np.append(self.observation_space.low, 0.0)
         high = np.append(self.observation_space.high, np.inf)
         self.observation_space = Box(low, high, dtype=np.float32)
-        self.is_vector_env = getattr(env, "is_vector_env", False)
+
+        try:
+            self.is_vector_env = self.get_wrapper_attr("is_vector_env")
+        except AttributeError:
+            self.is_vector_env = False
 
     def observation(self, observation):
         """Adds to the observation with the current time step.
 
         Args:
             observation: The observation to add the time step to
```

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/time_limit.py` & `gymnasium-0.29.0/gymnasium/wrappers/time_limit.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/transform_observation.py` & `gymnasium-0.29.0/gymnasium/wrappers/transform_observation.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium/wrappers/transform_reward.py` & `gymnasium-0.29.0/gymnasium/wrappers/transform_reward.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/gymnasium.egg-info/PKG-INFO` & `gymnasium-0.29.0/gymnasium.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gymnasium
-Version: 0.28.1
+Version: 0.29.0
 Summary: A standard API for reinforcement learning and a diverse set of reference environments (formerly Gym).
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://farama.org
 Project-URL: Repository, https://github.com/Farama-Foundation/Gymnasium
 Project-URL: Documentation, https://gymnasium.farama.org
 Project-URL: Bug Report, https://github.com/Farama-Foundation/Gymnasium/issues
 Keywords: Reinforcement Learning,game,RL,AI,gymnasium
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: atari
 Provides-Extra: accept-rom-license
 Provides-Extra: box2d
 Provides-Extra: classic-control
 Provides-Extra: classic_control
 Provides-Extra: mujoco-py
@@ -33,15 +32,16 @@
 Provides-Extra: toy_text
 Provides-Extra: jax
 Provides-Extra: other
 Provides-Extra: all
 Provides-Extra: testing
 License-File: LICENSE
 
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8127025.svg)](https://doi.org/10.5281/zenodo.8127025)
+
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/Gymnasium/main/gymnasium-text.png" width="500px"/>
 </p>
 
 Gymnasium is an open source Python library for developing and comparing reinforcement learning algorithms by providing a standard API to communicate between learning algorithms and environments, as well as a standard set of environments compliant with that API. This is a fork of OpenAI's [Gym](https://github.com/openai/gym) library by it's maintainers (OpenAI handed over maintenance a few years ago to an outside team), and is where future maintenance will occur going forward.
 
@@ -59,15 +59,15 @@
 
 ## Installation
 
 To install the base Gymnasium library, use `pip install gymnasium`
 
 This does not include dependencies for all families of environments (there's a massive number, and some can be problematic to install on certain systems). You can install these dependencies for one family like `pip install "gymnasium[atari]"` or use `pip install "gymnasium[all]"` to install all dependencies.
 
-We support and test for Python 3.7, 3.8, 3.9, 3.10, 3.11 on Linux and macOS. We will accept PRs related to Windows, but do not officially support it.
+We support and test for Python 3.8, 3.9, 3.10, 3.11 on Linux and macOS. We will accept PRs related to Windows, but do not officially support it.
 
 ## API
 
 The Gymnasium API models environments as simple Python `env` classes. Creating environment instances and interacting with them is very simple- here's an example using the "CartPole-v1" environment:
 
 ```python
 import gymnasium as gym
@@ -86,20 +86,40 @@
 ## Notable Related Libraries
 
 Please note that this is an incomplete list, and just includes libraries that the maintainers most commonly point newcommers to when asked for recommendations.
 
 * [CleanRL](https://github.com/vwxyzjn/cleanrl) is a learning library based on the Gymnasium API. It is designed to cater to newer people in the field and provides very good reference implementations.
 * [PettingZoo](https://github.com/Farama-Foundation/PettingZoo) is a multi-agent version of Gymnasium with a number of implemented environments, i.e. multi-agent Atari environments.
 * The Farama Foundation also has a collection of many other [environments](https://farama.org/projects) that are maintained by the same team as Gymnasium and use the Gymnasium API.
-* If you're looking to track your rewards, hyperparameters, random seeds and more you can use [Comet](https://www.comet.com/site/?utm_source=gymnasium&utm_medium=partner&utm_campaign=partner_gymnasium_2023&utm_content=github) which has a built-in integration for Gymnasium. [Here's tutorial on how to use them together](https://bit.ly/CometGymnasiumIntegration). Comet is a sponsor of the Farama Foundation.
+* [Comet](https://www.comet.com/site/?utm_source=gymnasium&utm_medium=partner&utm_campaign=partner_gymnasium_2023&utm_content=github) is a free ML-Ops tool that tracks rewards, metrics, hyperparameters, and code for ML training runs. Comet has an easy-to use integration with Gymnasium, here's a [tutorial](https://bit.ly/CometGymnasiumIntegration) on how to use them together! Comet is a sponsor of the Farama Foundation!
+
+
 
 ## Environment Versioning
 
 Gymnasium keeps strict versioning for reproducibility reasons. All environments end in a suffix like "-v0".  When changes are made to environments that might impact learning results, the number is increased by one to prevent potential confusion. These inherent from Gym.
 
 ## Development Roadmap
 
 We have a roadmap for future development work for Gymnasium available here: https://github.com/Farama-Foundation/Gymnasium/issues/12
 
 ## Support Gymnasium's Development
 
 If you are financially able to do so and would like to support the development of Gymnasium, please join others in the community in [donating to us](https://github.com/sponsors/Farama-Foundation).
+
+## Citation
+
+You can cite Gymnasium as:
+
+```
+@misc{towers_gymnasium_2023,
+        title = {Gymnasium},
+        url = {https://zenodo.org/record/8127025},
+        abstract = {An API standard for single-agent reinforcement learning environments, with popular reference environments and related utilities (formerly Gym)},
+        urldate = {2023-07-08},
+        publisher = {Zenodo},
+        author = {Towers, Mark and Terry, Jordan K. and Kwiatkowski, Ariel and Balis, John U. and Cola, Gianluca de and Deleu, Tristan and Goulão, Manuel and Kallinteris, Andreas and KG, Arjun and Krimmel, Markus and Perez-Vicente, Rodrigo and Pierré, Andrea and Schulhoff, Sander and Tai, Jun Jet and Shen, Andrew Tan Jin and Younis, Omar G.},
+        month = mar,
+        year = {2023},
+        doi = {10.5281/zenodo.8127026},
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gymnasium-0.28.1/gymnasium.egg-info/SOURCES.txt` & `gymnasium-0.29.0/gymnasium.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -69,16 +69,18 @@
 gymnasium/envs/mujoco/assets/pusher.xml
 gymnasium/envs/mujoco/assets/reacher.xml
 gymnasium/envs/mujoco/assets/swimmer.xml
 gymnasium/envs/mujoco/assets/walker2d.xml
 gymnasium/envs/phys2d/__init__.py
 gymnasium/envs/phys2d/cartpole.py
 gymnasium/envs/phys2d/pendulum.py
+gymnasium/envs/phys2d/assets/clockwise.png
 gymnasium/envs/tabular/__init__.py
 gymnasium/envs/tabular/blackjack.py
+gymnasium/envs/tabular/cliffwalking.py
 gymnasium/envs/toy_text/__init__.py
 gymnasium/envs/toy_text/blackjack.py
 gymnasium/envs/toy_text/cliffwalking.py
 gymnasium/envs/toy_text/frozen_lake.py
 gymnasium/envs/toy_text/taxi.py
 gymnasium/envs/toy_text/utils.py
 gymnasium/envs/toy_text/font/Minecraft.ttf
@@ -176,24 +178,31 @@
 gymnasium/experimental/vector/utils/space_utils.py
 gymnasium/experimental/wrappers/__init__.py
 gymnasium/experimental/wrappers/atari_preprocessing.py
 gymnasium/experimental/wrappers/common.py
 gymnasium/experimental/wrappers/jax_to_numpy.py
 gymnasium/experimental/wrappers/jax_to_torch.py
 gymnasium/experimental/wrappers/lambda_action.py
-gymnasium/experimental/wrappers/lambda_observations.py
+gymnasium/experimental/wrappers/lambda_observation.py
 gymnasium/experimental/wrappers/lambda_reward.py
 gymnasium/experimental/wrappers/numpy_to_torch.py
 gymnasium/experimental/wrappers/rendering.py
 gymnasium/experimental/wrappers/stateful_action.py
 gymnasium/experimental/wrappers/stateful_observation.py
+gymnasium/experimental/wrappers/stateful_reward.py
 gymnasium/experimental/wrappers/utils.py
 gymnasium/experimental/wrappers/vector/__init__.py
+gymnasium/experimental/wrappers/vector/dict_info_to_list.py
+gymnasium/experimental/wrappers/vector/jax_to_numpy.py
+gymnasium/experimental/wrappers/vector/jax_to_torch.py
+gymnasium/experimental/wrappers/vector/numpy_to_torch.py
 gymnasium/experimental/wrappers/vector/record_episode_statistics.py
-gymnasium/experimental/wrappers/vector/vector_list_info.py
+gymnasium/experimental/wrappers/vector/vectorize_action.py
+gymnasium/experimental/wrappers/vector/vectorize_observation.py
+gymnasium/experimental/wrappers/vector/vectorize_reward.py
 gymnasium/spaces/__init__.py
 gymnasium/spaces/box.py
 gymnasium/spaces/dict.py
 gymnasium/spaces/discrete.py
 gymnasium/spaces/graph.py
 gymnasium/spaces/multi_binary.py
 gymnasium/spaces/multi_discrete.py
@@ -201,16 +210,18 @@
 gymnasium/spaces/space.py
 gymnasium/spaces/text.py
 gymnasium/spaces/tuple.py
 gymnasium/spaces/utils.py
 gymnasium/utils/__init__.py
 gymnasium/utils/colorize.py
 gymnasium/utils/env_checker.py
+gymnasium/utils/env_match.py
 gymnasium/utils/ezpickle.py
 gymnasium/utils/passive_env_checker.py
+gymnasium/utils/performance.py
 gymnasium/utils/play.py
 gymnasium/utils/record_constructor.py
 gymnasium/utils/save_video.py
 gymnasium/utils/seeding.py
 gymnasium/utils/step_api_compatibility.py
 gymnasium/vector/__init__.py
 gymnasium/vector/async_vector_env.py
```

### Comparing `gymnasium-0.28.1/gymnasium.egg-info/requires.txt` & `gymnasium-0.29.0/gymnasium.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 numpy>=1.21.0
-jax-jumpy>=1.0.0
 cloudpickle>=1.2.0
 typing-extensions>=4.3.0
 farama-notifications>=0.0.1
 
 [:python_version < "3.10"]
 importlib-metadata>=4.8.0
 
 [accept-rom-license]
 autorom[accept-rom-license]~=0.4.2
 
 [all]
 shimmy[atari]<1.0,>=0.1.0
 box2d-py==2.3.5
-pygame==2.1.3
+pygame>=2.1.3
 swig==4.*
 mujoco-py<2.2,>=2.1
-mujoco>=2.3.2
+mujoco>=2.3.3
 imageio>=2.14.1
-jax==0.3.24
-jaxlib==0.3.24
+jax>=0.4.0
+jaxlib>=0.4.0
 lz4>=3.1.0
 opencv-python>=3.0
 matplotlib>=3.0
 moviepy>=1.0.0
 torch>=1.0.0
 
 [atari]
 shimmy[atari]<1.0,>=0.1.0
 
 [box2d]
 box2d-py==2.3.5
-pygame==2.1.3
+pygame>=2.1.3
 swig==4.*
 
 [classic-control]
-pygame==2.1.3
+pygame>=2.1.3
 
 [classic_control]
-pygame==2.1.3
+pygame>=2.1.3
 
 [jax]
-jax==0.3.24
-jaxlib==0.3.24
+jax>=0.4.0
+jaxlib>=0.4.0
 
 [mujoco]
-mujoco>=2.3.2
+mujoco>=2.3.3
 imageio>=2.14.1
 
 [mujoco-py]
 mujoco-py<2.2,>=2.1
 
 [mujoco_py]
 mujoco-py<2.2,>=2.1
@@ -59,14 +58,14 @@
 opencv-python>=3.0
 matplotlib>=3.0
 moviepy>=1.0.0
 torch>=1.0.0
 
 [testing]
 pytest==7.1.3
-scipy==1.7.3
+scipy>=1.7.3
 
 [toy-text]
-pygame==2.1.3
+pygame>=2.1.3
 
 [toy_text]
-pygame==2.1.3
+pygame>=2.1.3
```

### Comparing `gymnasium-0.28.1/pyproject.toml` & `gymnasium-0.29.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,91 +4,89 @@
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gymnasium"
 description = "A standard API for reinforcement learning and a diverse set of reference environments (formerly Gym)."
 readme = "README.md"
-requires-python = ">= 3.7"
+requires-python = ">= 3.8"
 authors = [{ name = "Farama Foundation", email = "contact@farama.org" }]
 license = { text = "MIT License" }
 keywords = ["Reinforcement Learning", "game", "RL", "AI", "gymnasium"]
 classifiers = [
     "Development Status :: 4 - Beta",  # change to `5 - Production/Stable` when ready
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
 ]
 dependencies = [
     "numpy >=1.21.0",
-    "jax-jumpy>=1.0.0",
     "cloudpickle >=1.2.0",
     "importlib-metadata >=4.8.0; python_version < '3.10'",
     "typing-extensions >=4.3.0",
     "farama-notifications >=0.0.1",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 # Update dependencies in `all` if any are added or removed
 atari = ["shimmy[atari] >=0.1.0,<1.0"]
 accept-rom-license = ["autorom[accept-rom-license] ~=0.4.2"]
-box2d = ["box2d-py ==2.3.5", "pygame ==2.1.3", "swig ==4.*"]
-classic-control = ["pygame ==2.1.3"]
-classic_control = ["pygame ==2.1.3"]  # kept for backward compatibility
+box2d = ["box2d-py ==2.3.5", "pygame >=2.1.3", "swig ==4.*"]
+classic-control = ["pygame >=2.1.3"]
+classic_control = ["pygame >=2.1.3"]  # kept for backward compatibility
 mujoco-py = ["mujoco-py >=2.1,<2.2"]
 mujoco_py = ["mujoco-py >=2.1,<2.2"]       # kept for backward compatibility
-mujoco = ["mujoco >=2.3.2", "imageio >=2.14.1"]
-toy-text = ["pygame ==2.1.3"]
-toy_text = ["pygame ==2.1.3"]         # kept for backward compatibility
-jax = ["jax ==0.3.24", "jaxlib ==0.3.24"]
+mujoco = ["mujoco >=2.3.3", "imageio >=2.14.1"]
+toy-text = ["pygame >=2.1.3"]
+toy_text = ["pygame >=2.1.3"]         # kept for backward compatibility
+jax = ["jax >=0.4.0", "jaxlib >=0.4.0"]
 other = [
     "lz4 >=3.1.0",
     "opencv-python >=3.0",
     "matplotlib >=3.0",
     "moviepy >=1.0.0",
     "torch >=1.0.0",
 ]
 all = [
     # All dependencies above except accept-rom-license
     # NOTE: No need to manually remove the duplicates, setuptools automatically does that.
     # atari
     "shimmy[atari] >=0.1.0,<1.0",
     # box2d
     "box2d-py ==2.3.5",
-    "pygame ==2.1.3",
+    "pygame >=2.1.3",
     "swig ==4.*",
     # classic-control
-    "pygame ==2.1.3",
+    "pygame >=2.1.3",
     # mujoco-py
     "mujoco-py >=2.1,<2.2",
     # mujoco
-    "mujoco >=2.3.2",
+    "mujoco >=2.3.3",
     "imageio >=2.14.1",
     # toy-text
-    "pygame ==2.1.3",
+    "pygame >=2.1.3",
     # jax
-    "jax ==0.3.24",
-    "jaxlib ==0.3.24",
+    "jax >=0.4.0",
+    "jaxlib >=0.4.0",
     # other
     "lz4 >=3.1.0",
     "opencv-python >=3.0",
     "matplotlib >=3.0",
     "moviepy >=1.0.0",
     "torch >=1.0.0",
 ]
 testing = [
     "pytest ==7.1.3",
-    "scipy ==1.7.3",
+    "scipy >= 1.7.3",
 ]
 
 [project.urls]
 Homepage = "https://farama.org"
 Repository = "https://github.com/Farama-Foundation/Gymnasium"
 Documentation = "https://gymnasium.farama.org"
 "Bug Report" = "https://github.com/Farama-Foundation/Gymnasium/issues"
@@ -99,40 +97,41 @@
 [tool.setuptools.packages.find]
 include = ["gymnasium", "gymnasium.*"]
 
 [tool.setuptools.package-data]
 gymnasium = [
     "envs/mujoco/assets/*.xml",
     "envs/classic_control/assets/*.png",
+    "envs/phys2d/assets/*.png",
     "envs/toy_text/font/*.ttf",
     "envs/toy_text/img/*.png",
     "py.typed",
 ]
 
 # Linters and Test tools #######################################################
 
 [tool.black]
 safe = true
 
 [tool.isort]
 atomic = true
 profile = "black"
-src_paths = ["gymnasium", "tests", "docs/scripts"]
+src_paths = ["gymnasium", "tests", "docs/_scripts"]
 extra_standard_library = ["typing_extensions"]
 indent = 4
 lines_after_imports = 2
 multi_line_output = 3
 
 [tool.pyright]
 include = ["gymnasium/**", "tests/**"]
 exclude = ["**/node_modules", "**/__pycache__"]
 strict = []
 
 typeCheckingMode = "basic"
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 pythonPlatform = "All"
 typeshedPath = "typeshed"
 enableTypeIgnoreComments = true
 
 # This is required as the CI pre-commit does not download the module (i.e. numpy, pygame, box2d)
 #   Therefore, we have to ignore missing imports
 reportMissingImports = "none"
@@ -142,14 +141,14 @@
 reportInvalidTypeVarUse = "none"
 
 # reportUnknownMemberType = "warning"  # -> raises 6035 warnings
 # reportUnknownParameterType = "warning"  # -> raises 1327 warnings
 # reportUnknownVariableType = "warning"  # -> raises 2585 warnings
 # reportUnknownArgumentType = "warning"  # -> raises 2104 warnings
 reportGeneralTypeIssues = "none"  # -> commented out raises 489 errors
-reportUntypedFunctionDecorator = "none"  # -> pytest.mark.parameterize issues
+# reportUntypedFunctionDecorator = "none"  # -> pytest.mark.parameterize issues
 
 reportPrivateUsage = "warning"
 reportUnboundVariable = "warning"
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning:gymnasium.*:"]
```

### Comparing `gymnasium-0.28.1/setup.py` & `gymnasium-0.29.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Setups the project."""
+"""Sets up the project."""
 
 import pathlib
 
 from setuptools import setup
 
 
 CWD = pathlib.Path(__file__).absolute().parent
```

### Comparing `gymnasium-0.28.1/tests/test_core.py` & `gymnasium-0.29.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.28.1/tests/testing_env.py` & `gymnasium-0.29.0/tests/testing_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         observation_space: spaces.Space = spaces.Box(0, 1, (1,)),
         reset_func: Callable = basic_reset_func,
         step_func: Callable = basic_step_func,
         render_func: Callable = basic_render_func,
         metadata: dict[str, Any] = {"render_modes": []},
         render_mode: str | None = None,
         spec: EnvSpec = EnvSpec(
-            "TestingEnv-v0", "testing-env-no-entry-point", max_episode_steps=100
+            "TestingEnv-v0", "tests.testing_env:GenericTestEnv", max_episode_steps=100
         ),
     ):
         """Generic testing environment constructor.
 
         Args:
             action_space: The environment action space
             observation_space: The environment observation space
```

