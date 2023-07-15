# Comparing `tmp/notion-graph-0.2.5.tar.gz` & `tmp/notion-graph-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-graph-0.2.5.tar", last modified: Sun Jul  2 11:55:38 2023, max compression
+gzip compressed data, was "notion-graph-0.2.6.tar", last modified: Sat Jul 15 02:45:11 2023, max compression
```

## Comparing `notion-graph-0.2.5.tar` & `notion-graph-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.5/LICENSE
--rw-r--r--   0        0        0     3451 2023-07-02 11:40:22.213830 notion-graph-0.2.5/README.md
--rw-r--r--   0        0        0      636 2023-07-02 09:44:33.956068 notion-graph-0.2.5/notion_graph/__init__.py
--rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.5/notion_graph/__main__.py
--rw-r--r--   0        0        0      641 2023-07-02 09:44:33.956068 notion-graph-0.2.5/notion_graph/cli.py
--rw-r--r--   0        0        0      426 2023-07-02 09:44:33.956068 notion-graph-0.2.5/notion_graph/helper.py
--rw-r--r--   0        0        0    12242 2023-07-02 11:55:19.633539 notion-graph-0.2.5/notion_graph/parser.py
--rw-r--r--   0        0        0      497 2023-07-02 11:53:13.083580 notion-graph-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 notion-graph-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3454 2023-07-09 14:58:23.798405 notion-graph-0.2.6/README.md
+-rw-r--r--   0        0        0      636 2023-07-02 09:44:33.956068 notion-graph-0.2.6/notion_graph/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.6/notion_graph/__main__.py
+-rw-r--r--   0        0        0      641 2023-07-02 09:44:33.956068 notion-graph-0.2.6/notion_graph/cli.py
+-rw-r--r--   0        0        0      426 2023-07-02 09:44:33.956068 notion-graph-0.2.6/notion_graph/helper.py
+-rw-r--r--   0        0        0    13792 2023-07-15 02:43:16.856958 notion-graph-0.2.6/notion_graph/parser.py
+-rw-r--r--   0        0        0      497 2023-07-15 02:44:58.536921 notion-graph-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 notion-graph-0.2.6/PKG-INFO
```

### Comparing `notion-graph-0.2.5/LICENSE` & `notion-graph-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.5/README.md` & `notion-graph-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 ### Notion API Setup
 
 1. Create a [notion internal integration](https://www.notion.so/my-integrations) and generate an `Internal Integration Token`.
 
    👉 [Learn more about authorization](https://developers.notion.com/docs/authorization)
 
-2. Open one notion page on browser, select "Add connections" and add your integration account.
-3. Find your base `Page ID` from browser url, for example:
+2. Open one notion page on the browser, select "Add connections" and add your integration account.
+3. Find your base `Page `ID` from the browser URL, for example:
 
 > if page url is: https://www.notion.so/yourName/PageTitle-8a4b5ff100d648fb8d39d4bfa756ff3f, `8a4b5ff100da48fb8d39d4bfa756ff3f` is the `Page ID`
 
 ### Quickly Running
 
 ```shell
 python -m notion_graph -p <Page ID> -t <Integration Token> -o <file path to export>
@@ -43,15 +43,15 @@
 
 `graph_out.html` would be generated at your specific path.
 
 ### Importing as a Python Library
 
 You can also import `notion_graph` as a library.
 
-For instance, drawing your own diagram in Jupyter Notebook.
+For instance, draw your diagram in Jupyter Notebook.
 
 ```python
 import notion_graph as ng
 
 my_ng = ng.NotionGraph(bearer_token="secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e")
 network = my_ng.parse(page_id="856391c93ae64bd1b7ebf699ca0cd861")
 # `network` is a `pyvis.network.Network` object, see more attributes: https://pyvis.readthedocs.io/en/latest/documentation.html
@@ -60,15 +60,15 @@
 network.prep_notebook()
 
 network.show("graph.html")
 ```
 
 ## Testing Environment
 
-The testing page is [Notion-grap-view-demo](https://sund.notion.site/Notion-graph-view-Demo-856391c93ae64bd1b7ebf699ca0cd861). You can duplicate the page to your Notion account and run the project to test if everything goes well.
+The testing page is [Notion-graph-view-demo](https://sund.notion.site/Notion-graph-view-Demo-856391c93ae64bd1b7ebf699ca0cd861). You can duplicate the page to your Notion account and run the project to test if everything goes well.
 
 ## Development Guide
 
 This project's dependencies are managed by [PDM](https://pdm.fming.dev/latest/).
 
 ```shell
 brew install pdm
```

### Comparing `notion-graph-0.2.5/notion_graph/__init__.py` & `notion-graph-0.2.6/notion_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.5/notion_graph/cli.py` & `notion-graph-0.2.6/notion_graph/cli.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.5/notion_graph/parser.py` & `notion-graph-0.2.6/notion_graph/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 rich_text | title -> mention objects
 relation object -> page titles
 mention object -> database title | page title
 column_list -> column -> block
 table -> table_row -> block
 '''
 
-from notion_client import Client, APIResponseError
+import time
+from notion_client import Client, APIResponseError, APIErrorCode
 from pyvis.network import Network
 from .helper import contains_mention_or_relation_type, is_same_block_id
 
 __all__ = ["Parser"]
 
 # All heading blocks("heading_1", "heading_2", and "heading_3") support children when the is_toggleable property is true.
 SUPPORTED_BLOCK_TYPES = [
@@ -37,50 +38,64 @@
                               height="750px",
                               width="100%",
                               cdn_resources="in_line",
                               select_menu=True,
                               )
 
     def parse(self, root_id: str) -> Network:
+        print('Parsing ...')
         self._parse_block(root_id)
+        print('Prasing ... done')
         return self._graph
 
     def export_to_html(self, file_path: str):
-        print('Graph is generated at:', file_path, end='\r', flush=True)
+        print('Graph is generated at:', file_path)
         self._graph.repulsion(node_distance=200, spring_length=200)
         self._graph.show(file_path)
 
     def _parse_block(self, root_id: str, obj: dict = None) -> None:
         if obj is None:
             try:
                 obj = self._notion.blocks.retrieve(root_id)
             except APIResponseError:
-                return
+                if APIResponseError.code == APIErrorCode.RateLimited:
+                    time.sleep(1)
+                    obj = self._notion.blocks.retrieve(root_id)
+                else:
+                    return
 
         self._parse_block_object(obj, root_id)
 
     def _parse_database(self, id: str, obj: dict = None, parent_page_or_database_id: str = None) -> None:
         if obj is None:
             try:
                 obj = self._notion.databases.retrieve(id)
             except APIResponseError:
-                return
+                if APIResponseError.code == APIErrorCode.RateLimited:
+                    time.sleep(1)
+                    obj = self._notion.databases.retrieve(id)
+                else:
+                    return
 
         if obj['archived']:
             return
 
         self._retrieve_page_or_database_title(id, parent_page_or_database_id)
         self._parse_database_pages(id)
 
     def _parse_page(self, id: str, obj: dict = None, parent_page_or_database_id: str = None) -> None:
         if obj is None:
             try:
                 obj = self._notion.pages.retrieve(id)
             except APIResponseError:
-                return
+                if APIResponseError.code == APIErrorCode.RateLimited:
+                    time.sleep(1)
+                    obj = self._notion.pages.retrieve(id)
+                else:
+                    return
 
         if obj['archived']:
             return
 
         self._retrieve_page_or_database_title(id, parent_page_or_database_id)
         self._parse_page_properties(obj['properties'], id)
 
@@ -212,27 +227,36 @@
         has_more = True
         next_cursor = None
         while has_more:
             try:
                 data = self._notion.databases.query(
                     database_id, page_size=100, start_cursor=next_cursor)
             except APIResponseError:
-                return
+                if APIResponseError.code == APIErrorCode.RateLimited:
+                    time.sleep(1)
+                    data = self._notion.databases.query(
+                        database_id, page_size=100, start_cursor=next_cursor)
+                else:
+                    return
 
             pages = data['results']
             has_more = data['has_more']
             next_cursor = data['next_cursor']
             for page in pages:
                 self._parse_page(page['id'], None, database_id)
 
     def _parse_block_children(self, block_id: str, parent_page_or_database_id: str) -> None:
         try:
             list_object = self._notion.blocks.children.list(block_id)
         except APIResponseError:
-            return
+            if APIResponseError.code == APIErrorCode.RateLimited:
+                time.sleep(1)
+                list_object = self._notion.blocks.children.list(block_id)
+            else:
+                return
 
         block_list = list_object['results']
 
         for block in block_list:
             self._parse_block_object(block, parent_page_or_database_id)
 
     def _parse_cells_metrics(self, cells_metrics: list, parent_page_or_database_id: str) -> None:
@@ -281,18 +305,21 @@
             }
         ]
         '''
         for relation_obj in relation_list:
             try:
                 block = self._notion.blocks.retrieve(relation_obj['id'])
             except APIResponseError:
-                continue
+                if APIResponseError.code == APIErrorCode.RateLimited:
+                    time.sleep(1)
+                    block = self._notion.blocks.retrieve(relation_obj['id'])
+                else:
+                    continue
 
             title = block[block['type']]['title']
-            print('Found relation node:', title, end='\r', flush=True)
             self._graph.add_node(block['id'], label=title)
             self._graph.add_edge(parent_page_or_database_id, block['id'])
 
     def _retrieve_mention_object_title(self, mention_obj: dict, parent_page_or_database_id: str):
         '''Example:
 
         {
@@ -303,26 +330,33 @@
         }
         '''
         if mention_obj['type'] == 'page':
             try:
                 block = self._notion.blocks.retrieve(
                     mention_obj[mention_obj['type']]['id'])
             except APIResponseError:
-                return
+                if APIResponseError.code == APIErrorCode.RateLimited:
+                    time.sleep(1)
+                    block = self._notion.blocks.retrieve(
+                        mention_obj[mention_obj['type']]['id'])
+                else:
+                    return
 
             title = block[block['type']]['title']
-            print('Found mention node:', title, end='\r', flush=True)
             self._graph.add_node(block['id'], label=title)
             self._graph.add_edge(parent_page_or_database_id, block['id'])
 
     def _retrieve_page_or_database_title(self, page_or_database_id: str, parent_page_or_database_id: str):
         try:
             block = self._notion.blocks.retrieve(page_or_database_id)
         except APIResponseError:
-            return
+            if APIResponseError.code == APIErrorCode.RateLimited:
+                time.sleep(1)
+                block = self._notion.blocks.retrieve(page_or_database_id)
+            else:
+                return
 
         title = block[block['type']]['title']
-        print('Found node:', title, end='\r', flush=True)
         self._graph.add_node(page_or_database_id, label=title)
         if not is_same_block_id(page_or_database_id, parent_page_or_database_id):
             self._graph.add_edge(
                 parent_page_or_database_id, page_or_database_id)
```

### Comparing `notion-graph-0.2.5/PKG-INFO` & `notion-graph-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-graph
-Version: 0.2.5
+Version: 0.2.6
 Summary: Generate a roam research like network graph view from your Notion pages.
 License: MIT
 Author-email: Steve Sun <sund.chn@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ![](images/snap.png)
@@ -29,16 +29,16 @@
 
 ### Notion API Setup
 
 1. Create a [notion internal integration](https://www.notion.so/my-integrations) and generate an `Internal Integration Token`.
 
    👉 [Learn more about authorization](https://developers.notion.com/docs/authorization)
 
-2. Open one notion page on browser, select "Add connections" and add your integration account.
-3. Find your base `Page ID` from browser url, for example:
+2. Open one notion page on the browser, select "Add connections" and add your integration account.
+3. Find your base `Page `ID` from the browser URL, for example:
 
 > if page url is: https://www.notion.so/yourName/PageTitle-8a4b5ff100d648fb8d39d4bfa756ff3f, `8a4b5ff100da48fb8d39d4bfa756ff3f` is the `Page ID`
 
 ### Quickly Running
 
 ```shell
 python -m notion_graph -p <Page ID> -t <Integration Token> -o <file path to export>
@@ -52,15 +52,15 @@
 
 `graph_out.html` would be generated at your specific path.
 
 ### Importing as a Python Library
 
 You can also import `notion_graph` as a library.
 
-For instance, drawing your own diagram in Jupyter Notebook.
+For instance, draw your diagram in Jupyter Notebook.
 
 ```python
 import notion_graph as ng
 
 my_ng = ng.NotionGraph(bearer_token="secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e")
 network = my_ng.parse(page_id="856391c93ae64bd1b7ebf699ca0cd861")
 # `network` is a `pyvis.network.Network` object, see more attributes: https://pyvis.readthedocs.io/en/latest/documentation.html
@@ -69,15 +69,15 @@
 network.prep_notebook()
 
 network.show("graph.html")
 ```
 
 ## Testing Environment
 
-The testing page is [Notion-grap-view-demo](https://sund.notion.site/Notion-graph-view-Demo-856391c93ae64bd1b7ebf699ca0cd861). You can duplicate the page to your Notion account and run the project to test if everything goes well.
+The testing page is [Notion-graph-view-demo](https://sund.notion.site/Notion-graph-view-Demo-856391c93ae64bd1b7ebf699ca0cd861). You can duplicate the page to your Notion account and run the project to test if everything goes well.
 
 ## Development Guide
 
 This project's dependencies are managed by [PDM](https://pdm.fming.dev/latest/).
 
 ```shell
 brew install pdm
```

