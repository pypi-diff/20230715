# Comparing `tmp/atwiki-python-0.0.8.tar.gz` & `tmp/atwiki-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atwiki-python-0.0.8.tar", last modified: Thu Sep 15 14:43:47 2022, max compression
+gzip compressed data, was "dist/atwiki-python-0.0.9.tar", last modified: Mon Sep 19 07:36:49 2022, max compression
```

## Comparing `atwiki-python-0.0.8.tar` & `atwiki-python-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-15 14:43:47.163855 atwiki-python-0.0.8/
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     1065 2022-01-26 13:03:41.000000 atwiki-python-0.0.8/LICENSE
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     3221 2022-09-15 14:43:47.163855 atwiki-python-0.0.8/PKG-INFO
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     2410 2022-09-15 14:39:48.000000 atwiki-python-0.0.8/README.rst
-drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-15 14:43:47.163855 atwiki-python-0.0.8/atwiki/
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)      167 2022-01-20 14:57:13.000000 atwiki-python-0.0.8/atwiki/__init__.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       20 2022-09-15 14:18:06.000000 atwiki-python-0.0.8/atwiki/_version.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     4010 2022-08-28 08:26:13.000000 atwiki-python-0.0.8/atwiki/core.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     2975 2022-01-20 14:57:13.000000 atwiki-python-0.0.8/atwiki/parser.py
-drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-15 14:43:47.163855 atwiki-python-0.0.8/atwiki/test/
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       52 2022-01-20 14:57:13.000000 atwiki-python-0.0.8/atwiki/test/__init__.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     4299 2022-09-15 14:39:35.000000 atwiki-python-0.0.8/atwiki/test/test_core.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     1038 2022-04-23 08:19:07.000000 atwiki-python-0.0.8/atwiki/test/test_parser.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     3388 2022-09-15 14:39:35.000000 atwiki-python-0.0.8/atwiki/test/test_uri.py
-drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-15 14:43:47.163855 atwiki-python-0.0.8/atwiki/test/tools/
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)        0 2022-01-20 14:57:13.000000 atwiki-python-0.0.8/atwiki/test/tools/__init__.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)      372 2022-01-20 14:57:13.000000 atwiki-python-0.0.8/atwiki/test/tools/test_dump.py
-drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-15 14:43:47.163855 atwiki-python-0.0.8/atwiki/tools/
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)        0 2022-01-20 14:57:13.000000 atwiki-python-0.0.8/atwiki/tools/__init__.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     1877 2022-01-20 14:57:13.000000 atwiki-python-0.0.8/atwiki/tools/dump.py
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     4830 2022-09-15 14:39:35.000000 atwiki-python-0.0.8/atwiki/uri.py
-drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-15 14:43:47.163855 atwiki-python-0.0.8/atwiki_python.egg-info/
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     3221 2022-09-15 14:43:47.000000 atwiki-python-0.0.8/atwiki_python.egg-info/PKG-INFO
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)      542 2022-09-15 14:43:47.000000 atwiki-python-0.0.8/atwiki_python.egg-info/SOURCES.txt
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)        1 2022-09-15 14:43:47.000000 atwiki-python-0.0.8/atwiki_python.egg-info/dependency_links.txt
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       55 2022-09-15 14:43:47.000000 atwiki-python-0.0.8/atwiki_python.egg-info/entry_points.txt
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       24 2022-09-15 14:43:47.000000 atwiki-python-0.0.8/atwiki_python.egg-info/requires.txt
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)        7 2022-09-15 14:43:47.000000 atwiki-python-0.0.8/atwiki_python.egg-info/top_level.txt
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       38 2022-09-15 14:43:47.163855 atwiki-python-0.0.8/setup.cfg
--rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     1409 2022-04-23 11:04:34.000000 atwiki-python-0.0.8/setup.py
+drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-19 07:36:49.277236 atwiki-python-0.0.9/
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     1065 2022-01-26 13:03:41.000000 atwiki-python-0.0.9/LICENSE
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     3221 2022-09-19 07:36:49.277236 atwiki-python-0.0.9/PKG-INFO
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     2410 2022-09-15 14:39:48.000000 atwiki-python-0.0.9/README.rst
+drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-19 07:36:49.277236 atwiki-python-0.0.9/atwiki/
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)      167 2022-01-20 14:57:13.000000 atwiki-python-0.0.9/atwiki/__init__.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       20 2022-09-19 07:20:23.000000 atwiki-python-0.0.9/atwiki/_version.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     4009 2022-09-19 07:20:23.000000 atwiki-python-0.0.9/atwiki/core.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     2975 2022-01-20 14:57:13.000000 atwiki-python-0.0.9/atwiki/parser.py
+drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-19 07:36:49.277236 atwiki-python-0.0.9/atwiki/test/
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       52 2022-01-20 14:57:13.000000 atwiki-python-0.0.9/atwiki/test/__init__.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     5552 2022-09-19 07:36:04.000000 atwiki-python-0.0.9/atwiki/test/test_core.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     1038 2022-04-23 08:19:07.000000 atwiki-python-0.0.9/atwiki/test/test_parser.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     3388 2022-09-15 14:39:35.000000 atwiki-python-0.0.9/atwiki/test/test_uri.py
+drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-19 07:36:49.277236 atwiki-python-0.0.9/atwiki/test/tools/
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)        0 2022-01-20 14:57:13.000000 atwiki-python-0.0.9/atwiki/test/tools/__init__.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)      372 2022-01-20 14:57:13.000000 atwiki-python-0.0.9/atwiki/test/tools/test_dump.py
+drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-19 07:36:49.277236 atwiki-python-0.0.9/atwiki/tools/
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)        0 2022-01-20 14:57:13.000000 atwiki-python-0.0.9/atwiki/tools/__init__.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     1877 2022-01-20 14:57:13.000000 atwiki-python-0.0.9/atwiki/tools/dump.py
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     4830 2022-09-15 14:39:35.000000 atwiki-python-0.0.9/atwiki/uri.py
+drwxrwxr-x   0 kenichi   (1000) kenichi   (1000)        0 2022-09-19 07:36:49.277236 atwiki-python-0.0.9/atwiki_python.egg-info/
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     3221 2022-09-19 07:36:49.000000 atwiki-python-0.0.9/atwiki_python.egg-info/PKG-INFO
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)      542 2022-09-19 07:36:49.000000 atwiki-python-0.0.9/atwiki_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)        1 2022-09-19 07:36:49.000000 atwiki-python-0.0.9/atwiki_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       55 2022-09-19 07:36:49.000000 atwiki-python-0.0.9/atwiki_python.egg-info/entry_points.txt
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       24 2022-09-19 07:36:49.000000 atwiki-python-0.0.9/atwiki_python.egg-info/requires.txt
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)        7 2022-09-19 07:36:49.000000 atwiki-python-0.0.9/atwiki_python.egg-info/top_level.txt
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)       38 2022-09-19 07:36:49.277236 atwiki-python-0.0.9/setup.cfg
+-rw-rw-r--   0 kenichi   (1000) kenichi   (1000)     1409 2022-04-23 11:04:34.000000 atwiki-python-0.0.9/setup.py
```

### Comparing `atwiki-python-0.0.8/LICENSE` & `atwiki-python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `atwiki-python-0.0.8/PKG-INFO` & `atwiki-python-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atwiki-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Atwiki Client Library
 Home-page: https://github.com/kmaehashi/atwiki-python
 Author: Kenichi Maehashi
 Author-email: webmaster@kenichimaehashi.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atwiki-python-0.0.8/README.rst` & `atwiki-python-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `atwiki-python-0.0.8/atwiki/core.py` & `atwiki-python-0.0.9/atwiki/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   def get_list(self, tag=None, _start=1):
     index = _start
     while True:
       count = 0
       if tag:
         soup = self._request(self._uri.tag(tag, index))
         links = soup.find('div', attrs={'class': 'cmd_tag'}).find('ul').select('a')
