# Comparing `tmp/statsplotly-0.0.0.tar.gz` & `tmp/statsplotly-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsplotly-0.0.0.tar", max compression
+gzip compressed data, was "statsplotly-0.1.2.tar", max compression
```

## Comparing `statsplotly-0.0.0.tar` & `statsplotly-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1519 2023-07-14 23:42:41.942165 statsplotly-0.0.0/LICENSE
--rw-r--r--   0        0        0     2548 2023-07-14 23:42:41.942165 statsplotly-0.0.0/README.md
--rw-r--r--   0        0        0     2545 2023-07-14 23:42:41.978165 statsplotly-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      225 2023-07-14 23:42:42.046165 statsplotly-0.0.0/statsplotly/__init__.py
--rw-r--r--   0        0        0     3680 2023-07-14 23:42:42.046165 statsplotly-0.0.0/statsplotly/constants.py
--rw-r--r--   0        0        0      713 2023-07-14 23:42:42.046165 statsplotly-0.0.0/statsplotly/exceptions.py
--rw-r--r--   0        0        0      111 2023-07-14 23:42:42.046165 statsplotly-0.0.0/statsplotly/plot_objects/__init__.py
--rw-r--r--   0        0        0     8506 2023-07-14 23:42:42.046165 statsplotly-0.0.0/statsplotly/plot_objects/layout_objects.py
--rw-r--r--   0        0        0    26618 2023-07-14 23:42:42.046165 statsplotly-0.0.0/statsplotly/plot_objects/trace_objects.py
--rw-r--r--   0        0        0       92 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/plot_specifiers/__init__.py
--rw-r--r--   0        0        0     5140 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/plot_specifiers/color.py
--rw-r--r--   0        0        0    23879 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/plot_specifiers/data.py
--rw-r--r--   0        0        0     8326 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/plot_specifiers/layout.py
--rw-r--r--   0        0        0    12126 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/plot_specifiers/trace.py
--rw-r--r--   0        0        0        0 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/plotting/__init__.py
--rw-r--r--   0        0        0     5860 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/plotting/helpers.py
--rw-r--r--   0        0        0    58341 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/plotting/main.py
--rw-r--r--   0        0        0        0 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/utils/__init__.py
--rw-r--r--   0        0        0     6986 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/utils/colors_utils.py
--rw-r--r--   0        0        0     6421 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/utils/figure_utils.py
--rw-r--r--   0        0        0     5623 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/utils/layout_utils.py
--rw-r--r--   0        0        0     4825 2023-07-14 23:42:42.050165 statsplotly-0.0.0/statsplotly/utils/stats_utils.py
--rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 statsplotly-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-07-14 16:56:05.097446 statsplotly-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2518 2023-07-14 16:56:05.099830 statsplotly-0.1.2/README.md
+-rw-r--r--   0        0        0     2519 2023-07-14 17:55:31.227261 statsplotly-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-07-14 16:56:05.807800 statsplotly-0.1.2/statsplotly/__init__.py
+-rw-r--r--   0        0        0     3680 2023-07-14 16:56:05.808906 statsplotly-0.1.2/statsplotly/constants.py
+-rw-r--r--   0        0        0      713 2023-07-14 16:56:05.810028 statsplotly-0.1.2/statsplotly/exceptions.py
+-rw-r--r--   0        0        0      111 2023-07-14 16:56:05.811271 statsplotly-0.1.2/statsplotly/plot_objects/__init__.py
+-rw-r--r--   0        0        0     8503 2023-07-14 16:56:05.812795 statsplotly-0.1.2/statsplotly/plot_objects/layout_objects.py
+-rw-r--r--   0        0        0    26615 2023-07-14 16:56:05.815166 statsplotly-0.1.2/statsplotly/plot_objects/trace_objects.py
+-rw-r--r--   0        0        0       92 2023-07-14 16:56:05.819046 statsplotly-0.1.2/statsplotly/plot_specifiers/__init__.py
+-rw-r--r--   0        0        0     5140 2023-07-14 16:56:05.821339 statsplotly-0.1.2/statsplotly/plot_specifiers/color.py
+-rw-r--r--   0        0        0    23879 2023-07-14 16:56:05.823592 statsplotly-0.1.2/statsplotly/plot_specifiers/data.py
+-rw-r--r--   0        0        0     8326 2023-07-14 16:56:05.825020 statsplotly-0.1.2/statsplotly/plot_specifiers/layout.py
+-rw-r--r--   0        0        0    12126 2023-07-14 16:56:05.826648 statsplotly-0.1.2/statsplotly/plot_specifiers/trace.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:56:05.827034 statsplotly-0.1.2/statsplotly/plotting/__init__.py
+-rw-r--r--   0        0        0     5860 2023-07-14 16:56:05.829730 statsplotly-0.1.2/statsplotly/plotting/helpers.py
+-rw-r--r--   0        0        0    58341 2023-07-14 16:56:05.831369 statsplotly-0.1.2/statsplotly/plotting/main.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:56:05.831712 statsplotly-0.1.2/statsplotly/utils/__init__.py
+-rw-r--r--   0        0        0     6986 2023-07-14 16:56:05.832967 statsplotly-0.1.2/statsplotly/utils/colors_utils.py
+-rw-r--r--   0        0        0     6421 2023-07-14 16:56:05.834825 statsplotly-0.1.2/statsplotly/utils/figure_utils.py
+-rw-r--r--   0        0        0     5623 2023-07-14 16:56:05.836062 statsplotly-0.1.2/statsplotly/utils/layout_utils.py
+-rw-r--r--   0        0        0     4825 2023-07-14 16:56:05.837014 statsplotly-0.1.2/statsplotly/utils/stats_utils.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 statsplotly-0.1.2/PKG-INFO
```

### Comparing `statsplotly-0.0.0/LICENSE` & `statsplotly-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/README.md` & `statsplotly-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,31 +10,26 @@
 - processes color coding scheme, trace slicer and plot dimensions independently.
 - can perform standard statistical processing procedure (e.g., zscore normalization) of data under the hood.
 - leverages the tidy DataFrame structure to easily style plot cues to be used as visual discriminators (e.g., marker color, symbol, size, and opacity).
 
 
 This flexibility takes advantage of the powerful interactivity offered by `plotly.js` without compromising statistical intelligibility for aesthetic choices, or vice-versa.
 
