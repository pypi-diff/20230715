# Comparing `tmp/streamlit-binary-tree-0.2.2.tar.gz` & `tmp/streamlit-binary-tree-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.2.2.tar", last modified: Sat Jul 15 08:55:05 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.2.3.tar", last modified: Sat Jul 15 10:38:17 2023, max compression
```

## Comparing `streamlit-binary-tree-0.2.2.tar` & `streamlit-binary-tree-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.864080 streamlit-binary-tree-0.2.2/
--rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-15 08:55:05.864080 streamlit-binary-tree-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.2/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 08:55:05.871082 streamlit-binary-tree-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-07-15 08:55:01.000000 streamlit-binary-tree-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.827540 streamlit-binary-tree-0.2.2/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    17411 2023-07-15 08:54:37.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.806593 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.847508 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.808593 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.849508 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     8091 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
--rw-rw-rw-   0        0        0    15517 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.863081 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   667302 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405682 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
--rw-rw-rw-   0        0        0     5066 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js
--rw-rw-rw-   0        0        0    16890 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.846509 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.742762 streamlit-binary-tree-0.2.3/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-15 10:38:17.742762 streamlit-binary-tree-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-15 10:38:17.749764 streamlit-binary-tree-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-15 10:38:12.000000 streamlit-binary-tree-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.702470 streamlit-binary-tree-0.2.3/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    21699 2023-07-15 10:37:39.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.695640 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.719475 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.696639 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.721475 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     8091 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
+-rw-rw-rw-   0        0        0    15517 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.741762 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   667302 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405682 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
+-rw-rw-rw-   0        0        0     5066 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js
+-rw-rw-rw-   0        0        0    16890 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-15 10:38:17.717475 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-15 10:38:17.000000 streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.2.2/LICENSE` & `streamlit-binary-tree-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/setup.py` & `streamlit-binary-tree-0.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-binary-tree",
-    version="0.2.2",
+    version="0.2.3",
     author="Abhishek Sharma",
     author_email="abhishek1995sharma@gmail.com",
     description="Interactive Binary Tree as a Streamlit component",
     long_description="Interactive Binary Tree as a Streamlit component",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,26 +7,37 @@
 from sklearn.tree import _tree
 from sklearn.tree._classes import DecisionTreeClassifier as DCTClass
 
 _RELEASE = True
 _DEBUG = True
 _NAME = "streamlit_binary_tree"
 
+# If release, use build or use dev
 if _RELEASE:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component(_NAME, path=build_dir)
 else:
     _component_func = components.declare_component(
         _NAME,
         url="http://localhost:3001",
     )
 
 
 def human_format(n, precision=0, large_value_precision=None):
