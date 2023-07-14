# Comparing `tmp/pileoffeather-0.2.0.tar.gz` & `tmp/pileoffeather-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pileoffeather-0.2.0.tar", last modified: Mon Jul 10 13:41:10 2023, max compression
+gzip compressed data, was "pileoffeather-0.3.0.tar", last modified: Fri Jul 14 23:44:26 2023, max compression
```

## Comparing `pileoffeather-0.2.0.tar` & `pileoffeather-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 13:41:10.298520 pileoffeather-0.2.0/
--rw-rw-rw-   0        0        0     1070 2023-07-09 14:44:27.000000 pileoffeather-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      349 2023-07-10 13:41:10.298520 pileoffeather-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3752 2023-07-10 13:10:38.000000 pileoffeather-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 13:41:10.282897 pileoffeather-0.2.0/pileoffeather/
--rw-rw-rw-   0        0        0       68 2023-07-09 14:43:17.000000 pileoffeather-0.2.0/pileoffeather/__init__.py
--rw-rw-rw-   0        0        0     1209 2023-07-10 13:34:27.000000 pileoffeather-0.2.0/pileoffeather/pod.py
--rw-rw-rw-   0        0        0     5288 2023-07-10 13:28:23.000000 pileoffeather-0.2.0/pileoffeather/pof.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:41:10.298520 pileoffeather-0.2.0/pileoffeather.egg-info/
--rw-rw-rw-   0        0        0      349 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-10 13:41:10.000000 pileoffeather-0.2.0/pileoffeather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 13:41:10.298520 pileoffeather-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-07-10 13:40:24.000000 pileoffeather-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:26.516637 pileoffeather-0.3.0/
+-rw-rw-rw-   0        0        0     1070 2023-07-09 14:44:27.000000 pileoffeather-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5699 2023-07-14 23:44:26.516637 pileoffeather-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5283 2023-07-14 23:42:34.000000 pileoffeather-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:26.516637 pileoffeather-0.3.0/pileoffeather/
+-rw-rw-rw-   0        0        0       68 2023-07-09 14:43:17.000000 pileoffeather-0.3.0/pileoffeather/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-07-14 23:15:39.000000 pileoffeather-0.3.0/pileoffeather/pod.py
+-rw-rw-rw-   0        0        0     4832 2023-07-14 08:20:13.000000 pileoffeather-0.3.0/pileoffeather/pof.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:26.516637 pileoffeather-0.3.0/pileoffeather.egg-info/
+-rw-rw-rw-   0        0        0     5699 2023-07-14 23:44:26.000000 pileoffeather-0.3.0/pileoffeather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-07-14 23:44:26.000000 pileoffeather-0.3.0/pileoffeather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 23:44:26.000000 pileoffeather-0.3.0/pileoffeather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-14 23:44:26.000000 pileoffeather-0.3.0/pileoffeather.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-14 23:44:26.000000 pileoffeather-0.3.0/pileoffeather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 23:44:26.516637 pileoffeather-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-07-14 15:58:57.000000 pileoffeather-0.3.0/setup.py
```

### Comparing `pileoffeather-0.2.0/LICENSE` & `pileoffeather-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pileoffeather-0.2.0/README.md` & `pileoffeather-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -15,91 +15,120 @@
 ---
 
 Install module
 ```cmd
 pip install pileoffeather
 ```
 # Examples
-Handwritten digit image classifier, dataset is made out of 500 images of ones and 500 images of zeros taken from the mnist dataset. The first code snippet is defining the neural network model, uploading the dataset and than training the model
+examples/simple_image_classifier - Handwritten digit image classifier, dataset is made out of 500 images of ones and 500 images of zeros taken from the mnist dataset. The first code snippet is defining the neural network model, uploading the dataset and than training the model
 ```python
 from pileoffeather import pof, pod
 import numpy as np
 
 #Define neural network model
 model = pof.neuralNetwork(layers = [[400,"input"],[30,"relu"],[10,"relu"],[1,"sigmoid"]], name = "test1")
 
 #Load the images for the dataset, 500 ones images and 500 zeros images
 ones = pod.load(data_type = "image", color = "grayscale", folder = "ones", resize = (20,20))
 zeros = pod.load(data_type = "image", color = "grayscale", folder = "zeros", resize = (20,20))
-input = np.vstack((ones, zeros))
+input = pod.merge(ones, zeros)
 
 #Generate expected output, first 500 images should output 1, the other 500 0
 output = np.concatenate((np.ones(500), np.zeros(500)))
 
 #Train the neural network using backpropagation
-model.train(input, output, batch_size = 16, epoch_number = 100, rate = 0.6)
+pof.train(model, input, output, batch_size = 16, epoch_number = 100, rate = 0.6)
 ```
 The second code snippet is testing the neural network on some examples
 ```python
 from pileoffeather import pof, pod
-import numpy as np
 
 #Define neural network model
 model = pof.neuralNetwork(load = "test1")
 
 #Run model
-output = model.run(pod.loadImage("example_image_one.png", (20,20), "grayscale"))
+input = pod.loadImage("example_image_one.png", (20,20), "grayscale")
+output = model.run(input)
 
 #Print result
 print(round(output[0],3))
 ```
 
 ---
 
