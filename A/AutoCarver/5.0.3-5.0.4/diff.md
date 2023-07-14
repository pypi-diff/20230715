# Comparing `tmp/AutoCarver-5.0.3.tar.gz` & `tmp/AutoCarver-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.3.tar", last modified: Fri Jul 14 20:32:07 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.4.tar", last modified: Fri Jul 14 23:45:29 2023, max compression
```

## Comparing `AutoCarver-5.0.3.tar` & `AutoCarver-5.0.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.393093 AutoCarver-5.0.3/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29849 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.393093 AutoCarver-5.0.3/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22567 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41746 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28712 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.393093 AutoCarver-5.0.3/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 20:32:07.000000 AutoCarver-5.0.3/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 20:32:07.000000 AutoCarver-5.0.3/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:32:07.000000 AutoCarver-5.0.3/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 20:32:07.000000 AutoCarver-5.0.3/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30748 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31419 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28756 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 23:45:29.000000 AutoCarver-5.0.4/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-14 23:45:29.000000 AutoCarver-5.0.4/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:45:29.000000 AutoCarver-5.0.4/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 23:45:29.000000 AutoCarver-5.0.4/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:45:29.291212 AutoCarver-5.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-14 23:45:16.000000 AutoCarver-5.0.4/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.3/AutoCarver/auto_carver.py` & `AutoCarver-5.0.4/AutoCarver/auto_carver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Tool to build optimized buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
-from typing import Any, Dict, List, Tuple
+from typing import Any
 
 import numpy as np
 from IPython.display import display_html  # TODO: remove this
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.pyplot import subplots
 from matplotlib.ticker import PercentFormatter
 from pandas import DataFrame, Series, crosstab, unique
 from scipy.stats import chi2_contingency
 from seaborn import color_palette, despine
 from tqdm import tqdm
+from json import loads
 
 from .discretizers.discretizers import Discretizer
 from .discretizers.utils.base_discretizers import (
-    GroupedList,
     GroupedListDiscretizer,
     convert_to_labels,
     convert_to_values,
-    is_equal,
 )
+from .discretizers.utils.grouped_list import is_equal, GroupedList
+from .discretizers.utils.serialization import json_deserialize_values_orders
 
 
 # TODO: display tables
 class AutoCarver(GroupedListDiscretizer):
     """Automatic carving of continuous, categorical and categorical ordinal
     features that maximizes association with a binary target.
 
@@ -115,43 +116,43 @@
     # applying pipe to a validation set or in production
     X_val = pipe.transform(X_val)
 
     """
 
     def __init__(
         self,
-        quantitative_features: List[str],
-        qualitative_features: List[str],
+        quantitative_features: list[str],
+        qualitative_features: list[str],
         min_freq: float,
         *,
-        ordinal_features: List[str] = None,
-        values_orders: Dict[str, GroupedList] = None,
+        ordinal_features: list[str] = None,
+        values_orders: dict[str, GroupedList] = None,
         max_n_mod: int = 5,
         min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
         sort_by: str = "tschuprowt",
         str_nan: str = "__NAN__",
         str_default: str = "__OTHER__",
         output_dtype: str = 'float',
         dropna: bool = True,
         copy: bool = False,
         verbose: bool = True,
     ) -> None:
         """_summary_
 
         Parameters
         ----------
-        quantitative_features : List[str]
+        quantitative_features : list[str]
             _description_
-        qualitative_features : List[str]
+        qualitative_features : list[str]
             _description_
         min_freq : float
             _description_
-        ordinal_features : List[str], optional
+        ordinal_features : list[str], optional
             _description_, by default None
-        values_orders : Dict[str, GroupedList], optional
+        values_orders : dict[str, GroupedList], optional
             _description_, by default None
         max_n_mod : int, optional
             _description_, by default 5
         min_carved_freq : float, optional
             _description_, by default 0
         str_nan : str, optional
             _description_, by default "__NAN__"
@@ -202,15 +203,15 @@
 
     def prepare_data(
         self,
         X: DataFrame,
         y: Series,
         X_test: DataFrame = None,
         y_test: Series = None,
-    ) -> Tuple[DataFrame, DataFrame]:
+    ) -> tuple[DataFrame, DataFrame]:
         """Checks validity of provided data
 
         Parameters
         ----------
         X : DataFrame
             _description_
         y : Series
