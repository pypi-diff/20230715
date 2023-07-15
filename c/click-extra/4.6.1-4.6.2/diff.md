# Comparing `tmp/click_extra-4.6.1.tar.gz` & `tmp/click_extra-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.6.1.tar", max compression
+gzip compressed data, was "click_extra-4.6.2.tar", max compression
```

## Comparing `click_extra-4.6.1.tar` & `click_extra-4.6.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6104 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/__init__.py
--rw-r--r--   0        0        0    30238 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/colorize.py
--rw-r--r--   0        0        0    16715 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/commands.py
--rw-r--r--   0        0        0    16405 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/config.py
--rw-r--r--   0        0        0     4069 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/decorators.py
--rw-r--r--   0        0        0     6211 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/docs_update.py
--rw-r--r--   0        0        0    11805 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/logging.py
--rw-r--r--   0        0        0    25392 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/parameters.py
--rw-r--r--   0        0        0    17118 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/py.typed
--rw-r--r--   0        0        0     7676 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/pygments.py
--rw-r--r--   0        0        0     4969 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/sphinx.py
--rw-r--r--   0        0        0     5969 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tabulate.py
--rw-r--r--   0        0        0     2542 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/telemetry.py
--rw-r--r--   0        0        0    23592 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/testing.py
--rw-r--r--   0        0        0      770 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    11504 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    18365 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    15075 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    17059 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7354 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0    18184 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0    10884 2023-07-13 15:33:32.394568 click_extra-4.6.1/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8396 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0    14491 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3165 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     8259 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_testing.py
--rw-r--r--   0        0        0     3551 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     6359 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2544 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/timer.py
--rw-r--r--   0        0        0    11757 2023-07-13 15:33:32.398569 click_extra-4.6.1/click_extra/version.py
--rw-r--r--   0        0        0     7584 2023-07-13 15:33:32.402569 click_extra-4.6.1/pyproject.toml
--rw-r--r--   0        0        0     6631 2023-07-13 15:33:32.402569 click_extra-4.6.1/readme.md
--rw-r--r--   0        0        0     9679 1970-01-01 00:00:00.000000 click_extra-4.6.1/PKG-INFO
+-rw-r--r--   0        0        0     6104 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/__init__.py
+-rw-r--r--   0        0        0    28997 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/colorize.py
+-rw-r--r--   0        0        0    16232 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/commands.py
+-rw-r--r--   0        0        0    16405 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/config.py
+-rw-r--r--   0        0        0     4069 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/decorators.py
+-rw-r--r--   0        0        0     6211 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11805 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/logging.py
+-rw-r--r--   0        0        0    25392 2023-07-15 09:31:25.184612 click_extra-4.6.2/click_extra/parameters.py
+-rw-r--r--   0        0        0    17118 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/py.typed
+-rw-r--r--   0        0        0     7676 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/pygments.py
+-rw-r--r--   0        0        0     4969 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/sphinx.py
+-rw-r--r--   0        0        0     5969 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2542 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/testing.py
+-rw-r--r--   0        0        0      770 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    11504 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    19238 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    15075 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    17059 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7354 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0    18184 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0    10884 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8396 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0    14491 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3165 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     8259 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_testing.py
+-rw-r--r--   0        0        0     3551 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     6359 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2544 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/timer.py
+-rw-r--r--   0        0        0    11757 2023-07-15 09:31:25.188612 click_extra-4.6.2/click_extra/version.py
+-rw-r--r--   0        0        0     7641 2023-07-15 09:31:25.196612 click_extra-4.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6631 2023-07-15 09:31:25.196612 click_extra-4.6.2/readme.md
+-rw-r--r--   0        0        0     9679 1970-01-01 00:00:00.000000 click_extra-4.6.2/PKG-INFO
```

### Comparing `click_extra-4.6.1/click_extra/__init__.py` & `click_extra-4.6.2/click_extra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.6.1"
+__version__ = "4.6.2"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
```

### Comparing `click_extra-4.6.1/click_extra/colorize.py` & `click_extra-4.6.2/click_extra/colorize.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Helpers and utilities to apply ANSI coloring to terminal content."""
 
 from __future__ import annotations
 
+import dataclasses
 import os
 import re
 from configparser import RawConfigParser
+from dataclasses import dataclass
 from gettext import gettext as _
 from operator import getitem
-from typing import NamedTuple, Sequence, cast
+from typing import Sequence, cast
 
 import click
+import cloup
 import regex as re3
 from boltons.strutils import complement_int_list, int_ranges_from_int_list
 from cloup._util import identity
 from cloup.styling import Color, IStyle
-from cloup.typing import MISSING, Possibly
 
 from . import (
     Choice,
     Context,
     HelpFormatter,
     Option,
     Parameter,
@@ -42,44 +44,17 @@
     cache,
     echo,
     get_current_context,
 )
 from .parameters import ExtraOption
 
 
-class HelpExtraTheme(NamedTuple):
-    """Extends ``cloup.HelpTheme`` with extra properties and ``logging.levels``.
-
-    .. caution::
-        We had to redefined all fields and couldn't extend ``cloup.HelpTheme`` as there
-        is no way to cleanly do it with MyPy.
-
-        See:
-        - https://github.com/python/typing/issues/427
-        - https://mypy.readthedocs.io/en/stable/runtime_troubles.html#future-annotations-import-pep-563
-
-    .. todo::
-        This is being `discussed upstream at janluke/cloup#159
-        <https://github.com/janluke/cloup/issues/159>`_.
-    """
-
-    invoked_command: IStyle = identity
-    command_help: IStyle = identity
-    heading: IStyle = identity
-    constraint: IStyle = identity
-    section_help: IStyle = identity
-    col1: IStyle = identity
-    col2: IStyle = identity
-    alias: IStyle = identity
-    alias_secondary: IStyle | None = None
-    epilog: IStyle = identity
-    """Set of properties inherited from ``cloup.HelpTheme``.
-
-    See: https://cloup.readthedocs.io/en/stable/autoapi/cloup/index.html#cloup.HelpTheme.invoked_command
-    """
+@dataclass(frozen=True)
+class HelpExtraTheme(cloup.HelpTheme):
+    """Extends ``cloup.HelpTheme`` with ``logging.levels`` and extra properties."""
 
     critical: IStyle = identity
     error: IStyle = identity
     warning: IStyle = identity
     info: IStyle = identity
     debug: IStyle = identity
     """Log levels from Python's logging module."""
