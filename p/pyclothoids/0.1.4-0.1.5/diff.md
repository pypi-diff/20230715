# Comparing `tmp/pyclothoids-0.1.4.tar.gz` & `tmp/pyclothoids-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\phild\Documents\Code\pyclothoids\dist\tmpdmmm7cf6\pyclothoids-0.1.4.tar", last modified: Fri Oct 29 04:02:59 2021, max compression
+gzip compressed data, was "C:\Users\phild\Documents\Code\pyclothoids\dist\.tmp-3ac4zm4t\pyclothoids-0.1.5.tar", last modified: Sat Jul 15 19:47:45 2023, max compression
```

## Comparing `pyclothoids-0.1.4.tar` & `pyclothoids-0.1.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/
--rw-rw-rw-   0        0        0     1089 2021-10-29 02:54:29.000000 pyclothoids-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      197 2021-10-29 02:54:29.000000 pyclothoids-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2353 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2028 2021-10-29 02:54:29.000000 pyclothoids-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids/
--rw-rw-rw-   0        0        0       39 2021-10-29 02:54:29.000000 pyclothoids-0.1.4/pyclothoids/__init__.py
--rw-rw-rw-   0        0        0     7813 2021-10-29 02:54:29.000000 pyclothoids-0.1.4/pyclothoids/clothoid.py
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids/src/
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/
--rw-rw-rw-   0        0        0    11902 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/AABBtree.cc
--rw-rw-rw-   0        0        0    10114 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/AABBtree.hh
--rw-rw-rw-   0        0        0     4099 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/BaseCurve_using.hxx
--rw-rw-rw-   0        0        0    26457 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Biarc.cc
--rw-rw-rw-   0        0        0    16279 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Biarc.hh
--rw-rw-rw-   0        0        0    38912 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/BiarcList.cc
--rw-rw-rw-   0        0        0    21888 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/BiarcList.hh
--rw-rw-rw-   0        0        0    23923 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Circle.cc
--rw-rw-rw-   0        0        0    17345 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Circle.hh
--rw-rw-rw-   0        0        0    24350 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Clothoid.cc
--rw-rw-rw-   0        0        0    30829 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Clothoid.hh
--rw-rw-rw-   0        0        0     3161 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidAsyPlot.hh
--rw-rw-rw-   0        0        0    15947 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidDistance.cc
--rw-rw-rw-   0        0        0    46631 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidG2.cc
--rw-rw-rw-   0        0        0    52265 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidList.cc
--rw-rw-rw-   0        0        0    42827 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidList.hh
--rw-rw-rw-   0        0        0    42321 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Fresnel.cc
--rw-rw-rw-   0        0        0    13771 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Fresnel.hh
--rw-rw-rw-   0        0        0    27928 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/G2lib.cc
--rw-rw-rw-   0        0        0    57204 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/G2lib.hh
--rw-rw-rw-   0        0        0    16680 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/G2lib_intersect.cc
--rw-rw-rw-   0        0        0    16276 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Line.cc
--rw-rw-rw-   0        0        0    17072 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Line.hh
--rw-rw-rw-   0        0        0    21020 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/PolyLine.cc
--rw-rw-rw-   0        0        0    14004 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/PolyLine.hh
--rw-rw-rw-   0        0        0     8405 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Triangle2D.cc
--rw-rw-rw-   0        0        0     6910 2021-10-29 04:00:57.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Triangle2D.hh
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/
--rw-rw-rw-   0        0        0     6188 2021-10-29 04:02:22.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-1-Quadratic.cc
--rw-rw-rw-   0        0        0    15893 2021-10-29 04:02:22.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-2-Cubic.cc
--rw-rw-rw-   0        0        0    25550 2021-10-29 04:02:22.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-3-Quartic.cc
--rw-rw-rw-   0        0        0    26814 2021-10-29 04:02:22.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Jenkins-Traub.cc
--rw-rw-rw-   0        0        0     9011 2021-10-29 04:02:22.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Utils.cc
--rw-rw-rw-   0        0        0     3966 2021-10-29 04:02:22.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Utils.hh
--rw-rw-rw-   0        0        0    22131 2021-10-29 04:02:22.000000 pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots.hh
--rw-rw-rw-   0        0        0     4157 2021-10-29 02:54:29.000000 pyclothoids-0.1.4/pyclothoids/src/main.cpp
-drwxrwxrwx   0        0        0        0 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids.egg-info/
--rw-rw-rw-   0        0        0     2353 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2456 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/pyclothoids.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-10-29 04:02:59.000000 pyclothoids-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     5418 2021-10-29 02:56:23.000000 pyclothoids-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/
+-rw-rw-rw-   0        0        0     1089 2021-10-29 02:54:29.000000 pyclothoids-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      197 2021-10-29 02:54:29.000000 pyclothoids-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2312 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2028 2021-10-29 02:54:29.000000 pyclothoids-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids/
+-rw-rw-rw-   0        0        0       39 2021-10-29 02:54:29.000000 pyclothoids-0.1.5/pyclothoids/__init__.py
+-rw-rw-rw-   0        0        0     7930 2023-05-22 02:07:28.000000 pyclothoids-0.1.5/pyclothoids/clothoid.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/
+-rw-rw-rw-   0        0        0    11902 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/AABBtree.cc
+-rw-rw-rw-   0        0        0    10114 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/AABBtree.hh
+-rw-rw-rw-   0        0        0     4099 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/BaseCurve_using.hxx
+-rw-rw-rw-   0        0        0    26457 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Biarc.cc
+-rw-rw-rw-   0        0        0    16279 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Biarc.hh
+-rw-rw-rw-   0        0        0    38912 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/BiarcList.cc
+-rw-rw-rw-   0        0        0    21888 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/BiarcList.hh
+-rw-rw-rw-   0        0        0    23923 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Circle.cc
+-rw-rw-rw-   0        0        0    17345 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Circle.hh
+-rw-rw-rw-   0        0        0    24350 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Clothoid.cc
+-rw-rw-rw-   0        0        0    30829 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Clothoid.hh
+-rw-rw-rw-   0        0        0     3161 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidAsyPlot.hh
+-rw-rw-rw-   0        0        0    15947 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidDistance.cc
+-rw-rw-rw-   0        0        0    46631 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidG2.cc
+-rw-rw-rw-   0        0        0    52265 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidList.cc
+-rw-rw-rw-   0        0        0    42827 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidList.hh
+-rw-rw-rw-   0        0        0    42321 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Fresnel.cc
+-rw-rw-rw-   0        0        0    13771 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Fresnel.hh
+-rw-rw-rw-   0        0        0    27928 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/G2lib.cc
+-rw-rw-rw-   0        0        0    57204 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/G2lib.hh
+-rw-rw-rw-   0        0        0    16680 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/G2lib_intersect.cc
+-rw-rw-rw-   0        0        0    16276 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Line.cc
+-rw-rw-rw-   0        0        0    17072 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Line.hh
+-rw-rw-rw-   0        0        0    21020 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/PolyLine.cc
+-rw-rw-rw-   0        0        0    14004 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/PolyLine.hh
+-rw-rw-rw-   0        0        0     8405 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Triangle2D.cc
+-rw-rw-rw-   0        0        0     6910 2021-10-29 04:00:57.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Triangle2D.hh
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/
+-rw-rw-rw-   0        0        0     6188 2021-10-29 04:02:22.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-1-Quadratic.cc
+-rw-rw-rw-   0        0        0    15893 2021-10-29 04:02:22.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-2-Cubic.cc
+-rw-rw-rw-   0        0        0    25550 2021-10-29 04:02:22.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-3-Quartic.cc
+-rw-rw-rw-   0        0        0    26814 2021-10-29 04:02:22.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Jenkins-Traub.cc
+-rw-rw-rw-   0        0        0     9011 2021-10-29 04:02:22.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Utils.cc
+-rw-rw-rw-   0        0        0     3966 2021-10-29 04:02:22.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Utils.hh
+-rw-rw-rw-   0        0        0    22131 2021-10-29 04:02:22.000000 pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots.hh
+-rw-rw-rw-   0        0        0     4157 2021-10-29 02:54:29.000000 pyclothoids-0.1.5/pyclothoids/src/main.cpp
+drwxrwxrwx   0        0        0        0 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids.egg-info/
+-rw-rw-rw-   0        0        0     2312 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2456 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-10-29 04:02:59.000000 pyclothoids-0.1.5/pyclothoids.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/pyclothoids.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 19:47:45.000000 pyclothoids-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     5418 2023-07-15 17:42:03.000000 pyclothoids-0.1.5/setup.py
```

### Comparing `pyclothoids-0.1.4/LICENSE` & `pyclothoids-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/PKG-INFO` & `pyclothoids-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyclothoids
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for clothoid curves in Python
 Home-page: https://github.com/phillipd94/PyClothoids
 Author: Phillip Dix
 Author-email: phildix11@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyclothoids
 A Python library for clothoid curves
 
 [Read the Documentation!](https://pyclothoids.readthedocs.io/en/latest/)
@@ -20,9 +18,7 @@
 There has been significant research into numerical algorithms to evaluate, construct, and manipulate these curves.  Software packages exist for this purpose but are often difficult to master.  This package takes a different approach, aiming to be easy to pick up and experiment with.  The ultimate goal is to provide a simple, intuitive, and pythonic interface to state of the art numerical software that allows you to leverage the latest research without the learning curve.
 
 If you have a problem that you think could be solved using clothoid curves, this package aims to handle all the complexities of clothoid geometry for you so that you can focus on the top level problem you are trying to solve.  
 
 That said, clothoid curves aren't always well behaved, and there are many other simpler curves that are far easier to understand and manipulate.  Before you use this library for a project, be sure that other simpler geometric constructs such as B-splines will not fulfill your needs.
 
 The main design goals of pyclothoids are minimalism and simplicity.  For that reason, the top level API for this module consists of only one class - Clothoid.  To prevent common errors and further simplify the interface, Clothoid was designed to be immutable from the top level.  This means any methods that transform a Clothoid will return a new Clothoid with the desired modifications while leaving the original Clothoid intact.
-
-
```

### Comparing `pyclothoids-0.1.4/README.md` & `pyclothoids-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/clothoid.py` & `pyclothoids-0.1.5/pyclothoids/clothoid.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             return getattr(self._ClothoidCurve,name)
         if name in CLOTHOID_PROPERTY_WINDOW:
             return getattr(self._ClothoidCurve,name)() #mimic property getter syntax
         return super().__getattribute__(name)()
 
     def __str__(self):
         return 'Clothoid: ' + ''.join(map(lambda m,n:m + ':' + str(getattr(self,n)) + ' ',
-                                             ('x0','y0','y0','k0','kd','s'),('XStart','YStart','ThetaStart','KappaStart','dk','length')))
+                                             ('x0','y0','t0','k0','kd','s'),('XStart','YStart','ThetaStart','KappaStart','dk','length')))
 
     def __repr__(self):
         return str(self)
 
     def __getstate__(self):
         return self.Parameters
 
