# Comparing `tmp/eznet_keras-0.0.3.tar.gz` & `tmp/eznet_keras-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eznet_keras-0.0.3.tar", last modified: Mon Feb  6 16:33:05 2023, max compression
+gzip compressed data, was "eznet_keras-1.0.0.tar", last modified: Sat Jul 15 17:58:53 2023, max compression
```

## Comparing `eznet_keras-0.0.3.tar` & `eznet_keras-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 16:33:05.126058 eznet_keras-0.0.3/
--rw-rw-rw-   0        0        0     1189 2023-01-20 13:30:59.000000 eznet_keras-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0    14339 2023-02-06 16:33:05.126058 eznet_keras-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    13276 2023-02-06 16:32:11.000000 eznet_keras-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-06 16:33:05.094070 eznet_keras-0.0.3/eznet_keras/
--rw-rw-rw-   0        0        0       40 2023-02-06 16:31:38.000000 eznet_keras-0.0.3/eznet_keras/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-06 16:33:05.111827 eznet_keras-0.0.3/eznet_keras/keras2cpp/
--rw-rw-rw-   0        0        0       24 2023-01-18 12:07:49.000000 eznet_keras-0.0.3/eznet_keras/keras2cpp/__init__.py
--rw-rw-rw-   0        0        0     9834 2022-07-10 10:31:49.000000 eznet_keras-0.0.3/eznet_keras/keras2cpp/create_unit_tests.py
--rw-rw-rw-   0        0        0     5519 2022-07-10 10:31:49.000000 eznet_keras-0.0.3/eznet_keras/keras2cpp/keras2cpp.py
--rw-rw-rw-   0        0        0      576 2022-07-10 10:31:49.000000 eznet_keras-0.0.3/eznet_keras/keras2cpp/python_model.py
-drwxrwxrwx   0        0        0        0 2023-02-06 16:33:05.125055 eznet_keras-0.0.3/eznet_keras/models/
--rw-rw-rw-   0        0        0      425 2023-01-19 20:08:07.000000 eznet_keras-0.0.3/eznet_keras/models/__init__.py
--rw-rw-rw-   0        0        0    10668 2023-01-19 20:15:26.000000 eznet_keras-0.0.3/eznet_keras/models/ann.py
--rw-rw-rw-   0        0        0    19924 2023-01-19 20:09:21.000000 eznet_keras-0.0.3/eznet_keras/models/conv_block.py
--rw-rw-rw-   0        0        0    22043 2023-01-19 20:16:25.000000 eznet_keras-0.0.3/eznet_keras/models/conv_network.py
--rw-rw-rw-   0        0        0     7571 2023-01-19 20:09:34.000000 eznet_keras-0.0.3/eznet_keras/models/dense_block.py
--rw-rw-rw-   0        0        0     9625 2023-01-19 20:06:17.000000 eznet_keras-0.0.3/eznet_keras/models/keras_smart_module.py
--rw-rw-rw-   0        0        0    16487 2023-02-03 13:49:26.000000 eznet_keras-0.0.3/eznet_keras/models/recurrent_network.py
--rw-rw-rw-   0        0        0     5319 2023-01-19 20:20:51.000000 eznet_keras-0.0.3/eznet_keras/models/var_ae.py
--rw-rw-rw-   0        0        0     2442 2023-01-19 20:22:43.000000 eznet_keras-0.0.3/eznet_keras/test.py
--rw-rw-rw-   0        0        0    13387 2023-01-19 20:11:44.000000 eznet_keras-0.0.3/eznet_keras/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-06 16:33:05.108827 eznet_keras-0.0.3/eznet_keras.egg-info/
--rw-rw-rw-   0        0        0    14339 2023-02-06 16:33:05.000000 eznet_keras-0.0.3/eznet_keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-02-06 16:33:05.000000 eznet_keras-0.0.3/eznet_keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 16:33:05.000000 eznet_keras-0.0.3/eznet_keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-02-06 16:33:05.000000 eznet_keras-0.0.3/eznet_keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-06 16:33:05.000000 eznet_keras-0.0.3/eznet_keras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-02-06 16:33:05.130765 eznet_keras-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1813 2023-02-06 16:31:20.000000 eznet_keras-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.317383 eznet_keras-1.0.0/
+-rw-rw-rw-   0        0        0     1189 2023-01-20 13:30:59.000000 eznet_keras-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    14243 2023-07-15 17:58:53.317383 eznet_keras-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13171 2023-07-15 17:55:34.000000 eznet_keras-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.300040 eznet_keras-1.0.0/eznet_keras/
+-rw-rw-rw-   0        0        0       40 2023-02-06 16:31:38.000000 eznet_keras-1.0.0/eznet_keras/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.312382 eznet_keras-1.0.0/eznet_keras/keras2cpp/
+-rw-rw-rw-   0        0        0       24 2023-01-18 12:07:49.000000 eznet_keras-1.0.0/eznet_keras/keras2cpp/__init__.py
+-rw-rw-rw-   0        0        0     9834 2022-07-10 10:31:49.000000 eznet_keras-1.0.0/eznet_keras/keras2cpp/create_unit_tests.py
+-rw-rw-rw-   0        0        0     5519 2022-07-10 10:31:49.000000 eznet_keras-1.0.0/eznet_keras/keras2cpp/keras2cpp.py
+-rw-rw-rw-   0        0        0      576 2022-07-10 10:31:49.000000 eznet_keras-1.0.0/eznet_keras/keras2cpp/python_model.py
+drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.316370 eznet_keras-1.0.0/eznet_keras/models/
+-rw-rw-rw-   0        0        0      425 2023-01-19 20:08:07.000000 eznet_keras-1.0.0/eznet_keras/models/__init__.py
+-rw-rw-rw-   0        0        0    17915 2023-07-15 17:25:36.000000 eznet_keras-1.0.0/eznet_keras/models/ann.py
+-rw-rw-rw-   0        0        0    26308 2023-07-14 09:38:07.000000 eznet_keras-1.0.0/eznet_keras/models/conv_block.py
+-rw-rw-rw-   0        0        0    31561 2023-07-15 17:26:46.000000 eznet_keras-1.0.0/eznet_keras/models/conv_network.py
+-rw-rw-rw-   0        0        0    11975 2023-07-14 12:26:34.000000 eznet_keras-1.0.0/eznet_keras/models/dense_block.py
+-rw-rw-rw-   0        0        0    11960 2023-07-15 17:49:42.000000 eznet_keras-1.0.0/eznet_keras/models/keras_smart_module.py
+-rw-rw-rw-   0        0        0    25219 2023-07-15 17:23:22.000000 eznet_keras-1.0.0/eznet_keras/models/recurrent_network.py
+-rw-rw-rw-   0        0        0     5319 2023-01-19 20:20:51.000000 eznet_keras-1.0.0/eznet_keras/models/var_ae.py
+-rw-rw-rw-   0        0        0     2442 2023-01-19 20:22:43.000000 eznet_keras-1.0.0/eznet_keras/test.py
+-rw-rw-rw-   0        0        0    13856 2023-07-15 13:47:05.000000 eznet_keras-1.0.0/eznet_keras/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 17:58:53.310390 eznet_keras-1.0.0/eznet_keras.egg-info/
+-rw-rw-rw-   0        0        0    14243 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-15 17:58:53.000000 eznet_keras-1.0.0/eznet_keras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-15 17:58:53.321459 eznet_keras-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2023-07-15 17:56:31.000000 eznet_keras-1.0.0/setup.py
```

### Comparing `eznet_keras-0.0.3/LICENSE.txt` & `eznet_keras-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eznet_keras-0.0.3/PKG-INFO` & `eznet_keras-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: eznet_keras
-Version: 0.0.3
-Summary: Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Conv blocks, etc.
+Version: 1.0.0
+Summary: Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc.
 Home-page: https://github.com/pniaz20/eznet_keras
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: tensorflow,keras,deep learning,neural network,keras2cpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -25,16 +25,16 @@
 
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.3  
-Last Update: Jan 20, 2023
+Version: 1.0.0  
+Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
 