@@ -218,15 +219,15 @@
         X_test : DataFrame, optional
             _description_, by default None
         y_test : Series, optional
             _description_, by default None
 
         Returns
         -------
-        Tuple[DataFrame, DataFrame]
+        tuple[DataFrame, DataFrame]
             Copies of (X, X_test)
         """
         # Checking for binary target and copying X
         x_copy = super().prepare_data(X, y)
         x_test_copy = super().prepare_data(X_test, y_test)
 
         return x_copy, x_test_copy
@@ -361,15 +362,15 @@
 
     def get_best_combination(
         self,
         order: GroupedList,
         xtab: DataFrame,
         *,
         xtab_test: DataFrame = None,
-    ) -> Tuple[GroupedList, DataFrame, DataFrame]:
+    ) -> tuple[GroupedList, DataFrame, DataFrame]:
         # raw ordering
         raw_order = GroupedList(order)
         if self.str_nan in raw_order:
             raw_order.remove(self.str_nan)
 
         # filtering out nans if requested from train/test crosstabs
         raw_xtab = filter_nan_xtab(xtab, self.str_nan)
@@ -475,16 +476,16 @@
 
         # displaying html of colored DataFrame
         display_html(html, raw=True)
 
 
 def stats_xtab(
     xtab: DataFrame,
-    known_order: List[Any] = None,
-    known_labels: List[Any] = None,
+    known_order: list[Any] = None,
+    known_labels: list[Any] = None,
 ) -> DataFrame:
     """Computes column (target) rate per row (modality) and row frequency"""
 
     # target rate and frequency statistics per modality
     stats = DataFrame(
         {
             # target rate per modality
@@ -542,16 +543,16 @@
         if str_nan in xtab.index:
             filtered_xtab = xtab.drop(str_nan, axis=0)
 
     return filtered_xtab
 
 
 def get_xtabs(
-    features: List[str], X: DataFrame, y: Series, labels_orders: Dict[str, GroupedList]
-) -> Dict[str, DataFrame]:
+    features: list[str], X: DataFrame, y: Series, labels_orders: dict[str, GroupedList]
+) -> dict[str, DataFrame]:
     """Computes crosstabs for specified features and ensures that the crosstab is ordered according to the known labels"""
 
     # checking for empty datasets
     xtabs = {feature: None for feature in features}
     if X is not None:
         # crosstab for each feature
         for feature in features:
@@ -563,15 +564,15 @@
 
             # storing results
             xtabs.update({feature: xtab})
 
     return xtabs
 
 
-def association_xtab(xtab: DataFrame, n_obs, n_mod_y) -> Dict[str, float]:
+def association_xtab(xtab: DataFrame, n_obs, n_mod_y) -> dict[str, float]:
     """Computes measures of association between feature x and feature2."""
 
     # number of values taken by the features
     n_mod_x = xtab.shape[0]
 
     # Chi2 statistic
     chi2 = chi2_contingency(xtab)[0]
@@ -581,15 +582,15 @@
 
     # Tschuprow's T
     tschuprowt = np.sqrt(chi2 / n_obs / np.sqrt((n_mod_x - 1) * (n_mod_y - 1)))
 
     return {"cramerv": cramerv, "tschuprowt": tschuprowt}
 
 
-def vectorized_groupby_sum(xtab: DataFrame, groupby: List[str]):
+def vectorized_groupby_sum(xtab: DataFrame, groupby: list[str]):
     """Groups a crosstab by groupby and sums column values by groups"""
 
     # all indices that may be duplicated
     index_values = np.array(groupby)
 
     # all unique indices deduplicated
     unique_indices = np.unique(index_values)
@@ -676,19 +677,19 @@
     """Computes target rate per row for a binary target (column) in a crosstab"""
 
     return xtab[1].divide(xtab[0]).sort_values()
 
 
 def get_best_association(
     xtab: DataFrame,
-    combinations: List[List[str]],
+    combinations: list[list[str]],
     sort_by: str,
     xtab_test: DataFrame = None,
     verbose: bool = False,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """Computes associations of the xtab for each combination"""
 
     # values to groupby indices with
     indices_to_groupby = [
         [value for values in ([group[0]] * len(group) for group in combination) for value in values]
         for combination in combinations
     ]
@@ -743,16 +744,16 @@
 
         # viable on test sample: grouped values have the same ranks in train/test
         if all(train_ranks == test_ranks):
             return association
 
 
 def add_nan_in_combinations(
-    combinations: List[List[str]], str_nan: str, max_n_mod: int
-) -> List[List[str]]:
+    combinations: list[list[str]], str_nan: str, max_n_mod: int
+) -> list[list[str]]:
     """Adds nan to each possible group and a last group only with nan if the max_n_mod is not reached by the combination"""
 
     # iterating over each combination
     nan_combinations = []
     for combination in combinations:
         # adding nan to each group of the combination
         nan_combination = []
@@ -772,15 +773,15 @@
             nan_combination += [new_combination + [[str_nan]]]
 
         nan_combinations += nan_combination
 
     return nan_combinations
 
 
-def order_apply_combination(order: GroupedList, combination: List[List[Any]]) -> GroupedList:
+def order_apply_combination(order: GroupedList, combination: list[list[Any]]) -> GroupedList:
     """Converts a list of combination to a GroupedList"""
 
     order_copy = GroupedList(order)
     for combi in combination:
         order_copy.group_list(combi, combi[0])
 
     return order_copy
@@ -794,28 +795,28 @@
     xtab : DataFrame
         Crosstab
     order : GroupedList
         Combination of index to apply to the crosstab
 
     Returns
     -------
-    Dict[str, Any]
+    dict[str, Any]
         _description_
     """
     # checking for input values
     combi_xtab = None
     if xtab is not None:
         # grouping modalities in the crosstab
         groups = list(map(order.get_group, xtab.index))
         combi_xtab = xtab.groupby(groups, dropna=False, sort=False).sum()
 
     return combi_xtab
 
 