+    """Human formats large numbers
+
+    Args:
+        n (int): Number to format
+        precision (int, optional): Precision of output. Defaults to 0.
+        large_value_precision (int, optional): Precision of larger number output. Defaults to precision if None.
+
+    Returns:
+        str: Readable small number
+    """
     if large_value_precision is None:
         large_value_precision = precision
 
     suffix = ["", "k", "M", "B", "T"]
     n = float(n)
     suffix_idx = max(
         0,
@@ -37,14 +48,25 @@
     precision = precision if suffix_idx == 0 else large_value_precision
     format = f",.{precision}f"
 
     return f"{n:{format}}{suffix[suffix_idx]}"
 
 
 def content_text(number, percentage, perc_precision=1, percentage_first=True):
+    """Return readable number with percentage out of total.
+
+    Args:
+        number (int or list): Number of samples
+        percentage (float or list): % samples out of total samples
+        perc_precision (int, optional): Precision of percentage. Defaults to 1.
+        percentage_first (bool, optional): Whether to put percentage first. Defaults to True.
+
+    Returns:
+        str: Formatted output
+    """
     if type(number) == list or type(number) == np.ndarray:
         num_texts = []
         perc_texts = []
         for n, p in zip(number, percentage):
             num_text = human_format(n, large_value_precision=1)
             perc_text = f"{p:{f'.{perc_precision}%'}}"
 
@@ -60,15 +82,24 @@
 
     text = (
         f"{perc_text} ({num_text})" if percentage_first else f"{num_text} ({perc_text})"
     )
     return text
 
 
-def combine_hex_values(colors, weight):
+def get_color_from_ternary_gradient(colors, weight):
+    """Provides color from gradient defined by three provided colors according to weight given.
+
+    Args:
+        colors (list of size 3): Colors defining ternary gradient
+        weight (int): Weight to calculate color
+
+    Returns:
+        str: Color from gradient as hex
+    """
     colors = [c[1:] for c in colors]
     colors = ["".join([char * 2 for char in c]) if len(c) == 3 else c for c in colors]
     if weight <= 0:
         weights = [-weight, 1 + weight, 0]
     else:
         weights = [0, 1 - weight, weight]
     total_weight = sum(weights)
@@ -84,14 +115,22 @@
     zpad = lambda x: x if len(x) == 2 else "0" + x
     color = zpad(hex(red)[2:]) + zpad(hex(green)[2:]) + zpad(hex(blue)[2:])
     color = "#" + color
     return color
 
 
 def get_balanced_class_weight(y):
+    """Return balanced class weight according to provided y
+
+    Args:
+        y (list or np.array): Target Values
+
+    Returns:
+        dict: Class weights in dict
+    """
     unique, counts = np.unique(np.array(y), return_counts=True)
     counts = 1 / counts
     class_weights = {u: c for u, c in zip(unique, counts)}
     return class_weights
 
 
 def export_dict(
@@ -105,48 +144,79 @@
     event_header="Events",
     sample_perc_precision=1,
     event_perc_precision=1,
     percentage_first=True,
     binary_formatting=False,
 ):
     """Export a decision tree in dict format.
-    Parameters
-    ----------
-    decision_tree : decision tree classifier
-        The decision tree to be exported
-    feature_names : list of strings, optional (default=None)
-        Names of each of the features.
-    max_depth : int, optional (default=None)
-        The maximum depth of the representation. If None, the tree is fully
-        generated.
-    Returns
-    -------
-    a dictionary of the format <tree> := {
-        'feature' <int> | <string>,
-        'threshold' : <float>,
-        'impurity' : <float>,
-        'n_node_samples' : <int>,
-        'left' : <tree>,
-        'right' : <tree>,
-        'value' : [<int>],
-    }
-    if feature_names is provided, it is used to map feature indices
-    to feature names.  All types (including the value list) are native
-    python types as opposed to numpy types to make exporting to json
-    and other pythonic operations easier.
-    Examples
-    --------
-    >>> from sklearn.datasets import load_iris
-    >>> from sklearn import tree
-    >>> import json
-    >>> clf = tree.DecisionTreeClassifier()
-    >>> iris = load_iris()
-    >>> clf = clf.fit(iris.data, iris.target)
-    >>> d = tree.export_dict(clf)
-    >>> j = json.dumps(d, indent=4)
+
+    Args:
+    decision_tree (decision tree classifier): The decision tree to be exported
+    feature_names (list of strings, optional): Names of each of the features. Defaults to None.
+    feature_value_formats (list of strings, optional): Formats for each feature value (used in Connectors). Defaults to "0.2f".
+    class_names (list of strings, optional): Names of each of the classes. Defaults to None.
+    class_colors (list of strings, optional): Hex of each of the class colors. Defaults to default class colors.
+        class_colors = [
+            "#198038",
+            "#fa4d56",
+            "#1192e8",
+            "#6929c4",
+            "#b28600",
+            "#009d9a",
+            "#9f1853",
+            "#002d9c",
+            "#ee538b",
+            "#570408",
+            "#005d5d",
+            "#8a3800",
+            "#a56eff",
+        ]
+    class_weights (dict of floats, optional): Dict with weights of the classes. Defaults to 1.
+    sample_header (str, optional): Header for samples line item. Defaults to "Samples".
+    event_header (str, optional): Header for events line item. Defaults to "Events".
+    sample_perc_precision (int, optional): Precision of % of samples line item. Defaults to 1.
+    event_perc_precision (int, optional): Precision of % of events line item. Defaults to 1.
+    percentage_first: Whether to show % first. Defaults to True.
+    binary_formatting: Improves formatting of dict for binary classification.
+        Blends outputted colors and shows only class 1 in line items.
+
+    Returns (list):
+        list of dictionaries of the format
+            {
+                "node_id": id (int),
+                "impurity": gini impurity (float),
+                "n_node_samples": num of samples (int),
+                "value": weighted event values (list of int),
+                "contents": [
+                    Samples text (str),
+                    Events text (str),
+                ],
+                "path": path (str),
+                "color": color hex (str),
+                "feature": feature name (str)
+                "threshold": threshold of split (float)
+                "left":{
+                    "id": id (int)
+                    "condition": condition of split (str)
+                }
+                "right":{
+                    "id": id (int)
+                    "condition": condition of split (str)
+                }
+            }
+
+    Examples:
+        from sklearn.datasets import load_iris
+        from sklearn import tree
+        import json
+        clf = tree.DecisionTreeClassifier()
+        iris = load_iris()
+        clf = clf.fit(iris.data, iris.target)
+        d = tree.export_dict(clf)
+        j = json.dumps(d, indent=4)
     """
     tree_ = tree.tree_
     master_list = []
     if feature_value_formats is None:
         feature_value_formats = ["0.2f"] * tree.max_features_
     if class_colors is None:
         class_colors = [
@@ -203,15 +273,15 @@
         if binary_formatting:
             bad_value = value_weighted[1]
             if bad_value >= root_bad_value:
                 ratio = (bad_value - root_bad_value) / (max_bad_value - root_bad_value)
             else:
                 ratio = (bad_value - root_bad_value) / (root_bad_value - min_bad_value)
 
-            color = combine_hex_values(
+            color = get_color_from_ternary_gradient(
                 [class_colors[0], class_equal_color, class_colors[1]],
                 ratio,
             )
         else:
             if np.argmax(value) == np.argmin(value):
                 color = class_equal_color
             else:
@@ -242,15 +312,15 @@
                 perc_precision=event_perc_precision,
                 percentage_first=percentage_first,
             )
 
         event_header_val = event_header
 
         if binary_formatting and event_header_val == "Events":
-            event_header_val = dataset.target_names[1]
+            event_header_val = class_names[1]
 
         tree_dict = {
             "node_id": i,
             "impurity": float(tree_.impurity[i]),
             "n_node_samples": int(samples),
             "value": value,
             "contents": [
@@ -294,21 +364,40 @@
 
     recur(0, master_list, "Root")
 
     return master_list, classes
 
 
 def get_node_data(data, node_id):
+    """Get node data from list of nodes data
+
+    Args:
+        data (list of dict): List of Node dicts
+        node_id (int): id of node
+
+    Returns:
+        dict: node data
+    """
     node_ids = [item["node_id"] for item in data]
     idx = node_ids.index(node_id)
     node_data = data[idx]
     return node_data
 
 
 def get_summary_streamlit(node_data, classes, spacing=[3, 2]):
+    """Display summary for tree visual using streamlit components (Nodes + Classes)
+
+    Args:
+        node_data (dict): Node data of selected node
+        classes (int): id of node
+        spacing (list of 2 ints): Input to streamlit column spacing. Defaults to [3,2]
+
+    Returns:
+        None
+    """
     col1, col2 = st.columns(spacing)
 
     with col1:
         st.header("Node data")
         st.write(
             f"""**Node ID:**  
                  {node_data['node_id']}"""
@@ -355,37 +444,37 @@
                     "id": int,
                     "condition": str
                 },
                 "contents": List[str],
                 "color": str
             }]
         key (str, optional): Name of tree. Defaults to None.
-        expanded (bool, optional): Whether completely expanded at the start. Defaults to True.
+        expanded_depth (int, optional): Initial expanded depth of the tree. Defaults to 3.
         show_node_ids (bool, optional): Whether node ids are shown at the left of every single node. Defaults to True.
         style (_type_, optional): Styling info: font style, color, spacing. Defaults to default_style.
-        default_style = {
-            "max_height": "2400px",
-            "padding_quantum": "5px",
-            "edge_size": "100px",
-            "edge_color": "#c2c9cc",
-            "edge_hover_color": "#adc2cc",
-            "node_size": "120px",
-            "node_border_color": "#c2c9cc",
-            "node_color": "#fff",
-            "node_hover_color": "#d5e6f0",
-            "font_family": "arial",
-            "font_size": "0.7em",
-            "text_color": "#333",
-            "text_hover_color": "#111",
-            "text_outline_color": "#fff",
-            "text_outline_alpha": "0.4",
-            "button_color": "#70b4c2",
-            "button_hover_color": "#2d6186",
-            "transition_time": "0.7s",
-        }
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
 
     Returns:
         int: Selected node id
 
     Example Usage:
         Tree with dummy data and changed style.
 
@@ -459,18 +548,18 @@
         "edge_size": "100px",
         "edge_color": "#c2c9cc",
         "edge_hover_color": "#adc2cc",
         "node_size": "120px",
         "node_border_color": "#c2c9cc",
         "node_color": "#fff",
         "node_hover_color": "#d5e6f0",
-        "font_family": "arial",
+        "font_family": '"Helvetica Neue",Helvetica,Arial,sans-serif',
         "font_size": "0.7em",
-        "text_color": "#333",
-        "text_hover_color": "#111",
+        "text_color": "#111",
+        "text_hover_color": "#000",
         "text_outline_color": "#fff",
         "text_outline_alpha": "0.4",
         "button_color": "#70b4c2",
         "button_hover_color": "#2d6186",
         "transition_time": "0.7s",
     }
 
@@ -489,69 +578,98 @@
         show_node_ids=show_node_ids,
         style=style,
     )
 
     return component_value
 
 