@@ -84,21 +84,20 @@
     def call(self, x, *args, **kwargs):
         return self.net(x, *args, **kwargs)
 
 sample_hparams = {
     'model_name': 'KerasSmartModel',                    # Name of the model
     'l2_reg': 0.0001,                                   # L2 regularization parameter
     'batch_size': 16,                                   # Mini-batch size
-    'epochs': 2,                                        # Maximum training epochs
+    'epochs': 40,                                       # Maximum training epochs
     'validation_data': [0.05,'trainset'],               # Portion of train set used for validation (if necessary)
-    'validation_tolerance_epochs': 10,                  # Validation patience for early stopping
+    'early_stopping_patience_epochs': 10,               # Validation patience for early stopping
     'learning_rate': 0.0001,                            # (Initial) Learning rate
-    'learning_rate_decay_gamma': 0.99,                  # Learning rate exponential decay gamma
+    'exponential decay rate': 0.99,                     # Learning rate exponential decay factor
     'loss_function': 'categorical_crossentropy',        # Loss function string
-    'loss_function_params': None,                       # Dictionary of parameters to pass to the loss function
     'metrics':['accuracy'],                             # List of metrics
     'optimizer': 'Adam',                                # Optimizer string
     'optimizer_params': None,                           # Dictionary of parameters to pass to the optimizer constructor
     'checkpoint_path':None,                             # Path to store checkpoints in every epoch
     'early_stopping_monitor':'loss',                    # Early stopping criteria (stop when alue is reached and performance is good enough)
     'early_stopping_mode':'min',                        # Early stopping variable mode (minimization or maximization)
     'early_stopping_value':1.0e-6                       # Threshold for early stopping
@@ -107,15 +106,15 @@
 model = MyModel(sample_hparams)
 
 x_train = ...
 y_train = ...
 x_test = ...
 y_test = ...
 
-model.train(x_train, x_test, y_train, y_test, verbose=1, saveto="my_model", export="my_model.model")
+model.train_model(x_train, y_train, x_test, y_test, verbose=1, saveto="my_model", export="my_model.model")
 model.plot_history(metrics=['loss','val_loss'], fig_title='model loss', saveto="training_history.png")
 ```
 
 A few implementation notes:
 
 - Whatever hyperparameters you have for the model itself, can be included in the hparams dictionary.
 - The model must always have a `self.net` atttribute which contains the network itself. It can be a Sequential or Functional model.
```

### Comparing `eznet_keras-0.0.3/README.md` & `eznet_keras-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.3  
-Last Update: Jan 20, 2023
+Version: 1.0.0  
+Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
 
@@ -59,21 +59,20 @@
     def call(self, x, *args, **kwargs):
         return self.net(x, *args, **kwargs)
 
 sample_hparams = {
     'model_name': 'KerasSmartModel',                    # Name of the model
     'l2_reg': 0.0001,                                   # L2 regularization parameter
     'batch_size': 16,                                   # Mini-batch size
-    'epochs': 2,                                        # Maximum training epochs
+    'epochs': 40,                                       # Maximum training epochs
     'validation_data': [0.05,'trainset'],               # Portion of train set used for validation (if necessary)
-    'validation_tolerance_epochs': 10,                  # Validation patience for early stopping
+    'early_stopping_patience_epochs': 10,               # Validation patience for early stopping
     'learning_rate': 0.0001,                            # (Initial) Learning rate
-    'learning_rate_decay_gamma': 0.99,                  # Learning rate exponential decay gamma
+    'exponential decay rate': 0.99,                     # Learning rate exponential decay factor
     'loss_function': 'categorical_crossentropy',        # Loss function string
-    'loss_function_params': None,                       # Dictionary of parameters to pass to the loss function
     'metrics':['accuracy'],                             # List of metrics
     'optimizer': 'Adam',                                # Optimizer string
     'optimizer_params': None,                           # Dictionary of parameters to pass to the optimizer constructor
     'checkpoint_path':None,                             # Path to store checkpoints in every epoch
     'early_stopping_monitor':'loss',                    # Early stopping criteria (stop when alue is reached and performance is good enough)
     'early_stopping_mode':'min',                        # Early stopping variable mode (minimization or maximization)
     'early_stopping_value':1.0e-6                       # Threshold for early stopping
@@ -82,15 +81,15 @@
 model = MyModel(sample_hparams)
 
 x_train = ...
 y_train = ...
 x_test = ...
 y_test = ...
 
-model.train(x_train, x_test, y_train, y_test, verbose=1, saveto="my_model", export="my_model.model")
+model.train_model(x_train, y_train, x_test, y_test, verbose=1, saveto="my_model", export="my_model.model")
 model.plot_history(metrics=['loss','val_loss'], fig_title='model loss', saveto="training_history.png")
 ```
 
 A few implementation notes:
 
 - Whatever hyperparameters you have for the model itself, can be included in the hparams dictionary.
 - The model must always have a `self.net` atttribute which contains the network itself. It can be a Sequential or Functional model.
```

### Comparing `eznet_keras-0.0.3/eznet_keras/keras2cpp/create_unit_tests.py` & `eznet_keras-1.0.0/eznet_keras/keras2cpp/create_unit_tests.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-0.0.3/eznet_keras/keras2cpp/keras2cpp.py` & `eznet_keras-1.0.0/eznet_keras/keras2cpp/keras2cpp.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-0.0.3/eznet_keras/keras2cpp/python_model.py` & `eznet_keras-1.0.0/eznet_keras/keras2cpp/python_model.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-0.0.3/eznet_keras/models/ann.py` & `eznet_keras-1.0.0/eznet_keras/models/dense_block.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,160 +1,213 @@
+
+
 if __package__=="eznet_keras.models":
-    from .keras_smart_module import *
-    from .dense_block import *
+    from ..utils import *
 else:
-    import sys, os
-    sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
-    from keras_smart_module import *
-    from dense_block import *
-
-class ANN(KerasSmartModel):
-    
-    sample_hparams = {
-        "model_name": "ANN",
-        "input_size": 10,
-        "output_size": 3,
-        "width": 32,
-        "depth": 2,
-        "hidden_activation": "relu",
-        "hidden_activation_params": None,
-        "output_activation": None,
-        "output_activation_params": None,
-        "norm_layer_type":"BatchNormalization",
-        "norm_layer_position": "before",
-        "norm_layer_params": None,
-        "dropout": 0.2,
-        "learning_rate": 0.001,
-        "learning_rate_decay_gamma": 0.99,
-        "batch_size": 32,
-        "epochs": 2,
-        "validation_tolerance_epochs": 2,
-        "validation_data":[0.05,'trainset'],
-        "l2_reg": 0.0001,
-        "loss_function": "categorical_crossentropy",
-        "loss_function_params": None,
-        'optimizer': 'Adam',
-        'optimizer_params': None,
-        'metrics':['accuracy'],
-        'checkpoint_path':None,
-        'early_stopping_monitor':'loss',
-        'early_stopping_mode':'min',
-        'early_stopping_value':1.0e-6
-    }
-    
-    
-    def __init__(self, hparams:dict=None):
-        """Typical Artificial Neural Network class, also known as multilayer perceptron. This class will create a fully connected feedforward artificial neural network.
-        It can be used for classification, regression, etc. It basically encompasses enough options to build all kinds of ANNs with any number of 
-        inputs, outputs, layers with custom or arbitrary width or depth, etc. Supports multiple activation functions for hidden layers and the output layer.
-        
-        ### Usage
-        `net = ANN(hparams)` where `hparams` is the dictionary of hyperparameters.
-
-        It can include the following keys:
-            - `input_size` (int): number of inputs to the ANN, i.e. size of the input layer.
-            - `output_size` (int): number of outputs to predict, i.e. size of the output layer.
-            - `width` (int|list): (list of) hidden layer widths. 
-                a number sets them all the same, and a list/array sets each hidden layer according to the list.
-            - `depth` (int): Specifies the depth of the network (number of hidden layers).
-                It must be specified unless `width` is provided as a list. Then the depth will be inferred form it.
-            - `hidden_activation` (str): (list of) Activations of the hidden layers. Examples include "relu", "leakyrelu", "sigmoid", "tanh", "softmax", etc.
-            - `hidden_activation_params` (dict): (list of) Parameters for the hidden layer activation function, if any.
-            - `output_activation` (str): Activation of the output layer, if any.
-                **Note**: For classification problems, you may want to choose "sigmoid" or "softmax".
-                That being said, you usually don't need to specify an activation for the output layer at all, if e.g. 'from_logits' is used.
-                **Note**: For regression problems, no activation is needed. It is by default linear, unless you want to manually specify an activation.
-            - `output_activation_params` (dict): Parameters for the output activation function, if any.
-            - `norm_layer_type` (str): (list of) Types of normalization layers to use for each hidden layer. Options are "BatchNormalization", "LayerNormalization", etc.
-            - `norm_layer_position` (str): (list of) where the normalization layer should be included relative to the activation function, 'before' or 'after'.
-            - `norm_layer_params` (dict): (list of) Dictionaries of parameters for the normalization layers.
-            - `dropout` (float): (list of) the dropout rates after every hidden layer. It should be a probability value between 0 and 1.
-            - `learning_rate` (float): Initial learning rate of training.
-            - `learning_rate_decay_gamma` (float): Exponential decay rate gamma for learning rate, if any.
-            - `optimizer` (str): Optimizer. Examples: "Adam", "SGD" ,"RMSProp", etc.
-            - `optimizer_params` (dict): Additional parameters of the optimizer, if any.
-            - `batch_size` (int): Minibatch size for training.
-            - `epochs` (int): Maximum number of epochs for training.
-            - `validation_tolerance_epochs` (int): Epochs to tolerate unimproved val loss, before early stopping.
-            - `validation_data` (list): List of [validation_split, 'trainset'|'testset'].
-            - `l2_reg` (float): L2 regularization parameter.
-            - `loss_function` (str): Loss function. Examples: "mse","binary_crossentropy", "categorical_crossentropy", etc.
-            - `loss_function_params` (dict): Additional parameters for the loss function, if any.
-            - `metrics` (list): list of metrics for Keras compilation, e.g. ['accuracy'].
-            - `checkpoint_path` (str): Path to the directory where checkpoints will be saved at every epoch.
-            - `early_stopping_monitor` (str): Monitor whose critical value will cause early stopping. Default is 'loss', but 'val_loss' is typically used.
-            - `early_stopping_mode` (str): Mode of the parameter whose critical value will be used for early stopping. Deafults to 'min' for any error. 'max' is for accuracy, etc.
-            - `early_stopping_value` (float): Value of the monitor at which point training will stop becasue the critical value has been reached.
-        
-        Note that for all such hyperparameters that have a (list of) at the beginning, the entry can be a single item repeated for all hidden layers, or it can be a list of items
-        for all hidden layers. If a list is provided, it must have the same length as the depth of the network. Also note that depth does not include the input and output layers.
-        This gives you the ability to specify different width, dropout rate, normalization layer and its parameters, and so forth.
-        
-        Also note that the hidden layer just before the output layer will not have any dropout, which is typical.
-
-        ### Returns
-        It returns a `tf.keras.models.Model` object that corresponds with an ANN model.
-        run `net.summary()` afterwards to see what the ANN holds.
-        The returned module is a `KerasSmartModel` object, which is a subclass. It has built-in functions for training, evaluation, etc.
+    import os, sys
+    parent_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+    sys.path.append(parent_dir)
+    from utils import *
+
+
+class Dense_Block(tf.keras.layers.Layer):
+    def __init__(self, input_shape:list=None, output_size:int=None, activation:str=None, activation_params:dict=None, norm_layer_type:str=None, norm_layer_position:str='before', 
+                 norm_layer_params:dict=None, dropout:float=None, kernel_regularizer:tf.keras.regularizers.Regularizer=None):
+        """Dense (fully connected) block containing one linear layer, followed optionally by a normalization layer, an activation function and a Dropout layer.
+
+        ### Args:
+            - `input_shape` (list|tuple): Shape of the input without the batch size.
+            - `output_size` (int, optional): Number of output features. Defaults to None, in which case it will be input_size.
+            - `activation` (str, optional): Activation. It can be an activation function name ("relu","sigmoid","tanh", etc.), an activation layer name ("ReLU", "LeakyReLU",
+                "Softmax", etc.), or a custom Keras Layer class (not instance). Defaults to None.
+            - `activation_params` (dict, optional): kwargs to pass to the activation function constructor. Defaults to None. Ignored if `activation` is a lower-case function name.
+                By the way, the slope of the negative section in `LeakyReLU` is `alpha`.
+            - `norm_layer_type` (str, optional): Type of normalization layer. Defaults to None. Examples: 'BatchNormalization', 'LayerNormalization', etc.
+                It can also be a Keras Layer class (not instance).
+            - `norm_layer_position` (str, optional): Position of norm layer relative to activation. Defaults to 'before'. Alternative is 'after'.
+            - `norm_layer_params` (dict, optional): kwargs to pass to the norm layer constructor. Defaults to None.
+            - `dropout` (float, optional): Dropout rate at the end. Defaults to None. Must be a float between 0 and 1.
+            - `kernel_regularizer` (regularizer, optinal): Regularizer instance to be used for the kernel weights in the layers.
+        
+        
+        **NOTE**: 
+        Activation functions come from `tf.keras.activations` and need to be wrapped in a `tf.keras.layers.Activation` layer, and do not accept any kwargs. Activation layers
+        come from `tf.keras.layers`, can accept kwargs in their constructors, and do not need to be wrapped in an `Activation` layer. Activation functions all have lower-case
+        names, but activation layers are classes and have every-word-capitalized names. We will use this as a clue to recognize what the user wants, and perform accordingly.
+        Most activation layers also have correpsonding activation functions (like `tf.keras.activations.relu` function and `tf.keras.layers.ReLU` layer). 
+        However, some activations are only available as functions (such as `tf.keras.activations.sigmoid`), and some are only available as layers 
+        (such as `tf.keras.layers.LeakyReLU`). Choose accordingly.
+            
+        ### Returns:
+        A `tf.keras.layers.Layer` object.
         """
-        super(ANN, self).__init__(hparams)
-        # Read and store hyperparameters
-        if not hparams: hparams=self.sample_hparams
-        self._insize = hparams["input_size"]
-        self._outsize = hparams["output_size"]
-        self._dropout = hparams.get("dropout")
-        self._width = hparams.get("width")
-        self._depth = hparams.get("depth")
-        self._denseactivation = hparams["hidden_activation"]
-        self._denseactivation_params = hparams.get("hidden_activation_params")
-        self._outactivation = hparams.get("output_activation") if hparams.get("output_activation") else None
-        self._outactivation_params = hparams.get("output_activation_params")
-        self._norm_layer_type = hparams.get("norm_layer_type")
-        self._norm_layer_position = hparams.get("norm_layer_position")
-        self._norm_layer_params = hparams.get("norm_layer_params")
-        self.batch_input_shape = (self._batch_size, self._insize)
-        self.batch_output_shape = (self._batch_size, self._outsize)
-        self._out_activation_module = actdict_keras[self._outactivation] if self._outactivation else None
-        
-        # Generate arrays containing parameters of each Dense Block (Every block contains a linear, normalization, activation, and dropout layer).
-        self._dense_width_vec = self._gen_hparam_vec_for_dense(self._width, 'width')
-        self._dense_activation_vec = self._gen_hparam_vec_for_dense(self._denseactivation, 'hidden_activation')
-        self._dense_activation_params_vec = self._gen_hparam_vec_for_dense(self._denseactivation_params, 'hidden_activation_params')
-        self._dense_norm_layer_type_vec = self._gen_hparam_vec_for_dense(self._norm_layer_type, 'norm_layer_type')
-        self._dense_norm_layer_params_vec = self._gen_hparam_vec_for_dense(self._norm_layer_params, 'norm_layer_params')
-        self._dense_norm_layer_position_vec = self._gen_hparam_vec_for_dense(self._norm_layer_position, 'norm_layer_position')
-        self._dense_dropout_vec = self._gen_hparam_vec_for_dense(self._dropout, 'dropout')
-        
-        # Initialize sequential model
+        super(Dense_Block, self).__init__()
+        if output_size is None: 
+            if input_shape:
+                output_size = input_shape[-1]
+            else:
+                raise ValueError("Either input_shape or output_size must be provided.")
+        self._input_shape = input_shape
+        self._output_size = output_size
+        self._activation = activation
+        self._activation_params = activation_params
+        self._norm_layer_type = norm_layer_type
+        self._norm_layer_position = norm_layer_position
+        self._norm_layer_params = norm_layer_params
+        self._dropout = dropout
+        if activation is not None:
+            if isinstance(activation, str):
+                if activation.lower()==activation:
+                    self._activation_module = getattr(tf.keras.activations, activation)
+                else:
+                    self._activation_module = getattr(tf.keras.layers, activation)
+            else:
+                self._activation_module = activation
+        else:
+            self._activation_module = None
+        if norm_layer_type is not None:
+            if isinstance(norm_layer_type, str):
+                self._norm_layer_module = getattr(tf.keras.layers, norm_layer_type)
+            else:
+                self._norm_layer_module = norm_layer_type
+        else:
+            self._norm_layer_module = None
+        self._dropout_module = tf.keras.layers.Dropout if dropout else None
+        self._kernel_regularizer = kernel_regularizer
         self.net = tf.keras.models.Sequential()
+        if input_shape:
+            self.net.add(tf.keras.layers.Dense(output_size, input_shape=input_shape, kernel_regularizer=kernel_regularizer))
+        else:
+            self.net.add(tf.keras.layers.Dense(output_size, kernel_regularizer=kernel_regularizer))
+        if norm_layer_type and norm_layer_position=='before': 
+            if norm_layer_params: self.net.add(self._norm_layer_module(**norm_layer_params))
+            else: self.net.add(self._norm_layer_module())
+        if activation:
+            if isinstance(activation, str) and activation.lower()==activation: 
+                self.net.add(tf.keras.layers.Activation(self._activation_module))
+            else:
+                if activation_params: self.net.add(self._activation_module(**activation_params))
+                else: self.net.add(self._activation_module())
+        if norm_layer_type and norm_layer_position=='after': 
+            if norm_layer_params: self.net.add(self._norm_layer_module(**norm_layer_params))
+            else: self.net.add(self._norm_layer_module())
+        if dropout: self.net.add(self._dropout_module(dropout))
+    
+    def call(self, x, *args, **kwargs):
+        return self.net(x, *args, **kwargs)
+    
+    def get_config(self):
+        config = super(Dense_Block, self).get_config()
+        hparams = {
+            'input_shape':self._input_shape,
+            'output_size':self._output_size,
+            'activation':self._activation,
+            'activation_params':self._activation_params,
+            'norm_layer_type':self._norm_layer_type,
+            'norm_layer_position':self._norm_layer_position,
+            'norm_layer_params':self._norm_layer_params,
+            'dropout':self._dropout,
+            'kernel_regularizer':self._kernel_regularizer
+        }
+        config['hparams'] = hparams
+        return config
+    
+    @classmethod
+    def from_config(cls, config):
+        return cls(**config['hparams'])
+    
+    def summary(self):
+        return self.net.summary()
         
-        # Construct the dense layers
-        in_size = self._insize
-        for i in range(self._depth):
-            out_size = self._dense_width_vec[i]
-            temp_dropout_rate = self._dense_dropout_vec[i] if (i != self._depth-1) else None # The hidden layer just before the output layer rarely has Dropout.
-            _kwargs = {
-                'model':self.net,
-                'output_size':self._dense_width_vec[i],
-                'activation':self._dense_activation_vec[i],
-                'activation_params':self._dense_activation_params_vec[i],
-                'norm_layer_type':self._dense_norm_layer_type_vec[i],
-                'norm_layer_position':self._dense_norm_layer_position_vec[i],
-                'norm_layer_params':self._dense_norm_layer_params_vec[i],
-                'dropout':temp_dropout_rate,
-                'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None)
-            }
-            if i==0:
-                _kwargs.update({'input_shape':[self._insize]})
-            add_dense_block(**_kwargs)
-            in_size = out_size
-        # Output layer
-        self.net.add(tf.keras.layers.Dense(self._outsize))
-        if self._outactivation:
-            if self._outactivation_params: self.net.add(tf.keras.layers.Activation(self._out_activation_module(**self._outactivation_params)))
-            else: self.net.add(tf.keras.layers.Activation(self._out_activation_module))
 
-    def _gen_hparam_vec_for_dense(self, hparam, hparam_name, **kwargs):
-        return generate_array_for_hparam(hparam, self._depth, hparam_name=hparam_name, count_if_not_list_name='depth', **kwargs)
+
+
+def add_dense_block(model:tf.keras.models.Sequential, output_size:int, input_shape:list=None, activation:str=None, activation_params:dict=None, 
+                    norm_layer_type:str=None, norm_layer_position:str='before', norm_layer_params:dict=None, dropout:float=None, 
+                    kernel_regularizer:tf.keras.regularizers.Regularizer=None):
+    """Add a Dense (fully connected) block containing one linear layer, followed optionally by a normalization layer, an activation function and a Dropout layer, 
+    to a `tf.keras.models.Sequential` instance.
+
+        ### Args:
+            - `input_shape` (list|tuple, optional): Shape of the input disregarding the batch size.
+            - `output_size` (int, optional): Number of output features. Defaults to None, in which case it will be input_size.
+            - `activation` (str, optional): Activation. It can be an activation function name ("relu","sigmoid","tanh", etc.), an activation layer name ("ReLU", "LeakyReLU",
+                "Softmax", etc.), or a custom Keras Layer class (not instance). Defaults to None.
+            - `activation_params` (dict, optional): kwargs to pass to the activation function constructor. Defaults to None. Ignored if `activation` is a lower-case function name.
+                By the way, the slope of the negative section in `LeakyReLU` is `alpha`.
+            - `norm_layer_type` (str, optional): Type of normalization layer. Defaults to None. Examples: 'BatchNormalization', 'LayerNormalization', etc.
+                It can also be a Keras Layer class (not instance).
+            - `norm_layer_position` (str, optional): Position of norm layer relative to activation. Defaults to 'before'. Alternative is 'after'.
+            - `norm_layer_params` (dict, optional): kwargs to pass to the norm layer constructor. Defaults to None.
+            - `dropout` (float, optional): Dropout rate at the end. Defaults to None. Must be a float between 0 and 1.
+            - `kernel_regularizer` (regularizer, optinal): Regularizer to be used for the kernel weights in the layers.
+            
+        ### Returns:
+        Nothing. It modifies the `model` argument passed to it.
+        """
+    
+    _dropout_module = tf.keras.layers.Dropout if dropout else None
+    
+    if activation is not None:
+        if isinstance(activation, str):
+            if activation.lower()==activation:
+                _activation_module = getattr(tf.keras.activations, activation)
+            else:
+                _activation_module = getattr(tf.keras.layers, activation)
+        else:
+            _activation_module = activation
+    else:
+        _activation_module = None
+        
+    if norm_layer_type is not None:
+        if isinstance(norm_layer_type, str):
+            _norm_layer_module = getattr(tf.keras.layers, norm_layer_type)
+        else:
+            _norm_layer_module = norm_layer_type
+    else:
+        _norm_layer_module = None
+    
+    if input_shape:
+        model.add(tf.keras.layers.Dense(output_size, input_shape=input_shape, kernel_regularizer=kernel_regularizer))
+    else:
+        model.add(tf.keras.layers.Dense(output_size, kernel_regularizer=kernel_regularizer))
+        
+    if norm_layer_type and norm_layer_position=='before': 
+        if norm_layer_params: model.add(_norm_layer_module(**norm_layer_params))
+        else: model.add(_norm_layer_module())
+        
+    if activation: 
+        if isinstance(activation, str) and activation.lower()==activation: 
+            model.add(tf.keras.layers.Activation(_activation_module))
+        else:
+            if activation_params: model.add(_activation_module(**activation_params))
+            else: model.add(_activation_module())
+            
+    if norm_layer_type and norm_layer_position=='after': 
+        if norm_layer_params: model.add(_norm_layer_module(**norm_layer_params))
+        else: model.add(_norm_layer_module())
         
-    def call(self, x, **kwargs):
-        return self.net(x, **kwargs)
+    if dropout: model.add(_dropout_module(dropout))
+    
+    
+    
+
+if __name__=='__main__':
+    
+    # Test Dense_Block class
+    print("Testing Dense_Block class...")
+    block = Dense_Block(input_shape=[5], output_size=20, activation="LeakyReLU", activation_params={'alpha':0.1}, norm_layer_type="BatchNormalization", 
+                        norm_layer_position='before', norm_layer_params=None, dropout=0.1, kernel_regularizer=None)
+    block.summary()
+    y = block(tf.random.normal([32,5]))
+    print("Shape of output tensor:", y.shape)
+    
+    print("\n")
+    print("Testing add_dense_block function...")
+    model = tf.keras.models.Sequential()
+    add_dense_block(model, output_size=20, input_shape=[10], activation="LeakyReLU", activation_params={'alpha':0.1}, 
+                    norm_layer_type="BatchNormalization", norm_layer_position='before', norm_layer_params=None, dropout=0.5, 
+                    kernel_regularizer=None)
+    model.summary()
+    y = model(tf.random.normal([32,10]))
+    print("Shape of output tensor:", y.shape)
+
```

### Comparing `eznet_keras-0.0.3/eznet_keras/models/conv_block.py` & `eznet_keras-1.0.0/eznet_keras/models/conv_block.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,46 +7,64 @@
     from utils import *
 import warnings
 
 class Conv_Block(tf.keras.layers.Layer):
     def __init__(self, input_shape:list, out_channels:int=None, conv_dim:int=1, input_image:list=[30], conv_kernel_size=3, conv_padding='valid', conv_stride=1, conv_dilation=1, 
                  conv_params:dict=None, conv_activation:str='relu', conv_activation_params:dict=None, norm_layer_position:str=None, norm_layer_type:str=None, 
                  norm_layer_params:dict=None, pool_type:str=None, pool_kernel_size=2, pool_padding:str='valid', pool_stride=1, pool_params:dict=None, 
-                 dropout:float=None, min_image_dim:int=1, kernel_regularizer:tf.keras.regularizers.Regularizer=None):
-        """Convolutional block, containing one convolution layer, followed optionally by a normalization layer, an activation layer, a pooling layer and a dropout layer. The
-        convolution layer is mandatory, but the other ones are optional. The convolution layer can be 1D, 2D or 3D. The normalization layer can be any such layer defined
-        in Keras. The activation layer can also be anything with lower-case strings, and the pooling layer can be any of the pooling layers defined for Keras. 
-        The dropout layer is a spatial dropout layer. The dimension of any dropout layer will match the dimension of the convolution layer. For `Conv1D` for instance, 
-        `SpatialDropout1D` will be used, if desired.
+                 dropout:float=None, spatial_dropout:float=None, min_image_dim:int=1, kernel_regularizer:tf.keras.regularizers.Regularizer=None):
+        """Convolutional block, used as a single building block for all kinds of convolutional neural networks.
+        It contains one convolution layer, followed optionally by a normalization layer, an activation layer, a pooling layer and a dropout layer.
+        The convolution layer is mandatory, but the other ones are optional. The convolution layer can be 1D, 2D or 3D. 
+        The normalization layer can be the name of any such layer defined in Keras, e.g. `BatchNormalization`, or a custom `tf.keras.Layer` class (not instance).
+        The pooling type can be `Avg`, `Max`, `GlobalAvg`, `GlobalMax`, or a custom `tf.keras.Layer` class (not instance).
+        The activation can be the name of an activation function (e.g. 'relu', 'sigmoid', etc.), or the name of a Keras activation layer (e.g. 'ReLU', 'LeakyReLU', etc.), 
+        or a custom Keras Layer class (not instance).
+        The dropout consists of a spatial dropout layer followed by a normal dropout layer. It is, however, not common to use both types of dropout in a single block. 
+        The dimension of any dropout layer will match the dimension of the convolution layer. For `Conv1D` for instance, `SpatialDropout1D` will be used, if desired.
         
         This module is meant to be used as a building block for larger modules.
+        
+        **NOTE**: 
+        Activation functions come from `tf.keras.activations` and need to be wrapped in a `tf.keras.layers.Activation` layer, and do not accept any kwargs. Activation layers
+        come from `tf.keras.layers`, can accept kwargs in their constructors, and do not need to be wrapped in an `Activation` layer. Activation functions all have lower-case
+        names, but activation layers are classes and have every-word-capitalized names. We will use this as a clue to recognize what the user wants, and perform accordingly.
+        Most activation layers also have correpsonding activation functions (like `tf.keras.activations.relu` function and `tf.keras.layers.ReLU` layer). 
+        However, some activations are only available as functions (such as `tf.keras.activations.sigmoid`), and some are only available as layers 
+        (such as `tf.keras.layers.LeakyReLU`). Choose accordingly.
 
         ### Args:
         
         - `input_shape` (list|tuple): Input shape.
         - `out_channels` (int, optional): Number of convolution filters. Defaults to the input channels size.
         - `conv_dim` (int, optional): Dimension of the convolution. Defaults to 1. 1 means Conv1d, 2 means Conv2d etc.
         - `input_image` (list, optional): Size of the input image. Defaults to [30]. This must be a list/tuple of integers, with legth equal to `conv_dim`.
         - `conv_kernel_size` (int, optional): Convolution kernel size. Defaults to 3. It is strongly recommended to provide a list of integers, with length equal to `conv_dim`.
         - `conv_padding` (str, optional): Convolution padding. Defaults to 'same'. Arrays are recommended over integers.
         - `conv_stride` (int, optional): Convolution stride. Defaults to 1.
         - `conv_dilation` (int, optional): Convolution dilation. Defaults to 1.
         - `conv_params` (dict, optional): Additional dictionary of kwargs for Conv?d module, to add or overwrite other parameters. Defaults to None.
           No matter what parameters are set by this class by default for Con?D layer, providing this dictionary will overwrite all of them.
-        - `conv_activation` (str, optional): String representing activation function. Defaults to 'relu'. Examples: 'leakyrelu', 'sigmoid', 'tanh' etc.
-        - `conv_activation_params` (dict, optional): kwargs dictionary for activation function. Defaults to None.
+        - `conv_activation` (str, optional): Name of activation layer class ("ReLU", "LeakyReLU", "Softmax", etc.), or activation function ("relu", "sigmoid", etc.),
+          or custom Keras Layer class (not instance). Defaults to 'ReLU'.
+        - `conv_activation_params` (dict, optional): kwargs dictionary for constructor of activation layer, if it is a layer or the name of a defined layer. 
+          Otherwise, if activation is the name of a function such as 'sigmoid', this entry will be ignored. Defaults to None. For `LeakyReLU`, `alpha` is the slope parameter
+          for the negative part.
         - `norm_layer_position` (str, optional): Position of the normalization layer relative to activation. Defaults to None. It should be 'before' or 'after' or None.
         - `norm_layer_type` (str, optional): Type of the normalization layer. Defaults to None. Examples: 'BatchNormalization', 'LayerNormalization', etc.
-        - `norm_layer_params` (dict, optional): kwargs dictionary for normalization layer. Defaults to None.
+          This can also be a custom-made Keras Layer class (not instance).
+        - `norm_layer_params` (dict, optional): kwargs dictionary for normalization layer constructor. Defaults to None.
         - `pool_type` (str, optional): Type of pooling layer, if any. Defaults to None. For example, 'Max', 'Avg', 'GlobalMax', 'GlobalAvg' etc.
+          This can also be a custom-made Keras Layer class (not instance).
         - `pool_kernel_size` (int, optional): Pooling kernel size. Defaults to 2. Arrays are recommended over integers.
         - `pool_padding` (int, optional): Padding for pooling layer. Defaults to 0. 'same' is NOT an option here.
         - `pool_stride` (int, optional): Pooling stride. Defaults to 1.
-        - `pool_params` (dict, optional): kwargs dictionary for pooling layer module to add to or overwrite its arguments. Defaults to None.
-        - `dropout` (float, optional): Dropout rate, if any. Defaults to None. for Conv?D, SpatialDropout?D is used.
+        - `pool_params` (dict, optional): kwargs dictionary for pooling layer constructor to add to or overwrite its arguments. Defaults to None.
+        - `dropout` (float, optional): Dropout rate, if any. Defaults to None.
+        - `spatial_dropout` (float, optional): Spatial dropout rate, if any. Defaults to None. For Conv?D, SpatialDropout?D is used.
         - `min_image_dim` (int, optional): Minimum image dimension. Defaults to 1. This is used for preventing the image dimension from becoming too small. 
             It can automatically adjust padding and stride for convolution and pooling layers to keep the image dimensions larger than this argument.
         - `kernel_regularizer` (regularizer, optinal): Regularizer to be used for the kernel weights in the layers.
         
         ### Returns:
         A `tf.keras.layers.Layer` instance representing a single convolutional block.
         
@@ -54,15 +72,15 @@
         `self.output_image` (list): Size of the output image.
         `self.net` (tf.keras.models.Sequential): The actual network, a `tf.keras.models.Sequential` instance.
         """
         super(Conv_Block, self).__init__()
         self.net = tf.keras.models.Sequential()
         ret = add_conv_block(self.net, out_channels, input_shape, conv_dim, input_image, conv_kernel_size, conv_padding, conv_stride, conv_dilation, conv_params,
                              conv_activation, conv_activation_params, norm_layer_position, norm_layer_type, norm_layer_params, 
-                             pool_type, pool_kernel_size, pool_padding, pool_stride, pool_params, dropout, min_image_dim, kernel_regularizer)
+                             pool_type, pool_kernel_size, pool_padding, pool_stride, pool_params, dropout, spatial_dropout, min_image_dim, kernel_regularizer)
         self.net = ret['model']
         self._input_shape = input_shape
         self.output_image = ret['output_image']
         self._out_channels = ret['out_channels']
         self._norm_layer_position = ret['norm_layer_position']
         self._norm_layer_type = ret['norm_layer_type']
         self._min_image_dim = ret['min_image_dim']