@@ -104,109 +79,90 @@
         <https://github.com/kdeldycke/mail-deduplicate/blob/0764287/mail_deduplicate/deduplicate.py#L445>`_.
 
     .. todo::
         Maybe this shouldn't be in Click Extra because it is a legacy inheritance from
         one of my other project.
     """
 
-    def with_(
+    def with_(  # type: ignore[override]
         self,
-        ### Cloup properties.
-        invoked_command: IStyle | None = None,
-        command_help: IStyle | None = None,
-        heading: IStyle | None = None,
-        constraint: IStyle | None = None,
-        section_help: IStyle | None = None,
-        col1: IStyle | None = None,
-        col2: IStyle | None = None,
-        alias: IStyle | None = None,
-        alias_secondary: Possibly[IStyle | None] = MISSING,
-        epilog: IStyle | None = None,
-        ### Log levels.
-        critical: IStyle | None = None,
-        error: IStyle | None = None,
-        warning: IStyle | None = None,
-        info: IStyle | None = None,
-        debug: IStyle | None = None,
-        ### Click Extra properties.
-        option: IStyle | None = None,
-        subcommand: IStyle | None = None,
-        choice: IStyle | None = None,
-        metavar: IStyle | None = None,
-        bracket: IStyle | None = None,
-        envvar: IStyle | None = None,
-        default: IStyle | None = None,
-        deprecated: IStyle | None = None,
-        search: IStyle | None = None,
-        success: IStyle | None = None,
-        ### Non-canonical Click Extra properties.
-        subheading: IStyle | None = None,
+        **kwargs: dict[str, IStyle | None],
     ) -> HelpExtraTheme:
-        """Copy of ``cloup.HelpTheme.with_``."""
-        kwargs = {key: val for key, val in locals().items() if val is not None}
-        kwargs.pop("self")
-        if kwargs:
-            return self._replace(**kwargs)
+        """Derives a new theme from the current one, with some styles overridden.
+
+        Returns the same instance if the provided styles are the same as the current.
+        """
+        # Check for unrecognized arguments.
+        unrecognized_args = set(kwargs).difference(self.__dataclass_fields__)
+        if unrecognized_args:
+            msg = f"Got unexpected keyword argument(s): {', '.join(unrecognized_args)}"
+            raise TypeError(
+                msg,
+            )
+
+        # List of styles that are different from the base theme.
+        new_styles = {
+            field_id: new_style
+            for field_id, new_style in kwargs.items()
+            if new_style != getattr(self, field_id)
+        }
+        if new_styles:
+            return dataclasses.replace(self, **new_styles)
+
+        # No new styles, return the same instance.
         return self
 
     @staticmethod
     def dark() -> HelpExtraTheme:
-        """A theme assuming a dark terminal background color.
-
-        .. todo::
-
-            Implement default dark theme.
-        """
-        raise NotImplementedError
+        """A theme assuming a dark terminal background color."""
+        return HelpExtraTheme(
+            invoked_command=Style(fg=Color.bright_white),
+            heading=Style(fg=Color.bright_blue, bold=True, underline=True),
+            constraint=Style(fg=Color.magenta),
+            # Neutralize Cloup's col1, as it interferes with our finer option styling
+            # which takes care of separators.
+            col1=identity,
+            # Style aliases like options and subcommands.
+            alias=Style(fg=Color.cyan),
+            # Style aliases punctuation like options, but dimmed.
+            alias_secondary=Style(fg=Color.cyan, dim=True),
+            ### Log styles.
+            critical=Style(fg=Color.red, bold=True),
+            error=Style(fg=Color.red),
+            warning=Style(fg=Color.yellow),
+            info=identity,  # INFO level is the default, so no style applied.
+            debug=Style(fg=Color.blue),
+            ### Click Extra styles.
+            option=Style(fg=Color.cyan),
+            # Style subcommands like options and aliases.
+            subcommand=Style(fg=Color.cyan),
+            choice=Style(fg=Color.magenta),
+            metavar=Style(fg=Color.cyan, dim=True),
+            bracket=Style(dim=True),
+            envvar=Style(fg=Color.yellow, dim=True),
+            default=Style(fg=Color.green, dim=True, italic=True),
+            deprecated=Style(fg=Color.bright_yellow, bold=True),
+            search=Style(fg=Color.green, bold=True),
+            success=Style(fg=Color.green),
+            ### Non-canonical Click Extra styles.
+            subheading=Style(fg=Color.blue),
+        )
 
     @staticmethod
     def light() -> HelpExtraTheme:
         """A theme assuming a light terminal background color.
 
         .. todo::