-if _DEBUG:
-    from sklearn.datasets import load_iris, load_breast_cancer
-    from sklearn import tree
-
-    st.set_page_config(layout="wide")
-
-    # Breast Cancer dataset (Binary Classification)
-    clf = tree.DecisionTreeClassifier(
-        class_weight="balanced", max_depth=4, random_state=42
-    )
-    dataset = load_breast_cancer()
-    clf = clf.fit(
-        dataset.data,
-        dataset.target,
-    )
-    get_balanced_class_weight(dataset.target)
+def binary_tree_complete(
+    key,
+    clf,
+    show_node_ids=True,
+    expanded_depth=3,
+    style=None,
+    feature_names=None,
+    feature_value_formats=None,
+    class_names=None,
+    class_colors=None,
+    class_weights=None,
+    sample_header="Samples",
+    event_header="Events",
+    sample_perc_precision=1,
+    event_perc_precision=1,
+    percentage_first=True,
+    binary_formatting=False,
+):
     data, classes = export_dict(
         clf,
-        feature_names=list(dataset.feature_names),
-        class_names=list(dataset.target_names),
-        class_weights=get_balanced_class_weight(dataset.target),
-        binary_formatting=True,
+        feature_names=feature_names,
+        feature_value_formats=feature_value_formats,
+        class_names=class_names,
+        class_colors=class_colors,
+        class_weights=class_weights,
+        sample_header=sample_header,
+        event_header=event_header,
+        sample_perc_precision=sample_perc_precision,
+        event_perc_precision=event_perc_precision,
+        percentage_first=percentage_first,
+        binary_formatting=binary_formatting,
     )
 
     st.markdown("---")
     node_id = binary_tree(
         data,
-        key="dct_sample_breast_cancer_dataset",
-        show_node_ids=True,
-        style={"node_size": "120px"},
+        key=key,
+        show_node_ids=show_node_ids,
+        expanded_depth=expanded_depth,
+        style=style,
     )
     node_data = get_node_data(data, node_id)
     get_summary_streamlit(node_data, classes)
     st.markdown("---")
 