-def plot_stats(stats: DataFrame) -> Tuple[Figure, Axes]:
+def plot_stats(stats: DataFrame) -> tuple[Figure, Axes]:
     """Barplot of the volume and target rate"""
 
     x = [0] + [elt for e in stats["frequency"].cumsum()[:-1] for elt in [e] * 2] + [1]
     y2 = [elt for e in list(stats["target_rate"]) for elt in [e] * 2]
     s = list(stats.index)
     scaled_y2 = [(y - min(y2)) / (max(y2) - min(y2)) for y in y2]
     c = color_palette("coolwarm", as_cmap=True)(scaled_y2)
@@ -839,7 +840,35 @@
     ax.set_xlabel("Volume")
     ax.set_ylabel("Target rate")
     ax.set_xlim(0, 1)
     ax.set_ylim(0)
     despine()
 
     return fig, ax
+
+def load_carver(json_serialized_auto_carver: str) -> GroupedListDiscretizer:
+    """_summary_
+
+    Parameters
+    ----------
+    json_serialized_auto_carver : str
+        _description_
+
+    Returns
+    -------
+    GroupedListDiscretizer
+        _description_
+    """
+    # loading json of auto_carver
+    json_deserialized_auto_carver = loads(json_serialized_auto_carver)
+
+    # deserializing values_orders
+    values_orders = json_deserialize_values_orders(json_deserialized_auto_carver['values_orders'])
+
+    # updating auto_carver attributes
+    json_deserialized_auto_carver.update({"values_orders": values_orders})
+
+    # initiating GroupedListDiscretizer
+    auto_carver = GroupedListDiscretizer(**json_deserialized_auto_carver)
+    auto_carver.fit()
+
+    return auto_carver
```

### Comparing `AutoCarver-5.0.3/AutoCarver/converters.py` & `AutoCarver-5.0.4/AutoCarver/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.3/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.0.4/AutoCarver/discretizers/discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Tools to build simple buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
-from typing import Any, Dict, List, Union
+from typing import Union
 from numpy import nan
 from pandas import DataFrame, Series, unique
 
 from .utils.base_discretizers import (
-    GroupedList,
     GroupedListDiscretizer,
     check_new_values,
     min_value_counts,
 )
 from .utils.qualitative_discretizers import DefaultDiscretizer, OrdinalDiscretizer
 from .utils.quantitative_discretizers import QuantileDiscretizer
 from .utils.type_discretizers import StringDiscretizer
 
