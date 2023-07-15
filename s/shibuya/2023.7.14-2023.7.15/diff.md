# Comparing `tmp/shibuya-2023.7.14.tar.gz` & `tmp/shibuya-2023.7.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shibuya-2023.7.14.tar", last modified: Fri Jul 14 14:01:42 2023, max compression
+gzip compressed data, was "shibuya-2023.7.15.tar", last modified: Sat Jul 15 06:28:44 2023, max compression
```

## Comparing `shibuya-2023.7.14.tar` & `shibuya-2023.7.15.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.855770 shibuya-2023.7.14/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-14 14:01:20.000000 shibuya-2023.7.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 14:01:20.000000 shibuya-2023.7.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-14 14:01:42.855770 shibuya-2023.7.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-14 14:01:20.000000 shibuya-2023.7.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 14:01:20.000000 shibuya-2023.7.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:01:42.855770 shibuya-2023.7.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 14:01:20.000000 shibuya-2023.7.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.847770 shibuya-2023.7.14/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.851770 shibuya-2023.7.14/src/shibuya/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.851770 shibuya-2023.7.14/src/shibuya/css/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/css/dark.css
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/css/light.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.847770 shibuya-2023.7.14/src/shibuya/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.851770 shibuya-2023.7.14/src/shibuya/theme/shibuya/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.851770 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/nav-languages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/nav-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/nav-versions.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/site-foot.html
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/site-head.html
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/components/variables.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.855770 shibuya-2023.7.14/src/shibuya/theme/shibuya/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/extensions/buysellads.html
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.855770 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/extra-head.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/globaltoc-above.html
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/opengraph.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/page-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/webfonts.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.855770 shibuya-2023.7.14/src/shibuya/theme/shibuya/sidebars/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/sidebars/carbon-ads.html
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/sidebars/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/sidebars/repo-stats.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.855770 shibuya-2023.7.14/src/shibuya/theme/shibuya/static/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/static/print.css
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    68672 2023-07-14 14:01:30.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/static/shibuya.css
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-14 14:01:28.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/static/shibuya.js
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-14 14:01:20.000000 shibuya-2023.7.14/src/shibuya/theme/shibuya/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:01:42.851770 shibuya-2023.7.14/src/shibuya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-14 14:01:42.000000 shibuya-2023.7.14/src/shibuya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-14 14:01:42.000000 shibuya-2023.7.14/src/shibuya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:01:42.000000 shibuya-2023.7.14/src/shibuya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 14:01:42.000000 shibuya-2023.7.14/src/shibuya.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 14:01:42.000000 shibuya-2023.7.14/src/shibuya.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 14:01:42.000000 shibuya-2023.7.14/src/shibuya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.057103 shibuya-2023.7.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-15 06:28:25.000000 shibuya-2023.7.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-15 06:28:25.000000 shibuya-2023.7.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-15 06:28:44.057103 shibuya-2023.7.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-15 06:28:25.000000 shibuya-2023.7.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-15 06:28:25.000000 shibuya-2023.7.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:28:44.057103 shibuya-2023.7.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-15 06:28:25.000000 shibuya-2023.7.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.049103 shibuya-2023.7.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.053103 shibuya-2023.7.15/src/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.053103 shibuya-2023.7.15/src/shibuya/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/css/dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/css/light.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.049103 shibuya-2023.7.15/src/shibuya/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.053103 shibuya-2023.7.15/src/shibuya/theme/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.053103 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/nav-languages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/nav-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/nav-versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/site-foot.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/site-head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/components/variables.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.053103 shibuya-2023.7.15/src/shibuya/theme/shibuya/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/extensions/buysellads.html
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.057103 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/extra-head.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/globaltoc-above.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/opengraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/page-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/webfonts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.057103 shibuya-2023.7.15/src/shibuya/theme/shibuya/sidebars/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/sidebars/carbon-ads.html
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/sidebars/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/sidebars/repo-stats.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.057103 shibuya-2023.7.15/src/shibuya/theme/shibuya/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/static/print.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    68672 2023-07-15 06:28:31.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/static/shibuya.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-15 06:28:29.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/static/shibuya.js
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-15 06:28:25.000000 shibuya-2023.7.15/src/shibuya/theme/shibuya/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:44.053103 shibuya-2023.7.15/src/shibuya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-15 06:28:44.000000 shibuya-2023.7.15/src/shibuya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-15 06:28:44.000000 shibuya-2023.7.15/src/shibuya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:28:44.000000 shibuya-2023.7.15/src/shibuya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-15 06:28:44.000000 shibuya-2023.7.15/src/shibuya.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 06:28:44.000000 shibuya-2023.7.15/src/shibuya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 06:28:44.000000 shibuya-2023.7.15/src/shibuya.egg-info/top_level.txt
```

### Comparing `shibuya-2023.7.14/LICENSE` & `shibuya-2023.7.15/LICENSE`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/PKG-INFO` & `shibuya-2023.7.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shibuya
-Version: 2023.7.14
+Version: 2023.7.15
 Summary: A clean, responsive, and customizable Sphinx documentation theme with light/dark mode.
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/lepture/shibuya
 Project-URL: Documentation, https://shibuya.lepture.com/
 Project-URL: Sponsors, https://github.com/sponsors/lepture
 Classifier: Framework :: Sphinx
```

