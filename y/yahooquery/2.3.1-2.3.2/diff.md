# Comparing `tmp/yahooquery-2.3.1.tar.gz` & `tmp/yahooquery-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yahooquery-2.3.1.tar", last modified: Sat Mar 18 20:48:39 2023, max compression
+gzip compressed data, was "yahooquery-2.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `yahooquery-2.3.1.tar` & `yahooquery-2.3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0       11 2023-03-18 20:48:04.501187 yahooquery-2.3.1/.gitattributes
--rw-r--r--   0        0        0      834 2023-03-18 20:48:04.501187 yahooquery-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2023-03-18 20:48:04.501187 yahooquery-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      687 2023-03-18 20:48:04.501187 yahooquery-2.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1359 2023-03-18 20:48:04.501187 yahooquery-2.3.1/.gitignore
--rw-r--r--   0        0        0      608 2023-03-18 20:48:04.501187 yahooquery-2.3.1/.travis.yml
--rw-r--r--   0        0        0     9472 2023-03-18 20:48:04.501187 yahooquery-2.3.1/CHANGELOG.rst
--rw-r--r--   0        0        0       25 2023-03-18 20:48:04.501187 yahooquery-2.3.1/CNAME
--rw-r--r--   0        0        0     3359 2023-03-18 20:48:04.501187 yahooquery-2.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2087 2023-03-18 20:48:04.501187 yahooquery-2.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1068 2023-03-18 20:48:04.501187 yahooquery-2.3.1/LICENSE.txt
--rw-r--r--   0        0        0       71 2023-03-18 20:48:04.501187 yahooquery-2.3.1/MANIFEST.in
--rw-r--r--   0        0        0     4020 2023-03-18 20:48:04.501187 yahooquery-2.3.1/README.md
--rw-r--r--   0        0        0   897270 2023-03-18 20:48:04.505187 yahooquery-2.3.1/demo/demo.gif
--rw-r--r--   0        0        0    94124 2023-03-18 20:48:04.509188 yahooquery-2.3.1/demo/valuation_measures.PNG
--rw-r--r--   0        0        0       24 2023-03-18 20:48:04.509188 yahooquery-2.3.1/docs/docs/CNAME
--rw-r--r--   0        0        0  1514796 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/alternative.ipynb
--rw-r--r--   0        0        0        0 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/contact.md
--rw-r--r--   0        0        0     1961 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/css/termynal.css
--rw-r--r--   0        0        0     1461 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/advanced.md
--rw-r--r--   0        0        0     1274 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/index.md
--rw-r--r--   0        0        0    10102 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/keyword_arguments.md
--rw-r--r--   0        0        0    56084 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/misc.md
--rw-r--r--   0        0        0    11889 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/research.md
--rw-r--r--   0        0        0    47729 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/screener.md
--rw-r--r--   0        0        0    61778 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/ticker/financials.md
--rw-r--r--   0        0        0     3571 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/ticker/historical.md
--rw-r--r--   0        0        0     1051 2023-03-18 20:48:04.513188 yahooquery-2.3.1/docs/docs/guide/ticker/intro.md
--rw-r--r--   0        0        0    35303 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/guide/ticker/miscellaneous.md
--rw-r--r--   0        0        0   103869 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/guide/ticker/modules.md
--rw-r--r--   0        0        0     2813 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/guide/ticker/options.md
--rw-r--r--   0        0        0   114808 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/guide/ticker/premium.md
--rw-r--r--   0        0        0        0 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/help.md
--rw-r--r--   0        0        0    11699 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/img/full.png
--rw-r--r--   0        0        0    11091 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/img/logo-purple.png
--rw-r--r--   0        0        0    10673 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/img/logo-white.png
--rw-r--r--   0        0        0   125884 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/img/stock-chart.png
--rw-r--r--   0        0        0     4480 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/index.md
--rw-r--r--   0        0        0     5662 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/js/custom.js
--rw-r--r--   0        0        0     9512 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/js/termynal.js
--rw-r--r--   0        0        0     8143 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/docs/release_notes.md
--rw-r--r--   0        0        0     1967 2023-03-18 20:48:04.517188 yahooquery-2.3.1/docs/mkdocs.yml
--rw-r--r--   0        0        0     1282 2023-03-18 20:48:04.517188 yahooquery-2.3.1/pyproject.toml
--rw-r--r--   0        0        0      157 2023-03-18 20:48:04.517188 yahooquery-2.3.1/pytest.ini
--rw-r--r--   0        0        0       79 2023-03-18 20:48:04.517188 yahooquery-2.3.1/requirements.txt
--rw-r--r--   0        0        0     1307 2023-03-18 20:48:04.517188 yahooquery-2.3.1/setup.py
--rw-r--r--   0        0        0        0 2023-03-18 20:48:04.517188 yahooquery-2.3.1/tests/__init__.py
--rw-r--r--   0        0        0      547 2023-03-18 20:48:04.517188 yahooquery-2.3.1/tests/test_country.py
--rw-r--r--   0        0        0      719 2023-03-18 20:48:04.517188 yahooquery-2.3.1/tests/test_miscellaneous.py
--rw-r--r--   0        0        0     1292 2023-03-18 20:48:04.517188 yahooquery-2.3.1/tests/test_research.py
--rw-r--r--   0        0        0      374 2023-03-18 20:48:04.517188 yahooquery-2.3.1/tests/test_screener.py
--rw-r--r--   0        0        0    28404 2023-03-18 20:48:04.517188 yahooquery-2.3.1/tests/test_ticker.py
--rw-r--r--   0        0        0      345 2023-03-18 20:48:04.517188 yahooquery-2.3.1/yahooquery/__init__.py
--rw-r--r--   0        0        0    46377 2023-03-18 20:48:04.517188 yahooquery-2.3.1/yahooquery/base.py
--rw-r--r--   0        0        0     2771 2023-03-18 20:48:04.517188 yahooquery-2.3.1/yahooquery/login.py
--rw-r--r--   0        0        0     3510 2023-03-18 20:48:04.517188 yahooquery-2.3.1/yahooquery/misc.py
--rw-r--r--   0        0        0    10189 2023-03-18 20:48:04.517188 yahooquery-2.3.1/yahooquery/research.py
--rw-r--r--   0        0        0     2920 2023-03-18 20:48:04.521188 yahooquery-2.3.1/yahooquery/screener.py
--rw-r--r--   0        0        0    43075 2023-03-18 20:48:04.521188 yahooquery-2.3.1/yahooquery/ticker.py
--rw-r--r--   0        0        0     7915 2023-03-18 20:48:04.521188 yahooquery-2.3.1/yahooquery/utils/__init__.py
--rw-r--r--   0        0        0     1450 2023-03-18 20:48:04.521188 yahooquery-2.3.1/yahooquery/utils/countries.py
--rw-r--r--   0        0        0    73414 2023-03-18 20:48:04.521188 yahooquery-2.3.1/yahooquery/utils/screeners.py
--rw-r--r--   0        0        0     5559 1970-01-01 00:00:00.000000 yahooquery-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2023-07-15 19:30:35.151144 yahooquery-2.3.2/.gitattributes
+-rw-r--r--   0        0        0      834 2023-07-15 19:30:35.151144 yahooquery-2.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2023-07-15 19:30:35.151144 yahooquery-2.3.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      687 2023-07-15 19:30:35.151144 yahooquery-2.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1359 2023-07-15 19:30:35.151144 yahooquery-2.3.2/.gitignore
+-rw-r--r--   0        0        0      608 2023-07-15 19:30:35.151144 yahooquery-2.3.2/.travis.yml
+-rw-r--r--   0        0        0    10255 2023-07-15 19:30:35.151144 yahooquery-2.3.2/CHANGELOG.rst
+-rw-r--r--   0        0        0       25 2023-07-15 19:30:35.151144 yahooquery-2.3.2/CNAME
+-rw-r--r--   0        0        0     3359 2023-07-15 19:30:35.151144 yahooquery-2.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2087 2023-07-15 19:30:35.151144 yahooquery-2.3.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1068 2023-07-15 19:30:35.151144 yahooquery-2.3.2/LICENSE.txt
+-rw-r--r--   0        0        0       71 2023-07-15 19:30:35.151144 yahooquery-2.3.2/MANIFEST.in
+-rw-r--r--   0        0        0     4020 2023-07-15 19:30:35.151144 yahooquery-2.3.2/README.md
+-rw-r--r--   0        0        0   897270 2023-07-15 19:30:35.155143 yahooquery-2.3.2/demo/demo.gif
+-rw-r--r--   0        0        0    94124 2023-07-15 19:30:35.155143 yahooquery-2.3.2/demo/valuation_measures.PNG
+-rw-r--r--   0        0        0       24 2023-07-15 19:30:35.155143 yahooquery-2.3.2/docs/docs/CNAME
+-rw-r--r--   0        0        0  1514796 2023-07-15 19:30:35.159143 yahooquery-2.3.2/docs/docs/alternative.ipynb
+-rw-r--r--   0        0        0        0 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/contact.md
+-rw-r--r--   0        0        0     1961 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/css/termynal.css
+-rw-r--r--   0        0        0     1461 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/advanced.md
+-rw-r--r--   0        0        0     1274 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/index.md
+-rw-r--r--   0        0        0    10102 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/keyword_arguments.md
+-rw-r--r--   0        0        0    56084 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/misc.md
+-rw-r--r--   0        0        0    11889 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/research.md
+-rw-r--r--   0        0        0    47729 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/screener.md
+-rw-r--r--   0        0        0    61778 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/ticker/financials.md
+-rw-r--r--   0        0        0     3571 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/ticker/historical.md
+-rw-r--r--   0        0        0     1051 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/ticker/intro.md
+-rw-r--r--   0        0        0    35303 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/ticker/miscellaneous.md
+-rw-r--r--   0        0        0   103869 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/ticker/modules.md
+-rw-r--r--   0        0        0     2813 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/ticker/options.md
+-rw-r--r--   0        0        0   114808 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/guide/ticker/premium.md
+-rw-r--r--   0        0        0        0 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/help.md
+-rw-r--r--   0        0        0    11699 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/img/full.png
+-rw-r--r--   0        0        0    11091 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/img/logo-purple.png
+-rw-r--r--   0        0        0    10673 2023-07-15 19:30:35.163143 yahooquery-2.3.2/docs/docs/img/logo-white.png
+-rw-r--r--   0        0        0   125884 2023-07-15 19:30:35.167143 yahooquery-2.3.2/docs/docs/img/stock-chart.png
+-rw-r--r--   0        0        0     4480 2023-07-15 19:30:35.167143 yahooquery-2.3.2/docs/docs/index.md
+-rw-r--r--   0        0        0     5662 2023-07-15 19:30:35.167143 yahooquery-2.3.2/docs/docs/js/custom.js
+-rw-r--r--   0        0        0     9512 2023-07-15 19:30:35.167143 yahooquery-2.3.2/docs/docs/js/termynal.js
+-rw-r--r--   0        0        0     8143 2023-07-15 19:30:35.167143 yahooquery-2.3.2/docs/docs/release_notes.md
+-rw-r--r--   0        0        0     1967 2023-07-15 19:30:35.167143 yahooquery-2.3.2/docs/mkdocs.yml
+-rw-r--r--   0        0        0     1282 2023-07-15 19:30:35.167143 yahooquery-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-07-15 19:30:35.167143 yahooquery-2.3.2/pytest.ini
+-rw-r--r--   0        0        0       79 2023-07-15 19:30:35.167143 yahooquery-2.3.2/requirements.txt
+-rw-r--r--   0        0        0     1307 2023-07-15 19:30:35.167143 yahooquery-2.3.2/setup.py
+-rw-r--r--   0        0        0        0 2023-07-15 19:30:35.167143 yahooquery-2.3.2/tests/__init__.py
+-rw-r--r--   0        0        0      547 2023-07-15 19:30:35.167143 yahooquery-2.3.2/tests/test_country.py
+-rw-r--r--   0        0        0      719 2023-07-15 19:30:35.167143 yahooquery-2.3.2/tests/test_miscellaneous.py
+-rw-r--r--   0        0        0     1292 2023-07-15 19:30:35.167143 yahooquery-2.3.2/tests/test_research.py
+-rw-r--r--   0        0        0      374 2023-07-15 19:30:35.167143 yahooquery-2.3.2/tests/test_screener.py
+-rw-r--r--   0        0        0    28404 2023-07-15 19:30:35.167143 yahooquery-2.3.2/tests/test_ticker.py
+-rw-r--r--   0        0        0      345 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/__init__.py
+-rw-r--r--   0        0        0    46376 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/base.py
+-rw-r--r--   0        0        0     2771 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/login.py
+-rw-r--r--   0        0        0     3510 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/misc.py
+-rw-r--r--   0        0        0    10189 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/research.py
+-rw-r--r--   0        0        0     2923 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/screener.py
+-rw-r--r--   0        0        0    43075 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/ticker.py
+-rw-r--r--   0        0        0     7915 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/utils/__init__.py
+-rw-r--r--   0        0        0     1450 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/utils/countries.py
+-rw-r--r--   0        0        0    73414 2023-07-15 19:30:35.167143 yahooquery-2.3.2/yahooquery/utils/screeners.py
+-rw-r--r--   0        0        0     5559 1970-01-01 00:00:00.000000 yahooquery-2.3.2/PKG-INFO
```

### Comparing `yahooquery-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `yahooquery-2.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `yahooquery-2.3.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/.github/workflows/python-publish.yml` & `yahooquery-2.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/.gitignore` & `yahooquery-2.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/.travis.yml` & `yahooquery-2.3.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/CHANGELOG.rst` & `yahooquery-2.3.2/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 Change Log
 ==========
 
