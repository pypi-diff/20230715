# Comparing `tmp/splatnet3_scraper-0.9.3.tar.gz` & `tmp/splatnet3_scraper-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splatnet3_scraper-0.9.3.tar", max compression
+gzip compressed data, was "splatnet3_scraper-0.9.4.tar", max compression
```

## Comparing `splatnet3_scraper-0.9.3.tar` & `splatnet3_scraper-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34915 2023-04-10 05:10:54.759478 splatnet3_scraper-0.9.3/LICENSE.md
--rw-r--r--   0        0        0    10984 2023-04-15 00:47:42.245111 splatnet3_scraper-0.9.3/README.md
--rw-r--r--   0        0        0     1916 2023-07-03 23:31:57.865780 splatnet3_scraper-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-03 23:31:57.865780 splatnet3_scraper-0.9.3/splatnet3_scraper/__init__.py
--rw-r--r--   0        0        0      271 2023-04-10 05:20:16.704543 splatnet3_scraper-0.9.3/splatnet3_scraper/auth/__init__.py
--rw-r--r--   0        0        0     3064 2023-04-10 05:20:16.704543 splatnet3_scraper-0.9.3/splatnet3_scraper/auth/environment_manager.py
--rw-r--r--   0        0        0      287 2023-04-10 05:10:54.769478 splatnet3_scraper-0.9.3/splatnet3_scraper/auth/exceptions.py
--rw-r--r--   0        0        0    10032 2023-04-14 23:55:14.106500 splatnet3_scraper-0.9.3/splatnet3_scraper/auth/graph_ql_queries.py
--rw-r--r--   0        0        0    44201 2023-07-03 19:28:53.887475 splatnet3_scraper-0.9.3/splatnet3_scraper/auth/nso.py
--rw-r--r--   0        0        0    31005 2023-07-03 21:28:37.215022 splatnet3_scraper-0.9.3/splatnet3_scraper/auth/token_manager.py
--rw-r--r--   0        0        0     7847 2023-05-26 03:02:35.840997 splatnet3_scraper-0.9.3/splatnet3_scraper/constants.py
--rw-r--r--   0        0        0      226 2023-04-10 05:20:16.704543 splatnet3_scraper-0.9.3/splatnet3_scraper/query/__init__.py
--rw-r--r--   0        0        0    13527 2023-07-03 23:31:57.865780 splatnet3_scraper-0.9.3/splatnet3_scraper/query/config.py
--rw-r--r--   0        0        0    19577 2023-07-03 21:28:18.895022 splatnet3_scraper-0.9.3/splatnet3_scraper/query/handler.py
--rw-r--r--   0        0        0    16980 2023-04-10 05:10:54.769478 splatnet3_scraper-0.9.3/splatnet3_scraper/query/json_parser.py
--rw-r--r--   0        0        0    27320 2023-07-02 23:51:51.516981 splatnet3_scraper-0.9.3/splatnet3_scraper/query/responses.py
--rw-r--r--   0        0        0      117 2023-04-10 05:10:54.769478 splatnet3_scraper-0.9.3/splatnet3_scraper/scraper/__init__.py
--rw-r--r--   0        0        0    10930 2023-07-03 19:28:53.887475 splatnet3_scraper-0.9.3/splatnet3_scraper/scraper/main.py
--rw-r--r--   0        0        0     6182 2023-04-14 04:47:23.115079 splatnet3_scraper-0.9.3/splatnet3_scraper/scraper/query_map.py
--rw-r--r--   0        0        0    18732 2023-07-03 05:07:37.608933 splatnet3_scraper-0.9.3/splatnet3_scraper/utils.py
--rw-r--r--   0        0        0    12156 1970-01-01 00:00:00.000000 splatnet3_scraper-0.9.3/setup.py
--rw-r--r--   0        0        0    11882 1970-01-01 00:00:00.000000 splatnet3_scraper-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    34915 2023-04-10 05:10:54.000000 splatnet3_scraper-0.9.4/LICENSE.md
+-rw-r--r--   0        0        0    10984 2023-04-15 00:47:42.000000 splatnet3_scraper-0.9.4/README.md
+-rw-r--r--   0        0        0     1916 2023-07-05 04:07:57.000000 splatnet3_scraper-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-05 04:08:07.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-10 05:20:16.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/auth/__init__.py
+-rw-r--r--   0        0        0     3064 2023-04-10 05:20:16.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/auth/environment_manager.py
+-rw-r--r--   0        0        0      287 2023-04-10 05:10:54.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/auth/exceptions.py
+-rw-r--r--   0        0        0    10032 2023-04-14 23:55:14.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/auth/graph_ql_queries.py
+-rw-r--r--   0        0        0    44201 2023-07-03 19:28:53.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/auth/nso.py
+-rw-r--r--   0        0        0    31005 2023-07-03 21:28:37.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/auth/token_manager.py
+-rw-r--r--   0        0        0     7847 2023-05-26 03:02:35.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/constants.py
+-rw-r--r--   0        0        0      226 2023-04-10 05:20:16.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/query/__init__.py
+-rw-r--r--   0        0        0    13527 2023-07-03 23:31:57.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/query/config.py
+-rw-r--r--   0        0        0    19577 2023-07-03 21:28:18.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/query/handler.py
+-rw-r--r--   0        0        0    16980 2023-04-10 05:10:54.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/query/json_parser.py
+-rw-r--r--   0        0        0    27331 2023-07-15 05:24:09.318214 splatnet3_scraper-0.9.4/splatnet3_scraper/query/responses.py
+-rw-r--r--   0        0        0      117 2023-04-10 05:10:54.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/scraper/__init__.py
+-rw-r--r--   0        0        0    12342 2023-07-05 04:10:36.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/scraper/main.py
+-rw-r--r--   0        0        0     6357 2023-07-04 22:43:38.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/scraper/query_map.py
+-rw-r--r--   0        0        0    18732 2023-07-03 05:07:37.000000 splatnet3_scraper-0.9.4/splatnet3_scraper/utils.py
+-rw-r--r--   0        0        0    12156 1970-01-01 00:00:00.000000 splatnet3_scraper-0.9.4/setup.py
+-rw-r--r--   0        0        0    11882 1970-01-01 00:00:00.000000 splatnet3_scraper-0.9.4/PKG-INFO
```

### Comparing `splatnet3_scraper-0.9.3/LICENSE.md` & `splatnet3_scraper-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/README.md` & `splatnet3_scraper-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/pyproject.toml` & `splatnet3_scraper-0.9.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splatnet3_scraper"
-version = "0.9.3"
+version = "0.9.4"
 description = "Scraper for SplatNet 3 for Splatoon 3"
 authors = ["Cesar E Garza <cesar@cegarza.com>"]
 readme = "README.md"
 packages = [{include = "splatnet3_scraper"}]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