+examples/mnist - Training script for the mnist dataset, 2 epochs -> 20~ seconds on 12600k -> 96%+ accuracy on 10k-test dataset
+```python
+from pileoffeather import pof, pod
+
+#Define neural network model
+model = pof.neuralNetwork(layers = [[784,""],[128,"relu"],[10,"sigmoid"]], name = "mnist")
+
+#Upload mnist dataset
+input_dataset = pod.load(data_type = "gz", path = "train-images-idx3-ubyte.gz", start_index = 16, input_number = 784, divide = 255)
+output_dataset = pod.load(data_type = "gz", path = "train-labels-idx1-ubyte.gz", start_index = 8, one_hot = 10)
+
+#Train the neural network using backpropagation
+pof.train(model, input_dataset, output_dataset, batch_size = 12, epoch_number = 2, rate = 1)
+```
+
+---
+
 # Documentation
-The library is structured in 2 files, pof.py (pile of feather) is the library for creating and training neural networks and pod.py (pile of data) is the library for importing your own data to create a training dataset for the neural network.
+The library is structured in 2 files, pof.py (pile of feather) is used to create and train neural networks, pod.py (pile of data) is used import your own data to generate a training dataset.
 ## pof.py - neural network module
 Install module
 ```cmd
 pip install pileoffeather
 ```
 Import module
 ```python
 from pileoffeather import pof
 ```
 Define neural network model, the available activation functions are "sigmoid","relu","leakyRelu"
 ```python
 model = pof.neuralNetwork(layers = [[400,""],[50,"relu"],[10,"relu"],[1,"sigmoid"]], name = "test1")
 ```
-Load an exsisting model
-```python
-model = pof.neuralNetwork(load = "test1")
-```
 Save the model
 ```python
 model.save()
 ```
-Train using backpropagation
+Load an exsisting model
 ```python
-model.train(input_matrix, output_matrix, batch_size = 16, epoch_number = 100, rate = 0.03)
+model = pof.neuralNetwork(load = "test1")
 ```
 Use the neural network
 ```python
 output = model.run(input)
 ```
+Compute backpropagation for a single batch, model.computeBatch(batch_input, batch_output, batch_size, learning_rate)
+```python
+model.computeBatch(batch_input, batch_output, 16, 0.3)
+```
+Method that contains model.computeBatch() in a loop so that it iterates over all the dataset for n epochs
+```python
+pof.train(model, input_matrix, output_matrix, batch_size = 16, epoch_number = 100, rate = 0.03)
+```
 
 ## pod.py - data load module
 Import module
 ```python
 from pileoffeather import pod
 ```
-Load images from a folder, color can be set to grayscale or rgb
+Load dataset of images from local folder
 ```python
 dataset = pod.load(data_type = "image", color = "grayscale", folder = "folder_name_containing_all_images", resize = (20,20))
 ```
+Load dataset from gz file like mnist
+```python
+#Load training input data of mnist, normalize input from 0 to 1 using divide = 255
+dataset = pod.load(data_type = "gz", path = "train-images-idx3-ubyte.gz", start_index = 16, input_number = 784, divide = 255)
+#Load training output data of mnist, use one_hot encoding to convert a decimal number to an array (pass total number of classes as parameter)
+#4 -> [0,0,0,0,1,0,0,0,0,0] 0 -> [1,0,0,0,0,0,0,0,0,0]
+dataset = pod.load(data_type = "gz", path = "train-labels-idx1-ubyte.gz", start_index = 8, one_hot = 10)
+```
 Load a single image to feed the neural network loadImage(name, resize, color)
 ```python
 input_vector = pod.loadImage("example_image.png", (20,20), "grayscale")
 ```
 Convert neural network output to image and save, saveImage(neural_network_output, image_path, resize, color)
 ```python
 pod.saveImage(neural_network_output, "image_path_and_name", (20,20), "grayscale")
```

### Comparing `pileoffeather-0.2.0/setup.py` & `pileoffeather-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+import os
 from setuptools import setup
 
+directory = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
+  long_description = f.read()
+
 setup(
     name='pileoffeather',
-    version='0.2.0',
+    version='0.3.0',
     license='MIT',
     url = 'https://github.com/usedToBeTomas/pile-of-feather',
     author='Daniele Tomaselli',
     description='Lightweight and easy to use ml library for small projects, create a neural network in minutes.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     packages=['pileoffeather'],
+    python_requires='>=3.6',
     keywords = ['neural network', 'ml', 'ai', 'machine learning','simple','nn'],
     install_requires=[
         'opencv-python',
         'numpy'
     ]
 )
```