+2.3.2
+-----
+## Update
+- Update quote summary endpoint from v10 to v6.  The v10 endpoint currently requires a crumb as a query parameter, which is not something this library does not currently support.
+
+## Fix
+- Bug related to retrieving screen IDs with a number
+
+2.3.1
+-----
+## FIx
+- Fixes for history method
+
+2.3.0
+-----
+## Added
+- `dividend_history` method that returns historical dividends paid for a given symbol(s)
+
+## Fixed
+- `history` method has been refactored pretty heavily with the help of @maread99 (Thank you!).  Timezone info is now included in the `date` column.  Also, a dataframe will always be returned regardless of bad symbols existing.  Previously, a dictionary was returned with the json response for the bad symbol(s) and dataframes for successful responses.
+
 2.2.15
 ------
 - Updated the data available from the cash flow statement
 
 2.2.14
 ------
 - Updated the financials dataframes (cash_flow, income_statement, balance_sheet, all_financial_data,
```

### Comparing `yahooquery-2.3.1/CODE_OF_CONDUCT.md` & `yahooquery-2.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/CONTRIBUTING.md` & `yahooquery-2.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/LICENSE.txt` & `yahooquery-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/README.md` & `yahooquery-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/demo/demo.gif` & `yahooquery-2.3.2/demo/demo.gif`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/demo/valuation_measures.PNG` & `yahooquery-2.3.2/demo/valuation_measures.PNG`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/alternative.ipynb` & `yahooquery-2.3.2/docs/docs/alternative.ipynb`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/css/termynal.css` & `yahooquery-2.3.2/docs/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/advanced.md` & `yahooquery-2.3.2/docs/docs/guide/advanced.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/index.md` & `yahooquery-2.3.2/docs/docs/guide/index.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/keyword_arguments.md` & `yahooquery-2.3.2/docs/docs/guide/keyword_arguments.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/misc.md` & `yahooquery-2.3.2/docs/docs/guide/misc.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/research.md` & `yahooquery-2.3.2/docs/docs/guide/research.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/screener.md` & `yahooquery-2.3.2/docs/docs/guide/screener.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/ticker/financials.md` & `yahooquery-2.3.2/docs/docs/guide/ticker/financials.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/ticker/historical.md` & `yahooquery-2.3.2/docs/docs/guide/ticker/historical.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/ticker/intro.md` & `yahooquery-2.3.2/docs/docs/guide/ticker/intro.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/ticker/miscellaneous.md` & `yahooquery-2.3.2/docs/docs/guide/ticker/miscellaneous.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/ticker/modules.md` & `yahooquery-2.3.2/docs/docs/guide/ticker/modules.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/ticker/options.md` & `yahooquery-2.3.2/docs/docs/guide/ticker/options.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/guide/ticker/premium.md` & `yahooquery-2.3.2/docs/docs/guide/ticker/premium.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/img/full.png` & `yahooquery-2.3.2/docs/docs/img/full.png`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/img/logo-purple.png` & `yahooquery-2.3.2/docs/docs/img/logo-purple.png`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/img/logo-white.png` & `yahooquery-2.3.2/docs/docs/img/logo-white.png`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/img/stock-chart.png` & `yahooquery-2.3.2/docs/docs/img/stock-chart.png`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/index.md` & `yahooquery-2.3.2/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/js/custom.js` & `yahooquery-2.3.2/docs/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/js/termynal.js` & `yahooquery-2.3.2/docs/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/docs/release_notes.md` & `yahooquery-2.3.2/docs/docs/release_notes.md`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/docs/mkdocs.yml` & `yahooquery-2.3.2/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/pyproject.toml` & `yahooquery-2.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/setup.py` & `yahooquery-2.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="yahooquery",
-    version="2.3.1",
+    version="2.3.2",
     author="Doug Guthrie",
     author_email="douglas.p.guthrie@gmail.com",
     description="Retrieve nearly all data from Yahoo Finance for one or more ticker symbols",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
```

### Comparing `yahooquery-2.3.1/tests/test_country.py` & `yahooquery-2.3.2/tests/test_country.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/tests/test_miscellaneous.py` & `yahooquery-2.3.2/tests/test_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/tests/test_research.py` & `yahooquery-2.3.2/tests/test_research.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/tests/test_ticker.py` & `yahooquery-2.3.2/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/yahooquery/base.py` & `yahooquery-2.3.2/yahooquery/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
                 "widths": {"required": False, "default": None},
                 "tags": {"required": False, "default": None},
                 "filterOldVideos": {"required": False, "default": None},
                 "category": {"required": False, "default": None},
             },
         },
         "quoteSummary": {
-            "path": "https://query2.finance.yahoo.com/v10/finance/quoteSummary/{symbol}",
+            "path": "https://query2.finance.yahoo.com/v6/finance/quoteSummary/{symbol}",
             "response_field": "quoteSummary",
             "query": {
                 "formatted": {"required": False, "default": False},
                 "modules": {
                     "required": True,
                     "default": None,
                     "options": list(_MODULES_DICT.keys()),
```

### Comparing `yahooquery-2.3.1/yahooquery/login.py` & `yahooquery-2.3.2/yahooquery/login.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/yahooquery/misc.py` & `yahooquery-2.3.2/yahooquery/misc.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/yahooquery/research.py` & `yahooquery-2.3.2/yahooquery/research.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/yahooquery/screener.py` & `yahooquery-2.3.2/yahooquery/screener.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         screener_id = query_params["scrIds"]
         key = next((k for k in SCREENERS if SCREENERS[k]["id"] == screener_id))
         return key
 
     def _check_screen_ids(self, screen_ids):
         all_screeners = list(SCREENERS.keys())
         if not isinstance(screen_ids, list):
-            screen_ids = re.findall(r"[a-zA-Z_]+", screen_ids)
+            screen_ids = re.findall(r"[a-zA-Z0-9_]+", screen_ids)
         if any(elem not in all_screeners for elem in screen_ids):
             raise ValueError(
                 "One of {} is not a valid screener.  \
                               Please check available_screeners".format(
                     ", ".join(screen_ids)
                 )
             )
```

### Comparing `yahooquery-2.3.1/yahooquery/ticker.py` & `yahooquery-2.3.2/yahooquery/ticker.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/yahooquery/utils/__init__.py` & `yahooquery-2.3.2/yahooquery/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/yahooquery/utils/countries.py` & `yahooquery-2.3.2/yahooquery/utils/countries.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/yahooquery/utils/screeners.py` & `yahooquery-2.3.2/yahooquery/utils/screeners.py`

 * *Files identical despite different names*

### Comparing `yahooquery-2.3.1/PKG-INFO` & `yahooquery-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yahooquery
-Version: 2.3.1
+Version: 2.3.2
 Summary: Python interface to unofficial Yahoo Finance API endpoints
 Home-page: https://github.com/dpguthrie/yahooquery
 Author: Doug Guthrie
 Author-email: douglas.p.guthrie@gmail.com
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yahooquery Version: 2.3.1 Summary: Python interface
+Metadata-Version: 2.1 Name: yahooquery Version: 2.3.2 Summary: Python interface
 to unofficial Yahoo Finance API endpoints Home-page: https://github.com/
 dpguthrie/yahooquery Author: Doug Guthrie Author-email:
 douglas.p.guthrie@gmail.com Description-Content-Type: text/markdown Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
 Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

