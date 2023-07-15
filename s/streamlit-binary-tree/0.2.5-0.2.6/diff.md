# Comparing `tmp/streamlit-binary-tree-0.2.5.tar.gz` & `tmp/streamlit-binary-tree-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.2.5.tar", last modified: Sat Jul 15 14:10:57 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.2.6.tar", last modified: Sat Jul 15 19:56:35 2023, max compression
```

## Comparing `streamlit-binary-tree-0.2.5.tar` & `streamlit-binary-tree-0.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.739947 streamlit-binary-tree-0.2.5/
--rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.5/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-15 14:10:57.739947 streamlit-binary-tree-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.5/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 14:10:57.741484 streamlit-binary-tree-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-07-15 14:10:46.000000 streamlit-binary-tree-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.467177 streamlit-binary-tree-0.2.5/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    28407 2023-07-15 14:10:35.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.430793 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.507929 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.430793 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.520398 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     8091 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
--rw-rw-rw-   0        0        0    15517 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.738436 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   667302 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405682 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
--rw-rw-rw-   0        0        0     5086 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js
--rw-rw-rw-   0        0        0    16927 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.499937 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 19:56:35.271579 streamlit-binary-tree-0.2.6/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-15 19:56:35.271579 streamlit-binary-tree-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-15 19:56:35.277580 streamlit-binary-tree-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-15 19:56:24.000000 streamlit-binary-tree-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:56:35.236571 streamlit-binary-tree-0.2.6/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    31109 2023-07-15 19:43:49.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:56:35.229570 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-15 19:56:35.256575 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-15 19:56:35.230570 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-15 19:56:35.258576 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     8091 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
+-rw-rw-rw-   0        0        0    15517 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-15 19:56:35.270579 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   667302 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405682 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
+-rw-rw-rw-   0        0        0     5086 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js
+-rw-rw-rw-   0        0        0    16927 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-15 19:56:35.254575 streamlit-binary-tree-0.2.6/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-15 19:56:35.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-15 19:56:35.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 19:56:35.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 19:56:35.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-15 19:56:35.000000 streamlit-binary-tree-0.2.6/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.2.5/LICENSE` & `streamlit-binary-tree-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/setup.py` & `streamlit-binary-tree-0.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-binary-tree",
-    version="0.2.5",
+    version="0.2.6",
     author="Abhishek Sharma",
     author_email="abhishek1995sharma@gmail.com",
     description="Interactive Binary Tree as a Streamlit component",
     long_description="Interactive Binary Tree as a Streamlit component",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
@@ -14,11 +14,12 @@
     classifiers=[],
     python_requires=">=3.6",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
         "streamlit >= 0.63",
-        "scikit-learn >= 1.3.0",
+        "scikit-learn",
         "numpy",
+        "pandas",
     ],
 )