-        pager = soup.find('div', attrs={'class': 'cmd_tag'}).select_one('a[href$="?&p={}"]'.format(index + 1))
+        pager = soup.find('div', attrs={'class': 'cmd_tag'}).select_one('a[href$="?p={}"]'.format(index + 1))
       else:
         soup = self._request(self._uri.list('create', index))
         links = soup.find('table', attrs={'class': 'pagelist'}).findAll('a', href=True, title=True)
         pager = soup.find('ul', attrs={'class': 'atwiki_pagination'})
         if pager is not None:
           pager = pager.select_one('a[href$="&pp={}"]'.format(index + 1))
       is_end = (pager is None or len(links) == 0)
```

### Comparing `atwiki-python-0.0.8/atwiki/parser.py` & `atwiki-python-0.0.9/atwiki/parser.py`

 * *Files identical despite different names*

### Comparing `atwiki-python-0.0.8/atwiki/test/test_core.py` & `atwiki-python-0.0.9/atwiki/test/test_core.py`

 * *Files 24% similar despite different names*

```diff
@@ -65,49 +65,84 @@
 
 class PagerizeTest(TestCase):
     def setUp(self):
         self._uri = AtWikiURI('https://w.atwiki.jp/hmiku')
         self._api = AtWikiAPI(self._uri)
 
     def test_get_list(self):
