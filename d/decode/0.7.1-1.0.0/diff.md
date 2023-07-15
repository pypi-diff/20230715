# Comparing `tmp/decode-0.7.1.tar.gz` & `tmp/decode-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decode-0.7.1.tar", max compression
+gzip compressed data, was "decode-1.0.0.tar", max compression
```

## Comparing `decode-0.7.1.tar` & `decode-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1083 2022-10-24 01:14:16.943677 decode-0.7.1/LICENSE
--rw-r--r--   0        0        0      824 2022-10-24 01:14:16.943677 decode-0.7.1/README.md
--rw-r--r--   0        0        0      324 2022-10-24 01:14:16.943677 decode-0.7.1/decode/__init__.py
--rw-r--r--   0        0        0     9687 2022-10-24 01:14:16.943677 decode-0.7.1/decode/array.py
--rw-r--r--   0        0        0    12250 2022-10-24 01:14:16.947677 decode-0.7.1/decode/cube.py
--rw-r--r--   0        0        0     1242 2022-10-24 01:14:16.947677 decode-0.7.1/decode/data/fitsinfo.toml
--rw-r--r--   0        0        0    14163 2022-10-24 01:14:16.947677 decode-0.7.1/decode/io.py
--rw-r--r--   0        0        0     1731 2022-10-24 01:14:16.947677 decode-0.7.1/decode/logging.py
--rw-r--r--   0        0        0    14491 2022-10-24 01:14:16.947677 decode-0.7.1/decode/models.py
--rw-r--r--   0        0        0     9840 2022-10-24 01:14:16.947677 decode-0.7.1/decode/plot.py
--rw-r--r--   0        0        0     9188 2022-10-24 01:14:16.947677 decode-0.7.1/decode/utils.py
--rw-r--r--   0        0        0     1095 2022-10-24 01:14:16.955677 decode-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 decode-0.7.1/setup.py
--rw-r--r--   0        0        0     2058 1970-01-01 00:00:00.000000 decode-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-15 15:14:59.746652 decode-1.0.0/LICENSE
+-rw-r--r--   0        0        0      830 2023-07-15 15:14:59.746652 decode-1.0.0/README.md
+-rw-r--r--   0        0        0      574 2023-07-15 15:14:59.746652 decode-1.0.0/decode/__init__.py
+-rw-r--r--   0        0        0     9658 2023-07-15 15:14:59.746652 decode-1.0.0/decode/array.py
+-rw-r--r--   0        0        0    12226 2023-07-15 15:14:59.746652 decode-1.0.0/decode/cube.py
+-rw-r--r--   0        0        0     1242 2023-07-15 15:14:59.746652 decode-1.0.0/decode/data/fitsinfo.toml
+-rw-r--r--   0        0        0    14143 2023-07-15 15:14:59.746652 decode-1.0.0/decode/io.py
+-rw-r--r--   0        0        0     1725 2023-07-15 15:14:59.746652 decode-1.0.0/decode/logging.py
+-rw-r--r--   0        0        0    14471 2023-07-15 15:14:59.746652 decode-1.0.0/decode/models.py
+-rw-r--r--   0        0        0     9803 2023-07-15 15:14:59.746652 decode-1.0.0/decode/plot.py
+-rw-r--r--   0        0        0     9190 2023-07-15 15:14:59.746652 decode-1.0.0/decode/utils.py
+-rw-r--r--   0        0        0      906 2023-07-15 15:14:59.754652 decode-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 decode-1.0.0/PKG-INFO
```

### Comparing `decode-0.7.1/LICENSE` & `decode-1.0.0/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2022 DESHIMA software team
+Copyright (c) 2018-2023 Akio Taniguchi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `decode-0.7.1/README.md` & `decode-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# De:code
+# de:code
 
-[![Release](https://img.shields.io/pypi/v/decode?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/pypi/decode/)
-[![Python](https://img.shields.io/pypi/pyversions/decode?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/pypi/decode/)
+[![Release](https://img.shields.io/pypi/v/decode?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/decode/)
+[![Python](https://img.shields.io/pypi/pyversions/decode?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/decode/)
 [![Downloads](https://img.shields.io/pypi/dm/decode?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/decode)
 [![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.3384216-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.3384216)
-[![Tests](https://img.shields.io/github/workflow/status/deshima-dev/decode/Tests?label=Tests&style=flat-square)](https://github.com/deshima-dev/decode/actions/tests.yml)
+[![Tests](https://img.shields.io/github/actions/workflow/status/deshima-dev/decode/tests.yml?label=Tests&style=flat-square)](https://github.com/deshima-dev/decode/actions)
 
 DESHIMA code for data analysis
 
 ## Installation
 
 ```shell
