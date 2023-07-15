# Comparing `tmp/AutoCarver-5.0.4.tar.gz` & `tmp/AutoCarver-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.4.tar", last modified: Fri Jul 14 23:45:29 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.5.tar", last modified: Sat Jul 15 10:32:27 2023, max compression
```

## Comparing `AutoCarver-5.0.4.tar` & `AutoCarver-5.0.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30748 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31419 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28756 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 23:45:29.000000 AutoCarver-5.0.4/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-14 23:45:29.000000 AutoCarver-5.0.4/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:45:29.000000 AutoCarver-5.0.4/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 23:45:29.000000 AutoCarver-5.0.4/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.484274 AutoCarver-5.0.5/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31467 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.484274 AutoCarver-5.0.5/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32230 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28779 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.484274 AutoCarver-5.0.5/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-15 10:32:27.000000 AutoCarver-5.0.5/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-15 10:32:27.000000 AutoCarver-5.0.5/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:32:27.000000 AutoCarver-5.0.5/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 10:32:27.000000 AutoCarver-5.0.5/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.4/AutoCarver/auto_carver.py` & `AutoCarver-5.0.5/AutoCarver/auto_carver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Tool to build optimized buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
+from json import loads
 from typing import Any
 
-import numpy as np
+from numpy import array, sqrt, searchsorted, add, unique, zeros
 from IPython.display import display_html  # TODO: remove this
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.pyplot import subplots
 from matplotlib.ticker import PercentFormatter
-from pandas import DataFrame, Series, crosstab, unique
+from pandas import DataFrame, Series, crosstab
 from scipy.stats import chi2_contingency
 from seaborn import color_palette, despine
 from tqdm import tqdm
-from json import loads
 
 from .discretizers.discretizers import Discretizer
 from .discretizers.utils.base_discretizers import (
     GroupedListDiscretizer,
     convert_to_labels,
     convert_to_values,
 )
-from .discretizers.utils.grouped_list import is_equal, GroupedList
+from .discretizers.utils.grouped_list import GroupedList, is_equal
 from .discretizers.utils.serialization import json_deserialize_values_orders
 
 
 # TODO: display tables
 class AutoCarver(GroupedListDiscretizer):
     """Automatic carving of continuous, categorical and categorical ordinal
     features that maximizes association with a binary target.
@@ -127,15 +127,15 @@
         ordinal_features: list[str] = None,
         values_orders: dict[str, GroupedList] = None,
         max_n_mod: int = 5,
         min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
         sort_by: str = "tschuprowt",
         str_nan: str = "__NAN__",
         str_default: str = "__OTHER__",
-        output_dtype: str = 'float',
+        output_dtype: str = "float",
         dropna: bool = True,
         copy: bool = False,
         verbose: bool = True,
     ) -> None:
         """_summary_
 
         Parameters
@@ -169,26 +169,30 @@
         """
         # Lists of features
         self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
         if ordinal_features is None:
             ordinal_features = []
         self.ordinal_features = list(set(ordinal_features))
 
+        # checking that qualitatitve and quantitative featues are distinct
+        assert all(quali_feature not in quantitative_features for quali_feature in qualitative_features + ordinal_features), f"A feature of `quantitative_features` also is in `qualitative_features` or `ordinal_features`. Be carreful with your inputs!"
+        assert all(quanti_feature not in qualitative_features + ordinal_features for quanti_feature in quantitative_features), f"A feature of `qualitative_features` or `ordinal_features` also is in `quantitative_features`. Be carreful with your inputs!"
+
         # initializing input_dtypes
         self.input_dtypes = {feature: "str" for feature in qualitative_features + ordinal_features}
         self.input_dtypes.update({feature: "float" for feature in quantitative_features})
 
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=self.input_dtypes,
             output_dtype=output_dtype,
             str_nan=str_nan,
-            str_default = str_default,
+            str_default=str_default,
             dropna=dropna,
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq  # minimum frequency per base bucket
@@ -229,21 +233,21 @@
         # Checking for binary target and copying X
         x_copy = super().prepare_data(X, y)
         x_test_copy = super().prepare_data(X_test, y_test)
 
         return x_copy, x_test_copy
 
     def remove_feature(self, feature: str) -> None:
-        """Removes a feature from all instances 
+        """Removes a feature from all instances
 
         Parameters
         ----------
         feature : str
             Column name
-        """        
+        """
         if feature in self.features:
             super().remove_feature(feature)
             if feature in self.ordinal_features:
                 self.ordinal_features.remove(feature)
 
     def fit(
         self,
@@ -303,17 +307,18 @@
         )
 
         # computing crosstabs for each feature on train/test
         xtabs = get_xtabs(self.features, x_copy, y, labels_orders)
         xtabs_test = get_xtabs(self.features, x_test_copy, y_test, labels_orders)
 
         # optimal butcketization/carving of each feature
-        for n, feature in enumerate(self.features):
+        all_features = self.features[:]  # necessary as features are being removed from self.features
+        for n, feature in enumerate(all_features):
             if self.verbose:  # verbose if requested
-                print(f"\n------\n[AutoCarver] Fit {feature} ({n+1}/{len(self.features)})\n---")
+                print(f"\n------\n[AutoCarver] Fit {feature} ({n+1}/{len(all_features)})\n---")
 
             # getting xtabs on train/test
             xtab = xtabs[feature]
             xtab_test = xtabs_test[feature]
             if self.verbose:  # verbose if requested
                 print(xtab)
 
@@ -327,18 +332,20 @@
             if best_combination is not None:
                 order, xtab, xtab_test = best_combination
                 if self.verbose:  # verbose if requested
                     print(xtab)  # TODO get the good labels
 
                 # updating label_orders
                 labels_orders.update({feature: order})
-            
+
             # no suitable combination has been found -> removing feature
             else:
-                print(f"No robust combination for feature '{feature}' could be found. It will be ignored. You might have to increase the size of your test sample (test sample not representative of test sample for this feature) or you should consider dropping this features.")
+                print(
+                    f"No robust combination for feature '{feature}' could be found. It will be ignored. You might have to increase the size of your test sample (test sample not representative of test sample for this feature) or you should consider dropping this features."
+                )
                 self.remove_feature(feature)
                 if feature in labels_orders:
                     labels_orders.pop(feature)
 
             if self.verbose:  # verbose if requested
                 print("------\n")
 
@@ -403,20 +410,20 @@
             if self.dropna and self.str_nan in order and best_association is not None:
                 # raw ordering without nans
                 raw_order = GroupedList(order)
                 raw_order.remove(self.str_nan)
 
                 # all possible consecutive combinations
                 combinations = consecutive_combinations(
-                    raw_order, self.max_n_mod, min_group_size=self.min_group_size
+                    raw_order, self.max_n_mod - 1, min_group_size=self.min_group_size
                 )
 
                 # adding combinations with NaNs
                 nan_combinations = add_nan_in_combinations(
-                    combinations, self.str_nan, self.max_n_mod
+                    combinations, self.str_nan, self.max_n_mod - 1
                 )
 
                 # getting most associated combination
                 best_association = get_best_association(
                     xtab,
                     nan_combinations,
                     sort_by=self.sort_by,
@@ -574,36 +581,36 @@
     # number of values taken by the features
     n_mod_x = xtab.shape[0]
 
     # Chi2 statistic
     chi2 = chi2_contingency(xtab)[0]
 
     # Cramer's V
-    cramerv = np.sqrt(chi2 / n_obs / (n_mod_y - 1))
+    cramerv = sqrt(chi2 / n_obs / (n_mod_y - 1))
 
     # Tschuprow's T
-    tschuprowt = np.sqrt(chi2 / n_obs / np.sqrt((n_mod_x - 1) * (n_mod_y - 1)))
+    tschuprowt = sqrt(chi2 / n_obs / sqrt((n_mod_x - 1) * (n_mod_y - 1)))
 
     return {"cramerv": cramerv, "tschuprowt": tschuprowt}
 
 
 def vectorized_groupby_sum(xtab: DataFrame, groupby: list[str]):
     """Groups a crosstab by groupby and sums column values by groups"""
 
     # all indices that may be duplicated
-    index_values = np.array(groupby)
+    index_values = array(groupby)
 
     # all unique indices deduplicated
-    unique_indices = np.unique(index_values)
+    unique_indices = unique(index_values)
 
     # initiating summed up array with zeros
-    summed_values = np.zeros((len(unique_indices), len(xtab.columns)))
+    summed_values = zeros((len(unique_indices), len(xtab.columns)))
 
     # for each unique_index found in index_values sums xtab.Values at corresponding position in summed_values
-    np.add.at(summed_values, np.searchsorted(unique_indices, index_values), xtab.values)
+    add.at(summed_values, searchsorted(unique_indices, index_values), xtab.values)
 
     # converting back to dataframe
     grouped_xtab = DataFrame(summed_values, index=unique_indices, columns=xtab.columns)
 
     return grouped_xtab
 
 
@@ -841,14 +848,15 @@
     ax.set_ylabel("Target rate")
     ax.set_xlim(0, 1)
     ax.set_ylim(0)
     despine()
 
     return fig, ax
 
+
 def load_carver(json_serialized_auto_carver: str) -> GroupedListDiscretizer:
     """_summary_
 
     Parameters
     ----------
     json_serialized_auto_carver : str
         _description_
@@ -858,15 +866,15 @@
     GroupedListDiscretizer
         _description_
     """
     # loading json of auto_carver
     json_deserialized_auto_carver = loads(json_serialized_auto_carver)
 
     # deserializing values_orders
-    values_orders = json_deserialize_values_orders(json_deserialized_auto_carver['values_orders'])
+    values_orders = json_deserialize_values_orders(json_deserialized_auto_carver["values_orders"])
 
     # updating auto_carver attributes
     json_deserialized_auto_carver.update({"values_orders": values_orders})
 
     # initiating GroupedListDiscretizer
     auto_carver = GroupedListDiscretizer(**json_deserialized_auto_carver)
     auto_carver.fit()
```

### Comparing `AutoCarver-5.0.4/AutoCarver/converters.py` & `AutoCarver-5.0.5/AutoCarver/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.4/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.0.5/AutoCarver/discretizers/discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """Tools to build simple buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
 from typing import Union
+
 from numpy import nan
 from pandas import DataFrame, Series, unique
 
-from .utils.base_discretizers import (
-    GroupedListDiscretizer,
-    check_new_values,
-    min_value_counts,
-)
+from .utils.base_discretizers import GroupedListDiscretizer, check_new_values, min_value_counts
+from .utils.grouped_list import GroupedList
 from .utils.qualitative_discretizers import DefaultDiscretizer, OrdinalDiscretizer
 from .utils.quantitative_discretizers import QuantileDiscretizer
 from .utils.type_discretizers import StringDiscretizer
 
-from .utils.grouped_list import GroupedList
 
 class Discretizer(GroupedListDiscretizer):
     """Automatic discretizing of continuous, categorical and categorical ordinal features.
 
     Modalities/values of features are grouped according to there respective orders:
      - [Qualitative features] order based on modality target rate.
      - [Qualitative ordinal features] user-specified order.
@@ -112,24 +109,24 @@
         self.input_dtypes.update({feature: "float" for feature in quantitative_features})
 
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=self.input_dtypes,
-            output_dtype='str',
+            output_dtype="str",
             str_nan=str_nan,
-            str_default = str_default,
+            str_default=str_default,
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
-    
+
     def remove_feature(self, feature: str) -> None:
         """Removes a feature from the Discretizer
 
         Parameters
         ----------
         feature : str
             Column name of the feature