@@ -70,27 +88,29 @@
         self._conv_stride = ret['conv_stride']
         self._pool_padding = ret['pool_padding']
         self._pool_stride = ret['pool_stride']
         self._conv_module = ret['conv_module']
         self._conv_activation_module = ret['conv_activation_module']
         self._pool_module = ret['pool_module']
         self._dropout_module = ret['dropout_module']
+        self._spatial_dropout_module = ret['spatial_dropout_module']
         self._norm_layer_module = ret['norm_layer_module']
         
         # Store parameters as class attributes
         self._conv_kernel_size = conv_kernel_size
         self._conv_dilation = conv_dilation
         self._conv_params = conv_params
         self._conv_activation = conv_activation
         self._conv_activation_params = conv_activation_params
         self._norm_layer_params = norm_layer_params
         self._pool_type = pool_type
         self._pool_kernel_size = pool_kernel_size
         self._pool_params = pool_params
         self._dropout = dropout if dropout else None
+        self._spatial_dropout = spatial_dropout if spatial_dropout else None
         self._kernel_regularizer = kernel_regularizer
 
     def call(self, x, *args, **kwargs):
         return self.net(x, *args, **kwargs)
     
     def get_config(self):
         config = super(Conv_Block, self).get_config()
@@ -111,14 +131,15 @@
             "norm_layer_params":self._norm_layer_params,
             "pool_type":self._pool_type,
             "pool_kernel_size":self._pool_kernel_size,
             "pool_padding":self._pool_padding,
             "pool_stride":self._pool_stride,
             "pool_params":self._pool_params,
             "dropout":self._dropout,
+            "spatial_dropout":self._spatial_dropout,
             "min_image_dim":self._min_image_dim,
             "kernel_regularizer":self._kernel_regularizer
         }
         config['hparams'] = hparams
         return config
     
     @classmethod
@@ -127,50 +148,67 @@
     
     def summary(self):
         return self.net.summary()
 
 
 
 def add_conv_block(model:tf.keras.models.Sequential, out_channels:int=None, input_shape:list=None, conv_dim:int=1, input_image:list=[30], conv_kernel_size=3, conv_padding='valid',
-    conv_stride=1, conv_dilation=1, conv_params:dict=None, conv_activation:str='relu', conv_activation_params:dict=None, norm_layer_position:str=None, norm_layer_type:str=None, 
-    norm_layer_params:dict=None, pool_type:str=None, pool_kernel_size=2, pool_padding:str='valid', pool_stride=1, pool_params:dict=None, dropout:float=None, min_image_dim:int=1,
-    kernel_regularizer:tf.keras.regularizers.Regularizer=None):
-    """ Add a Convolutional block, containing one convolution layer, followed optionally by a normalization layer, an activation layer, a pooling layer and a dropout layer,
+    conv_stride=1, conv_dilation=1, conv_params:dict=None, conv_activation:str='ReLU', conv_activation_params:dict=None, norm_layer_position:str=None, norm_layer_type:str=None, 
+    norm_layer_params:dict=None, pool_type:str=None, pool_kernel_size=2, pool_padding:str='valid', pool_stride=1, pool_params:dict=None, dropout:float=None, 
+    spatial_dropout:float=None, min_image_dim:int=1, kernel_regularizer:tf.keras.regularizers.Regularizer=None):
+    """Add a Convolutional block, containing one convolution layer, followed optionally by a normalization layer, an activation layer, a pooling layer and a dropout layer,
     to the end of an existing `tf.keras.models.Sequential` instance.
-    The convolution layer is mandatory, but the other ones are optional. The convolution layer can be 1D, 2D or 3D. The normalization layer can be any such layer defined
-    in Keras. The activation layer can also be anything with lower-case strings, and the pooling layer can be any of the pooling layers defined for Keras. 
-    The dropout layer is a spatial dropout layer. The dimension of any dropout layer will match the dimension of the convolution layer. For `Conv1D` for instance, 
-    `SpatialDropout1D` will be used, if desired.
+    The convolution layer is mandatory, but the other ones are optional. The convolution layer can be 1D, 2D or 3D. 
+    The normalization layer can be the name of any layer defined such as `BatchNormalization`, or a custom Keras Layer class (not instance). 
+    The activation layer can be the name of an activation function ('sigmoid', 'relu', 'tanh', etc.), the name of an activation layer ('ReLU', 'LeakyReLU', 'Softmax', etc.), 
+    or a custom Keras Layer class (not instance). 
+    The pooling layer can be `Avg`, `Max`, `GlobalAvg` or `GlobalMax`. Also, it can be a custom Keras Layer class (not instance), in which case all pooling-related arguments
+    of this function will be ignored, and you'll have to pass pooling layer constructor arguments via `pool_params`. Also, in this case the image size calculations are bypassed.
+    The dropout consists of a spatial dropout followed by a normal dropout. It is not common, however, to use both kinds of dropout in a single CNN block.
+    The dimension of any dropout layer will match the dimension of the convolution layer. For `Conv1D` for instance, `SpatialDropout1D` will be used, if desired.
 
     ### Args:
     
     - `input_shape` (list|tuple): Input shape.
     - `out_channels` (int, optional): Number of convolution filters. Defaults to the input channels size.
     - `conv_dim` (int, optional): Dimension of the convolution. Defaults to 1. 1 means Conv1d, 2 means Conv2d etc.
     - `input_image` (list, optional): Size of the input image. Defaults to [30]. This must be a list/tuple of integers, with legth equal to `conv_dim`.
     - `conv_kernel_size` (int, optional): Convolution kernel size. Defaults to 3. It is strongly recommended to provide a list of integers, with length equal to `conv_dim`.
-    - `conv_padding` (str, optional): Convolution padding. Defaults to 'same'. Arrays are recommended over integers.
+    - `conv_padding` (str, optional): Convolution padding. Defaults to 'same'. Arrays are preferred over integers.
     - `conv_stride` (int, optional): Convolution stride. Defaults to 1.
     - `conv_dilation` (int, optional): Convolution dilation. Defaults to 1.
     - `conv_params` (dict, optional): Additional dictionary of kwargs for constructor of Conv?d module. Defaults to None.
       If provided, this dictionary will not only add to, but also overwrite any existing arguments passed to the Conv?D constructor.
-    - `conv_activation` (str, optional): String representing activation function. Defaults to 'relu'. Examples: 'leakyrelu', 'sigmoid', 'tanh' etc.
-    - `conv_activation_params` (dict, optional): kwargs dictionary for activation function. Defaults to None.
+    - `conv_activation` (str, optional): String representing activation function ('sigmoid', 'relu', 'softmax', 'tanh', etc.) or layer ('ReLU', 'LeakyReLU', 'Softmax', etc.).
+      Instead of a string, one can also provide a custom Keras Layer class (not instance). Defaults to 'ReLU'.
+    - `conv_activation_params` (dict, optional): kwargs dictionary for activation layer constructor, if it is a layer. Defaults to None. 
+      If the passed argument is a lower-case function name, this argument will be ignored. By the way, for `LeakyReLU`, `alpha` is the slope parameter in negative part.
     - `norm_layer_position` (str, optional): Position of the normalization layer relative to activation. Defaults to None. It should be 'before' or 'after' or None.
     - `norm_layer_type` (str, optional): Type of the normalization layer. Defaults to None. Examples: 'BatchNormalization', 'LayerNormalization', etc.
-    - `norm_layer_params` (dict, optional): kwargs dictionary for normalization layer. Defaults to None.
+      Instead of a string, a custom Keras Layer class (not instance) can also be provided.
+    - `norm_layer_params` (dict, optional): kwargs dictionary for normalization layer constructor. Defaults to None.
     - `pool_type` (str, optional): Type of pooling layer, if any. Defaults to None. For example, 'Max', 'Avg', 'GlobalMax', 'GlobalAvg' etc.
+      Instead of a string, a custom Keras Layer class (not instance) can also be provided.
     - `pool_kernel_size` (int, optional): Pooling kernel size. Defaults to 2. Arrays are recommended over integers.
     - `pool_padding` (int, optional): Padding for pooling layer. Defaults to 0. 'same' is NOT an option here.
     - `pool_stride` (int, optional): Pooling stride. Defaults to 1.
-    - `pool_params` (dict, optional): kwargs dictionary for pooling layer module, to add to or overwrite existing parameters. Defaults to None.
-    - `dropout` (float, optional): Dropout rate, if any. Defaults to None. for Conv?D, SpatialDropout?D is used.
+    - `pool_params` (dict, optional): kwargs dictionary for pooling layer constructor, to add to or overwrite existing parameters. Defaults to None.
+    - `dropout` (float, optional): Dropout rate, if any. Defaults to None.
+    - `spatial_dropout` (float, optional): Spatial dropout rate, if any. Defaults to None. For Conv?D, SpatialDropout?D will be used.
     - `min_image_dim` (int, optional): Minimum image dimension. Defaults to 1. This is used for preventing the image dimension from becoming too small. 
         It can automatically adjust padding and stride for convolution and pooling layers to keep the image dimensions larger than this argument.
