# Comparing `tmp/streamlit-binary-tree-0.2.4.tar.gz` & `tmp/streamlit-binary-tree-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.2.4.tar", last modified: Sat Jul 15 10:50:27 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.2.5.tar", last modified: Sat Jul 15 14:10:57 2023, max compression
```

## Comparing `streamlit-binary-tree-0.2.4.tar` & `streamlit-binary-tree-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.979914 streamlit-binary-tree-0.2.4/
--rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-15 10:50:27.979914 streamlit-binary-tree-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.4/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 10:50:27.986423 streamlit-binary-tree-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-07-15 10:50:23.000000 streamlit-binary-tree-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.948003 streamlit-binary-tree-0.2.4/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    24750 2023-07-15 10:47:40.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.941001 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.963910 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.942001 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.965910 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     8091 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
--rw-rw-rw-   0        0        0    15517 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.977913 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   667302 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405682 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
--rw-rw-rw-   0        0        0     5066 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js
--rw-rw-rw-   0        0        0    16890 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.961909 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.739947 streamlit-binary-tree-0.2.5/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-15 14:10:57.739947 streamlit-binary-tree-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-15 14:10:57.741484 streamlit-binary-tree-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-15 14:10:46.000000 streamlit-binary-tree-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.467177 streamlit-binary-tree-0.2.5/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    28407 2023-07-15 14:10:35.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.430793 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.507929 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.430793 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.520398 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     8091 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
+-rw-rw-rw-   0        0        0    15517 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.738436 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   667302 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405682 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
+-rw-rw-rw-   0        0        0     5086 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js
+-rw-rw-rw-   0        0        0    16927 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-15 14:04:00.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-15 14:10:57.499937 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-15 14:10:57.000000 streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.2.4/LICENSE` & `streamlit-binary-tree-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.4/setup.py` & `streamlit-binary-tree-0.2.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-binary-tree",
-    version="0.2.4",
+    version="0.2.5",
     author="Abhishek Sharma",
     author_email="abhishek1995sharma@gmail.com",
     description="Interactive Binary Tree as a Streamlit component",
     long_description="Interactive Binary Tree as a Streamlit component",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from collections import defaultdict
 import os
 import math
+import pandas as pd
 import numpy as np
 from typing import List
 import streamlit as st
 import streamlit.components.v1 as components
 from sklearn.tree import _tree
 from sklearn.tree._classes import DecisionTreeClassifier as DCTClass
 
 _RELEASE = True
 _DEBUG = True
 _NAME = "streamlit_binary_tree"
+SEPARATOR = " !@#$ "
 
 # If release, use build or use dev
 if _RELEASE:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component(_NAME, path=build_dir)
 else:
@@ -148,15 +151,15 @@
     binary_formatting=False,
 ):
     """Export a decision tree in dict format.
 
     Args:
         tree (decision tree classifier): The decision tree to be exported
         feature_names (list of strings, optional): Names of each of the features. Defaults to None.
-        feature_value_formats (list of strings, optional): Formats for each feature value (used in Connectors). Defaults to "0.2f".
+        feature_value_formats (defaultDict, optional): Formats for each feature value (used in Connectors). Defaults to "0.2f".
         class_names (list of strings, optional): Names of each of the classes. Defaults to None.
         class_colors (list of strings, optional): Hex of each of the class colors. Defaults to default class colors.
             class_colors = [
                 "#198038",
                 "#fa4d56",
                 "#1192e8",
                 "#6929c4",
@@ -213,15 +216,15 @@
         clf = clf.fit(iris.data, iris.target)
         d = tree.export_dict(clf)
         j = json.dumps(d, indent=4)
     """
     tree_ = tree.tree_
     master_list = []
     if feature_value_formats is None:
-        feature_value_formats = ["0.2f"] * tree.max_features_
+        feature_value_formats = defaultdict(lambda: "0.2f")
     if class_colors is None:
         class_colors = [
             "#198038",
             "#fa4d56",
             "#1192e8",
             "#6929c4",
             "#b28600",
@@ -328,26 +331,42 @@
                 f"{event_header_val}: {bads_value}",
             ],
             "path": path,
             "color": color,
         }
 
         if hasChildren:
