# Comparing `tmp/eznet_torch-0.0.0.tar.gz` & `tmp/eznet_torch-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eznet_torch-0.0.0.tar", last modified: Fri Jan 20 17:40:43 2023, max compression
+gzip compressed data, was "eznet_torch-0.0.1.tar", last modified: Sat Jul 15 18:03:52 2023, max compression
```

## Comparing `eznet_torch-0.0.0.tar` & `eznet_torch-0.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-01-20 17:40:43.870803 eznet_torch-0.0.0/
--rw-rw-rw-   0        0        0     1186 2023-01-20 16:20:52.000000 eznet_torch-0.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0    12593 2023-01-20 17:40:43.870803 eznet_torch-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    11604 2023-01-20 17:31:07.000000 eznet_torch-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-20 17:40:43.853129 eznet_torch-0.0.0/eznet_torch/
--rw-rw-rw-   0        0        0       40 2023-01-19 17:38:59.000000 eznet_torch-0.0.0/eznet_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 17:40:43.870068 eznet_torch-0.0.0/eznet_torch/models/
--rw-rw-rw-   0        0        0      435 2023-01-19 20:24:54.000000 eznet_torch-0.0.0/eznet_torch/models/__init__.py
--rw-rw-rw-   0        0        0     9546 2023-01-19 20:27:16.000000 eznet_torch-0.0.0/eznet_torch/models/ann.py
--rw-rw-rw-   0        0        0    14022 2023-01-19 20:27:41.000000 eznet_torch-0.0.0/eznet_torch/models/conv_block.py
--rw-rw-rw-   0        0        0    20949 2023-01-19 20:48:06.000000 eznet_torch-0.0.0/eznet_torch/models/conv_network.py
--rw-rw-rw-   0        0        0     3053 2023-01-19 20:28:57.000000 eznet_torch-0.0.0/eznet_torch/models/dense_block.py
--rw-rw-rw-   0        0        0     3579 2023-01-19 20:40:29.000000 eznet_torch-0.0.0/eznet_torch/models/language_model.py
--rw-rw-rw-   0        0        0     5216 2023-01-19 20:38:19.000000 eznet_torch-0.0.0/eznet_torch/models/pytorch_smart_module.py
--rw-rw-rw-   0        0        0    16028 2023-01-19 20:39:19.000000 eznet_torch-0.0.0/eznet_torch/models/recurrent_network.py
--rw-rw-rw-   0        0        0     2211 2023-01-19 20:50:01.000000 eznet_torch-0.0.0/eznet_torch/test.py
--rw-rw-rw-   0        0        0    38714 2023-01-20 17:06:59.000000 eznet_torch-0.0.0/eznet_torch/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-20 17:40:43.865089 eznet_torch-0.0.0/eznet_torch.egg-info/
--rw-rw-rw-   0        0        0    12593 2023-01-20 17:40:43.000000 eznet_torch-0.0.0/eznet_torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-01-20 17:40:43.000000 eznet_torch-0.0.0/eznet_torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-20 17:40:43.000000 eznet_torch-0.0.0/eznet_torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-01-20 17:40:43.000000 eznet_torch-0.0.0/eznet_torch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-01-20 17:40:43.000000 eznet_torch-0.0.0/eznet_torch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-01-20 17:40:43.874313 eznet_torch-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1738 2023-01-20 17:38:29.000000 eznet_torch-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:03:52.186838 eznet_torch-0.0.1/
+-rw-rw-rw-   0        0        0     1186 2023-01-20 16:20:52.000000 eznet_torch-0.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    12644 2023-07-15 18:03:52.186838 eznet_torch-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11646 2023-07-15 18:02:37.000000 eznet_torch-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 18:03:52.171668 eznet_torch-0.0.1/eznet_torch/
+-rw-rw-rw-   0        0        0       40 2023-01-19 17:38:59.000000 eznet_torch-0.0.1/eznet_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:03:52.186337 eznet_torch-0.0.1/eznet_torch/models/
+-rw-rw-rw-   0        0        0      435 2023-01-19 20:24:54.000000 eznet_torch-0.0.1/eznet_torch/models/__init__.py
+-rw-rw-rw-   0        0        0     9546 2023-01-19 20:27:16.000000 eznet_torch-0.0.1/eznet_torch/models/ann.py
+-rw-rw-rw-   0        0        0    14022 2023-01-19 20:27:41.000000 eznet_torch-0.0.1/eznet_torch/models/conv_block.py
+-rw-rw-rw-   0        0        0    20949 2023-01-19 20:48:06.000000 eznet_torch-0.0.1/eznet_torch/models/conv_network.py
+-rw-rw-rw-   0        0        0     3053 2023-01-19 20:28:57.000000 eznet_torch-0.0.1/eznet_torch/models/dense_block.py
+-rw-rw-rw-   0        0        0     3579 2023-01-19 20:40:29.000000 eznet_torch-0.0.1/eznet_torch/models/language_model.py
+-rw-rw-rw-   0        0        0     5216 2023-01-19 20:38:19.000000 eznet_torch-0.0.1/eznet_torch/models/pytorch_smart_module.py
+-rw-rw-rw-   0        0        0    16028 2023-01-19 20:39:19.000000 eznet_torch-0.0.1/eznet_torch/models/recurrent_network.py
+-rw-rw-rw-   0        0        0     2211 2023-01-19 20:50:01.000000 eznet_torch-0.0.1/eznet_torch/test.py
+-rw-rw-rw-   0        0        0    38714 2023-01-20 17:06:59.000000 eznet_torch-0.0.1/eznet_torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:03:52.182351 eznet_torch-0.0.1/eznet_torch.egg-info/
+-rw-rw-rw-   0        0        0    12644 2023-07-15 18:03:52.000000 eznet_torch-0.0.1/eznet_torch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-07-15 18:03:52.000000 eznet_torch-0.0.1/eznet_torch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 18:03:52.000000 eznet_torch-0.0.1/eznet_torch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-15 18:03:52.000000 eznet_torch-0.0.1/eznet_torch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-15 18:03:52.000000 eznet_torch-0.0.1/eznet_torch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-15 18:03:52.190336 eznet_torch-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1740 2023-07-15 18:02:09.000000 eznet_torch-0.0.1/setup.py
```

### Comparing `eznet_torch-0.0.0/LICENSE.txt` & `eznet_torch-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/PKG-INFO` & `eznet_torch-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: eznet_torch
-Version: 0.0.0
-Summary: Easily build PyTorch models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Conv blocks, etc.
+Version: 0.0.1
+Summary: Easily build PyTorch models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc.
 Home-page: https://github.com/pniaz20/eznet_torch
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: torch,pytorch,deep learning,neural network
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -21,24 +21,24 @@
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ezNet-torch
 
 PyTorch implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