-$ pip install decode
+pip install decode
 ```
```

### Comparing `decode-0.7.1/decode/array.py` & `decode-1.0.0/decode/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,20 @@
     "concat",
 ]
 
 
 # standard library
 from dataclasses import dataclass
 from logging import getLogger
-from typing import Any, Tuple
+from typing import Any, Literal, Tuple
 
 
 # dependencies
 import numpy as np
 import xarray as xr
-from typing_extensions import Literal
 from xarray_dataclasses import AsDataArray, Coord, Data
 
 
 # type hints
 _ = Tuple[()]
 Ti = Literal["t"]
 Ch = Literal["ch"]
```

### Comparing `decode-0.7.1/decode/cube.py` & `decode-1.0.0/decode/cube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-__all__ = ["cube", "fromcube", "tocube", "makecontinuum"]
+__all__ = [
+    "cube",
+    "fromcube",
+    "tocube",
+    "makecontinuum",
+]
 
 
 # standard library
 from dataclasses import dataclass
 from logging import getLogger
-from typing import Any, Tuple
+from typing import Any, Literal, Tuple
 
 
 # dependencies
 import numpy as np
 import xarray as xr
 from astropy import units as u
 from scipy.interpolate import interp1d
-from scipy.ndimage.interpolation import map_coordinates
-from typing_extensions import Literal
+from scipy.ndimage import map_coordinates
 from xarray_dataclasses import AsDataArray, Coord, Data
 
 
 # type hints
 _ = Tuple[()]
 X = Literal["x"]
 Y = Literal["y"]
```

### Comparing `decode-0.7.1/decode/data/fitsinfo.toml` & `decode-1.0.0/decode/data/fitsinfo.toml`

 * *Files identical despite different names*

### Comparing `decode-0.7.1/decode/io.py` & `decode-1.0.0/decode/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-# coding: utf-8
-
-
-# public items
-__all__ = ["loaddfits", "savefits", "loadnetcdf", "savenetcdf"]
+__all__ = [
+    "loaddfits",
+    "savefits",
+    "loadnetcdf",
+    "savenetcdf",
+]
 
 
 # standard library
 from datetime import datetime
 from pytz import timezone
 from logging import getLogger
 from uuid import uuid4
 from pathlib import Path
 from pkgutil import get_data
 
 
-# dependent packages
+# dependencies
 import tomli
 import decode as dc
 import numpy as np
 import xarray as xr
 from astropy.io import fits
 from scipy.interpolate import interp1d
```

### Comparing `decode-0.7.1/decode/logging.py` & `decode-1.0.0/decode/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# coding: utf-8
 __all__ = ["setlogger"]
 
 
 # standard library
 import logging
 from copy import copy
 from pathlib import Path
 
-logger = logging.getLogger(__name__)
-
 
-# module constants
+# constants
 DATEFORMAT = "%Y-%m-%d %H:%M:%S"
 LOGFORMAT = "{asctime} | {levelname:8} | {funcName}: {message}"
 DEFAULTLEVEL = "INFO"
 
 
+# module logger
+logger = logging.getLogger(__name__)
+
+
 # classes
 class setlogger(object):
     def __init__(self, level=None, filename=None, overwrite=False, encoding="utf-8"):
         self.logger = logging.getLogger("decode")
         self.logger.addHandler(logging.NullHandler())
         # save current state
         self.oldhandlers = copy(self.logger.handlers)