-    - `kernel_regularizer` (regularizer, optional): Regularizer to be used for the kernel weights in the layers.
+    - `kernel_regularizer` (regularizer, optional): Keras Regularizer to be used for the kernel weights in the layers.
+    
+    **NOTE**: 
+        Activation functions come from `tf.keras.activations` and need to be wrapped in a `tf.keras.layers.Activation` layer, and do not accept any kwargs. Activation layers
+        come from `tf.keras.layers`, can accept kwargs in their constructors, and do not need to be wrapped in an `Activation` layer. Activation functions all have lower-case
+        names, but activation layers are classes and have every-word-capitalized names. We will use this as a clue to recognize what the user wants, and perform accordingly.
+        Most activation layers also have correpsonding activation functions (like `tf.keras.activations.relu` function and `tf.keras.layers.ReLU` layer). 
+        However, some activations are only available as functions (such as `tf.keras.activations.sigmoid`), and some are only available as layers 
+        (such as `tf.keras.layers.LeakyReLU`). Choose accordingly.
     
     ### Returns:
     A dictionary with the following fields:
     ```python
     {
         'model'
         'output_image'
@@ -182,43 +220,61 @@
         'conv_stride'
         'pool_padding'
         'pool_stride'
         'conv_module'
         'conv_activation_module'
         'pool_module'
         'dropout_module'
+        'spatial_dropout_module'
         'norm_layer_module'
     }
     ```
     """
     # Output channels check
     if not (isinstance(out_channels,int) and out_channels > 0):
-        warnings.warn("Invalid value out_channels={}. Using value {} equal to input_shape[-1].".format(out_channels,input_shape), UserWarning)
+        warnings.warn("Invalid value out_channels={}. Using value {} equal to input_shape[-1].".format(out_channels,input_shape[-1]), UserWarning)
         out_channels = input_shape[-1]
     # Convolution dimension check    
     assert isinstance(conv_dim, int) and conv_dim in [1,2,3], "`conv_dim` must be an integer among [1,2,3], not {} which has type {}.".format(conv_dim, str(type(conv_dim)))
     # Determine convolution module used
     _conv_module = convdict_keras["conv{}d".format(conv_dim)]
     # Input image size check
     assert isinstance(input_image, (list,tuple)) and len(input_image)==conv_dim, \
         "`input_image` must be a list or tuple of length equal to `conv_dim`, not {} which has type {}.".format(input_image, str(type(input_image)))
     # Check activation function and module
-    _conv_activation_module = actdict_keras[conv_activation]  if conv_activation else None
+    if isinstance(conv_activation, str):
+        if conv_activation.lower() == conv_activation: # activation function such as `sigmoid`
+            _conv_activation_module = getattr(tf.keras.activations, conv_activation)
+        else: # activation layer such as `ReLU`
+            _conv_activation_module = getattr(tf.keras.layers, conv_activation)
+    else:
+        _conv_activation_module = conv_activation
     # Check position, type and parameters of normalization layer
     if not norm_layer_position in ['before', 'after', None]:
         warnings.warn(("Invalid value {} for `norm_layer_position`: It can only be 'before' (before activation), 'after' (after activation) or None. "+
-                        "Using default value of None. There will be no normalization.").format(norm_layer_position), UserWarning)
+                        "Using default value of None. There will be no normalization layer.").format(norm_layer_position), UserWarning)
         norm_layer_position = None
     if norm_layer_position is None: norm_layer_type = None
     if norm_layer_type is None: norm_layer_position = None
-    _norm_layer_module = getattr(tf.keras.layers, norm_layer_type) if norm_layer_type else None
+    if isinstance(norm_layer_type, str):
+        _norm_layer_module = getattr(tf.keras.layers, norm_layer_type)
+    elif norm_layer_type is not None:
+        _norm_layer_module = norm_layer_type
+    else:
+        _norm_layer_module = None
     # Check pooling layer type, module and parameters
-    _pool_module = getattr(tf.keras.layers, "{}Pool{}D".format(pool_type, conv_dim)) if pool_type else None
+    if isinstance(pool_type, str):
+        _pool_module = getattr(tf.keras.layers, "{}Pool{}D".format(pool_type, conv_dim))
+    elif pool_type is not None:
+        _pool_module = pool_type
+    else:
+        _pool_module = None
     # Check Dropout parameters
-    _dropout_module = getattr(tf.keras.layers, 'SpatialDropout{}D'.format(conv_dim)) if dropout else None
+    _spatial_dropout_module = getattr(tf.keras.layers, 'SpatialDropout{}D'.format(conv_dim)) if spatial_dropout else None
+    _dropout_module = tf.keras.layers.Dropout if dropout else None
     # Store minimum desired image size
     min_image_dim = min_image_dim if min_image_dim>0 else 1
     img_size = input_image
     # -----------------------------------------------------------------------------        
     # Check if output image size is smaller than min_image_dim, and adjust parameters if necessary
     # print("Running calc_size for input image size {}".format(img_size))
     temp_img_size = calc_image_size(img_size, kernel_size=conv_kernel_size, stride=conv_stride, padding=conv_padding, dilation=conv_dilation)
@@ -239,44 +295,67 @@
     # ---------------------------------------------------------------------------
     # Construct normalization layer, if it should be here.
     if norm_layer_position=='before':
         if norm_layer_params: model.add(_norm_layer_module(**norm_layer_params))
         else: model.add(_norm_layer_module())
     # Construct activation layer
     if conv_activation:
-        if conv_activation_params: model.add(tf.keras.layers.Activation(_conv_activation_module(**conv_activation_params)))
-        else: model.add(tf.keras.layers.Activation(_conv_activation_module))
+        if isinstance(conv_activation, str) and conv_activation.lower() == conv_activation:
+            model.add(tf.keras.layers.Activation(_conv_activation_module))
+        elif conv_activation_params: 
+            model.add(_conv_activation_module(**conv_activation_params))
+        else: 
+            model.add(_conv_activation_module())
     # Construct normalization layer, if it should be here.
     if norm_layer_position=='after':
         if norm_layer_params: model.add(_norm_layer_module(**norm_layer_params))
         else: model.add(_norm_layer_module())
     # ---------------------------------------------------------------------------
     # Check type and parameters of the pooling layer, and calculate output image size
-    if pool_type is not None and 'global' in pool_type.lower():
-        if pool_params: model.add(_pool_module(**pool_params))
-        else: model.add(_pool_module())
-        img_size = [1]*conv_dim
-    elif pool_type is not None:
-        temp_img_size = calc_image_size(img_size, kernel_size=pool_kernel_size, stride=pool_stride, padding=pool_padding, dilation=1) # Keras pool has no support for dilation :(
-        if min(temp_img_size) < min_image_dim:
-            warnings.warn(
+    if pool_type is not None:
+        if isinstance(pool_type, str) and 'global' not in pool_type.lower():
+            temp_img_size = calc_image_size(img_size, kernel_size=pool_kernel_size, 
+                                            stride=pool_stride, padding=pool_padding, dilation=1) # Keras pool has no support for dilation :(
+            if min(temp_img_size) < min_image_dim:
+                warnings.warn(
                 "Output image ({}) of the pooling operation is smaller in one or more dimensions than min_image_dim={} for add_conv_block(). ".format(temp_img_size,min_image_dim)+ 
                 "Using padding={} and stride=1 instead of padding={} and stride={}".format('same', pool_padding, pool_stride), UserWarning)
-            pool_padding = 'same'
-            pool_stride = 1
-        _kwargs = {'pool_size':pool_kernel_size, 'strides':pool_stride, 'padding':pool_padding}
-        if pool_params: _kwargs.update(pool_params)
-        model.add(_pool_module(**_kwargs))
-        img_size = calc_image_size(img_size, kernel_size=pool_kernel_size, stride=pool_stride, padding=pool_padding, dilation=1)
+                pool_padding = 'same'
+                pool_stride = 1
+            _kwargs = {'pool_size':pool_kernel_size, 'strides':pool_stride, 'padding':pool_padding}
+            if pool_params: _kwargs.update(pool_params)
+            model.add(_pool_module(**_kwargs))
+            img_size = calc_image_size(img_size, kernel_size=pool_kernel_size, stride=pool_stride, padding=pool_padding, dilation=1)
+        else:
+            if pool_params: model.add(_pool_module(**pool_params))
+            else: model.add(_pool_module())
+            if isinstance(pool_type, str) and 'global' in pool_type.lower():
+                img_size = [1]*conv_dim
     # ---------------------------------------------------------------------------
     # Construct Dropout layer    
+    if spatial_dropout: model.add(_spatial_dropout_module(spatial_dropout))
     if dropout: model.add(_dropout_module(dropout))
     # Store output image size as attribute    
     output_image = img_size
     d = {
         'model':model, 'output_image':output_image, 'out_channels':out_channels, 'norm_layer_position':norm_layer_position,
         'norm_layer_type':norm_layer_type, 'min_image_dim':min_image_dim, 'conv_padding':conv_padding, 'conv_stride':conv_stride, 'pool_padding':pool_padding,
         'pool_stride':pool_stride, 'conv_module':_conv_module, 'conv_activation_module':_conv_activation_module, 'pool_module':_pool_module,
-        'dropout_module':_dropout_module, 'norm_layer_module':_norm_layer_module
+        'dropout_module':_dropout_module, 'spatial_dropout_module':_spatial_dropout_module, 'norm_layer_module':_norm_layer_module
     }
     return d
 
+
+
+
+if __name__ == '__main__':
+    # Test the add_conv_block function
+    model = tf.keras.models.Sequential()
+    add_conv_block(model, out_channels=64, input_shape=[28, 28, 3], conv_dim=2, input_image=[28, 28], conv_kernel_size=3, conv_padding='valid',
+    conv_stride=1, conv_dilation=1, conv_params=None, 
+    conv_activation='relu', 
+    conv_activation_params={'alpha':0.1}, norm_layer_position="before", 
+    norm_layer_type="BatchNormalization", 
+    norm_layer_params=None, pool_type="Max", pool_kernel_size=2, pool_padding='valid', pool_stride=1, pool_params=None, dropout=0.1, 
+    spatial_dropout=None, min_image_dim=1, kernel_regularizer=None)
+    model.summary()
+
```

### Comparing `eznet_keras-0.0.3/eznet_keras/models/conv_network.py` & `eznet_keras-1.0.0/eznet_keras/models/conv_network.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     import sys, os
     sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
     from keras_smart_module import *
     from conv_block import *
     from dense_block import *
 
 class Conv_Network(KerasSmartModel):
+    
     sample_hparams = {
         "model_name": "Conv_Network",
         # I/O shapes (without the batch dimension)
         "input_shape": [28, 28, 3],
         "output_shape": [10],
         # Convolution blocks
         "num_conv_blocks": 2,
@@ -26,173 +27,216 @@
         "conv_dilation": 1,
         "conv_activation": "relu",
         "conv_activation_params": None,
         "conv_norm_layer_type": "BatchNormalization",
         "conv_norm_layer_position": "before",
         "conv_norm_layer_params": None,
         "conv_dropout": 0.1,
+        "conv_spatial_dropout": None,
         "pool_type": "Max",
         "pool_kernel_size": 2,
         "pool_padding": 'valid',
         "pool_stride": 1,
         "pool_params": None,
         "min_image_size": 4,
+        "flatten_before_dense": True,
         # Fully connected blocks
         "dense_width": "auto",
         "dense_depth": 2,
         "dense_activation": "relu",
         "dense_activation_params": None,
-        "output_activation": "softmax",
-        "output_activation_params": None,
         "dense_norm_layer_type": "BatchNormalization",
         "dense_norm_layer_position": "before",
         "dense_norm_layer_params": None,
         "dense_dropout": 0.1,
+        "include_output_layer": True,
+        "output_activation": "softmax",
+        "output_activation_params": None,
         # Training procedure
         "l2_reg": 0.0001,
         "batch_size": 32,
         "epochs": 2,
         "validation_data": [0.05,'testset'],
-        "validation_tolerance_epochs": 5,
+        "early_stopping_patience_epochs": 5,
         "learning_rate": 0.01,
-        "learning_rate_decay_gamma": 0.9,
+        "exponential_decay_rate": 0.9,
         "loss_function": "categorical_crossentropy",
         "optimizer": "Adam",
         "optimizer_params": None,
         'metrics':['accuracy'],
         'checkpoint_path':None,
         'early_stopping_monitor':'loss',
         'early_stopping_mode':'min',
         'early_stopping_value':1.0e-6
     }
     
     
     def __init__(self, hparams:dict=None):
         """Standard Convolutional Neural Network, containing convolutional blocks followed by fully-connected blocks. It supports 1D, 2D, and 3D convolutions, and can be used for 
         image classification, timeseries classification, video classification, and so forth. The module can easily be trained and evaluated using its own methods,
-        because it inherits from `KerasSmartModel`.
+        because it inherits from `KerasSmartModel`. The architecture consists of conv blocks followed by dense blocks. Each conv block is assumed to contain a convolution layer, 
+        followed optionally be a normalization layer, an activation, pooling, and finally a dropout or spatial dropout layer. Each dense block is assumed to contain a dense layer,
+        followed optionally be a normalziation layer, an activation, and a dropout layer. Cnovolution blocks are mandatory, but Dense layers and an output layer are optional.
+        Using this class, any kind of serial CNN architecture can be built. However, no parallelism or skip connections are supported in the architecture.
 
         ### Usage
 
-        `model = Conv_Network(hparams)` where `hparams` is dictionary of hyperparameters containing the following:
+        `model = Conv_Network(hparams)` where `hparams` is dictionary of hyperparameters containing the following keys. 
+        
+        - Inspect the `sample_hparams` class attribute for a template of the hyperparameters dictionary.
+        - Many keys, especially those that have "(list of)" in their description, can be either scalar items or lists of items. If they are scalar, they will be broadcasted to all 
+          blocks. If they are lists, they must have the same length as the number (depth) of convolutional blocks, i.e. `num_conv_blocks` hyperparameter.
+        - Every block by default is assumed to have a convolution operation, a normalization layer, an activation, some form of pooling, and finally a dropout or spatial dropout. 
+          For every convolutional block, the convolution operation is mandatory but the rest are optional. Thsi way, any kind of CNN with any (fully serial) architecture can be 
+          built. If the key to some hyperparameter is a list, it must have a length equal to the number of convolutional blocks, that is, the `num_conv_blocks` hyperparameter. 
+          There must be one item per convolutional block. `None` is typically put for every block that doens't have that layer or that hyperparameter is inapplicable to that block.
+          Also note that we assume every convolutional block has a spatial dropout layer followed by a normal dropout layer, but this is not common in reality, which means for 
+          blocks that have spatial dropout the normal dropout rate should be `None`, and vice versa.
+        - The Training Procedure section of the hyperparameters are optional, and will only be used by the parent class `KerasSmartModel` if the model is trained using its methods.
+          Otherwise, it is not necessary at all.
+        - Activation functions come from `tf.keras.activations` and need to be wrapped in a `tf.keras.layers.Activation` layer, and do not accept any kwargs. Activation layers
+          come from `tf.keras.layers`, can accept kwargs in their constructors, and do not need to be wrapped in an `Activation` layer. Activation functions all have lower-case
+          names, but activation layers are classes and have every-word-capitalized names. We will use this as a clue to recognize what the user wants, and perform accordingly.
+          Most activation layers also have correpsonding activation functions (like `tf.keras.activations.relu` function and `tf.keras.layers.ReLU` layer). 
+          However, some activations are only available as functions (such as `tf.keras.activations.sigmoid`), and some are only available as layers 
+          (such as `tf.keras.layers.LeakyReLU`). Choose accordingly.
 
         #### I/O shapes
         
         - `input_shape` (list): Input shape *WITHOUT* the batch dimension. For instance, for 2D images, input should be [N, H, W, C], therefore `input_shape` should be [H, W, C].
         - `output_shape` (int): Output shape *WITHOUT* the batch dimension. For instance, for K-class classification, model outputs can be [N, K], so `output_shape` should be [K].
             
         #### Convolution blocks
         
         - `num_conv_blocks` (int): Number of convolutional blocks. Every block contains a convolutional layer, and
-            optionally a normalization layer, an activation layer, a pooling layer, and finally a dropout layer.
+            optionally a normalization layer, an activation layer, a pooling layer, and finally a dropout or spatial dropout layer.
         - `conv_dim` (int): Dimensionality of the convolution. 1, 2, or 3.
         - `conv_params` (dict): (list of) kwargs dict to pass to the convolution constructor in each block. Defaults to None.
-        - `conv_channels` (int|list|str): (list of) Number of filters of the convolution layer in each conv block. If `auto`, it will start
+        - `conv_channels` (int|list|str): (list of) Number of filters of the convolution layer in each conv block. If `"auto"`, it will start
             with the input channels, and double with every block, in powers of two. If `list`, it should be a list
-            of channels for each conv block. If `int`, it will be the same for all conv blocks. Default is `auto`.
+            of channels for each conv block. If `int`, it will be the same for all conv blocks. Default is `"auto"`.
         - `conv_kernel_size` (int|list): (list of) Kernel size of the convolution layers. Should be a list of integers,
             a list of tuples of integers (for conv2d or conv3d), or an integer. If it is a list, it MUST have the same 
-            length as `num_conv_blocks`. If it is an integer, it will be the same for all conv blocks. Defaults to 3.
-        - `conv_padding` (int|str|list): (list of) Paddings of convolution layers. Format is as `conv_kernel_size`. Defaults to "valid".
-        - `conv_stride` (int|list): (list of) Stride of convolution layers. Format is as `conv_kernel_size`. Defaults to 1.
-        - `conv_dilation` (int|list): (list of) Dilation of convolution layers. Format is as `conv_kernel_size`. Defaults to 1.
-        - `conv_activation` (str|list): (list of) string(s) representing activation func of the convolution layers. Examples: 'relu', 'leakyrelu', 'sigmoid', 'tanh', etc.
-        - `conv_activation_params` (dict|list): (list of) dicts for the convolution activation functions' constructors. Defaults to None.
+            length as `num_conv_blocks`. If it is an integer, it will be the same for all conv blocks. Defaults to `3`.
+        - `conv_padding` (int|str|list): (list of) Paddings of convolution layers. Format is as `conv_kernel_size`. Defaults to `"valid"`.
+        - `conv_stride` (int|list): (list of) Strides of convolution layers. Format is as `conv_kernel_size`. Defaults to `1`.
+        - `conv_dilation` (int|list): (list of) Dilations of convolution layers. Format is as `conv_kernel_size`. Defaults to `1`.
+        - `conv_activation` (str|list): (list of) activations of the convolution blocks. Defaults to None.
+            For each block, this entry can be an activation function ("relu", "sigmoid", "tanh", etc.), an activation layer ("ReLU", "LeakyReLU", "Softmax", etc.), or a custom
+            Layer class (not instance). `None` will assume no activation for the convolution layer.
+        - `conv_activation_params` (dict|list): (list of) dicts for the convolution activation constructors. Defaults to None. This will be ignored if lower-case activation
+            function names are provided. This is because in Keras, activation layers are classes with constructors, but activation functions are just functions, and have lower-case
+            names as mentioned earlier. By the way, the slope of the negative section in `LeakyReLU` is `alpha`.
         - `conv_norm_layer_type` (str|list): (list of) types of normalization layers to use in the conv blocks. Examples: 'BatchNormalization', 'LayerNormalization', etc.
-            Defaults to None.
-        - `conv_norm_layer_position` ("before"|"after"|list): (list of) positions of the normalization layers in the 
+            Defaults to None. Instead of a string, it can also be a custom Keras Layer class (not instance).
+        - `conv_norm_layer_position` ("before"|"after"|None|list): (list of) positions of the normalization layers in the 
             convolutional blocks relative to the activation functions. Defaults to "before". If it is a list, it should be a list of strings of the same length as `num_conv_blocks`
-        - `conv_norm_layer_params` (dict|list): (list of) kwargs dict for the convolution normalization layers' constructors. Defaults to None.    
+        - `conv_norm_layer_params` (dict|list): (list of) kwargs dicts for the convolution normalization layers' constructors. Defaults to None.    
         - `conv_dropout` (float|list): (list of) Dropout rates of the convolution blocks. Defaults to None.
-        - `pool_type` (str|list): (list of) types of pooling layer. "Max", "Avg", "GlobalMax", "GlobalAvg", etc. Defaults to None, in which case there will be no pooling layer.
-        - `pool_kernel_size` (int|list): (list of) kernel sizes of the pooling layers, with similar format to 
-            `conv_kernel_size`. Again, it can be a list of integers, a list of tuples of integers, or an integer.
+        - `conv_spatial_dropout` (float|list): (list of) Spatial dropout rates of the convolution blocks. Defaults to None.
+        - `pool_type` (str|list): (list of) types of pooling layers. "Max", "Avg", "GlobalMax", and "GlobalAvg" are acceptable. Defaults to None, in which case there will be no 
+            pooling layer. Insetad of the strings mentioned above, a custom Keras Layer class (not instance) can also be provided. In this case, one should note that the pooling
+            hyperparameters below will be ignored, and the custom pooling layer will be constructed with the `pool_params` kwargs only. Also, in this case, image dimensions will
+            not be calculated for this pooling layer because it is unknown since it is a custom layer.
+        - `pool_kernel_size` (int|list): (list of) kernel sizes of the pooling layers, with similar format to `conv_kernel_size`. Again, it can be a list of integers, where every
+            integer will be broadcasted to all dimensions, a list of tuples of integers for 2D or 3D images, or an integer to be boradcasted across dimensions and conv blocks.
         - `pool_padding` (str|list): (list of) paddings of the pooling layers.
         - `pool_stride` (int|list): (list of) strides of the pooling layers.
         - `pool_params` (dict|list): (list of) kwargs dicts for the pooling layers' constructors.
         - `min_image_size` (int): Minimum size of the image to be reduced to in convolutions and poolings.
             After this point, the padding and striding will be chosen such that image size does not decrease further. Defaults to 1.
+        - `flatten_before_dense` (bool): Whether to flatten the output of the convolutional blocks before the dense blocks. If it is False, all dense layers (if
+            any) will be applied to all pixels, acting on channels. If this argument is not provided, the default will depend on whether there are dense layers after conv layers,
+            in which case `dense_depth` would be greater than 0 and the default would be True, or not, in which case the default would be False since the absence of dense layers
+            negates any reason for flattening. Defaults to None.
             
         #### Dense blocks
         
         - `dense_width` ("auto"|int|list): Width of the hidden layers of the Dense network. "auto", a number (for all of them) or a list holding width of each hidden layer.
             If "auto", it will start with the output size of the Flatten() layer, halving at every Dense block.
