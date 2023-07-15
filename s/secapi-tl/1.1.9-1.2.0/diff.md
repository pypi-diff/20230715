# Comparing `tmp/secapi-tl-1.1.9.tar.gz` & `tmp/secapi-tl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secapi-tl-1.1.9.tar", last modified: Mon Apr 24 07:48:09 2023, max compression
+gzip compressed data, was "secapi-tl-1.2.0.tar", last modified: Sat Jul 15 15:25:45 2023, max compression
```

## Comparing `secapi-tl-1.1.9.tar` & `secapi-tl-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.9/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)     4873 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     3434 2023-04-23 18:15:51.000000 secapi-tl-1.1.9/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-24 07:47:45.000000 secapi-tl-1.1.9/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/src/secapi_tl/
--rw-rw-r--   0 tom       (1000) tom       (1000)      307 2023-04-23 18:15:51.000000 secapi-tl-1.1.9/src/secapi_tl/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.9/src/secapi_tl/filing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4041 2023-04-23 18:15:51.000000 secapi-tl-1.1.9/src/secapi_tl/filing_query.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-04-23 16:14:09.000000 secapi-tl-1.1.9/src/secapi_tl/key_mapper.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      916 2023-04-24 07:47:07.000000 secapi-tl-1.1.9/src/secapi_tl/request.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 07:48:09.373637 secapi-tl-1.1.9/src/secapi_tl.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     4873 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-24 07:48:09.000000 secapi-tl-1.1.9/src/secapi_tl.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-15 15:25:45.695405 secapi-tl-1.2.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.2.0/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6851 2023-07-15 15:25:45.695405 secapi-tl-1.2.0/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5412 2023-07-15 15:16:16.000000 secapi-tl-1.2.0/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-07-15 00:02:42.000000 secapi-tl-1.2.0/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-07-15 15:25:45.695405 secapi-tl-1.2.0/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-15 15:25:45.695405 secapi-tl-1.2.0/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-15 15:25:45.695405 secapi-tl-1.2.0/src/secapi_tl/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      561 2023-07-15 15:09:46.000000 secapi-tl-1.2.0/src/secapi_tl/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2554 2023-07-15 14:12:22.000000 secapi-tl-1.2.0/src/secapi_tl/request.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6233 2023-07-14 22:00:51.000000 secapi-tl-1.2.0/src/secapi_tl/submission.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4770 2023-07-15 15:04:20.000000 secapi-tl-1.2.0/src/secapi_tl/submission_query.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2473 2023-07-14 22:00:51.000000 secapi-tl-1.2.0/src/secapi_tl/utility_functions.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-15 15:25:45.695405 secapi-tl-1.2.0/src/secapi_tl.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6851 2023-07-15 15:25:45.000000 secapi-tl-1.2.0/src/secapi_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      364 2023-07-15 15:25:45.000000 secapi-tl-1.2.0/src/secapi_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-07-15 15:25:45.000000 secapi-tl-1.2.0/src/secapi_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-07-15 15:25:45.000000 secapi-tl-1.2.0/src/secapi_tl.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-07-15 15:25:45.000000 secapi-tl-1.2.0/src/secapi_tl.egg-info/top_level.txt
```

### Comparing `secapi-tl-1.1.9/LICENSE` & `secapi-tl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.9/src/secapi_tl/filing.py` & `secapi-tl-1.2.0/src/secapi_tl/submission.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 from datetime import datetime
 from datetime import date
 
 