-    # Iris dataset (Multi-class Classification)
-    clf = tree.DecisionTreeClassifier(
+
+# Debug code to help develop
+if _DEBUG:
+    from sklearn.datasets import load_iris, load_breast_cancer
+    from sklearn import tree
+
+    st.set_page_config(layout="wide")
+
+    # Breast Cancer dataset (Binary Classification)
+    clf_breast_cancer = tree.DecisionTreeClassifier(
         class_weight="balanced", max_depth=4, random_state=42
     )
-    dataset = load_iris()
-    clf = clf.fit(
-        dataset.data,
-        dataset.target,
-    )
-    get_balanced_class_weight(dataset.target)
-    data, classes = export_dict(
-        clf,
-        feature_names=list(dataset.feature_names),
-        class_names=list(dataset.target_names),
-        class_weights=get_balanced_class_weight(dataset.target),
+    dataset_breast_cancer = load_breast_cancer()
+    clf_breast_cancer = clf_breast_cancer.fit(
+        dataset_breast_cancer.data,
+        dataset_breast_cancer.target,
+    )
+    binary_tree_complete(
+        "test",
+        clf_breast_cancer,
+        show_node_ids=True,
+        style={"node_size": "120px"},
+        feature_names=list(dataset_breast_cancer.feature_names),
+        class_names=list(dataset_breast_cancer.target_names),
+        class_weights=get_balanced_class_weight(dataset_breast_cancer.target),
+        binary_formatting=True,
     )
 
-    st.markdown("---")
-    node_id = binary_tree(
-        data,
-        key="dct_sample_iris_dataset",
+    # Iris dataset (Multi-class Classification)
+    clf_iris = tree.DecisionTreeClassifier(
+        class_weight="balanced", max_depth=4, random_state=42
+    )
+    dataset_iris = load_iris()
+    clf_iris = clf_iris.fit(
+        dataset_iris.data,
+        dataset_iris.target,
+    )
+    binary_tree_complete(
+        "test2",
+        clf_iris,
         show_node_ids=True,
         style={"node_size": "120px"},
+        feature_names=list(dataset_iris.feature_names),
+        class_names=list(dataset_iris.target_names),
+        class_weights=get_balanced_class_weight(dataset_iris.target),
     )
-    node_data = get_node_data(data, node_id)
-    get_summary_streamlit(node_data, classes)
-    st.markdown("---")
```

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.2.3/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