+        # Get the first page from the first listing.
         top_page = next(self._api.get_list())
         assert top_page == {'id': 1, 'name': 'トップページ'}
 
+        # Detect number of all pages.
         soup = self._api._request(self._uri.list(sort='create', index=1))
         text = soup.find('div', class_='pagelist').text
         m = re.search(r'計 (\d+) ページ / 1 から 100 を表示', text)
         assert m is not None
         count = int(m.group(1))
         assert 45000 < count < 90000
         last_index = math.ceil(count / 100)
 
-        # Get list from the last page.
+        # Ensure listing pagerize works. (retrieve 3 listing, 100 pages in each)
+        count = 0
+        for page in self._api.get_list():
+            count += 1
+            if 100*3 <= count:
+                break
+        else:
+            assert False, "unexpected number of pages"
+
+        # Get list from the last listing.
         # N.B. The page counter is not updated immediately.
         pages = list(self._api.get_list(_start=last_index))
         expected = (count % 100)
         assert max(0, (expected - 50)) < len(pages) < min(100, (expected + 50))
 
+        # Get out-of-bounds listing. (expected to wrap around)
         top_page = next(self._api.get_list(_start=last_index + 1))
         assert top_page == {'id': 1, 'name': 'トップページ'}
 
     def test_get_list_tag(self):
+        # Detect number of listings.
         soup = self._api._request(self._uri.tag('曲', index=1))
         last_index = 1
         for link in soup.find('div', class_='cmd_tag').find_all('a'):
             if not link.attrs['href'].endswith('?p={}'.format(last_index + 1)):
                 break
             last_index += 1
         assert 750 <= last_index
 
+        # Ensure listing pagerize works. (retrieve 3 listing, 50 pages in each)
+        count = 0
+        for page in self._api.get_list('曲'):
+            count += 1
+            if 50*3 <= count:
+                break
+        else:
+            assert False, "unexpected number of pages for the tag"
+
+        # Get list from the last listing.
         pages = list(self._api.get_list('曲', _start=last_index))
         assert 1 <= len(pages) <= 50
 
+        # Get out-of-bounds listing.
         pages = list(self._api.get_list('曲', _start=last_index + 1))
         assert len(pages) == 0
 
     def test_get_tags(self):
+        # Get the first tag from the first listing.
         song = next(self._api.get_tags('num'))
         assert song['name'] == '曲'
         assert 35000 < song['weight'] < 70000
 
+        # Get the first tag from the second listing.
         not_song = next(self._api.get_tags('num', _start=2))
         assert not_song['name'] != '曲'
+
+        # Ensure listing pagerize works. (retrieve 3 listing, 500 pages in each)
+        count = 0
+        for page in self._api.get_tags():
+            count += 1
+            if 500*3 <= count:
+                break
+        else:
+            assert False, "unexpected number of tags"
```

### Comparing `atwiki-python-0.0.8/atwiki/test/test_parser.py` & `atwiki-python-0.0.9/atwiki/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `atwiki-python-0.0.8/atwiki/test/test_uri.py` & `atwiki-python-0.0.9/atwiki/test/test_uri.py`

 * *Files identical despite different names*

### Comparing `atwiki-python-0.0.8/atwiki/tools/dump.py` & `atwiki-python-0.0.9/atwiki/tools/dump.py`

 * *Files identical despite different names*

### Comparing `atwiki-python-0.0.8/atwiki/uri.py` & `atwiki-python-0.0.9/atwiki/uri.py`

 * *Files identical despite different names*

### Comparing `atwiki-python-0.0.8/atwiki_python.egg-info/PKG-INFO` & `atwiki-python-0.0.9/atwiki_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atwiki-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Atwiki Client Library
 Home-page: https://github.com/kmaehashi/atwiki-python
 Author: Kenichi Maehashi
 Author-email: webmaster@kenichimaehashi.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atwiki-python-0.0.8/atwiki_python.egg-info/SOURCES.txt` & `atwiki-python-0.0.9/atwiki_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atwiki-python-0.0.8/setup.py` & `atwiki-python-0.0.9/setup.py`

 * *Files identical despite different names*