@@ -145,15 +142,15 @@
         Parameters
         ----------
         X : DataFrame
             _description_
         y : Series
             _description_
         """
-        # Checking for binary target and copying X 
+        # Checking for binary target and copying X
         x_copy = self.prepare_data(X, y)
 
         # [Qualitative features] Grouping qualitative features
         if len(self.qualitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print("------\n[Discretizer] Fit Qualitative Features\n---")
 
@@ -290,17 +287,17 @@
         self.min_freq = min_freq
 
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=input_dtypes,
-            output_dtype='str',
+            output_dtype="str",
             str_nan=str_nan,
-            str_default = str_default,
+            str_default=str_default,
             copy=copy,
             verbose=verbose,
         )
 
         # non-ordinal qualitative features
         self.non_ordinal_features = [
             feature for feature in self.qualitative_features if feature not in self.ordinal_features
@@ -323,50 +320,60 @@
             Formatted X for bucketization
         """
         # checking for binary target, copying X
         x_copy = super().prepare_data(X, y)
 
         # checking for ids (unique value per row)
         frequencies = x_copy[self.features].apply(
-            lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors='ignore').max(), axis=0
+            lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors="ignore").max(),
+            axis=0,
         )
         # for each feature, checking that at least one value is more frequent than min_freq
-        for feature in self.features:
+        all_features = self.features[:]  # necessary as features are being removed from self.features
+        for feature in all_features:
             if frequencies[feature] < self.min_freq:
-                print(f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than {self.min_freq:2.2%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature.")
+                print(
+                    f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than min_freq={self.min_freq:2.1%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
+                )
                 self.remove_feature(feature)
 
         # checking for columns containing floats or integers even with filled nans
         dtypes = x_copy[self.features].fillna(self.str_nan).applymap(type).apply(unique)
         not_object = dtypes.apply(lambda u: any(typ != str for typ in u))
 
         # non qualitative features detected
         if any(not_object):
             features_to_convert = list(not_object.index[not_object])
             if self.verbose:
-                unexpected_dtypes = [typ for dtyp in dtypes[not_object] for typ in dtyp if typ != str]
+                unexpected_dtypes = [
+                    typ for dtyp in dtypes[not_object] for typ in dtyp if typ != str
+                ]
                 print(
                     f"""Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
                 )
 
             # converting specified features into qualitative features
-            string_discretizer = StringDiscretizer(features=features_to_convert, values_orders=self.values_orders, verbose=self.verbose)
+            string_discretizer = StringDiscretizer(
+                features=features_to_convert, values_orders=self.values_orders, verbose=self.verbose
+            )
             x_copy = string_discretizer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(string_discretizer.values_orders)
 
         # all known values for features
         known_values = {feature: values.values() for feature, values in self.values_orders.items()}
 
         # checking that all unique values in X are in values_orders
-        check_new_values(x_copy, self.ordinal_features, known_values, self.str_nan, self.str_default)
+        check_new_values(
+            x_copy, self.ordinal_features, known_values, self.str_nan, self.str_default
+        )
 
         return x_copy
-    
+
     def remove_feature(self, feature: str) -> None:
         """Removes a feature from the Discretizer
 
         Parameters
         ----------
         feature : str
             Column name of the feature
@@ -491,15 +498,15 @@
             _description_, by default False
         """
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=quantitative_features,
             values_orders=values_orders,
             input_dtypes=input_dtypes,
-            output_dtype='str',
+            output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
@@ -508,15 +515,17 @@
         """Checking data for bucketization"""
         # checking for binary target and copying X
         x_copy = super().prepare_data(X, y)
 
         # checking for quantitative columns
         dtypes = x_copy[self.features].applymap(type).apply(unique)
         not_numeric = dtypes.apply(lambda u: str in u)
-        assert all(~not_numeric), f"Non-numeric features: {str(list(not_numeric[not_numeric].index))}"
+        assert all(
+            ~not_numeric
+        ), f"Non-numeric features: {str(list(not_numeric[not_numeric].index))}"
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """Learning TRAIN distribution"""
 
         # checking data before bucketization
@@ -525,15 +534,15 @@
         # [Quantitative features] Grouping values into quantiles
         quantile_discretizer = QuantileDiscretizer(
             self.features,
             min_freq=self.min_freq,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
             copy=True,  # needs to be True so that it does not transform x_copy
-            verbose = self.verbose,
+            verbose=self.verbose,
         )
         x_copy = quantile_discretizer.fit_transform(x_copy, y)
 
         # storing orders of grouped features
         self.values_orders.update(quantile_discretizer.values_orders)
 
         # [Quantitative features] Grouping rare quantiles into closest common one
```

### Comparing `AutoCarver-5.0.4/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.0.5/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Base tools to build simple buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
+from json import dumps
 from typing import Any, Union
 
-from json import dumps
-from numpy import array, inf, isfinite, nan, select, floating, integer
+from numpy import array, floating, inf, integer, isfinite, nan, select
 from pandas import DataFrame, Series, isna, notna, unique
 from sklearn.base import BaseEstimator, TransformerMixin
 
-from .serialization import json_serialize_values_orders
 from .grouped_list import GroupedList
+from .serialization import json_serialize_values_orders
+
 
 def nan_unique(x: Series) -> list[Any]:
     """Unique non-NaN values.
 
     Parameters
     ----------
     x : Series
@@ -57,15 +58,21 @@
     if isinstance(applied, DataFrame):
         converted = applied.to_dict(orient="list")
 
     return converted
 
 
 # TODO: remove known_values
-def check_new_values(X: DataFrame, features: list[str], known_values: dict[str, list[Any]], str_nan: str, str_default: str) -> None:
+def check_new_values(
+    X: DataFrame,
+    features: list[str],
+    known_values: dict[str, list[Any]],
+    str_nan: str,
+    str_default: str,
+) -> None:
     """Checks for new, unexpected values, in X
 
     Parameters
     ----------
     X : DataFrame
         New DataFrame (at transform time)
     features : list[str]
@@ -80,16 +87,20 @@
         result_type="expand",
     )
     uniques = applied_to_dict_list(uniques)
 
     # checking for unexpected values for each feature
     for feature in features:
         unexpected = [val for val in uniques[feature] if val not in known_values[feature]]
-        assert str_nan not in unexpected, "It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_nan`. "
-        assert str_default not in unexpected, "It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_default`. "
+        assert (
+            str_nan not in unexpected
+        ), "It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_nan`. "
+        assert (
+            str_default not in unexpected
+        ), "It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_default`. "
         assert (
             len(unexpected) == 0
         ), f"Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was not provided. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
 
 
 def check_missing_values(
     X: DataFrame, features: list[str], known_values: dict[str, list[Any]]
@@ -117,26 +128,25 @@
     for feature in features:
         unexpected = [val for val in known_values[feature] if val not in uniques[feature]]
         assert (
             len(unexpected) == 0
         ), f"Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was provided but there are not matching value in provided X. You should check 'values_orders['{feature}']' for unwanted values."
 
 
-
 # TODO: output a json
 class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
     """Discretizer that uses a dict of grouped values."""
 
     def __init__(
         self,
         features: list[str],
         *,
         values_orders: dict[str, GroupedList] = None,
-        input_dtypes: Union[str, dict[str, str]] = 'str',
-        output_dtype: str = 'str',
+        input_dtypes: Union[str, dict[str, str]] = "str",
+        output_dtype: str = "str",
         str_nan: str = None,
         str_default: str = None,
         dropna: bool = True,
         copy: bool = True,
         verbose: bool = True,
     ) -> None:
         """Initiates a Discretizer by dict of GroupedList
@@ -159,15 +169,17 @@
             Default string value attributed to nan, by default None
         copy : bool, optional
             Whether or not to copy the input DataFrame, by default False
         """
         self.features = list(set(features))
         if values_orders is None:
             values_orders: dict[str, GroupedList] = {}
-        self.values_orders = {feature: GroupedList(values) for feature, values in values_orders.items()}
+        self.values_orders = {
+            feature: GroupedList(values) for feature, values in values_orders.items()
+        }
         self.copy = copy
 
         # input feature types
         if isinstance(input_dtypes, str):
             input_dtypes = {feature: input_dtypes for feature in features}
         self.input_dtypes = input_dtypes
 
@@ -193,15 +205,15 @@
 
         # identifying quantitative features by there type
         self.quantitative_features = [
             feature for feature in features if self.input_dtypes[feature] == "float"
         ]
 
         # for each feature, getting label associated to each value
-        self.labels_per_values: dict[str, dict[Any, Any]]= {}  # will be initiated during fit
+        self.labels_per_values: dict[str, dict[Any, Any]] = {}  # will be initiated during fit
 
     def get_labels_per_values(self, output_dtype: str) -> dict[str, dict[Any, Any]]:
         """Creates a dict that contains, for each feature, for each value, the associated label
 
         Parameters
         ----------
         output_dtype : str
@@ -222,32 +234,32 @@
 
             # case 0: quantitative feature -> labels per quantile (removes str_nan)
             if feature in self.quantitative_features:
                 labels = get_labels(values, self.str_nan)
             # case 1: qualitative feature -> by default, labels are values
             else:
                 labels = [value for value in values if value != self.str_nan]  # (removing str_nan)
-            
+
             # add NaNs if there are any
             if self.str_nan in values:
                 labels += [self.str_nan]
-                
+
             # requested float output (AutoCarver) -> converting to integers
-            if output_dtype == 'float':
+            if output_dtype == "float":
                 labels = [n for n, _ in enumerate(labels)]
 
             # building label per value
             label_per_value: dict[Any, Any] = {}
             for group_of_values, label in zip(values, labels):
                 for value in values.get(group_of_values):
                     label_per_value.update({value: label})
-            
+
             # storing in full dict
             labels_per_values.update({feature: label_per_value})
-        
+
         return labels_per_values
 
     def remove_feature(self, feature: str) -> None:
         """Removes a feature from the Discretizer
 
         Parameters
         ----------
@@ -260,15 +272,17 @@
                 self.qualitative_features.remove(feature)
             if feature in self.quantitative_features:
                 self.quantitative_features.remove(feature)
             if feature in self.values_orders:
                 self.values_orders.pop(feature)
             if feature in self.input_dtypes:
                 self.input_dtypes.pop(feature)
-    
+            if feature in self.labels_per_values:
+                self.labels_per_values.pop(feature)
+
     def prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
         """_summary_
 
         Parameters
         ----------
         X : DataFrame
             _description_
@@ -280,15 +294,17 @@
         DataFrame
             _description_
         """
         # copying X
         x_copy = X
         if self.copy and X is not None:
             missing_columns = [feature for feature in self.features if feature not in X]
-            assert len(missing_columns) == 0, f"Missing features from the provided DataFrame: {str(missing_columns)}"
+            assert (
+                len(missing_columns) == 0
+            ), f"Missing features from the provided DataFrame: {str(missing_columns)}"
             x_copy = X.copy()
 
         # checking for binary target
         if y is not None:
             y_values = unique(y)
             assert (0 in y_values) & (
                 1 in y_values
@@ -304,16 +320,20 @@
         ----------
         X : DataFrame
             Contains columns named after `features` attribute, by default None
         y : Series, optional
             Model target, by default None
         """
         # checking that all features to discretize are in values_orders
-        missing_features = [feature for feature in self.features if feature not in self.values_orders]
-        assert len(missing_features) == 0, f"Missing values_orders for following features {str(missing_features)}."
+        missing_features = [
+            feature for feature in self.features if feature not in self.values_orders
+        ]
+        assert (
+            len(missing_features) == 0
+        ), f"Missing values_orders for following features {str(missing_features)}."
 
         # for each feature, getting label associated to each value
         self.labels_per_values = self.get_labels_per_values(self.output_dtype)
 
         return self
 
     def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
@@ -338,23 +358,27 @@
         x_copy = X
         if self.copy:
             x_copy = X.copy()
 
         # transforming quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
-                print(f" - [GroupedListDiscretizer] Transform Quantitative {str(self.quantitative_features)}")
+                print(
+                    f" - [GroupedListDiscretizer] Transform Quantitative {str(self.quantitative_features)}"
+                )
             x_copy = self.transform_quantitative(x_copy, y)
 
         # transforming qualitative features
         if len(self.qualitative_features) > 0:
             if self.verbose:  # verbose if requested
-                print(f" - [GroupedListDiscretizer] Transform Qualitative {str(self.qualitative_features)}")
+                print(
+                    f" - [GroupedListDiscretizer] Transform Qualitative {str(self.qualitative_features)}"
+                )
             x_copy = self.transform_qualitative(x_copy, y)
-        
+
         # reinstating nans
         if not self.dropna:
             for feature in self.features:
                 label_per_value = self.labels_per_values[feature]
                 if self.str_nan in label_per_value:  # checking for nans in the feature
                     x_copy[feature] = x_copy[feature].replace(label_per_value[self.str_nan], nan)
 
@@ -386,27 +410,33 @@
             feature_values = self.values_orders[feature]
 
             # keeping track of nans
             nans = isna(X[feature])
 
             # converting nans to there corresponding quantile (if it was grouped to a quantile)
             if any(nans):
-                assert (
-                     feature_values.contains(self.str_nan)
+                assert feature_values.contains(
+                    self.str_nan
                 ), f"Unexpected value! Missing values found for feature '{feature}' at transform step but not during fit. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
                 nan_value = feature_values.get_group(self.str_nan)
                 # checking that nans have been grouped to a quantile otherwise they are left as numpy.nan (for comparison purposes)
                 if nan_value != self.str_nan:
                     X.loc[nans, feature] = nan_value
 
             # list of masks of values to replace with there respective group
-            values_to_group = [X[feature] <= value for value in feature_values if value != self.str_nan]
+            values_to_group = [
+                X[feature] <= value for value in feature_values if value != self.str_nan
+            ]
 
             # corressponding group for each value
-            group_labels = [[self.labels_per_values[feature][value]] * x_len for value in feature_values if value != self.str_nan]
+            group_labels = [
+                [self.labels_per_values[feature][value]] * x_len
+                for value in feature_values
+                if value != self.str_nan
+            ]
 
             # checking for values to group
             if len(values_to_group) > 0:
                 X[feature] = select(values_to_group, group_labels, default=X[feature])
 
             # converting nans to there value
             if any(nans):
@@ -432,22 +462,34 @@
             _description_
         """
         # filling up nans with specified value
         if self.str_nan:
             X[self.qualitative_features] = X[self.qualitative_features].fillna(self.str_nan)
 
         # checking that all unique values in X are in values_orders
-        check_new_values(X, self.qualitative_features, {feature: values.values() for feature, values in self.values_orders.items()}, self.str_nan, self.str_default)
+        check_new_values(
+            X,
+            self.qualitative_features,
+            {feature: values.values() for feature, values in self.values_orders.items()},
+            self.str_nan,
+            self.str_default,
+        )
 
         # replacing values for there corresponding label
-        X = X.replace({feature: label_per_value for feature, label_per_value in self.labels_per_values.items() if feature in self.qualitative_features})           
+        X = X.replace(
+            {
+                feature: label_per_value
+                for feature, label_per_value in self.labels_per_values.items()
+                if feature in self.qualitative_features
+            }
+        )
 
         return X
-    
-    def to_json(self) ->  str:
+
+    def to_json(self) -> str:
         """Converts the GroupedListDiscretizer's values_orders to .json
 
         Returns
         -------
         str
             JSON serialized GroupedListDiscretizer
         """
@@ -461,68 +503,84 @@
             "str_default": self.str_default,
             "dropna": self.dropna,
             "copy": self.copy,
         }
 
         # dumping as json
         return dumps(json_serialized_groupedlistdiscretizer)
-    
+
     def summary(self) -> DataFrame:
         """Summarizes the data bucketization
 
         TODO: add crosstabs per feature for a provided X?
 
         Returns
         -------
         DataFrame
             A summary of feature's values
         """
         # raw label per value with output_dtype 'str'
-        raw_labels_per_values = self.get_labels_per_values(output_dtype='str')
+        raw_labels_per_values = self.get_labels_per_values(output_dtype="str")
 
         # initiating summaries
         summaries: list[dict[str, Any]] = []
         for feature in self.features:
-            # adding each value/label 
+            # adding each value/label
             for value, label in self.labels_per_values[feature].items():
                 # initiating feature summary (default value/label)
-                feature_summary = {'feature': feature, 'dtype': self.input_dtypes[feature], 'label': label, 'content': value}
+                feature_summary = {
+                    "feature": feature,
+                    "dtype": self.input_dtypes[feature],
+                    "label": label,
+                    "content": value,
+                }
 
                 # case 0: qualitative feature -> not adding floats and integers str_default
                 if feature in self.qualitative_features:
-                    if not isinstance(value, floating) and not isinstance(value, float):  # checking for floats
-                        if not isinstance(value, integer) and not isinstance(value, int):  # checking for ints
+                    if not isinstance(value, floating) and not isinstance(
+                        value, float
+                    ):  # checking for floats
+                        if not isinstance(value, integer) and not isinstance(
+                            value, int
+                        ):  # checking for ints
                             if value != self.str_default:  # checking for str_default
                                 summaries += [feature_summary]
 
                 # case 1: quantitative feature -> take the raw label per value
                 elif feature in self.quantitative_features:
-                    feature_summary.update({'content': raw_labels_per_values[feature][value]})
+                    feature_summary.update({"content": raw_labels_per_values[feature][value]})
                     summaries += [feature_summary]
 
         # adding nans for quantitative features (when nan has been grouped)
         for feature in self.quantitative_features:
             # initiating feature summary (no value/label)
-            feature_summary = {'feature': feature, 'dtype': self.input_dtypes[feature]}
+            feature_summary = {"feature": feature, "dtype": self.input_dtypes[feature]}
             # if there are nans -> if already added it will be dropped afterwards (unique content)
             if self.str_nan in raw_labels_per_values[feature]:
                 nan_group = self.values_orders[feature].get_group(self.str_nan)
-                feature_summary.update({'label': self.labels_per_values[feature][nan_group], 'content': self.str_nan})
+                feature_summary.update(
+                    {"label": self.labels_per_values[feature][nan_group], "content": self.str_nan}
+                )
                 summaries += [feature_summary]
 
         # aggregating unique values per label
-        summaries = DataFrame(summaries).groupby(['feature', 'dtype', 'label'])['content'].apply(lambda u: list(unique(u))).reset_index()
+        summaries = (
+            DataFrame(summaries)
+            .groupby(["feature", "dtype", "label"])["content"]
+            .apply(lambda u: list(unique(u)))
+            .reset_index()
+        )
         # sorting content
         sorted_contents: list[list[Any]] = []
-        for content in summaries['content']:
+        for content in summaries["content"]:
             content.sort(key=repr)
             sorted_contents += [content]
-        summaries['content'] = sorted_contents
+        summaries["content"] = sorted_contents
         # sorting and seting index
-        summaries = summaries.sort_values(['dtype', 'feature']).set_index(['feature', 'dtype'])
+        summaries = summaries.sort_values(["dtype", "feature"]).set_index(["feature", "dtype"])
 
         return summaries
 
 
 def convert_to_labels(
     features: list[str],
     quantitative_features: list[str],
@@ -557,16 +615,14 @@
     if not dropna:
         for feature in features:
             if str_nan in values_orders[feature]:
                 order = labels_orders[feature]
                 order.append(str_nan)  # adding back nans at the end of the order
                 labels_orders.update({feature: order})
 
-
-
     return labels_orders
 
 
 def convert_to_values(
     features: list[str],
     quantitative_features: list[str],
     values_orders: dict[str, GroupedList],
```

### Comparing `AutoCarver-5.0.4/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.0.5/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from typing import Any, Union
 
 from numpy import ndarray, sort
 from pandas import isna
 
+
 class GroupedList(list):
     """An ordered list that's extended with a dict."""
 
     def __init__(self, iterable: Union[ndarray, dict, list, tuple] = ()) -> None:
         """An ordered list that historizes its elements' content.
 
         Parameters
@@ -323,15 +324,14 @@
 
             elif len(values) > 2:  # case 3: more than two values in this group
                 repr += [f"{values[-1]}"[:char_limit] + " to " + f"{values[0]}"[:char_limit]]
 
         return repr
 
 
-
 def is_equal(a: Any, b: Any) -> bool:
     """Checks if a and b are equal (NaN insensitive)
 
     Parameters
     ----------
     a : Any
         _description_
@@ -348,8 +348,7 @@
     equal = a == b
 
     # Case where a and b are NaNs
     if isna(a) and isna(b):
         equal = True
 
     return equal
-
```

### Comparing `AutoCarver-5.0.4/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.0.5/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 """Tools to build simple buckets out of Qualitative features
 for a binary classification model.
 """
 
 from typing import Any, Dict, List, Union
-from AutoCarver.discretizers.utils.base_discretizers import GroupedList
 
 from numpy import argmin, nan, select
 from pandas import DataFrame, Series, isna, notna, unique
 
-from .grouped_list import GroupedList
 from .base_discretizers import (
     GroupedListDiscretizer,
     check_missing_values,
     check_new_values,
     convert_to_labels,
     convert_to_values,
     nan_unique,
     target_rate,
     value_counts,
 )
+from .grouped_list import GroupedList
 from .type_discretizers import StringDiscretizer
 
+
 class DefaultDiscretizer(GroupedListDiscretizer):
     """Groups a qualitative features' values less frequent than min_freq into a str_default string
 
     Only use for qualitative non-ordinal features
     """
 
     def __init__(
         self,
-        features: List[str],
+        features: list[str],
         min_freq: float,
         *,
-        values_orders: Dict[str, GroupedList] = None,
+        values_orders: dict[str, GroupedList] = None,
         str_default: str = "__OTHER__",
         str_nan: str = "__NAN__",
         copy: bool = False,
         verbose: bool = False,
     ) -> None:
         """_summary_
 
         Parameters
         ----------
-        features : List[str]
+        features : list[str]
             List of column names to be discretized
         min_freq : float
             Minimum frequency per modality. Less frequent modalities are grouped in the closest value of the order.
-        values_orders : Dict[str, GroupedList], optional
+        values_orders : dict[str, GroupedList], optional
             Dict of column names (keys) and modalities' associated order (values), by default None
         str_default : str, optional
             _description_, by default "__OTHER__"
         str_nan : str, optional
             _description_, by default "__NAN__"
         copy : bool, optional
             _description_, by default False
         verbose : bool, optional
             _description_, by default False
         """
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=features,
             values_orders=values_orders,
-            input_dtypes='str',
-            output_dtype='str',
+            input_dtypes="str",
+            output_dtype="str",
             str_nan=str_nan,
-            str_default = str_default,
+            str_default=str_default,
             copy=copy,
             verbose=verbose,
         )
-        
+
         self.min_freq = min_freq
 
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """Called during fit step
 
         Parameters
         ----------
@@ -92,15 +92,17 @@
         # checks and initilizes values_orders
         for feature in self.features:
             # initiating features missing from values_orders
             if feature not in self.values_orders:
                 self.values_orders.update({feature: GroupedList(nan_unique(x_copy[feature]))})
 
         # checking that all unique values in X are in values_orders
-        check_new_values(x_copy, self.features, self.values_orders, self.str_nan, self.str_default)  # TODO problem here
+        check_new_values(
+            x_copy, self.features, self.values_orders, self.str_nan, self.str_default
+        )  # TODO problem here
         # checking that all unique values in values_orders are in X
         check_missing_values(x_copy, self.features, self.values_orders)
 
         # adding NANS
         for feature in self.features:
             if any(x_copy[feature].isna()):
                 self.values_orders[feature].append(self.str_nan)
@@ -118,15 +120,15 @@
         X : DataFrame
             _description_
         y : Series
             _description_
         """
         # copying dataframe and checking data before bucketization
         x_copy = self.prepare_data(X, y)
-        
+
         if self.verbose:  # verbose if requested
             print(f" - [DefaultDiscretizer] Fit {str(self.features)}")
 
         # computing frequencies of each modality
         frequencies = x_copy.apply(value_counts, normalize=True, axis=0)
 
         for feature in self.features:
@@ -168,15 +170,15 @@
             # sorting order updating values_orders
             self.values_orders.update({feature: order.sort_by(new_order)})
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
-    
+
 
 class OrdinalDiscretizer(GroupedListDiscretizer):
     """Discretizes ordered qualitative features into groups more frequent than min_freq.
     NaNs are left untouched.
 
     Modality is choosen amongst the preceding and following values in the provided order.
     The choosen modality is:
@@ -195,23 +197,23 @@
         copy: bool = False,
         verbose: bool = False,
     ):
         """Initializes a OrdinalDiscretizer
 
         Parameters
         ----------
-        features : List[str]
+        features : list[str]
             List of column names to be discretized
-        values_orders : Dict[str, Any]
+        values_orders : dict[str, Any]
             Dict of column names (keys) and modalities' associated order (values)
         min_freq : float
             Minimum frequency per modality. Less frequent modalities are grouped in the closest value of the order.
         str_nan : str, optional
             _description_, by default None
-        input_dtypes : Union[str, Dict[str, str]], optional
+        input_dtypes : Union[str, dict[str, str]], optional
             String of type to be considered for all features or
             Dict of column names and associated types:
             - if 'float' uses transform_quantitative
             - if 'str' uses transform_qualitative,
             default 'str'
         copy : bool, optional
             _description_, by default False
@@ -219,15 +221,15 @@
             _description_, by default False
         """
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=features,
             values_orders=values_orders,
             input_dtypes=input_dtypes,
-            output_dtype='str',
+            output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
@@ -275,17 +277,14 @@
         """
         if self.verbose:  # verbose if requested
             print(f" - [OrdinalDiscretizer] Fit {str(self.features)}")
 
         # checking values orders
         x_copy = self.prepare_data(X, y)
 
-        # getting label per value
-        labels_per_values = self.get_labels_per_values(output_dtype='str')
-
         # converting potential quantiles into there labels
         known_orders = convert_to_labels(
             features=self.features,
             quantitative_features=self.quantitative_features,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
             dropna=True,
@@ -333,19 +332,19 @@
         copy: bool = False,
         verbose: bool = False,
     ) -> None:
         """Initializes a ChainedDiscretizer
 
         Parameters
         ----------
-        features : List[str]
+        features : list[str]
             Columns to be bucketized
         min_freq : float
             Minimum frequency per modality
-        chained_orders : List[GroupedList]
+        chained_orders : list[GroupedList]
             List of modality orders
         remove_unknown : bool, optional
             Whether or not to remove unknown values. If true, they are grouped
             into the value of`str_nan` otherwise it throws an error,
             by default True
         str_nan : str, optional
             Value used to replace nan. If set, same value should be used across
@@ -355,53 +354,60 @@
         verbose : bool, optional
             Whether or not to print information during fit, by default False
         """
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=features,
             values_orders=values_orders,
-            input_dtypes='str',
-            output_dtype='str',
+            input_dtypes="str",
+            output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
 
         self.min_freq = min_freq
 
         self.chained_orders = [GroupedList(values) for values in chained_orders]
 
         # parameters to handle missing/unknown values
         self.remove_unknown = remove_unknown
 
         # known_values: all ordered values describe in each level of the chained_orders
-        # starting off with first level 
+        # starting off with first level
         known_values = self.chained_orders[0].values()
         # adding each level
         for next_level in self.chained_orders[1:]:
             # highest value per group of the level
-            highest_ranking_value = {group: [value for value in values if value!=group][-1] for group, values in next_level.content.items()}
-            
+            highest_ranking_value = {
+                group: [value for value in values if value != group][-1]
+                for group, values in next_level.content.items()
+            }
+
             # adding next_level group to the order
             for group, highest_value in highest_ranking_value.items():
                 highest_index = known_values.index(highest_value)
-                known_values = known_values[:highest_index + 1] + [group] + known_values[highest_index + 1:]
+                known_values = (
+                    known_values[: highest_index + 1] + [group] + known_values[highest_index + 1 :]
+                )
         self.known_values = known_values
 
         # adding known_values to each feature's order
         for feature in self.features:
             # checking for already known values of the feature
             if feature in self.values_orders:
                 order = self.values_orders[feature]
             # no known values for the feature
             else:
                 order = GroupedList([])
             # checking that all values from the order are in known_values
             for value in order:
-                assert value in self.known_values, f"Value {value} from feature {feature} provided in values_orders is missing from levels of chained_orders. Add value to a level of chained_orders or adapt values_orders."
+                assert (
+                    value in self.known_values
+                ), f"Value {value} from feature {feature} provided in values_orders is missing from levels of chained_orders. Add value to a level of chained_orders or adapt values_orders."
             # adding known values if missing from the order
             for value in self.known_values:
                 if value not in order.values():
                     order.append(value)
             order = order.sort_by(self.known_values)
             self.values_orders.update({feature: order})
 
@@ -424,37 +430,44 @@
             Formatted X for bucketization
         """
         # copying dataframe
         x_copy = X.copy()
 
         # checking for ids (unique value per row)
         frequencies = x_copy[self.features].apply(
-            lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors='ignore').max(), axis=0
+            lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors="ignore").max(),
+            axis=0,
         )
         # for each feature, checking that at least one value is more frequent than min_freq
         for feature in self.features:
             if frequencies[feature] < self.min_freq:
-                print(f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than {self.min_freq:2.2%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature.")
+                print(
+                    f"For feature '{feature}', the largest modality has {frequencies[feature]:2.2%} observations which is lower than {self.min_freq:2.2%}. This feature will not be Discretized. Consider decreasing parameter min_freq or removing this feature."
+                )
                 self.remove_feature(feature)
 
         # checking for columns containing floats or integers even with filled nans
         dtypes = x_copy[self.features].fillna(self.str_nan).applymap(type).apply(unique)
         not_object = dtypes.apply(lambda u: any(typ != str for typ in u))
 
         # non qualitative features detected
         if any(not_object):
             features_to_convert = list(not_object.index[not_object])
             if self.verbose:
-                unexpected_dtypes = [typ for dtyp in dtypes[not_object] for typ in dtyp if typ != str]
+                unexpected_dtypes = [
+                    typ for dtyp in dtypes[not_object] for typ in dtyp if typ != str
+                ]
                 print(
                     f"""Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
                 )
 
             # converting specified features into qualitative features
-            stringer = StringDiscretizer(features=features_to_convert, values_orders=self.values_orders)
+            stringer = StringDiscretizer(
+                features=features_to_convert, values_orders=self.values_orders
+            )
             x_copy = stringer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(stringer.values_orders)
 
         # all known values for features
         known_values = {feature: values.values() for feature, values in self.values_orders.items()}
@@ -462,15 +475,15 @@
         # checking that all unique values in X are in values_orders
         check_new_values(x_copy, self.features, known_values, self.str_nan, self.str_default)
 
         # filling nans
         x_copy = x_copy.fillna(self.str_nan)
 
         return x_copy
-    
+
     def fit(self, X: DataFrame, y: Series = None) -> None:
         """_summary_
 
         Parameters
         ----------
         X : DataFrame
             _description_
@@ -485,26 +498,29 @@
         # filling nans
         x_copy = self.prepare_data(X, y)
 
         # iterating over each feature
         if self.verbose:  # verbose if requested
             print(f" - [ChainedDiscretizer] Fit {str(self.features)}")
         for feature in self.features:
-
             # computing frequencies of each modality
             frequencies = x_copy[feature].value_counts(normalize=True)
             values, frequencies = frequencies.index, frequencies.values
 
             # adding NaNs to the order if any
             order = self.values_orders[feature]
             if self.str_nan in values:
                 order.append(self.str_nan)
 
             # checking for unknown values (missing from known_values)
-            missing = [value for value in values if value not in self.known_values and value != self.str_nan]
+            missing = [
+                value
+                for value in values
+                if value not in self.known_values and value != self.str_nan
+            ]
 
             # converting unknown values to NaN
             if self.remove_unknown & (len(missing) > 0):
                 # alerting user
                 print(
                     f"Order for feature '{feature}' was not provided for values:  {str(missing)}, these values will be converted to '{self.str_nan}' (policy remove_unknown=True)"
                 )
@@ -515,15 +531,17 @@
             # alerting user
             else:
                 assert (
                     not len(missing) > 0
                 ), f"Order for feature '{feature}' needs to be provided for values: {str(missing)}, otherwise set remove_unknown=True"
 
             # iterating over each specified orders
-            for level_order in self.chained_orders:  # TODO replace all of this with labels_per_orders
+            for (
+                level_order
+            ) in self.chained_orders:  # TODO replace all of this with labels_per_orders
                 # values that are frequent enough
                 to_keep = list(values[frequencies >= self.min_freq])
 
                 # values from the order to group (not frequent enough or absent)
                 values_to_group = [value for value in level_order.values() if value not in to_keep]
 
                 # values to group into discarded values
@@ -543,14 +561,15 @@
                 frequencies = x_copy[feature].value_counts(normalize=True)
                 values, frequencies = frequencies.index, frequencies.values
 
         super().fit(X, y)
 
         return self
 
+
 def find_common_modalities(
     df_feature: Series,
     y: Series,
     min_freq: float,
     values_orders: dict[str, GroupedList],
     len_df: int = None,
 ) -> dict[str, Any]:
@@ -572,15 +591,15 @@
     order : GroupedList
         _description_
     len_df : int, optional
         _description_, by default None
 
     Returns
     -------
-    Dict[str, Any]
+    dict[str, Any]
         _description_
     """
     # getting feature's order
     order = values_orders[df_feature.name]
 
     # initialisation de la taille totale du dataframe
     if len_df is None:
@@ -651,15 +670,15 @@
         series.groupby(list(map(order.get_group, series.index)), dropna=False).sum().reindex(order)
     )
 
     return grouped_series
 
 
 def find_closest_modality(
-    idx: int, order: GroupedList, frequencies: List[float], target_rates: Series, min_freq: float
+    idx: int, order: GroupedList, frequencies: list[float], target_rates: Series, min_freq: float
 ) -> Any:
     """HELPER Finds the closest modality in terms of frequency and target rate
 
     Parameters
     ----------
     idx : int
         _description_
```

### Comparing `AutoCarver-5.0.4/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.0.5/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         verbose : bool, optional
             _description_, by default False
         """
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=features,
             values_orders=values_orders,
-            input_dtypes='float',
-            output_dtype='str',
+            input_dtypes="float",
+            output_dtype="str",
             str_nan=str_nan,
             copy=copy,
             verbose=verbose,
         )
 
         self.min_freq = min_freq
         self.q = round(1 / min_freq)  # number of quantiles
```

### Comparing `AutoCarver-5.0.4/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.0.5/AutoCarver/discretizers/utils/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 """Sets of helper functions for GroupedListDiscretizer JSON serialization"""
 
 from json import dumps, loads
-from typing import Union, Any
-from numpy import floating, integer, isfinite, inf
+from typing import Any, Union
+
+from numpy import floating, inf, integer, isfinite
 
 from .grouped_list import GroupedList
 
+
 def convert_value_to_base_type(value: Any) -> Union[str, float, int]:
     """Converts a value to python's base types (str, int, float) for JSON serialization.
 
     Parameters
     ----------
     value : Any
         A value to serialize
 
     Returns
     -------
     Union[str, float, int]
         Serialized value
     """
-    
+
     output = value  # str/float/int value
     if not isinstance(value, str) and not isfinite(value):  # numpy.inf value
-        output = 'numpy.inf'
+        output = "numpy.inf"
     elif isinstance(value, integer):  # np.int value
         output = int(value)
     elif isinstance(value, floating):  # np.float value
         output = float(value)
-    
+
     return output
 
+
 def convert_value_to_numpy_type(value: Union[str, float, int]) -> Any:
     """Converts a list or a dict of lists values to numpy types for JSON deserialization.
 
     Parameters
     ----------
     value : Union[str, float, int]
         A value to deserialize
 
     Returns
     -------
     Any
         Deserialized value
     """
     output = value  # str/float/int value
-    if value == 'numpy.inf':  # numpy.inf value
+    if value == "numpy.inf":  # numpy.inf value
         output = inf
-    
+
     return output
 
-def convert_values_to_base_types(iterable: Union[list[Any], dict[str, list[Any]]]) -> Union[list[Union[str, int, float]], dict[str, list[Union[str, int, float]]]]:
+
+def convert_values_to_base_types(
+    iterable: Union[list[Any], dict[str, list[Any]]]
+) -> Union[list[Union[str, int, float]], dict[str, list[Union[str, int, float]]]]:
     """Converts a list or a dict of lists values to python's base types (str, int, float) for JSON serialization.
 
     Parameters
     ----------
     iterable : Union[list[Any], dict[str, list[Any]]]
         List or dict of lists of values to serialize
 
@@ -64,19 +70,25 @@
     """
     # list input
     output = None
     if isinstance(iterable, list):
         output = [convert_value_to_base_type(value) for value in iterable]
     # dict input
     elif isinstance(iterable, dict):
-        output = {convert_value_to_base_type(key): convert_values_to_base_types(values) for key, values in iterable.items()}
+        output = {
+            convert_value_to_base_type(key): convert_values_to_base_types(values)
+            for key, values in iterable.items()
+        }
 
     return output
 
-def convert_values_to_numpy_types(iterable: Union[list[Union[str, int, float]], dict[str, list[Union[str, int, float]]]]) -> Union[list[Any], dict[str, list[Any]]]:
+
+def convert_values_to_numpy_types(
+    iterable: Union[list[Union[str, int, float]], dict[str, list[Union[str, int, float]]]]
+) -> Union[list[Any], dict[str, list[Any]]]:
     """Converts a list or a dict of lists values to numpy types for JSON deserialization.
 
     Parameters
     ----------
     iterable : Union[list[Union[str, int, float]], dict[str, list[Union[str, int, float]]]]
         List or dict of lists of values to deserialize
 
@@ -87,18 +99,22 @@
     """
     # list input
     output = None
     if isinstance(iterable, list):
         output = [convert_value_to_numpy_type(value) for value in iterable]
     # dict input
     elif isinstance(iterable, dict):
-        output = {convert_value_to_numpy_type(key): convert_values_to_numpy_types(values) for key, values in iterable.items()}
+        output = {
+            convert_value_to_numpy_type(key): convert_values_to_numpy_types(values)
+            for key, values in iterable.items()
+        }
 
     return output
 
+
 def json_serialize_values_orders(values_orders: dict[str, GroupedList]) -> str:
     """JSON serializes a values_orders
 
     Parameters
     ----------
     values_orders : dict[str: GroupedList]
         values_orders to serialize
@@ -106,18 +122,25 @@
     Returns
     -------
     str
         JSON serialized values_orders
     """
 
     # converting values_orders to a json
-    json_serialized_values_orders = {feature: {'order': convert_values_to_base_types(order), 'content': convert_values_to_base_types(order.content)} for feature, order in values_orders.items()}
+    json_serialized_values_orders = {
+        feature: {
+            "order": convert_values_to_base_types(order),
+            "content": convert_values_to_base_types(order.content),
+        }
+        for feature, order in values_orders.items()
+    }
 
     return dumps(json_serialized_values_orders)
 
+
 def json_deserialize_values_orders(json_serialized_values_orders: str) -> dict[str, GroupedList]:
     """JSON serializes a values_orders
 
     Parameters
     ----------
     json_serialized_values_orders : str
         JSON serialized values_orders
@@ -128,23 +151,23 @@
         values_orders deserialized
     """
     # converting to dict
     json_deserialized_values_orders = loads(json_serialized_values_orders)
 
     # converting to numpy type
     json_deserialized_values_orders = convert_values_to_numpy_types(json_deserialized_values_orders)
-    
+
     # converting to GroupedList
     values_orders: dict[str, GroupedList] = {}
     for feature, content in json_deserialized_values_orders.items():
         # getting content from serialized dict
         feature_content: GroupedList = {}
-        for value in content['order']:
+        for value in content["order"]:
             content_key = value
             # float and int dict keys (converted in string by json.dumps)
             if not isinstance(value, str) and isfinite(value):
                 content_key = str(value)
-            feature_content.update({value: content['content'][content_key]})
+            feature_content.update({value: content["content"][content_key]})
         # saving up built GroupedList
         values_orders.update({feature: GroupedList(feature_content)})
 
     return values_orders
```

### Comparing `AutoCarver-5.0.4/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.0.5/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 """
 
 from pandas import DataFrame, Series
 
 from .base_discretizers import GroupedListDiscretizer, nan_unique
 from .grouped_list import GroupedList
 
+
 class StringDiscretizer(GroupedListDiscretizer):
     """Converts specified columns of a DataFrame into str.
     First step of a Qualitative Discretization pipe.
 
     - Keeps NaN inplace
     - Converts floats of int to int
     """
 
     def __init__(
         self,
         features: list[str],
         *,
         values_orders: dict[str, GroupedList] = None,
-        str_nan: str = '__NAN__',
+        str_nan: str = "__NAN__",
         copy: bool = False,
         verbose: bool = False,
     ) -> None:
         """_summary_
 
         Parameters
         ----------
@@ -73,16 +74,18 @@
                 # case 1: converting to string
                 else:
                     str_value = str(value)
 
                 # checking for string values already in the order
                 if str_value not in values_order:
                     values_order.append(str_value)  # adding string value to the order
-                    values_order.group(value, str_value)  # grouping integer value into the string value
-                
+                    values_order.group(
+                        value, str_value
+                    )  # grouping integer value into the string value
+
             # adding str_nan
             if any(x_copy[feature].isna()):
                 values_order.append(self.str_nan)
 
             # updating values_orders accordingly
             # case 0: non-ordinal features, updating as is (no order provided)
             if feature not in self.values_orders:
```

### Comparing `AutoCarver-5.0.4/AutoCarver/feature_selector.py` & `AutoCarver-5.0.5/AutoCarver/feature_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from sklearn.base import BaseEstimator, TransformerMixin
 from statsmodels.formula.api import ols
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 
 from .discretizers.utils.base_discretizers import GroupedListDiscretizer
 from .discretizers.utils.grouped_list import GroupedList
 
+
 # TODO: convert to groupedlistdiscretizer
 # TODO: add parameter to shut down displayed info
 class FeatureSelector(BaseEstimator, TransformerMixin):
     """A pipeline of measures to perform EDA and feature pre-selection
 
      - best features are the n_best of each measure
      - selected features are stored in FeatureSelector.best_features
@@ -128,15 +129,17 @@
             filters = []
         self.filters = [thresh_filter] + filters[:]
         self.sort_measures = [measure.__name__ for measure in measures[::-1]]
 
         # Values_orders from GroupedListDiscretizer
         if values_orders is None:
             values_orders = {}
-        self.values_orders = {feature: GroupedList(value) for feature, value in values_orders.items()}
+        self.values_orders = {
+            feature: GroupedList(value) for feature, value in values_orders.items()
+        }
 
         self.drop = drop
         self.copy = copy
         self.verbose = verbose
         self.params = params
 
         self.associations = None
```

### Comparing `AutoCarver-5.0.4/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.5/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.4
+Version: 5.0.5
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.0.4/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.0.5/AutoCarver.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 AutoCarver/discretizers/utils/serialization.py
 AutoCarver/discretizers/utils/type_discretizers.py
 tests/test_auto_carver.py
 tests/test_base_discretizers.py
 tests/test_converters.py
 tests/test_discretizers.py
 tests/test_feature_selector.py
+tests/test_grouped_list.py
 tests/test_qualitative_discretizers.py
 tests/test_quantitative_discretizers.py
 tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.4/LICENSE` & `AutoCarver-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.4/PKG-INFO` & `AutoCarver-5.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.4
+Version: 5.0.5
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.0.4/README.md` & `AutoCarver-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.4/setup.py` & `AutoCarver-5.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.4",
+    version="5.0.5",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.0.4/tests/test_auto_carver.py` & `AutoCarver-5.0.5/tests/test_auto_carver.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,95 @@
 """Set of tests for auto_carver module."""
 
-from AutoCarver.auto_carver import *
+from pandas import DataFrame
 from pytest import fixture
 
+from AutoCarver.auto_carver import AutoCarver, load_carver
+
+
 @fixture(scope="module", params=["float", "str"])
 def output_dtype(request) -> str:
     return request.param
 
+
 @fixture(scope="module", params=[True, False])
 def dropna(request) -> bool:
     return request.param
 
+
 @fixture(scope="module", params=["tschuprowt", "cramerv"])
 def sort_by(request) -> str:
     return request.param
 
-def test_auto_carver(x_train: DataFrame, x_test_1: DataFrame, output_dtype: str, dropna: bool, sort_by: str) -> None:
+
+def test_auto_carver(
+    x_train: DataFrame, x_test_1: DataFrame, output_dtype: str, dropna: bool, sort_by: str
+) -> None:
     """Tests AutoCarver
 
     Parameters
     ----------
     x_train : DataFrame
         Simulated Train DataFrame
     x_test_1 : DataFrame
         Simulated Test DataFrame
     """
 
-    quantitative_features = ['Quantitative', 'Discrete_Quantitative_highnan', 'Discrete_Quantitative_lownan', 'Discrete_Quantitative', 'Discrete_Quantitative_rarevalue']
-    qualitative_features = ["Qualitative", "Qualitative_grouped", "Qualitative_lownan", "Qualitative_highnan", "Discrete_Qualitative_noorder", "Discrete_Qualitative_lownan_noorder", "Discrete_Qualitative_rarevalue_noorder"]
-    ordinal_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan", "Discrete_Qualitative_highnan"]
+    quantitative_features = [
+        "Quantitative",
+        "Discrete_Quantitative_highnan",
+        "Discrete_Quantitative_lownan",
+        "Discrete_Quantitative",
+        "Discrete_Quantitative_rarevalue",
+        "one",
+        "one_nan",
+    ]
+    qualitative_features = [
+        "Qualitative",
+        "Qualitative_grouped",
+        "Qualitative_lownan",
+        "Qualitative_highnan",
+        "Discrete_Qualitative_noorder",
+        "Discrete_Qualitative_lownan_noorder",
+        "Discrete_Qualitative_rarevalue_noorder",
+        "nan",
+        "ones",
+        "ones_nan",
+    ]
+    ordinal_features = [
+        "Qualitative_Ordinal",
+        "Qualitative_Ordinal_lownan",
+        "Discrete_Qualitative_highnan",
+    ]
     values_orders = {
-        "Qualitative_Ordinal": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
-        "Qualitative_Ordinal_lownan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
-        "Discrete_Qualitative_highnan" : ["1", "2", "3", "4", "5", "6", "7"],
+        "Qualitative_Ordinal": [
+            "Low-",
+            "Low",
+            "Low+",
+            "Medium-",
+            "Medium",
+            "Medium+",
+            "High-",
+            "High",
+            "High+",
+        ],
+        "Qualitative_Ordinal_lownan": [
+            "Low-",
+            "Low",
+            "Low+",
+            "Medium-",
+            "Medium",
+            "Medium+",
+            "High-",
+            "High",
+            "High+",
+        ],
+        "Discrete_Qualitative_highnan": ["1", "2", "3", "4", "5", "6", "7"],
     }
 
-
-
     # minimum frequency per modality
     min_freq = 0.06
     max_n_mod = 4
 
     # tests with 'tschuprowt' measure
     auto_carver = AutoCarver(
         quantitative_features=quantitative_features,
@@ -51,38 +100,59 @@
         max_n_mod=max_n_mod,
         sort_by=sort_by,
         output_dtype=output_dtype,
         dropna=dropna,
         copy=True,
         verbose=False,
     )
-    x_discretized = auto_carver.fit_transform(x_train, x_train["quali_ordinal_target"], X_test=x_test_1, y_test=x_test_1["quali_ordinal_target"])
+    x_discretized = auto_carver.fit_transform(
+        x_train,
+        x_train["quali_ordinal_target"],
+        X_test=x_test_1,
+        y_test=x_test_1["quali_ordinal_target"],
+    )
     x_test_discretized = auto_carver.transform(x_test_1)
 
-    assert all(x_discretized[auto_carver.features].nunique() <= max_n_mod), "Too many values after carving of train sample"
-    assert all(x_test_discretized[auto_carver.features].nunique() <= max_n_mod), "Too many values after carving of test sample"
-    assert all(x_discretized[auto_carver.features].nunique() == x_test_discretized[auto_carver.features].nunique()), "More values in train or test samples"
+    assert all(
+        x_discretized[auto_carver.features].nunique() <= max_n_mod
+    ), "Too many values after carving of train sample"
+    assert all(
+        x_test_discretized[auto_carver.features].nunique() <= max_n_mod
+    ), "Too many values after carving of test sample"
+    assert all(
+        x_discretized[auto_carver.features].nunique()
+        == x_test_discretized[auto_carver.features].nunique()
+    ), "More values in train or test samples"
 
-    
     # test that all values still are in the values_orders
     for feature in auto_carver.qualitative_features:
         fitted_values = auto_carver.values_orders[feature].values()
-        init_values = x_train[feature].fillna('__NAN__').unique()
-        assert all(value in fitted_values for value in init_values), f"Missing value in output! Some values are been dropped for qualitative feature: {feature}"
-    
+        init_values = x_train[feature].fillna("__NAN__").unique()
+        assert all(
+            value in fitted_values for value in init_values
+        ), f"Missing value in output! Some values are been dropped for qualitative feature: {feature}"
+
     # testing output of nans
     if not dropna:
-        assert all(x_train[auto_carver.features].isna().mean()  == x_discretized[auto_carver.features].isna().mean()), "Some Nans are being dropped (grouped) or more nans than expected"
+        assert all(
+            x_train[auto_carver.features].isna().mean()
+            == x_discretized[auto_carver.features].isna().mean()
+        ), "Some Nans are being dropped (grouped) or more nans than expected"
     else:
-        assert all(x_discretized[auto_carver.features].isna().mean() == 0), "Some Nans are not dropped (grouped)"
-    
+        assert all(
+            x_discretized[auto_carver.features].isna().mean() == 0
+        ), "Some Nans are not dropped (grouped)"
+
     # testing json serialization
     json_serialized_auto_carver = auto_carver.to_json()
     loaded_carver = load_carver(json_serialized_auto_carver)
 
-    assert all(loaded_carver.summary() == auto_carver.summary()), "Non-identical AutoCarver when loading JSON"
+    assert all(
+        loaded_carver.summary() == auto_carver.summary()
+    ), "Non-identical AutoCarver when loading JSON"
+
 
 # def test_auto_carver_copy(x_train: DataFrame, x_test_1: DataFrame, output_dtype: str, dropna: bool, sort_by: str) -> None:
 
-    # TODO test missing values in test
-    # TODO try with copy = False
-    # TODO: test avec chained_discretizer
+# TODO test missing values in test
+# TODO try with copy = False
+# TODO: test avec chained_discretizer
```

### Comparing `AutoCarver-5.0.4/tests/test_discretizers.py` & `AutoCarver-5.0.5/tests/test_discretizers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,204 @@
 """Set of tests for discretizers module."""
 
-from AutoCarver.discretizers import discretizers
-from pandas import DataFrame
 from numpy import inf
+from pandas import DataFrame
+
+from AutoCarver.discretizers import discretizers
+
 
 def test_quantitative_discretizer(x_train: DataFrame):
     """Tests QuantitativeDiscretizer
 
     Parameters
     ----------
     x_train : DataFrame
         Simulated Train DataFrame
     """
 
-    features = ['Quantitative', 'Discrete_Quantitative', 'Discrete_Quantitative_highnan', 'Discrete_Quantitative_lownan', 'Discrete_Quantitative_rarevalue']
+    features = [
+        "Quantitative",
+        "Discrete_Quantitative",
+        "Discrete_Quantitative_highnan",
+        "Discrete_Quantitative_lownan",
+        "Discrete_Quantitative_rarevalue",
+    ]
     min_freq = 0.1
 
     discretizer = discretizers.QuantitativeDiscretizer(features, min_freq=min_freq)
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
-    assert '__NAN__' in discretizer.values_orders["Discrete_Quantitative_lownan"], "Missing order should not be grouped with ordinal_discretizer"
-    assert all(x_discretized.Quantitative.value_counts(normalize=True) >= min_freq), "Non-nan value was not grouped"
-    assert discretizer.values_orders["Discrete_Quantitative_lownan"] == [1.0, 2.0, 3.0, inf, '__NAN__'], "NaNs should not be grouped whatsoever"
-    assert discretizer.values_orders["Discrete_Quantitative_rarevalue"] == [1.0, 2.0, 3.0, inf], "Rare values should be grouped to the closest one (OrdinalDiscretizer)"
+    assert (
+        "__NAN__" in discretizer.values_orders["Discrete_Quantitative_lownan"]
+    ), "Missing order should not be grouped with ordinal_discretizer"
+    assert all(
+        x_discretized.Quantitative.value_counts(normalize=True) >= min_freq
+    ), "Non-nan value was not grouped"
+    assert discretizer.values_orders["Discrete_Quantitative_lownan"] == [
+        1.0,
+        2.0,
+        3.0,
+        inf,
+        "__NAN__",
+    ], "NaNs should not be grouped whatsoever"
+    assert discretizer.values_orders["Discrete_Quantitative_rarevalue"] == [
+        1.0,
+        2.0,
+        3.0,
+        inf,
+    ], "Rare values should be grouped to the closest one (OrdinalDiscretizer)"
 
 
 def test_qualitative_discretizer(x_train: DataFrame):
     """Tests QualitativeDiscretizer
 
     Parameters
     ----------
     x_train : DataFrame
         Simulated Train DataFrame
     """
 
-
     features = ["Qualitative", "Qualitative_grouped", "Qualitative_lownan", "Qualitative_highnan"]
     ordinal_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan"]
     values_orders = {
-        "Qualitative_Ordinal": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
-        "Qualitative_Ordinal_lownan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+        "Qualitative_Ordinal": [
+            "Low-",
+            "Low",
+            "Low+",
+            "Medium-",
+            "Medium",
+            "Medium+",
+            "High-",
+            "High",
+            "High+",
+        ],
+        "Qualitative_Ordinal_lownan": [
+            "Low-",
+            "Low",
+            "Low+",
+            "Medium-",
+            "Medium",
+            "Medium+",
+            "High-",
+            "High",
+            "High+",
+        ],
     }
 
     min_freq = 0.1
 
-    discretizer = discretizers.QualitativeDiscretizer(features, min_freq, ordinal_features=ordinal_features, values_orders=values_orders, copy=True, verbose=True)
+    discretizer = discretizers.QualitativeDiscretizer(
+        features,
+        min_freq,
+        ordinal_features=ordinal_features,
+        values_orders=values_orders,
+        copy=True,
+        verbose=True,
+    )
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
-
     quali_expected = {
-        '__OTHER__': ['Category A', 'Category D', 'Category F', '__OTHER__'],
-         'Category C': ['Category C'],
-         'Category E': ['Category E'],
-    }
-    assert discretizer.values_orders['Qualitative'].content == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
+        "__OTHER__": ["Category A", "Category D", "Category F", "__OTHER__"],
+        "Category C": ["Category C"],
+        "Category E": ["Category E"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative"].content == quali_expected
+    ), "Values less frequent than min_freq should be grouped into default_value"
     quali_lownan_expected = {
-        '__NAN__': ['__NAN__'],
-        '__OTHER__': ['Category D', 'Category F', '__OTHER__'],
-        'Category C': ['Category C'],
-        'Category E': ['Category E'],
-    }
-    assert discretizer.values_orders['Qualitative_lownan'].content == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
+        "__NAN__": ["__NAN__"],
+        "__OTHER__": ["Category D", "Category F", "__OTHER__"],
+        "Category C": ["Category C"],
+        "Category E": ["Category E"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_lownan"].content == quali_lownan_expected
+    ), "If any, NaN values should be put into str_nan and kept by themselves"
 
     expected_ordinal = {
-        'Low+': ['Low-', 'Low', 'Low+'],
-        'Medium-': ['Medium-'],
-        'Medium': ['Medium'],
-        'High': ['Medium+', 'High-', 'High'],
-        'High+': ['High+']
+        "Low+": ["Low-", "Low", "Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "High": ["Medium+", "High-", "High"],
+        "High+": ["High+"],
     }
     expected_ordinal_lownan = {
-        'Low+': ['Low', 'Low-', 'Low+'],
-        'Medium-': ['Medium-'],
-        'Medium': ['Medium'],
-        'High': ['Medium+', 'High-', 'High'],
-        'High+': ['High+'],
-        '__NAN__': ['__NAN__']
-    }
-    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected_ordinal, "Values not correctly grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected_ordinal_lownan, "NaNs should stay by themselves."
+        "Low+": ["Low", "Low-", "Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "High": ["Medium+", "High-", "High"],
+        "High+": ["High+"],
+        "__NAN__": ["__NAN__"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal"].content == expected_ordinal
+    ), "Values not correctly grouped"
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal_lownan"].content == expected_ordinal_lownan
+    ), "NaNs should stay by themselves."
+
 
 def test_discretizer(x_train: DataFrame, x_test_1: DataFrame):
     """Tests Discretizer
 
     Parameters
     ----------
     x_train : DataFrame
         Simulated Train DataFrame
     x_test_1 : DataFrame
         Simulated Test DataFrame
     """
 
-    quantitative_features = ['Quantitative', 'Discrete_Quantitative_highnan', 'Discrete_Quantitative_lownan', 'Discrete_Quantitative', 'Discrete_Quantitative_rarevalue']
-    qualitative_features = ["Qualitative", "Qualitative_grouped", "Qualitative_lownan", "Qualitative_highnan", "Discrete_Qualitative_noorder", "Discrete_Qualitative_lownan_noorder", "Discrete_Qualitative_rarevalue_noorder"]
-    ordinal_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan", "Discrete_Qualitative_highnan"]
+    quantitative_features = [
+        "Quantitative",
+        "Discrete_Quantitative_highnan",
+        "Discrete_Quantitative_lownan",
+        "Discrete_Quantitative",
+        "Discrete_Quantitative_rarevalue",
+    ]
+    qualitative_features = [
+        "Qualitative",
+        "Qualitative_grouped",
+        "Qualitative_lownan",
+        "Qualitative_highnan",
+        "Discrete_Qualitative_noorder",
+        "Discrete_Qualitative_lownan_noorder",
+        "Discrete_Qualitative_rarevalue_noorder",
+    ]
+    ordinal_features = [
+        "Qualitative_Ordinal",
+        "Qualitative_Ordinal_lownan",
+        "Discrete_Qualitative_highnan",
+    ]
     values_orders = {
-        "Qualitative_Ordinal": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
-        "Qualitative_Ordinal_lownan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
-        "Discrete_Qualitative_highnan" : ["1", "2", "3", "4", "5", "6", "7"],
+        "Qualitative_Ordinal": [
+            "Low-",
+            "Low",
+            "Low+",
+            "Medium-",
+            "Medium",
+            "Medium+",
+            "High-",
+            "High",
+            "High+",
+        ],
+        "Qualitative_Ordinal_lownan": [
+            "Low-",
+            "Low",
+            "Low+",
+            "Medium-",
+            "Medium",
+            "Medium+",
+            "High-",
+            "High",
+            "High+",
+        ],
+        "Discrete_Qualitative_highnan": ["1", "2", "3", "4", "5", "6", "7"],
     }
 
-
-
     # minimum frequency per modality + apply(find_common_modalities) outputs a Series
     min_freq = 0.1
 
     # discretizing features
     discretizer = discretizers.Discretizer(
         quantitative_features=quantitative_features,
         qualitative_features=qualitative_features,
@@ -113,78 +206,106 @@
         values_orders=values_orders,
         min_freq=min_freq,
         copy=True,
     )
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
     x_test_discretized = discretizer.transform(x_test_1)
 
-
-
-    assert all(x_discretized.Quantitative.value_counts(normalize=True) >= min_freq), "Non-nan value was not grouped"
-    assert discretizer.values_orders["Discrete_Quantitative_lownan"] == [1.0, 2.0, 3.0, inf, '__NAN__'], "NaNs should not be grouped whatsoever"
-    assert discretizer.values_orders["Discrete_Quantitative_rarevalue"] == [1.0, 2.0, 3.0, inf], "Rare values should be grouped to the closest one (OrdinalDiscretizer)"
-
+    assert all(
+        x_discretized.Quantitative.value_counts(normalize=True) >= min_freq
+    ), "Non-nan value was not grouped"
+    assert discretizer.values_orders["Discrete_Quantitative_lownan"] == [
+        1.0,
+        2.0,
+        3.0,
+        inf,
+        "__NAN__",
+    ], "NaNs should not be grouped whatsoever"
+    assert discretizer.values_orders["Discrete_Quantitative_rarevalue"] == [
+        1.0,
+        2.0,
+        3.0,
+        inf,
+    ], "Rare values should be grouped to the closest one (OrdinalDiscretizer)"
 
     quali_expected = {
-        '__OTHER__': ['Category A', 'Category D', 'Category F', '__OTHER__'],
-        'Category C': ['Category C'],
-        'Category E': ['Category E'],
-    }
-    assert discretizer.values_orders['Qualitative'].content == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
+        "__OTHER__": ["Category A", "Category D", "Category F", "__OTHER__"],
+        "Category C": ["Category C"],
+        "Category E": ["Category E"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative"].content == quali_expected
+    ), "Values less frequent than min_freq should be grouped into default_value"
     quali_lownan_expected = {
-        '__NAN__' : ['__NAN__'],
-        '__OTHER__': ['Category D', 'Category F', '__OTHER__'],
-        'Category C': ['Category C'],
-        'Category E': ['Category E'],
-    }
-    assert discretizer.values_orders['Qualitative_lownan'].content == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
+        "__NAN__": ["__NAN__"],
+        "__OTHER__": ["Category D", "Category F", "__OTHER__"],
+        "Category C": ["Category C"],
+        "Category E": ["Category E"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_lownan"].content == quali_lownan_expected
+    ), "If any, NaN values should be put into str_nan and kept by themselves"
 
     expected_ordinal = {
-        'Low+': ['Low-', 'Low', 'Low+'],
-        'Medium-': ['Medium-'],
-        'Medium': ['Medium'],
-        'High': ['Medium+', 'High-', 'High'],
-        'High+': ['High+']
+        "Low+": ["Low-", "Low", "Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "High": ["Medium+", "High-", "High"],
+        "High+": ["High+"],
     }
     expected_ordinal_lownan = {
-        'Low+': ['Low', 'Low-', 'Low+'],
-        'Medium-': ['Medium-'],
-        'Medium': ['Medium'],
-        'High': ['Medium+', 'High-', 'High'],
-        'High+': ['High+'],
-        '__NAN__': ['__NAN__'],
-    }
-    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected_ordinal, "Values not correctly grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected_ordinal_lownan, "NaNs should stay by themselves."
+        "Low+": ["Low", "Low-", "Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "High": ["Medium+", "High-", "High"],
+        "High+": ["High+"],
+        "__NAN__": ["__NAN__"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal"].content == expected_ordinal
+    ), "Values not correctly grouped"
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal_lownan"].content == expected_ordinal_lownan
+    ), "NaNs should stay by themselves."
 
     # Testing out qualitative with int/float values inside -> StringDiscretizer
     expected = {
-        '2': [2.0, '2'],
-        '4': [4.0, '4'],
-        '1': [1.0, '1'],
-        '3': [3.0, '3'],
-        '__OTHER__': [0.5, '0.5', 6.0, '6', 5.0, '5', '__OTHER__']
-    }
-    assert discretizer.values_orders["Discrete_Qualitative_rarevalue_noorder"].content == expected, "Qualitative features with float values should be converted to string and there values stored in the values_orders"
+        "2": [2.0, "2"],
+        "4": [4.0, "4"],
+        "1": [1.0, "1"],
+        "3": [3.0, "3"],
+        "__OTHER__": [0.5, "0.5", 6.0, "6", 5.0, "5", "__OTHER__"],
+    }
+    assert (
+        discretizer.values_orders["Discrete_Qualitative_rarevalue_noorder"].content == expected
+    ), "Qualitative features with float values should be converted to string and there values stored in the values_orders"
     expected = {
-        '2': [2, '2'],
-        '4': [4, '4'],
-        '1': [1, '1'],
-        '3': [3, '3'],
-        '__OTHER__': [7, '7', 6, '6', 5, '5', '__OTHER__']
-    }
-    assert discretizer.values_orders["Discrete_Qualitative_noorder"].content == expected, "Qualitative features with int values should be converted to string and there values stored in the values_orders"
+        "2": [2, "2"],
+        "4": [4, "4"],
+        "1": [1, "1"],
+        "3": [3, "3"],
+        "__OTHER__": [7, "7", 6, "6", 5, "5", "__OTHER__"],
+    }
+    assert (
+        discretizer.values_orders["Discrete_Qualitative_noorder"].content == expected
+    ), "Qualitative features with int values should be converted to string and there values stored in the values_orders"
     expected = {
-        '2': ['1', 2.0, '2'],
-        '3': [3.0, '3'],
-        '4': [4.0, '4'],
-        '5': [6.0, '6', 7.0, '7', 5.0, '5'],
-        '__NAN__': ['__NAN__']
-    }
-    assert discretizer.values_orders["Discrete_Qualitative_highnan"].content == expected, "Ordinal qualitative features with int or float values that contain nan should be converted to string and there values stored in the values_orders"
+        "2": ["1", 2.0, "2"],
+        "3": [3.0, "3"],
+        "4": [4.0, "4"],
+        "5": [6.0, "6", 7.0, "7", 5.0, "5"],
+        "__NAN__": ["__NAN__"],
+    }
+    assert (
+        discretizer.values_orders["Discrete_Qualitative_highnan"].content == expected
+    ), "Ordinal qualitative features with int or float values that contain nan should be converted to string and there values stored in the values_orders"
 
     # checking for inconsistancies in tranform
     for feature in discretizer.features:
         test_unique = x_test_discretized[feature].unique()
         train_unique = x_discretized[feature].unique()
-        assert all(value in test_unique for value in train_unique), "Missing value from test (at transform step)"
-        assert all(value in train_unique for value in test_unique), "Missing value from train (at transform step)"
+        assert all(
+            value in test_unique for value in train_unique
+        ), "Missing value from test (at transform step)"
+        assert all(
+            value in train_unique for value in test_unique
+        ), "Missing value from train (at transform step)"
```

### Comparing `AutoCarver-5.0.4/tests/test_qualitative_discretizers.py` & `AutoCarver-5.0.5/tests/test_qualitative_discretizers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,158 @@
 """Set of tests for qualitative_discretizers module."""
 
-from AutoCarver.discretizers.utils.qualitative_discretizers import *
+from pandas import DataFrame
 from pytest import raises
 
+from AutoCarver.discretizers.utils.qualitative_discretizers import ChainedDiscretizer, DefaultDiscretizer, OrdinalDiscretizer
+from AutoCarver.discretizers.utils.grouped_list import GroupedList
+
 
 def test_chained_discretizer(x_train: DataFrame) -> None:
     """Tests DefaultDiscretizer
 
     Parameters
     ----------
     x_train : DataFrame
         Simulated Train DataFrame
     """
     ordinal_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan"]
     values_orders = {
-        "Qualitative_Ordinal_lownan": ['Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
-        "Qualitative_Ordinal_highnan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+        "Qualitative_Ordinal_lownan": [
+            "Low+",
+            "Medium-",
+            "Medium",
+            "Medium+",
+            "High-",
+            "High",
+            "High+",
+        ],
+        "Qualitative_Ordinal_highnan": [
+            "Low-",
+            "Low",
+            "Low+",
+            "Medium-",
+            "Medium",
+            "Medium+",
+            "High-",
+            "High",
+            "High+",
+        ],
     }
 
     level0_to_level1 = {
-        "Lows": ['Low-', 'Low', 'Low+', 'Lows'],
-        "Mediums": ['Medium-', 'Medium', 'Medium+', 'Mediums'],
-        "Highs": ['High-', 'High', 'High+', 'Highs'],
+        "Lows": ["Low-", "Low", "Low+", "Lows"],
+        "Mediums": ["Medium-", "Medium", "Medium+", "Mediums"],
+        "Highs": ["High-", "High", "High+", "Highs"],
     }
     level1_to_level2 = {
-        "Worst": ['Lows', 'Mediums', 'Worst'],
-        "Best": ['Highs', "Best"],
+        "Worst": ["Lows", "Mediums", "Worst"],
+        "Best": ["Highs", "Best"],
     }
 
-
     min_freq = 0.15
 
     discretizer = ChainedDiscretizer(
         features=ordinal_features,
         chained_orders=[level0_to_level1, level1_to_level2],
         min_freq=min_freq,
         values_orders=values_orders,
         copy=True,
     )
     x_discretized = discretizer.fit_transform(x_train)
 
-    expected = {'High+': ['High+'],
-    'Best': ['High', 'High-', 'Highs', 'Best'],
-    'Mediums': ['Medium+', 'Medium-', 'Mediums'],
-    'Medium': ['Medium'],
-    'Worst': ['Low+', 'Low', 'Low-', 'Lows', 'Worst']}
-    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected, "Values less frequent than min_freq should be grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal'] == ['Medium', 'Mediums', 'Worst', 'High+', 'Best'], "Order of ordinal features is wrong"
-
-    expected = {'Low-': ['Low-'],
-    'Low': ['Low'],
-    'Low+': ['Low+'],
-    'Medium-': ['Medium-'],
-    'Medium': ['Medium'],
-    'Medium+': ['Medium+'],
-    'High-': ['High-'],
-    'High': ['High'],
-    'High+': ['High+']}
-    assert discretizer.values_orders['Qualitative_Ordinal_highnan'].content == expected, "Not specified features should not be modified"
-
-    expected = {'Medium': ['Medium'],
-    'High+': ['High+'],
-    'Best': ['High', 'High-', 'Highs', 'Best'],
-    'Mediums': ['Medium+', 'Medium-', 'Mediums'],
-    'Worst': ['Low+', 'Low', 'Low-', 'Lows', 'Worst'],
-    '__NAN__': ['__NAN__']}
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected, "NaNs should be added to the order and missing values from the values_orders should be added (from chained_orders)"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'] == ['Medium', 'Mediums', 'Worst', 'High+', 'Best', '__NAN__'], "Order of ordinal features is wrong"
+    expected = {
+        "High+": ["High+"],
+        "Best": ["High", "High-", "Highs", "Best"],
+        "Mediums": ["Medium+", "Medium-", "Mediums"],
+        "Medium": ["Medium"],
+        "Worst": ["Low+", "Low", "Low-", "Lows", "Worst"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal"].content == expected
+    ), "Values less frequent than min_freq should be grouped"
+    assert discretizer.values_orders["Qualitative_Ordinal"] == [
+        "Medium",
+        "Mediums",
+        "Worst",
+        "High+",
+        "Best",
+    ], "Order of ordinal features is wrong"
+
+    expected = {
+        "Low-": ["Low-"],
+        "Low": ["Low"],
+        "Low+": ["Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "Medium+": ["Medium+"],
+        "High-": ["High-"],
+        "High": ["High"],
+        "High+": ["High+"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal_highnan"].content == expected
+    ), "Not specified features should not be modified"
+
+    expected = {
+        "Medium": ["Medium"],
+        "High+": ["High+"],
+        "Best": ["High", "High-", "Highs", "Best"],
+        "Mediums": ["Medium+", "Medium-", "Mediums"],
+        "Worst": ["Low+", "Low", "Low-", "Lows", "Worst"],
+        "__NAN__": ["__NAN__"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal_lownan"].content == expected
+    ), "NaNs should be added to the order and missing values from the values_orders should be added (from chained_orders)"
+    assert discretizer.values_orders["Qualitative_Ordinal_lownan"] == [
+        "Medium",
+        "Mediums",
+        "Worst",
+        "High+",
+        "Best",
+        "__NAN__",
+    ], "Order of ordinal features is wrong"
 
     # testing that it does not work when there is a vale in values_orders missing from chained_orders
     with raises(AssertionError):
         values_orders = {
-            "Qualitative_Ordinal_lownan": ['-Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
-            "Qualitative_Ordinal_highnan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+            "Qualitative_Ordinal_lownan": [
+                "-Low",
+                "Low+",
+                "Medium-",
+                "Medium",
+                "Medium+",
+                "High-",
+                "High",
+                "High+",
+            ],
+            "Qualitative_Ordinal_highnan": [
+                "Low-",
+                "Low",
+                "Low+",
+                "Medium-",
+                "Medium",
+                "Medium+",
+                "High-",
+                "High",
+                "High+",
+            ],
         }
 
         level0_to_level1 = {
-            "Lows": ['Low-', 'Low', 'Low+', 'Lows'],
-            "Mediums": ['Medium-', 'Medium', 'Medium+', 'Mediums'],
-            "Highs": ['High-', 'High', 'High+', 'Highs'],
+            "Lows": ["Low-", "Low", "Low+", "Lows"],
+            "Mediums": ["Medium-", "Medium", "Medium+", "Mediums"],
+            "Highs": ["High-", "High", "High+", "Highs"],
         }
         level1_to_level2 = {
-            "Worst": ['Lows', 'Mediums', 'Worst'],
-            "Best": ['Highs', "Best"],
+            "Worst": ["Lows", "Mediums", "Worst"],
+            "Best": ["Highs", "Best"],
         }
 
-
         min_freq = 0.15
 
         discretizer = ChainedDiscretizer(
             features=ordinal_features,
             chained_orders=[level0_to_level1, level1_to_level2],
             min_freq=min_freq,
             values_orders=values_orders,
@@ -104,45 +167,43 @@
     Parameters
     ----------
     x_train : DataFrame
         Simulated Train DataFrame
     """
 
     # defining values_orders
-    order = ['Category A', 'Category B', 'Category C', 'Category D', 'Category E', 'Category F']
+    order = ["Category A", "Category B", "Category C", "Category D", "Category E", "Category F"]
     # ordering for base qualitative ordinal feature
     groupedlist = GroupedList(order)
-    groupedlist_lownan = GroupedList(['Category C', 'Category D', 'Category E', 'Category F'])
-    groupedlist_highnan = GroupedList(['Category A',  'Category C', 'Category D', 'Category E'])
+    groupedlist_lownan = GroupedList(["Category C", "Category D", "Category E", "Category F"])
+    groupedlist_highnan = GroupedList(["Category A", "Category C", "Category D", "Category E"])
 
     # ordering for qualitative ordinal feature that contains NaNs
     groupedlist_grouped = GroupedList(order)
     groupedlist_grouped.group("Category A", "Category D")
 
-
     # ordering for base qualitative ordinal feature
-    order = ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+']
+    order = ["Low-", "Low", "Low+", "Medium-", "Medium", "Medium+", "High-", "High", "High+"]
     groupedlist_ordinal = GroupedList(order)
-    groupedlist_ordinal.group_list(['Low-', 'Low'], 'Low+')
-    groupedlist_ordinal.group_list(['Medium+', 'High-'], 'High')
+    groupedlist_ordinal.group_list(["Low-", "Low"], "Low+")
+    groupedlist_ordinal.group_list(["Medium+", "High-"], "High")
 
     # storing per feature orders
     values_orders = {
         "Qualitative_grouped": groupedlist_grouped,
         "Qualitative_highnan": groupedlist,
         "Qualitative_lownan": groupedlist,
         "Qualitative_Ordinal": groupedlist_ordinal,
     }
 
     features = ["Qualitative", "Qualitative_grouped", "Qualitative_lownan", "Qualitative_highnan"]
 
     min_freq = 0.02
     # unwanted value in values_orders
     with raises(AssertionError):
-
         discretizer = DefaultDiscretizer(features, min_freq, values_orders=values_orders, copy=True)
         x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     # correct feature ordering
     groupedlist_grouped.group("Category B", "Category D")
     values_orders = {
         "Qualitative_grouped": groupedlist_grouped,
@@ -150,47 +211,75 @@
         "Qualitative_lownan": groupedlist_lownan,
         "Qualitative_Ordinal": groupedlist_ordinal,
     }
 
     discretizer = DefaultDiscretizer(features, min_freq, values_orders=values_orders, copy=True)
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
-    assert discretizer.values_orders['Qualitative_Ordinal'].content == groupedlist_ordinal.content, "Column names of values_orders not provided if features should not be discretized."
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal"].content == groupedlist_ordinal.content
+    ), "Column names of values_orders not provided if features should not be discretized."
     quali_expected = {
-        '__OTHER__': ['Category A', '__OTHER__'],
-        'Category C': ['Category C'],
-        'Category F': ['Category F'],
-        'Category E': ['Category E'],
-        'Category D': ['Category D']
-    }
-    quali_expected_order = ['Category D', '__OTHER__', 'Category F', 'Category C', 'Category E']
-    assert discretizer.values_orders['Qualitative'] == quali_expected_order, "Incorrect ordering by target rate"
-    assert discretizer.values_orders['Qualitative'].content == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
+        "__OTHER__": ["Category A", "__OTHER__"],
+        "Category C": ["Category C"],
+        "Category F": ["Category F"],
+        "Category E": ["Category E"],
+        "Category D": ["Category D"],
+    }
+    quali_expected_order = ["Category D", "__OTHER__", "Category F", "Category C", "Category E"]
+    assert (
+        discretizer.values_orders["Qualitative"] == quali_expected_order
+    ), "Incorrect ordering by target rate"
+    assert (
+        discretizer.values_orders["Qualitative"].content == quali_expected
+    ), "Values less frequent than min_freq should be grouped into default_value"
     quali_lownan_expected = {
-        '__NAN__': ['__NAN__'],
-        'Category C': ['Category C'],
-        'Category F': ['Category F'],
-        'Category E': ['Category E'],
-        'Category D': ['Category D']
-    }
-    quali_lownan_expected_order = ['Category D', 'Category F', 'Category C', 'Category E', '__NAN__']
-    assert discretizer.values_orders['Qualitative_lownan'] == quali_lownan_expected_order, "Incorrect ordering by target rate"
-    assert discretizer.values_orders['Qualitative_lownan'].content == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
+        "__NAN__": ["__NAN__"],
+        "Category C": ["Category C"],
+        "Category F": ["Category F"],
+        "Category E": ["Category E"],
+        "Category D": ["Category D"],
+    }
+    quali_lownan_expected_order = [
+        "Category D",
+        "Category F",
+        "Category C",
+        "Category E",
+        "__NAN__",
+    ]
+    assert (
+        discretizer.values_orders["Qualitative_lownan"] == quali_lownan_expected_order
+    ), "Incorrect ordering by target rate"
+    assert (
+        discretizer.values_orders["Qualitative_lownan"].content == quali_lownan_expected
+    ), "If any, NaN values should be put into str_nan and kept by themselves"
     quali_highnan_expected = {
-        '__OTHER__': ['Category A', '__OTHER__'],
-        'Category C': ['Category C'],
-        '__NAN__': ['__NAN__'],
-        'Category E': ['Category E'],
-        'Category D': ['Category D']
-    }
-    quali_highnan_expected_order = ['Category D', '__OTHER__', 'Category C', 'Category E', '__NAN__']
-    assert discretizer.values_orders['Qualitative_highnan'] == quali_highnan_expected_order, "Incorrect ordering by target rate"
-    assert discretizer.values_orders['Qualitative_highnan'].content == quali_highnan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
-
-    assert discretizer.values_orders['Qualitative_grouped'].content == groupedlist_grouped.content, "Grouped values should keep there group"
+        "__OTHER__": ["Category A", "__OTHER__"],
+        "Category C": ["Category C"],
+        "__NAN__": ["__NAN__"],
+        "Category E": ["Category E"],
+        "Category D": ["Category D"],
+    }
+    quali_highnan_expected_order = [
+        "Category D",
+        "__OTHER__",
+        "Category C",
+        "Category E",
+        "__NAN__",
+    ]
+    assert (
+        discretizer.values_orders["Qualitative_highnan"] == quali_highnan_expected_order
+    ), "Incorrect ordering by target rate"
+    assert (
+        discretizer.values_orders["Qualitative_highnan"].content == quali_highnan_expected
+    ), "If any, NaN values should be put into str_nan and kept by themselves"
+
+    assert (
+        discretizer.values_orders["Qualitative_grouped"].content == groupedlist_grouped.content
+    ), "Grouped values should keep there group"
 
 
 def test_ordinal_discretizer(x_train: DataFrame) -> None:
     """Tests OrdinalDiscretizer
 
     # TODO: add tests for quantitative features
 
@@ -201,15 +290,15 @@
     x_test_1 : DataFrame
         Simulated Test DataFrame
     x_test_2 : DataFrame
         Simulated Test DataFrame
     """
 
     # defining values_orders