```

### Comparing `decode-0.7.1/decode/models.py` & `decode-1.0.0/decode/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# coding: utf-8
-
-
-# public items
-__all__ = ["pca", "chopper_calibration", "r_division", "gauss_fit"]
+__all__ = [
+    "pca",
+    "chopper_calibration",
+    "r_division",
+    "gauss_fit",
+]
 
 
 # standard library
 from logging import getLogger
 
 
-# dependent packages
+# dependencies
 import decode as dc
 import numpy as np
 from astropy.modeling import fitting, models
 from sklearn.decomposition import TruncatedSVD
 
 
 def pca(onarray, offarray, n=10, exchs=None, pc=False, mode="mean"):
```

### Comparing `decode-0.7.1/decode/plot.py` & `decode-1.0.0/decode/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# coding: utf-8
-
-
-# public items
 __all__ = [
     "plotcoords",
     "plot_tcoords",
     "plottimestream",
     "plot_timestream",
     "plotspectrum",
     "plot_spectrum",
@@ -15,18 +11,18 @@
 ]
 
 
 # standard library
 from logging import getLogger
 
 
-# dependent packages
+# dependencies
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy.signal import hanning
+from scipy.signal.windows import hann
 from .utils import allan_variance, deprecation_warning, psd
 
 
 # module logger
 logger = getLogger(__name__)
 
 
@@ -232,15 +228,15 @@
     im = ax.pcolormesh(cube.x, cube.y, cube[:, :, index].T, **kwargs)
     ax.set_xlabel("x")
     ax.set_ylabel("y")
     ax.set_title("intensity map ch #{}".format(kidid))
     return im
 
 
-def plotpsd(data, dt, ndivide=1, window=hanning, overlap_half=False, ax=None, **kwargs):
+def plotpsd(data, dt, ndivide=1, window=hann, overlap_half=False, ax=None, **kwargs):
     """Plot PSD (Power Spectral Density).
 
     Args:
         data (np.ndarray): Input data.
         dt (float): Time between each data.
         ndivide (int): Do averaging (split data into ndivide,
             get psd of each, and average them).
```

### Comparing `decode-0.7.1/decode/utils.py` & `decode-1.0.0/decode/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # dependencies
 import numpy as np
 import xarray as xr
 from morecopy import copy
 from scipy import ndimage
 from scipy.fftpack import fftfreq, fft
-from scipy.signal import hanning
+from scipy.signal.windows import hann
 
 
 # constants
 DEFAULT_N_CHUNKS = 1
 try:
     MAX_WORKERS = cpu_count() - 1
 except NotImplementedError:
@@ -203,15 +203,15 @@
         finally:
             # revert to the original value
             mkl.set_num_threads(n_threads)
     else:
         yield
 
 
-def psd(data, dt, ndivide=1, window=hanning, overlap_half=False):
+def psd(data, dt, ndivide=1, window=hann, overlap_half=False):
     """Calculate power spectrum density of data.
 
     Args:
         data (np.ndarray): Input data.
         dt (float): Time between each data.
         ndivide (int): Do averaging (split data into ndivide,
             get psd of each, and average them).
```

### Comparing `decode-0.7.1/pyproject.toml` & `decode-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 [tool.poetry]
 name = "decode"
-version = "0.7.1"
+version = "1.0.0"
 description = "DESHIMA code for data analysis"