+from .utils.grouped_list import GroupedList
 
 class Discretizer(GroupedListDiscretizer):
     """Automatic discretizing of continuous, categorical and categorical ordinal features.
 
     Modalities/values of features are grouped according to there respective orders:
      - [Qualitative features] order based on modality target rate.
      - [Qualitative ordinal features] user-specified order.
```

### Comparing `AutoCarver-5.0.3/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.0.4/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Base tools to build simple buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
-from typing import Any, Dict, List, Union
+from typing import Any, Union
 
 from json import dumps
-from numpy import array, inf, isfinite, nan, ndarray, select, sort, floating, integer
+from numpy import array, inf, isfinite, nan, select, floating, integer
 from pandas import DataFrame, Series, isna, notna, unique
 from sklearn.base import BaseEstimator, TransformerMixin
 
+from .serialization import json_serialize_values_orders
+from .grouped_list import GroupedList
 
 def nan_unique(x: Series) -> list[Any]:
     """Unique non-NaN values.
 
     Parameters
     ----------
     x : Series
@@ -115,345 +117,16 @@
     for feature in features:
         unexpected = [val for val in known_values[feature] if val not in uniques[feature]]
         assert (
             len(unexpected) == 0
         ), f"Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was provided but there are not matching value in provided X. You should check 'values_orders['{feature}']' for unwanted values."
 
 
-class GroupedList(list):
-    """An ordered list that's extended with a dict."""
 
