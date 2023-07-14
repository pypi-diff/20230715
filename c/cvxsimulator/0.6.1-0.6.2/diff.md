# Comparing `tmp/cvxsimulator-0.6.1.tar.gz` & `tmp/cvxsimulator-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.6.1.tar", max compression
+gzip compressed data, was "cvxsimulator-0.6.2.tar", max compression
```

## Comparing `cvxsimulator-0.6.1.tar` & `cvxsimulator-0.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11375 2023-07-11 06:54:48.576622 cvxsimulator-0.6.1/LICENSE
--rw-r--r--   0        0        0     5166 2023-07-11 06:54:48.576622 cvxsimulator-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    16756 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1613 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1457 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/month.py
--rw-r--r--   0        0        0    20589 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      795 2023-07-11 06:54:48.664623 cvxsimulator-0.6.1/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      726 2023-07-11 06:55:14.244555 cvxsimulator-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5784 1970-01-01 00:00:00.000000 cvxsimulator-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10790 2023-07-14 22:59:44.301752 cvxsimulator-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5690 2023-07-14 22:59:44.301752 cvxsimulator-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    17055 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1613 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1457 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/month.py
+-rw-r--r--   0        0        0    23577 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      795 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      895 2023-07-14 23:00:18.521510 cvxsimulator-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 cvxsimulator-0.6.2/PKG-INFO
```

### Comparing `cvxsimulator-0.6.1/LICENSE` & `cvxsimulator-0.6.2/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -171,25 +171,14 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
    Copyright 2023 Stanford University Convex Optimization Group
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cvxsimulator-0.6.1/README.md` & `cvxsimulator-0.6.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,25 +9,30 @@
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$,
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
 
