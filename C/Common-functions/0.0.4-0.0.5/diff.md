# Comparing `tmp/Common_functions-0.0.4.tar.gz` & `tmp/Common_functions-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Common_functions-0.0.4.tar", last modified: Sat Jul 15 21:06:05 2023, max compression
+gzip compressed data, was "Common_functions-0.0.5.tar", last modified: Sat Jul 15 21:10:53 2023, max compression
```

## Comparing `Common_functions-0.0.4.tar` & `Common_functions-0.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:06:05.792692 Common_functions-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:06:05.784692 Common_functions-0.0.4/AI_ML/
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/a_star_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/alpha_beta_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/ao_star_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/breadth_first_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/check_prime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/classification_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/depth_first_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/factorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/genetic_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/hill_climbing.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/iterative_deepening_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/min_max_game.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/multiplication_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/simple_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/simple_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/text_to_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/traveling_salesperson_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/uniform_cost_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-15 21:05:51.000000 Common_functions-0.0.4/AI_ML/water_jug_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:06:05.784692 Common_functions-0.0.4/C/
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-15 21:05:51.000000 Common_functions-0.0.4/C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 21:05:51.000000 Common_functions-0.0.4/C/createfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:06:05.788692 Common_functions-0.0.4/Common_functions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-15 21:06:05.000000 Common_functions-0.0.4/Common_functions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-15 21:06:05.000000 Common_functions-0.0.4/Common_functions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:06:05.000000 Common_functions-0.0.4/Common_functions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 21:06:05.000000 Common_functions-0.0.4/Common_functions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:06:05.792692 Common_functions-0.0.4/Data_Mining/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/Makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/binary_logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/data_exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/data_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/frequent_itemset_mining.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/hierarchical_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/k_means_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/knn_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/naive_bayes_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/social_network_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Data_Mining/standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:06:05.792692 Common_functions-0.0.4/Java_Programs/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Java_Programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Java_Programs/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-15 21:05:51.000000 Common_functions-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-15 21:06:05.792692 Common_functions-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:06:05.792692 Common_functions-0.0.4/Python_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    30718 2023-07-15 21:05:51.000000 Common_functions-0.0.4/Python_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-15 21:05:51.000000 Common_functions-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 21:06:05.792692 Common_functions-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-15 21:05:51.000000 Common_functions-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:53.731816 Common_functions-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:53.723816 Common_functions-0.0.5/AI_ML/
+-rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/a_star_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/alpha_beta_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/ao_star_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/breadth_first_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/check_prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/classification_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/depth_first_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/genetic_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/hill_climbing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/iterative_deepening_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/min_max_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/multiplication_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/simple_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/simple_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/text_to_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/traveling_salesperson_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/uniform_cost_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-15 21:10:38.000000 Common_functions-0.0.5/AI_ML/water_jug_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:53.723816 Common_functions-0.0.5/C/
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-15 21:10:38.000000 Common_functions-0.0.5/C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 21:10:38.000000 Common_functions-0.0.5/C/createfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:53.723816 Common_functions-0.0.5/Common_functions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-15 21:10:53.000000 Common_functions-0.0.5/Common_functions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-15 21:10:53.000000 Common_functions-0.0.5/Common_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:10:53.000000 Common_functions-0.0.5/Common_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 21:10:53.000000 Common_functions-0.0.5/Common_functions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:53.727816 Common_functions-0.0.5/Data_Mining/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/Makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/binary_logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/data_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/data_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/frequent_itemset_mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/hierarchical_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/k_means_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/knn_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/naive_bayes_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/social_network_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Data_Mining/standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:53.727816 Common_functions-0.0.5/Java_Programs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Java_Programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Java_Programs/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-15 21:10:38.000000 Common_functions-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-15 21:10:53.727816 Common_functions-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:10:53.727816 Common_functions-0.0.5/Python_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    30718 2023-07-15 21:10:38.000000 Common_functions-0.0.5/Python_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-15 21:10:38.000000 Common_functions-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 21:10:53.731816 Common_functions-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-15 21:10:38.000000 Common_functions-0.0.5/setup.py
```

### Comparing `Common_functions-0.0.4/AI_ML/__init__.py` & `Common_functions-0.0.5/AI_ML/__init__.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/a_star_algorithm.py` & `Common_functions-0.0.5/AI_ML/a_star_algorithm.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/alpha_beta_pruning.py` & `Common_functions-0.0.5/AI_ML/alpha_beta_pruning.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/ao_star_algorithm.py` & `Common_functions-0.0.5/AI_ML/ao_star_algorithm.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/breadth_first_search.py` & `Common_functions-0.0.5/AI_ML/breadth_first_search.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/classification_algorithms.py` & `Common_functions-0.0.5/AI_ML/classification_algorithms.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/genetic_algorithm.py` & `Common_functions-0.0.5/AI_ML/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/hill_climbing.py` & `Common_functions-0.0.5/AI_ML/hill_climbing.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/iterative_deepening_search.py` & `Common_functions-0.0.5/AI_ML/iterative_deepening_search.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/makefile.py` & `Common_functions-0.0.5/AI_ML/makefile.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/min_max_game.py` & `Common_functions-0.0.5/AI_ML/min_max_game.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/neural_network.py` & `Common_functions-0.0.5/AI_ML/neural_network.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/simple_calculator.py` & `Common_functions-0.0.5/AI_ML/simple_calculator.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/tic_tac_toe.py` & `Common_functions-0.0.5/AI_ML/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/traveling_salesperson_problem.py` & `Common_functions-0.0.5/AI_ML/traveling_salesperson_problem.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/uniform_cost_search.py` & `Common_functions-0.0.5/AI_ML/uniform_cost_search.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/AI_ML/water_jug_problem.py` & `Common_functions-0.0.5/AI_ML/water_jug_problem.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/C/__init__.py` & `Common_functions-0.0.5/C/__init__.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/Common_functions.egg-info/PKG-INFO` & `Common_functions-0.0.5/Common_functions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Common-functions
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mini Project on creating a library for all the program in 5 syllabus
 Home-page: https://github.com/Jyotijaladi/Common_functions
 Author: Jyoti
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: pandas
```

### Comparing `Common_functions-0.0.4/Common_functions.egg-info/SOURCES.txt` & `Common_functions-0.0.5/Common_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/Data_Mining/__init__.py` & `Common_functions-0.0.5/Data_Mining/__init__.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/Java_Programs/__init__.py` & `Common_functions-0.0.5/Java_Programs/__init__.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/LICENSE` & `Common_functions-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/PKG-INFO` & `Common_functions-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Common_functions
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mini Project on creating a library for all the program in 5 syllabus
 Home-page: https://github.com/Jyotijaladi/Common_functions
 Author: Jyoti
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: pandas
```

### Comparing `Common_functions-0.0.4/Python_lib/__init__.py` & `Common_functions-0.0.5/Python_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `Common_functions-0.0.4/setup.py` & `Common_functions-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 from typing import List
 REQUIREMENT_FILE_NAME="requirements.txt"
 Project_Name="Common_functions"
-Version="0.0.4"
+Version="0.0.5"
 AUTHOR="Jyoti"
 DESCRIPTION="Mini Project on creating a library for all the program in 5 syllabus"
```

