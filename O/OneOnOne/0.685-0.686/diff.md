# Comparing `tmp/OneOnOne-0.685.tar.gz` & `tmp/OneOnOne-0.686.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.685.tar", last modified: Thu Jul 13 18:22:01 2023, max compression
+gzip compressed data, was "OneOnOne-0.686.tar", last modified: Sat Jul 15 11:13:11 2023, max compression
```

## Comparing `OneOnOne-0.685.tar` & `OneOnOne-0.686.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 18:22:01.336634 OneOnOne-0.685/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.685/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 18:22:01.333928 OneOnOne-0.685/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    34180 2023-07-13 18:18:44.000000 OneOnOne-0.685/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.685/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14754 2023-07-12 17:06:31.000000 OneOnOne-0.685/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.685/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.685/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 18:22:01.335648 OneOnOne-0.685/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-13 18:22:01.000000 OneOnOne-0.685/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-13 18:22:01.000000 OneOnOne-0.685/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-13 18:22:01.000000 OneOnOne-0.685/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      114 2023-07-13 18:22:01.000000 OneOnOne-0.685/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-13 18:22:01.000000 OneOnOne-0.685/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-13 18:22:01.336206 OneOnOne-0.685/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.685/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-13 18:22:01.336756 OneOnOne-0.685/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1909 2023-07-13 18:19:21.000000 OneOnOne-0.685/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-15 11:13:11.879034 OneOnOne-0.686/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.686/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-15 11:13:11.874533 OneOnOne-0.686/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    35653 2023-07-15 11:12:22.000000 OneOnOne-0.686/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.686/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.686/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.686/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.686/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-15 11:13:11.877633 OneOnOne-0.686/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      114 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-15 11:13:11.000000 OneOnOne-0.686/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-15 11:13:11.878352 OneOnOne-0.686/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.686/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-15 11:13:11.879239 OneOnOne-0.686/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1909 2023-07-15 11:12:34.000000 OneOnOne-0.686/setup.py
```

### Comparing `OneOnOne-0.685/LICENSE` & `OneOnOne-0.686/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.685/OneOnOne/__init__.py` & `OneOnOne-0.686/OneOnOne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,32 +30,36 @@
 from sklearn.model_selection import cross_val_score
 from sklearn import metrics
 from sklearn import preprocessing
 from sklearn.utils import shuffle
 
 from tqdm import keras
 import urllib.request
-
-
+import urllib
+import pkgutil
+# from urllib.request import urlretrieve
+# from urllib import urlretrieve
 class PretrainedModel:
-    def __init__(self, model_type="resnet50", dataset="cifar10", sampling="none"):
-        filepath = resource_filename(__name__, 'resnet50_cifar10_none')
+    def __init__(self, model_type="resnet50", dataset="cifar10", samplingtype="none"):
 
         self.model_type=model_type
         self.dataset=dataset
-        self.sampling=sampling
+        self.samplingtype=samplingtype
 
         if self.dataset=="tinyimagenet":
             self.model_type="efficientnetb6"
-            self.sampling="none"
+            self.samplingtype="none"
 
-        # self.model=urllib.request.urlretrieve('https://github.com/sohini-bhattacharya/OneOnOne/blob/e4adf61b6c3b73a917b1f2b0d441318d981a5aa4/OneOnOne/resnet50_cifar10_none',f"{self.model_type}_{self.dataset}_{self.sampling}")
-        # print(self.model)
-        self.model=load_model(f'{filepath}')
-        print(self.model)
+        if self.samplingtype=="none" or self.samplingtype=="None":
+            self.path=os.getcwd()+f'/models_to_load/{self.model_type}_{self.dataset}'
+        else:
+            self.path=os.getcwd()+f'/models_to_load/{self.model_type}_{self.dataset}_{self.samplingtype}'
+
+        self.model=urllib.request.urlretrieve('https://github.com/sohini-bhattacharya/OneOnOne/blob/master/saved_models/resnet50_cifar10_none.zip',f"{self.path}_none_webzip")
+        self.model=load_model(self.path)
         self.model.summary()
 
 
 
 
 class Classification:
     def __init__(self, model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
@@ -102,15 +106,15 @@
                                          epochs=self.epochs, verbose=1, workers=4,
                                          callbacks=self.callbacks)
             else:
                 history = self.model.fit(self.train_it, validation_data=self.val_it,
                                      epochs=self.epochs, verbose=1, workers=4,
                                      callbacks=self.callbacks)
 
-            self.model.save(os.getcwd()+f"/fully_trained/{self.model_type}_{self.dataset}_{self.date}")
+            self.model.save(os.getcwd()+f"/saved_models/{self.model_type}_{self.dataset}_{self.date}_completed")
 
             history_token = input("Save/Discard?  :   ")
 
             if history_token.lower()=="save":
                 with open(f'{self.model_type}_{self.dataset}_{self.date}_history', 'wb') as file_pi:
                     pickle.dump(history.history, file_pi)
                 print("saved")