-    order = ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+']
+    order = ["Low-", "Low", "Low+", "Medium-", "Medium", "Medium+", "High-", "High", "High+"]
     # ordering for base qualitative ordinal feature
     groupedlist = GroupedList(order)
 
     # ordering for qualitative ordinal feature that contains NaNs
     groupedlist_lownan = GroupedList(order)
 
     # storing per feature orders
@@ -223,51 +312,61 @@
     min_freq = 0.01
 
     # discretizing features
     discretizer = OrdinalDiscretizer(features, values_orders, min_freq, copy=True)
     discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     expected_ordinal_01 = {
-        'Low-': ['Low', 'Low-'],
-        'Low+': ['Low+'],
-        'Medium-': ['Medium-'],
-        'Medium': ['Medium'],
-        'Medium+': ['High-', 'Medium+'],
-        'High': ['High'],
-        'High+': ['High+']
+        "Low-": ["Low", "Low-"],
+        "Low+": ["Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "Medium+": ["High-", "Medium+"],
+        "High": ["High"],
+        "High+": ["High+"],
     }
     expected_ordinal_lownan_01 = {
-        'Low+': ['Low', 'Low-', 'Low+'],
-        'Medium-': ['Medium-'],
-        'Medium': ['Medium'],
-        'Medium+': ['High-', 'Medium+'],
-        'High': ['High'],
-        'High+': ['High+'],
-        '__NAN__': ['__NAN__']
-    }
-    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected_ordinal_01, "Missing value in order not correctly grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected_ordinal_lownan_01, "Missing value in order not correctly grouped or introduced nans."
+        "Low+": ["Low", "Low-", "Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "Medium+": ["High-", "Medium+"],
+        "High": ["High"],
+        "High+": ["High+"],
+        "__NAN__": ["__NAN__"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal"].content == expected_ordinal_01
+    ), "Missing value in order not correctly grouped"
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal_lownan"].content
+        == expected_ordinal_lownan_01
+    ), "Missing value in order not correctly grouped or introduced nans."
 
     # minimum frequency per modality + apply(find_common_modalities) outputs a DataFrame
     min_freq = 0.08
 
     # discretizing features
     discretizer = OrdinalDiscretizer(features, values_orders, min_freq, copy=True)
     discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     expected_ordinal_08 = {
-        'Low+': ['Low-', 'Low', 'Low+'],
-        'Medium-': ['Medium-'],
-        'Medium': ['Medium'],
-        'High': ['Medium+', 'High-', 'High'],
-        'High+': ['High+']
+        "Low+": ["Low-", "Low", "Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "High": ["Medium+", "High-", "High"],
+        "High+": ["High+"],
     }
     expected_ordinal_lownan_08 = {
-        'Low+': ['Low', 'Low-', 'Low+'],
-        'Medium-': ['Medium-'],
-        'Medium': ['Medium'],
-        'High': ['Medium+', 'High-', 'High'],
-        'High+': ['High+'],
-        '__NAN__': ['__NAN__']
-    }
-    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected_ordinal_08, "Values not correctly grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected_ordinal_lownan_08, "NaNs should stay by themselves."
+        "Low+": ["Low", "Low-", "Low+"],
+        "Medium-": ["Medium-"],
+        "Medium": ["Medium"],
+        "High": ["Medium+", "High-", "High"],
+        "High+": ["High+"],
+        "__NAN__": ["__NAN__"],
+    }
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal"].content == expected_ordinal_08
+    ), "Values not correctly grouped"
+    assert (
+        discretizer.values_orders["Qualitative_Ordinal_lownan"].content
+        == expected_ordinal_lownan_08
+    ), "NaNs should stay by themselves."
```