-## Modus operandi
+## Creating portfolios
 
 The simulator shall be completely agnostic as to the trading policy/strategy.
 Our approach follows a rather common pattern:
 
 * [Create the builder object](#create-the-builder-object)
 * [Loop through time](#loop-through-time)
-* [Analyse results](#analyse-results)
+* [Build the portfolio](#build-the-portfolio)
 
 We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
 
+Of course, some users may know prices and weights in advance. In that case, the building procedure can be bypassed.
+We discuss this in
+
+* [Bypassing the builder](#bypassing-the-builder)
+
 ### Create the builder object
 
 The user defines a builder object by loading a frame of prices
 and initialize the amount of cash used in our experiment:
 
 ```python
 from pathlib import Path
@@ -80,35 +85,23 @@
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b.set_weights(t[-1], pd.Series(index=b.assets, data = 0.25))
 ```
 
+### Build the portfolio
+
 Once finished it is possible to build the portfolio object
 
 ```python
 portfolio = b.build()
 ```
 
-### Analyse results
-
-The loop above is filling up the desired positions.
-After triggering the `build()` the resulting portfolio
-is ready for further analysis.
-It is possible dive into the data, e.g.
-
-```python
-portfolio.nav
-portfolio.cash
-portfolio.equity
-...
-```
-
-## Bypassing the builder
+### Bypassing the builder
 
 Some may know the positions the portfolio shall enter for eternity.
 Running through a loop is rather non-pythonic waste of time in such a case.
 It is possible to completely bypass this step by submitting
 a frame of positions together with a frame of prices when creating the portfolio object.
 
 ```python
@@ -118,14 +111,50 @@
 from cvx.simulator.portfolio import EquityPortfolio
 
 prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 stocks = pd.read_csv(Path("resources") / "stock.csv", index_col=0, parse_dates=True, header=0)
 portfolio = EquityPortfolio(prices=prices, stocks=stocks, initial_cash=1e6)
 ```
 
+
+## Analytics
+
+The portfolio object supports further analysis and exposes
+a number of properties, e.g.
+
+```python
+portfolio.nav
+portfolio.cash
+portfolio.equity
+```
+
+We have also integrated the [quantstats](https://github.com/ranaroussi/quantstats) package for further analysis.
+Hence it is possible to perform
+
+```python
+portfolio.snapshot()
+portfolio.metrics()
+portfolio.plots()
+portfolio.html()
+```
+
+We also added an enum
+
+
+```python
+portfolio.plot(kind=Plot.DRAWDOWN)
+```
+
+supporting all plots defined in quantstats.
+
+![quantstats snapshot](portfolio.png)
+
+
+
+
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
```

### Comparing `cvxsimulator-0.6.1/cvx/simulator/builder.py` & `cvxsimulator-0.6.2/cvx/simulator/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,39 +276,44 @@
         cov = self.returns.ewm(**kwargs).cov()
         cov = cov.dropna(how="all", axis=0)
         for t in cov.index.get_level_values(level=0).unique():
             yield t, cov.loc[t, :, :]
 
         # {t: cov.loc[t, :, :] for t in cov.index.get_level_values('date').unique()}
 
-    def set_weights(self, time, weights):
+    def set_weights(self, time, weights: pd.Series):
         """
         Set the position via weights (e.g. fractions of the nav)
 
         :param time: time
         :param weights: series of weights
         """
+        assert isinstance(weights, pd.Series), "weights must be a pandas Series"
         self[time] = (self._state.nav * weights) / self._state.prices
 
-    def set_cashposition(self, time, cashposition):
+    def set_cashposition(self, time, cashposition: pd.Series):
         """
         Set the position via cash positions (e.g. USD invested per asset)
 
         :param time: time
         :param cashposition: series of cash positions
         """
+        assert isinstance(
+            cashposition, pd.Series
+        ), "cashposition must be a pandas Series"
         self[time] = cashposition / self._state.prices
 
     def set_position(self, time, position):
         """
         Set the position via number of assets (e.g. number of stocks)
 
         :param time: time
         :param position: series of number of stocks
         """
+        assert isinstance(position, pd.Series), "position must be a pandas Series"
         self[time] = position
 
     def __iter__(self):
         """
         The __iter__ method allows the object to be iterated over in a for loop,
         yielding time and the current state of the portfolio.
         The method yields a list of dates seen so far
```

### Comparing `cvxsimulator-0.6.1/cvx/simulator/grid.py` & `cvxsimulator-0.6.2/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.1/cvx/simulator/month.py` & `cvxsimulator-0.6.2/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.1/cvx/simulator/portfolio.py` & `cvxsimulator-0.6.2/cvx/simulator/portfolio.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,23 +27,21 @@
     RETURNS = 10
     ROLLING_BETA = 11
     ROLLING_SHARPE = 12
     ROLLING_SORTINO = 13
     ROLLING_VOLATILITY = 14
     YEARLY_RETURNS = 15
 
-    # def __call__(self, *args, **kwargs):
-    #    return self.func(*args, **kwargs)
-
-    @property
-    def func(self):
-        return getattr(qs.plots, self.name.lower())
-
-    def plot(self, *args, **kwargs):
-        return self.func(*args, **kwargs)
+    #
+    # def __call__(self, returns, **kwargs):
+    #     return self._func(returns=returns, **kwargs)
+
+    def plot(self, returns, **kwargs):
+        func = getattr(qs.plots, self.name.lower())
+        return func(returns=returns, **kwargs)
 
 
 def diff(portfolio1, portfolio2, initial_cash=1e6, trading_cost_model=None):
     # check both portfolios are on the same price grid
     pd.testing.assert_frame_equal(portfolio1.prices, portfolio2.prices)
 
     stocks = portfolio1.stocks - portfolio2.stocks
@@ -466,21 +464,143 @@
         return EquityPortfolio(
             prices=self.prices,
             stocks=stocks,
             trading_cost_model=self.trading_cost_model,
             initial_cash=self.initial_cash,
         )
 
-    def metrics(self, **kwargs):
-        return qs.reports.metrics(self.nav.pct_change().dropna(), **kwargs)
+    def metrics(
+        self,
+        benchmark=None,
+        rf=0.0,
+        display=True,
+        mode="basic",
+        sep=False,
+        compound=True,
+        periods_per_year=252,
+        prepare_returns=True,
+        match_dates=True,
+        **kwargs,
+    ):
+        """
+        The metrics method calculates the performance metrics of an EquityPortfolio object.
 
-    def plots(self, **kwargs):
-        return qs.reports.plots(self.nav.pct_change().dropna(), **kwargs)
+        :param kwargs:
+        :return:
+        """
+        return qs.reports.metrics(
+            returns=self.nav.pct_change().dropna(),
+            benchmark=benchmark,
+            rf=rf,
+            display=display,
+            mode=mode,
+            sep=sep,
+            compounded=compound,
+            periods_per_year=periods_per_year,
+            prepare_returns=prepare_returns,
+            match_dates=match_dates,
+            **kwargs,
+        )
+
+    def plots(
+        self,
+        benchmark=None,
+        grayscale=False,
+        figsize=(8, 5),
+        mode="basic",
+        compounded=True,
+        periods_per_year=252,
+        prepare_returns=True,
+        match_dates=True,
+        **kwargs,
+    ):
+        return qs.reports.plots(
+            returns=self.nav.pct_change().dropna(),
+            benchmark=benchmark,
+            grayscale=grayscale,
+            figsize=figsize,
+            mode=mode,
+            compounded=compounded,
+            periods_per_year=periods_per_year,
+            prepare_returns=prepare_returns,
+            match_dates=match_dates,
+            **kwargs,
+        )
 
     def plot(self, kind: Plot, **kwargs):
         return kind.plot(returns=self.nav.pct_change().dropna(), **kwargs)
 
-    def html(self, **kwargs):
-        return qs.reports.html(self.nav.pct_change().dropna(), **kwargs)
+    def html(
+        self,
+        benchmark=None,
+        rf=0.0,
+        grayscale=False,
+        title="Strategy Tearsheet",
+        output=None,
+        compounded=True,
+        periods_per_year=252,
+        download_filename="quantstats-tearsheet.html",
+        figfmt="svg",
+        template_path=None,
+        match_dates=True,
+        **kwargs,
+    ):
+        return qs.reports.html(
+            returns=self.nav.pct_change().dropna(),
+            benchmark=benchmark,
+            rf=rf,
+            grayscale=grayscale,
+            title=title,
+            output=output,
+            compounded=compounded,
+            periods_per_year=periods_per_year,
+            download_filename=download_filename,
+            figfmt=figfmt,
+            template_path=template_path,
+            match_dates=match_dates,
+            **kwargs,
+        )
 
-    def snapshot(self, **kwargs):
-        return qs.plots.snapshot(self.nav.pct_change().dropna(), **kwargs)
+    def snapshot(
+        self,
+        grayscale=False,
+        figsize=(10, 8),
+        title="Portfolio Summary",
+        fontname="Arial",
+        lw=1.5,
+        mode="comp",
+        subtitle=True,
+        savefig=None,
+        show=True,
+        log_scale=False,
+        **kwargs,
+    ):
+        """
+        The snapshot method creates a snapshot of the performance of an EquityPortfolio object.
+
+        :param grayscale:
+        :param figsize:
+        :param title:
+        :param fontname:
+        :param lw:
+        :param mode:
+        :param subtitle:
+        :param savefig:
+        :param show:
+        :param log_scale:
+        :param kwargs:
+        :return:
+        """
+        return qs.plots.snapshot(
+            returns=self.nav.pct_change().dropna(),
+            grayscale=grayscale,
+            figsize=figsize,
+            title=title,
+            fontname=fontname,
+            lw=lw,
+            mode=mode,
+            subtitle=subtitle,
+            savefig=savefig,
+            show=show,
+            log_scale=log_scale,
+            **kwargs,
+        )
```

### Comparing `cvxsimulator-0.6.1/cvx/simulator/trading_costs.py` & `cvxsimulator-0.6.2/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.1/pyproject.toml` & `cvxsimulator-0.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.6.1"
+version = "v0.6.2"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 numpy = "*"
 pandas = "*"
 quantstats = "*"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.test.dependencies]
 pytest = "7.2.0"
-pytest-cov = "*"
+pytest-cov = "4.0.0"
+mock = "*"
+
+[tool.poetry.group.jupyter.dependencies]
+jupyterlab = "*"
+jupyter-book = "0.15.1"
+
+[tool.peotry.group.linting.dependencies]
+pylint = "*"
+ruff = "0.0.277"
+pre-commit = "*"
+black = "23.3.0"
+
+
+[tool.poetry.group.dev.dependencies]
 yfinance = "*"
 plotly = "*"
 cvxpy = "*"
-jupyterlab = "*"
-jupyter-book = "0.15.1"
 loguru = "*"
-ruff = "*"
-black = "*"
-pre-commit = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = ["E", "F", "I"]
```

### Comparing `cvxsimulator-0.6.1/PKG-INFO` & `cvxsimulator-0.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,25 +27,30 @@
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$,
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
 
-## Modus operandi
+## Creating portfolios
 
 The simulator shall be completely agnostic as to the trading policy/strategy.
 Our approach follows a rather common pattern:
 
 * [Create the builder object](#create-the-builder-object)
 * [Loop through time](#loop-through-time)
-* [Analyse results](#analyse-results)
+* [Build the portfolio](#build-the-portfolio)
 
 We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
 
+Of course, some users may know prices and weights in advance. In that case, the building procedure can be bypassed.
+We discuss this in
+
+* [Bypassing the builder](#bypassing-the-builder)
+
 ### Create the builder object
 
 The user defines a builder object by loading a frame of prices
 and initialize the amount of cash used in our experiment:
 
 ```python
 from pathlib import Path
@@ -98,35 +103,23 @@
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b.set_weights(t[-1], pd.Series(index=b.assets, data = 0.25))
 ```
 
+### Build the portfolio
+
 Once finished it is possible to build the portfolio object
 
 ```python
 portfolio = b.build()
 ```
 
-### Analyse results
-
-The loop above is filling up the desired positions.
-After triggering the `build()` the resulting portfolio
-is ready for further analysis.
-It is possible dive into the data, e.g.
-
-```python
-portfolio.nav
-portfolio.cash
-portfolio.equity
-...
-```
-
-## Bypassing the builder
+### Bypassing the builder
 
 Some may know the positions the portfolio shall enter for eternity.
 Running through a loop is rather non-pythonic waste of time in such a case.
 It is possible to completely bypass this step by submitting
 a frame of positions together with a frame of prices when creating the portfolio object.
 
 ```python
@@ -136,14 +129,50 @@
 from cvx.simulator.portfolio import EquityPortfolio
 
 prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 stocks = pd.read_csv(Path("resources") / "stock.csv", index_col=0, parse_dates=True, header=0)
 portfolio = EquityPortfolio(prices=prices, stocks=stocks, initial_cash=1e6)
 ```
 
+
+## Analytics
+
+The portfolio object supports further analysis and exposes
+a number of properties, e.g.
+
+```python
+portfolio.nav
+portfolio.cash
+portfolio.equity
+```
+
+We have also integrated the [quantstats](https://github.com/ranaroussi/quantstats) package for further analysis.
+Hence it is possible to perform
+
+```python
+portfolio.snapshot()
+portfolio.metrics()
+portfolio.plots()
+portfolio.html()
+```
+
+We also added an enum
+
+
+```python
+portfolio.plot(kind=Plot.DRAWDOWN)
+```
+
+supporting all plots defined in quantstats.
+
+![quantstats snapshot](portfolio.png)
+
+
+
+
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
```