### Comparing `shibuya-2023.7.14/README.md` & `shibuya-2023.7.15/README.md`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/pyproject.toml` & `shibuya-2023.7.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/__init__.py` & `shibuya-2023.7.15/src/shibuya/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     create_edit_source_link,
 )
 from ._sphinx import (
     WrapperPostTransform,
     WrapLineFormatter,
 )
 
-__version__ = "2023.7.14"
+__version__ = "2023.7.15"
 
 shibuya_version = __version__
 
 THEME_PATH = (Path(__file__).parent / "theme" / "shibuya").resolve()
 
 
 def _add_version(name: str):
```

### Comparing `shibuya-2023.7.14/src/shibuya/_sphinx.py` & `shibuya-2023.7.15/src/shibuya/_sphinx.py`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/context.py` & `shibuya-2023.7.15/src/shibuya/context.py`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/css/base.css` & `shibuya-2023.7.15/src/shibuya/css/base.css`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/base.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/base.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/components/breadcrumbs.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/components/nav-links.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/components/nav-links.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/components/nav-versions.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/components/nav-versions.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/components/navigation.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/components/navigation.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/components/site-foot.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/components/site-foot.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/components/site-head.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/components/site-head.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/components/variables.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/components/variables.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/extensions/buysellads.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/extensions/buysellads.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/layout.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/layout.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/page.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/page.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/partials/opengraph.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/partials/opengraph.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/sidebars/repo-stats.html` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/sidebars/repo-stats.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/static/pygments.css` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/static/pygments.css`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/static/shibuya.css` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/static/shibuya.css`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/static/shibuya.js` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/static/shibuya.js`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya/theme/shibuya/theme.conf` & `shibuya-2023.7.15/src/shibuya/theme/shibuya/theme.conf`

 * *Files identical despite different names*

### Comparing `shibuya-2023.7.14/src/shibuya.egg-info/PKG-INFO` & `shibuya-2023.7.15/src/shibuya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shibuya
-Version: 2023.7.14
+Version: 2023.7.15
 Summary: A clean, responsive, and customizable Sphinx documentation theme with light/dark mode.
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/lepture/shibuya
 Project-URL: Documentation, https://shibuya.lepture.com/
 Project-URL: Sponsors, https://github.com/sponsors/lepture
 Classifier: Framework :: Sphinx
```

### Comparing `shibuya-2023.7.14/src/shibuya.egg-info/SOURCES.txt` & `shibuya-2023.7.15/src/shibuya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