-        - `dense_depth` (int): Depth (number of hidden layers) of the Dense network.
-        - `dense_activation` (str|list): (list of) activation function for hidden layers of the Dense network. Examples: 'relu', 'leakyrelu', 'sigmoid', 'tanh', etc.
-        - `dense_activation_params` (dict|list): (list of) dicts for the dense activation functions' constructors.
-        - `output_activation` (str): Activation function for the output layer of the Dense network, if any.
-            **NOTE** Depending on the loss function, you may not need an activation function.
-        - `output_activation_params` (dict): Dictionary of parameters for the output activation function's constructor.
+        - `dense_depth` (int): Depth (number of hidden layers) of the Dense network. `0` will mean no hidden layers, meaning Flatten will be directly followed by the output layer.
+        - `dense_activation` (str|list): (list of) activation function for hidden layers of the Dense network. These can be activation functions ("relu", "sigmoid", "tanh", etc.),
+            activation layers ("ReLU", "LeakyReLU", "Softmax", etc.), or custom Layer classes (not instances). Defaults to None, in which case no activation function will be used.
+        - `dense_activation_params` (dict|list): (list of) dicts for the dense activation functions' constructors. Ignored if lower-case activation functions are provided.
+            By the way, the slope of the negative section in `LeakyReLU` is `alpha`.
         - `dense_norm_layer_type` (str|list): (list of) types of normalization layers to use in the dense blocks. Examples: 'BatchNormalization', 'LayerNormalization', etc.
-            Defaults to None, in which case no normalization layer will be used.
+            Defaults to None, in which case no normalization layer will be used. Instead of strings, custom Keras Layer classes (not instances) can also be provided.
         - `dense_norm_layer_position` ("before"|"after"|list): (list of) positions of the normalization layers in the dense blocks relative to the activation functions. 
             Defaults to "before". If it is a list, it should be a list of strings of the same length as `dense_depth`.
         - `dense_norm_layer_params` (dict|list): (list of) kwargs dict for the dense normalization layers' constructors.
         - `dense_dropout` (float|list): (list of) Dropout rates (if any) for the hidden layers of the Dense network.
+        - `include_output_layer` (bool): Whether to include an output layer. Defaults to True.
+        - `output_activation` (str): Activation (with the same format as dense activation) for the output layer, if any.
+            **NOTE** Depending on the loss function, you may not need an activation function.
+            For classification problems, you may want to choose "sigmoid" or "softmax".
+            That being said, you usually don't need to specify an activation for the output layer at all, if e.g. 'from_logits' is used.
+            For regression problems, no activation is needed. It is by default linear, unless you want to manually specify an activation.
+        - `output_activation_params` (dict): Dictionary of parameters for the output activation function's constructor. Ignored if a lower-case function name is provided.
         
         #### Training procedure
         
         - `batch_size` (int): Minibatch size, the expected input size of the network.
         - `learning_rate` (float): Initial learning rate of training.
-        - `learning_rate_decay_gamma` (float): Exponential decay rate gamma for learning rate, if any.
-        - `optimizer` (str): Optimizer. Examples: 'Adam', 'SGD', 'RMSprop', etc.
-        - `optimizer_params` (dict): Additional parameters of the optimizer, if any.
+        - `exponential_decay_rate` (float): Exponential decay rate gamma for learning rate, if any.
+        - `optimizer` (str): Optimizer. Examples: 'Adam', 'SGD', 'RMSprop', etc. It can be the name of any Keras optimizer.
+        - `optimizer_params` (dict): Additional parameters of the optimizer constructor, if any.
         - `epochs` (int): Maximum number of epochs for training.
-        - `validation_tolerance_epochs` (int): Epochs to tolerate unimproved val loss, before early stopping.
+        - `early_stopping_patience_epochs` (int): Epochs to tolerate unimproved (val) loss, before early stopping.
         - `l2_reg` (float): L2 regularization parameter.
-        - `loss_function` (str): Loss function. Examples: 'mse','categorical_crossentropy',etc.
-        - `loss_function_params` (dict): Additional parameters for the loss function, if any.
-        - `validation_data` (tuple): Validation data, if any. It should be a tuple of (portion, from_dataset). For instance, [0.05, 'testset'] means 5% of the testset will be used 
-            for validation.The second element of the tuple can only be 'trainset' and 'testset'. The first element must be a float between 0 and 1. 
+        - `loss_function` (str): Loss function. Examples: 'mse','categorical_crossentropy', etc. A Keras loss function instance can also be provided rather than a string.
+        - `validation_data` (tuple): Validation data, if any. It should be a tuple of `(portion, from_dataset)`. For instance, `[0.05, 'testset']` means 5% of the testset will be 
+            used for validation. The second element of the tuple can only be `'trainset'` and `'testset'`. The first element must be a float between 0 and 1. 
             If the second element is not specified, testset will be used by default.
-        - `metrics` (list): list of metrics for Keras compilation, e.g. ['accuracy'].
+        - `metrics` (list): list of metrics for Keras compilation, e.g. ['accuracy']. This will be passed directly to Keras compile function, so it can be a list of class instances
+            or a list of strings.
         - `checkpoint_path` (str): Path to the directory where checkpoints will be saved at every epoch.
         - `early_stopping_monitor` (str): Monitor whose critical value will cause early stopping. Default is 'loss', but 'val_loss' is typically used.
         - `early_stopping_mode` (str): Mode of the parameter whose critical value will be used for early stopping. Deafults to 'min' for any error. 'max' is for accuracy, etc.
-        - `early_stopping_value` (float): Value of the monitor at which point training will stop becasue the critical value has been reached.
+        - `early_stopping_value` (float): Value of the monitor at which point training will stop because the critical value has been reached.
         
         ### Returns
         
         - Returns a `tf.keras.models.Model` object that can be trained and used accordingly.
         - Run `net.summary()` afterwards to see what you have inside the network.
         - A `KerasSmartModel` object is returned. This module has its own functions for training, evaluation, etc.
         """
         super(Conv_Network, self).__init__(hparams)
         if not hparams: hparams = self.sample_hparams
         # Input and output shapes
-        self.model_name = hparams["model_name"] if hparams.get("model_name") else "Conv_Network"
+        self._model_name = hparams["model_name"] if "model_name" in hparams else "Conv_Network"
         self._input_shape = hparams["input_shape"]
         self._output_shape = hparams["output_shape"]
-        self._N = int(hparams["batch_size"])
+        self._N = int(hparams["batch_size"]) if "batch_size" in hparams else 32
         self.batch_input_shape = list(self._input_shape).copy()
         self.batch_input_shape.insert(0, self._N)
         self.batch_output_shape = list(self._output_shape).copy()
         self.batch_output_shape.insert(0, self._N)
         self.size_list = [self._input_shape]
     
         # Initialiaing sequential network
-        self.net = tf.keras.models.Sequential()
+        self.net = tf.keras.models.Sequential(name=self._model_name)
         
         # Convolutional layers hyperparameters
-        self._num_conv_blocks = hparams.get("num_conv_blocks")
-        self._conv_dim = hparams.get("conv_dim")
+        self._num_conv_blocks = hparams["num_conv_blocks"]
+        self._conv_dim = hparams["conv_dim"]
         self._conv_params = hparams.get("conv_params")    
         self._conv_channels = hparams.get("conv_channels") if hparams.get("conv_channels") else "auto"
         self._conv_kernel_size = hparams.get("conv_kernel_size") if hparams.get("conv_kernel_size") else 3
         self._conv_padding = hparams["conv_padding"] if hparams.get("conv_padding") else "valid"
         self._conv_stride = hparams["conv_stride"] if hparams.get("conv_stride") else 1
         self._conv_dilation = hparams["conv_dilation"] if hparams.get("conv_dilation") else 1
-        self._conv_activation = hparams["conv_activation"] if hparams.get("conv_activation") else "relu"
+        self._conv_activation = hparams.get("conv_activation")
         self._conv_activation_params = hparams.get("conv_activation_params")
         self._conv_norm_layer_type = hparams.get("conv_norm_layer_type")
         self._conv_norm_layer_position = hparams.get("conv_norm_layer_position")
         self._conv_norm_layer_params = hparams.get("conv_norm_layer_params")
         self._conv_dropout = hparams.get("conv_dropout")
+        self._conv_spatial_dropout = hparams.get("conv_spatial_dropout")
         self._pool_type = hparams.get("pool_type")
-        self._pool_kernel_size = hparams.get("pool_kernel_size") if hparams.get("pool_kernel_size") else 2
+        self._pool_kernel_size = hparams["pool_kernel_size"] if hparams.get("pool_kernel_size") else 2
         self._pool_padding = hparams["pool_padding"] if hparams.get("pool_padding") else 'valid'
         self._pool_stride = hparams["pool_stride"] if hparams.get("pool_stride") else 1
         self._pool_params = hparams.get("pool_params")
         self._min_image_size = hparams["min_image_size"] if hparams.get("min_image_size") else 1        
         
         # Generate lists of hyperparameters for conv/pool layers
         self._conv_channels_vec = self._gen_hparam_vec_for_conv(self._conv_channels, "conv_channels", 
@@ -209,18 +253,19 @@
         self._pool_type_vec = self._gen_hparam_vec_for_conv(self._pool_type, 'pool_type')
         self._pool_params_vec = self._gen_hparam_vec_for_conv(self._pool_params, 'pool_params')
         self._conv_params_vec = self._gen_hparam_vec_for_conv(self._conv_params, 'conv_params')
         self._conv_norm_layer_type_vec = self._gen_hparam_vec_for_conv(self._conv_norm_layer_type, 'conv_norm_layer_type')
         self._conv_norm_layer_params_vec = self._gen_hparam_vec_for_conv(self._conv_norm_layer_params, 'conv_norm_layer_params')
         self._conv_norm_layer_position_vec = self._gen_hparam_vec_for_conv(self._conv_norm_layer_position, 'conv_norm_layer_position')
         self._conv_dropout_vec = self._gen_hparam_vec_for_conv(self._conv_dropout, 'conv_dropout')
+        self._conv_spatial_dropout_vec = self._gen_hparam_vec_for_conv(self._conv_spatial_dropout, 'conv_spatial_dropout')
         
         # Constructing the encoder (convolutional blocks)
         # print("input_shape: ", self._input_shape)
-        in_channels = self._input_shape[-1]
+        # in_channels = self._input_shape[-1]
         input_image = list(self._input_shape[:-1])
         for i in range(self._num_conv_blocks):
             out_channels = self._conv_channels_vec[i]
             # print("in_channels: ", in_channels)
             # print("out_channels: ", out_channels)
             # print("input_image: ", input_image)
             _kwargs = {
@@ -239,83 +284,155 @@
                 'norm_layer_type':self._conv_norm_layer_type_vec[i], 
                 'norm_layer_params':self._conv_norm_layer_params_vec[i], 
                 'pool_type':self._pool_type_vec[i], 
                 'pool_kernel_size':self._pool_kernel_size_vec[i], 
                 'pool_padding':self._pool_padding_vec[i], 
                 'pool_stride':self._pool_stride_vec[i], 
                 'pool_params':self._pool_params_vec[i], 
-                'dropout':self._conv_dropout_vec[i], 
+                'dropout':self._conv_dropout_vec[i],
+                'spatial_dropout':self._conv_spatial_dropout_vec[i], 
                 'min_image_dim':self._min_image_size,
                 'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)
             }
             if i==0:
                 _kwargs.update({'input_shape':self._input_shape})
             d = add_conv_block(**_kwargs)
             self.net = d['model']
             output_image = d['output_image']
             self.size_list.append(output_image+[out_channels])
-            in_channels = out_channels
+            # in_channels = out_channels
             input_image = output_image
             
         # Flattening (Image embedding)
-        self.net.add(tf.keras.layers.Flatten())
-        self._dense_input_size = np.prod(output_image) * out_channels
+        self._dense_depth = hparams.get("dense_depth")
+        self._flatten_before_dense = hparams["flatten_before_dense"] if "flatten_before_dense" in hparams else \
+            (self._dense_depth is not None and self._dense_depth > 0)
+        if self._flatten_before_dense:
+            self.net.add(tf.keras.layers.Flatten())
+            self._dense_input_size = np.prod(output_image) * out_channels
+        else:
+            self._dense_input_size = out_channels
         self.size_list.append([self._dense_input_size])
         
-        # Dense layers hyperparameters
-        self._dense_width = hparams["dense_width"]
-        self._dense_depth = hparams["dense_depth"]
-        self._dense_activation = hparams["dense_activation"] if hparams.get("dense_activation") else "relu"
-        self._dense_activation_params = hparams.get("dense_activation_params")
-        self._output_activation = hparams.get("output_activation") if hparams.get("output_activation") else None
-        self._output_activation_params = hparams.get("output_activation_params")
-        self._dense_norm_layer_type = hparams.get("dense_norm_layer_type")
-        self._dense_norm_layer_params = hparams.get("dense_norm_layer_params")
-        self._dense_norm_layer_position = hparams.get("dense_norm_layer_position")
-        self._dense_dropout = hparams.get("dense_dropout")
-        self._out_activation_module = actdict_keras[self._output_activation] if self._output_activation else None
-        
-        # Generate lists of hyperparameters for the dense layers
-        self._dense_width_vec = self._gen_hparam_vec_for_dense(self._dense_width, 'dense_width',
-            check_auto=True, init_for_auto=self._dense_input_size, powers_of_two_if_auto=True, direction_if_auto="down")
-        self._dense_activation_vec = self._gen_hparam_vec_for_dense(self._dense_activation, 'dense_activation')
-        self._dense_activation_params_vec = self._gen_hparam_vec_for_dense(self._dense_activation_params, 'dense_activation_params')
-        self._dense_norm_layer_type_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_type, 'dense_norm_layer_type')
-        self._dense_norm_layer_params_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_params, 'dense_norm_layer_params')
-        self._dense_norm_layer_position_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_position, 'dense_norm_layer_position')
-        self._dense_dropout_vec = self._gen_hparam_vec_for_dense(self._dense_dropout, 'dense_dropout')
-        
-        # Construct the dense layers
-        in_size = self._dense_input_size
-        for i in range(self._dense_depth):
-            out_size = self._dense_width_vec[i]
-            temp_dropout_rate = self._dense_dropout_vec[i] if (i != self._dense_depth-1) else None # The hidden layer just before the output layer rarely has Dropout.
-            _kwargs = {
-                'model':self.net,
-                'output_size':self._dense_width_vec[i],
-                'activation':self._dense_activation_vec[i],
-                'activation_params':self._dense_activation_params_vec[i],
-                'norm_layer_type':self._dense_norm_layer_type_vec[i],
-                'norm_layer_position':self._dense_norm_layer_position_vec[i],
-                'norm_layer_params':self._dense_norm_layer_params_vec[i],
-                'dropout':temp_dropout_rate,
-                'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)
-            }
-            add_dense_block(**_kwargs)
-            in_size = out_size
-            self.size_list.append([out_size])
-        
-        # Output layer
-        self.net.add(tf.keras.layers.Dense(self._output_shape[-1]))
-        if self._output_activation:
-            if self._output_activation_params: self.net.add(tf.keras.layers.Activation(self._out_activation_module(**self._output_activation_params)))
-            else: self.net.add(tf.keras.layers.Activation(self._out_activation_module))
+        # Check to see if we will have dense layers
+        if self._dense_depth is not None and self._dense_depth > 0:
+            
+            # Dense layers hyperparameters
+            self._dense_width = hparams.get("dense_width")
+            self._dense_activation = hparams.get("dense_activation")
+            self._dense_activation_params = hparams.get("dense_activation_params")
+            self._dense_norm_layer_type = hparams.get("dense_norm_layer_type")
+            self._dense_norm_layer_params = hparams.get("dense_norm_layer_params")
+            self._dense_norm_layer_position = hparams.get("dense_norm_layer_position")
+            self._dense_dropout = hparams.get("dense_dropout")
+            
+            # Generate lists of hyperparameters for the dense layers
+            self._dense_width_vec = self._gen_hparam_vec_for_dense(self._dense_width, 'dense_width',
+                check_auto=True, init_for_auto=self._dense_input_size, powers_of_two_if_auto=True, direction_if_auto="down")
+            self._dense_activation_vec = self._gen_hparam_vec_for_dense(self._dense_activation, 'dense_activation')
+            self._dense_activation_params_vec = self._gen_hparam_vec_for_dense(self._dense_activation_params, 'dense_activation_params')
+            self._dense_norm_layer_type_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_type, 'dense_norm_layer_type')
+            self._dense_norm_layer_params_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_params, 'dense_norm_layer_params')
+            self._dense_norm_layer_position_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_position, 'dense_norm_layer_position')
+            self._dense_dropout_vec = self._gen_hparam_vec_for_dense(self._dense_dropout, 'dense_dropout')
+            
+            # Construct the dense layers
+            # in_size = self._dense_input_size
+            if self._dense_depth > 0:
+                for i in range(self._dense_depth):
+                    out_size = self._dense_width_vec[i]
+                    _kwargs = {
+                        'model':self.net,
+                        'output_size':self._dense_width_vec[i],
+                        'activation':self._dense_activation_vec[i],
+                        'activation_params':self._dense_activation_params_vec[i],
+                        'norm_layer_type':self._dense_norm_layer_type_vec[i],
+                        'norm_layer_position':self._dense_norm_layer_position_vec[i],
+                        'norm_layer_params':self._dense_norm_layer_params_vec[i],
+                        'dropout': self._dense_dropout_vec[i],
+                        'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)
+                    }
+                    add_dense_block(**_kwargs)
+                    # in_size = out_size
+                    self.size_list.append([out_size])
+        
+        
+        
+        # Check to see if there will be an output layer
+        self._include_output_layer = hparams.get("include_output_layer")
+        
+        if self._include_output_layer:
+            # Output hyperparameters
+            self._output_activation = hparams.get("output_activation")
+            self._output_activation_params = hparams.get("output_activation_params")
+        
+            # Output layer
+            self.net.add(tf.keras.layers.Dense(self._output_shape[-1], kernel_regularizer=(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)))
+            if self._output_activation:
+                if isinstance(self._output_activation, str):
+                    if self._output_activation.lower() == self._output_activation:
+                        self.net.add(tf.keras.layers.Activation(self._output_activation))
+                    elif self._output_activation_params:
+                        self.net.add(getattr(tf.keras.layers, self._output_activation)(**self._output_activation_params))
+                    else:
+                        self.net.add(getattr(tf.keras.layers, self._output_activation)())
+                elif self._output_activation_params:
+                    self.net.add(self._output_activation(**self._output_activation_params))
+                else:
+                    self.net.add(self._output_activation())
 
     
     def _gen_hparam_vec_for_conv(self, hparam, hparam_name, **kwargs):
         return generate_array_for_hparam(hparam, self._num_conv_blocks, hparam_name=hparam_name, count_if_not_list_name='num_conv_blocks', **kwargs)
     
     def _gen_hparam_vec_for_dense(self, hparam, hparam_name, **kwargs):
         return generate_array_for_hparam(hparam, self._dense_depth, hparam_name=hparam_name, count_if_not_list_name='dense_depth', **kwargs)
     
     def call(self, inputs, **kwargs):
         return self.net(inputs, **kwargs)
+
+
+
+
+
+if __name__ == '__main__':
+    # Test Conv_Network
+    print("Minimal example with only convolution layers and no dense or output layers:")
+    sample_hparams = {
+        "model_name": "Conv_Network",
+        # I/O shapes (without the batch dimension)
+        "input_shape": [28, 28, 3],
+        "output_shape": [10],
+        # Convolution blocks
+        "num_conv_blocks": 2,
+        "conv_dim": 2,
+        "conv_params": None,
+        "conv_channels": "auto",
+        "conv_kernel_size": 3,
+        "conv_padding": "valid",
+        "conv_stride": 1,
+        "conv_dilation": 1,
+        "conv_activation": "LeakyReLU",
+        "conv_activation_params": {'alpha':0.1},
+        "conv_norm_layer_type": "BatchNormalization",
+        "conv_norm_layer_position": ["before", "after"],
+        "conv_norm_layer_params": None,
+        "conv_dropout": [0.1, None],
+        "conv_spatial_dropout": None,
+        "pool_type": "Max",
+        "pool_kernel_size": 2,
+        "pool_padding": 'valid',
+        "pool_stride": 1,
+        "pool_params": None,
+        "min_image_size": 4
+    }
+    model = Conv_Network(sample_hparams)
+    model.summary()
+    print("Trying with sample data ...")
+    y = model(tf.random.normal([32, 28, 28, 3]))
+    print("Output shape:", y.shape)
+    
+    
+    print("")
+    print("Testing full example with convolution layers, dense layers and output layer:")
+    test_keras_model_class(Conv_Network)
+
```

### Comparing `eznet_keras-0.0.3/eznet_keras/models/keras_smart_module.py` & `eznet_keras-1.0.0/eznet_keras/models/keras_smart_module.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     
     sample_hparams = {
         'model_name': 'KerasSmartModel',
         'l2_reg': 0.0001,
         'batch_size': 16,
         'epochs': 2,
         'validation_data': 0.1,
-        'validation_tolerance_epochs': 10,
+        'early_stopping_patience_epochs': 10,
         'learning_rate': 0.0001,
-        'learning_rate_decay_gamma': 0.99,
+        'exponential_decay_rate': 0.99,
         'loss_function': 'categorical_crossentropy',
         'loss_function_params': None,
         'metrics':['accuracy'],
         'optimizer': 'Adam',
         'optimizer_params': None,
         'checkpoint_path':None,
         'early_stopping_monitor':'loss',
@@ -38,70 +38,72 @@
 
         ### Usage
 
         `net = KerasSmartModel(hparams)` where `hparams` is dictionary of hyperparameters containing the following:
             - `model_name` (str): Name of the model.
             - `batch_size` (int): Minibatch size, the expected input size of the network.
             - `learning_rate` (float): Initial learning rate of training.
-            - `learning_rate_decay_gamma` (float): Exponential decay rate gamma for learning rate, if any.
-            - `optimizer` (str): Optimizer. Examples are "Adam", "SGD", "RMSprop", "Adagrad", etc.
-            - `optimizer_params` (dict): Additional parameters of the optimizer, if any.
+            - `exponential_decay_rate` (float): Exponential decay rate for learning rate, if any.
+            - `optimizer` (str): Optimizer. Examples are "Adam", "SGD", "RMSprop", "Adagrad", etc. The name of any Keras optimizer can be used.
+            - `optimizer_params` (dict): Additional parameters of the optimizer constructor, if any.
             - `epochs` (int): Maximum number of epochs for training.
-            - `validation_tolerance_epochs` (int): Epochs to tolerate unimproved val loss, before early stopping (patience).
+            - `early_stopping_patience_epochs` (int): Epochs to tolerate unimproved (val) loss, before early stopping (i.e., patience).
             - `l2_reg` (float): L2 regularization parameter.
-            - `loss_function` (str): Loss function. Examples: "MSELoss", "CrossEntropyLoss", "NLLLoss", etc.
-            - `loss_function_params` (dict): Additional parameters for the loss function, if any.
-            - `metrics` (list): list of metrics for Keras compilation.
+            - `loss_function` (str): Loss function. Examples: "mse", "binary_crossentropy", "categorical_crossentropy", etc. It can also be a Keras loss function instance.
+            - `metrics` (list): list of metrics for Keras compilation. Examples: ['mse'], ['accuracy'], etc. It can also be a Keras metric instance.
             - `checkpoint_path` (str): Path to the directory where checkpoints will be saved at every epoch.
             - `early_stopping_monitor` (str): Monitor whose critical value will cause early stopping. Default is 'loss', but 'val_loss' is typically used.
             - `early_stopping_mode` (str): Mode of the parameter whose critical value will be used for early stopping. Deafults to 'min' for any error. 'max' is for accuracy, etc.
             - `early_stopping_value` (float): Value of the monitor at which point training will stop becasue the critical value has been reached.
 
         ### Returns
 
         Returns a `tf.keras.models.Model` object that can be trained and used accordingly.
         Run `net.summary()` afterwards to see what you have inside the network.
         
         ### Notes:
+        
         - `self.batch_input_shape` attribute must be set in the `__init__` method.
         - `self.batch_output_shape` attribute must be set in the `__init__` method.
         - `self._callbacks` is a list of callbacks sent to the training method of Keras. It already includes garbage collection.
         - `self._es` is an EarlyStopping instance of Keras, if specified, otherwise None.
         - `self._chkpt` is the hyperparameter `checkpoint_path` from the input dictionary, if it exists, otherwise None.
         - `self._chk` is a ModelCheckpoint instance sent to the training function of Keras, if specified, otherwise None.
         - `self._es_crit` is an EarlyStopAtCriteria instance that stops the training if 'val_loss' for instance, reaches a certain value.
         - `self.net` **MUST** always exist so that Keras2Cpp can serialize the layers that it understands.
           `self.net` is always used as the model within this module, that contains the network itself. It is typically a Sequential or Functional model built in the `__init__` 
           method.
         """
         super(KerasSmartModel, self).__init__()
         if not hparams: hparams = self.sample_hparams
         self.hparams = hparams
