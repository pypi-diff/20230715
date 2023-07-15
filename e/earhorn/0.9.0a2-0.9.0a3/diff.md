# Comparing `tmp/earhorn-0.9.0a2.tar.gz` & `tmp/earhorn-0.9.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earhorn-0.9.0a2.tar", max compression
+gzip compressed data, was "earhorn-0.9.0a3.tar", max compression
```

## Comparing `earhorn-0.9.0a2.tar` & `earhorn-0.9.0a3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/LICENSE
--rw-r--r--   0        0        0     4152 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/README.md
--rw-r--r--   0        0        0        0 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/__init__.py
--rw-r--r--   0        0        0       64 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/_ffmpeg.py
--rw-r--r--   0        0        0     1997 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/archive.py
--rw-r--r--   0        0        0      847 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/check.py
--rw-r--r--   0        0        0     2641 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/event.py
--rw-r--r--   0        0        0     5210 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/main.py
--rw-r--r--   0        0        0     3684 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/prometheus.py
--rw-r--r--   0        0        0     2596 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/silence.py
--rw-r--r--   0        0        0     4951 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/earhorn/stats.py
--rw-r--r--   0        0        0     1362 2022-04-24 20:38:54.745736 earhorn-0.9.0a2/pyproject.toml
--rw-r--r--   0        0        0     5166 2022-04-24 20:39:11.960936 earhorn-0.9.0a2/setup.py
--rw-r--r--   0        0        0     5129 2022-04-24 20:39:11.961421 earhorn-0.9.0a2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/LICENSE
+-rw-r--r--   0        0        0     4152 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/README.md
+-rw-r--r--   0        0        0        0 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/__init__.py
+-rw-r--r--   0        0        0       64 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/_ffmpeg.py
+-rw-r--r--   0        0        0     1997 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/archive.py
+-rw-r--r--   0        0        0      847 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/check.py
+-rw-r--r--   0        0        0     2641 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/event.py
+-rw-r--r--   0        0        0     5222 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/main.py
+-rw-r--r--   0        0        0     3684 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/prometheus.py
+-rw-r--r--   0        0        0     2596 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/silence.py
+-rw-r--r--   0        0        0     4951 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/earhorn/stats.py
+-rw-r--r--   0        0        0     1362 2022-04-24 21:04:36.559500 earhorn-0.9.0a3/pyproject.toml
+-rw-r--r--   0        0        0     5166 2022-04-24 21:04:49.288610 earhorn-0.9.0a3/setup.py
+-rw-r--r--   0        0        0     5129 2022-04-24 21:04:49.289056 earhorn-0.9.0a3/PKG-INFO
```

### Comparing `earhorn-0.9.0a2/LICENSE` & `earhorn-0.9.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `earhorn-0.9.0a2/README.md` & `earhorn-0.9.0a3/README.md`

 * *Files identical despite different names*

### Comparing `earhorn-0.9.0a2/earhorn/archive.py` & `earhorn-0.9.0a3/earhorn/archive.py`

 * *Files identical despite different names*

### Comparing `earhorn-0.9.0a2/earhorn/check.py` & `earhorn-0.9.0a3/earhorn/check.py`

 * *Files identical despite different names*

### Comparing `earhorn-0.9.0a2/earhorn/event.py` & `earhorn-0.9.0a3/earhorn/event.py`

 * *Files identical despite different names*

### Comparing `earhorn-0.9.0a2/earhorn/main.py` & `earhorn-0.9.0a3/earhorn/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,15 +145,14 @@
 
     event_handler.start()
 
     # Starting services
     threads: List[Thread] = []
 
     if stats_url is not None:
-        logger.info("loading icecast stats handler")
         stats_exporter = StatsExporter(
             stop=stop_event,
             url=stats_url,
             auth=(stats_user, stats_password),
         )
         stats_exporter.start()
         threads.append(stats_exporter)
@@ -176,9 +175,12 @@
                     archive_segment_format,
                     archive_segment_format_options,
                     archive_copy_stream,
                 )
                 archiver.start()
                 threads.append(archiver)
 
+            silence_listener.join()
+            archiver.join()
+
     for thread in threads:
         thread.join()