-    def __init__(self, iterable: Union[ndarray, dict, list, tuple] = (), order: list[Any] = None, content: dict[str, list[Any]] = None) -> None:
-        """An ordered list that historizes its elements' content.
-
-        Parameters
-        ----------
-        iterable : Union[ndarray, dict, list, tuple], optional
-            List-like or GroupedList, by default ()
-        order : list[Any], optional
-            Used when loading .json, ordering of values, by default None
-        content : dict[str, list[Any]], optional
-            Used when loading .json, (learned) content per value, by default None
-        """
-
-        # initiating iterable from order and content # TODO: move list to an attribute?
-        if order is not None and content is not None:
-            iterable = {group: content[group] for group in order}
-
-        # case -1: iterable is an array
-        if isinstance(iterable, ndarray):
-            iterable = list(iterable)
-
-        # case 0: iterable is the content dict
-        if isinstance(iterable, dict):
-            # storing ordered keys of the dict
-            keys = list(iterable)
-
-            # storing the values content per key
-            self.content = dict(iterable.items())
-
-            # checking that all values are only present once
-            all_values = [val for _, values in iterable.items() for val in values]
-            assert len(list(set(all_values))) == len(
-                all_values
-            ), "A value is present in several keys (groups)"
-
-            # adding key to itself if it's not present in an other key
-            keys_copy = keys[:]  # copying initial keys
-            for key in keys_copy:
-                # checking that the value is not comprised in an other key
-                all_values = [
-                    val
-                    for iter_key, values in iterable.items()
-                    for val in values
-                    if key != iter_key
-                ]
-                if key not in all_values:
-                    # checking that key is missing from its values
-                    if key not in iterable[key]:
-                        self.content.update({key: self.content[key] + [key]})
-                # the key already is in another key (and its values are empty)
-                # the key as already been grouped
-                else:
-                    self.content.pop(key)
-                    keys.remove(key)
-
-            # initiating the list with those keys
-            super().__init__(keys)
-
-        # case 1: copying a GroupedList
-        elif hasattr(iterable, "content"):
-            # initiating the list with the provided list of keys
-            super().__init__(iterable)
-
-            # copying values associated to keys
-            self.content = dict(iterable.content.items())
-
-        # case 2: initiating GroupedList from a list
-        elif isinstance(iterable, list):
-            # initiating the list with the provided list of keys
-            super().__init__(iterable)
-
-            # initiating the values with the provided list of keys
-            self.content = {v: [v] for v in iterable}
-
-    def get(self, key: Any) -> list[Any]:
-        """List of values content in key
-
-        Parameters
-        ----------
-        key : Any
-            Group.
-
-        Returns
-        -------
-        list[Any]
-            Values content in key
-        """
-
-        # default to fing an element
-        found = self.content.get(key)
-
-        return found
-
-    def group(self, discarded: Any, kept: Any) -> None:
-        """Groups the discarded value with the kept value
-
-        Parameters
-        ----------
-        discarded : Any
-            Value to be grouped into the key `to_keep`.
-        kept : Any
-            Key value in which to group `discarded`.
-        """
-
-        # checking that those values are distinct
-        if not is_equal(discarded, kept):
-            # checking that those values exist in the list
-            assert discarded in self, f"{discarded} not in list"
-            assert kept in self, f"{kept} not in list"
-
-            # accessing values content in each value
-            content_discarded = self.content.get(discarded)
-            content_kept = self.content.get(kept)
-
-            # updating content dict
-            self.content.update({kept: content_discarded + content_kept, discarded: []})
-
-            # removing discarded from the list
-            self.remove(discarded)
-
-    def group_list(self, to_discard: list[Any], to_keep: Any) -> None:
-        """Groups elements to_discard into values to_keep
-
-        Parameters
-        ----------
-        to_discard : list[Any]
-            Values to be grouped into the key `to_keep`.
-        to_keep : Any
-            Key value in which to group `to_discard` values.
-        """
-
-        for discarded, kept in zip(to_discard, [to_keep] * len(to_discard)):
-            self.group(discarded, kept)
-
-    def append(self, new_value: Any) -> None:
-        """Appends a new_value to the GroupedList
-
-        Parameters
-        ----------
-        new_value : Any
-            New key to be added.
-        """
-
-        self += [new_value]
-        self.content.update({new_value: [new_value]})
-
-    def update(self, new_value: Dict[Any, list[Any]]) -> None:  # TODO: not working as expected
-        """Updates the GroupedList via a dict
-
-        Parameters
-        ----------
-        new_value : Dict[Any, list[Any]]
-            Dict of key, values to updated `content` dict
-        """
-
-        # adding keys to the order if they are new values
-        self += [key for key, _ in new_value.items() if key not in self]
-
-        # updating content according to new_value
-        self.content.update(new_value)
-
-    def sort(self):
-        """Sorts the values of the list and dict (if any, NaNs are last).
-
-        Returns
-        -------
-        GroupedList
-            Sorted GroupedList
-        """
-        # str values
-        keys_str = [key for key in self if isinstance(key, str)]
-
-        # non-str values
-        keys_float = [key for key in self if not isinstance(key, str)]
-
-        # sorting and merging keys
-        keys = list(sort(keys_str)) + list(sort(keys_float))
-
-        # recreating an ordered GroupedList
-        sorted = GroupedList({k: self.get(k) for k in keys})
-
-        return sorted
-
-    def sort_by(self, ordering: list[Any]) -> None:
-        """Sorts the values of the list and dict according to `ordering`, if any, NaNs are the last.
-
-        Parameters
-        ----------
-        ordering : list[Any]
-            Order used for ordering of the list of keys.
-
-        Returns
-        -------
-        GroupedList
-            Sorted GroupedList
-        """
-
-        # checking that all values are given an order
-        assert all(
-            o in self for o in ordering
-        ), f"Unknown values in ordering: {str([v for v in ordering if v not in self])}"
-        assert all(
-            s in ordering for s in self
-        ), f"Missing value from ordering: {str([v for v in self if v not in ordering])}"
-
-        # ordering the content
-        sorted = GroupedList({k: self.get(k) for k in ordering})
-
-        return sorted
-
-    def remove(self, value: Any) -> None:
-        """Removes a value from the GroupedList
-
-        Parameters
-        ----------
-        value : Any
-            value to be removed
-        """
-        super().remove(value)
-        self.content.pop(value)
-
-    def pop(self, idx: int) -> None:
-        """Pop a value from the GroupedList by index
-
-        Parameters
-        ----------
-        idx : int
-            Index of the value to be popped out
-        """
-        value = self[idx]
-        self.remove(value)
-
-    def get_group(self, value: Any) -> Any:
-        """Returns the key (group) containing the specified value
-
-        Parameters
-        ----------
-        value : Any
-            Value for which to find the group.
-
-        Returns
-        -------
-        Any
-            Corresponding key (group)
-        """
-
-        found = [
-            key
-            for key, values in self.content.items()
-            if any(is_equal(value, elt) for elt in values)
-        ]
-
-        if any(found):
-            return found[0]
-
-        return value
-
-    def values(self) -> list[Any]:
-        """All values content in all groups
-
-        Returns
-        -------
-        list[Any]
-            List of all values in the GroupedList
-        """
-
-        known = [value for values in self.content.values() for value in values]
-
-        return known
-
-    def contains(self, value: Any) -> bool:
-        """Checks if a value is content in any group, also matches NaNs.
-
-        Parameters
-        ----------
-        value : Any
-            Value to search for
-
-        Returns
-        -------
-        bool
-            Whether the value is in the GroupedList
-        """
-
-        known_values = self.values()
-
-        return any(is_equal(value, known) for known in known_values)
-
-    def get_repr(self, char_limit: int = 6) -> list[str]:
-        """Returns a representative list of strings of values of groups.
-
-        Parameters
-        ----------
-        char_limit : int, optional
-            Maximum number of character per string, by default 6
-
-        Returns
-        -------
-        list[str]
-            List of short str representation of the keys' values
-        """
-
-        # initiating list of group representation
-        repr: list[str] = []
-
-        # iterating over each group
-        for group in self:
-            # accessing group's values
-            values = self.get(group)
-
-            if len(values) == 0:  # case 0: there are no value in this group
-                pass
-
-            elif len(values) == 1:  # case 1: there is only one value in this group
-                repr += [values[0]]
-
-            elif len(values) == 2:  # case 2: two values in this group
-                repr += [f"{values[1]}"[:char_limit] + " and " + f"{values[0]}"[:char_limit]]
-
-            elif len(values) > 2:  # case 3: more than two values in this group
-                repr += [f"{values[-1]}"[:char_limit] + " to " + f"{values[0]}"[:char_limit]]
-
-        return repr
-
-
-# TODO: add a summary
 # TODO: output a json
