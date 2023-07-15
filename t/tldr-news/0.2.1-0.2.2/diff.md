# Comparing `tmp/tldr_news-0.2.1.tar.gz` & `tmp/tldr_news-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldr_news-0.2.1.tar", max compression
+gzip compressed data, was "tldr_news-0.2.2.tar", max compression
```

## Comparing `tldr_news-0.2.1.tar` & `tldr_news-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1046 2023-07-15 05:01:12.864621 tldr_news-0.2.1/README.md
--rw-r--r--   0        0        0     1195 2023-07-15 05:01:39.537379 tldr_news-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-15 05:01:39.537379 tldr_news-0.2.1/tldr_news/__init__.py
--rw-r--r--   0        0        0     1081 2023-07-15 05:01:12.868622 tldr_news-0.2.1/tldr_news/cli.py
--rw-r--r--   0        0        0      204 2023-07-15 05:01:12.872622 tldr_news-0.2.1/tldr_news/main.css
--rw-r--r--   0        0        0      698 2023-07-15 05:01:12.872622 tldr_news-0.2.1/tldr_news/ui.py
--rw-r--r--   0        0        0     1873 2023-07-15 05:01:12.872622 tldr_news-0.2.1/tldr_news/utils.py
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 tldr_news-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1046 2023-07-15 08:58:40.442652 tldr_news-0.2.2/README.md
+-rw-r--r--   0        0        0     1195 2023-07-15 08:59:05.071240 tldr_news-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-15 08:59:05.071240 tldr_news-0.2.2/tldr_news/__init__.py
+-rw-r--r--   0        0        0     1081 2023-07-15 08:58:40.446652 tldr_news-0.2.2/tldr_news/cli.py
+-rw-r--r--   0        0        0      204 2023-07-15 08:58:40.446652 tldr_news-0.2.2/tldr_news/main.css
+-rw-r--r--   0        0        0      698 2023-07-15 08:58:40.446652 tldr_news-0.2.2/tldr_news/ui.py
+-rw-r--r--   0        0        0     1810 2023-07-15 08:58:40.446652 tldr_news-0.2.2/tldr_news/utils.py
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 tldr_news-0.2.2/PKG-INFO
```

### Comparing `tldr_news-0.2.1/README.md` & `tldr_news-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.1/pyproject.toml` & `tldr_news-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tldr-news"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Harry Tran <huytran.quang080199@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tldr_news"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tldr_news-0.2.1/tldr_news/cli.py` & `tldr_news-0.2.2/tldr_news/cli.py`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.1/tldr_news/ui.py` & `tldr_news-0.2.2/tldr_news/ui.py`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.1/tldr_news/utils.py` & `tldr_news-0.2.2/tldr_news/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,28 +18,25 @@
     icon_headers = soup.find_all("div", class_="text-3xl")
     text_headers = soup.find_all("h6")
     headers = [icon_header.contents[0] + " " + text_header.contents[0]
                for icon_header, text_header in zip(icon_headers, text_headers)]
     list_contents = soup.find_all("div", class_="mt-3")
     header_index = 0
     output = ""
-    output += title.contents[0] + "\n\n"
-    output += summary.contents[0] + "\n\n"
+    output += f"{title.contents[0]} \n\n {summary.contents[0]} \n\n"
     news_index = 1
     for list_content in list_contents[1:]:
         if list_content.find("h3"):
             output += str(news_index) + ". " + \
-                list_content.find("h3").contents[0] + "\n"
-            output += '-' * 50 + "\n"
+                list_content.find("h3").contents[0] + "\n" + '-' * 50 + "\n"
             news_index += 1
-        else:
-            if header_index < len(headers):
-                output += headers[header_index] + "\n\n"
-                header_index += 1
-                news_index = 1
+        elif header_index < len(headers):
+            output += headers[header_index] + "\n\n"
+            header_index += 1
+            news_index = 1
         if list_content.find("div"):
             print(list_content.find("div"))
             output += list_content.find("div").contents[0] + "\n\n"
     return output
 
 
 def get_days():
```

### Comparing `tldr_news-0.2.1/PKG-INFO` & `tldr_news-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldr-news
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Harry Tran
 Author-email: huytran.quang080199@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