```

### Comparing `earhorn-0.9.0a2/earhorn/prometheus.py` & `earhorn-0.9.0a3/earhorn/prometheus.py`

 * *Files identical despite different names*

### Comparing `earhorn-0.9.0a2/earhorn/silence.py` & `earhorn-0.9.0a3/earhorn/silence.py`

 * *Files identical despite different names*

### Comparing `earhorn-0.9.0a2/earhorn/stats.py` & `earhorn-0.9.0a3/earhorn/stats.py`

 * *Files identical despite different names*

### Comparing `earhorn-0.9.0a2/pyproject.toml` & `earhorn-0.9.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "earhorn"
-version = "0.9.0-alpha.2"
+version = "0.9.0-alpha.3"
 description = "Listen, monitor and archive your streams!"
 authors = ["Joola <jooola@users.noreply.github.com>"]
 readme = "README.md"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `earhorn-0.9.0a2/setup.py` & `earhorn-0.9.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pydantic>=1.9.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['earhorn = earhorn.main:cli']}
 
 setup_kwargs = {
     'name': 'earhorn',
-    'version': '0.9.0a2',
+    'version': '0.9.0a3',
     'description': 'Listen, monitor and archive your streams!',
     'long_description': '# earhorn\n\nListen, monitor and archive your streams!\n\n[![](https://mermaid.ink/svg/pako:eNqNlD9PwzAQxb_KySNqFySWqCoDMLAw0AEhgiorvhIriV1dnAJCfHcuzj8nzsDmvHv383Muzo_IrEKRiNpJh_dafpCstpfr1AB4CVJxcJIc4AWNg1waVSKlAmTdGsgdB4k73q7eYbvdLwsx7Ey2QpdjU4ekQO06JkiADV0TWZ-O7aI-NlTCbpflVme436-DQnMCj35_V0PbqvCkDSq4jUN3ppU34AutfxZiSuy1BF4xTkwoq_9HHtx95vYxDj3ntr1ZjlnRi1GMVNy1ZSCsLD92ru50Yd9ablvEsUcEl06Wiq4QkhbHsYU_DQ90aGTsbZdwtlX3PoMzLOdT6tqhmY9m1CK3pCzXl7l71Lx7DLuGWhSnznCn58Z0eGqM0eZjGu0A84ioOtCW1X7pZb5rCTx8abe4X2gUIJElcHb10rLh6A1L4lRh8GCIRxC4nux88xepHfDU4YZtmTWqv96frE8Y3zFSPDQ2zJXoMxYbUSFVUiv-d_20DangT6jCVCS85Ashm9KlIjW_bG3OigM-KO0sieQkyxo3QjbOHr5NJhJHDQ6m_hfYu37_AFEs0XE)](https://mermaid.live/edit#pako:eNqNlD9PwzAQxb_KySNqFySWqCoDMLAw0AEhgiorvhIriV1dnAJCfHcuzj8nzsDmvHv383Muzo_IrEKRiNpJh_dafpCstpfr1AB4CVJxcJIc4AWNg1waVSKlAmTdGsgdB4k73q7eYbvdLwsx7Ey2QpdjU4ekQO06JkiADV0TWZ-O7aI-NlTCbpflVme436-DQnMCj35_V0PbqvCkDSq4jUN3ppU34AutfxZiSuy1BF4xTkwoq_9HHtx95vYxDj3ntr1ZjlnRi1GMVNy1ZSCsLD92ru50Yd9ablvEsUcEl06Wiq4QkhbHsYU_DQ90aGTsbZdwtlX3PoMzLOdT6tqhmY9m1CK3pCzXl7l71Lx7DLuGWhSnznCn58Z0eGqM0eZjGu0A84ioOtCW1X7pZb5rCTx8abe4X2gUIJElcHb10rLh6A1L4lRh8GCIRxC4nux88xepHfDU4YZtmTWqv96frE8Y3zFSPDQ2zJXoMxYbUSFVUiv-d_20DangT6jCVCS85Ashm9KlIjW_bG3OigM-KO0sieQkyxo3QjbOHr5NJhJHDQ6m_hfYu37_AFEs0XE)\n\n## Install\n\nIf you need to listen or archive an Icecast stream, you will need `ffmpeg`:\n\n```sh\nsudo apt install ffmpeg\n```\n\nInstall earhorn from pip:\n\n```sh\npip install earhorn\n```\n\nYou can start archiving an Icecast stream by providing a stream url and an archive path:\n\n```sh\nearhorn \\\n  --stream-url https://stream.example.org/live.ogg \\\n  --archive-path=/to/my/archive\n```\n\nYou can also start exporting the Icecast stats as prometheus metrics by providing an Icecast stats url:\n\n```sh\nearhorn \\\n  --stats-url https://stream.example.org/admin/stats.xml \\\n  --stats-user admin \\\n  --stats-password hackme\n```\n\n### Docker\n\n```sh\ndocker pull ghcr.io/jooola/earhorn\n```\n\n## Usage\n\n```\nUsage: earhorn [OPTIONS]\n\n  See the ffmpeg documentation for details about the `--archive-segment-*` options:\n  https://ffmpeg.org/ffmpeg-formats.html#segment_002c-stream_005fsegment_002c-ssegment\n\nOptions:\n  --listen-port INTEGER           Listen port for the prometheus metrics endpoint.  [default: 9950]\n  --hook PATH                     Path to a custom script executed to handle stream state `events`.\n  --stream-url TEXT               URL to the icecast stream.\n  --stats-url TEXT                URL to the icecast admin xml stats page.\n  --stats-user TEXT               Username for the icecast admin xml stats page.  [default: admin]\n  --stats-password TEXT           Password for the icecast admin xml stats page.\n  --archive-path PATH             Path to the archive storage directory. If defined, the archiver will save the\n                                  `stream` in segments in the storage path.\n  --archive-segment-size INTEGER  Archive segment size in seconds.  [default: 3600]\n  --archive-segment-filename TEXT\n                                  Archive segment filename (without extension).  [default: archive-%Y%m%d_%H%M%S]\n  --archive-segment-format TEXT   Archive segment format.  [default: ogg]\n  --archive-segment-format-options TEXT\n                                  Archive segment format options.\n  --archive-copy-stream           Copy the `stream` without transcoding (reduce CPU usage). WARNING: The stream has to\n                                  be in the same format as the `--archive-segment-format`.\n  --help                          Show this message and exit.\n\n```\n\n## Developmement\n\nTo develop this project, start by reading the `Makefile` to have a basic understanding of the possible tasks.\n\nInstall the project and the dependencies in a virtual environment:\n\n```sh\nmake install\nsource .venv/bin/activate\nearhorn --help\n```\n\n## Releases\n\nTo release a new version, first bump the version number in `pyproject.toml` by hand or by using:\n\n```sh\n# poetry version --help\npoetry version <patch|minor|major>\n```\n\nRun the release target:\n\n```sh\nmake release\n```\n\nFinally, push the release commit and tag to publish them to Pypi:\n\n```sh\ngit push --follow-tags\n```\n',
     'author': 'Joola',
     'author_email': 'jooola@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `earhorn-0.9.0a2/PKG-INFO` & `earhorn-0.9.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earhorn
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: Listen, monitor and archive your streams!
 Author: Joola
 Author-email: jooola@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

