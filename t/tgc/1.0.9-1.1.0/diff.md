# Comparing `tmp/tgc-1.0.9.tar.gz` & `tmp/tgc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgc-1.0.9.tar", last modified: Mon Mar  6 20:14:04 2023, max compression
+gzip compressed data, was "tgc-1.1.0.tar", last modified: Sat Jul 15 17:21:11 2023, max compression
```

## Comparing `tgc-1.0.9.tar` & `tgc-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-03-06 20:14:04.868545 tgc-1.0.9/
--rw-r--r--   0 azalea    (1000) azalea    (1000)       66 2023-01-13 09:42:09.000000 tgc-1.0.9/.gitattributes
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2853 2023-01-13 09:42:09.000000 tgc-1.0.9/.gitignore
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1069 2023-01-13 09:42:09.000000 tgc-1.0.9/LICENSE
--rw-r--r--   0 azalea    (1000) azalea    (1000)     6902 2023-03-06 20:14:04.868545 tgc-1.0.9/PKG-INFO
--rw-r--r--   0 azalea    (1000) azalea    (1000)     5296 2023-03-06 20:06:44.000000 tgc-1.0.9/README.md
--rw-r--r--   0 azalea    (1000) azalea    (1000)       99 2023-01-13 09:42:09.000000 tgc-1.0.9/package.json
--rw-r--r--   0 azalea    (1000) azalea    (1000)      966 2023-03-06 20:06:16.000000 tgc-1.0.9/pyproject.toml
--rw-r--r--   0 azalea    (1000) azalea    (1000)       38 2023-03-06 20:14:04.868545 tgc-1.0.9/setup.cfg
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-03-06 20:14:04.865212 tgc-1.0.9/tgc/
--rw-r--r--   0 azalea    (1000) azalea    (1000)       22 2023-03-06 20:13:44.000000 tgc-1.0.9/tgc/__init__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)    10441 2023-01-13 09:42:09.000000 tgc-1.0.9/tgc/convert_export.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2544 2023-01-30 15:56:59.000000 tgc-1.0.9/tgc/convert_media_types.py
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-03-06 20:14:04.868545 tgc-1.0.9/tgc/pyro/
--rw-r--r--   0 azalea    (1000) azalea    (1000)        0 2023-01-13 09:42:09.000000 tgc-1.0.9/tgc/pyro/__init__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)       61 2023-01-13 09:42:09.000000 tgc-1.0.9/tgc/pyro/__main__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      796 2023-01-13 09:42:09.000000 tgc-1.0.9/tgc/pyro/config.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      763 2023-01-13 09:42:09.000000 tgc-1.0.9/tgc/pyro/consts.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     3281 2023-01-13 09:42:09.000000 tgc-1.0.9/tgc/pyro/convert.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     6793 2023-03-06 19:49:44.000000 tgc-1.0.9/tgc/pyro/crawl.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     4780 2023-01-14 03:55:35.000000 tgc-1.0.9/tgc/pyro/download_media.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2292 2023-01-13 09:42:09.000000 tgc-1.0.9/tgc/pyro/grouper.py
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-03-06 20:14:04.868545 tgc-1.0.9/tgc/rss/
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1709 2023-03-06 19:37:33.000000 tgc-1.0.9/tgc/rss/__main__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1535 2023-03-06 20:13:26.000000 tgc-1.0.9/tgc/rss/posts_to_feed.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      796 2023-01-13 09:42:09.000000 tgc-1.0.9/tgc/tg-blog.html
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-03-06 20:14:04.865212 tgc-1.0.9/tgc.egg-info/
--rw-r--r--   0 azalea    (1000) azalea    (1000)     6902 2023-03-06 20:14:04.000000 tgc-1.0.9/tgc.egg-info/PKG-INFO
--rw-r--r--   0 azalea    (1000) azalea    (1000)      563 2023-03-06 20:14:04.000000 tgc-1.0.9/tgc.egg-info/SOURCES.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)        1 2023-03-06 20:14:04.000000 tgc-1.0.9/tgc.egg-info/dependency_links.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)       76 2023-03-06 20:14:04.000000 tgc-1.0.9/tgc.egg-info/entry_points.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)      169 2023-03-06 20:14:04.000000 tgc-1.0.9/tgc.egg-info/requires.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)        4 2023-03-06 20:14:04.000000 tgc-1.0.9/tgc.egg-info/top_level.txt
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-03-06 20:14:04.868545 tgc-1.0.9/tools/
--rw-r--r--   0 azalea    (1000) azalea    (1000)      681 2023-01-30 16:19:44.000000 tgc-1.0.9/tools/pyproject_update.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)    31910 2023-01-13 09:42:09.000000 tgc-1.0.9/yarn.lock
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-07-15 17:21:11.118303 tgc-1.1.0/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       66 2023-01-13 09:42:09.000000 tgc-1.1.0/.gitattributes
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2883 2023-07-15 17:18:53.000000 tgc-1.1.0/.gitignore
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1069 2023-01-13 09:42:09.000000 tgc-1.1.0/LICENSE
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     6902 2023-07-15 17:21:11.118303 tgc-1.1.0/PKG-INFO
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     5296 2023-03-06 20:06:44.000000 tgc-1.1.0/README.md
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1497 2023-07-15 17:18:53.000000 tgc-1.1.0/flake.lock
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2781 2023-07-15 17:18:53.000000 tgc-1.1.0/flake.nix
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       99 2023-01-13 09:42:09.000000 tgc-1.1.0/package.json
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      966 2023-03-06 20:06:16.000000 tgc-1.1.0/pyproject.toml
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       38 2023-07-15 17:21:11.118303 tgc-1.1.0/setup.cfg
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-07-15 17:21:11.115303 tgc-1.1.0/tgc/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       22 2023-07-15 17:19:30.000000 tgc-1.1.0/tgc/__init__.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    10441 2023-01-13 09:42:09.000000 tgc-1.1.0/tgc/convert_export.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2544 2023-01-30 15:56:59.000000 tgc-1.1.0/tgc/convert_media_types.py
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-07-15 17:21:11.117303 tgc-1.1.0/tgc/pyro/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)        0 2023-01-13 09:42:09.000000 tgc-1.1.0/tgc/pyro/__init__.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       61 2023-01-13 09:42:09.000000 tgc-1.1.0/tgc/pyro/__main__.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      796 2023-01-13 09:42:09.000000 tgc-1.1.0/tgc/pyro/config.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      763 2023-01-13 09:42:09.000000 tgc-1.1.0/tgc/pyro/consts.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     3347 2023-07-15 17:18:56.000000 tgc-1.1.0/tgc/pyro/convert.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     6973 2023-07-15 17:19:13.000000 tgc-1.1.0/tgc/pyro/crawl.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     4780 2023-01-14 03:55:35.000000 tgc-1.1.0/tgc/pyro/download_media.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2292 2023-01-13 09:42:09.000000 tgc-1.1.0/tgc/pyro/grouper.py
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-07-15 17:21:11.118303 tgc-1.1.0/tgc/rss/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1709 2023-03-06 19:37:33.000000 tgc-1.1.0/tgc/rss/__main__.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1535 2023-03-06 20:13:26.000000 tgc-1.1.0/tgc/rss/posts_to_feed.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      796 2023-01-13 09:42:09.000000 tgc-1.1.0/tgc/tg-blog.html
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-07-15 17:21:11.116303 tgc-1.1.0/tgc.egg-info/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     6902 2023-07-15 17:21:11.000000 tgc-1.1.0/tgc.egg-info/PKG-INFO
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      584 2023-07-15 17:21:11.000000 tgc-1.1.0/tgc.egg-info/SOURCES.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)        1 2023-07-15 17:21:11.000000 tgc-1.1.0/tgc.egg-info/dependency_links.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       76 2023-07-15 17:21:11.000000 tgc-1.1.0/tgc.egg-info/entry_points.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      169 2023-07-15 17:21:11.000000 tgc-1.1.0/tgc.egg-info/requires.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)        4 2023-07-15 17:21:11.000000 tgc-1.1.0/tgc.egg-info/top_level.txt
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-07-15 17:21:11.118303 tgc-1.1.0/tools/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      681 2023-01-30 16:19:44.000000 tgc-1.1.0/tools/pyproject_update.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    31910 2023-01-13 09:42:09.000000 tgc-1.1.0/yarn.lock
```

### Comparing `tgc-1.0.9/.gitignore` & `tgc-1.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -155,7 +155,11 @@
 node_modules
 config.toml
 /*.iml
 test
 exports
 .DS_Store
 ._*
+
+# Nix Flakes
+result
+result-*
```

### Comparing `tgc-1.0.9/LICENSE` & `tgc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/PKG-INFO` & `tgc-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgc
-Version: 1.0.9
+Version: 1.1.0
 Summary: Telegram Channel Backup Crawler
 Author-email: Azalea Gui <me@hydev.org>
 License: MIT License
         
         Copyright (c) 2022 Hykilpikonna
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tgc-1.0.9/README.md` & `tgc-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/pyproject.toml` & `tgc-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/convert_export.py` & `tgc-1.1.0/tgc/convert_export.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/convert_media_types.py` & `tgc-1.1.0/tgc/convert_media_types.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/pyro/config.py` & `tgc-1.1.0/tgc/pyro/config.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/pyro/consts.py` & `tgc-1.1.0/tgc/pyro/consts.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/pyro/convert.py` & `tgc-1.1.0/tgc/pyro/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
             if dct:
                 return dict(vars(dct))
         return {}
 
     d = deep_dict(helper(), {'_client'})
     if d:
         d['media_type'] = MEDIA_TYPE_MAP.get(msg.media)
+        if msg.has_media_spoiler:
+            d['spoiler'] = True
 
     # Move location to one place
     if msg.venue:
         d.pop('location', None)
         if msg.venue.location:
             d['longitude'] = msg.venue.location.longitude
             d['latitude'] = msg.venue.location.latitude
```

### Comparing `tgc-1.0.9/tgc/pyro/crawl.py` & `tgc-1.1.0/tgc/pyro/crawl.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,19 @@
         "text": effective_text(msg),
         "author": msg.author_signature,
         "views": msg.views,
         "forwards": msg.forwards,
         "forwarded_from": {
             "name": get_user_name(msg.forward_from),
             "url": f'https://t.me/{msg.forward_from.username}' if msg.forward_from.username else None,
-        } if msg.forward_from else None,
+        } if msg.forward_from else {
+            "name": msg.forward_from_chat.title,
+        } if msg.forward_from_chat else {
+            "name": msg.forward_sender_name,
+        } if msg.forward_sender_name else None,
         "media_group_id": msg.media_group_id,
         "reply_id": msg.reply_to_message_id,
         "file": convert_media_dict(msg)
     }
 
     # Download file
     f = m.get('file')
```

### Comparing `tgc-1.0.9/tgc/pyro/download_media.py` & `tgc-1.1.0/tgc/pyro/download_media.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/pyro/grouper.py` & `tgc-1.1.0/tgc/pyro/grouper.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/rss/__main__.py` & `tgc-1.1.0/tgc/rss/__main__.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/rss/posts_to_feed.py` & `tgc-1.1.0/tgc/rss/posts_to_feed.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc/tg-blog.html` & `tgc-1.1.0/tgc/tg-blog.html`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/tgc.egg-info/PKG-INFO` & `tgc-1.1.0/tgc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgc
-Version: 1.0.9
+Version: 1.1.0
 Summary: Telegram Channel Backup Crawler
 Author-email: Azalea Gui <me@hydev.org>
 License: MIT License
         
         Copyright (c) 2022 Hykilpikonna
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tgc-1.0.9/tgc.egg-info/SOURCES.txt` & `tgc-1.1.0/tgc.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 .gitattributes
 .gitignore
 LICENSE
 README.md
+flake.lock
+flake.nix
 package.json
 pyproject.toml
 yarn.lock
 tgc/__init__.py
 tgc/convert_export.py
 tgc/convert_media_types.py
 tgc/tg-blog.html
```

### Comparing `tgc-1.0.9/tools/pyproject_update.py` & `tgc-1.1.0/tools/pyproject_update.py`

 * *Files identical despite different names*

### Comparing `tgc-1.0.9/yarn.lock` & `tgc-1.1.0/yarn.lock`

 * *Files identical despite different names*