-
-            Implement default light theme.
+            Tweak colors to make them more readable.
         """
-        raise NotImplementedError
+        return HelpExtraTheme.dark()
 
 
 # Populate our global theme with all default styles.
-default_theme = HelpExtraTheme(
-    ### Cloup styles.
-    invoked_command=Style(fg=Color.bright_white),
-    heading=Style(fg=Color.bright_blue, bold=True, underline=True),
-    constraint=Style(fg=Color.magenta),
-    # Neutralize Cloup's col1, as it interferes with our finer option styling
-    # which takes care of separators.
-    col1=identity,
-    # Style aliases like options and subcommands.
-    alias=Style(fg=Color.cyan),
-    # Style aliases punctuation like options, but dimmed.
-    alias_secondary=Style(fg=Color.cyan, dim=True),
-    ### Log styles.
-    critical=Style(fg=Color.red, bold=True),
-    error=Style(fg=Color.red),
-    warning=Style(fg=Color.yellow),
-    info=identity,  # INFO level is the default, so no style applied.
-    debug=Style(fg=Color.blue),
-    ### Click Extra styles.
-    option=Style(fg=Color.cyan),
-    # Style subcommands like options and aliases.
-    subcommand=Style(fg=Color.cyan),
-    choice=Style(fg=Color.magenta),
-    metavar=Style(fg=Color.cyan, dim=True),
-    bracket=Style(dim=True),
-    envvar=Style(fg=Color.yellow, dim=True),
-    default=Style(fg=Color.green, dim=True, italic=True),
-    deprecated=Style(fg=Color.bright_yellow, bold=True),
-    search=Style(fg=Color.green, bold=True),
-    success=Style(fg=Color.green),
-    ### Non-canonical Click Extra styles.
-    subheading=Style(fg=Color.blue),
-)
+default_theme = HelpExtraTheme.dark()
 
 
 # No color theme.
 nocolor_theme = HelpExtraTheme()
 
 
 OK = default_theme.success("✓")
```

### Comparing `click_extra-4.6.1/click_extra/commands.py` & `click_extra-4.6.2/click_extra/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -376,34 +376,23 @@
                     # TODO: pretty print JSON output (easier to read in bug reports)?
                     logger.debug(line)
 
         return super().invoke(ctx)
 
 
 class ExtraGroup(ExtraCommand, Group):  # type: ignore[misc]
-    """Same as ``cloup.group``, but with sane defaults and extra help screen
-    colorization."""
+    """Like``cloup.Group``, with sane defaults and extra help screen colorization."""
 
     command_class = ExtraCommand
     """Makes commands of an ``ExtraGroup`` be instances of ``ExtraCommand``.
 
     That way all subcommands created from an ``ExtraGroup`` benefits from the same
     defaults and extra help screen colorization.
 