-# TODO: add a base discretizer that implements prepare_data (add reset_index ? -> add duplicate column check)
 class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
     """Discretizer that uses a dict of grouped values."""
 
     def __init__(
         self,
         features: list[str],
         *,
@@ -620,21 +293,21 @@
             assert (0 in y_values) & (
                 1 in y_values
             ), "y must be a binary Series (int or float, not object)"
             assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
 
         return x_copy
 
-    def fit(self, X: DataFrame, y: Series = None) -> None:
+    def fit(self, X: DataFrame = None, y: Series = None) -> None:
         """Learns the labels associated to each value for each feature
 
         Parameters
         ----------
         X : DataFrame
-            Contains columns named after `features` attribute
+            Contains columns named after `features` attribute, by default None
         y : Series, optional
             Model target, by default None
         """
         # checking that all features to discretize are in values_orders
         missing_features = [feature for feature in self.features if feature not in self.values_orders]
         assert len(missing_features) == 0, f"Missing values_orders for following features {str(missing_features)}."
 
@@ -772,32 +445,36 @@
     
     def to_json(self) ->  str:
         """Converts the GroupedListDiscretizer's values_orders to .json
 
         Returns
         -------
         str
-            _description_
+            JSON serialized GroupedListDiscretizer
         """
         # extracting content dictionnaries
-        content = {
+        json_serialized_groupedlistdiscretizer = {
             "features": self.features,
-            "values_ordres": self.values_orders,  # TODO: adapt maybe init GroupedList with {"values": values, "content": values.content} ?
+            "values_orders": json_serialize_values_orders(self.values_orders),
             "input_dtypes": self.input_dtypes,
             "output_dtype": self.output_dtype,
             "str_nan": self.str_nan,
+            "str_default": self.str_default,
+            "dropna": self.dropna,
             "copy": self.copy,
         }
-        # content_orders = {feature: {"values": values, "content": values.content} for feature, values in self.values_orders.items()}
+
         # dumping as json
-        return dumps(content)
+        return dumps(json_serialized_groupedlistdiscretizer)
     
     def summary(self) -> DataFrame:
         """Summarizes the data bucketization
 
+        TODO: add crosstabs per feature for a provided X?
+
         Returns
         -------
         DataFrame
             A summary of feature's values
         """
         # raw label per value with output_dtype 'str'
         raw_labels_per_values = self.get_labels_per_values(output_dtype='str')
@@ -808,16 +485,16 @@
             # adding each value/label 
             for value, label in self.labels_per_values[feature].items():
                 # initiating feature summary (default value/label)
                 feature_summary = {'feature': feature, 'dtype': self.input_dtypes[feature], 'label': label, 'content': value}
 
                 # case 0: qualitative feature -> not adding floats and integers str_default
                 if feature in self.qualitative_features:
-                    if not isinstance(value, floating):  # checking for floats
-                        if not isinstance(value, integer):  # checking for ints
+                    if not isinstance(value, floating) and not isinstance(value, float):  # checking for floats
+                        if not isinstance(value, integer) and not isinstance(value, int):  # checking for ints
                             if value != self.str_default:  # checking for str_default
                                 summaries += [feature_summary]
 
                 # case 1: quantitative feature -> take the raw label per value
                 elif feature in self.quantitative_features:
                     feature_summary.update({'content': raw_labels_per_values[feature][value]})
                     summaries += [feature_summary]
@@ -829,17 +506,23 @@
             # if there are nans -> if already added it will be dropped afterwards (unique content)
             if self.str_nan in raw_labels_per_values[feature]:
                 nan_group = self.values_orders[feature].get_group(self.str_nan)
                 feature_summary.update({'label': self.labels_per_values[feature][nan_group], 'content': self.str_nan})
                 summaries += [feature_summary]
 
         # aggregating unique values per label
-        summaries = DataFrame(summaries).groupby(['feature', 'dtype', 'label'])['content'].apply(lambda u: list(unique(u)))
+        summaries = DataFrame(summaries).groupby(['feature', 'dtype', 'label'])['content'].apply(lambda u: list(unique(u))).reset_index()
+        # sorting content
+        sorted_contents: list[list[Any]] = []
+        for content in summaries['content']:
+            content.sort(key=repr)
+            sorted_contents += [content]
+        summaries['content'] = sorted_contents
         # sorting and seting index
-        summaries = summaries.reset_index().sort_values(['dtype', 'feature']).set_index(['feature', 'dtype'])
+        summaries = summaries.sort_values(['dtype', 'feature']).set_index(['feature', 'dtype'])
 
         return summaries
 
 
 def convert_to_labels(
     features: list[str],
     quantitative_features: list[str],
@@ -1039,40 +722,14 @@
     if dropna:
         if any(isna(uniques)):
             n -= 1
 
     return n
 
 
-def is_equal(a: Any, b: Any) -> bool:
-    """Checks if a and b are equal (NaN insensitive)
-
-    Parameters
-    ----------
-    a : Any
-        _description_
-    b : Any
-        _description_
-
-    Returns
-    -------
-    bool
-        _description_
-    """
-
-    # default equality
-    equal = a == b
-
-    # Case where a and b are NaNs
-    if isna(a) and isna(b):
-        equal = True
-
-    return equal
-
-
 def get_labels(quantiles: list[float], str_nan: str) -> list[str]:
     """_summary_
 
     Parameters
     ----------
     feature : str
         _description_
```

### Comparing `AutoCarver-5.0.3/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.0.4/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from typing import Any, Dict, List, Union
 from AutoCarver.discretizers.utils.base_discretizers import GroupedList
 
 from numpy import argmin, nan, select
 from pandas import DataFrame, Series, isna, notna, unique
 
+from .grouped_list import GroupedList
 from .base_discretizers import (
-    GroupedList,
     GroupedListDiscretizer,
     check_missing_values,
     check_new_values,
     convert_to_labels,
     convert_to_values,
     nan_unique,
     target_rate,
```

### Comparing `AutoCarver-5.0.3/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.0.4/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 
 from typing import Any, Dict, List
 
 from numpy import array, inf, linspace, nan, quantile
 from pandas import DataFrame, Series, isna, notna
 
-from .base_discretizers import GroupedList, GroupedListDiscretizer, applied_to_dict_list
+from .base_discretizers import GroupedListDiscretizer, applied_to_dict_list
+from .grouped_list import GroupedList
 
 
 class QuantileDiscretizer(GroupedListDiscretizer):
     """Builds per-feature buckets of quantiles"""
 
     def __init__(
         self,
```

### Comparing `AutoCarver-5.0.3/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.0.4/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Base tools to convert values into specific types.
 """
 
 from pandas import DataFrame, Series
 
-from .base_discretizers import GroupedList, GroupedListDiscretizer, nan_unique
-
+from .base_discretizers import GroupedListDiscretizer, nan_unique
+from .grouped_list import GroupedList
 
 class StringDiscretizer(GroupedListDiscretizer):
     """Converts specified columns of a DataFrame into str.
     First step of a Qualitative Discretization pipe.
 
     - Keeps NaN inplace
     - Converts floats of int to int
```

### Comparing `AutoCarver-5.0.3/AutoCarver/feature_selector.py` & `AutoCarver-5.0.4/AutoCarver/feature_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from numpy import inf, nan, ones, triu
 from pandas import DataFrame, Series, crosstab, notna
 from scipy.stats import chi2_contingency, kruskal
 from sklearn.base import BaseEstimator, TransformerMixin
 from statsmodels.formula.api import ols
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 
-from .discretizers.utils.base_discretizers import GroupedList, GroupedListDiscretizer
+from .discretizers.utils.base_discretizers import GroupedListDiscretizer
+from .discretizers.utils.grouped_list import GroupedList
 
 # TODO: convert to groupedlistdiscretizer
 # TODO: add parameter to shut down displayed info
 class FeatureSelector(BaseEstimator, TransformerMixin):
     """A pipeline of measures to perform EDA and feature pre-selection
 
      - best features are the n_best of each measure
```

### Comparing `AutoCarver-5.0.3/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.4/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.3
+Version: 5.0.4
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.0.3/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.0.4/AutoCarver.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 AutoCarver.egg-info/SOURCES.txt
 AutoCarver.egg-info/dependency_links.txt
 AutoCarver.egg-info/top_level.txt
 AutoCarver/discretizers/__init__.py
 AutoCarver/discretizers/discretizers.py
 AutoCarver/discretizers/utils/__init__.py
 AutoCarver/discretizers/utils/base_discretizers.py
+AutoCarver/discretizers/utils/grouped_list.py
 AutoCarver/discretizers/utils/qualitative_discretizers.py
 AutoCarver/discretizers/utils/quantitative_discretizers.py
+AutoCarver/discretizers/utils/serialization.py
 AutoCarver/discretizers/utils/type_discretizers.py
 tests/test_auto_carver.py
 tests/test_base_discretizers.py
 tests/test_converters.py
 tests/test_discretizers.py
 tests/test_feature_selector.py
 tests/test_qualitative_discretizers.py
```

### Comparing `AutoCarver-5.0.3/LICENSE` & `AutoCarver-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.3/PKG-INFO` & `AutoCarver-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.3
+Version: 5.0.4
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.0.3/README.md` & `AutoCarver-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.3/setup.py` & `AutoCarver-5.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.3",
+    version="5.0.4",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.0.3/tests/test_auto_carver.py` & `AutoCarver-5.0.4/tests/test_auto_carver.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,13 +70,19 @@
         assert all(value in fitted_values for value in init_values), f"Missing value in output! Some values are been dropped for qualitative feature: {feature}"
     
     # testing output of nans
     if not dropna:
         assert all(x_train[auto_carver.features].isna().mean()  == x_discretized[auto_carver.features].isna().mean()), "Some Nans are being dropped (grouped) or more nans than expected"
     else:
         assert all(x_discretized[auto_carver.features].isna().mean() == 0), "Some Nans are not dropped (grouped)"
+    
+    # testing json serialization
+    json_serialized_auto_carver = auto_carver.to_json()
+    loaded_carver = load_carver(json_serialized_auto_carver)
+
+    assert all(loaded_carver.summary() == auto_carver.summary()), "Non-identical AutoCarver when loading JSON"
 
 # def test_auto_carver_copy(x_train: DataFrame, x_test_1: DataFrame, output_dtype: str, dropna: bool, sort_by: str) -> None:
 
     # TODO test missing values in test
     # TODO try with copy = False
-    # TODO: test avec chained_discretizer
+    # TODO: test avec chained_discretizer
```

### Comparing `AutoCarver-5.0.3/tests/test_base_discretizers.py` & `AutoCarver-5.0.4/tests/test_base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.3/tests/test_discretizers.py` & `AutoCarver-5.0.4/tests/test_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.3/tests/test_qualitative_discretizers.py` & `AutoCarver-5.0.4/tests/test_qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.3/tests/test_quantitative_discretizers.py` & `AutoCarver-5.0.4/tests/test_quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.3/tests/test_type_discretizers.py` & `AutoCarver-5.0.4/tests/test_type_discretizers.py`

 * *Files identical despite different names*