@@ -118,17 +122,15 @@
                 print("discarded")
             else:
                 print("Invalid Input!")
 
         elif self.token.lower() == 'load':
             print("loading")
 
-            path_token = input("Model Path?  :   ")
-
-            self.model = load_model(os.getcwd()+path_token)
+            self.model = load_model(os.getcwd()+"/models_to_load/"+f"{self.model_type}_{self.dataset}")
 
         else:
             print("invalid input")
 
     def lr_schedule(self, epoch):
         lr = 1e-3
         if epoch > 180:
@@ -226,15 +228,15 @@
             input_images = input_images.astype('float32')
             output_ims = tf.keras.applications.resnet50.preprocess_input(input_images)
 
         return output_ims
 
     def get_callbacks(self):
 
-        save_dir = os.path.join(os.getcwd(), f'saved_models_{self.model_type}_{self.dataset}_{self.date}')
+        save_dir = os.getcwd()+f'/saved_models/{self.model_type}_{self.dataset}'
         model_name = self.model_type + '_model_' + str(self.date.day) + '_' + str(self.date.month) + '_' + str(
             self.date.year) + '.{epoch:03d}.h5'
 
         if not os.path.isdir(save_dir):
             os.makedirs(save_dir)
         filepath = os.path.join(save_dir, model_name)
         checkpoint = ModelCheckpoint(filepath=filepath,
@@ -303,17 +305,35 @@
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
             print(number_of_train_samples)
             print(number_of_val_samples)
-        elif self.dataset=="cifar10":
-            (train_it), (val_it) = tf.keras.datasets.cifar10.load_data()
-            self.datagen.fit(train_it)
+        elif self.dataset == "cifar10":
+            classes = ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
+            num_classes = len(classes)
+            (training_images, training_labels), (
+                    validation_images, validation_labels) = tf.keras.datasets.cifar10.load_data()
+
+            train_X = self.preprocess_image_input(training_images)
+            valid_X = self.preprocess_image_input(validation_images)
+
+            training_labels = to_categorical(training_labels, num_classes)
+            validation_labels = to_categorical(validation_labels, num_classes)
+            self.datagen.fit(train_X)
+
+            train_it = self.datagen.flow(train_X, training_labels, batch_size=self.batch_size)
+            val_it = (valid_X, validation_labels)
+
+            # self.X_train = train_X
+            # self.X_test = valid_X
+            # self.y_train = training_labels
+            # self.y_test = validation_labels
+
 
 
         return train_it, val_it
 
     def save_history_details(self, history_data, keys):
 
         pd.DataFrame(history_data).to_csv(os.getcwd()+f"history_{self.model_type}_{self.dataset}_{self.date}.csv", header=keys)
@@ -340,32 +360,31 @@
         loss, accuracy = self.model.evaluate(self.val_it, batch_size=self.batch_size, verbose=1)
 
 
 class Sampling:
     def __init__(self, samplingtype, dataset="cifar10", model_type = "resnet50", goal=99, jump=5000, first_data_samples=10000, batch_size = 16, epochs = 250, shuffle_bool = True, early_stopping_patience = 10, lr_reducer_patience = 10):
 
         self.validation_split=0
-        self.samplingtype = samplingtype
-        self.dataset = dataset
-        self.goal = goal
-        self.date=datetime.datetime.now()
+        self.model_type = model_type
         self.epochs=epochs
         self.jump = jump
-        self.first_data_samples = first_data_samples
-        self.model_type = model_type
-        self.callbacks = self.get_callbacks()
-        self.datagen = self.get_datagen()
-        self.train_it, self.val_it = self.get_dataset()
+        self.samplingtype = samplingtype
+        self.goal = goal
         self.shuffle_bool = shuffle
         self.batch_size = batch_size
+        self.dataset = dataset
         self.output_layer_classes = 0
         self.input_shape = (32, 32, 3)
+        self.date=datetime.datetime.now()
+        self.first_data_samples = first_data_samples
         self.early_stopping_patience = early_stopping_patience
         self.lr_reducer_patience = lr_reducer_patience
         self.callbacks = self.get_callbacks()
+        self.datagen = self.get_datagen()
+        self.train_it, self.val_it = self.get_dataset()
 
         if self.dataset == "cifar10" or self.dataset == "mnist":
             self.output_layer_classes = 10
             self.input_shape = (224, 224, 3)
 
 
         elif self.dataset == "tinyimagenet":
@@ -480,21 +499,22 @@
             input_images = input_images.astype('float32')
             output_ims = tf.keras.applications.resnet50.preprocess_input(input_images)
 
         return output_ims
 
     def get_callbacks(self):
 
-        save_dir = os.path.join(os.getcwd(), f'saved_models_{self.model_type}_{self.dataset}_{self.date}')
+        save_dir = os.getcwd()+f'/saved_models/{self.model_type}_{self.dataset}_{self.samplingtype}'
         model_name = self.model_type + '_model_' + str(self.date.day) + '_' + str(self.date.month) + '_' + str(
             self.date.year) + '.{epoch:03d}.h5'
 
         if not os.path.isdir(save_dir):
             os.makedirs(save_dir)
         filepath = os.path.join(save_dir, model_name)
+
         checkpoint = ModelCheckpoint(filepath=filepath,
                                      monitor='val_accuracy',
                                      verbose=1,
                                      save_best_only=True)
         early_stopping = EarlyStopping(monitor='val_accuracy', mode='max', verbose=1,
                                        patience=self.early_stopping_patience,
                                        restore_best_weights=True)
@@ -729,43 +749,46 @@
 
         probarray.sort(key=lambda x:x[1],reverse=True)
 
         return probarray
 
     # def load_trained_model(self):
 
-
-
     def initial_training(self):
 
         print("training")
 
         if self.dataset=="tinyimagenet":
             self.model = self.define_compile_model()
             self.model.summary()
 
             history = self.model.fit(self.train_it, validation_data=self.val_it,
                                      epochs=self.epochs, verbose=1, workers=4,
                                      callbacks=self.callbacks)
 
-            self.model.save(os.getcwd() + f"/initial_training/{self.model_type}_{self.dataset}_{self.first_data_samples}_{self.date}")
+            self.model.save(os.getcwd() + f"/saved_models/{self.model_type}_{self.dataset}_{self.samplingtype}_{self.first_data_samples}_{self.date}_initial_training")
 
 
             with open(f'{self.model_type}_{self.dataset}_{self.date}_history', 'wb') as file_pi:
                 pickle.dump(history.history, file_pi)
             print("saved")
 
         else:
 
             self.model = self.define_compile_model()
             self.model.summary()
 
             history = self.model.fit(self.datagen.flow(self.X_train, self.y_train, batch_size=self.batch_size), validation_data=(self.X_test, self.y_test),
                                      epochs=self.epochs, verbose=1, workers=4,
                                      callbacks=self.callbacks)
+            self.model.save(os.getcwd() + f"/saved_models/{self.model_type}_{self.dataset}_{self.samplingtype}_{self.first_data_samples}_{self.date}_initial_training")
+
+            with open(f'{self.model_type}_{self.dataset}_{self.date}_history', 'wb') as file_pi:
+                pickle.dump(history.history, file_pi)
+            print("saved")
 
 
 
     def get_iterations(self):
 
 
         eval_metrics=[0,0]
@@ -850,11 +873,13 @@
             for element in total_index:
               if element not in index:
                 a.append(element)
 
             X_train_copy=X_train_copy[a]
             y_train_copy=y_train_copy[a]
 
+        self.model.save(os.getcwd() + f"/saved_models/{self.model_type}_{self.dataset}_{self.samplingtype}_{self.date}_completed")
+
         return history_data,epoch_data,batch_size_data,acuracy_data
```

### Comparing `OneOnOne-0.685/OneOnOne/classes.py` & `OneOnOne-0.686/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.685/OneOnOne/classification.py` & `OneOnOne-0.686/OneOnOne/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 
 import torch
 from torchvision import transforms
 from torch.utils.data import Dataset
 
 
 class Classification:
-    def __init__(self, date = datetime.datetime.now(), model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
+    def __init__(self, model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
 
         self.model_type = model_type
-        self.date = date
+        self.date = datetime.datetime.now()
         self.dataset=dataset
         self.shuffle_bool = shuffle
         self.batch_size = batch_size
         self.epochs = epochs
         self.output_layer_classes=0
         self.input_shape = (32,32,3)
         self.early_stopping_patience=early_stopping_patience
@@ -94,17 +94,17 @@
                 print("discarded")
             else:
                 print("Invalid Input!")
 
         elif self.token.lower() == 'load':
             print("loading")
 
-            path_token = input("Model Path?  :   ")
+            print(os.getcwd())
 
-            self.model = load_model(os.getcwd()+path_token)
+            self.model = load_model(os.getcwd()+"models_to_load/"+f'{self.model_type}_{self.dataset}_none')
 
         else:
             print("invalid input")
 
     def lr_schedule(self, epoch):
         lr = 1e-3
         if epoch > 180:
```

### Comparing `OneOnOne-0.685/OneOnOne/contextdecider.py` & `OneOnOne-0.686/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.685/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.686/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.685
+Version: 0.686
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.685/PKG-INFO` & `OneOnOne-0.686/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.685
+Version: 0.686
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.685/README.md` & `OneOnOne-0.686/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.685/setup.py` & `OneOnOne-0.686/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.685
+VERSION=0.686
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

