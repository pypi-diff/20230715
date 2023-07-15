# Comparing `tmp/psychoanalyze-0.5.0.tar.gz` & `tmp/psychoanalyze-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.5.0.tar", max compression
+gzip compressed data, was "psychoanalyze-0.6.0.tar", max compression
```

## Comparing `psychoanalyze-0.5.0.tar` & `psychoanalyze-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-14 03:05:50.334003 psychoanalyze-0.5.0/LICENSE
--rw-r--r--   0        0        0     1105 2023-07-14 03:05:50.334003 psychoanalyze-0.5.0/README.md
--rw-r--r--   0        0        0     1357 2023-07-14 03:07:52.912887 psychoanalyze-0.5.0/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1639 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     8559 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     8048 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5256 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     2938 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1589 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     1963 2023-07-14 03:07:52.912887 psychoanalyze-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 psychoanalyze-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-15 09:39:04.526433 psychoanalyze-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1105 2023-07-15 09:39:04.526433 psychoanalyze-0.6.0/README.md
+-rw-r--r--   0        0        0     1357 2023-07-15 09:41:16.677281 psychoanalyze-0.6.0/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1153 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     8080 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     7763 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5206 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     2938 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1589 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     1881 2023-07-15 09:41:16.677281 psychoanalyze-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 psychoanalyze-0.6.0/PKG-INFO
```

### Comparing `psychoanalyze-0.5.0/LICENSE` & `psychoanalyze-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/README.md` & `psychoanalyze-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/__init__.py` & `psychoanalyze-0.6.0/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.6.0/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.6.0/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.6.0/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.6.0/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.6.0/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/data/__init__.py` & `psychoanalyze-0.6.0/psychoanalyze/data/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,37 +10,16 @@
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Data modules and general-purpose data transformation utilities.
 