@@ -176,16 +176,17 @@
             return Clothoid.StandardParams(-xp,yp,atan2(dy,-dx),-self.KappaStart,-self.dk,self.length)
         if axis == 'x':
             return Clothoid.StandardParams(xp,-yp,atan2(-dy,dx),-self.KappaStart,-self.dk,self.length)
         if axis == 'start':
             return Clothoid.StandardParams(xp,yp,th,-self.KappaStart,-self.dk,self.length)
 
 
-def SolveG2(x0,y0,t0,k0,x1,y1,t1,k1):
+def SolveG2(x0,y0,t0,k0,x1,y1,t1,k1,Dmax=0,dmax=0):
     """
     Returns a tuple of three Clothoids that form a G2 continuous path that interpolates two cartesian
-    endpoints, two tangents, and two curvatures
+    endpoints, two tangents, and two curvatures.  Exposes two additional parameters for fine tuning
+    the properties of the desired solution.
     """
     solver = G2solve3arc()
-    solver.build(x0,y0,t0,k0,x1,y1,t1,k1,0,0)
+    solver.build(x0,y0,t0,k0,x1,y1,t1,k1,Dmax,dmax)
     return tuple(map(Clothoid,(solver.getS0(),solver.getSM(),solver.getS1())))
```

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/AABBtree.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/AABBtree.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/AABBtree.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/AABBtree.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/BaseCurve_using.hxx` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/BaseCurve_using.hxx`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Biarc.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Biarc.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Biarc.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Biarc.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/BiarcList.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/BiarcList.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/BiarcList.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/BiarcList.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Circle.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Circle.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Circle.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Circle.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Clothoid.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Clothoid.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Clothoid.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Clothoid.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidAsyPlot.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidAsyPlot.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidDistance.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidDistance.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidG2.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidG2.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidList.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidList.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/ClothoidList.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/ClothoidList.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Fresnel.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Fresnel.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Fresnel.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Fresnel.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/G2lib.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/G2lib.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/G2lib.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/G2lib.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/G2lib_intersect.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/G2lib_intersect.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Line.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Line.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Line.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Line.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/PolyLine.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/PolyLine.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/PolyLine.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/PolyLine.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Triangle2D.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Triangle2D.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/src/Triangle2D.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/src/Triangle2D.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-1-Quadratic.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-1-Quadratic.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-2-Cubic.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-2-Cubic.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-3-Quartic.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-3-Quartic.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Jenkins-Traub.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Jenkins-Traub.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Utils.cc` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Utils.cc`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Utils.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots-Utils.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots.hh` & `pyclothoids-0.1.5/pyclothoids/src/Submodules/Clothoids/submodules/quarticRootsFlocke/src/PolynomialRoots.hh`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids/src/main.cpp` & `pyclothoids-0.1.5/pyclothoids/src/main.cpp`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/pyclothoids.egg-info/PKG-INFO` & `pyclothoids-0.1.5/pyclothoids.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyclothoids
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for clothoid curves in Python
 Home-page: https://github.com/phillipd94/PyClothoids
 Author: Phillip Dix
 Author-email: phildix11@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyclothoids
 A Python library for clothoid curves
 
 [Read the Documentation!](https://pyclothoids.readthedocs.io/en/latest/)
@@ -20,9 +18,7 @@
 There has been significant research into numerical algorithms to evaluate, construct, and manipulate these curves.  Software packages exist for this purpose but are often difficult to master.  This package takes a different approach, aiming to be easy to pick up and experiment with.  The ultimate goal is to provide a simple, intuitive, and pythonic interface to state of the art numerical software that allows you to leverage the latest research without the learning curve.
 
 If you have a problem that you think could be solved using clothoid curves, this package aims to handle all the complexities of clothoid geometry for you so that you can focus on the top level problem you are trying to solve.  
 
 That said, clothoid curves aren't always well behaved, and there are many other simpler curves that are far easier to understand and manipulate.  Before you use this library for a project, be sure that other simpler geometric constructs such as B-splines will not fulfill your needs.
 
 The main design goals of pyclothoids are minimalism and simplicity.  For that reason, the top level API for this module consists of only one class - Clothoid.  To prevent common errors and further simplify the interface, Clothoid was designed to be immutable from the top level.  This means any methods that transform a Clothoid will return a new Clothoid with the desired modifications while leaving the original Clothoid intact.
-
-
```

### Comparing `pyclothoids-0.1.4/pyclothoids.egg-info/SOURCES.txt` & `pyclothoids-0.1.5/pyclothoids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyclothoids-0.1.4/setup.py` & `pyclothoids-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 from pathlib import Path
 
 from os import listdir
 from os.path import isfile, join, abspath, dirname
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 
 class get_pybind_include(object):
     """Helper class to determine the pybind11 include path
 
     The purpose of this class is to postpone importing pybind11
     until it is actually installed, so that the ``get_include()``
```