```

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/auth/environment_manager.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/auth/environment_manager.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/auth/graph_ql_queries.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/auth/graph_ql_queries.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/auth/nso.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/auth/nso.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/auth/token_manager.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/auth/token_manager.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/constants.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/constants.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/query/config.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/query/config.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/query/handler.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/query/handler.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/query/json_parser.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/query/json_parser.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/query/responses.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/query/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,9 +677,9 @@
 
         Returns:
             Any: The value at the given key or the default value if the key is
                 not found.
         """
         try:
             return self[key]
-        except (KeyError, IndexError):
+        except (KeyError, IndexError, TypeError):
             return default
```

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/scraper/main.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/scraper/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,63 @@
 
         Args:
             query_handler (QueryHandler): The query handler to use.
         """
         self._query_handler = query_handler
         self.logger = logging.getLogger(__name__)
 
+    @property
+    def query_handler(self) -> QueryHandler:
+        """The query handler used by the scraper.
+
+        Returns:
+            QueryHandler: The query handler.
+        """
+        return self._query_handler
+
     @staticmethod
     def from_session_token(session_token: str) -> "SplatNet_Scraper":
         """Creates a SplatNet_Scraper instance using the given session token.
 
         Args:
             session_token (str): The session token to use.
 
         Returns:
             SplatNet_Scraper: The SplatNet_Scraper instance.
         """
         query_handler = QueryHandler.from_session_token(session_token)
         return SplatNet_Scraper(query_handler)
 
     @staticmethod
+    def from_tokens(
+        session_token: str,
+        gtoken: str | None = None,
+        bullet_token: str | None = None,
+    ) -> "SplatNet_Scraper":
+        """Creates a SplatNet_Scraper instance using the given tokens. This is
+        useful if you already have the tokens and don't want to have to
+        retrieve them again. This does not guarantee that the tokens are valid,
+        that will be checked when the first query is run.
+
+        Args:
+            session_token (str): The session token to use.
+            gtoken (str | None): The gtoken to use. If None, it will be
+                retrieved from the session token. Defaults to None.
+            bullet_token (str | None): The bullet token to use. If None, it
+                will be retrieved from the session token. Defaults to None.
+
+        Returns:
+            SplatNet_Scraper: The SplatNet_Scraper instance.
+        """
+        query_handler = QueryHandler.from_tokens(
+            session_token, gtoken, bullet_token
+        )
+        return SplatNet_Scraper(query_handler)
+
+    @staticmethod
     def from_config_file(config_path: str | None = None) -> "SplatNet_Scraper":
         """Creates a SplatNet_Scraper instance using the given config file.
 
         Args:
             config_path (str | None): The path to the config file. If None, it
                 will look for ".splatnet3_scraper" in the current working
                 directory.