-        self._batch_size = int(hparams["batch_size"])
+        self._batch_size = int(hparams["batch_size"]) if hparams.get("batch_size") else 32
         self._loss_function = hparams.get("loss_function")
-        self._loss_function_params = hparams.get("loss_function_params")
+        # self._loss_function_params = hparams.get("loss_function_params")
         self._metrics_list = hparams.get("metrics")
         self._optimizer = hparams.get("optimizer")
         self._optimizer_params = hparams.get("optimizer_params")
-        self._validation_tolerance_epochs = hparams.get("validation_tolerance_epochs")
+        self._early_stopping_patience_epochs = hparams.get("early_stopping_patience_epochs")
         self._learning_rate = hparams.get("learning_rate")
-        self._learning_rate_decay_gamma = hparams.get("learning_rate_decay_gamma")
+        self._exponential_decay_rate = hparams.get("exponential_decay_rate")
         self._validation_data = hparams.get("validation_data")
         self._epochs = hparams.get("epochs")
         self._l2_reg = hparams.get("l2_reg") if hparams.get("l2_reg") else 0.0
         self.history = None
         self.batch_input_shape = (self._batch_size, 1)
         self.batch_output_shape = (self._batch_size, 1)
         self._callbacks = [GarbageCollectionCallback()]
-        self._es = tf.keras.callbacks.EarlyStopping(monitor='val_loss', mode="min", patience=self._validation_tolerance_epochs) if self._validation_tolerance_epochs else None
+        self._es = tf.keras.callbacks.EarlyStopping(monitor='val_loss' if 'validation_data' in hparams else 'loss', 
+                                                    mode="min", patience=self._early_stopping_patience_epochs) if self._early_stopping_patience_epochs else None
         if self._es:
             self._callbacks.append(self._es)
         self._chkpt = hparams.get("checkpoint_path")
         if self._chkpt:
-            self._chk = tf.keras.callbacks.ModelCheckpoint(self._chkpt, monitor='val_loss', verbose=0, save_best_only=True, mode='min')
+            self._chk = tf.keras.callbacks.ModelCheckpoint(self._chkpt, monitor=('val_loss' if 'validation_data' in hparams else 'loss'), 
+                                                           verbose=0, save_best_only=True, mode='min')
         else:
             self._chk = None
         if self._chk:
             self._callbacks.append(self._chk)
         self.early_stopping_monitor = hparams.get("early_stopping_monitor")
         self.early_stopping_mode = hparams.get("early_stopping_mode")
         self.early_stopping_value = hparams.get("early_stopping_value")
@@ -112,68 +114,107 @@
             self._es_crit = None
         self.net = tf.keras.models.Sequential()
     
     
     def call(self, x, *args, **kwargs):
         return self.net(x, *args, **kwargs)
     
-    def build(self):
-        super().build(input_shape=self.batch_input_shape) 
+    # def build(self):
+    #     super().build(input_shape=self.batch_input_shape) 
         
     def summary(self):
         return self.net.summary()
         
     def get_config(self):
         config = super(KerasSmartModel, self).get_config()
         config['hparams'] = self.hparams
         return config
     
     @classmethod
     def from_config(cls, config):
         return cls(config['hparams'])
     
-    def compile(self, num_samples=None):
+    def compile_model(self, num_samples=None):
+        """Compiles Keras Smart Model based on its constructor hyperparameters
+
+        Args:
+            num_samples (int, optional): Number of samples. Defaults to None.
+        """
         compile_keras_model(self.net, self._batch_size, self._learning_rate, self._optimizer, self._loss_function, 
-                              self._metrics_list, self._optimizer_params, self._learning_rate_decay_gamma, num_samples)
+                              self._metrics_list, self._optimizer_params, self._exponential_decay_rate, num_samples)
+            
+    def fit_model(self, x_train, y_train, x_val=None, y_val=None, verbose:int=1, **kwargs):
+        """Fit (train) the Keras Smart Model to training data.
+
+        Args:
+            x_train (array): Training inputs
+            y_train (array): Training target outputs
+            x_val (array, optional): Validation inputs. Defaults to None.
+            y_val (array, optional): Validation target outputs. Defaults to None.
+            verbose (int, optional): Verbosity passed to the Keras Fit function. Defaults to 1.
             
-    def fit(self, x_train, y_train, x_val, y_val, verbose:bool=True, **kwargs):
+            Other keyword arguments are passed to the Keras fit function.
+
+        Returns:
+            History object returned by the Keras fit function
+        """
         self.history = fit_keras_model(self.net, x_train, y_train, x_val, y_val, 
             self._batch_size, self._epochs, self._callbacks, verbose, **kwargs)
         return self.history
 
     def __str__(self):
         s = "KerasSmartModel with the following attributes:\n" + str(self.hparams)
         return s
     
-    def train(self, x_train, x_val, y_train, y_val, verbose:bool=True, saveto:str=None, export:str=None, **kwargs):
+    def train_model(self, x_train, y_train, x_val=None, y_val=None, verbose:int=1, saveto:str=None, export:str=None, **kwargs):
         """Train the model according to its hyperparameters.
 
         ### Args:
             - `x_train` (numpy array): Training inputs
-            - `x_val` (numpy array): Validation inputs
             - `y_train` (numpy array): Training target outputs
+            - `x_val` (numpy array): Validation inputs
             - `y_val` (numpy array): Validation target outputs
-            - `verbose` (bool, optional): Verbosity of training. Defaults to True.
+            - `verbose` (int, optional): Verbosity of training passed to Keras fit function. Defaults to 1.
             - `saveto` (str, optional): Save Keras model in path. Defaults to None.
             - `export` (str, optional): Save Keras model in .model file using keras2cpp for later use in C++. Defaults to None.
+            
+            Other keyword arguments are passed to the Keras fit function.
 
         ### Returns:
             Nothing. It modifies the "net" attribute of the model, and the history of the training in self.history.
         
         """
         N = x_train.shape[0]
-        self.compile(num_samples=N)
-        _ = self.fit(x_train, y_train, x_val, y_val, verbose=verbose, **kwargs)
+        self.compile_model(num_samples=N)
+        _ = self.fit_model(x_train, y_train, x_val, y_val, verbose=verbose, **kwargs)
         if saveto:
             save_keras_model(self.net, self.history.history, saveto, self.hparams)
         if export:
             export_keras_model(self.net, export)
 
-    def plot_history(self, metrics=['loss','val_loss'], fig_title='model loss', saveto:str=None):
-        plot_keras_model_history(self.history.history, metrics, fig_title, saveto)
+    def plot_history(self, metrics=['loss'], fig_title='model loss', saveto:str=None, close_after_finish:bool=True):
+        """Plot the training history of the model after training is done.
+
+        ### Args:
+            - `metrics` (list, optional): Metrics list. Defaults to ['loss']. It can also be ['loss','val_loss'] if validation data was provided, or ['accuracy','val_accuracy'].
+            - `fig_title` (str, optional): Title of the figure. Defaults to 'model loss'.
+            - `saveto` (str, optional): Path to where to save the figure. Defaults to None. Path does not need to exist.
+            - `close_after_finish` (bool, optional): Clsoe the figure after saving it with `plt.close()`. Defaults to True. Only applicable if `saveto` is provided.
+        """
+        plot_keras_model_history(self.history.history, metrics, fig_title, saveto, close_after_finish)
         
-    def evaluate(self, *args, **kwargs):
-        return self.net.evaluate(*args, **kwargs)
-    
-    def predict(self, *args, **kwargs):
-        return self.net.predict(*args, **kwargs)
+    # def evaluate(self, *args, **kwargs):
+    #     """Evaluate model performance on test data.
+
+    #     Returns:
+    #         The same thing that Keras evaluate returns.
+    #     """
+    #     return self.net.evaluate(*args, **kwargs)
+    
+    # def predict(self, *args, **kwargs):
+    #     """Predict the outputs given inputs
+
+    #     Returns:
+    #         Teh same thing that Keras predict returns.
+    #     """
+    #     return self.net.predict(*args, **kwargs)
```

### Comparing `eznet_keras-0.0.3/eznet_keras/models/recurrent_network.py` & `eznet_keras-1.0.0/eznet_keras/models/ann.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,240 +1,269 @@
 if __package__=="eznet_keras.models":
-    from ..utils import *
     from .keras_smart_module import *
     from .dense_block import *
 else:
-    import os, sys
-    current_dir = os.path.dirname(os.path.abspath(__file__))
-    parent_dir = os.path.dirname(current_dir)
-    sys.path.append(parent_dir)
-    sys.path.append(current_dir)
-    from utils import *
+    import sys, os
+    sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
     from keras_smart_module import *
     from dense_block import *
 
+import warnings
 
-class Recurrent_Network(KerasSmartModel):
+class ANN(KerasSmartModel):
     
     sample_hparams = {
-        'model_name': 'Recurrent_Network',
-        'in_features': 10,
-        'out_features': 3,
-        'in_seq_len': 13,
-        'out_seq_len': 1,
-        'rnn_type': 'LSTM',
-        'rnn_hidden_sizes': 8,
-        'rnn_bidirectional': False,
-        'rnn_depth': 2,
-        'rnn_dropout': 0.1,
-        'rnn_params': None,
-        'final_rnn_return_sequences': False,
-        'apply_dense_for_each_time_step': True,
-        'permute_output': False,
-        'dense_width': 16,
-        'dense_depth': 2,
-        'dense_dropout': 0.2,
-        'dense_activation': 'relu',
-        'dense_activation_params': None,
-        'output_activation': None,
-        'output_activation_params': None,
-        'norm_layer_type': 'BatchNormalization',
-        'norm_layer_params': None,
-        'norm_layer_position': 'before',
-        'l2_reg': 0.0001,
-        'batch_size': 16,
-        'epochs': 2,
-        'validation_data': [0.05,'testset'],
-        'validation_tolerance_epochs': 10,
-        'learning_rate': 0.0001,
-        'learning_rate_decay_gamma': 0.99,
-        'loss_function': 'categorical_crossentropy',
-        'loss_function_params': None,
-        'metrics':['accuracy'],
+        # General and I/O parameters
+        "model_name": "ANN",
+        "input_shape": [10],
+        "output_size": 3,
+        # Architecture parameters
+        "width": 32,
+        "depth": 2,
+        "hidden_activation": "LeakyReLU",
+        "hidden_activation_params": {'alpha': 0.1},
+        "norm_layer_type":"BatchNormalization",
+        "norm_layer_position": "before",
+        "norm_layer_params": None,
+        "dropout": 0.2,
+        "include_output_layer": True,
+        "output_activation": "Softmax",
+        "output_activation_params": None,
+        # Training procedure parameters
+        "learning_rate": 0.001,
+        "exponential_decay_rate": 0.9,
+        "batch_size": 32,
+        "epochs": 2,
+        "early_stopping_patience_epochs": 2,
+        "validation_data": [0.05,'trainset'],
+        "l2_reg": 0.0001,
+        "loss_function": "categorical_crossentropy",
         'optimizer': 'Adam',
         'optimizer_params': None,
-        'checkpoint_path':None,
-        'early_stopping_monitor':'loss',
-        'early_stopping_mode':'min',
-        'early_stopping_value':1.0e-6
+        'metrics': ['accuracy'],
+        'checkpoint_path': None,
+        'early_stopping_monitor': 'loss',
+        'early_stopping_mode': 'min',
+        'early_stopping_value': 1.0e-6
     }
     
+    
     def __init__(self, hparams:dict=None):
-        """Sequence to Dense network with RNN for time-series classification, regression, and forecasting, as well as NLP applications.
-        This network uses any RNN layers as encoders to extract information from input sequences, and fully-connected 
-        multilayer perceptrons (Dense) to decode the sequence into an output, which can be class probabilitites 
-        (timeseries classification), a continuous number (regression), or an unfolded sequence (forecasting) of a 
-        target timeseries.
-
+        """Typical Artificial Neural Network class, also known as multilayer perceptron. This class will create a fully connected feedforward artificial neural network.
+        It can be used for classification, regression, etc. It basically encompasses enough options to build all kinds of serial ANNs with any number of 
+        inputs, outputs, layers with custom or arbitrary width or depth, etc. Supports multiple activation functions for hidden layers and the output layer. The netwrok consists
+        of many `Dense_Block` layers, each consisting of a linear (dense) layer, followed optionally by a normalization, activation, and dropout layers. There is optionally an 
+        output layer after all the `Dense_Block` instances. This class can be used for making virtually any kind of serial MLP. No parallelism or skip connections are supported
+        in this calss yet.
+        
         ### Usage
