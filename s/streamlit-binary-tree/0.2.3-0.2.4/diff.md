# Comparing `tmp/streamlit-binary-tree-0.2.3.tar.gz` & `tmp/streamlit-binary-tree-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.2.3.tar", last modified: Sat Jul 15 10:38:17 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.2.4.tar", last modified: Sat Jul 15 10:50:27 2023, max compression
```

## Comparing `streamlit-binary-tree-0.2.3.tar` & `streamlit-binary-tree-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.742762 streamlit-binary-tree-0.2.3/
--rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-15 10:38:17.742762 streamlit-binary-tree-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.3/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 10:38:17.749764 streamlit-binary-tree-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-07-15 10:38:12.000000 streamlit-binary-tree-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.702470 streamlit-binary-tree-0.2.3/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    21699 2023-07-15 10:37:39.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.695640 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.719475 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.696639 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.721475 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     8091 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
--rw-rw-rw-   0        0        0    15517 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.741762 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   667302 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405682 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
--rw-rw-rw-   0        0        0     5066 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js
--rw-rw-rw-   0        0        0    16890 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.717475 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.979914 streamlit-binary-tree-0.2.4/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-15 10:50:27.979914 streamlit-binary-tree-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-15 10:50:27.986423 streamlit-binary-tree-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-15 10:50:23.000000 streamlit-binary-tree-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.948003 streamlit-binary-tree-0.2.4/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    24750 2023-07-15 10:47:40.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.941001 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.963910 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.942001 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.965910 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     8091 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
+-rw-rw-rw-   0        0        0    15517 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.977913 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   667302 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405682 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
+-rw-rw-rw-   0        0        0     5066 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js
+-rw-rw-rw-   0        0        0    16890 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-15 10:50:27.961909 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-15 10:50:27.000000 streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.2.3/LICENSE` & `streamlit-binary-tree-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/setup.py` & `streamlit-binary-tree-0.2.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-binary-tree",
-    version="0.2.3",
+    version="0.2.4",
     author="Abhishek Sharma",
     author_email="abhishek1995sharma@gmail.com",
     description="Interactive Binary Tree as a Streamlit component",
     long_description="Interactive Binary Tree as a Streamlit component",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,42 +146,42 @@
     event_perc_precision=1,
     percentage_first=True,
     binary_formatting=False,
 ):
     """Export a decision tree in dict format.
 
     Args:
-    decision_tree (decision tree classifier): The decision tree to be exported
-    feature_names (list of strings, optional): Names of each of the features. Defaults to None.
-    feature_value_formats (list of strings, optional): Formats for each feature value (used in Connectors). Defaults to "0.2f".
-    class_names (list of strings, optional): Names of each of the classes. Defaults to None.
-    class_colors (list of strings, optional): Hex of each of the class colors. Defaults to default class colors.
-        class_colors = [
-            "#198038",
-            "#fa4d56",
-            "#1192e8",
-            "#6929c4",
-            "#b28600",
-            "#009d9a",
-            "#9f1853",
-            "#002d9c",
-            "#ee538b",
-            "#570408",
-            "#005d5d",
-            "#8a3800",
-            "#a56eff",
-        ]
-    class_weights (dict of floats, optional): Dict with weights of the classes. Defaults to 1.
-    sample_header (str, optional): Header for samples line item. Defaults to "Samples".
-    event_header (str, optional): Header for events line item. Defaults to "Events".
-    sample_perc_precision (int, optional): Precision of % of samples line item. Defaults to 1.
-    event_perc_precision (int, optional): Precision of % of events line item. Defaults to 1.
-    percentage_first: Whether to show % first. Defaults to True.
-    binary_formatting: Improves formatting of dict for binary classification.
-        Blends outputted colors and shows only class 1 in line items.
+        tree (decision tree classifier): The decision tree to be exported
+        feature_names (list of strings, optional): Names of each of the features. Defaults to None.
+        feature_value_formats (list of strings, optional): Formats for each feature value (used in Connectors). Defaults to "0.2f".
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
+        class_weights (dict of floats, optional): Dict with weights of the classes. Defaults to 1.
+        sample_header (str, optional): Header for samples line item. Defaults to "Samples".
+        event_header (str, optional): Header for events line item. Defaults to "Events".
+        sample_perc_precision (int, optional): Precision of % of samples line item. Defaults to 1.
+        event_perc_precision (int, optional): Precision of % of events line item. Defaults to 1.
+        percentage_first: Whether to show % first. Defaults to True.
+        binary_formatting: Improves formatting of dict for binary classification.
+            Blends outputted colors and shows only class 1 in line items.
 
     Returns (list):
         list of dictionaries of the format
             {
                 "node_id": id (int),
                 "impurity": gini impurity (float),
                 "n_node_samples": num of samples (int),
@@ -386,17 +386,14 @@
 def get_summary_streamlit(node_data, classes, spacing=[3, 2]):
     """Display summary for tree visual using streamlit components (Nodes + Classes)
 
     Args:
         node_data (dict): Node data of selected node
         classes (int): id of node
         spacing (list of 2 ints): Input to streamlit column spacing. Defaults to [3,2]
