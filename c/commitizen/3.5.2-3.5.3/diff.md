# Comparing `tmp/commitizen-3.5.2.tar.gz` & `tmp/commitizen-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.5.2.tar", max compression
+gzip compressed data, was "commitizen-3.5.3.tar", max compression
```

## Comparing `commitizen-3.5.2.tar` & `commitizen-3.5.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-06-25 23:58:43.352577 commitizen-3.5.2/LICENSE
--rw-r--r--   0        0        0      609 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/__version__.py
--rw-r--r--   0        0        0     4609 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/bump.py
--rw-r--r--   0        0        0    12112 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/changelog.py
--rw-r--r--   0        0        0     3455 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    18106 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    14245 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7145 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5208 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/info.py
--rw-r--r--   0        0        0    12966 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/__init__.py
--rw-r--r--   0        0        0      898 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1568 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1746 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1431 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7070 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3337 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/defaults.py
--rw-r--r--   0        0        0     4706 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/factory.py
--rw-r--r--   0        0        0     7295 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/out.py
--rw-r--r--   0        0        0     7109 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     9732 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/version_schemes.py
--rw-r--r--   0        0        0     5750 2023-06-25 23:58:43.356577 commitizen-3.5.2/docs/README.md
--rw-r--r--   0        0        0     4290 2023-06-25 23:58:43.368577 commitizen-3.5.2/pyproject.toml
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-15 15:41:12.908831 commitizen-3.5.3/LICENSE
+-rw-r--r--   0        0        0      609 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/__version__.py
+-rw-r--r--   0        0        0     4543 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/bump.py
+-rw-r--r--   0        0        0    12112 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/changelog.py
+-rw-r--r--   0        0        0     3455 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    18106 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    14245 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7148 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5208 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/info.py
+-rw-r--r--   0        0        0    13053 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      898 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1568 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1746 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1431 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7070 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3121 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3336 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/factory.py
+-rw-r--r--   0        0        0     7295 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/out.py
+-rw-r--r--   0        0        0     7134 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9732 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5750 2023-07-15 15:41:12.912832 commitizen-3.5.3/docs/README.md
+-rw-r--r--   0        0        0     4300 2023-07-15 15:41:12.924832 commitizen-3.5.3/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.3/PKG-INFO
```

### Comparing `commitizen-3.5.2/LICENSE` & `commitizen-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/__init__.py` & `commitizen-3.5.3/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/bump.py` & `commitizen-3.5.3/commitizen/bump.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 def _version_to_regex(version: str) -> str:
     return version.replace(".", r"\.").replace("+", r"\+")
 
 
 def normalize_tag(
     version: Version | str,
-    tag_format: str | None = None,
+    tag_format: str,
     scheme: VersionScheme | None = None,
 ) -> str:
     """The tag and the software version might be different.
 
     That's why this function exists.
 
     Example:
@@ -114,17 +114,14 @@
     | v0.9.0 | 0.9.0 |
     | ver1.0.0 | 1.0.0 |
     | ver1.0.0.a0 | 1.0.0a0 |
     """
     scheme = scheme or DEFAULT_SCHEME
     version = scheme(version) if isinstance(version, str) else version
 
-    if not tag_format:
-        return str(version)
-
     major, minor, patch = version.release
     prerelease = version.prerelease or ""
 
     t = Template(tag_format)
     return t.safe_substitute(
         version=version, major=major, minor=minor, patch=patch, prerelease=prerelease
     )
```

### Comparing `commitizen-3.5.2/commitizen/changelog.py` & `commitizen-3.5.3/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/changelog_parser.py` & `commitizen-3.5.3/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cli.py` & `commitizen-3.5.3/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cmd.py` & `commitizen-3.5.3/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/commands/bump.py` & `commitizen-3.5.3/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/commands/changelog.py` & `commitizen-3.5.3/commitizen/commands/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         )
         self.change_type_order = (
             self.config.settings.get("change_type_order")
             or self.cz.change_type_order
             or defaults.change_type_order
         )
         self.rev_range = args.get("rev_range")