-            feature = feature_names[feature_idx] if feature_names else str(feature_idx)
-            format = feature_value_formats[feature_idx]
+            feature = (
+                feature_names[feature_idx]
+                if feature_names is not None
+                else str(feature_idx)
+            )
+            format = feature_value_formats[feature]
             tree_dict["feature"] = feature
             tree_dict["threshold"] = threshold
 
+            if SEPARATOR in feature:
+                left_condition = f"{feature.split(SEPARATOR)[0]} IS NOT {feature.split(SEPARATOR)[1]}"
+            else:
+                left_condition = f"{feature} ≤ {threshold:{format}}"
+
+            if SEPARATOR in feature:
+                right_condition = (
+                    f"{feature.split(SEPARATOR)[0]} IS {feature.split(SEPARATOR)[1]}"
+                )
+            else:
+                right_condition = f"{feature} > {threshold:{format}}"
+
             tree_dict["left"] = {
                 "id": left_idx,
-                "condition": f"{feature} ≤ {threshold:{format}}",
+                "condition": left_condition,
             }
             tree_dict["right"] = {
                 "id": right_idx,
-                "condition": f"{feature} > {threshold:{format}}",
+                "condition": right_condition,
             }
 
         master_list.append(tree_dict)
 
         if hasChildren:
             recur(
                 left_idx,
@@ -415,15 +434,15 @@
         for c in classes:
             st.markdown(
                 f"""<span style="background-color: {c['color']}; padding:5px;">{c['name']}</span>""",
                 unsafe_allow_html=True,
             )
 
 
-def binary_tree(
+def binary_tree_component(
     data: List[dict],
     key: str = None,
     expanded_depth: int = 3,
     show_node_ids: bool = True,
     style: dict = None,
 ):
     """
@@ -575,38 +594,62 @@
         show_node_ids=show_node_ids,
         style=style,
     )
 
     return component_value
 
 
-def binary_tree_complete(
+def binary_tree(
     key,
-    clf,
+    data_set,
+    features,
+    target,
+    clf_params=None,
+    feature_value_formats=None,
+    categorise_binaries=True,
+    class_names=None,
+    class_colors=None,
     show_node_ids=True,
     expanded_depth=3,
     style=None,
     spacing=[3, 2],
-    feature_names=None,
-    feature_value_formats=None,
-    class_names=None,
-    class_colors=None,
-    class_weights=None,
     sample_header="Samples",
     event_header="Events",
     sample_perc_precision=1,
     event_perc_precision=1,
     percentage_first=True,
     binary_formatting=False,
 ):
-    """_summary_
+    """Creates an interactive binary tree.
 
     Args:
         key (str): Name of tree
-        clf (decision tree classifier): The decision tree to be shown
+        data_set (DataFrame): The data to make the decision tree on
+        features (list of str): Features of the tree
+        target (str): Target of the tree
+        clf_params (dict): Parameters for the classifier
+        feature_value_formats (defaultDict, optional): Formats for each feature value (used in Connectors). Defaults to "0.2f".
+        categorise_binaries (bool, optional): Whether to treat binary features as categories. Defaults to True.
+        class_names (list of strings, optional): Names of each of the classes. Defaults to None.
+        class_colors (list of strings, optional): Hex of each of the class colors. Defaults to default class colors.
+            class_colors = [
+                "#198038",
+                "#fa4d56",
+                "#1192e8",
+                "#6929c4",
+                "#b28600",
+                "#009d9a",
+                "#9f1853",
+                "#002d9c",
+                "#ee538b",
+                "#570408",
+                "#005d5d",
+                "#8a3800",
+                "#a56eff",
+            ]
         expanded_depth (int, optional): Initial expanded depth of the tree. Defaults to 3.
         show_node_ids (bool, optional): Whether node ids are shown at the left of every single node. Defaults to True.
         style (_type_, optional): Styling info: font style, color, spacing. Defaults to default_style.
             default_style = {
                 "max_height": "2400px",
                 "padding_quantum": "5px",
                 "edge_size": "100px",
@@ -623,59 +666,114 @@
                 "text_outline_color": "#fff",
                 "text_outline_alpha": "0.4",
                 "button_color": "#70b4c2",
                 "button_hover_color": "#2d6186",
                 "transition_time": "0.7s",
             }
         spacing (list of 2 ints): Input to streamlit column spacing for summary. Defaults to [3,2]
-        feature_names (list of strings, optional): Names of each of the features. Defaults to None.
-        feature_value_formats (list of strings, optional): Formats for each feature value (used in Connectors). Defaults to "0.2f".
-        class_names (list of strings, optional): Names of each of the classes. Defaults to None.
-        class_colors (list of strings, optional): Hex of each of the class colors. Defaults to default class colors.
-            class_colors = [
-                "#198038",
-                "#fa4d56",
-                "#1192e8",
-                "#6929c4",
-                "#b28600",
-                "#009d9a",
-                "#9f1853",
-                "#002d9c",
-                "#ee538b",
-                "#570408",
-                "#005d5d",
-                "#8a3800",
-                "#a56eff",
-            ]
         class_weights (dict of floats, optional): Dict with weights of the classes. Defaults to 1.
         sample_header (str, optional): Header for samples line item. Defaults to "Samples".
         event_header (str, optional): Header for events line item. Defaults to "Events".
         sample_perc_precision (int, optional): Precision of % of samples line item. Defaults to 1.
         event_perc_precision (int, optional): Precision of % of events line item. Defaults to 1.
         percentage_first: Whether to show % first. Defaults to True.
         binary_formatting: Improves formatting of dict for binary classification.
             Blends outputted colors and shows only class 1 in line items.
+
+    Examples:
+        Examples with dummy data
+
+        # Breast Cancer dataset (Binary Classification)
+        clf_breast_cancer = tree.DecisionTreeClassifier(
+            class_weight="balanced", max_depth=4, random_state=42
+        )
+        dataset_breast_cancer = load_breast_cancer()
+        clf_breast_cancer = clf_breast_cancer.fit(
+            dataset_breast_cancer.data,
+            dataset_breast_cancer.target,
+        )
+        binary_tree_complete(
+            "test",
+            clf_breast_cancer,
+            show_node_ids=True,
+            style={"node_size": "120px"},
+            feature_names=list(dataset_breast_cancer.feature_names),
+            class_names=list(dataset_breast_cancer.target_names),
+            class_weights=get_balanced_class_weight(dataset_breast_cancer.target),
+            binary_formatting=True,
+        )
+
+        # Iris dataset (Multi-class Classification)
+        clf_iris = tree.DecisionTreeClassifier(
+            class_weight="balanced", max_depth=4, random_state=42
+        )
+        dataset_iris = load_iris()
+        clf_iris = clf_iris.fit(
+            dataset_iris.data,
+            dataset_iris.target,
+        )
+        binary_tree_complete(
+            "test2",
+            clf_iris,
+            show_node_ids=True,
+            style={"node_size": "120px"},
+            feature_names=list(dataset_iris.feature_names),
+            class_names=list(dataset_iris.target_names),
+            class_weights=get_balanced_class_weight(dataset_iris.target),
+        )
     """
+    if clf_params is None:
+        clf_params = {
+            "class_weight": "balanced",
+            "max_depth": 4,
+            "min_samples_leaf": 0.005,
+            "min_impurity_decrease": 1e-4,
+            "random_state": 42,
+        }
+
+    clf = tree.DecisionTreeClassifier()
+    clf = clf.set_params(**clf_params)
+
+    X = data_set[features]
+    y = data_set[target]
+
+    if categorise_binaries:
+        for col in X.columns:
+            if X[col].nunique() == 2:
+                X[col] = X[col].astype("category")
+
+    X = pd.get_dummies(X, prefix_sep=SEPARATOR)
+    X.columns = [str(col) for col in X.columns]
+
+    features = X.columns
+
+    clf = clf.fit(X, y)
+
+    if clf_params["class_weight"] == "balanced":
+        class_weights = get_balanced_class_weight(y)
+    else:
+        class_weights = clf_params["class_weight"]
+
     data, classes = export_dict(
         clf,
-        feature_names=feature_names,
+        feature_names=features,
         feature_value_formats=feature_value_formats,
         class_names=class_names,
         class_colors=class_colors,
         class_weights=class_weights,
         sample_header=sample_header,
         event_header=event_header,
         sample_perc_precision=sample_perc_precision,
         event_perc_precision=event_perc_precision,
         percentage_first=percentage_first,
         binary_formatting=binary_formatting,
     )
 
     st.markdown("---")
-    node_id = binary_tree(
+    node_id = binary_tree_component(
         data,
         key=key,
         show_node_ids=show_node_ids,
         expanded_depth=expanded_depth,
         style=style,
     )
     node_data = get_node_data(data, node_id)
@@ -687,44 +785,57 @@
 if _DEBUG:
     from sklearn.datasets import load_iris, load_breast_cancer
     from sklearn import tree
 
     st.set_page_config(layout="wide")
 
     # Breast Cancer dataset (Binary Classification)
-    clf_breast_cancer = tree.DecisionTreeClassifier(
-        class_weight="balanced", max_depth=4, random_state=42
-    )
     dataset_breast_cancer = load_breast_cancer()
-    clf_breast_cancer = clf_breast_cancer.fit(
-        dataset_breast_cancer.data,
-        dataset_breast_cancer.target,
-    )
-    binary_tree_complete(
+    features_breast_cancer = list(dataset_breast_cancer.feature_names)
+    target_breast_cancer = "target"
+    classes_breast_cancer = list(dataset_breast_cancer.target_names)
+    df_breast_cancer = pd.DataFrame(dataset_breast_cancer.data)
+    df_breast_cancer.columns = features_breast_cancer
+    df_breast_cancer[target_breast_cancer] = list(dataset_breast_cancer.target)
+    df_breast_cancer["mean compactness band"] = pd.cut(
+        df_breast_cancer["mean compactness"],
+        [-np.Inf, 0.2, 0.5, 0.8, np.Inf],
+        labels=["<0.2", "0.2-0.5", "0.5-0.8", ">0.8"],
+    )
+    df_breast_cancer["mean area flag"] = (df_breast_cancer["mean area"] > 1000).map(
+        {True: 1, False: 0}
+    )
+    features_breast_cancer = [
+        "mean compactness band",
+        "mean area flag",
+    ]
+
+    binary_tree(
         "test",
-        clf_breast_cancer,
+        df_breast_cancer,
+        features_breast_cancer,
+        target_breast_cancer,
         show_node_ids=True,
-        style={"node_size": "120px"},
-        feature_names=list(dataset_breast_cancer.feature_names),
+        style={"node_size": "120px", "edge_size": "150px"},
         class_names=list(dataset_breast_cancer.target_names),
-        class_weights=get_balanced_class_weight(dataset_breast_cancer.target),
         binary_formatting=True,
     )
 
     # Iris dataset (Multi-class Classification)
-    clf_iris = tree.DecisionTreeClassifier(
-        class_weight="balanced", max_depth=4, random_state=42
-    )
-    dataset_iris = load_iris()
-    clf_iris = clf_iris.fit(
-        dataset_iris.data,
-        dataset_iris.target,
-    )
-    binary_tree_complete(
-        "test2",
-        clf_iris,
-        show_node_ids=True,
-        style={"node_size": "120px"},
-        feature_names=list(dataset_iris.feature_names),
-        class_names=list(dataset_iris.target_names),
-        class_weights=get_balanced_class_weight(dataset_iris.target),
-    )
+
+    # dataset_iris = load_iris()
+    # features_iris = list(dataset_iris.feature_names)
+    # target_iris = "target"
+    # classes_iris = list(dataset_iris.target_names)
+    # df_iris = pd.DataFrame(dataset_iris.data)
+    # df_iris.columns = features_iris
+    # df_iris[target_iris] = list(dataset_iris.target)
+
+    # binary_tree(
+    #     "test2",
+    #     df_iris,
+    #     features_iris,
+    #     target_iris,
+    #     show_node_ids=True,
+    #     style={"node_size": "120px"},
+    #     class_names=list(dataset_iris.target_names),
+    # )
```

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'entrypoints'": "{insert: [(3, 'static/js/main.475c611d.chunk.js')], delete: [3]}",*

 * * "'files'": "{'main.js': './static/js/main.475c611d.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.475c611d.chunk.js.map'}"}*

```diff
@@ -1,19 +1,19 @@
 {
     "entrypoints": [
         "static/js/runtime-main.624f085e.js",
         "static/js/2.41f15472.chunk.js",
         "static/css/main.3a4c9b92.chunk.css",
-        "static/js/main.50b0a73e.chunk.js"
+        "static/js/main.475c611d.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.3a4c9b92.chunk.css",
-        "main.js": "./static/js/main.50b0a73e.chunk.js",
-        "main.js.map": "./static/js/main.50b0a73e.chunk.js.map",
+        "main.js": "./static/js/main.475c611d.chunk.js",
+        "main.js.map": "./static/js/main.475c611d.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.624f085e.js",
         "runtime-main.js.map": "./static/js/runtime-main.624f085e.js.map",
         "static/css/main.3a4c9b92.chunk.css.map": "./static/css/main.3a4c9b92.chunk.css.map",
         "static/js/2.41f15472.chunk.js": "./static/js/2.41f15472.chunk.js",
         "static/js/2.41f15472.chunk.js.LICENSE.txt": "./static/js/2.41f15472.chunk.js.LICENSE.txt",
         "static/js/2.41f15472.chunk.js.map": "./static/js/2.41f15472.chunk.js.map"
     }
```

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style><link href="./static/css/main.3a4c9b92.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.41f15472.chunk.js"></script><script src="./static/js/main.50b0a73e.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style><link href="./static/css/main.3a4c9b92.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.41f15472.chunk.js"></script><script src="./static/js/main.475c611d.chunk.js"></script></body></html>
```

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -54,21 +54,22 @@
                                 }))
                             })]
                         })
                     })
                 },
                 v = function(e) {
                     var t = e.id,
-                        n = (e.isLeft, Object(o.useContext)(O).data.find((function(e) {
+                        n = e.isLeft,
+                        r = Object(o.useContext)(O).data.find((function(e) {
                             return e.node_id === t
-                        })));
+                        }));
                     return Object(m.jsx)(m.Fragment, {
                         children: Object(m.jsx)("div", {
                             className: "edge-content",
-                            children: n.left.condition
+                            children: n ? r.left.condition : r.right.condition
                         })
                     })
                 },
                 p = function e(t) {
                     var n = t.id,
                         r = t.depth,
                         c = Object(o.useContext)(O),
@@ -220,8 +221,8 @@
             }), document.getElementById("root"))
         }
     },
     [
         [29, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.50b0a73e.chunk.js.map
+//# sourceMappingURL=main.475c611d.chunk.js.map
```

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8357694429122999%*

 * *Differences: {"'file'": "'static/js/main.475c611d.chunk.js'",*

 * * "'mappings'": "'2RAEMA,EAAoB,CAAC,EACdC,EAAcC,wBAAcF,G,OCwC1BG,EAtCK,SAAHC,GAAwB,IAAlBC,EAAED,EAAFC,GACfC,EAAOC,qBAAWN,GAClBO,EAAqBF,EAAKE,KAC1BC,EAAyBH,EAAKG,cAC9BC,EAAYF,EAAKG,MAAK,SAACC,GAAC,OAAKA,EAAEC,UAAYR,CAAE,IAMnD,OACES,cAAAC,WAAA,CAAAC,SACEC,eAAA,OAAKC,UAAU,OAAMF,SAAA,CAClBP,GACCK,cAAA,OACEI,UAAU,oBACVC,QAAS,SAACC,GAVA,IAACC,IAWGhB,EAVtBiB,YAAUC,kBAAkBF,EAWpB,EACAG,MAAO,CAAEC,gBAAiBf,EAAWgB,OAAQV,SAE7CF,cAAA,OAAAE,SAAMN,EAAWG,YAGrBC,cAAA,OAAKI,UAAU […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.50b0a73e.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.475c611d.chunk.js",
+    "mappings": "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",
     "names": [
         "default_args",
         "ArgsContext",
         "createContext",
         "NodeContent",
         "_ref",
         "id",
@@ -33,26 +33,26 @@
         "map",
         "content",
         "i",
         "EdgeContent",
         "isLeft",
         "left",
         "condition",
+        "right",
         "Node",
         "depth",
         "expanded",
         "expanded_depth",
         "_useState",
         "useState",
         "childrenVisible",
         "_useState2",
         "_slicedToArray",
         "setChildrenVisible",
         "hasChildren",
-        "right",
         "childrenVisibleStyle",
         "opacity",
         "maxHeight",
         "maxWidth",
         "overflowX",
         "transform",
         "invertColor",
@@ -158,14 +158,14 @@
         "Node.tsx",
         "Tree.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "import { createContext } from \"react\"\r\n\r\nconst default_args: any = {}\r\nexport const ArgsContext = createContext(default_args)\r\n",
         "import { useContext } from \"react\"\r\nimport { Streamlit } from \"streamlit-component-lib\"\r\nimport { ArgsContext } from \"./ArgsContext\"\r\nimport type { NodeObject, NodeId } from \"./Node\"\r\n\r\nconst NodeContent = ({ id }: NodeId) => {\r\n  const args = useContext(ArgsContext)\r\n  const data: NodeObject[] = args.data\r\n  const show_node_ids: boolean = args.show_node_ids\r\n  const node_data = data.find((a) => a.node_id === id)\r\n\r\n  const updateValue = (value: number) => {\r\n    Streamlit.setComponentValue(value)\r\n  }\r\n\r\n  return (\r\n    <>\r\n      <div className=\"node\">\r\n        {show_node_ids && (\r\n          <div\r\n            className=\"node-content-left\"\r\n            onClick={(e) => {\r\n              updateValue(id)\r\n            }}\r\n            style={{ backgroundColor: node_data!.color }}\r\n          >\r\n            <div>{node_data!.node_id}</div>\r\n          </div>\r\n        )}\r\n        <div className=\"node-content-right\">\r\n          {node_data!.contents.map(function (content, i) {\r\n            return (\r\n              <div className=\"node-content-right-item\" key={i}>\r\n                {content}\r\n              </div>\r\n            )\r\n          })}\r\n        </div>\r\n      </div>\r\n    </>\r\n  )\r\n}\r\n\r\nexport default NodeContent\r\n",
-        "import { useContext } from \"react\"\r\nimport { ArgsContext } from \"./ArgsContext\"\r\nimport type { NodeObject } from \"./Node\"\r\n\r\ninterface EdgeType {\r\n  id: number\r\n  isLeft: boolean\r\n}\r\n\r\nconst EdgeContent = ({ id, isLeft }: EdgeType) => {\r\n  const args = useContext(ArgsContext)\r\n  const data: NodeObject[] = args.data\r\n  const node_data = data.find((a) => a.node_id === id)\r\n\r\n  return (\r\n    <>\r\n      <div className=\"edge-content\">\r\n        {isLeft ? node_data!.left.condition : node_data!.left.condition}\r\n      </div>\r\n    </>\r\n  )\r\n}\r\n\r\nexport default EdgeContent\r\n",
+        "import { useContext } from \"react\"\r\nimport { ArgsContext } from \"./ArgsContext\"\r\nimport type { NodeObject } from \"./Node\"\r\n\r\ninterface EdgeType {\r\n  id: number\r\n  isLeft: boolean\r\n}\r\n\r\nconst EdgeContent = ({ id, isLeft }: EdgeType) => {\r\n  const args = useContext(ArgsContext)\r\n  const data: NodeObject[] = args.data\r\n  const node_data = data.find((a) => a.node_id === id)\r\n\r\n  return (\r\n    <>\r\n      <div className=\"edge-content\">\r\n        {isLeft ? node_data!.left.condition : node_data!.right.condition}\r\n      </div>\r\n    </>\r\n  )\r\n}\r\n\r\nexport default EdgeContent\r\n",
         "import { useState, useContext } from \"react\"\r\nimport { ArgsContext } from \"./ArgsContext\"\r\n\r\nimport NodeContent from \"./NodeContent\"\r\nimport EdgeContent from \"./EdgeContent\"\r\n\r\nexport interface NodeObject {\r\n  node_id: number\r\n  left: {\r\n    id: number\r\n    condition: string\r\n  }\r\n  right: {\r\n    id: number\r\n    condition: string\r\n  }\r\n  contents: string[]\r\n  color: string\r\n  childrenVisible: boolean\r\n}\r\n\r\nexport interface NodeId {\r\n  id: number\r\n  depth: number\r\n}\r\n\r\nconst Node = ({ id, depth }: NodeId) => {\r\n  const args = useContext(ArgsContext)\r\n  const data: NodeObject[] = args.data\r\n  const expanded = depth < args.expanded_depth\r\n\r\n  const node_data = data.find((a) => a.node_id === id)\r\n  const [childrenVisible, setChildrenVisible] = useState(\r\n    node_data!.childrenVisible != null ? node_data!.childrenVisible : expanded\r\n  )\r\n\r\n  node_data!.childrenVisible = childrenVisible\r\n\r\n  const hasChildren = node_data!.left != null && node_data!.right != null\r\n  const childrenVisibleStyle = childrenVisible\r\n    ? {}\r\n    : ({\r\n        opacity: 0,\r\n        maxHeight: 0,\r\n        maxWidth: 0,\r\n        overflowX: \"hidden\",\r\n      } as React.CSSProperties)\r\n\r\n  // console.log(\"id \", id, node_data, hasChildren)\r\n\r\n  function switchChildrenVisible() {\r\n    setChildrenVisible(!childrenVisible)\r\n  }\r\n\r\n  return (\r\n    <>\r\n      <NodeContent id={id} depth={depth} />\r\n      {hasChildren && (\r\n        <div\r\n          className=\"child-button\"\r\n          onClick={(e) => switchChildrenVisible()}\r\n          style={childrenVisible ? {} : { transform: \"scaleX(-1)\" }}\r\n        ></div>\r\n      )}\r\n\r\n      {hasChildren && (\r\n        <ul style={childrenVisibleStyle}>\r\n          <li>\r\n            <EdgeContent id={id} isLeft={true} key={id} />\r\n            <Node\r\n              id={node_data!.left.id}\r\n              key={node_data!.left.id}\r\n              depth={depth + 1}\r\n            />\r\n          </li>\r\n          <li>\r\n            <EdgeContent id={id} isLeft={false} key={id} />\r\n            <Node\r\n              id={node_data!.right.id}\r\n              key={node_data!.right.id}\r\n              depth={depth + 1}\r\n            />\r\n          </li>\r\n        </ul>\r\n      )}\r\n    </>\r\n  )\r\n}\r\n\r\nexport default Node\r\n",
         "import {\n  ComponentProps,\n  Streamlit,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { useEffect, useState, useRef } from \"react\"\n\nimport downloadjs from \"downloadjs\"\nimport html2canvas from \"html2canvas\"\nimport { ArgsContext } from \"./ArgsContext\"\nimport Node from \"./Node\"\nimport \"./Node.scss\"\n\ninterface styleType {\n  button_color: string\n  button_hover_color: string\n  edge_color: string\n  edge_hover_color: string\n  edge_size: string\n  font_family: string\n  font_size: string\n  max_height: string\n  node_border_color: string\n  node_color: string\n  node_hover_color: string\n  node_size: string\n  padding_quantum: string\n  text_color: string\n  text_hover_color: string\n  text_outline_alpha: string\n  text_outline_color: string\n  text_outline_color_mix: string\n  transition_time: string\n}\n\nconst invertColor = (hex: string) => {\n  if (hex.indexOf(\"#\") === 0) {\n    hex = hex.slice(1)\n  }\n  // convert 3-digit hex to 6-digits.\n  if (hex.length === 3) {\n    hex = hex[0] + hex[0] + hex[1] + hex[1] + hex[2] + hex[2]\n  }\n  if (hex.length !== 6) {\n    console.log(\"dfs\", hex)\n    throw new Error(\"Invalid HEX color.\")\n  }\n  // invert color components\n  var r = (255 - parseInt(hex.slice(0, 2), 16)).toString(16),\n    g = (255 - parseInt(hex.slice(2, 4), 16)).toString(16),\n    b = (255 - parseInt(hex.slice(4, 6), 16)).toString(16)\n  // pad each with zeros and return\n  return \"#\" + padZero(r, 2) + padZero(g, 2) + padZero(b, 2)\n}\n\nconst colorToRGB = (hex: string) => {\n  if (hex.indexOf(\"#\") === 0) {\n    hex = hex.slice(1)\n  }\n  // convert 3-digit hex to 6-digits.\n  if (hex.length === 3) {\n    hex = hex[0] + hex[0] + hex[1] + hex[1] + hex[2] + hex[2]\n  }\n  if (hex.length !== 6) {\n    throw new Error(\"Invalid Alpha-HEX color.\")\n  }\n  // break color components\n  var r = parseInt(hex.slice(0, 2), 16),\n    g = parseInt(hex.slice(2, 4), 16),\n    b = parseInt(hex.slice(4, 6), 16)\n  // pad each with zeros and return\n  var rgb = `${r}, ${g}, ${b}`\n  return rgb\n}\n\nconst padZero = (str: string, len: number) => {\n  len = len || 2\n  var zeros = new Array(len).join(\"0\")\n  return (zeros + str).slice(-len)\n}\n\nconst setStyle = (originalStyle: styleType, theme: any) => {\n  const style = { ...originalStyle }\n  style.text_outline_color_mix = `rgba(${colorToRGB(\n    style.text_outline_color\n  )}, ${style.text_outline_alpha})`\n\n  if (theme.base === \"dark\") {\n    style.button_color = invertColor(style.button_color)\n    style.button_hover_color = invertColor(style.button_hover_color)\n    style.edge_color = invertColor(style.edge_color)\n    style.edge_hover_color = invertColor(style.edge_hover_color)\n    style.node_border_color = invertColor(style.node_border_color)\n    style.node_color = invertColor(style.node_color)\n    style.node_hover_color = invertColor(style.node_hover_color)\n    style.text_color = invertColor(style.text_color)\n    style.text_hover_color = invertColor(style.text_hover_color)\n    style.text_outline_color = invertColor(style.text_outline_color)\n    style.text_outline_color_mix = `rgba(${colorToRGB(\n      style.text_outline_color\n    )}, ${style.text_outline_alpha})`\n  }\n  Object.entries(style).forEach(([key, value]) => {\n    key = `--${key.replaceAll(\"_\", \"-\")}`\n    document.getElementById(\"root\")!.style.setProperty(key, value)\n  })\n  document\n    .getElementById(\"root\")!\n    .style.setProperty(\"--backgroundColor\", theme.backgroundColor)\n}\n\nconst Tree = (props: ComponentProps) => {\n  const args = props.args\n  const key = args.key\n  const style: styleType = args.style\n  const theme = props.theme\n  const [lastFrameHeight, setLastFrameHeight] = useState(0)\n  const treeRef: any = useRef(null)\n\n  setStyle(style, theme)\n\n  useEffect(() => {\n    const intervalId = setInterval(() => {\n      if (treeRef.current != null) {\n        setLastFrameHeight(treeRef.current!.clientHeight)\n      }\n    }, 20)\n    Streamlit.setFrameHeight()\n    // console.log(\n    //   lastFrameHeight,\n    //   Streamlit.lastFrameHeight,\n    //   treeRef.current!.clientHeight\n    // )\n    return () => clearInterval(intervalId)\n  }, [lastFrameHeight])\n\n  const treeToPng = async () => {\n    const element = document.querySelector(\".tree\")!\n    console.log(element.scrollWidth, element.clientWidth)\n    const useWidth = element.scrollWidth\n    const canvas = await html2canvas(document.querySelector(\".tree\")!, {\n      width: useWidth,\n      windowWidth: useWidth,\n      scale: 4,\n    })\n    const dataURL = canvas.toDataURL(\"image/jpg\")\n    downloadjs(dataURL, `${key}.jpg`, \"image/jpg\")\n  }\n\n  // const style: React.CSSProperties = {}\n\n  return (\n    <ArgsContext.Provider value={args}>\n      <button className=\"download-button\" onClick={(e) => treeToPng()}>\n        Download as Image\n      </button>\n      <div className=\"tree\" ref={treeRef}>\n        <ul className=\"rootNode\">\n          <li>\n            <Node id={0} depth={0} />\n          </li>\n        </ul>\n      </div>\n      <br />\n    </ArgsContext.Provider>\n  )\n}\n\nexport default withStreamlitConnection(Tree)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport { StreamlitProvider } from \"streamlit-component-lib-react-hooks\"\nimport Tree from \"./Tree\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <StreamlitProvider>\n      <Tree />\n    </StreamlitProvider>\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.2.5/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 streamlit_binary_tree/frontend/build/asset-manifest.json
 streamlit_binary_tree/frontend/build/index.html
 streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
 streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
 streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
 streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
 streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
-streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js
-streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map
+streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js
+streamlit_binary_tree/frontend/build/static/js/main.475c611d.chunk.js.map
 streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
 streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
```