+        
+        `net = ANN(hparams)` where `hparams` is the dictionary of hyperparameters.
+        
+        - Inspect the `sample_hparams` class attribute to find a complete sample of hyperparameters dictionary.
+        - The training procedure section of the hyperparameters is the same as in `KerasSmartModel` class, and is only used in training. Otherwise, it is not necessary for building
+          the model itself.
+        - Many hyperparameters, especially those that have a (list of) in their description below, can be either None, in which case that item will not be included, or a scalar
+          value which will be broadcasted to all dense blocks, or a list with the same length as the `depth` hyperparameter, in which case each item will be used for the 
+          corresponding dense block. Use None for any dense block for which an item or hyperparameter should not be included or applied.
+        - Every `Dense_Block` by default is assumed to have a dense layer, followed by a normalization, activation, and dropout layers. We also assume that there will be an output
+          layer at the end, unless `include_output_layer` hyperparameter is set to `False`. Normalization layer can come `before` or `after` the activation.
+        - Activation functions come from `tf.keras.activations` and need to be wrapped in a `tf.keras.layers.Activation` layer, and do not accept any kwargs. Activation layers
+          come from `tf.keras.layers`, can accept kwargs in their constructors, and do not need to be wrapped in an `Activation` layer. Activation functions all have lower-case
+          names, but activation layers are classes and have every-word-capitalized names. We will use this as a clue to recognize what the user wants, and perform accordingly.
+          Most activation layers also have correpsonding activation functions (like `tf.keras.activations.relu` function and `tf.keras.layers.ReLU` layer). 
+          However, some activations are only available as functions (such as `tf.keras.activations.sigmoid`), and some are only available as layers 
+          (such as `tf.keras.layers.LeakyReLU`). Choose accordingly.
 
-        `net = Recurrent_Network(hparams)` where `hparams` is dictionary of hyperparameters containing the following:
+        The hyperparameters dictionary should include the following keys:
         
-            - `model_name` (str): Name of the model, can be used later for saving, etc.
-            - `rnn_type` (str): RNN type, options are "LSTM", "GRU", "SimpleRNN", etc.
-            - `in_seq_len` (int): Input sequence length, in number of timesteps
-            - `out_seq_len` (int): Output sequence length, in number of timesteps, assuming output is also a sequence. This will affect the output layer in the dense section.
-                Use 1 for when the output is not a sequence, or do not supply this key.
-            - `in_features` (int): Number of features of the input.
-            - `out_features` (int): Number of features of the output.
-            - `rnn_hidden_sizes` (int): RNN layer hidden size. A number sets them all the same. Default is 16.
-            - `rnn_bidirectional` (bool): Whether the RNN layers are bidirectional or not. Default is False.
-            - `rnn_depth` (int): Number of stacked RNN layers. Default is 1.
-            - `rnn_dropout` (float): Dropout rates, if any, of the RNN layers. 
-                Please note that using dropout in RNN layers is generally discouraged, for it decreases determinism during inference.
-            - `rnn_params` (dict): Dictionary of kwargs for the RNN layer constructor. Default is None.
-              If specified, the keys in this dictionary will not only add to, but also overwrite any existing arguments this class passes to the RNN layer constructor.
-            - `final_rnn_return_sequences` (bool): Whether the final RNN layer returns sequences of hidden state. 
-                **NOTE** Setting this to True will make the model much, much larger.
-            - `apply_dense_for_each_time_step` (bool): Whether to apply the Dense network to each time step of the 
-                RNN output. If False, the Dense network is applied to the last time step only if 
-                `final_rnn_retrurn_sequences` is False, or applied to a flattened version of the output sequence
-                otherwise (the dimensionality of the input feature space to the dense network will be multiplied
-                by the sequence length. PLEASE NOTE that this only works if the entered sequence is exactly as long
-                as the priorly defined sequence length according to the hyperparameters).
-            - `permute_output` (bool): Whether to permute the output sequence to be (N, D*H_out, L_out)
-            - `dense_width` (int|list): (list of) Widths of the Dense network. It can be a number (for all) or a list holding width of each hidden layer.
-            - `dense_depth` (int): Depth (number of hidden layers) of the Dense network.
-            - `dense_activation` (str|list): (list of) Activation functions for hidden layers of the Dense network. Examples: "relu", "leaklyrelu", "sigmoid", "tanh", etc.
-            - `dense_activation_params` (dict|list): (list of) Dictionaries of parameters for the activation func constructors of the Dense network.
-            - `output_activation` (str): Activation function for the output layer of the Dense network, if any. Examples: "softmax", "sigmoid", etc.
-                **NOTE** If the loss function is `sparse_categorical_crossentropy`, then no output activation is erquired.
-                However, if the loss function is `categorical_crossentropy` (a.k.a. negative loglikelihood), then you must specify an output activation as in "softmax".
-            - `output_activation_params` (dict): Dictionary of parameters for the activation func constructor of the output layer.
-            - `norm_layer_type` (str|list): (list of) Types of normalization layers to use in the dense section, if any. Options are "BatchNormalization", "LayerNormalization",etc.
-            - `norm_layer_params` (dict|list): (list of) Dictionaries of parameters for the normalization layer constructors.
-            - `norm_layer_position` (str|list): (list of) Whether the normalization layer should come 'before' or 'after' the activation of each hidden layer in the dense network.
-            - `dense_dropout` (float|list): (list of) Dropout rates (if any) for the hidden layers of the Dense network.
-            - `batch_size` (int): Minibatch size, the expected input size of the network.
+            - `input_shape` (list): shape of the input layer minus the batch size. It can have any number of elements. In higher dimensionalities the dense layer will be applied to
+                all feature maps, such that only the last dimension will change. An input of `[batch, dim1, dim2, in_dim]` will come out as `[batch, dim1, dim2, layer_size]`
+                from a dense block.
+            - `output_size` (int): number of outputs to predict, i.e. size of the output layer, if there is going to be an output layer.
+            - `width` (int|list): (list of) hidden layer widths. 
+                a number sets them all the same, and a list/array sets each hidden layer according to the list.
+            - `depth` (int): Specifies the depth of the network (number of hidden layers).
+                It must be specified unless `width` is provided as a list. Then the depth will be inferred form it.
+            - `hidden_activation` (str): (list of) Activations. It can be an activation function name ("relu","sigmoid","tanh", etc.), an activation layer name ("ReLU", 
+                "LeakyReLU", "Softmax", etc.), or a custom Keras Layer class (not instance). Defaults to None.
+            - `hidden_activation_params` (dict): (list of) kwargs parameters for the hidden layer activation constructor, if any. Ignored for any dense block if the activation is
+                provided as a lower-case function name. By the way, the slope of the negative section in `LeakyReLU` is `alpha`. Defaults to None.
+            - `norm_layer_type` (str): (list of) Types of normalization layers to use for each hidden layer. Options are "BatchNormalization", "LayerNormalization", etc.
+                This can also be a Keras Layer class (not instance) rather than a string. Defaults to None.
+            - `norm_layer_position` (str): (list of) where the normalization layer should be included relative to the activation function (if any), 'before' or 'after'.
+            - `norm_layer_params` (dict): (list of) Dictionaries of kwargs parameters for the normalization layers' constructors. Defaults to None.
+            - `dropout` (float): (list of) the dropout rates after every hidden layer. It should be a probability value between 0 and 1, or None by default.
+            - `include_output_layer` (bool): Whether to include an output layer at the end of the network. Defaults to True.
+            - `output_activation` (str): Activation of the output layer, if any. Defaults to None.
+                For classification problems, you may want to choose "sigmoid" or "softmax".
+                That being said, you usually don't need to specify an activation for the output layer at all, if e.g. 'from_logits' is used.
+                For regression problems, no activation is needed. It is by default linear, unless you want to manually specify an activation.
+            - `output_activation_params` (dict): Parameters for the output activation function, if any. Ignored if lower-case function name is provided for activation.
+                Defaults to None.
             - `learning_rate` (float): Initial learning rate of training.
-            - `learning_rate_decay_gamma` (float): Exponential decay rate gamma for learning rate, if any.
-            - `optimizer` (str): Optimizer. Examples: 'Adam', 'SGD', 'RMSProp', etc.
-            - `optimizer_params` (dict): Additional parameters of the optimizer, if any.
+            - `exponential_decay_rate` (float): Exponential decay rate for learning rate, if any. Defaults to None.
+            - `optimizer` (str): Optimizer. Examples: "Adam", "SGD" ,"RMSProp", etc. The name of any optimizer class in `tf.keras.optimizers` can be used, or a custom class.
+            - `optimizer_params` (dict): Additional parameters of the optimizer, if any. Defaults to None.
+            - `batch_size` (int): Minibatch size for training.
             - `epochs` (int): Maximum number of epochs for training.
-            - `validation_tolerance_epochs` (int): Epochs to tolerate unimproved val loss, before early stopping.
-            - `validation_data` (list): Portion of validation data. Should be a tuple like [validation split, dataset as in 'trainset' or 'testset']
-            - `l2_reg` (float): L2 regularization parameter.
-            - `loss_function` (str): Loss function. Examples: 'binary_crossentropy', 'categorical_crossentropy', 'mse', etc.
-            - `loss_function_params` (dict): Additional parameters for the loss function, if any.
-            - `metrics` (list): list of metrics for Keras compilation.
+            - `early_stopping_patience_epochs` (int): Epochs to tolerate unimproved (val) loss, before early stopping.
+            - `validation_data` (list): List of [validation_split, 'trainset'|'testset']. Defaults to None.
+            - `l2_reg` (float): L2 regularization parameter. Defaults to None.
+            - `loss_function` (str): Loss function. Examples: "mse","binary_crossentropy", "categorical_crossentropy", etc. It can also be a loss function instance.
+            - `metrics` (list): list of metrics for Keras compilation, e.g. ['accuracy'].
             - `checkpoint_path` (str): Path to the directory where checkpoints will be saved at every epoch.
             - `early_stopping_monitor` (str): Monitor whose critical value will cause early stopping. Default is 'loss', but 'val_loss' is typically used.
             - `early_stopping_mode` (str): Mode of the parameter whose critical value will be used for early stopping. Deafults to 'min' for any error. 'max' is for accuracy, etc.
             - `early_stopping_value` (float): Value of the monitor at which point training will stop becasue the critical value has been reached.
+        
+        Note that for all such hyperparameters that have a (list of) at the beginning, the entry can be a single item repeated for all hidden layers, or it can be a list of items
+        for all hidden layers. If a list is provided, it must have the same length as the depth of the network. 
+        
+        Also note that depth does not include the input and output layers.
+        This gives you the ability to specify different width, dropout rate, normalization layer and its parameters, and so forth.
 
         ### Returns
         