```

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import streamlit.components.v1 as components
 from sklearn.tree import _tree
 from sklearn.tree._classes import DecisionTreeClassifier as DCTClass
 
 _RELEASE = True
 _DEBUG = True
 _NAME = "streamlit_binary_tree"
-SEPARATOR = " !@#$ "
+
+CATEGORICAL_INDICATOR = " !@#$ "
+BINARY_INDICATOR = " $#@! "
 
 # If release, use build or use dev
 if _RELEASE:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component(_NAME, path=build_dir)
 else:
@@ -340,23 +342,25 @@
                 if feature_names is not None
                 else str(feature_idx)
             )
             format = feature_value_formats[feature]
             tree_dict["feature"] = feature
             tree_dict["threshold"] = threshold
 
-            if SEPARATOR in feature:
-                left_condition = f"{feature.split(SEPARATOR)[0]} IS NOT {feature.split(SEPARATOR)[1]}"
+            if BINARY_INDICATOR in feature:
+                left_condition = f"{feature.split(BINARY_INDICATOR)[1]} is FALSE"
+            elif CATEGORICAL_INDICATOR in feature:
+                left_condition = f"{feature.split(CATEGORICAL_INDICATOR)[0]} IS NOT {feature.split(CATEGORICAL_INDICATOR)[1]}"
             else:
                 left_condition = f"{feature} ≤ {threshold:{format}}"
 
-            if SEPARATOR in feature:
-                right_condition = (
-                    f"{feature.split(SEPARATOR)[0]} IS {feature.split(SEPARATOR)[1]}"
-                )
+            if BINARY_INDICATOR in feature:
+                right_condition = f"{feature.split(BINARY_INDICATOR)[1]} is TRUE"
+            elif CATEGORICAL_INDICATOR in feature:
+                right_condition = f"{feature.split(CATEGORICAL_INDICATOR)[0]} IS {feature.split(CATEGORICAL_INDICATOR)[1]}"
             else:
                 right_condition = f"{feature} > {threshold:{format}}"
 
             tree_dict["left"] = {
                 "id": left_idx,
                 "condition": left_condition,
             }
@@ -679,51 +683,87 @@
         binary_formatting: Improves formatting of dict for binary classification.
             Blends outputted colors and shows only class 1 in line items.
 
     Examples:
         Examples with dummy data
 
         # Breast Cancer dataset (Binary Classification)
-        clf_breast_cancer = tree.DecisionTreeClassifier(
-            class_weight="balanced", max_depth=4, random_state=42
-        )
+
         dataset_breast_cancer = load_breast_cancer()
-        clf_breast_cancer = clf_breast_cancer.fit(
-            dataset_breast_cancer.data,
-            dataset_breast_cancer.target,
-        )
-        binary_tree_complete(
-            "test",
-            clf_breast_cancer,
+        features_breast_cancer = list(dataset_breast_cancer.feature_names)
+        target_breast_cancer = "target"
+        classes_breast_cancer = list(dataset_breast_cancer.target_names)
+        df_breast_cancer = pd.DataFrame(dataset_breast_cancer.data)
+        df_breast_cancer.columns = features_breast_cancer
+        df_breast_cancer[target_breast_cancer] = list(dataset_breast_cancer.target)
+
+        binary_tree(
+            "breast_cancer",
+            df_breast_cancer,
+            features_breast_cancer,
+            target_breast_cancer,
             show_node_ids=True,
-            style={"node_size": "120px"},
-            feature_names=list(dataset_breast_cancer.feature_names),
+            style={"node_size": "120px", "edge_size": "150px"},
             class_names=list(dataset_breast_cancer.target_names),
-            class_weights=get_balanced_class_weight(dataset_breast_cancer.target),
             binary_formatting=True,
         )
 
-        # Iris dataset (Multi-class Classification)
-        clf_iris = tree.DecisionTreeClassifier(
-            class_weight="balanced", max_depth=4, random_state=42
+        # Breast Cancer dataset with categorical features (Binary Classification)
+
+        dataset_breast_cancer2 = load_breast_cancer()
+        features_breast_cancer2 = list(dataset_breast_cancer2.feature_names)
+        target_breast_cancer2 = "target"
+        classes_breast_cancer2 = list(dataset_breast_cancer2.target_names)
+        df_breast_cancer2 = pd.DataFrame(dataset_breast_cancer2.data)
+        df_breast_cancer2.columns = features_breast_cancer2
+        df_breast_cancer2[target_breast_cancer2] = list(dataset_breast_cancer2.target)
+        df_breast_cancer2["mean compactness band"] = pd.cut(
+            df_breast_cancer2["mean compactness"],
+            [-np.Inf, 0.2, 0.5, 0.8, np.Inf],
+            labels=["<0.2", "0.2-0.5", "0.5-0.8", ">0.8"],
+        )
+        df_breast_cancer2["mean area flag"] = (df_breast_cancer2["mean area"] > 1000).map(
+            {True: 1, False: 0}
+        )
+        features_breast_cancer2 = [
+            "mean compactness band",
+            "mean area flag",
+        ]
+
+        binary_tree(
+            "breast_cancer2",
+            df_breast_cancer2,
+            features_breast_cancer2,
+            target_breast_cancer2,
+            show_node_ids=True,
+            style={"node_size": "120px", "edge_size": "150px"},
+            class_names=list(dataset_breast_cancer2.target_names),
+            binary_formatting=True,
         )
+
+        # Iris dataset (Multi-class Classification)
+
         dataset_iris = load_iris()
-        clf_iris = clf_iris.fit(
-            dataset_iris.data,
-            dataset_iris.target,
-        )
-        binary_tree_complete(
-            "test2",
-            clf_iris,
+        features_iris = list(dataset_iris.feature_names)
+        target_iris = "target"
+        classes_iris = list(dataset_iris.target_names)
+        df_iris = pd.DataFrame(dataset_iris.data)
+        df_iris.columns = features_iris
+        df_iris[target_iris] = list(dataset_iris.target)
+
+        binary_tree(
+            "iris",
+            df_iris,
+            features_iris,
+            target_iris,
             show_node_ids=True,
             style={"node_size": "120px"},
-            feature_names=list(dataset_iris.feature_names),
             class_names=list(dataset_iris.target_names),
-            class_weights=get_balanced_class_weight(dataset_iris.target),
         )
+
     """
     if clf_params is None:
         clf_params = {
             "class_weight": "balanced",
             "max_depth": 4,
             "min_samples_leaf": 0.005,
             "min_impurity_decrease": 1e-4,
@@ -734,18 +774,18 @@
     clf = clf.set_params(**clf_params)
 
     X = data_set[features]
     y = data_set[target]
 
     if categorise_binaries:
         for col in X.columns:
-            if X[col].nunique() == 2:
-                X[col] = X[col].astype("category")
+            if set(X[col].unique()) == {0, 1}:
+                X.rename(columns={col: f"{BINARY_INDICATOR}{col}"}, inplace=True)
 
-    X = pd.get_dummies(X, prefix_sep=SEPARATOR)
+    X = pd.get_dummies(X, prefix_sep=CATEGORICAL_INDICATOR)
     X.columns = [str(col) for col in X.columns]
 
     features = X.columns
 
     clf = clf.fit(X, y)
 
     if clf_params["class_weight"] == "balanced":
@@ -777,65 +817,86 @@
         style=style,
     )
     node_data = get_node_data(data, node_id)
     get_summary_streamlit(node_data, classes, spacing=spacing)
     st.markdown("---")
 
 
-# Debug code to help develop
+# ------------------------------------------------------------------------------------
+# Debugging is developing
 if _DEBUG:
     from sklearn.datasets import load_iris, load_breast_cancer
     from sklearn import tree
 
     st.set_page_config(layout="wide")
 
     # Breast Cancer dataset (Binary Classification)
     dataset_breast_cancer = load_breast_cancer()
     features_breast_cancer = list(dataset_breast_cancer.feature_names)
     target_breast_cancer = "target"
     classes_breast_cancer = list(dataset_breast_cancer.target_names)
     df_breast_cancer = pd.DataFrame(dataset_breast_cancer.data)
     df_breast_cancer.columns = features_breast_cancer
     df_breast_cancer[target_breast_cancer] = list(dataset_breast_cancer.target)
-    df_breast_cancer["mean compactness band"] = pd.cut(
-        df_breast_cancer["mean compactness"],
+
+    binary_tree(
+        "breast_cancer",
+        df_breast_cancer,
+        features_breast_cancer,
+        target_breast_cancer,
+        show_node_ids=True,
+        style={"node_size": "120px", "edge_size": "150px"},
+        class_names=list(dataset_breast_cancer.target_names),
+        binary_formatting=True,
+    )
+
+    # Breast Cancer dataset with categorical features (Binary Classification)
+    dataset_breast_cancer2 = load_breast_cancer()
+    features_breast_cancer2 = list(dataset_breast_cancer2.feature_names)
+    target_breast_cancer2 = "target"
+    classes_breast_cancer2 = list(dataset_breast_cancer2.target_names)
+    df_breast_cancer2 = pd.DataFrame(dataset_breast_cancer2.data)
+    df_breast_cancer2.columns = features_breast_cancer2
+    df_breast_cancer2[target_breast_cancer2] = list(dataset_breast_cancer2.target)
+    df_breast_cancer2["mean compactness band"] = pd.cut(
+        df_breast_cancer2["mean compactness"],
         [-np.Inf, 0.2, 0.5, 0.8, np.Inf],
         labels=["<0.2", "0.2-0.5", "0.5-0.8", ">0.8"],
     )
-    df_breast_cancer["mean area flag"] = (df_breast_cancer["mean area"] > 1000).map(
+    df_breast_cancer2["mean area flag"] = (df_breast_cancer2["mean area"] > 1000).map(
         {True: 1, False: 0}
     )
-    features_breast_cancer = [
+    features_breast_cancer2 = [
         "mean compactness band",
         "mean area flag",
     ]
 
     binary_tree(
-        "test",
-        df_breast_cancer,
-        features_breast_cancer,
-        target_breast_cancer,
+        "breast_cancer2",
+        df_breast_cancer2,
+        features_breast_cancer2,
+        target_breast_cancer2,
         show_node_ids=True,
         style={"node_size": "120px", "edge_size": "150px"},
-        class_names=list(dataset_breast_cancer.target_names),
+        class_names=list(dataset_breast_cancer2.target_names),
         binary_formatting=True,
     )
 
     # Iris dataset (Multi-class Classification)
 
-    # dataset_iris = load_iris()
-    # features_iris = list(dataset_iris.feature_names)
-    # target_iris = "target"
-    # classes_iris = list(dataset_iris.target_names)
-    # df_iris = pd.DataFrame(dataset_iris.data)
-    # df_iris.columns = features_iris
-    # df_iris[target_iris] = list(dataset_iris.target)
-
-    # binary_tree(
-    #     "test2",
-    #     df_iris,
-    #     features_iris,
-    #     target_iris,
-    #     show_node_ids=True,
-    #     style={"node_size": "120px"},
-    #     class_names=list(dataset_iris.target_names),
-    # )
+    dataset_iris = load_iris()
+    features_iris = list(dataset_iris.feature_names)
+    target_iris = "target"
+    classes_iris = list(dataset_iris.target_names)
+    df_iris = pd.DataFrame(dataset_iris.data)
+    df_iris.columns = features_iris
+    df_iris[target_iris] = list(dataset_iris.target)
+
+    binary_tree(
+        "iris",
+        df_iris,
+        features_iris,
+        target_iris,
+        show_node_ids=True,
+        style={"node_size": "120px"},
+        class_names=list(dataset_iris.target_names),
+    )
```

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js.map` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.2.6/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