-
-    Returns:
-        None
     """
     col1, col2 = st.columns(spacing)
 
     with col1:
         st.header("Node data")
         st.write(
             f"""**Node ID:**  
@@ -584,26 +581,84 @@
 
 def binary_tree_complete(
     key,
     clf,
     show_node_ids=True,
     expanded_depth=3,
     style=None,
+    spacing=[3, 2],
     feature_names=None,
     feature_value_formats=None,
     class_names=None,
     class_colors=None,
     class_weights=None,
     sample_header="Samples",
     event_header="Events",
     sample_perc_precision=1,
     event_perc_precision=1,
     percentage_first=True,
     binary_formatting=False,
 ):
+    """_summary_
+
+    Args:
+        key (str): Name of tree
+        clf (decision tree classifier): The decision tree to be shown
+        expanded_depth (int, optional): Initial expanded depth of the tree. Defaults to 3.
+        show_node_ids (bool, optional): Whether node ids are shown at the left of every single node. Defaults to True.
+        style (_type_, optional): Styling info: font style, color, spacing. Defaults to default_style.
+            default_style = {
+                "max_height": "2400px",
+                "padding_quantum": "5px",
+                "edge_size": "100px",
+                "edge_color": "#c2c9cc",
+                "edge_hover_color": "#adc2cc",
+                "node_size": "120px",
+                "node_border_color": "#c2c9cc",
+                "node_color": "#fff",
+                "node_hover_color": "#d5e6f0",
+                "font_family": '"Helvetica Neue",Helvetica,Arial,sans-serif',
+                "font_size": "0.7em",
+                "text_color": "#111",
+                "text_hover_color": "#000",
+                "text_outline_color": "#fff",
+                "text_outline_alpha": "0.4",
+                "button_color": "#70b4c2",
+                "button_hover_color": "#2d6186",
+                "transition_time": "0.7s",
+            }
+        spacing (list of 2 ints): Input to streamlit column spacing for summary. Defaults to [3,2]
+        feature_names (list of strings, optional): Names of each of the features. Defaults to None.
+        feature_value_formats (list of strings, optional): Formats for each feature value (used in Connectors). Defaults to "0.2f".
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
+        class_weights (dict of floats, optional): Dict with weights of the classes. Defaults to 1.
+        sample_header (str, optional): Header for samples line item. Defaults to "Samples".
+        event_header (str, optional): Header for events line item. Defaults to "Events".
+        sample_perc_precision (int, optional): Precision of % of samples line item. Defaults to 1.
+        event_perc_precision (int, optional): Precision of % of events line item. Defaults to 1.
+        percentage_first: Whether to show % first. Defaults to True.
+        binary_formatting: Improves formatting of dict for binary classification.
+            Blends outputted colors and shows only class 1 in line items.
+    """
     data, classes = export_dict(
         clf,
         feature_names=feature_names,
         feature_value_formats=feature_value_formats,
         class_names=class_names,
         class_colors=class_colors,
         class_weights=class_weights,
@@ -620,15 +675,15 @@
         data,
         key=key,
         show_node_ids=show_node_ids,
         expanded_depth=expanded_depth,
         style=style,
     )
     node_data = get_node_data(data, node_id)
-    get_summary_streamlit(node_data, classes)
+    get_summary_streamlit(node_data, classes, spacing=spacing)
     st.markdown("---")
 
 
 # Debug code to help develop
 if _DEBUG:
     from sklearn.datasets import load_iris, load_breast_cancer
     from sklearn import tree
```

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.2.4/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