@@ -123,14 +158,15 @@
         """
         if query not in (
             QueryMap.SALMON,
             QueryMap.TURF,
             QueryMap.ANARCHY,
             QueryMap.XBATTLE,
             QueryMap.PRIVATE,
+            QueryMap.CHALLENGE,
         ):
             raise ValueError(f"Invalid query: {query}")
 
         if query in (QueryMap.SALMON, QueryMap.SALMON_DETAIL):
             detail_query = QueryMap.SALMON_DETAIL
             variable_name = "coopHistoryDetailId"
         else:
@@ -184,59 +220,60 @@
             detailed_game = self.__query(detail_query, variables)
             out.append(detailed_game)
             if progress_callback is not None:
                 progress_callback(idx + 1, len(queue))
         return summary_query, out
 
     @overload
-    def get_vs_battles(
+    def get_matches(
         self,
         mode: str,
         detail: Literal[False],
         limit: int | None = None,
         existing_ids: list[str] | str | None = None,
         progress_callback: Callable[[int, int], None] | None = None,
     ) -> QueryResponse:
         ...
 
     @overload
-    def get_vs_battles(
+    def get_matches(
         self,
         mode: str,
         detail: Literal[True],
         limit: int | None = None,
         existing_ids: list[str] | str | None = None,
         progress_callback: Callable[[int, int], None] | None = None,
     ) -> tuple[QueryResponse, list[QueryResponse]]:
         ...
 
     @overload
-    def get_vs_battles(
+    def get_matches(
         self,
         mode: str,
         detail: bool = False,
         limit: int | None = None,
         existing_ids: list[str] | str | None = None,
         progress_callback: Callable[[int, int], None] | None = None,
     ) -> QueryResponse | tuple[QueryResponse, list[QueryResponse]]:
         ...
 
-    def get_vs_battles(
+    def get_matches(
         self,
         mode: str,
         detail: bool = False,
         limit: int | None = None,
         existing_ids: list[str] | str | None = None,
         progress_callback: Callable[[int, int], None] | None = None,
     ) -> QueryResponse | tuple[QueryResponse, list[QueryResponse]]:
-        """Gets the vs battles.
+        """Gets matches for the given mode.
 
         Args:
-            mode (str): The mode to get the battles for. Some values are:
-                "turf", "anarchy", "xbattle", "private",
+            mode (str): The mode to get the battles for. Valid values are:
+                "turf", "anarchy", "xbattle", "private", "challenge",
+                and "salmon".
             detail (bool): Whether to get the detailed results or not.
                 Defaults to False.
             limit (int | None): The maximum number of battles to get. If None,
                 it will get all battles. Defaults to None.
             existing_ids (list[str] | str | None): The existing IDs to check
                 against. If a string is passed, it will return the results
                 upon finding the first match. If a list is passed, it will
@@ -254,37 +291,39 @@
                 the value of detail.
             (list[QueryResponse]): The list of detailed query responses
                 associated with each battle until the limit is reached. Only
                 returned if detail is True, along with the summary query
                 response.
         """
         mapped_query = QueryMap.get(mode)