-Functions:
-
-- [`psychoanalyze.data.load`][psychoanalyze.data.load]
-
 Submodules:
 
 - [`psychoanalyze.data.blocks`][psychoanalyze.data.blocks]
 - [`psychoanalyze.data.points`][psychoanalyze.data.points]
 - [`psychoanalyze.data.trials`][psychoanalyze.data.trials]
 - [`psychoanalyze.data.sessions`][psychoanalyze.data.sessions]
 - [`psychoanalyze.data.subjects`][psychoanalyze.data.subjects]
 - [`psychoanalyze.data.types`][psychoanalyze.data.types]
 """
-from pathlib import Path
-
-import pandas as pd
-
-from psychoanalyze.data import blocks, points, sessions, subjects
-
-
-def load(
-    data_dir: Path = Path("data"),
-) -> dict[str, pd.DataFrame]:
-    """Load all tables into dict."""
-    return {
-        "Sessions": sessions.load(data_dir),
-        "Subjects": subjects.load(data_dir),
-        "Blocks": blocks.load(data_dir),
-        "Points": points.load(data_dir),
-    }
```

### Comparing `psychoanalyze-0.5.0/psychoanalyze/data/blocks.py` & `psychoanalyze-0.6.0/psychoanalyze/data/blocks.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 """
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
-from pandera.typing import DataFrame
 from scipy.special import expit, logit
 from scipy.stats import logistic as scipy_logistic
 from sklearn.linear_model import LogisticRegression
 
 from psychoanalyze.data import (
     points,
     sessions,
@@ -130,23 +129,14 @@
     ref_stim_cols = ["Amp2", "Width2", "Freq2", "Dur2"]
     channel_config = ["Active Channels", "Return Channels"]
     return trials.groupby(session_cols + ref_stim_cols + channel_config)[
         "Result"
     ].count()
 
 
-def experiment_type(blocks: pd.DataFrame) -> pd.Series:
-    """Determine experimental type (detection/discrimination) from data."""
-    ref_stim = blocks.reset_index()[["Amp2", "Width2", "Freq2", "Dur2"]]
-    ref_charge = ref_stim["Amp2"] * ref_stim["Width2"]
-    blocks.loc[ref_charge == 0, "Experiment Type"] = "Detection"
-    blocks.loc[ref_charge != 0, "Experiment Type"] = "Discrimination"
-    return blocks["Experiment Type"]
-
-
 def is_valid(block: pd.DataFrame) -> bool:
     """Determine if curve data is valid."""
     return any(block["Hit Rate"] > 0.5) & any(block["Hit Rate"] < 0.5)  # noqa: PLR2004
 
 
 def subject_counts(data: pd.DataFrame) -> pd.DataFrame:
     """Determine how many subjects are in the data."""
@@ -191,15 +181,15 @@
 
 
 def generate_trials(n_trials: int, model_params: dict[str, float]) -> pd.DataFrame:
     """Generate trials for block-level context."""
     return trials.moc_sample(n_trials, model_params)
 
 
-def from_points(points: DataFrame[types.Points]) -> pd.DataFrame:
+def from_points(points: pd.DataFrame) -> pd.DataFrame:
     """Aggregate block measures from points data."""
     return points.groupby("BlockID")[["n"]].sum()
 
 
 def plot_thresholds(blocks: pd.DataFrame) -> go.Figure:
     """Plot longitudinal threshold data.
 
@@ -240,21 +230,20 @@
     param_fits.index = x
     return param_fits
 
 
 def logistic(params: dict[str, float]) -> pd.DataFrame:
     """Generate logistic function from parameters."""
     x = np.linspace(
-        scipy_logistic.ppf(0.01) + params["Threshold"],
-        scipy_logistic.ppf(0.99) + params["Threshold"],
+        scipy_logistic.ppf(0.01, loc=params["x_0"], scale=params["k"]),
+        scipy_logistic.ppf(0.99, loc=params["x_0"], scale=params["k"]),
         100,
     )
-    y = params["Guess Rate"] + (
-        1 - params["Guess Rate"] - params["Lapse Rate"]
-    ) * scipy_logistic.cdf(x, params["Threshold"], params["Slope"])
+    # ) * scipy_logistic.cdf(x, params["Threshold"], params["Slope"])
+    y = scipy_logistic.cdf(x, params["x_0"], params["k"])
     index = pd.Index(x, name="Intensity")
     logistic_points = pd.Series(
         y,
         index=index,
         name="Hit Rate",
     )
     logit_hit_rate = pd.Series(
```

### Comparing `psychoanalyze-0.5.0/psychoanalyze/data/points.py` & `psychoanalyze-0.6.0/psychoanalyze/data/points.py`

 * *Files 6% similar despite different names*

```diff
@@ -208,23 +208,24 @@
 
 def to_block(points: pd.DataFrame) -> pd.DataFrame:
     """Aggregate to block-level measures from points-level data."""
     return points.groupby(level="Block").sum()
 
 
 def psi(
-    x: np.ndarray,
-    threshold: float,
-    width: float,
-    gamma: float,
-    lambda_: float,
-) -> float:
+    x: pd.Index,
+    params: dict[str, float],
+) -> pd.Series:
     """Calculate psi for an array of intensity levels x."""
-    return gamma + (1 - gamma - lambda_) / (
-        1 + np.exp(-gamma * (x - threshold) / width) ** lambda_
+    return pd.Series(
+        params["gamma"]
+        + (1 - params["gamma"] - params["lambda"])
+        / (1 + np.exp(-params["k"] * (x - params["x_0"]))),
+        index=x,
+        name="p(x)",
     )
 
 
 def plot(points: pd.DataFrame, y: str) -> go.Figure:
     """Plot the psychometric function."""
     return px.scatter(
         points.reset_index(),
@@ -241,24 +242,12 @@
 
 
 def transform(hit_rate: float, y: str) -> float:
     """Logit transform hit rate."""
     return logit(hit_rate) if y == "alpha" else hit_rate
 
 
-def plot_logistic(logistic: pd.DataFrame, y: str, name: str, color: str) -> go.Scatter:
-    """Plot a smooth logistic function."""
-    logistic = logistic.reset_index()
-    return go.Scatter(
-        x=logistic["Intensity"],
-        y=logistic[y],
-        mode="lines",
-        name=name,
-        marker_color=color,
-    )
-
-
 def generate_index(n_levels: int, x_range: list[float]) -> pd.Index:
     """Generate evenly-spaced values along the modulated stimulus dimension."""
     min_x = x_range[0]
     max_x = x_range[1]
     return pd.Index(np.linspace(min_x, max_x, n_levels), name="Intensity")
```

### Comparing `psychoanalyze-0.5.0/psychoanalyze/data/sessions.py` & `psychoanalyze-0.6.0/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.6.0/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/data/subjects.py` & `psychoanalyze-0.6.0/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/data/trials.py` & `psychoanalyze-0.6.0/psychoanalyze/data/trials.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,17 @@
 def generate(
     n_trials: int,
     options: pd.Index,
     params: dict[str, float],
 ) -> pd.DataFrame:
     """Generate n trials with outcomes."""
     x = generate_trial_index(n_trials, options)
-    p = {option: psi(option, params) for option in options}
     return pd.DataFrame(
         {
-            "Result": [int(random.random() <= p[x_val]) for x_val in x],
+            "Result": [int(random.random() <= psi(x_val, params)) for x_val in x],
             "Intensity": x,
         },
     )
 
 
 def load(data_path: Path = Path("data")) -> pd.DataFrame:
     """Load trials data from csv."""
```

### Comparing `psychoanalyze-0.5.0/psychoanalyze/data/types.py` & `psychoanalyze-0.6.0/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/plot.py` & `psychoanalyze-0.6.0/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/psychoanalyze/sigmoids.py` & `psychoanalyze-0.6.0/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.5.0/pyproject.toml` & `psychoanalyze-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.5.0"
+version = "0.6.0"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
@@ -28,17 +28,14 @@
 gunicorn = "^20.1.0"
 mypy = "^1.4.1"
 click = "^8.1.3"
 typer = {extras = ["all"], version = "^0.9.0"}
 tuna = "^0.5.11"
 ruff = "^0.0.276"
 black = "^23.3.0"
-mkdocs = "^1.4.3"
-mkdocs-material = "^9.1.18"
-mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 ipykernel = "^6.24.0"
 ipywidgets = "^8.0.7"
 kaleido = "0.2.1"
 pyarrow = "^12.0.1"
 
 [tool.poetry.scripts]
 psychoanalyze = "psychoanalyze.__main__:main"
@@ -72,15 +69,16 @@
     'plotly.express',
     'scipy.stats',
     'scipy.special',
     'sklearn.linear_model',
     'dash_daq',
     'datatest',
     'bambi',
-    'hypothesis'
+    'hypothesis',
+    'statsmodels.*',
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 fix = true
 select = ["ALL", "CPY001"]
 ignore = ["S101", "S311", "D211", "D213"]
```

### Comparing `psychoanalyze-0.5.0/PKG-INFO` & `psychoanalyze-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -18,17 +18,14 @@
 Requires-Dist: datatest (>=0.11.1,<0.12.0)
 Requires-Dist: dbt-duckdb (>=1.5.1,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: hypothesis (>=6.79.0,<7.0.0)
 Requires-Dist: ipykernel (>=6.24.0,<7.0.0)
 Requires-Dist: ipywidgets (>=8.0.7,<9.0.0)
 Requires-Dist: kaleido (==0.2.1)
-Requires-Dist: mkdocs (>=1.4.3,<2.0.0)
-Requires-Dist: mkdocs-material (>=9.1.18,<10.0.0)
-Requires-Dist: mkdocstrings[python] (>=0.22.0,<0.23.0)
 Requires-Dist: mypy (>=1.4.1,<2.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
 Requires-Dist: pandera[mypy] (>=0.15.1,<0.16.0)
 Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
```