-authors = [
-    "Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>",
-    "Tsuyoshi Ishida <tishida@ioa.s.u-tokyo.ac.jp>",
-]
+authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 keywords = [
     "astronomy",
     "data-analysis",
     "deshima",
     "spectroscopy",
     "submillimeter",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/deshima-dev/decode/"
 documentation = "https://deshima-dev.github.io/decode/"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1, <3.10"
-astropy = [
-    { version = "^4.3", python = ">=3.7.1, <3.8" },
-    { version = "^5.1", python = ">=3.8, <3.10" },
-]
-matplotlib = "^3.2"
-morecopy = "^0.2"
-netcdf4 = "^1.5"
-numpy = "^1.21"
-scikit-learn = "^1.0"
-scipy = "^1.7"
+python = ">=3.8, <3.12"
+astropy = "^5.2"
+matplotlib = "^3.6"
+morecopy = "^0.3"
+netcdf4 = "^1.6"
+numpy = "^1.22"
+scikit-learn = "^1.2"
+scipy = "^1.9"
 tomli = "^2.0"
-tqdm = "^4.64"
-typing-extensions = "^3.10"
-xarray = "^0.20"
-xarray-dataclasses = "^1.2"
+tqdm = "^4.65"
+xarray = "^2022.3"
+xarray-dataclasses = "^1.6"
 
-[tool.poetry.dev-dependencies]
-black = "^22.3"
-ipython = "^7.32"
-myst-parser = "^0.18"
-pydata-sphinx-theme = "^0.8"
-pytest = "^7.1"
-sphinx = "^5.0"
+[tool.poetry.group.dev.dependencies]
+black = "^23.7"
+ipython = "^8.12"
+myst-parser = "^2.0"
+pydata-sphinx-theme = "^0.13"
+pytest = "^7.4"
+sphinx = "^7.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `decode-0.7.1/PKG-INFO` & `decode-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: decode
-Version: 0.7.1
+Version: 1.0.0
 Summary: DESHIMA code for data analysis
 Home-page: https://github.com/deshima-dev/decode/
 License: MIT
 Keywords: astronomy,data-analysis,deshima,spectroscopy,submillimeter
 Author: Akio Taniguchi
 Author-email: taniguchi@a.phys.nagoya-u.ac.jp
-Requires-Python: >=3.7.1,<3.10
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: astropy (>=4.3,<5.0); python_full_version >= "3.7.1" and python_version < "3.8"
-Requires-Dist: astropy (>=5.1,<6.0); python_version >= "3.8" and python_version < "3.10"
-Requires-Dist: matplotlib (>=3.2,<4.0)
-Requires-Dist: morecopy (>=0.2,<0.3)
-Requires-Dist: netcdf4 (>=1.5,<2.0)
-Requires-Dist: numpy (>=1.21,<2.0)
-Requires-Dist: scikit-learn (>=1.0,<2.0)
-Requires-Dist: scipy (>=1.7,<2.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astropy (>=5.2,<6.0)
+Requires-Dist: matplotlib (>=3.6,<4.0)
+Requires-Dist: morecopy (>=0.3,<0.4)
+Requires-Dist: netcdf4 (>=1.6,<2.0)
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: scikit-learn (>=1.2,<2.0)
+Requires-Dist: scipy (>=1.9,<2.0)
 Requires-Dist: tomli (>=2.0,<3.0)
-Requires-Dist: tqdm (>=4.64,<5.0)
-Requires-Dist: typing-extensions (>=3.10,<4.0)
-Requires-Dist: xarray (>=0.20,<0.21)
-Requires-Dist: xarray-dataclasses (>=1.2,<2.0)
+Requires-Dist: tqdm (>=4.65,<5.0)
+Requires-Dist: xarray (>=2022.3,<2023.0)
+Requires-Dist: xarray-dataclasses (>=1.6,<2.0)
 Project-URL: Documentation, https://deshima-dev.github.io/decode/
 Description-Content-Type: text/markdown
 
-# De:code
+# de:code
 
-[![Release](https://img.shields.io/pypi/v/decode?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/pypi/decode/)
-[![Python](https://img.shields.io/pypi/pyversions/decode?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/pypi/decode/)
+[![Release](https://img.shields.io/pypi/v/decode?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/decode/)
+[![Python](https://img.shields.io/pypi/pyversions/decode?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/decode/)
 [![Downloads](https://img.shields.io/pypi/dm/decode?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/decode)
 [![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.3384216-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.3384216)
-[![Tests](https://img.shields.io/github/workflow/status/deshima-dev/decode/Tests?label=Tests&style=flat-square)](https://github.com/deshima-dev/decode/actions/tests.yml)
+[![Tests](https://img.shields.io/github/actions/workflow/status/deshima-dev/decode/tests.yml?label=Tests&style=flat-square)](https://github.com/deshima-dev/decode/actions)
 
 DESHIMA code for data analysis
 
 ## Installation
 
 ```shell
-$ pip install decode
+pip install decode
 ```
```