-        if mapped_query == QueryMap.SALMON:
-            raise ValueError("Use get_coop_battles for salmon run battles.")
 
         if mapped_query in (
             QueryMap.TURF_DETAIL,
             QueryMap.ANARCHY_DETAIL,
             QueryMap.XBATTLE_DETAIL,
             QueryMap.PRIVATE_DETAIL,
+            QueryMap.CHALLENGE_DETAIL,
         ):
             non_detail_map = {
                 QueryMap.TURF_DETAIL: QueryMap.TURF,
                 QueryMap.ANARCHY_DETAIL: QueryMap.ANARCHY,
                 QueryMap.XBATTLE_DETAIL: QueryMap.XBATTLE,
                 QueryMap.PRIVATE_DETAIL: QueryMap.PRIVATE,
+                QueryMap.CHALLENGE_DETAIL: QueryMap.CHALLENGE,
             }
             mapped_query = non_detail_map[mapped_query]
             detail = True
 
         if mapped_query not in (
             QueryMap.TURF,
             QueryMap.ANARCHY,
             QueryMap.XBATTLE,
             QueryMap.PRIVATE,
+            QueryMap.SALMON,
+            QueryMap.CHALLENGE,
         ):
             raise ValueError(f"Invalid mode: {mode}")
 
         if detail:
             return self.__detailed_vs_or_coop(
                 mapped_query, limit, existing_ids, progress_callback
             )
```

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/scraper/query_map.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/scraper/query_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,22 +116,26 @@
     XBATTLE = "XBattleHistoriesQuery"
     PRIVATE = "PrivateBattleHistoriesQuery"
     LATEST = "LatestBattleHistoriesQuery"
     SALMON = "CoopHistoryQuery"
     SALMON_RUN = "CoopHistoryQuery"
     TURF = "RegularBattleHistoriesQuery"
     COOP = "CoopHistoryQuery"
+    CHALLENGE = "EventBattleHistoriesQuery"
+    EVENT = "EventBattleHistoriesQuery"
     ANARCHY_DETAIL = "VsHistoryDetailQuery"
     TURF_DETAIL = "VsHistoryDetailQuery"
     REGULAR_DETAIL = "VsHistoryDetailQuery"
     X_DETAIL = "VsHistoryDetailQuery"
     XBATTLE_DETAIL = "VsHistoryDetailQuery"
     PRIVATE_DETAIL = "VsHistoryDetailQuery"
     LATEST_DETAIL = "VsHistoryDetailQuery"
     COOP_DETAIL = "CoopHistoryDetailQuery"
+    SALMON_DETAIL = "CoopHistoryDetailQuery"
+    CHALLENGE_DETAIL = "VsHistoryDetailQuery"
 
     @staticmethod
     def get(query: str) -> str:
         """Gets the query from the query map.
 
         Args:
             query (str): The query to get.
```