-        Returns a `tf.keras.models.Model` object that can be trained and used accordingly.
-        Run `net.summary()` afterwards to see what you have inside the network.
-        The returned model is an instance of `KerasSmartModel`, which has built-in functions for training, evaluation, etc.
+        It returns a `tf.keras.models.Model` object that corresponds with an ANN model.
+        run `net.summary()` afterwards to see what the ANN holds.
+        The returned module is a `KerasSmartModel` instance, which is a subclass. It has built-in functions for training, evaluation, etc.
         """
-        super(Recurrent_Network, self).__init__(hparams)
-        hparams = hparams if hparams is not None else self.sample_hparams
-        self._rnn_type = hparams["rnn_type"]
-        self._rnn = getattr(tf.keras.layers, self._rnn_type)
-        self._denseactivation = hparams["dense_activation"] if hparams.get("dense_activation") else "relu"
-        self._denseactivation_params = hparams.get("dense_activation_params")
-        self._outactivation = hparams.get("output_activation")
-        self._outactivation_params = hparams.get("output_activation_params")
-        self._normlayer_type = hparams.get("norm_layer_type")
-        self._normlayer_params = hparams.get("norm_layer_params")
-        self._normlayer_position = hparams.get("norm_layer_position")
-        self._infeatures = hparams["in_features"]
-        self._outfeatures = hparams["out_features"]
-        self._rnnhidsizes = hparams["rnn_hidden_sizes"] if hparams.get("rnn_hidden_sizes") else 16
-        self._densehidsizes = hparams["dense_width"] if hparams.get("dense_width") else 16
-        self._densedepth = hparams["dense_depth"] if hparams.get("dense_depth") else 0
-        self._rnndepth = hparams["rnn_depth"] if hparams.get("rnn_depth") else 1
-        self._bidirectional = True if hparams.get("rnn_bidirectional") else False
-        self._rnndropout = hparams["rnn_dropout"] if hparams.get("rnn_dropout") else 0
-        self._densedropout = hparams["dense_dropout"] if hparams.get("dense_dropout") else None
-        self._final_rnn_return_sequences = True if hparams.get("final_rnn_return_sequences") else False
-        self._apply_dense_for_each_timestep = True if hparams.get("apply_dense_for_each_timestep") else False
-        self._permute_output = True if hparams.get("permute_output") else False
-        self._N = int(hparams["batch_size"])
-        self._L_in = int(hparams["in_seq_len"])
-        self._L_out = int(hparams["out_seq_len"]) if hparams.get("out_seq_len") else 1
-        self._D = int(2 if self._bidirectional else 1)
-        self._rnn_params = hparams.get("rnn_params")
-        self._H_in = int(self._infeatures)
-        if self._rnnhidsizes == "auto": self._H_cell = int(2**(np.round(math.log2(self._H_in*self._L_in))))
-        else: self._H_cell = int(self._rnnhidsizes)
-        self._H_out = int(self._H_cell)
-        self.batch_input_shape = (self._N, self._L_in, self._H_in)
-        if self._final_rnn_return_sequences and self._apply_dense_for_each_timestep:
-            if self._permute_output: self.batch_output_shape = (self._N, self._outfeatures, self._L_out)
-            else: self.batch_output_shape = (self._N, self._L_out, self._outfeatures)
-        else: self.batch_output_shape = (self._N, self._L_out * self._outfeatures)
-        self._out_activation_module = actdict_keras[self._outactivation] if self._outactivation else None
-        
-        # Initializing sequential network
-        self.net = tf.keras.models.Sequential()
-        
-        # Constructing RNN layers
-        _kwargs = {'units':self._H_cell, 'dropout':self._rnndropout, 
-            'return_sequences':(True if self._rnndepth > 1 else self._final_rnn_return_sequences), 
-            'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None)}
-        if self._rnn_params: 
-            _kwargs.update(self._rnn_params)
-        self.net.add(tf.keras.Input((self._L_in,self._H_in)))
-        for i in range(self._rnndepth):
-            if i != self._rnndepth-1:
-                _kwargs.update({'return_sequences':True})
+        super(ANN, self).__init__(hparams)
+        # Read and store hyperparameters
+        if not hparams: hparams=self.sample_hparams
+        self._model_name = hparams.get("model_name") if "model_name" in hparams else "ANN"
+        self._input_shape = hparams.get("input_shape")
+        if self._input_shape is not None:
+            assert isinstance(self._input_shape, (list,tuple)), "input_shape must be a list or tuple."
+        self._output_size = hparams.get("output_size")
+        self._dropout = hparams.get("dropout")
+        self._width = hparams.get("width")
+        self._depth = hparams.get("depth")
+        if self._depth is None:
+            assert isinstance(self._width, (list,tuple)), "If depth is not provided, width must be a list or tuple."
+            self._depth = len(self._width)
+        elif self._width is None:
+            assert isinstance(self._depth, int), "If width is not provided, depth must be an integer."
+            warnings.warn("Width is not provided. It will be set to the same value as the final dimension of the input shape.", UserWarning)
+            self._width = self._input_shape[-1]
+        elif isinstance(self._width, (list,tuple)):
+            assert len(self._width) == self._depth, "If width is a list or tuple, it must have length equal to the depth."
+            
+            
+        self._hidden_activation = hparams.get("hidden_activation")
+        self._hidden_activation_params = hparams.get("hidden_activation_params")
+        self._include_output_layer = hparams.get("include_output_layer")
+        self._output_activation = hparams.get("output_activation")
+        self._output_activation_params = hparams.get("output_activation_params")
+        self._norm_layer_type = hparams.get("norm_layer_type")
+        self._norm_layer_position = hparams.get("norm_layer_position")
+        self._norm_layer_params = hparams.get("norm_layer_params")
+        self.batch_input_shape = (self._batch_size,) + tuple(self._input_shape)
+        self.batch_output_shape = (self._batch_size,) + tuple(self._input_shape[:-1]) + (self._output_size,)
+        if self._output_activation is not None:
+            if isinstance(self._output_activation, str):
+                if self._output_activation.lower()==self._output_activation:
+                    self._output_activation_module = getattr(tf.keras.activations, self._output_activation)
+                else:
+                    self._output_activation_module = getattr(tf.keras.layers, self._output_activation)
             else:
-                _kwargs.update({'return_sequences':self._final_rnn_return_sequences})
-            self.net.add(tf.keras.layers.Bidirectional(self._rnn(**_kwargs)) if self._bidirectional else self._rnn(**_kwargs))
-        
-        # If the final RNN layer returns sequences, and we are NOT applying the dense on each time step of it, then the returned sequence must be flattened before being decocded.
-        if self._final_rnn_return_sequences and not self._apply_dense_for_each_timestep:
-            self.net.add(tf.keras.layers.Flatten())
-        
-        # Calculating Dense layers widths
-        cf = self._L_in if (self._final_rnn_return_sequences and not self._apply_dense_for_each_timestep) else 1 
-        self._dense_input_size = self._H_out * self._D * cf
-        if self._final_rnn_return_sequences and not self._apply_dense_for_each_timestep:
-            self._dense_output_size = int(self._L_out*self._outfeatures)
+                self._output_activation_module = self._output_activation
         else:
-            self._dense_output_size = int(self._outfeatures)
-            
+            self._output_activation_module = None
+        
         # Generate arrays containing parameters of each Dense Block (Every block contains a linear, normalization, activation, and dropout layer).
-        self._dense_width_vec = self._gen_hparam_vec_for_dense(self._densehidsizes, 'dense_width')
-        self._dense_activation_vec = self._gen_hparam_vec_for_dense(self._denseactivation, 'dense_activation')
-        self._dense_activation_params_vec = self._gen_hparam_vec_for_dense(self._denseactivation_params, 'dense_activation_params')
-        self._dense_norm_layer_type_vec = self._gen_hparam_vec_for_dense(self._normlayer_type, 'norm_layer_type')
-        self._dense_norm_layer_params_vec = self._gen_hparam_vec_for_dense(self._normlayer_params, 'norm_layer_params')
-        self._dense_norm_layer_position_vec = self._gen_hparam_vec_for_dense(self._normlayer_position, 'norm_layer_position')
-        self._dense_dropout_vec = self._gen_hparam_vec_for_dense(self._densedropout, 'dense_dropout')
+        self._dense_width_vec = self._gen_hparam_vec_for_dense(self._width, 'width')
+        self._dense_activation_vec = self._gen_hparam_vec_for_dense(self._hidden_activation, 'hidden_activation')
+        self._dense_activation_params_vec = self._gen_hparam_vec_for_dense(self._hidden_activation_params, 'hidden_activation_params')
+        self._dense_norm_layer_type_vec = self._gen_hparam_vec_for_dense(self._norm_layer_type, 'norm_layer_type')
+        self._dense_norm_layer_params_vec = self._gen_hparam_vec_for_dense(self._norm_layer_params, 'norm_layer_params')
+        self._dense_norm_layer_position_vec = self._gen_hparam_vec_for_dense(self._norm_layer_position, 'norm_layer_position')
+        self._dense_dropout_vec = self._gen_hparam_vec_for_dense(self._dropout, 'dropout')
+        
+        # Initialize sequential model
+        self.net = tf.keras.models.Sequential(name=self._model_name)
         
         # Construct the dense layers
-        in_size = self._dense_input_size
-        for i in range(self._densedepth):
-            out_size = self._dense_width_vec[i]
-            temp_dropout_rate = self._dense_dropout_vec[i] if (i != self._densedepth-1) else None # The hidden layer just before the output layer rarely has Dropout.
-            add_dense_block(self.net, output_size=out_size, input_shape=None, activation=self._dense_activation_vec[i], activation_params=self._dense_activation_params_vec[i], 
-                    norm_layer_type=self._dense_norm_layer_type_vec[i], norm_layer_position=self._dense_norm_layer_position_vec[i], 
-                    norm_layer_params=self._dense_norm_layer_params_vec[i], dropout=temp_dropout_rate, 
-                    kernel_regularizer=(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None))
-            in_size = out_size
+        # in_size = self._input_shape
+        for i in range(self._depth):
+            # out_size = self._dense_width_vec[i]
+            _kwargs = {
+                'model':self.net,
+                'output_size':self._dense_width_vec[i],
+                'activation':self._dense_activation_vec[i],
+                'activation_params':self._dense_activation_params_vec[i],
+                'norm_layer_type':self._dense_norm_layer_type_vec[i],
+                'norm_layer_position':self._dense_norm_layer_position_vec[i],
+                'norm_layer_params':self._dense_norm_layer_params_vec[i],
+                'dropout':self._dense_dropout_vec[i],
+                'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None)
+            }
+            if i==0 and self._input_shape is not None:
+                _kwargs.update({'input_shape':self._input_shape})
+            add_dense_block(**_kwargs)
+            # in_size = out_size
         
         # Output layer
-        self.net.add(tf.keras.layers.Dense(self._dense_output_size))
-        if self._outactivation:
-            if self._outactivation_params: self.net.add(tf.keras.layers.Activation(self._out_activation_module(**self._outactivation_params)))
-            else: self.net.add(tf.keras.layers.Activation(self._out_activation_module))
-            
-        # Permute if necessary
-        if self._final_rnn_return_sequences and self._apply_dense_for_each_timestep and self._permute_output:
-            self.net.add(tf.keras.layers.Permute((2,1)))
-        
+        if self._include_output_layer:
+            self.net.add(tf.keras.layers.Dense(self._output_size, kernel_regularizer=(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None)))
+            if self._output_activation:
+                if isinstance(self._output_activation, str):
+                    if self._output_activation.lower() == self._output_activation:
+                        self.net.add(tf.keras.layers.Activation(self._output_activation))
+                    elif self._output_activation_params:
+                        self.net.add(getattr(tf.keras.layers, self._output_activation)(**self._output_activation_params))
+                    else:
+                        self.net.add(getattr(tf.keras.layers, self._output_activation)())
+                elif self._output_activation_params:
+                    self.net.add(self._output_activation(**self._output_activation_params))
+                else:
+                    self.net.add(self._output_activation())
+
     def _gen_hparam_vec_for_dense(self, hparam, hparam_name, **kwargs):
-        return generate_array_for_hparam(hparam, self._densedepth, hparam_name=hparam_name, count_if_not_list_name='dense_depth', **kwargs)
-    
-    def call(self, x, *args, **kwargs):
-        return self.net(x, *args, **kwargs)
+        return generate_array_for_hparam(hparam, self._depth, hparam_name=hparam_name, count_if_not_list_name='depth', **kwargs)
+        
+    def call(self, x, **kwargs):
+        return self.net(x, **kwargs)
+
+
 
 
 
 if __name__ == '__main__':
-    hparams = Recurrent_Network.sample_hparams
-    hparams['rnn_bidirectional'] = True
-    model = Recurrent_Network(hparams)
-    model.summary()
+    
+    hparams = {
+        # General and I/O parameters
+        "model_name": "My Model",
+        "input_shape": [28, 28, 3], #[10],
+        "output_size": 24,
+        # Architecture parameters
+        "width": 32,
+        "depth": 3,
+        "hidden_activation": "LeakyReLU",
+        "hidden_activation_params": {'alpha':0.1},
+        "norm_layer_type":"BatchNormalization",
+        "norm_layer_position": "before",
+        "norm_layer_params": None,
+        "dropout": 0.2,
+        "include_output_layer": True,
+        "output_activation": "Softmax",
+        "output_activation_params": None,
+        # Training procedure parameters
+        "learning_rate": 0.001,
+        "exponential_decay_rate": 0.9,
+        "batch_size": 32,
+        "epochs": 2,
+        "early_stopping_patience_epochs": 2,
+        "validation_data": [0.05,'trainset'],
+        "l2_reg": 0.0001,
+        "loss_function": "categorical_crossentropy",
+        'optimizer': 'Adam',
+        'optimizer_params': None,
+        'metrics': ['accuracy'],
+        'checkpoint_path': None,
+        'early_stopping_monitor': 'loss',
+        'early_stopping_mode': 'min',
+        'early_stopping_value': 1.0e-6
+    }
+    test_keras_model_class(ANN, hparams, False)
+
```

### Comparing `eznet_keras-0.0.3/eznet_keras/models/var_ae.py` & `eznet_keras-1.0.0/eznet_keras/models/var_ae.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-0.0.3/eznet_keras/test.py` & `eznet_keras-1.0.0/eznet_keras/test.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-0.0.3/eznet_keras/utils.py` & `eznet_keras-1.0.0/eznet_keras/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,27 +46,28 @@
 
 
 def make_path(path:str):
     Path.mkdir(Path(path).parent, parents=True, exist_ok=True)
     return path
     
 
-def plot_keras_model_history(history:dict, metrics:list=['loss','val_loss'], 
-                             fig_title:str='model loss', saveto:str=None):
-    plt.figure(figsize=(15, 7))
+def plot_keras_model_history(history:dict, metrics:list=['loss'], fig_title:str='model loss', saveto:str=None, close_after_finish:bool=True):
+    plt.figure(figsize=(7, 5))
     plt.grid(True)
-    plt.plot(history[metrics[0]])
-    plt.plot(history[metrics[1]])
+    plt.plot(history[metrics[0]], label='training')
+    if len(metrics) > 1:
+        plt.plot(history[metrics[1]], label='validation')
     plt.title(fig_title)
     plt.ylabel(metrics[0])
     plt.xlabel('epoch')
-    plt.legend(['train', 'val'], loc='upper left')
-    plt.show()
+    plt.legend(loc='upper right')
     if saveto:
         plt.savefig(make_path(saveto), dpi=600)
+        if close_after_finish:
+            plt.close()
         
 
 def compile_keras_model(model, _batchsize:int, _learnrate:float, _optimizer:str, _loss:str, _metrics:list, 
                           _optimizerparams:dict=None, _learnrate_decay_gamma:float=None, num_samples:int=None):
     if _learnrate_decay_gamma:
         itersPerEpoch = (num_samples//_batchsize) if num_samples else 1
         sch = tf.keras.optimizers.schedules.ExponentialDecay(initial_learning_rate=_learnrate, 
@@ -80,20 +81,20 @@
         opt = getattr(tf.keras.optimizers, _optimizer)(learning_rate=lr, **optparam)
     else:
         # opt = optdict_keras[_optimizer](learning_rate=lr)
         opt = getattr(tf.keras.optimizers, _optimizer)(learning_rate=lr)
     model.compile(optimizer=opt, loss=_loss, metrics=_metrics)
     
 
-def fit_keras_model(model, x_train, y_train, x_val, y_val, 
-    _batchsize:int, _epochs:int, _callbacks:list, verbose:bool=True, **kwargs):
+def fit_keras_model(model, x_train, y_train, x_val=None, y_val=None, 
+    _batchsize:int=None, _epochs:int=1, _callbacks:list=None, verbose:int=1, **kwargs):
     while True:
         try:
             history = model.fit(x_train, y_train, batch_size=_batchsize, epochs=_epochs, 
-                validation_data=(x_val, y_val), verbose=verbose, 
+                validation_data=((x_val, y_val) if x_val is not None and y_val is not None else None), verbose=verbose, 
                 callbacks=_callbacks, **kwargs)
             break
         except Exception as e:
             print(e)
             print(("\nTraining failed with batchsize={}. "+\
                 "Trying again with a lower batchsize...").format(_batchsize))
             _batchsize = _batchsize // 2
@@ -127,28 +128,32 @@
             export_model(net, make_path(path))
             print("Model exported successfully.")
         except Exception as e2:
             print(e2)
             print("Cannot export model using Keras2Cpp.")
     
 
-def test_keras_model_class(model_class):
+def test_keras_model_class(model_class, hparams:dict=None, save_and_export:bool=True):
     print("Constructing model...\n")
-    model = model_class()
+    model = model_class(hparams)
     print("Summary of model:")
     print(model.summary())
     print("\nGenerating random dataset...\n")
     (x_train, y_train) = generate_sample_batch(model)
     (x_val, y_val) = generate_sample_batch(model)
+    print("Trying forward pass on training data: ")
+    y = model(x_train)
+    print("\nOutput shape: ", y.shape)
     print("\nTraining model...\n")
-    model.train(x_train, x_val, y_train, y_val, 
-                verbose=True, saveto="test_"+model.hparams["model_name"], 
-                export="test_"+model.hparams["model_name"]+".model")
+    model.train_model(x_train, y_train, x_val, y_val, 
+                verbose=1, 
+                saveto=(("test_"+model.hparams["model_name"]) if save_and_export else None), 
+                export=(("test_"+model.hparams["model_name"]+".model") if save_and_export else None))
     print("\nEvaluating model...\n")
-    model.evaluate(x_val, y_val, verbose=True)
+    model.evaluate(x_val, y_val, verbose=1)
     print("Done.")
     
 
 
 # Perform garbage collection
 class GarbageCollectionCallback(tf.keras.callbacks.Callback):
     def on_epoch_end(self, epoch, logs=None):
@@ -196,21 +201,23 @@
 
 def calc_image_size(size_in:int, kernel_size:int, padding:int, stride:int, dilation:int):
     """Calculate image size after convolution or pooling.
     
     **NOTE** grouping is not supported yet.
 
     ### Args:
+    
         - `size_in` (int|list): (list of) image input dimension(s).
         - `kernel_size` (int|list): (list of) kernel (or pool) size
         - `padding` (int|list): (list of) padding sizes, or string such as 'valid' and 'same'.
         - `stride` (int|list): (list of) strides.
         - `dilation` (int|list): (list of) dilation rates.
 
     ### Returns:
+    
         int or list: Output image dimensions
     """
     if padding == 'same':
         return size_in
     else:
         if padding == 'valid':
             padding = 0
@@ -229,20 +236,22 @@
             return math.floor((size_in + 2*padding - dilation*(kernel_size-1) - 1)/stride + 1)
 
 
 def generate_geometric_array(init, count, direction, powers_of_two=True):
     """Generate array filled with incrementally doubling/halving values, optionally with powers of two.
 
     ### Args:
-        `init` (int): The first value to begin.
-        `count` (int): Number of elements to generate.
-        `direction` (str): Direction of the array. Can be either 'up' or 'down', i.e. increasing or decreasing.
-        `powers_of_two` (bool, optional): Generate numbers that are powers of two. Defaults to True.
+    
+        - `init` (int): The first value to begin.
+        - `count` (int): Number of elements to generate.
+        - `direction` (str): Direction of the array. Can be either 'up' or 'down', i.e. increasing or decreasing.
+        - `powers_of_two` (bool, optional): Generate numbers that are powers of two. Defaults to True.
 
     ### Returns:
+    
         list: List containing elements
     """
     lst = []
     old = int(2**math.ceil(math.log2(init))) if powers_of_two else init
     new = old
     for _ in range(count):
         lst.append(new)
@@ -260,25 +269,27 @@
     that generate models with hyperparameters as inputs, which can be lists, a single item, or "auto".
     Examples include width of a neural network's hidden layers, channels of conv layers, etc.
     For these hyperparameters, the user is typically free to specify an array-like, a single item to be repeated,
     or "auto" for automatic calculation of the parameter.
     This function is meant to be used in the body of the code of class constructors and other functions in the API.
 
     ### Args:
-        `hparam` (var): A specific hyperparameter, e.g., input by user to your network's constructor.
-        `count_if_not_list` (int): Number of elements to generate if `hparam` is not an array-like.
-        `hparam_name` (str, optional): Name of the hyperparameter. Defaults to 'parameter'.
-        `count_if_not_list_name` (str, optional): Name of the "count" that must be provided. Defaults to 'its count'.
-        `check_auto` (bool, optional): Check for the "auto" case. Defaults to False.
-        `init_for_auto` (int, optional): Initial value in case of "auto". Defaults to 2.
-        `powers_of_two_if_auto` (bool, optional): Generate powers of two in case of "auto". Defaults to True.
-        `direction_if_auto` (str, optional): Direction of geometric increment in case of "auto". Defaults to None.
-        This can be "up" or "down". If check_for_auto is True, then this argument must be specified.
+    
+        - `hparam` (var): A specific hyperparameter, e.g., input by user to your network's constructor.
+        - `count_if_not_list` (int): Number of elements to generate if `hparam` is not an array-like.
+        - `hparam_name` (str, optional): Name of the hyperparameter. Defaults to 'parameter'.
+        - `count_if_not_list_name` (str, optional): Name of the "count" that must be provided. Defaults to 'its count'.
+        - `check_auto` (bool, optional): Check for the "auto" case. Defaults to False.
+        - `init_for_auto` (int, optional): Initial value in case of "auto". Defaults to 2.
+        - `powers_of_two_if_auto` (bool, optional): Generate powers of two in case of "auto". Defaults to True.
+        - `direction_if_auto` (str, optional): Direction of geometric increment in case of "auto". Defaults to None.
+           This can be "up" or "down". If check_for_auto is True, then this argument must be specified.
 
     ### Returns:
+    
         list: List containing elements
     """
     assert count_if_not_list is not None, \
         "Since %s may not be a list/tuple, %s must always be specified."%(hparam_name, count_if_not_list_name)
     if isinstance(hparam, (list,tuple)) and len(hparam) == count_if_not_list:
         lst = hparam
     elif hparam == "auto" and check_auto:
```

### Comparing `eznet_keras-0.0.3/eznet_keras.egg-info/PKG-INFO` & `eznet_keras-1.0.0/eznet_keras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: eznet-keras
-Version: 0.0.3
-Summary: Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Conv blocks, etc.
+Version: 1.0.0
+Summary: Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc.
 Home-page: https://github.com/pniaz20/eznet_keras
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: tensorflow,keras,deep learning,neural network,keras2cpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -25,16 +25,16 @@
 
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.3  
-Last Update: Jan 20, 2023
+Version: 1.0.0  
+Last Update: July 15, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
 
@@ -84,21 +84,20 @@
     def call(self, x, *args, **kwargs):
         return self.net(x, *args, **kwargs)
 
 sample_hparams = {
     'model_name': 'KerasSmartModel',                    # Name of the model
     'l2_reg': 0.0001,                                   # L2 regularization parameter
     'batch_size': 16,                                   # Mini-batch size
-    'epochs': 2,                                        # Maximum training epochs
+    'epochs': 40,                                       # Maximum training epochs
     'validation_data': [0.05,'trainset'],               # Portion of train set used for validation (if necessary)
-    'validation_tolerance_epochs': 10,                  # Validation patience for early stopping
+    'early_stopping_patience_epochs': 10,               # Validation patience for early stopping
     'learning_rate': 0.0001,                            # (Initial) Learning rate
-    'learning_rate_decay_gamma': 0.99,                  # Learning rate exponential decay gamma
+    'exponential decay rate': 0.99,                     # Learning rate exponential decay factor
     'loss_function': 'categorical_crossentropy',        # Loss function string
-    'loss_function_params': None,                       # Dictionary of parameters to pass to the loss function
     'metrics':['accuracy'],                             # List of metrics
     'optimizer': 'Adam',                                # Optimizer string
     'optimizer_params': None,                           # Dictionary of parameters to pass to the optimizer constructor
     'checkpoint_path':None,                             # Path to store checkpoints in every epoch
     'early_stopping_monitor':'loss',                    # Early stopping criteria (stop when alue is reached and performance is good enough)
     'early_stopping_mode':'min',                        # Early stopping variable mode (minimization or maximization)
     'early_stopping_value':1.0e-6                       # Threshold for early stopping
@@ -107,15 +106,15 @@
 model = MyModel(sample_hparams)
 
 x_train = ...
 y_train = ...
 x_test = ...
 y_test = ...
 
-model.train(x_train, x_test, y_train, y_test, verbose=1, saveto="my_model", export="my_model.model")
+model.train_model(x_train, y_train, x_test, y_test, verbose=1, saveto="my_model", export="my_model.model")
 model.plot_history(metrics=['loss','val_loss'], fig_title='model loss', saveto="training_history.png")
 ```
 
 A few implementation notes:
 
 - Whatever hyperparameters you have for the model itself, can be included in the hparams dictionary.
 - The model must always have a `self.net` atttribute which contains the network itself. It can be a Sequential or Functional model.
```

### Comparing `eznet_keras-0.0.3/eznet_keras.egg-info/SOURCES.txt` & `eznet_keras-1.0.0/eznet_keras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eznet_keras-0.0.3/setup.py` & `eznet_keras-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.0.3' 
-DESCRIPTION = "Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Conv blocks, etc."
+VERSION = '1.0.0' 
+DESCRIPTION = "Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc."
 
 # Setting up
 setup(
-       # the name must match the folder name
+        # the name must match the folder name
         name="eznet_keras", 
         version=VERSION,
         author="Pouya P. Niaz",
         author_email="<pniaz20@ku.edu.tr>",
         url='https://github.com/pniaz20/eznet_keras',
         description=DESCRIPTION,
         long_description=long_description,
```

