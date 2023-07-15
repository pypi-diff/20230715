# Comparing `tmp/render_engine-2023.7.2a1.tar.gz` & `tmp/render_engine-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.7.2a1.tar", last modified: Sun Jul  2 23:53:28 2023, max compression
+gzip compressed data, was "render_engine-2023.7.3.tar", last modified: Sat Jul 15 15:16:07 2023, max compression
```

## Comparing `render_engine-2023.7.2a1.tar` & `render_engine-2023.7.3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.031108 render_engine-2023.7.2a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.011108 render_engine-2023.7.2a1/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.011108 render_engine-2023.7.2a1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.011108 render_engine-2023.7.2a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.011108 render_engine-2023.7.2a1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.011108 render_engine-2023.7.2a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.015108 render_engine-2023.7.2a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-02 23:53:28.031108 render_engine-2023.7.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.015108 render_engine-2023.7.2a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.015108 render_engine-2023.7.2a1/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.019108 render_engine-2023.7.2a1/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.019108 render_engine-2023.7.2a1/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.019108 render_engine-2023.7.2a1/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 23:53:28.031108 render_engine-2023.7.2a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.019108 render_engine-2023.7.2a1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.023109 render_engine-2023.7.2a1/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.027109 render_engine-2023.7.2a1/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.027109 render_engine-2023.7.2a1/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.027109 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.023109 render_engine-2023.7.2a1/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-02 23:53:27.000000 render_engine-2023.7.2a1/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-02 23:53:28.000000 render_engine-2023.7.2a1/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:53:27.000000 render_engine-2023.7.2a1/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 23:53:27.000000 render_engine-2023.7.2a1/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-02 23:53:27.000000 render_engine-2023.7.2a1/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 23:53:27.000000 render_engine-2023.7.2a1/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.031108 render_engine-2023.7.2a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.031108 render_engine-2023.7.2a1/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.031108 render_engine-2023.7.2a1/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:53:28.031108 render_engine-2023.7.2a1/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-02 23:53:11.000000 render_engine-2023.7.2a1/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-15 15:15:45.000000 render_engine-2023.7.3/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-15 15:16:07.074638 render_engine-2023.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-15 15:15:45.000000 render_engine-2023.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-15 15:15:45.000000 render_engine-2023.7.3/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-15 15:15:45.000000 render_engine-2023.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-15 15:15:45.000000 render_engine-2023.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:16:07.074638 render_engine-2023.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.070638 render_engine-2023.7.3/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.070638 render_engine-2023.7.3/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.070638 render_engine-2023.7.3/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.070638 render_engine-2023.7.3/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_site.py
```

### Comparing `render_engine-2023.7.2a1/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.7.3/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/.devcontainer/devcontainer.json` & `render_engine-2023.7.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.7.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/.github/CONTRIBUTION.md` & `render_engine-2023.7.3/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/.github/FUNDING.yml` & `render_engine-2023.7.3/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/.github/LICENSE` & `render_engine-2023.7.3/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/.github/dependabot.yml` & `render_engine-2023.7.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/.github/workflows/publish.yml` & `render_engine-2023.7.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/.gitignore` & `render_engine-2023.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/PKG-INFO` & `render_engine-2023.7.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.7.2a1
+Version: 2023.7.3
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-> ***Warning***
-> 
-> **BREAKING CHANGE**
-> As of 2023.4.2a1 Render Engine no longer uses the `date_published` or `date_modified` attributes for `Blog` objects. Please instead use `date`.
->
-> **BREAKING CHANGE**
-> As of 2023.4.2a1 Render Engine enforces that the `Blog.date` attribute is a `datetime` object. If using frontmatter please use [iso8601](https://en.wikipedia.org/wiki/ISO_8601) format for the date attribute.
+# Render Engine
+[![PyTest](https://github.com/kjaymiller/render_engine/actions/workflows/test.yml/badge.svg)](https://github.com/kjaymiller/render_engine/actions/workflows/test.yml)
 
 ## What is RenderEngine
 ## The _3 layer_ Architecture 
 
 * **[Page](.github/render_engine/page.html)** - A single webpage item built from content, a template, raw data, or a combination of those things.
 * **[Collection](.github/render_engine/collection.html)** - A group of webpages built from the same template, organized in a single directory
 * **[Site](.github/render_engine/site.html)** - The container that helps to render all Pages and Collections in with uniform settigns and variables
```

### Comparing `render_engine-2023.7.2a1/README.md` & `render_engine-2023.7.3/src/render_engine.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-> ***Warning***
-> 
-> **BREAKING CHANGE**
-> As of 2023.4.2a1 Render Engine no longer uses the `date_published` or `date_modified` attributes for `Blog` objects. Please instead use `date`.
->
-> **BREAKING CHANGE**
-> As of 2023.4.2a1 Render Engine enforces that the `Blog.date` attribute is a `datetime` object. If using frontmatter please use [iso8601](https://en.wikipedia.org/wiki/ISO_8601) format for the date attribute.
+Metadata-Version: 2.1
+Name: render-engine
+Version: 2023.7.3
+Summary: A Flexible Static Site Generator for Python
+Project-URL: homepage, https://github.com/kjaymiller/render_engine/
+Project-URL: repository, https://github.com/kjaymiller/render_engine/
+Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
+# Render Engine
+[![PyTest](https://github.com/kjaymiller/render_engine/actions/workflows/test.yml/badge.svg)](https://github.com/kjaymiller/render_engine/actions/workflows/test.yml)
 
 ## What is RenderEngine
 ## The _3 layer_ Architecture 
 
 * **[Page](.github/render_engine/page.html)** - A single webpage item built from content, a template, raw data, or a combination of those things.
 * **[Collection](.github/render_engine/collection.html)** - A group of webpages built from the same template, organized in a single directory
 * **[Site](.github/render_engine/site.html)** - The container that helps to render all Pages and Collections in with uniform settigns and variables
```

### Comparing `render_engine-2023.7.2a1/changelog.md` & `render_engine-2023.7.3/changelog.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/archive.md` & `render_engine-2023.7.3/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/assets/create-app-help.png` & `render_engine-2023.7.3/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.7.3/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/assets/render-engine-init.png` & `render_engine-2023.7.3/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/cli.md` & `render_engine-2023.7.3/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/contributing/pages.md` & `render_engine-2023.7.3/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/custom_collections.md` & `render_engine-2023.7.3/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.7.3/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.7.3/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.7.3/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/getting-started/installation.md` & `render_engine-2023.7.3/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/getting-started/layout.md` & `render_engine-2023.7.3/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/index.md` & `render_engine-2023.7.3/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/page.md` & `render_engine-2023.7.3/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/parsers.md` & `render_engine-2023.7.3/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/docs/templates.md` & `render_engine-2023.7.3/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/docs/mkdocs.yml` & `render_engine-2023.7.3/docs/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     - Page Objects: page.md
     - Collection:
       - Collection: collection.md
       - Archive: archive.md
       - RSS Feed: feeds.md
     - Site:
       - Site: site.md
-      - Plugins: hookspecs.md
   - Extending Render Engine:
-    - Built-in Plugins: plugins.md
     - Plugins: plugins.md
+    - Plugins Entrypoints: hookspecs.md
+    - Built-in Plugins: plugins.md
   - Parsers: parsers.md
   - CLI: cli.md
   - Templates: templates.md
 markdown_extensions:
   - toc
   - codehilite:
       guess_lang: false
```

### Comparing `render_engine-2023.7.2a1/pyproject.toml` & `render_engine-2023.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/requirements.txt` & `render_engine-2023.7.3/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile pyproject.toml
 #
-click==8.1.3
+click==8.1.5
     # via typer
 dtyper==2.1.0
     # via render-engine (pyproject.toml)
 gitdb==4.0.10
     # via gitpython
-gitpython==3.1.31
+gitpython==3.1.32
     # via render-engine (pyproject.toml)
 jinja2==3.1.2
     # via render-engine (pyproject.toml)
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via rich
-markdown2==2.4.8
+markdown2==2.4.9
     # via render-engine (pyproject.toml)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via render-engine (pyproject.toml)
-pluggy==1.0.0
+pluggy==1.2.0
     # via render-engine (pyproject.toml)
 pygments==2.15.1
     # via rich
 python-dateutil==2.8.2
     # via render-engine (pyproject.toml)
 python-frontmatter==1.0.0
     # via render-engine (pyproject.toml)
 python-slugify==8.0.1
     # via render-engine (pyproject.toml)
 pyyaml==6.0
     # via python-frontmatter
-rich==13.3.5
+rich==13.4.2
     # via render-engine (pyproject.toml)
 six==1.16.0
     # via python-dateutil
 smmap==5.0.0
     # via gitdb
 text-unidecode==1.3
     # via python-slugify
 typer==0.9.0
     # via
     #   dtyper
     #   render-engine (pyproject.toml)
+typing-extensions==4.7.1
+    # via typer
```

### Comparing `render_engine-2023.7.2a1/src/.DS_Store` & `render_engine-2023.7.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/.DS_Store` & `render_engine-2023.7.3/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/_base_object.py` & `render_engine-2023.7.3/src/render_engine/_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/archive.py` & `render_engine-2023.7.3/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/blog.py` & `render_engine-2023.7.3/src/render_engine/blog.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/cli.py` & `render_engine-2023.7.3/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/collection.py` & `render_engine-2023.7.3/src/render_engine/collection.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/engine.py` & `render_engine-2023.7.3/src/render_engine/engine.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/feeds.py` & `render_engine-2023.7.3/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/hookspecs.py` & `render_engine-2023.7.3/src/render_engine/hookspecs.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 class SiteSpecs:
     """Plugin hook specifications for the Site class"""
 
     @hook_spec
     def pre_build_site(self, site: "Site") -> None:
         """Steps Prior to Building the site"""
 
+
     @hook_spec
     def post_build_site(self, site: "Site") -> None:
         """Build After Building the site"""
 
     @hook_spec
     def render_content(page: "page"):
         """
```

### Comparing `render_engine-2023.7.2a1/src/render_engine/links.py` & `render_engine-2023.7.3/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/page.py` & `render_engine-2023.7.3/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/parsers/.DS_Store` & `render_engine-2023.7.3/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.7.3/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.7.3/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.7.3/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/plugins.py` & `render_engine-2023.7.3/src/render_engine/plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Plugins are a way to extend the functionality of the render engine site.
-"""
+
 
 import pathlib
 import shutil
 
 from render_engine.engine import engine
 from render_engine.hookspecs import hook_impl
 from render_engine.site import Site
```

### Comparing `render_engine-2023.7.2a1/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.7.3/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.7.3/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.7.3/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.7.3/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/src/render_engine/site.py` & `render_engine-2023.7.3/src/render_engine/site.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from rich.progress import Progress
 
 from .collection import Collection
 from .engine import engine
 from .hookspecs import register_plugins
 from .page import Page
 
-
 class Site:
     """
     The site stores your pages and collections to be rendered.
 
     Attributes:
         engine: Jinja2 Environment used to render pages
         output_path: 
@@ -79,15 +78,20 @@
         class Posts(Collection):
             pass
 
         site.collection(Posts) # also works
         ```
         """
         _Collection = Collection()
-        _Collection.register_plugins(self.plugins)
+        plugins = [*self.plugins, *getattr(_Collection, "plugins", [])]
+        
+        for plugin in getattr(_Collection, 'ignore_plugins', []):
+            plugins.remove(plugin)
+        _Collection.register_plugins(plugins)
+
         self._pm.hook.pre_build_collection(collection=_Collection) #type: ignore
         self.route_list[_Collection._slug] = _Collection
         return _Collection
 
     def page(self, Page: Page) -> Page:
         """
         Add the page to the route list to be rendered later.
@@ -112,15 +116,20 @@
             pass
 
         site.page(About) # also works
         ```
         """
         page = Page()
         page.title = page._title # Expose _title to the user through `title`
-        page.register_plugins(self.plugins)
+        
+        plugins = [*self.plugins, *getattr(page, "plugins", [])]
+        
+        for plugin in getattr(page, 'ignore_plugins', []):
+            plugins.remove(plugin)
+        page.register_plugins(plugins)
         self.route_list[getattr(page, page._reference)] = page
 
     def _render_static(self) -> None:
         """Copies a Static Directory to the output folder"""
         shutil.copytree(
             self.static_path,
             pathlib.Path(self.output_path) / pathlib.Path(self.static_path).name,
```

### Comparing `render_engine-2023.7.2a1/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.7.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,9 @@
-Metadata-Version: 2.1
-Name: render-engine
-Version: 2023.7.2a1
-Summary: A Flexible Static Site Generator for Python
-Project-URL: homepage, https://github.com/kjaymiller/render_engine/
-Project-URL: repository, https://github.com/kjaymiller/render_engine/
-Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-> ***Warning***
-> 
-> **BREAKING CHANGE**
-> As of 2023.4.2a1 Render Engine no longer uses the `date_published` or `date_modified` attributes for `Blog` objects. Please instead use `date`.
->
-> **BREAKING CHANGE**
-> As of 2023.4.2a1 Render Engine enforces that the `Blog.date` attribute is a `datetime` object. If using frontmatter please use [iso8601](https://en.wikipedia.org/wiki/ISO_8601) format for the date attribute.
+# Render Engine
+[![PyTest](https://github.com/kjaymiller/render_engine/actions/workflows/test.yml/badge.svg)](https://github.com/kjaymiller/render_engine/actions/workflows/test.yml)
 
 ## What is RenderEngine
 ## The _3 layer_ Architecture 
 
 * **[Page](.github/render_engine/page.html)** - A single webpage item built from content, a template, raw data, or a combination of those things.
 * **[Collection](.github/render_engine/collection.html)** - A group of webpages built from the same template, organized in a single directory
 * **[Site](.github/render_engine/site.html)** - The container that helps to render all Pages and Collections in with uniform settigns and variables
```

### Comparing `render_engine-2023.7.2a1/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.7.3/src/render_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/conftest.py` & `render_engine-2023.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/create_app_check_file.txt` & `render_engine-2023.7.3/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/test_base_object.py` & `render_engine-2023.7.3/tests/test_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/test_base_parser.py` & `render_engine-2023.7.3/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/test_collections.py` & `render_engine-2023.7.3/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/test_create_app.py` & `render_engine-2023.7.3/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/test_feeds.py` & `render_engine-2023.7.3/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/test_page.py` & `render_engine-2023.7.3/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.2a1/tests/test_site.py` & `render_engine-2023.7.3/tests/test_site.py`

 * *Files identical despite different names*