+![statsplotly-demo](statsplotly-demo.gif)
+
 Examples
 -
 Main features of the API are demonstrated in a demo [notebook](https://nbviewer.org/github/parici75/statsplotly/blob/main/docs/notebooks/statsplotly_demo.ipynb).
 
-![statsplotly-demo](statsplotly-demo.gif)
-
-
 Installation
 -
 ### Using Pip
 
 `pip install statsplotly`
 
-Documentation
--
-Details of the public API can be found in the [documentation](https://parici75.github.io/statsplotly).
-
 
 Development
 -
 ### Using Poetry
 First make sure you have Poetry installed on your system (see [instruction](https://python-poetry.org/docs/#installing-with-the-official-installer)).
 
 Then, assuming you have a Unix shell with make, create and set up a new Poetry environment :
@@ -52,16 +47,20 @@
 The Makefile provides several targets to assist in development and code quality :
 - `init` creates a project-specific virtual environment and installs the dependencies of the .lock file.
 - `ci` launches Black, Ruff, mypy and pytest on your source code.
 - `pre-commit` set up pre-commit hooks (see pre-commit [documentation](https://pre-commit.com/)).
 - `clean` clears bytecode, poetry/pip caches. Use with caution.
 
 
+Documentation
+-
+Details of the public API can be found in the [documentation](https://parici75.github.io/statsplotly).
+
+
 Requirements
 -
 - [Plotly](https://plotly.com/python/)
-- [SciPy](https://scipy.org/)
 
 
 Author
 -
 [Benjamin Roland](benjamin.roland@hotmail.fr)
```

### Comparing `statsplotly-0.0.0/pyproject.toml` & `statsplotly-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 authors = ["Benjamin Roland <benjamin.roland@hotmail.fr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/parici75/statsplotly"
 documentation = "https://parici75.github.io/statsplotly/"
 
 [tool.poetry.dependencies]
-python = ">=3.11, <3.13"
+python = "^3.11"
 pydantic = "^2.0"
 seaborn = "^0.12.2"
-scipy = "^1.11.1"
 plotly = "^5.15.0"
 ipykernel = "^6.24.0"
 jupyter = "^1.0.0"
 poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.25.0"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
```

### Comparing `statsplotly-0.0.0/statsplotly/constants.py` & `statsplotly-0.1.2/statsplotly/constants.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/exceptions.py` & `statsplotly-0.1.2/statsplotly/exceptions.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/plot_objects/layout_objects.py` & `statsplotly-0.1.2/statsplotly/plot_objects/layout_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import logging
 from typing import Any
 
 from pydantic import FieldValidationInfo, field_validator, model_validator
-from pydantic.v1.utils import deep_update
+from pydantic.utils import deep_update
 
 from statsplotly.constants import AXIS_TITLEFONT, DEFAULT_HOVERMODE, TICKFONT
 from statsplotly.exceptions import StatsPlotInvalidArgumentError
 from statsplotly.plot_specifiers.data import BaseModel
 from statsplotly.plot_specifiers.layout import AxesSpecifier, BarMode
 
 logger = logging.getLogger(__name__)
```

### Comparing `statsplotly-0.0.0/statsplotly/plot_objects/trace_objects.py` & `statsplotly-0.1.2/statsplotly/plot_objects/trace_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from abc import ABCMeta, abstractmethod
 from typing import Any
 
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
-from pydantic.v1.utils import deep_update
+from pydantic.utils import deep_update
 
 from statsplotly import constants
 from statsplotly.plot_specifiers.color import ColorSpecifier
 from statsplotly.plot_specifiers.data import (
     TRACE_DIMENSION_MAP,
     AggregationTraceData,
     BaseModel,
```

### Comparing `statsplotly-0.0.0/statsplotly/plot_specifiers/color.py` & `statsplotly-0.1.2/statsplotly/plot_specifiers/color.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/plot_specifiers/data.py` & `statsplotly-0.1.2/statsplotly/plot_specifiers/data.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/plot_specifiers/layout.py` & `statsplotly-0.1.2/statsplotly/plot_specifiers/layout.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/plot_specifiers/trace.py` & `statsplotly-0.1.2/statsplotly/plot_specifiers/trace.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/plotting/helpers.py` & `statsplotly-0.1.2/statsplotly/plotting/helpers.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/plotting/main.py` & `statsplotly-0.1.2/statsplotly/plotting/main.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/utils/colors_utils.py` & `statsplotly-0.1.2/statsplotly/utils/colors_utils.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/utils/figure_utils.py` & `statsplotly-0.1.2/statsplotly/utils/figure_utils.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/utils/layout_utils.py` & `statsplotly-0.1.2/statsplotly/utils/layout_utils.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/statsplotly/utils/stats_utils.py` & `statsplotly-0.1.2/statsplotly/utils/stats_utils.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.0.0/PKG-INFO` & `statsplotly-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: statsplotly
-Version: 0.0.0
+Version: 0.1.2
 Summary: Tidy API for statistical visualization with Plotly
 Home-page: https://github.com/parici75/statsplotly
 License: BSD-3-Clause
 Author: Benjamin Roland
 Author-email: benjamin.roland@hotmail.fr
-Requires-Python: >=3.11,<3.13
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipykernel (>=6.24.0,<7.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: poetry-dynamic-versioning[plugin] (>=0.25.0,<0.26.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
-Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Project-URL: Documentation, https://parici75.github.io/statsplotly/
 Description-Content-Type: text/markdown
 
 [Statsplotly](https://github.com/parici75/statsplotly) is a Python data visualization library based on Plotly. It provides a high-level interface for drawing attractive and interactive statistical data visualization plots.
 
 The inception of this library predated the fantastic [plotly.express](https://plotly.com/python/plotly-express/) API.
@@ -32,31 +31,26 @@
 - processes color coding scheme, trace slicer and plot dimensions independently.
 - can perform standard statistical processing procedure (e.g., zscore normalization) of data under the hood.
 - leverages the tidy DataFrame structure to easily style plot cues to be used as visual discriminators (e.g., marker color, symbol, size, and opacity).
 
 
 This flexibility takes advantage of the powerful interactivity offered by `plotly.js` without compromising statistical intelligibility for aesthetic choices, or vice-versa.
 
+![statsplotly-demo](statsplotly-demo.gif)
+
 Examples
 -
 Main features of the API are demonstrated in a demo [notebook](https://nbviewer.org/github/parici75/statsplotly/blob/main/docs/notebooks/statsplotly_demo.ipynb).
 
-![statsplotly-demo](statsplotly-demo.gif)
-
-
 Installation
 -
 ### Using Pip
 
 `pip install statsplotly`
 
-Documentation
--
-Details of the public API can be found in the [documentation](https://parici75.github.io/statsplotly).
-
 
 Development
 -
 ### Using Poetry
 First make sure you have Poetry installed on your system (see [instruction](https://python-poetry.org/docs/#installing-with-the-official-installer)).
 
 Then, assuming you have a Unix shell with make, create and set up a new Poetry environment :
@@ -74,17 +68,21 @@
 The Makefile provides several targets to assist in development and code quality :
 - `init` creates a project-specific virtual environment and installs the dependencies of the .lock file.
 - `ci` launches Black, Ruff, mypy and pytest on your source code.
 - `pre-commit` set up pre-commit hooks (see pre-commit [documentation](https://pre-commit.com/)).
 - `clean` clears bytecode, poetry/pip caches. Use with caution.
 
 
+Documentation
+-
+Details of the public API can be found in the [documentation](https://parici75.github.io/statsplotly).
+
+
 Requirements
 -
 - [Plotly](https://plotly.com/python/)
-- [SciPy](https://scipy.org/)
 
 
 Author
 -
 [Benjamin Roland](benjamin.roland@hotmail.fr)
```

