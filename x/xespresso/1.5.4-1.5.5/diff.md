# Comparing `tmp/xespresso-1.5.4.tar.gz` & `tmp/xespresso-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xespresso-1.5.4.tar", last modified: Sun Jan  1 21:29:27 2023, max compression
+gzip compressed data, was "dist/xespresso-1.5.5.tar", last modified: Sat Jul 15 12:38:55 2023, max compression
```

## Comparing `xespresso-1.5.4.tar` & `xespresso-1.5.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-01-01 21:29:27.934132 xespresso-1.5.4/
--rw-rw-r--   0 xing      (1000) xing      (1000)    35149 2020-10-07 08:05:45.000000 xespresso-1.5.4/LICENSE
--rw-rw-r--   0 xing      (1000) xing      (1000)     5926 2023-01-01 21:29:27.934132 xespresso-1.5.4/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     5462 2023-01-01 14:57:56.000000 xespresso-1.5.4/README.md
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2023-01-01 21:29:27.934132 xespresso-1.5.4/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)      909 2023-01-01 21:13:33.000000 xespresso-1.5.4/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-01-01 21:29:27.930132 xespresso-1.5.4/xespresso/
--rw-rw-r--   0 xing      (1000) xing      (1000)       41 2022-08-10 17:50:49.000000 xespresso-1.5.4/xespresso/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7393 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/cohp.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-01-01 21:29:27.930132 xespresso-1.5.4/xespresso/data/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-21 07:48:10.000000 xespresso-1.5.4/xespresso/data/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7244 2023-01-01 14:58:09.000000 xespresso-1.5.4/xespresso/data/pseudo.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    18703 2023-01-01 21:11:11.000000 xespresso-1.5.4/xespresso/dos.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    27084 2022-12-21 07:43:57.000000 xespresso-1.5.4/xespresso/hpxespresso.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    29500 2022-12-21 07:43:58.000000 xespresso-1.5.4/xespresso/input_parameters.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6917 2022-12-21 07:43:56.000000 xespresso-1.5.4/xespresso/neb.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-01-01 21:29:27.930132 xespresso-1.5.4/xespresso/post/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-08-10 17:05:22.000000 xespresso-1.5.4/xespresso/post/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      666 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/post/bands.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6655 2022-12-21 07:43:56.000000 xespresso-1.5.4/xespresso/post/base.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      669 2023-01-01 18:19:53.000000 xespresso-1.5.4/xespresso/post/dos.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      707 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/post/dynmat.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1069 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/post/hp.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1045 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/post/matdyn.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5822 2022-12-21 07:43:56.000000 xespresso-1.5.4/xespresso/post/nscf.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2083 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/post/ph.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1439 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/post/pp.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      884 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/post/projwfc.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      421 2022-12-21 07:43:55.000000 xespresso-1.5.4/xespresso/post/q2r.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2416 2022-12-21 07:43:56.000000 xespresso-1.5.4/xespresso/scheduler.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6777 2022-12-21 07:43:56.000000 xespresso-1.5.4/xespresso/tools.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    24768 2022-12-21 07:43:57.000000 xespresso-1.5.4/xespresso/uscsd.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-01-01 21:29:27.930132 xespresso-1.5.4/xespresso/utils/
--rw-rw-r--   0 xing      (1000) xing      (1000)     2421 2022-12-21 07:43:56.000000 xespresso-1.5.4/xespresso/utils/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3298 2022-12-21 07:43:56.000000 xespresso-1.5.4/xespresso/utils/qe_dos_parser.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7189 2022-12-21 07:43:57.000000 xespresso-1.5.4/xespresso/utils/xml_parser.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-01-01 21:29:27.934132 xespresso-1.5.4/xespresso/workflow/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2020-12-08 21:30:08.000000 xespresso-1.5.4/xespresso/workflow/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7263 2022-12-21 07:43:57.000000 xespresso-1.5.4/xespresso/workflow/base.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    32533 2022-12-21 07:43:58.000000 xespresso-1.5.4/xespresso/workflow/oer.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7086 2022-12-21 07:43:57.000000 xespresso-1.5.4/xespresso/workflow/phonon.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    30286 2023-01-01 14:58:10.000000 xespresso-1.5.4/xespresso/xespresso.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    20839 2023-01-01 17:01:38.000000 xespresso-1.5.4/xespresso/xio.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3352 2022-12-21 07:43:57.000000 xespresso-1.5.4/xespresso/xlog.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-01-01 21:29:27.930132 xespresso-1.5.4/xespresso.egg-info/
--rw-rw-r--   0 xing      (1000) xing      (1000)     5926 2023-01-01 21:29:27.000000 xespresso-1.5.4/xespresso.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      974 2023-01-01 21:29:27.000000 xespresso-1.5.4/xespresso.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2023-01-01 21:29:27.000000 xespresso-1.5.4/xespresso.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       27 2023-01-01 21:29:27.000000 xespresso-1.5.4/xespresso.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       10 2023-01-01 21:29:27.000000 xespresso-1.5.4/xespresso.egg-info/top_level.txt
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-15 12:38:55.482190 xespresso-1.5.5/
+-rw-rw-r--   0 xing      (1000) xing      (1000)    35149 2020-10-07 08:05:45.000000 xespresso-1.5.5/LICENSE
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6157 2023-07-15 12:38:55.482190 xespresso-1.5.5/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5693 2023-03-23 05:50:22.000000 xespresso-1.5.5/README.md
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2023-07-15 12:38:55.482190 xespresso-1.5.5/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)      909 2023-07-15 12:38:42.000000 xespresso-1.5.5/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-15 12:38:55.478190 xespresso-1.5.5/xespresso/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       41 2022-08-10 17:50:49.000000 xespresso-1.5.5/xespresso/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7393 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/cohp.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-15 12:38:55.478190 xespresso-1.5.5/xespresso/data/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/data/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7244 2023-06-13 12:28:02.000000 xespresso-1.5.5/xespresso/data/pseudo.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    18703 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/dos.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    27084 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/hpxespresso.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    29500 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/input_parameters.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6917 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/neb.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-15 12:38:55.478190 xespresso-1.5.5/xespresso/post/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-08-10 17:05:22.000000 xespresso-1.5.5/xespresso/post/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      666 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/post/bands.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6753 2023-04-25 08:27:31.000000 xespresso-1.5.5/xespresso/post/base.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      669 2023-06-12 10:53:54.000000 xespresso-1.5.5/xespresso/post/dos.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      707 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/post/dynmat.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1069 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/post/hp.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1045 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/post/matdyn.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6331 2023-04-25 08:27:31.000000 xespresso-1.5.5/xespresso/post/nscf.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2083 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/post/ph.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1441 2023-03-23 06:46:49.000000 xespresso-1.5.5/xespresso/post/pp.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      884 2023-06-12 10:53:50.000000 xespresso-1.5.5/xespresso/post/projwfc.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      421 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/post/q2r.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2416 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/scheduler.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6777 2023-01-02 08:23:39.000000 xespresso-1.5.5/xespresso/tools.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    24768 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/uscsd.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-15 12:38:55.482190 xespresso-1.5.5/xespresso/utils/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5558 2023-01-02 08:23:39.000000 xespresso-1.5.5/xespresso/utils/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3298 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/utils/qe_dos_parser.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7189 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/utils/xml_parser.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-15 12:38:55.482190 xespresso-1.5.5/xespresso/workflow/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2020-12-08 21:30:08.000000 xespresso-1.5.5/xespresso/workflow/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7263 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/workflow/base.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    32533 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/workflow/oer.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7086 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/workflow/phonon.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    26942 2023-07-14 13:20:49.000000 xespresso-1.5.5/xespresso/xespresso.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    20839 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/xio.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3352 2023-01-02 07:45:26.000000 xespresso-1.5.5/xespresso/xlog.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-15 12:38:55.478190 xespresso-1.5.5/xespresso.egg-info/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6157 2023-07-15 12:38:55.000000 xespresso-1.5.5/xespresso.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      974 2023-07-15 12:38:55.000000 xespresso-1.5.5/xespresso.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2023-07-15 12:38:55.000000 xespresso-1.5.5/xespresso.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       27 2023-07-15 12:38:55.000000 xespresso-1.5.5/xespresso.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       10 2023-07-15 12:38:55.000000 xespresso-1.5.5/xespresso.egg-info/top_level.txt
```

### Comparing `xespresso-1.5.4/LICENSE` & `xespresso-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/PKG-INFO` & `xespresso-1.5.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xespresso
-Version: 1.5.4
+Version: 1.5.5
 Summary: Quantum ESPRESSO Calculator for Atomic Simulation Environment (ASE).
 Home-page: https://github.com/superstar54/xespresso
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: GPL
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.5
@@ -16,19 +16,21 @@
 [![Unit test](https://github.com/superstar54/xespresso/actions/workflows/unit_test.yaml/badge.svg)](https://github.com/superstar54/xespresso/actions/workflows/unit_test.yaml)
 
 Quantum ESPRESSO Calculator for Atomic Simulation Environment (ASE).
 
 For the introduction of ASE , please visit https://wiki.fysik.dtu.dk/ase/index.html
 
 
-### Functions:
+### Features
+
 * Support all QE packages, including: pw, band, neb, dos, projwfc, pp ...
 * Spin-polarized calculation
 * LD(S)A+U
 * Automatic submit job
+* Automatic check a new calculation required or not
 * Automatic set up "nscf" calculation
 * Read and plot dos, pdos and layer resolved pdos
 * Plot NEB
 
 ### Author
 * Xing Wang  <xingwang1991@gmail.com>
 
@@ -72,15 +74,15 @@
 ```
 
 
 
 
 #### Automatic check a new calculation required or not
 
-Before the calculation, first check the working directory. If the same geometry and parameters are used, try to check the results are available or not. Automatic check input parameters with Quantum Espresso document.
+Before the calculation, it will first check the working directory. If the same geometry and parameters are used, try to check whether the results are available or not. Automatic check input parameters with Quantum Espresso document.
 
 ``` python
 calc = Espresso(label = 'scf/fe')
 ```
 
 #### Show debug information.
 
@@ -165,16 +167,23 @@
             DeltaE = 0.01)
 projwfc.run()
 ```
 <img src="docs/source/_static/images/co-pdos.png" width="500"/>
 
 #### Calculate work function
 ``` python
-calc.post(queue = queue, package = 'pp', plot_num = 11, fileout = 'potential.cube', iflag = 3, output_format=6)
-calc.get_work_function()
+from xespresso.post.pp import EspressoPp
+pp = EspressoPp(calc.directory, prefix = calc.prefix,
+                plot_num = 11,
+                fileout = 'potential.cube',
+                iflag = 3,
+                output_format=6,
+                debug = True,
+                )
+pp.get_work_function()
 ```
 
 #### Restart from previous calculation
 ``` python
 calc.read_results()
 atoms = calc.results['atoms']
 calc.run(atoms = atoms, restart = 1)
```

### Comparing `xespresso-1.5.4/README.md` & `xespresso-1.5.5/xespresso.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,36 @@
+Metadata-Version: 2.1
+Name: xespresso
+Version: 1.5.5
+Summary: Quantum ESPRESSO Calculator for Atomic Simulation Environment (ASE).
+Home-page: https://github.com/superstar54/xespresso
+Author: Xing Wang
+Author-email: xingwang1991@gmail.com
+License: GPL
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.5
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## xespresso
 [![Unit test](https://github.com/superstar54/xespresso/actions/workflows/unit_test.yaml/badge.svg)](https://github.com/superstar54/xespresso/actions/workflows/unit_test.yaml)
 
 Quantum ESPRESSO Calculator for Atomic Simulation Environment (ASE).
 
 For the introduction of ASE , please visit https://wiki.fysik.dtu.dk/ase/index.html
 
 
-### Functions:
+### Features
+
 * Support all QE packages, including: pw, band, neb, dos, projwfc, pp ...
 * Spin-polarized calculation
 * LD(S)A+U
 * Automatic submit job
+* Automatic check a new calculation required or not
 * Automatic set up "nscf" calculation
 * Read and plot dos, pdos and layer resolved pdos
 * Plot NEB
 
 ### Author
 * Xing Wang  <xingwang1991@gmail.com>
 
@@ -58,15 +74,15 @@
 ```
 
 
 
 
 #### Automatic check a new calculation required or not
 
-Before the calculation, first check the working directory. If the same geometry and parameters are used, try to check the results are available or not. Automatic check input parameters with Quantum Espresso document.
+Before the calculation, it will first check the working directory. If the same geometry and parameters are used, try to check whether the results are available or not. Automatic check input parameters with Quantum Espresso document.
 
 ``` python
 calc = Espresso(label = 'scf/fe')
 ```
 
 #### Show debug information.
 
@@ -151,16 +167,23 @@
             DeltaE = 0.01)
 projwfc.run()
 ```
 <img src="docs/source/_static/images/co-pdos.png" width="500"/>
 
 #### Calculate work function
 ``` python
-calc.post(queue = queue, package = 'pp', plot_num = 11, fileout = 'potential.cube', iflag = 3, output_format=6)
-calc.get_work_function()
+from xespresso.post.pp import EspressoPp
+pp = EspressoPp(calc.directory, prefix = calc.prefix,
+                plot_num = 11,
+                fileout = 'potential.cube',
+                iflag = 3,
+                output_format=6,
+                debug = True,
+                )
+pp.get_work_function()
 ```
 
 #### Restart from previous calculation
 ``` python
 calc.read_results()
 atoms = calc.results['atoms']
 calc.run(atoms = atoms, restart = 1)
```

### Comparing `xespresso-1.5.4/setup.py` & `xespresso-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="xespresso",
-    version="1.5.4",
+    version="1.5.5",
     description="Quantum ESPRESSO Calculator for Atomic Simulation Environment (ASE).",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/superstar54/xespresso",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="GPL",
```

### Comparing `xespresso-1.5.4/xespresso/cohp.py` & `xespresso-1.5.5/xespresso/cohp.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/data/pseudo.py` & `xespresso-1.5.5/xespresso/data/pseudo.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/dos.py` & `xespresso-1.5.5/xespresso/dos.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/hpxespresso.py` & `xespresso-1.5.5/xespresso/hpxespresso.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/input_parameters.py` & `xespresso-1.5.5/xespresso/input_parameters.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/neb.py` & `xespresso-1.5.5/xespresso/neb.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/post/bands.py` & `xespresso-1.5.5/xespresso/post/bands.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/post/base.py` & `xespresso-1.5.5/xespresso/post/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 
 class PostCalculation:
 
     package = "dos"
     package_parameters = {}
 
     def __init__(
-        self, parent_directory, prefix, queue=False, parallel="", **kwargs
+        self, parent_directory, prefix, queue=False, parallel="", debug=False, **kwargs
     ) -> None:
+        if debug:
+            logger.setLevel(debug)
         self.parent_directory = parent_directory
         self.prefix = prefix
         self.queue = queue
         self.parallel = parallel
         self.parameters = kwargs
         self.directory = os.path.join(self.parent_directory, "%s/" % self.package)
         self.set_label(self.directory, self.prefix)
         self.parameters["prefix"] = self.prefix
         self.parameters["outdir"] = "../"
         self.state_info = None
 
     def set_label(self, label, prefix):
-        """
-        set directory and prefix from label
-        """
+        """Set directory and prefix from label"""
         self.directory = label
         if not prefix:
             self.prefix = os.path.split(label)[1]
         else:
             self.prefix = prefix
         if not os.path.exists(self.directory):
             os.makedirs(self.directory)
@@ -42,17 +42,15 @@
         self.asei_temp = os.path.join(self.directory, ".%s.asei_temp" % self.prefix)
         self.post_asei = os.path.join(self.directory, "%s.post_asei" % self.prefix)
         self.save_directory = os.path.join(self.directory, "%s.save" % self.prefix)
         logger.debug("Directory: %s" % (self.directory))
         logger.debug("Prefix: %s" % (self.prefix))
 
     def run(self):
-        """
-        todo:
-        """
+        """todo:"""
         from xespresso.scheduler import set_queue
 
         print("{0:=^60}".format(self.package))
         if self.check_state() == 0:
             return
         self.write_input()
         set_queue(self, package=self.package, parallel=self.parallel, queue=self.queue)
@@ -96,19 +94,20 @@
         self.write_package_input()
         write_espresso_asei(self.post_asei, self.state_info, self.parameters)
 
     def write_package_input(self):
         filename = os.path.join(self.directory, "%s.%si" % (self.prefix, self.package))
         with open(filename, "w") as f:
             for section, parameters in self.package_parameters.items():
-                # logger.debug(section)
+                logger.debug(f"section: {section}")
                 if section != "LINE":
                     f.write("&%s\n" % section)
                     for key, value in self.parameters.items():
                         if key in parameters:
+                            logger.debug(f"key: {key}")
                             if isinstance(value, dict):
                                 for subkey, subvalue in value.items():
                                     if isinstance(subvalue, str):
                                         f.write(
                                             '  %s(%s) = "%s", \n'
                                             % (key, subkey, subvalue)
                                         )
```

### Comparing `xespresso-1.5.4/xespresso/post/dos.py` & `xespresso-1.5.5/xespresso/post/dos.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/post/dynmat.py` & `xespresso-1.5.5/xespresso/post/dynmat.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/post/hp.py` & `xespresso-1.5.5/xespresso/post/hp.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/post/matdyn.py` & `xespresso-1.5.5/xespresso/post/matdyn.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/post/nscf.py` & `xespresso-1.5.5/xespresso/post/nscf.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,18 +88,30 @@
         write_espresso_asei(self.asei, self.state_info, self.parameters)
         logger.debug("Write input successfully")
 
     @property
     def state_info(self):
         from xespresso.utils import get_hash
 
-        chargeFile = os.path.join(
+        # get state information from charge-density file
+        # it could has two format ".dat", "hdf5"
+        # if charge-density.hdf5 does not exist, use charge-density.dat
+        charge_dat = os.path.join(
             self.scf_directory, "%s.save/charge-density.dat" % self.prefix
         )
-        state_info = get_hash(chargeFile)
+        charge_hdf5 = os.path.join(
+            self.scf_directory, "%s.save/charge-density.hdf5" % self.prefix
+        )
+        if os.path.isfile(charge_dat):
+            state_info = get_hash(charge_dat)
+        elif os.path.isfile(charge_hdf5):
+            state_info = get_hash(charge_hdf5)
+        else:
+            raise ValueError("No charge-density file found!")
+
         return state_info
 
     def check_state(
         self,
     ):
         # read information of the charge-density file
         self.state_parameters = self.parameters
```

### Comparing `xespresso-1.5.4/xespresso/post/ph.py` & `xespresso-1.5.5/xespresso/post/ph.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/post/pp.py` & `xespresso-1.5.5/xespresso/post/pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from xespresso.post.base import PostCalculation
 
 
 class EspressoPp(PostCalculation):
 
     package = "pp"
-    state_parameters = {
+    package_parameters = {
         "INPUTPP": [
             "prefix",
             "outdir",
             "filplot",
             "plot_num",
             "spin_component",
             "spin_component",
```

### Comparing `xespresso-1.5.4/xespresso/post/projwfc.py` & `xespresso-1.5.5/xespresso/post/projwfc.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/scheduler.py` & `xespresso-1.5.5/xespresso/scheduler.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/tools.py` & `xespresso-1.5.5/xespresso/tools.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/uscsd.py` & `xespresso-1.5.5/xespresso/uscsd.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/utils/qe_dos_parser.py` & `xespresso-1.5.5/xespresso/utils/qe_dos_parser.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/utils/xml_parser.py` & `xespresso-1.5.5/xespresso/utils/xml_parser.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/workflow/base.py` & `xespresso-1.5.5/xespresso/workflow/base.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/workflow/oer.py` & `xespresso-1.5.5/xespresso/workflow/oer.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/workflow/phonon.py` & `xespresso-1.5.5/xespresso/workflow/phonon.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/xespresso.py` & `xespresso-1.5.5/xespresso/xespresso.py`

 * *Files 19% similar despite different names*

```diff
@@ -58,14 +58,45 @@
     'Please try running Quantum Espresso with "high" verbosity.'
 )
 
 _blocked_keywords = {}
 
 
 class Espresso(FileIOCalculator):
+    """
+    Accepts all the options for pw.x as given in the QE docs, plus some
+    additional options:
+
+    input_data, pseudopotentials, kspacing, kpts, koffset
+        Please have a look at Espresso module in ASE.
+        https://wiki.fysik.dtu.dk/ase/ase/calculators/espresso.html
+    queue: dict
+        A dictionary with parameters for job submission, e.g.
+
+        >>> queue = {'nodes': 4, 'ntasks-per-node': 20,
+        >>>         'account': 'xxx', 'partition': 'normal',
+        >>>         'time': '23:59:00'}
+    package: str
+        Choose the quantum espresso package: pw, dos, projwfc, band, pp, ph, ..
+        For NEB calculation, please use neb.NEBEspresso module.
+        Calculaiton use phonon is not implemented yet.
+    parallel: str
+        A str which control the parallelization parameters: -nimage, -npools,
+        -nband, -ntg, -ndiag or -northo (shorthands, respectively:
+        -ni, -nk, -nb, -nt, -nd).
+
+    Examples:
+
+    1. Perform a regular self-consistent calculation:
+
+    >>> calc = Espresso(input_data=input_data, ...)
+    >>> atoms.set_calculator(calc)
+    >>> atoms.get_potential_energy()
+    """
+
     implemented_properties = ["energy", "forces", "stress", "magmoms", "time"]
     command = "PACKAGE.x  PARALLEL  -in  PREFIX.PACKAGEi  >  PREFIX.PACKAGEo"
     discard_results_on_any_change = False
 
     def __init__(
         self,
         label="xespresso",
@@ -74,46 +105,15 @@
         package="pw",
         parallel="",
         queue=None,
         debug=False,
         pseudo_group=None,
         **kwargs
     ):
-        """
-        Accepts all the options for pw.x as given in the QE docs, plus some
-        additional options:
 
-        input_data, pseudopotentials, kspacing, kpts, koffset
-            Please have a look at Espresso module in ASE
-        queue: dict
-            A dictionary with parameters for job submission, e.g.
-             queue = {'nodes': 4, 'ntasks-per-node': 20,
-                      'account': 'xxx', 'partition': 'normal',
-                      'time': '23:59:00'}
-        package: str
-            Choose the quantum espresso package: pw, dos, projwfc, band, pp, ph, ..
-            For NEB calculation, please use neb.NEBEspresso module.
-            Calculaiton use phonon is not implemented yet.
-        parallel: str
-            A str which control the parallelization parameters: -nimage, -npools,
-            -nband, -ntg, -ndiag or -northo (shorthands, respectively:
-            -ni, -nk, -nb, -nt, -nd).
-
-        General working procedure is as follows:
-            1. Perform a regular self-consistent calculation:
-              >>> calc = Espresso(input_data=input_data, ...)
-              >>> atoms.set_calculator(calc)
-              >>> atoms.get_potential_energy()
-            2. post calculation can be made as follows:
-              >>> calc.post('package' = 'dos', **kwargs)
-              >>> calc.post('package' = 'pp', **kwargs)
-            3. non-self-consistent calculation can be made as follows:
-              >>> calc.nscf(calculation = 'nscf', kpts=(4, 4, 4))
-              >>> calc.nscf_calculate()
-        """
         print("{0:=^60}".format(package))
         if debug:
             logger.setLevel(debug)
         self.set_label(label, prefix)
         self.scf_directory = None
         self.scf_parameters = None
         self.scf_results = None
@@ -134,30 +134,28 @@
         self.parallel = parallel
         self.package = package
         self.parallel = parallel
         self.debug = debug
 
         # self.discard_results_on_any_change = False
 
-    def find_pseudopotentials(self, pseudo_group):
-        """_summary_
+    def find_pseudopotentials(self, pseudo_group="SSSP_1.1.2_PBE_efficiency"):
+        """Get pseudo potential by family name.
 
         Args:
-            pseudo_group (_type_): _description_
+            pseudo_group (str): name of the pseudo family.
         """
         elements = set(self.atoms.get_chemical_symbols())
         pseudopotentials = {}
         for ele in elements:
             pseudopotentials[ele] = pseudo_gropus[pseudo_group][ele.upper()]
         return pseudopotentials
 
     def set_label(self, label, prefix):
-        """
-        set directory and prefix from label
-        """
+        """Set directory and prefix from label"""
         self.directory = label
         if not prefix:
             self.prefix = os.path.split(label)[1]
         else:
             self.prefix = prefix
         if not os.path.exists(self.directory):
             os.makedirs(self.directory)
@@ -167,15 +165,15 @@
         self.asei = os.path.join(self.directory, "%s.asei" % self.prefix)
         self.asei_temp = os.path.join(self.directory, ".%s.asei_temp" % self.prefix)
         self.save_directory = os.path.join(self.directory, "%s.save" % self.prefix)
         logger.debug("Directory: %s" % (self.directory))
         logger.debug("Prefix: %s" % (self.prefix))
 
     def check_pseudopotentials(self, pseudopotentials):
-        """ """
+        """check pseudopotentials"""
         # pseudopotentials
         if "species" not in self.atoms.arrays:
             all_species = set(self.atoms.get_chemical_symbols())
         else:
             all_species = set(self.atoms.arrays["species"])
         new_pseudopotentials = {}
         for species in all_species:
@@ -229,16 +227,17 @@
                 "Directory %s is not a espresso folder, start a new calculation:"
                 % (label)
             )
 
     def set(self, **kwargs):
         """ """
         from xespresso.input_parameters import restart_ignore
+        from xespresso.utils import compare_parameters
 
-        self.changed_parameters, self.igonre_parameters = self.compare_parameters(
+        self.changed_parameters, self.igonre_parameters = compare_parameters(
             self.restart_parameters, self.ase_parameters, ignore=restart_ignore["PW"]
         )
         self.parameters = kwargs
         if self.discard_results_on_any_change and self.changed_parameters:
             self.reset()
         return self.changed_parameters
 
@@ -277,103 +276,16 @@
         logger.debug("Same geometry and parameters, use previous results.")
         converged, meg = self.read_convergence()
         if converged > 0:
             logger.debug("Not converged: %s" % meg)
             return True
         return False
 
-    def compare_parameters(self, para1, para2, ignore=[]):
-        """ """
-        from xespresso.input_parameters import (
-            qe_namespace,
-            default_parameters,
-            restart_ignore,
-        )
-
-        changed_parameters = []
-        igonre_parameters = []
-        if not para1:
-            changed_parameters = ["all"]
-            return changed_parameters, igonre_parameters
-        default_parameters = default_parameters["PW"]
-        # pseudopotentials
-        key = "pseudopotentials"
-        try:
-            for species, value in para1[key].items():
-                if value != para2[key][species]:
-                    changed_parameters.append(key)
-                    continue
-        except:
-            changed_parameters.append(key)
-        # kpts
-        key = "kpts"
-        try:
-            if para1[key] != para2[key]:
-                changed_parameters.append(key)
-        except:
-            changed_parameters.append(key)
-        # input_data
-        for section, paras in para1["input_data"].items():
-            if section == "INPUT_NTYP":
-                changed_parameters1, igonre_parameters1 = self.compare_dict(
-                    para1["input_data"][section],
-                    para2["input_data"][section],
-                    restart_ignore["PW"],
-                )
-            else:
-                changed_parameters1, igonre_parameters1 = self.compare_dict(
-                    para1["input_data"][section],
-                    para2["input_data"][section],
-                    restart_ignore["PW"],
-                    default=default_parameters[section],
-                )
-            changed_parameters.extend(changed_parameters1)
-            igonre_parameters.extend(igonre_parameters1)
-        return changed_parameters, igonre_parameters
-
-    def compare_dict(self, dict1, dict2, ignore=[], default=None):
-        igonre_parameters = []
-        changed_parameters = []
-        keys = set(list(dict1.keys()) + list(dict2.keys()))
-        print
-        for key in keys:
-            if key in ignore:
-                igonre_parameters.append(key)
-            elif key not in dict1:
-                changed_parameters.append(key)
-            elif key not in dict2:
-                if default and self.compare_value(dict1[key], default[key]):
-                    continue
-                changed_parameters.append(key)
-            elif not self.compare_value(dict1[key], dict2[key]):
-                changed_parameters.append(key)
-        return changed_parameters, igonre_parameters
-
-    def compare_value(self, v1, v2, tol=1e-5):
-        """ """
-        if isinstance(v1, str):
-            if v1.upper() != v2.upper():
-                return False
-        elif isinstance(v1, dict):
-            changed_parameters, igonre_parameters = self.compare_dict(v1, v2)
-            if changed_parameters:
-                return False
-            for key, value in v1.items():
-                if not self.compare_value(value, v2[key]):
-                    return False
-        elif isinstance(v1, bool):
-            if v1 != v2:
-                return False
-        else:
-            if abs(v1 - v2) > tol:
-                return False
-        return True
-
     def read_results(self):
-        """
+        """Read PW results.
         get atomic species
         """
         pwo = os.path.join(self.directory, "%s.pwo" % self.prefix)
         pwi = os.path.join(self.directory, "%s.pwi" % self.prefix)
         convergence, meg = self.read_convergence()
         if convergence != 0:
             logger.debug("Not converged. %s" % (meg))
@@ -395,14 +307,15 @@
             self.results["atoms"] = output
             self.efermi = self.get_fermi_level()
             # self.nspins = self.get_number_of_spins()
             logger.debug("Read result successfully!")
         except Exception as e:
             logger.debug("Read output: %s, failed! %s" % (pwo, e))
         self.results["convergence"] = convergence
+        self.results["label"] = self.label
         # logger.debug('Read result failed!')
         # pwos = [file for file in os.listdir(self.directory) if pwo in file]
         # output = None
         # for pwo in pwos:
         # atomic_species = None
         # pwo = os.path.join(self.directory, pwo)
         # atomic_species = get_atomic_species(pwo)
@@ -463,23 +376,22 @@
             logger.debug("Read xml file failed.")
             return None, {}
         return atoms, xml_input
 
     def read_convergence(self):
         """
         Read the status of the calculation.
-        {
+        exit code:
         '0': 'Done',
         '-1': ' manual cancelled',
         '1': 'Maximum CPU time exceeded', convergence NOT achieved after n iterations
              Then, change the parameter: 1) mixing_beta or 2) degauss
         '2': 'manual restart', 'Pending or not submit',
         '3': 'other errors',
         '4': 'unknow error',
-        }
         """
         # read the error file from queue
         # if self.queue:
         #     errfile = self.label + '.err'
         #     if not os.path.exists(errfile):
         #         logger.debug('%s not exists'%errfile)
         #         # return 2, 'Pending or not submit'
@@ -657,27 +569,31 @@
         ax.set_xlabel("Frequency (cm^-1)")
         ax.set_ylabel("DOS (a.u.)")
         if output is not None:
             plt.savefig("%s" % output)
         return ax
 
     def get_work_function(
-        self, ax=None, inpfile="potential.cube", output=None, shift=False
+        self,
+        ax=None,
+        inpfile="potential.cube",
+        output=None,
+        shift=False,
     ):
         import matplotlib.pyplot as plt
         from ase.io.cube import read_cube_data
         from ase.units import create_units
 
         if ax is None:
             import matplotlib.pyplot as plt
 
             ax = plt.gca()
         units = create_units("2006")
         #
-        filename = os.path.join(self.directory, inpfile)
+        filename = os.path.join(self.directory, "pp", inpfile)
         data, atoms = read_cube_data(filename)
         data = data * units["Ry"]
         ef = self.get_fermi_level()
         # x, y, z, lp = calc.get_local_potential()
         nx, ny, nz = data.shape
         axy = np.array([np.average(data[:, :, z]) for z in range(nz)])
         # setup the x-axis in realspace
@@ -696,25 +612,28 @@
         # plt.show()
         atoms = self.results["atoms"]
         pos = max(atoms.positions[:, 2] + 3)
         ind = (xaxis > pos) & (xaxis < pos + 3)
         wf = np.average(axy[ind]) - ef
         print("min: %s, max: %s" % (pos, pos + 3))
         print("The workfunction is {0:1.2f} eV".format(wf))
+        return wf
 
     def get_bader_charge(self, inpfile=None):
         """ """
         from ase.io.bader import attach_charges
 
         if not inpfile:
             inpfile = "%s.cube" % self.prefix
         command = "bader %s" % inpfile
         print(command)
         try:
-            proc = subprocess.Popen(command, shell=True, cwd=self.directory)
+            proc = subprocess.Popen(
+                command, shell=True, cwd=os.path.join(self.directory, "pp")
+            )
         except OSError as err:
             msg = 'Failed to execute "{}"'.format(command)
             raise EnvironmentError(msg) from err
         acf = os.path.join(self.directory, "ACF.dat")
         attach_charges(self.results["atoms"], acf)
 
     def read_time(
```

### Comparing `xespresso-1.5.4/xespresso/xio.py` & `xespresso-1.5.5/xespresso/xio.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso/xlog.py` & `xespresso-1.5.5/xespresso/xlog.py`

 * *Files identical despite different names*

### Comparing `xespresso-1.5.4/xespresso.egg-info/PKG-INFO` & `xespresso-1.5.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-Metadata-Version: 2.1
-Name: xespresso
-Version: 1.5.4
-Summary: Quantum ESPRESSO Calculator for Atomic Simulation Environment (ASE).
-Home-page: https://github.com/superstar54/xespresso
-Author: Xing Wang
-Author-email: xingwang1991@gmail.com
-License: GPL
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.5
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## xespresso
 [![Unit test](https://github.com/superstar54/xespresso/actions/workflows/unit_test.yaml/badge.svg)](https://github.com/superstar54/xespresso/actions/workflows/unit_test.yaml)
 
 Quantum ESPRESSO Calculator for Atomic Simulation Environment (ASE).
 
 For the introduction of ASE , please visit https://wiki.fysik.dtu.dk/ase/index.html
 
 
-### Functions:
+### Features
+
 * Support all QE packages, including: pw, band, neb, dos, projwfc, pp ...
 * Spin-polarized calculation
 * LD(S)A+U
 * Automatic submit job
+* Automatic check a new calculation required or not
 * Automatic set up "nscf" calculation
 * Read and plot dos, pdos and layer resolved pdos
 * Plot NEB
 
 ### Author
 * Xing Wang  <xingwang1991@gmail.com>
 
@@ -72,15 +60,15 @@
 ```
 
 
 
 
 #### Automatic check a new calculation required or not
 
-Before the calculation, first check the working directory. If the same geometry and parameters are used, try to check the results are available or not. Automatic check input parameters with Quantum Espresso document.
+Before the calculation, it will first check the working directory. If the same geometry and parameters are used, try to check whether the results are available or not. Automatic check input parameters with Quantum Espresso document.
 
 ``` python
 calc = Espresso(label = 'scf/fe')
 ```
 
 #### Show debug information.
 
@@ -165,16 +153,23 @@
             DeltaE = 0.01)
 projwfc.run()
 ```
 <img src="docs/source/_static/images/co-pdos.png" width="500"/>
 
 #### Calculate work function
 ``` python
-calc.post(queue = queue, package = 'pp', plot_num = 11, fileout = 'potential.cube', iflag = 3, output_format=6)
-calc.get_work_function()
+from xespresso.post.pp import EspressoPp
+pp = EspressoPp(calc.directory, prefix = calc.prefix,
+                plot_num = 11,
+                fileout = 'potential.cube',
+                iflag = 3,
+                output_format=6,
+                debug = True,
+                )
+pp.get_work_function()
 ```
 
 #### Restart from previous calculation
 ``` python
 calc.read_results()
 atoms = calc.results['atoms']
 calc.run(atoms = atoms, restart = 1)
```

### Comparing `xespresso-1.5.4/xespresso.egg-info/SOURCES.txt` & `xespresso-1.5.5/xespresso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

