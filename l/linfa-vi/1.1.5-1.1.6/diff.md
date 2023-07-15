# Comparing `tmp/linfa_vi-1.1.5.tar.gz` & `tmp/linfa_vi-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.1.5.tar", last modified: Mon Jul 10 15:27:59 2023, max compression
+gzip compressed data, was "linfa_vi-1.1.6.tar", last modified: Sat Jul 15 04:38:43 2023, max compression
```

## Comparing `linfa_vi-1.1.5.tar` & `linfa_vi-1.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/plot_res.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/plot_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/setup.py
```

### Comparing `linfa_vi-1.1.5/LICENSE` & `linfa_vi-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.5/PKG-INFO` & `linfa_vi-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -73,15 +73,15 @@
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
-* `rcr_nofas_adaann_example` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
+* `rcr_nofas_adaann` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
 
 At regular intervals set by the parameter `experiment.save_interval` LINFA writes a few results files. The sub-string `NAME` refers to the experiment name specified in the `experiment.name` variable, and `IT` indicates the iteration at which the file is written. The results files are
 
 * `log.txt` contains the log profile information, i.e.
   * Iteration number.
   * Annealing temperature at each iteration.
   * Loss function at each iteration.
@@ -91,15 +91,15 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-python linfa.plot_res -n NAME -i IT -f FOLDER
+python -m linfa.plot_res -n NAME -i IT -f FOLDER
 ```
 where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest, while `FOLDER` is the name of the folder with the results of the inference task are kept.
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
```

### Comparing `linfa_vi-1.1.5/README.md` & `linfa_vi-1.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
-* `rcr_nofas_adaann_example` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
+* `rcr_nofas_adaann` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
 
 At regular intervals set by the parameter `experiment.save_interval` LINFA writes a few results files. The sub-string `NAME` refers to the experiment name specified in the `experiment.name` variable, and `IT` indicates the iteration at which the file is written. The results files are
 
 * `log.txt` contains the log profile information, i.e.
   * Iteration number.
   * Annealing temperature at each iteration.
   * Loss function at each iteration.
@@ -69,15 +69,15 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-python linfa.plot_res -n NAME -i IT -f FOLDER
+python -m linfa.plot_res -n NAME -i IT -f FOLDER
 ```
 where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest, while `FOLDER` is the name of the folder with the results of the inference task are kept.
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
```

### Comparing `linfa_vi-1.1.5/linfa/maf.py` & `linfa_vi-1.1.6/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.5/linfa/nofas.py` & `linfa_vi-1.1.6/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.5/linfa/plot_res.py` & `linfa_vi-1.1.6/linfa/plot_res.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
   parser = argparse.ArgumentParser(description='.')
 
   # folder name
   parser.add_argument('-f', '--folder',
                       action=None,
                       # nargs='+',
                       const=None,
-                      default='./tests/results/',
+                      default='./',
                       type=str,
                       required=False,
                       help='Folder with experiment results',
                       metavar='',
                       dest='folder_name')
 
 
@@ -128,28 +128,30 @@
   out_info    = args.exp_name + '_' + str(args.step_num)
 
   # Plot loss profile
   if(os.path.isfile(log_file)):
     print('Plotting log...')
     plot_log(log_file,out_dir)
   else:
-    print('Log file not found...')
+    print('Log file not found: '+log_file)
 
   # Plot 2D slice of posterior samples
   if(os.path.isfile(param_file) and os.path.isfile(LL_file)):
     tot_params  = np.loadtxt(param_file).shape[1]
     print('Plotting posterior samples...')
     for loopA in range(tot_params):
       for loopB in range(loopA+1, tot_params):
         plot_params(param_file,LL_file,loopA,loopB,out_dir,out_info)
   else:
-    print('File with posterior samples not found...')
+    print('File with posterior samples not found: '+param_file)
+    print('File with log-density not found: '+LL_file)
 
   # Plot 2D slice of outputs and observations
   if(os.path.isfile(output_file) and os.path.isfile(obs_file)):
     tot_outputs = np.loadtxt(output_file).shape[1]
     print('Plotting posterior predictive samples...')
     for loopA in range(tot_outputs):
       for loopB in range(loopA+1, tot_outputs):
         plot_outputs(output_file,obs_file,loopA,loopB,out_dir,out_info)
   else:
-    print('File with posterior predictive samples not found...')
+    print('File with posterior predictive samples not found: '+output_file)
+    print('File with observations not found: '+obs_file)
```

### Comparing `linfa_vi-1.1.5/linfa/run_experiment.py` & `linfa_vi-1.1.6/linfa/run_experiment.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.5/linfa/transform.py` & `linfa_vi-1.1.6/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.5/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.1.6/linfa_vi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -73,15 +73,15 @@
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
-* `rcr_nofas_adaann_example` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
+* `rcr_nofas_adaann` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
 
 At regular intervals set by the parameter `experiment.save_interval` LINFA writes a few results files. The sub-string `NAME` refers to the experiment name specified in the `experiment.name` variable, and `IT` indicates the iteration at which the file is written. The results files are
 
 * `log.txt` contains the log profile information, i.e.
   * Iteration number.
   * Annealing temperature at each iteration.
   * Loss function at each iteration.
@@ -91,15 +91,15 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-python linfa.plot_res -n NAME -i IT -f FOLDER
+python -m linfa.plot_res -n NAME -i IT -f FOLDER
 ```
 where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest, while `FOLDER` is the name of the folder with the results of the inference task are kept.
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
```

### Comparing `linfa_vi-1.1.5/pyproject.toml` & `linfa_vi-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.1.5"
+version = "1.1.6"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