-    Fixes `click-extra#479 <https://github.com/kdeldycke/click-extra/issues/479>`_.
+    See: https://click.palletsprojects.com/en/8.1.x/api/#click.Group.command_class
     """
 
-    def command(self, *args, **kwargs):
-        """Bypass ``cloup.Group.command()`` to produce an ``ExtraCommand`` decorator.
+    group_class = type
+    """Let ``ExtraGroup`` produce sub-groups that are also of ``ExtraGroup`` type.
 
-        Starts the seach for the ``command()`` method after the ``cloup.Group`` class
-        in the MRO chain, effectively bypassing ``cloup.Group.command()``, which does
-        not support the ``command_class`` property.
-
-        .. todo::
-            Removes this workaround when `Cloup issue #160 is addressed
-            <https://github.com/janluke/cloup/issues/160>`_.
-
-        .. todo::
-            Allow this decorator to be called without parenthesis.
-        """
-        return super(cloup.Group, self).command(*args, **kwargs)
+    See: https://click.palletsprojects.com/en/8.1.x/api/#click.Group.group_class
+    """
```

### Comparing `click_extra-4.6.1/click_extra/config.py` & `click_extra-4.6.2/click_extra/config.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/decorators.py` & `click_extra-4.6.2/click_extra/decorators.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/docs_update.py` & `click_extra-4.6.2/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/logging.py` & `click_extra-4.6.2/click_extra/logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/parameters.py` & `click_extra-4.6.2/click_extra/parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/platforms.py` & `click_extra-4.6.2/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/pygments.py` & `click_extra-4.6.2/click_extra/pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/sphinx.py` & `click_extra-4.6.2/click_extra/sphinx.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tabulate.py` & `click_extra-4.6.2/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/telemetry.py` & `click_extra-4.6.2/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/testing.py` & `click_extra-4.6.2/click_extra/testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/__init__.py` & `click_extra-4.6.2/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/conftest.py` & `click_extra-4.6.2/click_extra/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_colorize.py` & `click_extra-4.6.2/click_extra/tests/test_colorize.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import click
 import cloup
 import pytest
 from boltons.strutils import strip_ansi
 from pytest_cases import parametrize
 
 from click_extra import (
+    Color,
     HelpTheme,
     Style,
     argument,
     echo,
     option,
     option_group,
     pass_context,
@@ -63,19 +64,45 @@
     skip_windows_colors,
 )
 
 
 def test_theme_definition():
     """Ensure we do not leave any property we would have inherited from cloup and
     logging primitives."""
-    assert set(HelpTheme._fields).issubset(HelpExtraTheme._fields)
+    assert set(HelpTheme.__dataclass_fields__).issubset(
+        HelpExtraTheme.__dataclass_fields__,
+    )
 
     log_levels = {level.lower() for level in LOG_LEVELS}
-    assert log_levels.issubset(HelpExtraTheme._fields)
-    assert log_levels.isdisjoint(HelpTheme._fields)
+    assert log_levels.issubset(HelpExtraTheme.__dataclass_fields__)
+    assert log_levels.isdisjoint(HelpTheme.__dataclass_fields__)
+
+
+def test_extra_theme():
+    theme = HelpExtraTheme()
+
+    # Check the same instance is returned when no attribute is set.
+    assert theme.with_() == theme
+    assert theme.with_() is theme
+
+    # Check that we can't set a non-existing attribute.
+    with pytest.raises(TypeError):
+        theme.with_(random_arg=Style())
+
+    # Create a new theme with a different color.
+    assert theme.choice != Style(fg=Color.magenta)
+    new_theme = theme.with_(choice=Style(fg=Color.magenta))
+    assert new_theme != theme
+    assert new_theme is not theme
+    assert new_theme.choice == Style(fg=Color.magenta)
+
+    # Derives a second theme from the first one.
+    second_theme = new_theme.with_(choice=Style(fg=Color.magenta))
+    assert second_theme == new_theme
+    assert second_theme is new_theme
 
 
 def test_options_highlight():
     formatter = HelpExtraFormatter()
     formatter.write("applies filtering by --manager and --exclude options")
 
     formatter.long_options = {"--manager", "--exclude"}
```

### Comparing `click_extra-4.6.1/click_extra/tests/test_commands.py` & `click_extra-4.6.2/click_extra/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_config.py` & `click_extra-4.6.2/click_extra/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_logging.py` & `click_extra-4.6.2/click_extra/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_parameters.py` & `click_extra-4.6.2/click_extra/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_platforms.py` & `click_extra-4.6.2/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_pygments.py` & `click_extra-4.6.2/click_extra/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_tabulate.py` & `click_extra-4.6.2/click_extra/tests/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_telemetry.py` & `click_extra-4.6.2/click_extra/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_testing.py` & `click_extra-4.6.2/click_extra/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_timer.py` & `click_extra-4.6.2/click_extra/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/tests/test_version.py` & `click_extra-4.6.2/click_extra/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/timer.py` & `click_extra-4.6.2/click_extra/timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/click_extra/version.py` & `click_extra-4.6.2/click_extra/version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/pyproject.toml` & `click_extra-4.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.6.1"
+version = "4.6.2"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -72,16 +72,17 @@
 # Investigation of the root cause is being discussed upstream at:
 # https://github.com/mahmoud/boltons/issues/334
 boltons = "^23.0.0"
 # Click 8.1.4 fix @group.command calls with a custom command_class. See:
 # https://github.com/pallets/click/issues/2416
 # https://github.com/pallets/click/pull/2417
 click = "^8.1.4"
-# Cloup 2.1.1 fix heading colorization.
-cloup = "^2.1.1"
+# Cloup 3.0.0 changed HelpTheme to a dataclass. See:
+# https://github.com/janluke/cloup/pull/163
+cloup = "^3.0.0"
 commentjson = "^0.9.0"
 mergedeep = "^1.3.4"
 # Pallets-Sphinx-Themes 2.1.1 is the first version removing old and conflicting Python 2 code.
 Pallets-Sphinx-Themes = "^2.1.1"
 # Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
 pygments = "^2.14"
 # pygments-ansi-color 0.3.0 is the first version to set the default theme of ANSI colors.
@@ -182,15 +183,15 @@
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
 [tool.bumpversion]
-current_version = "4.6.1"
+current_version = "4.6.2"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./click_extra/__init__.py"
 
 [[tool.bumpversion.files]]
 filename = "./pyproject.toml"
```

### Comparing `click_extra-4.6.1/readme.md` & `click_extra-4.6.2/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.6.1/PKG-INFO` & `click_extra-4.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.6.1
+Version: 4.6.2
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
@@ -38,15 +38,15 @@
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0)
 Requires-Dist: boltons (>=23.0.0,<24.0.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
-Requires-Dist: cloup (>=2.1.1,<3.0.0)
+Requires-Dist: cloup (>=3.0.0,<4.0.0)
 Requires-Dist: commentjson (>=0.9.0,<0.10.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pygments (>=2.14,<3.0)
 Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: regex (>=2023.3.22,<2024.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.6.1 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.6.2 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
@@ -21,15 +21,15 @@
 Classifier: Topic :: System :: Shells Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing :: Filters Classifier: Topic :: Text
 Processing :: Markup :: HTML Classifier: Topic :: Text Processing :: Markup ::
 Markdown Classifier: Topic :: Text Processing :: Markup :: XML Classifier:
 Topic :: Text Processing :: Markup :: reStructuredText Classifier: Topic ::
 Utilities Classifier: Typing :: Typed Requires-Dist: Pallets-Sphinx-Themes
 (>=2.1.1,<3.0.0) Requires-Dist: boltons (>=23.0.0,<24.0.0) Requires-Dist: click
-(>=8.1.4,<9.0.0) Requires-Dist: cloup (>=2.1.1,<3.0.0) Requires-Dist:
+(>=8.1.4,<9.0.0) Requires-Dist: cloup (>=3.0.0,<4.0.0) Requires-Dist:
 commentjson (>=0.9.0,<0.10.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pygments (>=2.14,<3.0) Requires-Dist: pygments-ansi-color
 (>=0.3.0,<0.4.0) Requires-Dist: pyyaml (>=6.0.0,<7.0.0) Requires-Dist: regex
 (>=2023.3.22,<2024.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-
 Dist: sphinx (>=6,<7) Requires-Dist: tabulate[widechars] (>=0.9,<0.10)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11" Requires-Dist:
 wcmatch (>=8.4.1,<9.0.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-
```