### Comparing `splatnet3_scraper-0.9.3/splatnet3_scraper/utils.py` & `splatnet3_scraper-0.9.4/splatnet3_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.9.3/setup.py` & `splatnet3_scraper-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'examples': ['pandas[examples]>=1.5.3,<2.0.0',
               'sqlalchemy[examples]>=2.0.1,<3.0.0',
               'psycopg2[examples]>=2.9.5,<3.0.0'],
  'parquet': ['pyarrow[parquet]>=10.0.1,<11.0.0']}
 
 setup_kwargs = {
     'name': 'splatnet3-scraper',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Scraper for SplatNet 3 for Splatoon 3',
     'long_description': '# SplatNet 3 Scraper\n\n[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.\n\n**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.\n\n## Table of Contents\n\n1. [Features](#features)\n2. [Documentation](#documentation)\n3. [Installation](#installation)\n4. [Usage](#usage)\n   - [Using the `scraper` module](#using-the-scraper-module)\n   - [Using the `query` module](#using-the-query-module)\n   - [Using the `auth` module](#using-the-auth-module)\n5. [Roadmap](#roadmap)\n6. [Contributing](#contributing)\n7. [License](#license)\n\n## Features\n\n- Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.\n- The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.\n- The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.\n- The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.\n- Compatibility with the configuration file format used by `s3s`.\n- Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:\n  - JSON\n  - gzip-compressed JSON\n  - csv\n  - parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n- Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).\n\n## Documentation\n\nDetailed documentation for SplatNet 3 Scraper, including usage instructions, examples, and API reference, is available on Read the Docs:\n\n[**SplatNet 3 Scraper Documentation**](https://splatnet3-scraper.readthedocs.io/en/latest/index.html)\n\nWe highly recommend referring to the documentation to get the most out of SplatNet 3 Scraper and understand its full capabilities.\n\n## Installation\n\n**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:\n\n```bash\npip install splatnet3_scraper\n```\n\nNote that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.\n\n## Usage\n\nThere are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can\'t find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.\n\n### Using the `scraper` module\n\nThe `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.\n\nThis module is currently under active development and is not yet complete. Please check back later for more functions.\n\n### Using the `query` module\n\nThe `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.\n\nThe `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.\n\n### Using the `auth` module\n\n:warning: **Warning: The `auth` module is intended for advanced users only. Most users should use the `scraper` or `query` modules for a simpler and more convenient experience.**\n\nThe `auth` module provides a low-level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication and is designed for advanced developers who need full control over the authentication process.\n\nTo use the `auth` module, you will need to import the necessary components and handle the authentication flow manually. Please refer to the [documentation](https://splatnet3-scraper.readthedocs.io/en/latest/index.html) for detailed instructions and examples on how to use the `auth` module.\n\n#### Instantiating the `QueryHandler` class by providing a session token\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_session_token("session_token")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by providing the path to a configuration file\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_config_file(".splatnet3_scraper")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by loading environment variables\n\nThe following environment variables are supported:\n\n- `SN3S_SESSION_TOKEN`\n- `SN3S_GTOKEN`\n- `SN3S_BULLET_TOKEN`\n\n```python\nfrom splatnet3_scrape.query import QueryHandler\nhandler = QueryHandler.from_env()\nhandler.query("StageScheduleQuery")\n```\n\n#### Querying the SplatNet 3 API\n\nThe `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nprint(response["xSchedules", "nodes", 0, "vsRule", "name"])\n```\n\n#### Saving and loading responses\n\nThe `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:\n\n- JSON\n- gzip-compressed JSON\n- csv\n- parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n\nNote: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.\n\nThe following code will save the response data to a file named `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nresponse.parsed_json().to_json("response.json")\n```\n\nAdditionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import JSONParser\nparser = JSONParser.from_json("response.json")\n```\n\n## Symbols\n\n| Symbol | Meaning |\n| ------ | ------- |\n| :white_check_mark: | Implemented |\n| :construction: | In progress |\n| :world_map: | Planned |\n| :x: | Not planned |\n\n## Roadmap\n\n| Feature | Status |\n| ------- | ------ |\n| Support for the SplatNet 3 API | :white_check_mark: |\n| Full support for the SplatNet 3 API | :white_check_mark: |\n| Support for the SplatNet 2 API | :x: |\n| Obtaining session tokens | :white_check_mark: |\n| Full documentation | :white_check_mark: |\n| Full unit test coverage | :white_check_mark: |\n| Columnar data format support | :construction: |\n| CLI interface | :x: |\n| Integration with stat.ink | :x: |\n| PyPI package | :white_check_mark: |\n| Docker image | :world_map: |\n| Executable binary | :x: |\n\n## Contributing\n\nWe welcome contributions to SplatNet 3 Scraper! For detailed information on how to contribute, please refer to our [CONTRIBUTING.md](./CONTRIBUTING.md) file.\n\nTo report issues or request new features, please open an issue on the GitHub repository.\n\n## License\n\nSplatNet 3 Scraper is licensed under the GPLv3. See the [LICENSE](./LICENSE) file for more details.\n',
     'author': 'Cesar E Garza',
     'author_email': 'cesar@cegarza.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `splatnet3_scraper-0.9.3/PKG-INFO` & `splatnet3_scraper-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splatnet3-scraper
-Version: 0.9.3
+Version: 0.9.4
 Summary: Scraper for SplatNet 3 for Splatoon 3
 License: GPL-3.0-or-later
 Author: Cesar E Garza
 Author-email: cesar@cegarza.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