-This implementation is for PyTorch. See (where?) for identical Keras (TensorFlow) implementation.
+This implementation is for PyTorch. See [here](https://github.com/pniaz20/eznet_keras) for an identical Keras (TensorFlow) implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.0  
-Last Update: Jan 20, 2023
+Version: 0.0.1  
+Last Update: July 15, 2023
 
 Install with:
 
 ```bash
-pip install eznet_torch
+pip install eznet-torch
 ```
 
 -----------------------------------
 
 ## 1- Intro
 
 You can build, train and evaluate all manner of PyTorch models using the utilities in this package, similar to torch-lightning, but with additional functionality, and easier.
```

### Comparing `eznet_torch-0.0.0/README.md` & `eznet_torch-0.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # ezNet-torch
 
 PyTorch implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
-This implementation is for PyTorch. See (where?) for identical Keras (TensorFlow) implementation.
+This implementation is for PyTorch. See [here](https://github.com/pniaz20/eznet_keras) for an identical Keras (TensorFlow) implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.0  
-Last Update: Jan 20, 2023
+Version: 0.0.1  
+Last Update: July 15, 2023
 
 Install with:
 
 ```bash
-pip install eznet_torch
+pip install eznet-torch
 ```
 
 -----------------------------------
 
 ## 1- Intro
 
 You can build, train and evaluate all manner of PyTorch models using the utilities in this package, similar to torch-lightning, but with additional functionality, and easier.
```

### Comparing `eznet_torch-0.0.0/eznet_torch/models/ann.py` & `eznet_torch-0.0.1/eznet_torch/models/ann.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch/models/conv_block.py` & `eznet_torch-0.0.1/eznet_torch/models/conv_block.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch/models/conv_network.py` & `eznet_torch-0.0.1/eznet_torch/models/conv_network.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch/models/dense_block.py` & `eznet_torch-0.0.1/eznet_torch/models/dense_block.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch/models/language_model.py` & `eznet_torch-0.0.1/eznet_torch/models/language_model.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch/models/pytorch_smart_module.py` & `eznet_torch-0.0.1/eznet_torch/models/pytorch_smart_module.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch/models/recurrent_network.py` & `eznet_torch-0.0.1/eznet_torch/models/recurrent_network.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch/test.py` & `eznet_torch-0.0.1/eznet_torch/test.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch/utils.py` & `eznet_torch-0.0.1/eznet_torch/utils.py`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/eznet_torch.egg-info/PKG-INFO` & `eznet_torch-0.0.1/eznet_torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: eznet-torch
-Version: 0.0.0
-Summary: Easily build PyTorch models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Conv blocks, etc.
+Version: 0.0.1
+Summary: Easily build PyTorch models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc.
 Home-page: https://github.com/pniaz20/eznet_torch
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: torch,pytorch,deep learning,neural network
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -21,24 +21,24 @@
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ezNet-torch
 
 PyTorch implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
-This implementation is for PyTorch. See (where?) for identical Keras (TensorFlow) implementation.
+This implementation is for PyTorch. See [here](https://github.com/pniaz20/eznet_keras) for an identical Keras (TensorFlow) implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.0  
-Last Update: Jan 20, 2023
+Version: 0.0.1  
+Last Update: July 15, 2023
 
 Install with:
 
 ```bash
-pip install eznet_torch
+pip install eznet-torch
 ```
 
 -----------------------------------
 
 ## 1- Intro
 
 You can build, train and evaluate all manner of PyTorch models using the utilities in this package, similar to torch-lightning, but with additional functionality, and easier.
```

### Comparing `eznet_torch-0.0.0/eznet_torch.egg-info/SOURCES.txt` & `eznet_torch-0.0.1/eznet_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eznet_torch-0.0.0/setup.py` & `eznet_torch-0.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.0.0' 
-DESCRIPTION = "Easily build PyTorch models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Conv blocks, etc."
+VERSION = '0.0.1' 
+DESCRIPTION = "Easily build PyTorch models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc."
 
 # Setting up
 setup(
        # the name must match the folder name
         name="eznet_torch", 
         version=VERSION,
         author="Pouya P. Niaz",
@@ -22,15 +22,15 @@
         long_description_content_type="text/markdown",
         packages=find_packages(),
         # packages=find_packages('eznet_torch'),
         # package_dir={'': 'eznet_torch'},
         python_requires=">=3.7, <4",
         license='MIT',
         install_requires=[
-            'numpy','tqdm','scikit-learn','torch (<2.0)'
+            'numpy','tqdm','scikit-learn','torch'
         ],
         keywords=['torch','pytorch','deep learning','neural network'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: End Users/Desktop",
             "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
```