-class Filing:
+class Submission:
     """
-    The filing class contains all the metadata of a filing.
-    It is used to store the filings metadata in a uniform format.
+    The submission class stores all metadata of a submission.
+    It is used to store the submission metadata in a uniform format.
     """
 
     def __init__(self,
                  accession_number: str = None,
                  ticker_symbol: str = None,
                  cik: str = None,
                  filing_date: date = None,
@@ -56,27 +56,27 @@
         self._size: int = size
         self._is_xbrl: bool = is_xbrl
         self._is_inline_xbrl: bool = is_inline_xbrl
         self._primary_document: str = primary_document
         self._primary_doc_description: str = primary_doc_description
 
     @staticmethod
-    def from_dict(filing_dict: dict) -> Filing:
+    def _from_dict(filing_dict: dict) -> Submission:
         """
-        Creates a filing object from the json that is returned by the web request to the sec server.
+        Creates a submission object from the json that is returned by the web request to the sec server.
         The values are converted to appropriate python types.
         """
-        accession_number: str = filing_dict.get('accessionNumber')
+        accession_number: str = str(filing_dict.get('accessionNumber'))
         filing_date: date = datetime.strptime(filing_dict.get("filingDate"), '%Y-%m-%d').date()
         if filing_dict.get("reportDate") == '':
             report_date = None
         else:
             report_date: date = datetime.strptime(filing_dict.get("reportDate"), '%Y-%m-%d').date()
-        ticker_symbol: str = filing_dict.get('tickerSymbol')
-        cik: str = filing_dict.get('cik')
+        ticker_symbol: str = str(filing_dict.get('tickerSymbol'))
+        cik: str = str(filing_dict.get('cik'))
 
         datetime_str = filing_dict.get("acceptanceDateTime")
         datetime_str = datetime_str.replace("T", " ")
         datetime_str = datetime_str.replace(".000Z", "")
         acceptance_date_time: datetime = datetime.strptime(datetime_str, "%Y-%m-%d %H:%M:%S")
 
         act: str = filing_dict.get('act')
@@ -88,30 +88,30 @@
 
         is_xbrl: bool = bool(filing_dict.get('isXBRL'))
         is_inline_xbrl: bool = bool(filing_dict.get('isInlineXBRL'))
 
         primary_document: str = filing_dict.get('primaryDocument')
         primary_doc_description: str = filing_dict.get('primaryDocDescription')
 
-        return Filing(accession_number=accession_number,
-                      ticker_symbol=ticker_symbol,
-                      cik=cik,
-                      filing_date=filing_date,
-                      report_date=report_date,
-                      acceptance_date_time=acceptance_date_time,
-                      act=act,
-                      form=form,
-                      file_number=file_number,
-                      film_number=film_number,
-                      items=items,
-                      size=size,
-                      is_xbrl=is_xbrl,
-                      is_inline_xbrl=is_inline_xbrl,
-                      primary_document=primary_document,
-                      primary_doc_description=primary_doc_description)
+        return Submission(accession_number=accession_number,
+                          ticker_symbol=ticker_symbol,
+                          cik=cik,
+                          filing_date=filing_date,
+                          report_date=report_date,
+                          acceptance_date_time=acceptance_date_time,
+                          act=act,
+                          form=form,
+                          file_number=file_number,
+                          film_number=film_number,
+                          items=items,
+                          size=size,
+                          is_xbrl=is_xbrl,
+                          is_inline_xbrl=is_inline_xbrl,
+                          primary_document=primary_document,
+                          primary_doc_description=primary_doc_description)
 
     @property
     def accession_number(self) -> str:
         return self._accession_number
 
     @property
     def ticker_symbol(self) -> str:
```

### Comparing `secapi-tl-1.1.9/src/secapi_tl/filing_query.py` & `secapi-tl-1.2.0/src/secapi_tl/submission_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import List
-from warnings import warn
+from typing import List, Union
 from openDateRange import DateRange
+import re
 
 from .request import sec_request
-from .key_mapper import get_cik
-from .filing import Filing
+from .utility_functions import ticker_to_cik
+from .submission import Submission
 
-# list of keys for all existing metadata points
+
+# list of existing metadata points for a submission
 FILING_INFORMATION_KEYS = ['accessionNumber',
                            'filingDate',
                            'reportDate',
                            'acceptanceDateTime',
                            'act',
                            'form',
                            'fileNumber',
@@ -18,83 +19,99 @@
                            'items',
                            'size',
                            'isXBRL',
                            'isInlineXBRL',
                            'primaryDocument',
                            'primaryDocDescription']
 
+DATE_FORMAT = '%Y-%m-%d'
 JSON_FILE = ".json"
 BASE_URL_SUBMISSIONS = r'https://data.sec.gov/submissions/'
 
 CIK_STRING = r'CIK'
 REQUIRED_CIK_LENGTH = 10
+CIK_REGEX = re.compile('\d{0,10}')
 
 
-def get_filings(ticker_symbol: str,
-                date_from: str = None,
-                date_to: str = None,
-                form_types: List[str] = None,
-                filing_information: List[str] = None) -> List[Filing]:
+def get_submissions(ticker_symbol_or_cik: str,
+                    date_from: str = None,
+                    date_to: str = None,
+                    form_types: Union[List[str], str] = None) -> List[Submission]:
     """
-    This method returns the metadata for all filings of the given form types that belong to the company
-    with the given ticker and have been filed within the given daterange.
-    The returned metadata only contains the datapoints given in the filing_information parameter.
-    The ticker symbol is the only information that must be given.
-    If the form_type parameter is set to None all form types will be returned.
-    If the filing_information parameter is set to None all metadata points will be returned.
+    Returns a list of submissions that match the given parameters.
+    The parameters are used to create a query to the sec server and filter the data afterward.
+    The function accesses the https://data.sec.gov/submissions/ endpoint as it recommended by the sec.
+
+    !!!
+    It can happen that a TooManyRequestsError is raised. This happens when the https://data.sec.gov/submissions/
+    endpoint is overloaded. The SEC returns a 429 status code in this case. Requests to other endpoints are not blocked
+    since the method uses the sec_request function and thus the allowed request limit is not exceeded. You may need to
+    implement your own strategy to handle this error since this error depends strongly on the usage of this function.
+    !!!
+
+    :param ticker_symbol_or_cik: ticker symbol or cik of the company cik should be a string
+    :param date_from: the date from which the submissions should be returned "YYYY-MM-DD"
+    :param date_to: the date to which the submissions should be returned "YYYY-MM-DD"
+    :param form_types: submission form types that should be returned. Valid form types are all form types that
+                     are used by the sec for submissions.
+    :return: the list of Submission instances each instance contains the data for one submission
     """
 
+    format_before = DateRange.DATE_FORMAT
+    DateRange.DATE_FORMAT = DATE_FORMAT
     search_daterange = DateRange(date_from=date_from, date_to=date_to)
+    DateRange.DATE_FORMAT = format_before
+
+    if isinstance(form_types, str):
+        form_types = [form_types]
     checker = create_filing_checker(search_daterange, form_types)
-    if filing_information is None:
-        information_keys = FILING_INFORMATION_KEYS
-    else:
-        information_keys = [i for i in FILING_INFORMATION_KEYS if i in filing_information]
-        # proofs if the filing_information parameter contains metadata points that do not exist
-        if len(information_keys) < len(filing_information):
-            warn("filing_information list contains key that does not exist")
 
     # get the main submissions file
-    cik = get_cik(ticker_symbol)
+    # the ticker symbol can also be a cik
+    if CIK_REGEX.fullmatch(ticker_symbol_or_cik):
+        cik = ticker_symbol_or_cik
+    else:
+        cik = ticker_to_cik(ticker_symbol_or_cik)
     length_diff = REQUIRED_CIK_LENGTH - len(cik)
     cik_formatted = ('0' * length_diff) + cik
     submissions_url = BASE_URL_SUBMISSIONS + CIK_STRING + cik_formatted + JSON_FILE
 
     response = sec_request(url=submissions_url)
     submissions_dict = response.json()
 
     filings = []
     # parse recent
     data = submissions_dict['filings']['recent']
     if search_daterange.intersects(date_from=data['filingDate'][-1], date_to=data['filingDate'][0]):
-        filings += filter_filings(data, checker, information_keys, cik, ticker_symbol)
+        filings += filter_filings(data, checker, cik, ticker_symbol_or_cik)
 
     # parse files
     files = submissions_dict['filings']['files']
     for file in files:
         if search_daterange.intersects(date_from=file['filingFrom'], date_to=file['filingTo']):
             url = BASE_URL_SUBMISSIONS + file['name']
             response = sec_request(url=url)
             data = response.json()
-            filings += filter_filings(data, checker, information_keys, cik, ticker_symbol)
+            filings += filter_filings(data, checker, cik, ticker_symbol_or_cik)
 
-    return [Filing.from_dict(filing_dict=filing) for filing in filings]
+    return [Submission._from_dict(filing_dict=filing) for filing in filings]
 
 
-def filter_filings(raw_filings, checker, required_information, cik, ticker_symbol):
+def filter_filings(raw_filings, checker, cik, ticker_symbol):
     filings = []
 
     dates = raw_filings['filingDate']
     forms = raw_filings['form']
     for i, (date, form) in enumerate(zip(dates, forms)):
         if checker(date, form):
             filing = {'tickerSymbol': ticker_symbol.upper(), 'cik': cik}
-            for key in required_information:
+            for key in FILING_INFORMATION_KEYS:
                 filing[key] = raw_filings[key][i]
             filings.append(filing)
     return filings
 
 
 def create_filing_checker(date_range, form_types):
     def filing_checker(filing_date, form):
         return filing_date in date_range and (form_types is None or form in form_types)
+
     return filing_checker
```