-        self.tag_format = args.get("tag_format") or self.config.settings.get(
-            "tag_format"
+        self.tag_format: str = (
+            args.get("tag_format") or self.config.settings["tag_format"]
         )
         self.merge_prerelease = args.get(
             "merge_prerelease"
         ) or self.config.settings.get("changelog_merge_prerelease")
 
     def _find_incremental_rev(self, latest_version: str, tags: list[GitTag]) -> str:
         """Try to find the 'start_rev'.
```

### Comparing `commitizen-3.5.2/commitizen/commands/check.py` & `commitizen-3.5.3/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/commands/commit.py` & `commitizen-3.5.3/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/commands/init.py` & `commitizen-3.5.3/commitizen/commands/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import questionary
 import yaml
 from commitizen import cmd, factory, out
 from commitizen.__version__ import __version__
 from commitizen.config import BaseConfig, JsonConfig, TomlConfig, YAMLConfig
 from commitizen.cz import registry
-from commitizen.defaults import config_files
+from commitizen.defaults import DEFAULT_SETTINGS, config_files
 from commitizen.exceptions import InitFailedError, NoAnswersError
 from commitizen.git import get_latest_tag_name, get_tag_names, smart_open
 from commitizen.version_schemes import KNOWN_SCHEMES, Version, get_version_scheme
 
 
 class ProjectInfo:
     """Discover information about the current folder."""
@@ -199,22 +199,23 @@
         is_correct_format = False
         if latest_tag.startswith("v"):
             tag_format = r"v$version"
             is_correct_format = questionary.confirm(
                 f'Is "{tag_format}" the correct tag format?', style=self.cz.style
             ).unsafe_ask()
 
+        default_format = DEFAULT_SETTINGS["tag_format"]
         if not is_correct_format:
             tag_format = questionary.text(
-                'Please enter the correct version format: (default: "$version")',
+                f'Please enter the correct version format: (default: "{default_format}")',
                 style=self.cz.style,
             ).unsafe_ask()
 
             if not tag_format:
-                tag_format = "$version"
+                tag_format = default_format
         return tag_format
 
     def _ask_version_provider(self) -> str:
         """Ask for setting: version_provider"""
 
         OPTS = {
             "commitizen": "commitizen: Fetch and set version in commitizen config (default)",
```

### Comparing `commitizen-3.5.2/commitizen/commands/version.py` & `commitizen-3.5.3/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/config/__init__.py` & `commitizen-3.5.3/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/config/base_config.py` & `commitizen-3.5.3/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/config/json_config.py` & `commitizen-3.5.3/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/config/toml_config.py` & `commitizen-3.5.3/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/config/yaml_config.py` & `commitizen-3.5.3/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cz/__init__.py` & `commitizen-3.5.3/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cz/base.py` & `commitizen-3.5.3/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.5.3/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.5.3/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cz/customize/customize.py` & `commitizen-3.5.3/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cz/jira/jira.py` & `commitizen-3.5.3/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/cz/jira/jira_info.txt` & `commitizen-3.5.3/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/defaults.py` & `commitizen-3.5.3/commitizen/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 class Settings(TypedDict, total=False):
     name: str
     version: str | None
     version_files: list[str]
     version_provider: str | None
     version_scheme: str | None
     version_type: str | None
-    tag_format: str | None
+    tag_format: str
     bump_message: str | None
     allow_abort: bool
     allowed_prefixes: list[str]
     changelog_file: str
     changelog_incremental: bool
     changelog_start_rev: str | None
     changelog_merge_prerelease: bool
@@ -69,15 +69,15 @@
 
 DEFAULT_SETTINGS: Settings = {
     "name": "cz_conventional_commits",
     "version": None,
     "version_files": [],
     "version_provider": "commitizen",
     "version_scheme": None,
-    "tag_format": None,  # example v$version
+    "tag_format": "$version",  # example v$version
     "bump_message": None,  # bumped v$current_version to $new_version
     "allow_abort": False,
     "allowed_prefixes": [
         "Merge",
         "Revert",
         "Pull request",
         "fixup!",
```

### Comparing `commitizen-3.5.2/commitizen/exceptions.py` & `commitizen-3.5.3/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/factory.py` & `commitizen-3.5.3/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/git.py` & `commitizen-3.5.3/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/hooks.py` & `commitizen-3.5.3/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/out.py` & `commitizen-3.5.3/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/commitizen/providers.py` & `commitizen-3.5.3/commitizen/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,17 +191,17 @@
         "$patch": r"(?P<patch>\d+)",
         "$prerelease": r"(?P<prerelease>\w+\d+)?",
         "$devrelease": r"(?P<devrelease>\.dev\d+)?",
     }
 
     def _tag_format_matcher(self) -> Callable[[str], str | None]:
         version_scheme = get_version_scheme(self.config)
-        pattern = (
-            self.config.settings.get("tag_format") or version_scheme.parser.pattern
-        )
+        pattern = self.config.settings["tag_format"]
+        if pattern == "$version":
+            pattern = version_scheme.parser.pattern
         for var, tag_pattern in self.TAG_FORMAT_REGEXS.items():
             pattern = pattern.replace(var, tag_pattern)
 
         regex = re.compile(f"^{pattern}$", re.VERBOSE)
 
         def matcher(tag: str) -> str | None:
             match = regex.match(tag)
```

### Comparing `commitizen-3.5.2/commitizen/version_schemes.py` & `commitizen-3.5.3/commitizen/version_schemes.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/docs/README.md` & `commitizen-3.5.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.2/pyproject.toml` & `commitizen-3.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.5.2"
+version = "3.5.3"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.5.2"
+version = "3.5.3"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -57,15 +57,15 @@
 pytest-mock = "^3.10"
 pytest-regressions = "^2.4.0"
 pytest-freezer = "^0.4.6"
 pytest-xdist = "^3.1.0"
 # code formatter
 black = "^22.10"
 # linter
-ruff = "^0.0.275"
+ruff = ">=0.0.275,<0.0.279"
 pre-commit = "^2.18.0"
 mypy = "^1.4"
 types-PyYAML = "^5.4.3"
 types-termcolor = "^0.1.1"
 # documentation
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.6"
```

### Comparing `commitizen-3.5.2/PKG-INFO` & `commitizen-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.5.2
+Version: 3.5.3
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

