# Comparing `tmp/jsonpath-extractor-0.8.0.tar.gz` & `tmp/jsonpath-extractor-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonpath-extractor-0.8.0.tar", last modified: Tue Aug 17 15:26:54 2021, max compression
+gzip compressed data, was "jsonpath-extractor-0.9.0.tar", last modified: Sat Jul 15 02:49:58 2023, max compression
```

## Comparing `jsonpath-extractor-0.8.0.tar` & `jsonpath-extractor-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5806 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      868 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/jsonpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/jsonpath/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    30237 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/jsonpath/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/jsonpath/lark.py
--rw-r--r--   0 runner    (1001) docker     (121)   129381 2021-08-17 15:26:54.242635 jsonpath-extractor-0.8.0/jsonpath/lark_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/jsonpath/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/jsonpath/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4816 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/jsonpath/transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/jsonpath_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2021-08-17 15:26:44.217963 jsonpath-extractor-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-17 15:26:44.221963 jsonpath-extractor-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2021-08-17 15:26:44.221963 jsonpath-extractor-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    13113 2021-08-17 15:26:44.221963 jsonpath-extractor-0.8.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)    15735 2021-08-17 15:26:44.221963 jsonpath-extractor-0.8.0/tests/test_lark.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-08-17 15:26:44.221963 jsonpath-extractor-0.8.0/tests/utils.py
--rw-------   0 runner    (1001) docker     (121)     8750 2021-08-17 15:26:54.330637 jsonpath-extractor-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4652 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/README.rst
+-rw-r--r--   0        0        0      868 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath/__init__.py
+-rw-r--r--   0        0        0     1318 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath/cli.py
+-rw-r--r--   0        0        0    30237 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath/core.py
+-rw-r--r--   0        0        0     1550 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath/grammar.lark
+-rw-r--r--   0        0        0      525 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath/lark.py
+-rw-r--r--   0        0        0   142139 2023-07-15 02:49:58.141529 jsonpath-extractor-0.9.0/jsonpath/lark_parser.py
+-rw-r--r--   0        0        0     1410 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath/parser.py
+-rw-r--r--   0        0        0        0 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath/py.typed
+-rw-r--r--   0        0        0     4810 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath/transformer.py
+-rw-r--r--   0        0        0     1542 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/jsonpath_build.py
+-rw-r--r--   0        0        0     1863 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1880 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/tests/test_cli.py
+-rw-r--r--   0        0        0    13113 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/tests/test_core.py
+-rw-r--r--   0        0        0    15802 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/tests/test_lark.py
+-rw-r--r--   0        0        0      400 2023-07-15 02:49:44.557213 jsonpath-extractor-0.9.0/tests/utils.py
+-rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 jsonpath-extractor-0.9.0/PKG-INFO
```

### Comparing `jsonpath-extractor-0.8.0/LICENSE` & `jsonpath-extractor-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonpath-extractor-0.8.0/README.rst` & `jsonpath-extractor-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: jsonpath-extractor
+Version: 0.9.0
+Summary: A selector expression for extracting data from JSON.
+License: MIT
+Keywords: data-extractor,data-extraction,jsonpath,json
+Author-email: 林玮 (Jade Lin) <linw1995@icloud.com>
+Requires-Python: >=3.8
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: parser
+Project-URL: documentation, https://jsonpath.rtfd.io/en/latest/
+Project-URL: homepage, https://github.com/linw1995/jsonpath
+Project-URL: repository, https://github.com/linw1995/jsonpath
+Description-Content-Type: text/x-rst
+
 ========
 JSONPATH
 ========
 
 |license| |Pypi Status| |Python version| |Package version| |PyPI - Downloads|
 |GitHub last commit| |Code style: black| |Build Status| |codecov| |PDM managed|
 
@@ -92,50 +118,21 @@
         "category": "Comic book"
       }
     ]
 
 Changelog
 <<<<<<<<<
 
-v0.8.0
+v0.9.0
 ~~~~~~
 
-Features
-********
-
-- 69ff6cb_ add iter_find and find_first methods
-- be22151_ better JSONPath object representations
-
-Refactor
-********
-
-- 9d9d78f_ raise AttributeError by object.__getattribute__
-- 4191b8c_ not registers base class "Expr" for chaining invocations
-
 Build
 *****
 
-- cc6ab56_ 2040721_ upgrade lark-parser package to latest
-- fb7e902_ fit with latest PDM
-- 10ea6d3_ excludes .mypy_cache for local build
-
-Fix
-***
-
-- 1dccec1_ fix: right way to generate standalone parser
-
-.. _69ff6cb: https://github.com/linw1995/jsonpath/commit/69ff6cb47a08d3f957224adb163970454b6a1c87
-.. _be22151: https://github.com/linw1995/jsonpath/commit/be221513bd8a1821e8007eb1c2d4f10aa6d3f987
-.. _9d9d78f: https://github.com/linw1995/jsonpath/commit/9d9d78fd60b7b284c446c06e7102d05decd24c2b
-.. _4191b8c: https://github.com/linw1995/jsonpath/commit/4191b8c745871733e58e97be11cdbcd845870484
-.. _cc6ab56: https://github.com/linw1995/jsonpath/commit/cc6ab56
-.. _2040721: https://github.com/linw1995/jsonpath/commit/2040721
-.. _1dccec1: https://github.com/linw1995/jsonpath/commit/1dccec1
-.. _fb7e902: https://github.com/linw1995/jsonpath/commit/fb7e902
-.. _10ea6d3: https://github.com/linw1995/jsonpath/commit/10ea6d3
+- Remove support for Python 3.7
 
 
 Contributing
 <<<<<<<<<<<<
 
 
 Environment Setup
@@ -151,15 +148,15 @@
 Setup the development environment.
 Please make sure you install the pdm_,
 pre-commit_ and nox_ CLIs in your environment.
 
 .. code-block:: shell
 
     make init
-    make PYTHON=3.7 init  # for specific python version
+    make PYTHON=3.8 init  # for specific python version
 
 Linting
 ~~~~~~~
 
 Use pre-commit_ for installing linters to ensure a good code style.
 
 .. code-block:: shell
@@ -232,7 +229,8 @@
     :target: https://github.com/linw1995/jsonpath/actions?query=workflow%3ALint%26Test
 
 .. |codecov| image:: https://codecov.io/gh/linw1995/jsonpath/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/linw1995/jsonpath
 
 .. |PDM managed| image:: https://img.shields.io/badge/pdm-managed-blueviolet
     :target: https://pdm.fming.dev
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jsonpath-extractor-0.8.0/jsonpath/__init__.py` & `jsonpath-extractor-0.9.0/jsonpath/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonpath-extractor-0.8.0/jsonpath/cli.py` & `jsonpath-extractor-0.9.0/jsonpath/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .parser import parse
 
 
 def cli(args: argparse.Namespace) -> None:
     try:
         jp = parse(args.expression)
     except JSONPathError as exc:
-        sys.exit(exc)
+        sys.exit(str(exc))
 
     if args.file:
         file_path = Path(args.file)
         with file_path.open() as f:
             data = json.load(f)
     elif not sys.stdin.isatty():
         data = json.load(sys.stdin)
```

### Comparing `jsonpath-extractor-0.8.0/jsonpath/core.py` & `jsonpath-extractor-0.9.0/jsonpath/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 from contextlib import contextmanager, suppress
 from contextvars import ContextVar
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
-    Iterable,
+    Iterator,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
-    cast,
 )
 from weakref import ReferenceType
 
 # Third Party Library
 from typing_extensions import Literal
 
 var_root: ContextVar[Any] = ContextVar("root")
@@ -129,15 +128,14 @@
     """
 
     _classes: Dict[str, "ExprMeta"] = {}
 
     def __new__(
         metacls, name: str, bases: Tuple[type], attr_dict: Dict[str, Any]
     ) -> "ExprMeta":
-
         if "find" not in attr_dict:
             return _create_expr_cls(metacls, name, bases, attr_dict)
 
         actual_find = attr_dict["find"]
 
         @functools.wraps(actual_find)
         def find(self: "Expr", element: Any) -> List[Any]:
@@ -160,17 +158,14 @@
 def _create_expr_cls(
     metacls: Type[ExprMeta],
     name: str,
     bases: Tuple[type],
     attr_dict: Dict[str, Any],
 ) -> ExprMeta:
     cls = type.__new__(metacls, name, bases, attr_dict)
-    # cast for the type checker
-    # https://mypy.readthedocs.io/en/stable/casts.html
-    cls = cast(ExprMeta, cls)
     if name != "Expr":
         # not registers the base class
         metacls._classes[name] = cls
 
     return cls
 
 
@@ -458,15 +453,19 @@
         super().__init__()
         self.name = name
 
     def _get_partial_expression(self) -> str:
         if self.name is None:
             return "*"
 
-        return self.name
+        name = self.name
+        if name in ("*", "$", "@"):
+            name = repr(name)
+
+        return name
 
     def find(self, element: Any) -> List[Any]:
         if not isinstance(element, dict):
             raise JSONPathFindError
 
         if self.name is None:
             return list(element.values())
@@ -569,21 +568,21 @@
             expr, Expr
         ), '"expr" parameter must be an instance of the "Expr" class.'
         self.expr = expr
 
     def _get_partial_expression(self) -> str:
         return f"[{self.expr.get_expression()}]"
 
-    def find(self, element: Any) -> List[Any]:
+    def find(self, element: Union[List[Any], Dict[str, Any]]) -> List[Any]:
         filtered_items = []
-        items: Union[Iterable[Tuple[int, Any]], Iterable[Tuple[str, Any]]]
+        items: Union[Iterator[tuple[str, Any]], Iterator[tuple[int, Any]]]
         if isinstance(element, list):
-            items = enumerate(element)
+            items = iter(enumerate(element))
         elif isinstance(element, dict):
-            items = element.items()
+            items = iter(element.items())
         else:
             raise JSONPathFindError
 
         for item in items:
             # save the current item into var_self for Self()
             with temporary_set(var_self, item):
                 _, value = item
@@ -688,25 +687,25 @@
     >>> p = Brace(p); print(p.get_expression())
     ($[*].a)
     >>> p.find([{"a": 1}])
     [[1]]
 
     It seems to be useless but makes chaining filtering become possible.
     The expressions like `"$[@ < 100][@ >= 50]"` can not perform chaining filtering.
-    Because the Preidcate (and Array) class always unarrays the found elements to
+    Because the Predicate (and Array) class always unpacks the found elements to
     avoid the found result looking like `[[[[[[[...]]]]]]]`.
     So the right way to do chaining filter is that it should use with Brace class.
 
     >>> p = Brace(Root().Predicate(Self() < 100)).Predicate(Self() >= 50)
     >>> print(p.get_expression())
     ($[@ < 100])[@ >= 50]
     >>> p.find([100, 99, 50, 1])
     [99, 50]
 
-    Generally, we will use And expresion do that. e.g. `"$[@ < 100 and @ >= 50]"`
+    Generally, we will use And expression do that. e.g. `"$[@ < 100 and @ >= 50]"`
 
     >>> p = Brace(
     ...     Root().Array().Name("a")
     ... ).Predicate(Self() == 1)
     >>> print(p.get_expression())
     ($[*].a)[@ = 1]
     >>> p.find([{"a": 1}, {"a": 2}, {"a": 1}, {}])
```

### Comparing `jsonpath-extractor-0.8.0/jsonpath/lark.py` & `jsonpath-extractor-0.9.0/jsonpath/lark.py`

 * *Files identical despite different names*

### Comparing `jsonpath-extractor-0.8.0/jsonpath/lark_parser.py` & `jsonpath-extractor-0.9.0/jsonpath/lark_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# The file was automatically generated by Lark v0.11.3
-__version__ = "0.11.3"
+# The file was automatically generated by Lark v1.1.5
+__version__ = "1.1.5"
 
 #
 #
 #   Lark Stand-alone Generator Tool
 # ----------------------------------
-# Generates a stand-alone LALR(1) parser with a standard lexer
+# Generates a stand-alone LALR(1) parser
 #
 # Git:    https://github.com/erezsh/lark
 # Author: Erez Shinan (erezshin@gmail.com)
 #
 #
 #    >>> LICENSE
 #
@@ -22,27 +22,33 @@
 #    generated code, you may contact me via email or otherwise.
 #
 #    If MPL2 is incompatible with your free or open-source project,
 #    contact me and we'll work it out.
 #
 #
 
-from io import open
-
+from abc import ABC, abstractmethod
+from collections.abc import Sequence
+from types import ModuleType
+from typing import (
+    TypeVar, Generic, Type, Tuple, List, Dict, Iterator, Collection, Callable, Optional, FrozenSet, Any,
+    Union, Iterable, IO, TYPE_CHECKING, overload,
+    Pattern as REPattern, ClassVar, Set, Mapping
+)
 
 
 class LarkError(Exception):
     pass
 
 
 class ConfigurationError(LarkError, ValueError):
     pass
 
 
-def assert_config(value, options, msg='Got %r, expected one of %s'):
+def assert_config(value, options: Collection, msg='Got %r, expected one of %s'):
     if value not in options:
         raise ConfigurationError(msg % (value, options))
 
 
 class GrammarError(LarkError):
     pass
 
@@ -50,106 +56,131 @@
 class ParseError(LarkError):
     pass
 
 
 class LexError(LarkError):
     pass
 
+T = TypeVar('T')
 
 class UnexpectedInput(LarkError):
     #--
+    line: int
+    column: int
     pos_in_stream = None
+    state: Any
     _terminals_by_name = None
 
-    def get_context(self, text, span=40):
+    def get_context(self, text: str, span: int=40) -> str:
         #--
         assert self.pos_in_stream is not None, self
         pos = self.pos_in_stream
         start = max(pos - span, 0)
         end = pos + span
         if not isinstance(text, bytes):
             before = text[start:pos].rsplit('\n', 1)[-1]
             after = text[pos:end].split('\n', 1)[0]
             return before + after + '\n' + ' ' * len(before.expandtabs()) + '^\n'
         else:
             before = text[start:pos].rsplit(b'\n', 1)[-1]
             after = text[pos:end].split(b'\n', 1)[0]
             return (before + after + b'\n' + b' ' * len(before.expandtabs()) + b'^\n').decode("ascii", "backslashreplace")
 
-    def match_examples(self, parse_fn, examples, token_type_match_fallback=False, use_accepts=False):
+    def match_examples(self, parse_fn: 'Callable[[str], Tree]',
+                             examples: Union[Mapping[T, Iterable[str]], Iterable[Tuple[T, Iterable[str]]]],
+                             token_type_match_fallback: bool=False,
+                             use_accepts: bool=True
+                         ) -> Optional[T]:
         #--
         assert self.state is not None, "Not supported for this exception"
 
-        if isinstance(examples, dict):
+        if isinstance(examples, Mapping):
             examples = examples.items()
 
         candidate = (None, False)
         for i, (label, example) in enumerate(examples):
-            assert not isinstance(example, STRING_TYPE)
+            assert not isinstance(example, str), "Expecting a list"
 
             for j, malformed in enumerate(example):
                 try:
                     parse_fn(malformed)
                 except UnexpectedInput as ut:
                     if ut.state == self.state:
-                        if use_accepts and hasattr(self, 'accepts') and ut.accepts != self.accepts:
+                        if (
+                            use_accepts
+                            and isinstance(self, UnexpectedToken)
+                            and isinstance(ut, UnexpectedToken)
+                            and ut.accepts != self.accepts
+                        ):
                             logger.debug("Different accepts with same state[%d]: %s != %s at example [%s][%s]" %
                                          (self.state, self.accepts, ut.accepts, i, j))
                             continue
-                        try:
+                        if (
+                            isinstance(self, (UnexpectedToken, UnexpectedEOF))
+                            and isinstance(ut, (UnexpectedToken, UnexpectedEOF))
+                        ):
                             if ut.token == self.token:  ##
 
                                 logger.debug("Exact Match at example [%s][%s]" % (i, j))
                                 return label
 
                             if token_type_match_fallback:
                                 ##
 
                                 if (ut.token.type == self.token.type) and not candidate[-1]:
                                     logger.debug("Token Type Fallback at example [%s][%s]" % (i, j))
                                     candidate = label, True
 
-                        except AttributeError:
-                            pass
                         if candidate[0] is None:
                             logger.debug("Same State match at example [%s][%s]" % (i, j))
                             candidate = label, False
 
         return candidate[0]
 
     def _format_expected(self, expected):
         if self._terminals_by_name:
             d = self._terminals_by_name
             expected = [d[t_name].user_repr() if t_name in d else t_name for t_name in expected]
         return "Expected one of: \n\t* %s\n" % '\n\t* '.join(expected)
 
 
 class UnexpectedEOF(ParseError, UnexpectedInput):
+    #--
+    expected: 'List[Token]'
+
     def __init__(self, expected, state=None, terminals_by_name=None):
+        super(UnexpectedEOF, self).__init__()
+
         self.expected = expected
         self.state = state
         from .lexer import Token
         self.token = Token("<EOF>", "")  ##
 
         self.pos_in_stream = -1
         self.line = -1
         self.column = -1
         self._terminals_by_name = terminals_by_name
 
-        super(UnexpectedEOF, self).__init__()
 
     def __str__(self):
         message = "Unexpected end-of-input. "
         message += self._format_expected(self.expected)
         return message
 
 
 class UnexpectedCharacters(LexError, UnexpectedInput):
+    #--
+
+    allowed: Set[str]
+    considered_tokens: Set[Any]
+
     def __init__(self, seq, lex_pos, line, column, allowed=None, considered_tokens=None, state=None, token_history=None,
                  terminals_by_name=None, considered_rules=None):
+        super(UnexpectedCharacters, self).__init__()
+
         ##
 
         self.line = line
         self.column = column
         self.pos_in_stream = lex_pos
         self.state = state
         self._terminals_by_name = terminals_by_name
@@ -161,384 +192,433 @@
 
         if isinstance(seq, bytes):
             self.char = seq[lex_pos:lex_pos + 1].decode("ascii", "backslashreplace")
         else:
             self.char = seq[lex_pos]
         self._context = self.get_context(seq)
 
-        super(UnexpectedCharacters, self).__init__()
 
     def __str__(self):
         message = "No terminal matches '%s' in the current parser context, at line %d col %d" % (self.char, self.line, self.column)
         message += '\n\n' + self._context
         if self.allowed:
             message += self._format_expected(self.allowed)
         if self.token_history:
             message += '\nPrevious tokens: %s\n' % ', '.join(repr(t) for t in self.token_history)
         return message
 
 
 class UnexpectedToken(ParseError, UnexpectedInput):
     #--
 
+    expected: Set[str]
+    considered_rules: Set[str]
+    interactive_parser: 'InteractiveParser'
+
     def __init__(self, token, expected, considered_rules=None, state=None, interactive_parser=None, terminals_by_name=None, token_history=None):
+        super(UnexpectedToken, self).__init__()
+
         ##
 
         self.line = getattr(token, 'line', '?')
         self.column = getattr(token, 'column', '?')
-        self.pos_in_stream = getattr(token, 'pos_in_stream', None)
+        self.pos_in_stream = getattr(token, 'start_pos', None)
         self.state = state
 
         self.token = token
         self.expected = expected  ##
 
         self._accepts = NO_VALUE
         self.considered_rules = considered_rules
         self.interactive_parser = interactive_parser
         self._terminals_by_name = terminals_by_name
         self.token_history = token_history
 
-        super(UnexpectedToken, self).__init__()
 
     @property
-    def accepts(self):
+    def accepts(self) -> Set[str]:
         if self._accepts is NO_VALUE:
             self._accepts = self.interactive_parser and self.interactive_parser.accepts()
         return self._accepts
 
     def __str__(self):
         message = ("Unexpected token %r at line %s, column %s.\n%s"
                    % (self.token, self.line, self.column, self._format_expected(self.accepts or self.expected)))
         if self.token_history:
             message += "Previous tokens: %r\n" % self.token_history
 
         return message
 
-    @property
-    def puppet(self):
-        warn("UnexpectedToken.puppet attribute has been renamed to interactive_parser", DeprecationWarning)
-        return self.interactive_parser
-    
 
 
 class VisitError(LarkError):
     #--
 
+    obj: 'Union[Tree, Token]'
+    orig_exc: Exception
+
     def __init__(self, rule, obj, orig_exc):
+        message = 'Error trying to process rule "%s":\n\n%s' % (rule, orig_exc)
+        super(VisitError, self).__init__(message)
+
+        self.rule = rule
         self.obj = obj
         self.orig_exc = orig_exc
 
-        message = 'Error trying to process rule "%s":\n\n%s' % (rule, orig_exc)
-        super(VisitError, self).__init__(message)
+
+class MissingVariableError(LarkError):
+    pass
 
 
 import sys, re
 import logging
-from io import open
-logger = logging.getLogger("lark")
+
+logger: logging.Logger = logging.getLogger("lark")
 logger.addHandler(logging.StreamHandler())
 ##
 
 ##
 
 logger.setLevel(logging.CRITICAL)
 
-if sys.version_info[0]>2:
-    from abc import ABC, abstractmethod
-else:
-    from abc import ABCMeta, abstractmethod
-    class ABC(object): ##
-
-        __slots__ = ()
-        __metclass__ = ABCMeta
-
-
-Py36 = (sys.version_info[:2] >= (3, 6))
 
 NO_VALUE = object()
 
+T = TypeVar("T")
+
 
-def classify(seq, key=None, value=None):
-    d = {}
+def classify(seq: Sequence, key: Optional[Callable] = None, value: Optional[Callable] = None) -> Dict:
+    d: Dict[Any, Any] = {}
     for item in seq:
         k = key(item) if (key is not None) else item
         v = value(item) if (value is not None) else item
         if k in d:
             d[k].append(v)
         else:
             d[k] = [v]
     return d
 
 
-def _deserialize(data, namespace, memo):
+def _deserialize(data: Any, namespace: Dict[str, Any], memo: Dict) -> Any:
     if isinstance(data, dict):
         if '__type__' in data:  ##
 
             class_ = namespace[data['__type__']]
             return class_.deserialize(data, memo)
         elif '@' in data:
             return memo[data['@']]
         return {key:_deserialize(value, namespace, memo) for key, value in data.items()}
     elif isinstance(data, list):
         return [_deserialize(value, namespace, memo) for value in data]
     return data
 
 
-class Serialize(object):
+_T = TypeVar("_T", bound="Serialize")
+
+class Serialize:
     #--
 
-    def memo_serialize(self, types_to_memoize):
+    def memo_serialize(self, types_to_memoize: List) -> Any:
         memo = SerializeMemoizer(types_to_memoize)
         return self.serialize(memo), memo.serialize()
 
-    def serialize(self, memo=None):
+    def serialize(self, memo = None) -> Dict[str, Any]:
         if memo and memo.in_types(self):
             return {'@': memo.memoized.get(self)}
 
         fields = getattr(self, '__serialize_fields__')
         res = {f: _serialize(getattr(self, f), memo) for f in fields}
         res['__type__'] = type(self).__name__
-        postprocess = getattr(self, '_serialize', None)
-        if postprocess:
-            postprocess(res, memo)
+        if hasattr(self, '_serialize'):
+            self._serialize(res, memo)  ##
+
         return res
 
     @classmethod
-    def deserialize(cls, data, memo):
-        namespace = getattr(cls, '__serialize_namespace__', {})
+    def deserialize(cls: Type[_T], data: Dict[str, Any], memo: Dict[int, Any]) -> _T:
+        namespace = getattr(cls, '__serialize_namespace__', [])
         namespace = {c.__name__:c for c in namespace}
 
         fields = getattr(cls, '__serialize_fields__')
 
         if '@' in data:
             return memo[data['@']]
 
         inst = cls.__new__(cls)
         for f in fields:
             try:
                 setattr(inst, f, _deserialize(data[f], namespace, memo))
             except KeyError as e:
                 raise KeyError("Cannot find key for class", cls, e)
-        postprocess = getattr(inst, '_deserialize', None)
-        if postprocess:
-            postprocess()
+
+        if hasattr(inst, '_deserialize'):
+            inst._deserialize()  ##
+
+
         return inst
 
 
 class SerializeMemoizer(Serialize):
     #--
 
     __serialize_fields__ = 'memoized',
 
-    def __init__(self, types_to_memoize):
+    def __init__(self, types_to_memoize: List) -> None:
         self.types_to_memoize = tuple(types_to_memoize)
         self.memoized = Enumerator()
 
-    def in_types(self, value):
+    def in_types(self, value: Serialize) -> bool:
         return isinstance(value, self.types_to_memoize)
 
-    def serialize(self):
+    def serialize(self) -> Dict[int, Any]:  ##
+
         return _serialize(self.memoized.reversed(), None)
 
     @classmethod
-    def deserialize(cls, data, namespace, memo):
-        return _deserialize(data, namespace, memo)
-
-
-try:
-    STRING_TYPE = basestring
-except NameError:   ##
-
-    STRING_TYPE = str
-
-
-import types
-from functools import wraps, partial
-from contextlib import contextmanager
-
-Str = type(u'')
-try:
-    classtype = types.ClassType  ##
-
-except AttributeError:
-    classtype = type    ##
-
-
-
-def smart_decorator(f, create_decorator):
-    if isinstance(f, types.FunctionType):
-        return wraps(f)(create_decorator(f, True))
+    def deserialize(cls, data: Dict[int, Any], namespace: Dict[str, Any], memo: Dict[Any, Any]) -> Dict[int, Any]:  ##
 
-    elif isinstance(f, (classtype, type, types.BuiltinFunctionType)):
-        return wraps(f)(create_decorator(f, False))
-
-    elif isinstance(f, types.MethodType):
-        return wraps(f)(create_decorator(f.__func__, True))
-
-    elif isinstance(f, partial):
-        ##
-
-        return wraps(f.func)(create_decorator(lambda *args, **kw: f(*args[1:], **kw), True))
-
-    else:
-        return create_decorator(f.__func__.__call__, True)
+        return _deserialize(data, namespace, memo)
 
 
 try:
     import regex
+    _has_regex = True
 except ImportError:
-    regex = None
+    _has_regex = False
+
+if sys.version_info >= (3, 11):
+    import re._parser as sre_parse
+    import re._constants as sre_constants
+else:
+    import sre_parse
+    import sre_constants
 
-import sre_parse
-import sre_constants
 categ_pattern = re.compile(r'\\p{[A-Za-z_]+}')
 
-def get_regexp_width(expr):
-    if regex:
+def get_regexp_width(expr: str) -> Union[Tuple[int, int], List[int]]:
+    if _has_regex:
         ##
 
         ##
 
         ##
 
         regexp_final = re.sub(categ_pattern, 'A', expr)
     else:
         if re.search(categ_pattern, expr):
             raise ImportError('`regex` module must be installed in order to use Unicode categories.', expr)
         regexp_final = expr
     try:
-        return [int(x) for x in sre_parse.parse(regexp_final).getwidth()]
+        ##
+
+        return [int(x) for x in sre_parse.parse(regexp_final).getwidth()]   ##
+
     except sre_constants.error:
-        raise ValueError(expr)
+        if not _has_regex:
+            raise ValueError(expr)
+        else:
+            ##
 
+            ##
 
-from collections import OrderedDict
+            c = regex.compile(regexp_final)
+            if c.match('') is None:
+                ##
+
+                return 1, int(sre_constants.MAXREPEAT)
+            else:
+                return 0, int(sre_constants.MAXREPEAT)
 
 
+from collections import OrderedDict
+
 class Meta:
+
+    empty: bool
+    line: int
+    column: int
+    start_pos: int
+    end_line: int
+    end_column: int
+    end_pos: int
+    orig_expansion: 'List[TerminalDef]'
+    match_tree: bool
+
     def __init__(self):
         self.empty = True
 
 
-class Tree(object):
+_Leaf_T = TypeVar("_Leaf_T")
+Branch = Union[_Leaf_T, 'Tree[_Leaf_T]']
+
+
+class Tree(Generic[_Leaf_T]):
     #--
-    def __init__(self, data, children, meta=None):
+
+    data: str
+    children: 'List[Branch[_Leaf_T]]'
+
+    def __init__(self, data: str, children: 'List[Branch[_Leaf_T]]', meta: Optional[Meta]=None) -> None:
         self.data = data
         self.children = children
         self._meta = meta
 
     @property
-    def meta(self):
+    def meta(self) -> Meta:
         if self._meta is None:
             self._meta = Meta()
         return self._meta
 
     def __repr__(self):
         return 'Tree(%r, %r)' % (self.data, self.children)
 
     def _pretty_label(self):
         return self.data
 
     def _pretty(self, level, indent_str):
+        yield f'{indent_str*level}{self._pretty_label()}'
         if len(self.children) == 1 and not isinstance(self.children[0], Tree):
-            return [indent_str*level, self._pretty_label(), '\t', '%s' % (self.children[0],), '\n']
-
-        l = [indent_str*level, self._pretty_label(), '\n']
-        for n in self.children:
-            if isinstance(n, Tree):
-                l += n._pretty(level+1, indent_str)
-            else:
-                l += [indent_str*(level+1), '%s' % (n,), '\n']
-
-        return l
+            yield f'\t{self.children[0]}\n'
+        else:
+            yield '\n'
+            for n in self.children:
+                if isinstance(n, Tree):
+                    yield from n._pretty(level+1, indent_str)
+                else:
+                    yield f'{indent_str*(level+1)}{n}\n'
 
-    def pretty(self, indent_str='  '):
+    def pretty(self, indent_str: str='  ') -> str:
         #--
         return ''.join(self._pretty(0, indent_str))
 
+    def __rich__(self, parent:'rich.tree.Tree'=None) -> 'rich.tree.Tree':
+        #--
+        return self._rich(parent)
+
+    def _rich(self, parent):
+        if parent:
+            tree = parent.add(f'[bold]{self.data}[/bold]')
+        else:
+            import rich.tree
+            tree = rich.tree.Tree(self.data)
+
+        for c in self.children:
+            if isinstance(c, Tree):
+                c._rich(tree)
+            else:
+                tree.add(f'[green]{c}[/green]')
+
+        return tree
+
     def __eq__(self, other):
         try:
             return self.data == other.data and self.children == other.children
         except AttributeError:
             return False
 
     def __ne__(self, other):
         return not (self == other)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash((self.data, tuple(self.children)))
 
-    def iter_subtrees(self):
+    def iter_subtrees(self) -> 'Iterator[Tree[_Leaf_T]]':
         #--
         queue = [self]
         subtrees = OrderedDict()
         for subtree in queue:
             subtrees[id(subtree)] = subtree
-            queue += [c for c in reversed(subtree.children)
+            ##
+
+            queue += [c for c in reversed(subtree.children)  ##
+
                       if isinstance(c, Tree) and id(c) not in subtrees]
 
         del queue
         return reversed(list(subtrees.values()))
 
-    def find_pred(self, pred):
+    def iter_subtrees_topdown(self):
+        #--
+        stack = [self]
+        stack_append = stack.append
+        stack_pop = stack.pop
+        while stack:
+            node = stack_pop()
+            if not isinstance(node, Tree):
+                continue
+            yield node
+            for child in reversed(node.children):
+                stack_append(child)
+
+    def find_pred(self, pred: 'Callable[[Tree[_Leaf_T]], bool]') -> 'Iterator[Tree[_Leaf_T]]':
         #--
         return filter(pred, self.iter_subtrees())
 
-    def find_data(self, data):
+    def find_data(self, data: str) -> 'Iterator[Tree[_Leaf_T]]':
         #--
         return self.find_pred(lambda t: t.data == data)
 
 
+from functools import wraps, update_wrapper
 from inspect import getmembers, getmro
 
+_Return_T = TypeVar('_Return_T')
+_Return_V = TypeVar('_Return_V')
+_Leaf_T = TypeVar('_Leaf_T')
+_Leaf_U = TypeVar('_Leaf_U')
+_R = TypeVar('_R')
+_FUNC = Callable[..., _Return_T]
+_DECORATED = Union[_FUNC, type]
 
-class Discard(Exception):
+class _DiscardType:
     #--
-    pass
 
-##
+    def __repr__(self):
+        return "lark.visitors.Discard"
+
+Discard = _DiscardType()
 
+##
 
 
 class _Decoratable:
     #--
 
     @classmethod
-    def _apply_decorator(cls, decorator, **kwargs):
+    def _apply_v_args(cls, visit_wrapper):
         mro = getmro(cls)
         assert mro[0] is cls
         libmembers = {name for _cls in mro[1:] for name, _ in getmembers(_cls)}
         for name, value in getmembers(cls):
 
             ##
 
             if name.startswith('_') or (name in libmembers and name not in cls.__dict__):
                 continue
             if not callable(value):
                 continue
 
             ##
 
-            if hasattr(cls.__dict__[name], 'vargs_applied') or hasattr(value, 'vargs_applied'):
+            if isinstance(cls.__dict__[name], _VArgsWrapper):
                 continue
 
-            static = isinstance(cls.__dict__[name], (staticmethod, classmethod))
-            setattr(cls, name, decorator(value, static=static, **kwargs))
+            setattr(cls, name, _VArgsWrapper(cls.__dict__[name], visit_wrapper))
         return cls
 
     def __class_getitem__(cls, _):
         return cls
 
 
-class Transformer(_Decoratable):
+class Transformer(_Decoratable, ABC, Generic[_Leaf_T, _Return_T]):
     #--
     __visit_tokens__ = True   ##
 
 
-    def __init__(self,  visit_tokens=True):
+    def __init__(self,  visit_tokens: bool=True) -> None:
         self.__visit_tokens__ = visit_tokens
 
     def _call_userfunc(self, tree, new_children=None):
         ##
 
         children = new_children if new_children is not None else tree.children
         try:
@@ -548,139 +628,180 @@
         else:
             try:
                 wrapper = getattr(f, 'visit_wrapper', None)
                 if wrapper is not None:
                     return f.visit_wrapper(f, tree.data, children, tree.meta)
                 else:
                     return f(children)
-            except (GrammarError, Discard):
+            except GrammarError:
                 raise
             except Exception as e:
                 raise VisitError(tree.data, tree, e)
 
     def _call_userfunc_token(self, token):
         try:
             f = getattr(self, token.type)
         except AttributeError:
             return self.__default_token__(token)
         else:
             try:
                 return f(token)
-            except (GrammarError, Discard):
+            except GrammarError:
                 raise
             except Exception as e:
                 raise VisitError(token.type, token, e)
 
     def _transform_children(self, children):
         for c in children:
-            try:
-                if isinstance(c, Tree):
-                    yield self._transform_tree(c)
-                elif self.__visit_tokens__ and isinstance(c, Token):
-                    yield self._call_userfunc_token(c)
-                else:
-                    yield c
-            except Discard:
-                pass
+            if isinstance(c, Tree):
+                res = self._transform_tree(c)
+            elif self.__visit_tokens__ and isinstance(c, Token):
+                res = self._call_userfunc_token(c)
+            else:
+                res = c
+
+            if res is not Discard:
+                yield res
 
     def _transform_tree(self, tree):
         children = list(self._transform_children(tree.children))
         return self._call_userfunc(tree, children)
 
-    def transform(self, tree):
+    def transform(self, tree: Tree[_Leaf_T]) -> _Return_T:
         #--
         return self._transform_tree(tree)
 
-    def __mul__(self, other):
+    def __mul__(
+            self: 'Transformer[_Leaf_T, Tree[_Leaf_U]]',
+            other: 'Union[Transformer[_Leaf_U, _Return_V], TransformerChain[_Leaf_U, _Return_V,]]'
+    ) -> 'TransformerChain[_Leaf_T, _Return_V]':
         #--
         return TransformerChain(self, other)
 
     def __default__(self, data, children, meta):
         #--
         return Tree(data, children, meta)
 
     def __default_token__(self, token):
         #--
         return token
 
 
+def merge_transformers(base_transformer=None, **transformers_to_merge):
+    #--
+    if base_transformer is None:
+        base_transformer = Transformer()
+    for prefix, transformer in transformers_to_merge.items():
+        for method_name in dir(transformer):
+            method = getattr(transformer, method_name)
+            if not callable(method):
+                continue
+            if method_name.startswith("_") or method_name == "transform":
+                continue
+            prefixed_method = prefix + "__" + method_name
+            if hasattr(base_transformer, prefixed_method):
+                raise AttributeError("Cannot merge: method '%s' appears more than once" % prefixed_method)
+
+            setattr(base_transformer, prefixed_method, method)
+
+    return base_transformer
+
+
 class InlineTransformer(Transformer):   ##
 
     def _call_userfunc(self, tree, new_children=None):
         ##
 
         children = new_children if new_children is not None else tree.children
         try:
             f = getattr(self, tree.data)
         except AttributeError:
             return self.__default__(tree.data, children, tree.meta)
         else:
             return f(*children)
 
 
-class TransformerChain(object):
-    def __init__(self, *transformers):
+class TransformerChain(Generic[_Leaf_T, _Return_T]):
+
+    transformers: 'Tuple[Union[Transformer, TransformerChain], ...]'
+
+    def __init__(self, *transformers: 'Union[Transformer, TransformerChain]') -> None:
         self.transformers = transformers
 
-    def transform(self, tree):
+    def transform(self, tree: Tree[_Leaf_T]) -> _Return_T:
         for t in self.transformers:
             tree = t.transform(tree)
-        return tree
+        return cast(_Return_T, tree)
 
-    def __mul__(self, other):
+    def __mul__(
+            self: 'TransformerChain[_Leaf_T, Tree[_Leaf_U]]',
+            other: 'Union[Transformer[_Leaf_U, _Return_V], TransformerChain[_Leaf_U, _Return_V]]'
+    ) -> 'TransformerChain[_Leaf_T, _Return_V]':
         return TransformerChain(*self.transformers + (other,))
 
 
 class Transformer_InPlace(Transformer):
     #--
     def _transform_tree(self, tree):           ##
 
         return self._call_userfunc(tree)
 
-    def transform(self, tree):
+    def transform(self, tree: Tree[_Leaf_T]) -> _Return_T:
         for subtree in tree.iter_subtrees():
             subtree.children = list(self._transform_children(subtree.children))
 
         return self._transform_tree(tree)
 
 
 class Transformer_NonRecursive(Transformer):
     #--
 
-    def transform(self, tree):
+    def transform(self, tree: Tree[_Leaf_T]) -> _Return_T:
         ##
 
         rev_postfix = []
-        q = [tree]
+        q: List[Branch[_Leaf_T]] = [tree]
         while q:
             t = q.pop()
             rev_postfix.append(t)
             if isinstance(t, Tree):
                 q += t.children
 
         ##
 
-        stack = []
+        stack: List = []
         for x in reversed(rev_postfix):
             if isinstance(x, Tree):
                 size = len(x.children)
                 if size:
                     args = stack[-size:]
                     del stack[-size:]
                 else:
                     args = []
-                stack.append(self._call_userfunc(x, args))
+
+                res = self._call_userfunc(x, args)
+                if res is not Discard:
+                    stack.append(res)
+
             elif self.__visit_tokens__ and isinstance(x, Token):
-                stack.append(self._call_userfunc_token(x))
+                res = self._call_userfunc_token(x)
+                if res is not Discard:
+                    stack.append(res)
             else:
                 stack.append(x)
 
-        t ,= stack  ##
+        result, = stack  ##
 
-        return t
+        ##
+
+        ##
+
+        ##
+
+        return cast(_Return_T, result)
 
 
 class Transformer_InPlaceRecursive(Transformer):
     #--
     def _transform_tree(self, tree):
         tree.children = list(self._transform_children(tree.children))
         return self._call_userfunc(tree)
@@ -697,146 +818,155 @@
         #--
         return tree
 
     def __class_getitem__(cls, _):
         return cls
 
 
-class Visitor(VisitorBase):
+class Visitor(VisitorBase, ABC, Generic[_Leaf_T]):
     #--
 
-    def visit(self, tree):
+    def visit(self, tree: Tree[_Leaf_T]) -> Tree[_Leaf_T]:
         #--
         for subtree in tree.iter_subtrees():
             self._call_userfunc(subtree)
         return tree
 
-    def visit_topdown(self,tree):
+    def visit_topdown(self, tree: Tree[_Leaf_T]) -> Tree[_Leaf_T]:
         #--
         for subtree in tree.iter_subtrees_topdown():
             self._call_userfunc(subtree)
         return tree
 
 
-class Visitor_Recursive(VisitorBase):
+class Visitor_Recursive(VisitorBase, Generic[_Leaf_T]):
     #--
 
-    def visit(self, tree):
+    def visit(self, tree: Tree[_Leaf_T]) -> Tree[_Leaf_T]:
         #--
         for child in tree.children:
             if isinstance(child, Tree):
                 self.visit(child)
 
         self._call_userfunc(tree)
         return tree
 
-    def visit_topdown(self,tree):
+    def visit_topdown(self,tree: Tree[_Leaf_T]) -> Tree[_Leaf_T]:
         #--
         self._call_userfunc(tree)
 
         for child in tree.children:
             if isinstance(child, Tree):
                 self.visit_topdown(child)
 
         return tree
 
 
-def visit_children_decor(func):
+class Interpreter(_Decoratable, ABC, Generic[_Leaf_T, _Return_T]):
     #--
-    @wraps(func)
-    def inner(cls, tree):
-        values = cls.visit_children(tree)
-        return func(cls, values)
-    return inner
 
+    def visit(self, tree: Tree[_Leaf_T]) -> _Return_T:
+        ##
 
-class Interpreter(_Decoratable):
-    #--
+        ##
 
-    def visit(self, tree):
+        ##
+
+        return self._visit_tree(tree)
+
+    def _visit_tree(self, tree: Tree[_Leaf_T]):
         f = getattr(self, tree.data)
         wrapper = getattr(f, 'visit_wrapper', None)
         if wrapper is not None:
             return f.visit_wrapper(f, tree.data, tree.children, tree.meta)
         else:
             return f(tree)
 
-    def visit_children(self, tree):
-        return [self.visit(child) if isinstance(child, Tree) else child
+    def visit_children(self, tree: Tree[_Leaf_T]) -> List:
+        return [self._visit_tree(child) if isinstance(child, Tree) else child
                 for child in tree.children]
 
     def __getattr__(self, name):
         return self.__default__
 
     def __default__(self, tree):
         return self.visit_children(tree)
 
 
+_InterMethod = Callable[[Type[Interpreter], _Return_T], _R]
+
+def visit_children_decor(func: _InterMethod) -> _InterMethod:
+    #--
+    @wraps(func)
+    def inner(cls, tree):
+        values = cls.visit_children(tree)
+        return func(cls, values)
+    return inner
+
 ##
 
 
-def _apply_decorator(obj, decorator, **kwargs):
+def _apply_v_args(obj, visit_wrapper):
     try:
-        _apply = obj._apply_decorator
+        _apply = obj._apply_v_args
     except AttributeError:
-        return decorator(obj, **kwargs)
+        return _VArgsWrapper(obj, visit_wrapper)
     else:
-        return _apply(decorator, **kwargs)
+        return _apply(visit_wrapper)
 
 
-def _inline_args__func(func):
-    @wraps(func)
-    def create_decorator(_f, with_self):
-        if with_self:
-            def f(self, children):
-                return _f(self, *children)
-        else:
-            def f(self, children):
-                return _f(*children)
-        return f
+class _VArgsWrapper:
+    #--
+    base_func: Callable
 
-    return smart_decorator(func, create_decorator)
+    def __init__(self, func: Callable, visit_wrapper: Callable[[Callable, str, list, Any], Any]):
+        if isinstance(func, _VArgsWrapper):
+            func = func.base_func
+        ##
+
+        self.base_func = func  ##
 
+        self.visit_wrapper = visit_wrapper
+        update_wrapper(self, func)
 
-def inline_args(obj):   ##
+    def __call__(self, *args, **kwargs):
+        return self.base_func(*args, **kwargs)
 
-    return _apply_decorator(obj, _inline_args__func)
+    def __get__(self, instance, owner=None):
+        try:
+            ##
 
+            ##
 
-def _visitor_args_func_dec(func, visit_wrapper=None, static=False):
-    def create_decorator(_f, with_self):
-        if with_self:
-            def f(self, *args, **kwargs):
-                return _f(self, *args, **kwargs)
+            g = type(self.base_func).__get__
+        except AttributeError:
+            return self
         else:
-            def f(self, *args, **kwargs):
-                return _f(*args, **kwargs)
-        return f
+            return _VArgsWrapper(g(self.base_func, instance, owner), self.visit_wrapper)
 
-    if static:
-        f = wraps(func)(create_decorator(func, False))
-    else:
-        f = smart_decorator(func, create_decorator)
-    f.vargs_applied = True
-    f.visit_wrapper = visit_wrapper
-    return f
+    def __set_name__(self, owner, name):
+        try:
+            f = type(self.base_func).__set_name__
+        except AttributeError:
+            return
+        else:
+            f(self.base_func, owner, name)
 
 
 def _vargs_inline(f, _data, children, _meta):
     return f(*children)
 def _vargs_meta_inline(f, _data, children, meta):
     return f(meta, *children)
 def _vargs_meta(f, _data, children, meta):
-    return f(children, meta)   ##
-
+    return f(meta, children)
 def _vargs_tree(f, data, children, meta):
     return f(Tree(data, children, meta))
 
 
-def v_args(inline=False, meta=False, tree=False, wrapper=None):
+def v_args(inline: bool = False, meta: bool = False, tree: bool = False, wrapper: Optional[Callable] = None) -> Callable[[_DECORATED], _DECORATED]:
     #--
     if tree and (meta or inline):
         raise ValueError("Visitor functions cannot combine 'tree' with 'meta' or 'inline'.")
 
     func = None
     if meta:
         if inline:
@@ -850,26 +980,29 @@
 
     if wrapper is not None:
         if func is not None:
             raise ValueError("Cannot use 'wrapper' along with 'tree', 'meta' or 'inline'.")
         func = wrapper
 
     def _visitor_args_dec(obj):
-        return _apply_decorator(obj, _visitor_args_func_dec, visit_wrapper=func)
+        return _apply_v_args(obj, func)
     return _visitor_args_dec
 
 
 
+TOKEN_DEFAULT_PRIORITY = 0
+
 
 class Symbol(Serialize):
     __slots__ = ('name',)
 
-    is_term = NotImplemented
+    name: str
+    is_term: ClassVar[bool] = NotImplemented
 
-    def __init__(self, name):
+    def __init__(self, name: str) -> None:
         self.name = name
 
     def __eq__(self, other):
         assert isinstance(other, Symbol), other
         return self.is_term == other.is_term and self.name == other.name
 
     def __ne__(self, other):
@@ -879,39 +1012,51 @@
         return hash(self.name)
 
     def __repr__(self):
         return '%s(%r)' % (type(self).__name__, self.name)
 
     fullrepr = property(__repr__)
 
+    def renamed(self, f):
+        return type(self)(f(self.name))
+
 
 class Terminal(Symbol):
     __serialize_fields__ = 'name', 'filter_out'
 
-    is_term = True
+    is_term: ClassVar[bool] = True
 
     def __init__(self, name, filter_out=False):
         self.name = name
         self.filter_out = filter_out
 
     @property
     def fullrepr(self):
         return '%s(%r, %r)' % (type(self).__name__, self.name, self.filter_out)
 
+    def renamed(self, f):
+        return type(self)(f(self.name), self.filter_out)
+
 
 class NonTerminal(Symbol):
     __serialize_fields__ = 'name',
 
-    is_term = False
+    is_term: ClassVar[bool] = False
 
 
 class RuleOptions(Serialize):
     __serialize_fields__ = 'keep_all_tokens', 'expand1', 'priority', 'template_source', 'empty_indices'
 
-    def __init__(self, keep_all_tokens=False, expand1=False, priority=None, template_source=None, empty_indices=()):
+    keep_all_tokens: bool
+    expand1: bool
+    priority: Optional[int]
+    template_source: Optional[str]
+    empty_indices: Tuple[bool, ...]
+
+    def __init__(self, keep_all_tokens: bool=False, expand1: bool=False, priority: Optional[int]=None, template_source: Optional[str]=None, empty_indices: Tuple[bool, ...]=()) -> None:
         self.keep_all_tokens = keep_all_tokens
         self.expand1 = expand1
         self.priority = priority
         self.template_source = template_source
         self.empty_indices = empty_indices
 
     def __repr__(self):
@@ -956,19 +1101,22 @@
         return self.origin == other.origin and self.expansion == other.expansion
 
 
 
 from copy import copy
 
 
-class Pattern(Serialize):
-    raw = None
-    type = None
+class Pattern(Serialize, ABC):
+
+    value: str
+    flags: Collection[str]
+    raw: Optional[str]
+    type: ClassVar[str]
 
-    def __init__(self, value, flags=(), raw=None):
+    def __init__(self, value: str, flags: Collection[str]=(), raw: Optional[str]=None) -> None:
         self.value = value
         self.flags = frozenset(flags)
         self.raw = raw
 
     def __repr__(self):
         return repr(self.to_regexp())
 
@@ -976,145 +1124,213 @@
 
     def __hash__(self):
         return hash((type(self), self.value, self.flags))
 
     def __eq__(self, other):
         return type(self) == type(other) and self.value == other.value and self.flags == other.flags
 
-    def to_regexp(self):
+    @abstractmethod
+    def to_regexp(self) -> str:
         raise NotImplementedError()
 
-    def min_width(self):
+    @property
+    @abstractmethod
+    def min_width(self) -> int:
         raise NotImplementedError()
 
-    def max_width(self):
+    @property
+    @abstractmethod
+    def max_width(self) -> int:
         raise NotImplementedError()
 
-    if Py36:
-        ##
-
-        def _get_flags(self, value):
-            for f in self.flags:
-                value = ('(?%s:%s)' % (f, value))
-            return value
-
-    else:
-        def _get_flags(self, value):
-            for f in self.flags:
-                value = ('(?%s)' % f) + value
-            return value
-
+    def _get_flags(self, value):
+        for f in self.flags:
+            value = ('(?%s:%s)' % (f, value))
+        return value
 
 
 class PatternStr(Pattern):
     __serialize_fields__ = 'value', 'flags'
 
-    type = "str"
+    type: ClassVar[str] = "str"
 
-    def to_regexp(self):
+    def to_regexp(self) -> str:
         return self._get_flags(re.escape(self.value))
 
     @property
-    def min_width(self):
+    def min_width(self) -> int:
+        return len(self.value)
+
+    @property
+    def max_width(self) -> int:
         return len(self.value)
-    max_width = min_width
 
 
 class PatternRE(Pattern):
     __serialize_fields__ = 'value', 'flags', '_width'
 
-    type = "re"
+    type: ClassVar[str] = "re"
 
-    def to_regexp(self):
+    def to_regexp(self) -> str:
         return self._get_flags(self.value)
 
     _width = None
     def _get_width(self):
         if self._width is None:
             self._width = get_regexp_width(self.to_regexp())
         return self._width
 
     @property
-    def min_width(self):
+    def min_width(self) -> int:
         return self._get_width()[0]
 
     @property
-    def max_width(self):
+    def max_width(self) -> int:
         return self._get_width()[1]
 
 
 class TerminalDef(Serialize):
     __serialize_fields__ = 'name', 'pattern', 'priority'
     __serialize_namespace__ = PatternStr, PatternRE
 
-    def __init__(self, name, pattern, priority=1):
+    name: str
+    pattern: Pattern
+    priority: int
+
+    def __init__(self, name: str, pattern: Pattern, priority: int=TOKEN_DEFAULT_PRIORITY) -> None:
         assert isinstance(pattern, Pattern), pattern
         self.name = name
         self.pattern = pattern
         self.priority = priority
 
     def __repr__(self):
         return '%s(%r, %r)' % (type(self).__name__, self.name, self.pattern)
 
-    def user_repr(self):
+    def user_repr(self) -> str:
         if self.name.startswith('__'): ##
 
             return self.pattern.raw or self.name
         else:
             return self.name
 
+_T = TypeVar('_T', bound="Token")
 
-class Token(Str):
+class Token(str):
     #--
-    __slots__ = ('type', 'pos_in_stream', 'value', 'line', 'column', 'end_line', 'end_column', 'end_pos')
+    __slots__ = ('type', 'start_pos', 'value', 'line', 'column', 'end_line', 'end_column', 'end_pos')
 
-    def __new__(cls, type_, value, pos_in_stream=None, line=None, column=None, end_line=None, end_column=None, end_pos=None):
-        try:
-            self = super(Token, cls).__new__(cls, value)
-        except UnicodeDecodeError:
-            value = value.decode('latin1')
-            self = super(Token, cls).__new__(cls, value)
+    __match_args__ = ('type', 'value')
 
-        self.type = type_
-        self.pos_in_stream = pos_in_stream
-        self.value = value
-        self.line = line
-        self.column = column
-        self.end_line = end_line
-        self.end_column = end_column
-        self.end_pos = end_pos
-        return self
+    type: str
+    start_pos: Optional[int]
+    value: Any
+    line: Optional[int]
+    column: Optional[int]
+    end_line: Optional[int]
+    end_column: Optional[int]
+    end_pos: Optional[int]
+
+
+    @overload
+    def __new__(
+        cls,
+        type: str,
+        value: Any,
+        start_pos: Optional[int]=None,
+        line: Optional[int]=None,
+        column: Optional[int]=None,
+        end_line: Optional[int]=None,
+        end_column: Optional[int]=None,
+        end_pos: Optional[int]=None
+    ) -> 'Token':
+        ...
+
+    @overload
+    def __new__(
+        cls,
+        type_: str,
+        value: Any,
+        start_pos: Optional[int]=None,
+        line: Optional[int]=None,
+        column: Optional[int]=None,
+        end_line: Optional[int]=None,
+        end_column: Optional[int]=None,
+        end_pos: Optional[int]=None
+    ) -> 'Token':        ...
+
+    def __new__(cls, *args, **kwargs):
+        if "type_" in kwargs:
+            warnings.warn("`type_` is deprecated use `type` instead", DeprecationWarning)
+
+            if "type" in kwargs:
+                raise TypeError("Error: using both 'type' and the deprecated 'type_' as arguments.")
+            kwargs["type"] = kwargs.pop("type_")
+
+        return cls._future_new(*args, **kwargs)
+
+
+    @classmethod
+    def _future_new(cls, type, value, start_pos=None, line=None, column=None, end_line=None, end_column=None, end_pos=None):
+        inst = super(Token, cls).__new__(cls, value)
+
+        inst.type = type
+        inst.start_pos = start_pos
+        inst.value = value
+        inst.line = line
+        inst.column = column
+        inst.end_line = end_line
+        inst.end_column = end_column
+        inst.end_pos = end_pos
+        return inst
+
+    @overload
+    def update(self, type: Optional[str]=None, value: Optional[Any]=None) -> 'Token':
+        ...
 
-    def update(self, type_=None, value=None):
+    @overload
+    def update(self, type_: Optional[str]=None, value: Optional[Any]=None) -> 'Token':
+        ...
+
+    def update(self, *args, **kwargs):
+        if "type_" in kwargs:
+            warnings.warn("`type_` is deprecated use `type` instead", DeprecationWarning)
+
+            if "type" in kwargs:
+                raise TypeError("Error: using both 'type' and the deprecated 'type_' as arguments.")
+            kwargs["type"] = kwargs.pop("type_")
+
+        return self._future_update(*args, **kwargs)
+
+    def _future_update(self, type: Optional[str]=None, value: Optional[Any]=None) -> 'Token':
         return Token.new_borrow_pos(
-            type_ if type_ is not None else self.type,
+            type if type is not None else self.type,
             value if value is not None else self.value,
             self
         )
 
     @classmethod
-    def new_borrow_pos(cls, type_, value, borrow_t):
-        return cls(type_, value, borrow_t.pos_in_stream, borrow_t.line, borrow_t.column, borrow_t.end_line, borrow_t.end_column, borrow_t.end_pos)
+    def new_borrow_pos(cls: Type[_T], type_: str, value: Any, borrow_t: 'Token') -> _T:
+        return cls(type_, value, borrow_t.start_pos, borrow_t.line, borrow_t.column, borrow_t.end_line, borrow_t.end_column, borrow_t.end_pos)
 
     def __reduce__(self):
-        return (self.__class__, (self.type, self.value, self.pos_in_stream, self.line, self.column))
+        return (self.__class__, (self.type, self.value, self.start_pos, self.line, self.column))
 
     def __repr__(self):
         return 'Token(%r, %r)' % (self.type, self.value)
 
     def __deepcopy__(self, memo):
-        return Token(self.type, self.value, self.pos_in_stream, self.line, self.column)
+        return Token(self.type, self.value, self.start_pos, self.line, self.column)
 
     def __eq__(self, other):
         if isinstance(other, Token) and self.type != other.type:
             return False
 
-        return Str.__eq__(self, other)
+        return str.__eq__(self, other)
 
-    __hash__ = Str.__hash__
+    __hash__ = str.__hash__
 
 
 class LineCounter:
     __slots__ = 'char_pos', 'line', 'column', 'line_start_pos', 'newline_char'
 
     def __init__(self, newline_char):
         self.newline_char = newline_char
@@ -1125,118 +1341,185 @@
 
     def __eq__(self, other):
         if not isinstance(other, LineCounter):
             return NotImplemented
 
         return self.char_pos == other.char_pos and self.newline_char == other.newline_char
 
-    def feed(self, token, test_newline=True):
+    def feed(self, token: Token, test_newline=True):
         #--
         if test_newline:
             newlines = token.count(self.newline_char)
             if newlines:
                 self.line += newlines
                 self.line_start_pos = self.char_pos + token.rindex(self.newline_char) + 1
 
         self.char_pos += len(token)
         self.column = self.char_pos - self.line_start_pos + 1
 
 
 class UnlessCallback:
-    def __init__(self, mres):
-        self.mres = mres
+    def __init__(self, scanner):
+        self.scanner = scanner
 
     def __call__(self, t):
-        for mre, type_from_index in self.mres:
-            m = mre.match(t.value)
-            if m:
-                t.type = type_from_index[m.lastindex]
-                break
+        res = self.scanner.match(t.value, 0)
+        if res:
+            _value, t.type = res
         return t
 
 
 class CallChain:
     def __init__(self, callback1, callback2, cond):
         self.callback1 = callback1
         self.callback2 = callback2
         self.cond = cond
 
     def __call__(self, t):
         t2 = self.callback1(t)
         return self.callback2(t) if self.cond(t2) else t2
 
 
+def _get_match(re_, regexp, s, flags):
+    m = re_.match(regexp, s, flags)
+    if m:
+        return m.group(0)
+
 def _create_unless(terminals, g_regex_flags, re_, use_bytes):
     tokens_by_type = classify(terminals, lambda t: type(t.pattern))
     assert len(tokens_by_type) <= 2, tokens_by_type.keys()
     embedded_strs = set()
     callback = {}
     for retok in tokens_by_type.get(PatternRE, []):
         unless = []
         for strtok in tokens_by_type.get(PatternStr, []):
-            if strtok.priority > retok.priority:
+            if strtok.priority != retok.priority:
                 continue
             s = strtok.pattern.value
-            m = re_.match(retok.pattern.to_regexp(), s, g_regex_flags)
-            if m and m.group(0) == s:
+            if s == _get_match(re_, retok.pattern.to_regexp(), s, g_regex_flags):
                 unless.append(strtok)
                 if strtok.pattern.flags <= retok.pattern.flags:
                     embedded_strs.add(strtok)
         if unless:
-            callback[retok.name] = UnlessCallback(build_mres(unless, g_regex_flags, re_, match_whole=True, use_bytes=use_bytes))
+            callback[retok.name] = UnlessCallback(Scanner(unless, g_regex_flags, re_, match_whole=True, use_bytes=use_bytes))
 
-    terminals = [t for t in terminals if t not in embedded_strs]
-    return terminals, callback
+    new_terminals = [t for t in terminals if t not in embedded_strs]
+    return new_terminals, callback
 
 
-def _build_mres(terminals, max_size, g_regex_flags, match_whole, re_, use_bytes):
-    ##
+class Scanner:
+    def __init__(self, terminals, g_regex_flags, re_, use_bytes, match_whole=False):
+        self.terminals = terminals
+        self.g_regex_flags = g_regex_flags
+        self.re_ = re_
+        self.use_bytes = use_bytes
+        self.match_whole = match_whole
 
-    ##
+        self.allowed_types = {t.name for t in self.terminals}
 
-    ##
+        self._mres = self._build_mres(terminals, len(terminals))
 
-    postfix = '$' if match_whole else ''
-    mres = []
-    while terminals:
-        pattern = u'|'.join(u'(?P<%s>%s)' % (t.name, t.pattern.to_regexp() + postfix) for t in terminals[:max_size])
-        if use_bytes:
-            pattern = pattern.encode('latin-1')
-        try:
-            mre = re_.compile(pattern, g_regex_flags)
-        except AssertionError:  ##
+    def _build_mres(self, terminals, max_size):
+        ##
 
-            return _build_mres(terminals, max_size//2, g_regex_flags, match_whole, re_, use_bytes)
+        ##
 
-        mres.append((mre, {i: n for n, i in mre.groupindex.items()}))
-        terminals = terminals[max_size:]
-    return mres
+        ##
 
+        postfix = '$' if self.match_whole else ''
+        mres = []
+        while terminals:
+            pattern = u'|'.join(u'(?P<%s>%s)' % (t.name, t.pattern.to_regexp() + postfix) for t in terminals[:max_size])
+            if self.use_bytes:
+                pattern = pattern.encode('latin-1')
+            try:
+                mre = self.re_.compile(pattern, self.g_regex_flags)
+            except AssertionError:  ##
 
-def build_mres(terminals, g_regex_flags, re_, use_bytes, match_whole=False):
-    return _build_mres(terminals, len(terminals), g_regex_flags, match_whole, re_, use_bytes)
+                return self._build_mres(terminals, max_size//2)
 
+            mres.append(mre)
+            terminals = terminals[max_size:]
+        return mres
 
-def _regexp_has_newline(r):
+    def match(self, text, pos):
+        for mre in self._mres:
+            m = mre.match(text, pos)
+            if m:
+                return m.group(0), m.lastgroup
+
+
+def _regexp_has_newline(r: str):
     #--
     return '\n' in r or '\\n' in r or '\\s' in r or '[^' in r or ('(?s' in r and '.' in r)
 
 
-class Lexer(object):
+class LexerState:
+    #--
+
+    __slots__ = 'text', 'line_ctr', 'last_token'
+
+    def __init__(self, text, line_ctr=None, last_token=None):
+        self.text = text
+        self.line_ctr = line_ctr or LineCounter(b'\n' if isinstance(text, bytes) else '\n')
+        self.last_token = last_token
+
+    def __eq__(self, other):
+        if not isinstance(other, LexerState):
+            return NotImplemented
+
+        return self.text is other.text and self.line_ctr == other.line_ctr and self.last_token == other.last_token
+
+    def __copy__(self):
+        return type(self)(self.text, copy(self.line_ctr), self.last_token)
+
+
+class LexerThread:
+    #--
+
+    def __init__(self, lexer: 'Lexer', lexer_state: LexerState):
+        self.lexer = lexer
+        self.state = lexer_state
+
+    @classmethod
+    def from_text(cls, lexer: 'Lexer', text: str):
+        return cls(lexer, LexerState(text))
+
+    def lex(self, parser_state):
+        return self.lexer.lex(self.state, parser_state)
+
+    def __copy__(self):
+        return type(self)(self.lexer, copy(self.state))
+
+    _Token = Token
+
+
+_Callback = Callable[[Token], Token]
+
+class Lexer(ABC):
     #--
-    lex = NotImplemented
+    @abstractmethod
+    def lex(self, lexer_state: LexerState, parser_state: Any) -> Iterator[Token]:
+        return NotImplemented
 
     def make_lexer_state(self, text):
-        line_ctr = LineCounter(b'\n' if isinstance(text, bytes) else '\n')
-        return LexerState(text, line_ctr)
+        #--
+        return LexerState(text)
 
 
-class TraditionalLexer(Lexer):
+class BasicLexer(Lexer):
 
-    def __init__(self, conf):
+    terminals: Collection[TerminalDef]
+    ignore_types: FrozenSet[str]
+    newline_types: FrozenSet[str]
+    user_callbacks: Dict[str, _Callback]
+    callback: Dict[str, _Callback]
+    re: ModuleType
+
+    def __init__(self, conf: 'LexerConf') -> None:
         terminals = list(conf.terminals)
         assert all(isinstance(t, TerminalDef) for t in terminals), terminals
 
         self.re = conf.re_module
 
         if not conf.skip_validation:
             ##
@@ -1261,53 +1544,50 @@
         terminals.sort(key=lambda x: (-x.priority, -x.pattern.max_width, -len(x.pattern.value), x.name))
         self.terminals = terminals
         self.user_callbacks = conf.callbacks
         self.g_regex_flags = conf.g_regex_flags
         self.use_bytes = conf.use_bytes
         self.terminals_by_name = conf.terminals_by_name
 
-        self._mres = None
+        self._scanner = None
 
-    def _build(self):
+    def _build_scanner(self):
         terminals, self.callback = _create_unless(self.terminals, self.g_regex_flags, self.re, self.use_bytes)
         assert all(self.callback.values())
 
         for type_, f in self.user_callbacks.items():
             if type_ in self.callback:
                 ##
 
                 self.callback[type_] = CallChain(self.callback[type_], f, lambda t: t.type == type_)
             else:
                 self.callback[type_] = f
 
-        self._mres = build_mres(terminals, self.g_regex_flags, self.re, self.use_bytes)
+        self._scanner = Scanner(terminals, self.g_regex_flags, self.re, self.use_bytes)
 
     @property
-    def mres(self):
-        if self._mres is None:
-            self._build()
-        return self._mres
+    def scanner(self):
+        if self._scanner is None:
+            self._build_scanner()
+        return self._scanner
 
     def match(self, text, pos):
-        for mre, type_from_index in self.mres:
-            m = mre.match(text, pos)
-            if m:
-                return m.group(0), type_from_index[m.lastindex]
+        return self.scanner.match(text, pos)
 
-    def lex(self, state, parser_state):
+    def lex(self, state: LexerState, parser_state: Any) -> Iterator[Token]:
         with suppress(EOFError):
             while True:
                 yield self.next_token(state, parser_state)
 
-    def next_token(self, lex_state, parser_state=None):
+    def next_token(self, lex_state: LexerState, parser_state: Any=None) -> Token:
         line_ctr = lex_state.line_ctr
         while line_ctr.char_pos < len(lex_state.text):
             res = self.match(lex_state.text, line_ctr.char_pos)
             if not res:
-                allowed = {v for m, tfi in self.mres for v in tfi.values()} - self.ignore_types
+                allowed = self.scanner.allowed_types - self.ignore_types
                 if not allowed:
                     allowed = {"<END-OF-FILE>"}
                 raise UnexpectedCharacters(lex_state.text, line_ctr.char_pos, line_ctr.line, line_ctr.column,
                                            allowed=allowed, token_history=lex_state.last_token and [lex_state.last_token],
                                            state=parser_state, terminals_by_name=self.terminals_by_name)
 
             value, type_ = res
@@ -1331,63 +1611,45 @@
                 line_ctr.feed(value, type_ in self.newline_types)
 
         ##
 
         raise EOFError(self)
 
 
-class LexerState(object):
-    __slots__ = 'text', 'line_ctr', 'last_token'
-
-    def __init__(self, text, line_ctr, last_token=None):
-        self.text = text
-        self.line_ctr = line_ctr
-        self.last_token = last_token
-
-    def __eq__(self, other):
-        if not isinstance(other, LexerState):
-            return NotImplemented
-
-        return self.text is other.text and self.line_ctr == other.line_ctr and self.last_token == other.last_token
-
-    def __copy__(self):
-        return type(self)(self.text, copy(self.line_ctr), self.last_token)
-
-
 class ContextualLexer(Lexer):
 
-    def __init__(self, conf, states, always_accept=()):
+    lexers: Dict[str, BasicLexer]
+    root_lexer: BasicLexer
+
+    def __init__(self, conf: 'LexerConf', states: Dict[str, Collection[str]], always_accept: Collection[str]=()) -> None:
         terminals = list(conf.terminals)
         terminals_by_name = conf.terminals_by_name
 
         trad_conf = copy(conf)
         trad_conf.terminals = terminals
 
-        lexer_by_tokens = {}
+        lexer_by_tokens: Dict[FrozenSet[str], BasicLexer] = {}
         self.lexers = {}
         for state, accepts in states.items():
             key = frozenset(accepts)
             try:
                 lexer = lexer_by_tokens[key]
             except KeyError:
                 accepts = set(accepts) | set(conf.ignore) | set(always_accept)
                 lexer_conf = copy(trad_conf)
                 lexer_conf.terminals = [terminals_by_name[n] for n in accepts if n in terminals_by_name]
-                lexer = TraditionalLexer(lexer_conf)
+                lexer = BasicLexer(lexer_conf)
                 lexer_by_tokens[key] = lexer
 
             self.lexers[state] = lexer
 
         assert trad_conf.terminals is terminals
-        self.root_lexer = TraditionalLexer(trad_conf)
+        self.root_lexer = BasicLexer(trad_conf)
 
-    def make_lexer_state(self, text):
-        return self.root_lexer.make_lexer_state(text)
-
-    def lex(self, lexer_state, parser_state):
+    def lex(self, lexer_state: LexerState, parser_state: Any) -> Iterator[Token]:
         try:
             while True:
                 lexer = self.lexers[parser_state.position]
                 yield lexer.next_token(lexer_state, parser_state)
         except EOFError:
             pass
         except UnexpectedCharacters as e:
@@ -1400,57 +1662,61 @@
 
                 token = self.root_lexer.next_token(lexer_state, parser_state)
                 raise UnexpectedToken(token, e.allowed, state=parser_state, token_history=[last_token], terminals_by_name=self.root_lexer.terminals_by_name)
             except UnexpectedCharacters:
                 raise e  ##
 
 
-class LexerThread(object):
-    #--
-
-    def __init__(self, lexer, text):
-        self.lexer = lexer
-        self.state = lexer.make_lexer_state(text)
-
-    def lex(self, parser_state):
-        return self.lexer.lex(self.state, parser_state)
-
-    def __copy__(self):
-        copied = object.__new__(LexerThread)
-        copied.lexer = self.lexer
-        copied.state = copy(self.state)
-        return copied
 
 
+_ParserArgType: 'TypeAlias' = 'Literal["earley", "lalr", "cyk", "auto"]'
+_LexerArgType: 'TypeAlias' = 'Union[Literal["auto", "basic", "contextual", "dynamic", "dynamic_complete"], Type[Lexer]]'
+_Callback = Callable[[Token], Token]
 
 class LexerConf(Serialize):
     __serialize_fields__ = 'terminals', 'ignore', 'g_regex_flags', 'use_bytes', 'lexer_type'
     __serialize_namespace__ = TerminalDef,
 
-    def __init__(self, terminals, re_module, ignore=(), postlex=None, callbacks=None, g_regex_flags=0, skip_validation=False, use_bytes=False):
+    terminals: Collection[TerminalDef]
+    re_module: ModuleType
+    ignore: Collection[str]
+    postlex: 'Optional[PostLex]'
+    callbacks: Dict[str, _Callback]
+    g_regex_flags: int
+    skip_validation: bool
+    use_bytes: bool
+    lexer_type: Optional[_LexerArgType]
+
+    def __init__(self, terminals: Collection[TerminalDef], re_module: ModuleType, ignore: Collection[str]=(), postlex: 'Optional[PostLex]'=None, callbacks: Optional[Dict[str, _Callback]]=None, g_regex_flags: int=0, skip_validation: bool=False, use_bytes: bool=False):
         self.terminals = terminals
         self.terminals_by_name = {t.name: t for t in self.terminals}
         assert len(self.terminals) == len(self.terminals_by_name)
         self.ignore = ignore
         self.postlex = postlex
         self.callbacks = callbacks or {}
         self.g_regex_flags = g_regex_flags
         self.re_module = re_module
         self.skip_validation = skip_validation
         self.use_bytes = use_bytes
         self.lexer_type = None
 
-    @property
-    def tokens(self):
-        warn("LexerConf.tokens is deprecated. Use LexerConf.terminals instead", DeprecationWarning)
-        return self.terminals
-
     def _deserialize(self):
         self.terminals_by_name = {t.name: t for t in self.terminals}
 
+    def __deepcopy__(self, memo=None):
+        return type(self)(
+            deepcopy(self.terminals, memo),
+            self.re_module,
+            deepcopy(self.ignore, memo),
+            deepcopy(self.postlex, memo),
+            deepcopy(self.callbacks, memo),
+            deepcopy(self.g_regex_flags, memo),
+            deepcopy(self.skip_validation, memo),
+            deepcopy(self.use_bytes, memo),
+        )
 
 
 class ParserConf(Serialize):
     __serialize_fields__ = 'rules', 'start', 'parser_type'
 
     def __init__(self, rules, callbacks, start):
         assert isinstance(start, list)
@@ -1458,73 +1724,97 @@
         self.callbacks = callbacks
         self.start = start
 
         self.parser_type = None
 
 
 from functools import partial, wraps
-from itertools import repeat, product
+from itertools import product
 
 
 class ExpandSingleChild:
     def __init__(self, node_builder):
         self.node_builder = node_builder
 
     def __call__(self, children):
         if len(children) == 1:
             return children[0]
         else:
             return self.node_builder(children)
 
 
+
 class PropagatePositions:
-    def __init__(self, node_builder):
+    def __init__(self, node_builder, node_filter=None):
         self.node_builder = node_builder
+        self.node_filter = node_filter
 
     def __call__(self, children):
         res = self.node_builder(children)
 
-        ##
-
         if isinstance(res, Tree):
+            ##
+
+            ##
+
+            ##
+
+            ##
+
+
             res_meta = res.meta
-            for c in children:
-                if isinstance(c, Tree):
-                    child_meta = c.meta
-                    if not child_meta.empty:
-                        res_meta.line = child_meta.line
-                        res_meta.column = child_meta.column
-                        res_meta.start_pos = child_meta.start_pos
-                        res_meta.empty = False
-                        break
-                elif isinstance(c, Token):
-                    res_meta.line = c.line
-                    res_meta.column = c.column
-                    res_meta.start_pos = c.pos_in_stream
+
+            first_meta = self._pp_get_meta(children)
+            if first_meta is not None:
+                if not hasattr(res_meta, 'line'):
+                    ##
+
+                    res_meta.line = getattr(first_meta, 'container_line', first_meta.line)
+                    res_meta.column = getattr(first_meta, 'container_column', first_meta.column)
+                    res_meta.start_pos = getattr(first_meta, 'container_start_pos', first_meta.start_pos)
                     res_meta.empty = False
-                    break
 
-            for c in reversed(children):
-                if isinstance(c, Tree):
-                    child_meta = c.meta
-                    if not child_meta.empty:
-                        res_meta.end_line = child_meta.end_line
-                        res_meta.end_column = child_meta.end_column
-                        res_meta.end_pos = child_meta.end_pos
-                        res_meta.empty = False
-                        break
-                elif isinstance(c, Token):
-                    res_meta.end_line = c.end_line
-                    res_meta.end_column = c.end_column
-                    res_meta.end_pos = c.end_pos
+                res_meta.container_line = getattr(first_meta, 'container_line', first_meta.line)
+                res_meta.container_column = getattr(first_meta, 'container_column', first_meta.column)
+
+            last_meta = self._pp_get_meta(reversed(children))
+            if last_meta is not None:
+                if not hasattr(res_meta, 'end_line'):
+                    res_meta.end_line = getattr(last_meta, 'container_end_line', last_meta.end_line)
+                    res_meta.end_column = getattr(last_meta, 'container_end_column', last_meta.end_column)
+                    res_meta.end_pos = getattr(last_meta, 'container_end_pos', last_meta.end_pos)
                     res_meta.empty = False
-                    break
+
+                res_meta.container_end_line = getattr(last_meta, 'container_end_line', last_meta.end_line)
+                res_meta.container_end_column = getattr(last_meta, 'container_end_column', last_meta.end_column)
 
         return res
 
+    def _pp_get_meta(self, children):
+        for c in children:
+            if self.node_filter is not None and not self.node_filter(c):
+                continue
+            if isinstance(c, Tree):
+                if not c.meta.empty:
+                    return c.meta
+            elif isinstance(c, Token):
+                return c
+            elif hasattr(c, '__lark_meta__'):
+                return c.__lark_meta__()
+
+def make_propagate_positions(option):
+    if callable(option):
+        return partial(PropagatePositions, node_filter=option)
+    elif option is True:
+        return PropagatePositions
+    elif option is False:
+        return None
+
+    raise ConfigurationError('Invalid option for propagate_positions: %r' % option)
+
 
 class ChildFilter:
     def __init__(self, to_include, append_none, node_builder):
         self.node_builder = node_builder
         self.to_include = to_include
         self.append_none = append_none
 
@@ -1588,15 +1878,15 @@
         return self.node_builder(filtered)
 
 
 def _should_expand(sym):
     return not sym.is_term and sym.name.startswith('_')
 
 
-def maybe_create_child_filter(expansion, keep_all_tokens, ambiguous, _empty_indices):
+def maybe_create_child_filter(expansion, keep_all_tokens, ambiguous, _empty_indices: List[bool]):
     ##
 
     if _empty_indices:
         assert _empty_indices.count(False) == len(expansion)
         s = ''.join(str(int(b)) for b in _empty_indices)
         empty_indices = [len(ones) for ones in s.split('0')]
         assert len(empty_indices) == len(expansion)+1, (empty_indices, len(expansion))
@@ -1643,22 +1933,21 @@
 
         ambiguous = []
         for i, child in enumerate(children):
             if _is_ambig_tree(child):
                 if i in self.to_expand:
                     ambiguous.append(i)
 
-                to_expand = [j for j, grandchild in enumerate(child.children) if _is_ambig_tree(grandchild)]
-                child.expand_kids_by_index(*to_expand)
+                child.expand_kids_by_data('_ambig')
 
         if not ambiguous:
             return self.node_builder(children)
 
-        expand = [iter(child.children) if i in ambiguous else repeat(child) for i, child in enumerate(children)]
-        return self.tree_class('_ambig', [self.node_builder(list(f[0])) for f in product(zip(*expand))])
+        expand = [child.children if i in ambiguous else (child,) for i, child in enumerate(children)]
+        return self.tree_class('_ambig', [self.node_builder(list(f)) for f in product(*expand)])
 
 
 def maybe_create_ambiguous_expander(tree_class, expansion, keep_all_tokens):
     to_expand = [i for i, sym in enumerate(expansion)
                  if keep_all_tokens or ((not (sym.is_term and sym.filter_out)) and _should_expand(sym))]
     if to_expand:
         return partial(AmbiguousExpander, to_expand, tree_class)
@@ -1700,20 +1989,14 @@
         if collapsed:
             processed_nodes = [self.node_builder(c.children) for c in collapsed]
             return self.tree_class('_ambig', processed_nodes)
 
         return self.node_builder(children)
 
 
-def ptb_inline_args(func):
-    @wraps(func)
-    def f(children):
-        return func(*children)
-    return f
-
 
 def inplace_transformer(func):
     @wraps(func)
     def f(children):
         ##
 
         tree = Tree(func.__name__, children)
@@ -1737,49 +2020,53 @@
         self.propagate_positions = propagate_positions
         self.ambiguous = ambiguous
         self.maybe_placeholders = maybe_placeholders
 
         self.rule_builders = list(self._init_builders(rules))
 
     def _init_builders(self, rules):
+        propagate_positions = make_propagate_positions(self.propagate_positions)
+
         for rule in rules:
             options = rule.options
             keep_all_tokens = options.keep_all_tokens
             expand_single_child = options.expand1
 
             wrapper_chain = list(filter(None, [
                 (expand_single_child and not rule.alias) and ExpandSingleChild,
                 maybe_create_child_filter(rule.expansion, keep_all_tokens, self.ambiguous, options.empty_indices if self.maybe_placeholders else None),
-                self.propagate_positions and PropagatePositions,
+                propagate_positions,
                 self.ambiguous and maybe_create_ambiguous_expander(self.tree_class, rule.expansion, keep_all_tokens),
                 self.ambiguous and partial(AmbiguousIntermediateExpander, self.tree_class)
             ]))
 
             yield rule, wrapper_chain
 
     def create_callback(self, transformer=None):
         callbacks = {}
 
+        default_handler = getattr(transformer, '__default__', None)
+        if default_handler:
+            def default_callback(data, children):
+                return default_handler(data, children, None)
+        else:
+            default_callback = self.tree_class
+
         for rule, wrapper_chain in self.rule_builders:
 
             user_callback_name = rule.alias or rule.options.template_source or rule.origin.name
             try:
                 f = getattr(transformer, user_callback_name)
-                ##
-
                 wrapper = getattr(f, 'visit_wrapper', None)
                 if wrapper is not None:
                     f = apply_visit_wrapper(f, user_callback_name, wrapper)
-                else:
-                    if isinstance(transformer, InlineTransformer):
-                        f = ptb_inline_args(f)
-                    elif isinstance(transformer, Transformer_InPlace):
-                        f = inplace_transformer(f)
+                elif isinstance(transformer, Transformer_InPlace):
+                    f = inplace_transformer(f)
             except AttributeError:
-                f = partial(self.tree_class, user_callback_name)
+                f = partial(default_callback, user_callback_name)
 
             for w in wrapper_chain:
                 f = w(f)
 
             if rule in callbacks:
                 raise GrammarError("Rule '%s' already exists" % (rule,))
 
@@ -1802,30 +2089,30 @@
     @classmethod
     def deserialize(cls, data, memo, callbacks, debug=False):
         inst = cls.__new__(cls)
         inst._parse_table = IntParseTable.deserialize(data, memo)
         inst.parser = _Parser(inst._parse_table, callbacks, debug)
         return inst
 
-    def serialize(self, memo):
+    def serialize(self, memo: Any = None) -> Dict[str, Any]:
         return self._parse_table.serialize(memo)
-    
+
     def parse_interactive(self, lexer, start):
         return self.parser.parse(lexer, start, start_interactive=True)
 
     def parse(self, lexer, start, on_error=None):
         try:
             return self.parser.parse(lexer, start)
         except UnexpectedInput as e:
             if on_error is None:
                 raise
 
             while True:
                 if isinstance(e, UnexpectedCharacters):
-                    s = e.interactive_parser.lexer_state.state
+                    s = e.interactive_parser.lexer_thread.state
                     p = s.line_ctr.char_pos
 
                 if not on_error(e):
                     raise e
 
                 if isinstance(e, UnexpectedCharacters):
                     ##
@@ -1843,29 +2130,29 @@
 
                         raise e2
                     e = e2
                 except UnexpectedCharacters as e2:
                     e = e2
 
 
-class ParseConf(object):
+class ParseConf:
     __slots__ = 'parse_table', 'callbacks', 'start', 'start_state', 'end_state', 'states'
 
     def __init__(self, parse_table, callbacks, start):
         self.parse_table = parse_table
 
         self.start_state = self.parse_table.start_states[start]
         self.end_state = self.parse_table.end_states[start]
         self.states = self.parse_table.states
 
         self.callbacks = callbacks
         self.start = start
 
 
-class ParserState(object):
+class ParserState:
     __slots__ = 'parse_conf', 'lexer', 'state_stack', 'value_stack'
 
     def __init__(self, parse_conf, lexer, state_stack=None, value_stack=None):
         self.parse_conf = parse_conf
         self.lexer = lexer
         self.state_stack = state_stack or [self.parse_conf.start_state]
         self.value_stack = value_stack or []
@@ -1935,38 +2222,37 @@
                 assert _action is Shift
                 state_stack.append(new_state)
                 value_stack.append(value)
 
                 if is_end and state_stack[-1] == end_state:
                     return value_stack[-1]
 
-class _Parser(object):
+class _Parser:
     def __init__(self, parse_table, callbacks, debug=False):
         self.parse_table = parse_table
         self.callbacks = callbacks
         self.debug = debug
 
     def parse(self, lexer, start, value_stack=None, state_stack=None, start_interactive=False):
         parse_conf = ParseConf(self.parse_table, self.callbacks, start)
         parser_state = ParserState(parse_conf, lexer, state_stack, value_stack)
         if start_interactive:
             return InteractiveParser(self, parser_state, parser_state.lexer)
         return self.parse_from_state(parser_state)
-    
 
-    def parse_from_state(self, state):
-        ##
 
+    def parse_from_state(self, state, last_token=None):
+        #--
         try:
-            token = None
+            token = last_token
             for token in state.lexer.lex(state):
                 state.feed_token(token)
 
-            token = Token.new_borrow_pos('$END', '', token) if token else Token('$END', '', 0, 1, 1)
-            return state.feed_token(token, True)
+            end_token = Token.new_borrow_pos('$END', '', token) if token else Token('$END', '', 0, 1, 1)
+            return state.feed_token(end_token, True)
         except UnexpectedInput as e:
             try:
                 e.interactive_parser = InteractiveParser(self, state, state.lexer)
             except NameError:
                 pass
             raise e
         except Exception as e:
@@ -1997,15 +2283,14 @@
     def __init__(self, states, start_states, end_states):
         self.states = states
         self.start_states = start_states
         self.end_states = end_states
 
     def serialize(self, memo):
         tokens = Enumerator()
-        rules = Enumerator()
 
         states = {
             state: {tokens.get(token): ((1, arg.serialize(memo)) if action is Reduce else (0, arg))
                     for token, (action, arg) in actions.items()}
             for state, actions in self.states.items()
         }
 
@@ -2056,230 +2341,248 @@
             def __init__(self, lexer_conf):
                 self.lexer = lexer_class(lexer_conf)
             def lex(self, lexer_state, parser_state):
                 return self.lexer.lex(lexer_state.text)
         return CustomLexerWrapper
 
 
-class MakeParsingFrontend:
-    def __init__(self, parser_type, lexer_type):
-        self.parser_type = parser_type
-        self.lexer_type = lexer_type
-
-    def __call__(self, lexer_conf, parser_conf, options):
-        assert isinstance(lexer_conf, LexerConf)
-        assert isinstance(parser_conf, ParserConf)
-        parser_conf.parser_type = self.parser_type
-        lexer_conf.lexer_type = self.lexer_type
-        return ParsingFrontend(lexer_conf, parser_conf, options)
-
-    @classmethod
-    def deserialize(cls, data, memo, lexer_conf, callbacks, options):
-        parser_conf = ParserConf.deserialize(data['parser_conf'], memo)
-        parser = LALR_Parser.deserialize(data['parser'], memo, callbacks, options.debug)
-        parser_conf.callbacks = callbacks
-        return ParsingFrontend(lexer_conf, parser_conf, options, parser=parser)
+def _deserialize_parsing_frontend(data, memo, lexer_conf, callbacks, options):
+    parser_conf = ParserConf.deserialize(data['parser_conf'], memo)
+    cls = (options and options._plugins.get('LALR_Parser')) or LALR_Parser
+    parser = cls.deserialize(data['parser'], memo, callbacks, options.debug)
+    parser_conf.callbacks = callbacks
+    return ParsingFrontend(lexer_conf, parser_conf, options, parser=parser)
 
 
+_parser_creators: 'Dict[str, Callable[[LexerConf, Any, Any], Any]]' = {}
 
 
 class ParsingFrontend(Serialize):
-    __serialize_fields__ = 'lexer_conf', 'parser_conf', 'parser', 'options'
+    __serialize_fields__ = 'lexer_conf', 'parser_conf', 'parser'
 
     def __init__(self, lexer_conf, parser_conf, options, parser=None):
         self.parser_conf = parser_conf
         self.lexer_conf = lexer_conf
         self.options = options
 
         ##
 
         if parser:  ##
 
             self.parser = parser
         else:
-            create_parser = {
-                'lalr': create_lalr_parser,
-                'earley': create_earley_parser,
-                'cyk': CYK_FrontEnd,
-            }[parser_conf.parser_type]
+            create_parser = _parser_creators.get(parser_conf.parser_type)
+            assert create_parser is not None, "{} is not supported in standalone mode".format(
+                    parser_conf.parser_type
+                )
             self.parser = create_parser(lexer_conf, parser_conf, options)
 
         ##
 
         lexer_type = lexer_conf.lexer_type
         self.skip_lexer = False
         if lexer_type in ('dynamic', 'dynamic_complete'):
             assert lexer_conf.postlex is None
             self.skip_lexer = True
             return
 
         try:
             create_lexer = {
-                'standard': create_traditional_lexer,
+                'basic': create_basic_lexer,
                 'contextual': create_contextual_lexer,
             }[lexer_type]
         except KeyError:
             assert issubclass(lexer_type, Lexer), lexer_type
             self.lexer = _wrap_lexer(lexer_type)(lexer_conf)
         else:
-            self.lexer = create_lexer(lexer_conf, self.parser, lexer_conf.postlex)
+            self.lexer = create_lexer(lexer_conf, self.parser, lexer_conf.postlex, options)
 
         if lexer_conf.postlex:
             self.lexer = PostLexConnector(self.lexer, lexer_conf.postlex)
-    
+
     def _verify_start(self, start=None):
         if start is None:
-            start = self.parser_conf.start
-            if len(start) > 1:
-                raise ConfigurationError("Lark initialized with more than 1 possible start rule. Must specify which start rule to parse", start)
-            start ,= start
+            start_decls = self.parser_conf.start
+            if len(start_decls) > 1:
+                raise ConfigurationError("Lark initialized with more than 1 possible start rule. Must specify which start rule to parse", start_decls)
+            start ,= start_decls
         elif start not in self.parser_conf.start:
             raise ConfigurationError("Unknown start rule %s. Must be one of %r" % (start, self.parser_conf.start))
         return start
 
+    def _make_lexer_thread(self, text):
+        cls = (self.options and self.options._plugins.get('LexerThread')) or LexerThread
+        return text if self.skip_lexer else cls.from_text(self.lexer, text)
+
     def parse(self, text, start=None, on_error=None):
-        start = self._verify_start(start)
-        stream = text if self.skip_lexer else LexerThread(self.lexer, text)
+        chosen_start = self._verify_start(start)
         kw = {} if on_error is None else {'on_error': on_error}
-        return self.parser.parse(stream, start, **kw)
-    
+        stream = self._make_lexer_thread(text)
+        return self.parser.parse(stream, chosen_start, **kw)
+
     def parse_interactive(self, text=None, start=None):
-        start = self._verify_start(start)
+        chosen_start = self._verify_start(start)
         if self.parser_conf.parser_type != 'lalr':
             raise ConfigurationError("parse_interactive() currently only works with parser='lalr' ")
-        stream = text if self.skip_lexer else LexerThread(self.lexer, text)
-        return self.parser.parse_interactive(stream, start)
+        stream = self._make_lexer_thread(text)
+        return self.parser.parse_interactive(stream, chosen_start)
 
 
-def get_frontend(parser, lexer):
+def _validate_frontend_args(parser, lexer) -> None:
     assert_config(parser, ('lalr', 'earley', 'cyk'))
     if not isinstance(lexer, type):     ##
 
         expected = {
-            'lalr': ('standard', 'contextual'),
-            'earley': ('standard', 'dynamic', 'dynamic_complete'),
-            'cyk': ('standard', ),
+            'lalr': ('basic', 'contextual'),
+            'earley': ('basic', 'dynamic', 'dynamic_complete'),
+            'cyk': ('basic', ),
          }[parser]
         assert_config(lexer, expected, 'Parser %r does not support lexer %%r, expected one of %%s' % parser)
 
-    return MakeParsingFrontend(parser, lexer)
-
 
 def _get_lexer_callbacks(transformer, terminals):
     result = {}
     for terminal in terminals:
         callback = getattr(transformer, terminal.name, None)
         if callback is not None:
             result[terminal.name] = callback
     return result
 
 class PostLexConnector:
     def __init__(self, lexer, postlexer):
         self.lexer = lexer
         self.postlexer = postlexer
 
-    def make_lexer_state(self, text):
-        return self.lexer.make_lexer_state(text)
-
     def lex(self, lexer_state, parser_state):
         i = self.lexer.lex(lexer_state, parser_state)
         return self.postlexer.process(i)
 
 
 
-def create_traditional_lexer(lexer_conf, parser, postlex):
-    return TraditionalLexer(lexer_conf)
+def create_basic_lexer(lexer_conf, parser, postlex, options):
+    cls = (options and options._plugins.get('BasicLexer')) or BasicLexer
+    return cls(lexer_conf)
 
-def create_contextual_lexer(lexer_conf, parser, postlex):
+def create_contextual_lexer(lexer_conf, parser, postlex, options):
+    cls = (options and options._plugins.get('ContextualLexer')) or ContextualLexer
     states = {idx:list(t.keys()) for idx, t in parser._parse_table.states.items()}
     always_accept = postlex.always_accept if postlex else ()
-    return ContextualLexer(lexer_conf, states, always_accept=always_accept)
+    return cls(lexer_conf, states, always_accept=always_accept)
 
 def create_lalr_parser(lexer_conf, parser_conf, options=None):
     debug = options.debug if options else False
-    return LALR_Parser(parser_conf, debug=debug)
+    cls = (options and options._plugins.get('LALR_Parser')) or LALR_Parser
+    return cls(parser_conf, debug=debug)
 
+_parser_creators['lalr'] = create_lalr_parser
 
-create_earley_parser = NotImplemented
-CYK_FrontEnd = NotImplemented
 
 
 
+class PostLex(ABC):
+    @abstractmethod
+    def process(self, stream: Iterator[Token]) -> Iterator[Token]:
+        return stream
+
+    always_accept: Iterable[str] = ()
+
 class LarkOptions(Serialize):
     #--
+
+    start: List[str]
+    debug: bool
+    transformer: 'Optional[Transformer]'
+    propagate_positions: Union[bool, str]
+    maybe_placeholders: bool
+    cache: Union[bool, str]
+    regex: bool
+    g_regex_flags: int
+    keep_all_tokens: bool
+    tree_class: Any
+    parser: _ParserArgType
+    lexer: _LexerArgType
+    ambiguity: 'Literal["auto", "resolve", "explicit", "forest"]'
+    postlex: Optional[PostLex]
+    priority: 'Optional[Literal["auto", "normal", "invert"]]'
+    lexer_callbacks: Dict[str, Callable[[Token], Token]]
+    use_bytes: bool
+    edit_terminals: Optional[Callable[[TerminalDef], TerminalDef]]
+    import_paths: 'List[Union[str, Callable[[Union[None, str, PackageResource], str], Tuple[str, str]]]]'
+    source_path: Optional[str]
+
     OPTIONS_DOC = """
     **===  General Options  ===**
 
     start
             The start symbol. Either a string, or a list of strings for multiple possible starts (Default: "start")
     debug
-            Display debug information and extra warnings. Use only when debugging (default: False)
+            Display debug information and extra warnings. Use only when debugging (Default: ``False``)
             When used with Earley, it generates a forest graph as "sppf.png", if 'dot' is installed.
     transformer
             Applies the transformer to every parse tree (equivalent to applying it after the parse, but faster)
     propagate_positions
             Propagates (line, column, end_line, end_column) attributes into all tree branches.
+            Accepts ``False``, ``True``, or a callable, which will filter which nodes to ignore when propagating.
     maybe_placeholders
-            When True, the ``[]`` operator returns ``None`` when not matched.
-
+            When ``True``, the ``[]`` operator returns ``None`` when not matched.
             When ``False``,  ``[]`` behaves like the ``?`` operator, and returns no value at all.
-            (default= ``False``. Recommended to set to ``True``)
+            (default= ``True``)
     cache
             Cache the results of the Lark grammar analysis, for x2 to x3 faster loading. LALR only for now.
 
             - When ``False``, does nothing (default)
             - When ``True``, caches to a temporary file in the local directory
             - When given a string, caches to the path pointed by the string
     regex
             When True, uses the ``regex`` module instead of the stdlib ``re``.
     g_regex_flags
             Flags that are applied to all terminals (both regex and strings)
     keep_all_tokens
-            Prevent the tree builder from automagically removing "punctuation" tokens (default: False)
+            Prevent the tree builder from automagically removing "punctuation" tokens (Default: ``False``)
     tree_class
             Lark will produce trees comprised of instances of this class instead of the default ``lark.Tree``.
 
     **=== Algorithm Options ===**
 
     parser
             Decides which parser engine to use. Accepts "earley" or "lalr". (Default: "earley").
             (there is also a "cyk" option for legacy)
     lexer
             Decides whether or not to use a lexer stage
 
             - "auto" (default): Choose for me based on the parser
-            - "standard": Use a standard lexer
+            - "basic": Use a basic lexer
             - "contextual": Stronger lexer (only works with parser="lalr")
             - "dynamic": Flexible and powerful (only with parser="earley")
             - "dynamic_complete": Same as dynamic, but tries *every* variation of tokenizing possible.
     ambiguity
             Decides how to handle ambiguity in the parse. Only relevant if parser="earley"
 
             - "resolve": The parser will automatically choose the simplest derivation
               (it chooses consistently: greedy for tokens, non-greedy for rules)
             - "explicit": The parser will return all derivations wrapped in "_ambig" tree nodes (i.e. a forest).
             - "forest": The parser will return the root of the shared packed parse forest.
 
     **=== Misc. / Domain Specific Options ===**
 
     postlex
-            Lexer post-processing (Default: None) Only works with the standard and contextual lexers.
+            Lexer post-processing (Default: ``None``) Only works with the basic and contextual lexers.
     priority
-            How priorities should be evaluated - auto, none, normal, invert (Default: auto)
+            How priorities should be evaluated - "auto", ``None``, "normal", "invert" (Default: "auto")
     lexer_callbacks
             Dictionary of callbacks for the lexer. May alter tokens during lexing. Use with caution.
     use_bytes
-            Accept an input of type ``bytes`` instead of ``str`` (Python 3 only).
+            Accept an input of type ``bytes`` instead of ``str``.
     edit_terminals
             A callback for editing the terminals before parse.
     import_paths
             A List of either paths or loader functions to specify from where grammars are imported
     source_path
             Override the source of from where the grammar was loaded. Useful for relative imports and unconventional grammar loading
-    **=== End Options ===**
+    **=== End of Options ===**
     """
     if __doc__:
         __doc__ += OPTIONS_DOC
 
 
     ##
 
@@ -2289,195 +2592,207 @@
 
     ##
 
     ##
 
     ##
 
-    ##
-
-    ##
-
-    _defaults = {
+    _defaults: Dict[str, Any] = {
         'debug': False,
         'keep_all_tokens': False,
         'tree_class': None,
         'cache': False,
         'postlex': None,
         'parser': 'earley',
         'lexer': 'auto',
         'transformer': None,
         'start': 'start',
         'priority': 'auto',
         'ambiguity': 'auto',
         'regex': False,
         'propagate_positions': False,
         'lexer_callbacks': {},
-        'maybe_placeholders': False,
+        'maybe_placeholders': True,
         'edit_terminals': None,
         'g_regex_flags': 0,
         'use_bytes': False,
         'import_paths': [],
         'source_path': None,
+        '_plugins': {},
     }
 
-    def __init__(self, options_dict):
+    def __init__(self, options_dict: Dict[str, Any]) -> None:
         o = dict(options_dict)
 
         options = {}
         for name, default in self._defaults.items():
             if name in o:
                 value = o.pop(name)
-                if isinstance(default, bool) and name not in ('cache', 'use_bytes'):
+                if isinstance(default, bool) and name not in ('cache', 'use_bytes', 'propagate_positions'):
                     value = bool(value)
             else:
                 value = default
 
             options[name] = value
 
-        if isinstance(options['start'], STRING_TYPE):
+        if isinstance(options['start'], str):
             options['start'] = [options['start']]
 
         self.__dict__['options'] = options
 
 
         assert_config(self.parser, ('earley', 'lalr', 'cyk', None))
 
         if self.parser == 'earley' and self.transformer:
-            raise ConfigurationError('Cannot specify an embedded transformer when using the Earley algorithm.'
+            raise ConfigurationError('Cannot specify an embedded transformer when using the Earley algorithm. '
                              'Please use your transformer on the resulting parse tree, or use a different algorithm (i.e. LALR)')
 
         if o:
             raise ConfigurationError("Unknown options: %s" % o.keys())
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> Any:
         try:
             return self.__dict__['options'][name]
         except KeyError as e:
             raise AttributeError(e)
 
-    def __setattr__(self, name, value):
+    def __setattr__(self, name: str, value: str) -> None:
         assert_config(name, self.options.keys(), "%r isn't a valid option. Expected one of: %s")
         self.options[name] = value
 
-    def serialize(self, memo):
+    def serialize(self, memo = None) -> Dict[str, Any]:
         return self.options
 
     @classmethod
-    def deserialize(cls, data, memo):
+    def deserialize(cls, data: Dict[str, Any], memo: Dict[int, Union[TerminalDef, Rule]]) -> "LarkOptions":
         return cls(data)
 
 
 ##
 
 ##
 
-_LOAD_ALLOWED_OPTIONS = {'postlex', 'transformer', 'lexer_callbacks', 'use_bytes', 'debug', 'g_regex_flags', 'regex', 'propagate_positions', 'tree_class'}
+_LOAD_ALLOWED_OPTIONS = {'postlex', 'transformer', 'lexer_callbacks', 'use_bytes', 'debug', 'g_regex_flags', 'regex', 'propagate_positions', 'tree_class', '_plugins'}
 
 _VALID_PRIORITY_OPTIONS = ('auto', 'normal', 'invert', None)
 _VALID_AMBIGUITY_OPTIONS = ('auto', 'resolve', 'explicit', 'forest')
 
 
-class PostLex(ABC):
-    @abstractmethod
-    def process(self, stream):
-        return stream
-
-    always_accept = ()
-
+_T = TypeVar('_T', bound="Lark")
 
 class Lark(Serialize):
     #--
-    def __init__(self, grammar, **options):
+
+    source_path: str
+    source_grammar: str
+    grammar: 'Grammar'
+    options: LarkOptions
+    lexer: Lexer
+    terminals: Collection[TerminalDef]
+
+    def __init__(self, grammar: 'Union[Grammar, str, IO[str]]', **options) -> None:
         self.options = LarkOptions(options)
+        re_module: types.ModuleType
 
         ##
 
         use_regex = self.options.regex
         if use_regex:
-            if regex:
+            if _has_regex:
                 re_module = regex
             else:
                 raise ImportError('`regex` module must be installed if calling `Lark(regex=True)`.')
         else:
             re_module = re
 
         ##
 
         if self.options.source_path is None:
             try:
-                self.source_path = grammar.name
+                self.source_path = grammar.name  ##
+
             except AttributeError:
                 self.source_path = '<string>'
         else:
             self.source_path = self.options.source_path
 
         ##
 
         try:
-            read = grammar.read
+            read = grammar.read  ##
+
         except AttributeError:
             pass
         else:
             grammar = read()
 
         cache_fn = None
         cache_md5 = None
-        if isinstance(grammar, STRING_TYPE):
+        if isinstance(grammar, str):
             self.source_grammar = grammar
             if self.options.use_bytes:
                 if not isascii(grammar):
                     raise ConfigurationError("Grammar must be ascii only, when use_bytes=True")
-                if sys.version_info[0] == 2 and self.options.use_bytes != 'force':
-                    raise ConfigurationError("`use_bytes=True` may have issues on python2."
-                                              "Use `use_bytes='force'` to use it at your own risk.")
 
             if self.options.cache:
                 if self.options.parser != 'lalr':
                     raise ConfigurationError("cache only works with parser='lalr' for now")
 
-                unhashable = ('transformer', 'postlex', 'lexer_callbacks', 'edit_terminals')
+                unhashable = ('transformer', 'postlex', 'lexer_callbacks', 'edit_terminals', '_plugins')
                 options_str = ''.join(k+str(v) for k, v in options.items() if k not in unhashable)
                 from . import __version__
                 s = grammar + options_str + __version__ + str(sys.version_info[:2])
-                cache_md5 = hashlib.md5(s.encode('utf8')).hexdigest()
+                cache_md5 = md5_digest(s)
 
-                if isinstance(self.options.cache, STRING_TYPE):
+                if isinstance(self.options.cache, str):
                     cache_fn = self.options.cache
                 else:
                     if self.options.cache is not True:
                         raise ConfigurationError("cache argument must be bool or str")
-                    ##
 
-                    cache_fn = tempfile.gettempdir() + '/.lark_cache_%s_%s_%s.tmp' % ((cache_md5,) + sys.version_info[:2])
+                    try:
+                        username = getpass.getuser()
+                    except Exception:
+                        ##
 
-                if FS.exists(cache_fn):
-                    logger.debug('Loading grammar from cache: %s', cache_fn)
-                    ##
+                        ##
+
+                        ##
+
+                        username = "unknown"
+
+                    cache_fn = tempfile.gettempdir() + "/.lark_cache_%s_%s_%s_%s.tmp" % (username, cache_md5, *sys.version_info[:2])
 
-                    for name in (set(options) - _LOAD_ALLOWED_OPTIONS):
-                        del options[name]
+                old_options = self.options
+                try:
                     with FS.open(cache_fn, 'rb') as f:
-                        old_options = self.options
-                        try:
-                            file_md5 = f.readline().rstrip(b'\n')
-                            cached_used_files = pickle.load(f)
-                            if file_md5 == cache_md5.encode('utf8') and verify_used_files(cached_used_files):
-                                cached_parser_data = pickle.load(f)
-                                self._load(cached_parser_data, **options)
-                                return
-                        except Exception: ##
-
-                            logger.exception("Failed to load Lark from cache: %r. We will try to carry on." % cache_fn)
-                            
-                            ##
+                        logger.debug('Loading grammar from cache: %s', cache_fn)
+                        ##
+
+                        for name in (set(options) - _LOAD_ALLOWED_OPTIONS):
+                            del options[name]
+                        file_md5 = f.readline().rstrip(b'\n')
+                        cached_used_files = pickle.load(f)
+                        if file_md5 == cache_md5.encode('utf8') and verify_used_files(cached_used_files):
+                            cached_parser_data = pickle.load(f)
+                            self._load(cached_parser_data, **options)
+                            return
+                except FileNotFoundError:
+                    ##
 
-                            ##
+                    pass
+                except Exception: ##
 
-                            self.options = old_options
+                    logger.exception("Failed to load Lark from cache: %r. We will try to carry on.", cache_fn)
+
+                    ##
+
+                    ##
+
+                    self.options = old_options
 
 
             ##
 
             self.grammar, used_files = load_grammar(grammar, self.source_path, self.options.import_paths, self.options.keep_all_tokens)
         else:
             assert isinstance(grammar, Grammar)
@@ -2485,48 +2800,49 @@
 
 
         if self.options.lexer == 'auto':
             if self.options.parser == 'lalr':
                 self.options.lexer = 'contextual'
             elif self.options.parser == 'earley':
                 if self.options.postlex is not None:
-                    logger.info("postlex can't be used with the dynamic lexer, so we use standard instead. "
+                    logger.info("postlex can't be used with the dynamic lexer, so we use 'basic' instead. "
                                 "Consider using lalr with contextual instead of earley")
-                    self.options.lexer = 'standard'
+                    self.options.lexer = 'basic'
                 else:
                     self.options.lexer = 'dynamic'
             elif self.options.parser == 'cyk':
-                self.options.lexer = 'standard'
+                self.options.lexer = 'basic'
             else:
                 assert False, self.options.parser
         lexer = self.options.lexer
         if isinstance(lexer, type):
             assert issubclass(lexer, Lexer)     ##
 
         else:
-            assert_config(lexer, ('standard', 'contextual', 'dynamic', 'dynamic_complete'))
+            assert_config(lexer, ('basic', 'contextual', 'dynamic', 'dynamic_complete'))
             if self.options.postlex is not None and 'dynamic' in lexer:
-                raise ConfigurationError("Can't use postlex with a dynamic lexer. Use standard or contextual instead")
+                raise ConfigurationError("Can't use postlex with a dynamic lexer. Use basic or contextual instead")
 
         if self.options.ambiguity == 'auto':
             if self.options.parser == 'earley':
                 self.options.ambiguity = 'resolve'
         else:
             assert_config(self.options.parser, ('earley', 'cyk'), "%r doesn't support disambiguation. Use one of these parsers instead: %s")
 
         if self.options.priority == 'auto':
             self.options.priority = 'normal'
 
         if self.options.priority not in _VALID_PRIORITY_OPTIONS:
             raise ConfigurationError("invalid priority option: %r. Must be one of %r" % (self.options.priority, _VALID_PRIORITY_OPTIONS))
-        assert self.options.ambiguity not in ('resolve__antiscore_sum', ), 'resolve__antiscore_sum has been replaced with the option priority="invert"'
         if self.options.ambiguity not in _VALID_AMBIGUITY_OPTIONS:
             raise ConfigurationError("invalid ambiguity option: %r. Must be one of %r" % (self.options.ambiguity, _VALID_AMBIGUITY_OPTIONS))
 
-        if self.options.postlex is not None:
+        if self.options.parser is None:
+            terminals_to_keep = '*'
+        elif self.options.postlex is not None:
             terminals_to_keep = set(self.options.postlex.always_accept)
         else:
             terminals_to_keep = set()
 
         ##
 
         self.terminals, self.rules, self.ignore_tokens = self.grammar.compile(self.options.start, terminals_to_keep)
@@ -2535,30 +2851,32 @@
             for t in self.terminals:
                 self.options.edit_terminals(t)
 
         self._terminals_dict = {t.name: t for t in self.terminals}
 
         ##
 
-        ##
-
         if self.options.priority == 'invert':
             for rule in self.rules:
                 if rule.options.priority is not None:
                     rule.options.priority = -rule.options.priority
+            for term in self.terminals:
+                term.priority = -term.priority
         ##
 
         ##
 
         ##
 
         elif self.options.priority is None:
             for rule in self.rules:
                 if rule.options.priority is not None:
                     rule.options.priority = None
+            for term in self.terminals:
+                term.priority = 0
 
         ##
 
         self.lexer_conf = LexerConf(
                 self.terminals, re_module, self.ignore_tokens, self.options.postlex,
                 self.options.lexer_callbacks, self.options.g_regex_flags, use_bytes=self.options.use_bytes
             )
@@ -2566,98 +2884,110 @@
         if self.options.parser:
             self.parser = self._build_parser()
         elif lexer:
             self.lexer = self._build_lexer()
 
         if cache_fn:
             logger.debug('Saving grammar to cache: %s', cache_fn)
-            with FS.open(cache_fn, 'wb') as f:
-                f.write(cache_md5.encode('utf8') + b'\n')
-                pickle.dump(used_files, f)
-                self.save(f)
+            try:
+                with FS.open(cache_fn, 'wb') as f:
+                    assert cache_md5 is not None
+                    f.write(cache_md5.encode('utf8') + b'\n')
+                    pickle.dump(used_files, f)
+                    self.save(f, _LOAD_ALLOWED_OPTIONS)
+            except IOError as e:
+                logger.exception("Failed to save Lark to cache: %r.", cache_fn, e)
 
     if __doc__:
         __doc__ += "\n\n" + LarkOptions.OPTIONS_DOC
 
     __serialize_fields__ = 'parser', 'rules', 'options'
 
-    def _build_lexer(self, dont_ignore=False):
+    def _build_lexer(self, dont_ignore: bool=False) -> BasicLexer:
         lexer_conf = self.lexer_conf
         if dont_ignore:
             from copy import copy
             lexer_conf = copy(lexer_conf)
             lexer_conf.ignore = ()
-        return TraditionalLexer(lexer_conf)
+        return BasicLexer(lexer_conf)
 
-    def _prepare_callbacks(self):
+    def _prepare_callbacks(self) -> None:
         self._callbacks = {}
         ##
 
         if self.options.ambiguity != 'forest':
             self._parse_tree_builder = ParseTreeBuilder(
                     self.rules,
                     self.options.tree_class or Tree,
                     self.options.propagate_positions,
                     self.options.parser != 'lalr' and self.options.ambiguity == 'explicit',
                     self.options.maybe_placeholders
                 )
             self._callbacks = self._parse_tree_builder.create_callback(self.options.transformer)
         self._callbacks.update(_get_lexer_callbacks(self.options.transformer, self.terminals))
 
-    def _build_parser(self):
+    def _build_parser(self) -> "ParsingFrontend":
         self._prepare_callbacks()
-        parser_class = get_frontend(self.options.parser, self.options.lexer)
+        _validate_frontend_args(self.options.parser, self.options.lexer)
         parser_conf = ParserConf(self.rules, self._callbacks, self.options.start)
-        return parser_class(self.lexer_conf, parser_conf, options=self.options)
+        return _construct_parsing_frontend(
+            self.options.parser,
+            self.options.lexer,
+            self.lexer_conf,
+            parser_conf,
+            options=self.options
+        )
 
-    def save(self, f):
+    def save(self, f, exclude_options: Collection[str] = ()) -> None:
         #--
         data, m = self.memo_serialize([TerminalDef, Rule])
+        if exclude_options:
+            data["options"] = {n: v for n, v in data["options"].items() if n not in exclude_options}
         pickle.dump({'data': data, 'memo': m}, f, protocol=pickle.HIGHEST_PROTOCOL)
 
     @classmethod
-    def load(cls, f):
+    def load(cls: Type[_T], f) -> _T:
         #--
         inst = cls.__new__(cls)
         return inst._load(f)
 
-    def _deserialize_lexer_conf(self, data, memo, options):
+    def _deserialize_lexer_conf(self, data: Dict[str, Any], memo: Dict[int, Union[TerminalDef, Rule]], options: LarkOptions) -> LexerConf:
         lexer_conf = LexerConf.deserialize(data['lexer_conf'], memo)
         lexer_conf.callbacks = options.lexer_callbacks or {}
         lexer_conf.re_module = regex if options.regex else re
         lexer_conf.use_bytes = options.use_bytes
         lexer_conf.g_regex_flags = options.g_regex_flags
         lexer_conf.skip_validation = True
         lexer_conf.postlex = options.postlex
         return lexer_conf
 
-    def _load(self, f, **kwargs):
+    def _load(self: _T, f: Any, **kwargs) -> _T:
         if isinstance(f, dict):
             d = f
         else:
             d = pickle.load(f)
-        memo = d['memo']
+        memo_json = d['memo']
         data = d['data']
 
-        assert memo
-        memo = SerializeMemoizer.deserialize(memo, {'Rule': Rule, 'TerminalDef': TerminalDef}, {})
+        assert memo_json
+        memo = SerializeMemoizer.deserialize(memo_json, {'Rule': Rule, 'TerminalDef': TerminalDef}, {})
         options = dict(data['options'])
         if (set(kwargs) - _LOAD_ALLOWED_OPTIONS) & set(LarkOptions._defaults):
             raise ConfigurationError("Some options are not allowed when loading a Parser: {}"
                              .format(set(kwargs) - _LOAD_ALLOWED_OPTIONS))
         options.update(kwargs)
         self.options = LarkOptions.deserialize(options, memo)
         self.rules = [Rule.deserialize(r, memo) for r in data['rules']]
         self.source_path = '<deserialized>'
-        parser_class = get_frontend(self.options.parser, self.options.lexer)
+        _validate_frontend_args(self.options.parser, self.options.lexer)
         self.lexer_conf = self._deserialize_lexer_conf(data['parser'], memo, self.options)
         self.terminals = self.lexer_conf.terminals
         self._prepare_callbacks()
         self._terminals_dict = {t.name: t for t in self.terminals}
-        self.parser = parser_class.deserialize(
+        self.parser = _deserialize_parsing_frontend(
             data['parser'],
             memo,
             self.lexer_conf,
             self._callbacks,
             self.options,  ##
 
         )
@@ -2665,89 +2995,77 @@
 
     @classmethod
     def _load_from_dict(cls, data, memo, **kwargs):
         inst = cls.__new__(cls)
         return inst._load({'data': data, 'memo': memo}, **kwargs)
 
     @classmethod
-    def open(cls, grammar_filename, rel_to=None, **options):
+    def open(cls: Type[_T], grammar_filename: str, rel_to: Optional[str]=None, **options) -> _T:
         #--
         if rel_to:
             basepath = os.path.dirname(rel_to)
             grammar_filename = os.path.join(basepath, grammar_filename)
         with open(grammar_filename, encoding='utf8') as f:
             return cls(f, **options)
 
     @classmethod
-    def open_from_package(cls, package, grammar_path, search_paths=("",), **options):
+    def open_from_package(cls: Type[_T], package: str, grammar_path: str, search_paths: 'Sequence[str]'=[""], **options) -> _T:
         #--
-        package = FromPackageLoader(package, search_paths)
-        full_path, text = package(None, grammar_path)
+        package_loader = FromPackageLoader(package, search_paths)
+        full_path, text = package_loader(None, grammar_path)
         options.setdefault('source_path', full_path)
         options.setdefault('import_paths', [])
-        options['import_paths'].append(package)
+        options['import_paths'].append(package_loader)
         return cls(text, **options)
 
     def __repr__(self):
         return 'Lark(open(%r), parser=%r, lexer=%r, ...)' % (self.source_path, self.options.parser, self.options.lexer)
 
 
-    def lex(self, text, dont_ignore=False):
+    def lex(self, text: str, dont_ignore: bool=False) -> Iterator[Token]:
         #--
+        lexer: Lexer
         if not hasattr(self, 'lexer') or dont_ignore:
             lexer = self._build_lexer(dont_ignore)
         else:
             lexer = self.lexer
-        lexer_thread = LexerThread(lexer, text)
+        lexer_thread = LexerThread.from_text(lexer, text)
         stream = lexer_thread.lex(None)
         if self.options.postlex:
             return self.options.postlex.process(stream)
         return stream
 
-    def get_terminal(self, name):
+    def get_terminal(self, name: str) -> TerminalDef:
         #--
         return self._terminals_dict[name]
-    
-    def parse_interactive(self, text=None, start=None):
+
+    def parse_interactive(self, text: Optional[str]=None, start: Optional[str]=None) -> 'InteractiveParser':
+        #--
         return self.parser.parse_interactive(text, start=start)
 
-    def parse(self, text, start=None, on_error=None):
+    def parse(self, text: str, start: Optional[str]=None, on_error: 'Optional[Callable[[UnexpectedInput], bool]]'=None) -> 'ParseTree':
         #--
         return self.parser.parse(text, start=start, on_error=on_error)
 
-    @property
-    def source(self):
-        warn("Lark.source attribute has been renamed to Lark.source_path", DeprecationWarning)
-        return self.source_path
-
-    @source.setter
-    def source(self, value):
-        self.source_path = value
-
-    @property
-    def grammar_source(self):
-        warn("Lark.grammar_source attribute has been renamed to Lark.source_grammar", DeprecationWarning)
-        return self.source_grammar
-
-    @grammar_source.setter
-    def grammar_source(self, value):
-        self.source_grammar = value
 
 
 
 class DedentError(LarkError):
     pass
 
-class Indenter(PostLex):
-    def __init__(self):
-        self.paren_level = None
-        self.indent_level = None
+class Indenter(PostLex, ABC):
+    paren_level: int
+    indent_level: List[int]
+
+    def __init__(self) -> None:
+        self.paren_level = 0
+        self.indent_level = [0]
         assert self.tab_len > 0
 
-    def handle_NL(self, token):
+    def handle_NL(self, token: Token) -> Iterator[Token]:
         if self.paren_level > 0:
             return
 
         yield token
 
         indent_str = token.rsplit('\n', 1)[1] ##
 
@@ -2763,16 +3081,15 @@
 
             if indent != self.indent_level[-1]:
                 raise DedentError('Unexpected dedent to column %s. Expected dedent to %s' % (indent, self.indent_level[-1]))
 
     def _process(self, stream):
         for token in stream:
             if token.type == self.NL_type:
-                for t in self.handle_NL(token):
-                    yield t
+                yield from self.handle_NL(token)
             else:
                 yield token
 
             if token.type in self.OPEN_PAREN_types:
                 self.paren_level += 1
             elif token.type in self.CLOSE_PAREN_types:
                 self.paren_level -= 1
@@ -2791,19 +3108,58 @@
 
     ##
 
     @property
     def always_accept(self):
         return (self.NL_type,)
 
+    @property
+    @abstractmethod
+    def NL_type(self) -> str:
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def OPEN_PAREN_types(self) -> List[str]:
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def CLOSE_PAREN_types(self) -> List[str]:
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def INDENT_type(self) -> str:
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def DEDENT_type(self) -> str:
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def tab_len(self) -> int:
+        raise NotImplementedError()
+
+
+class PythonIndenter(Indenter):
+    NL_type = '_NEWLINE'
+    OPEN_PAREN_types = ['LPAR', 'LSQB', 'LBRACE']
+    CLOSE_PAREN_types = ['RPAR', 'RSQB', 'RBRACE']
+    INDENT_type = '_INDENT'
+    DEDENT_type = '_DEDENT'
+    tab_len = 8
+
 
 import pickle, zlib, base64
 DATA = (
-{'parser': {'lexer_conf': {'terminals': [{'@': 0}, {'@': 1}, {'@': 2}, {'@': 3}, {'@': 4}, {'@': 5}, {'@': 6}, {'@': 7}, {'@': 8}, {'@': 9}, {'@': 10}, {'@': 11}, {'@': 12}, {'@': 13}, {'@': 14}, {'@': 15}, {'@': 16}, {'@': 17}, {'@': 18}, {'@': 19}, {'@': 20}, {'@': 21}], 'ignore': ['WS_INLINE'], 'g_regex_flags': 0, 'use_bytes': False, 'lexer_type': 'contextual', '__type__': 'LexerConf'}, 'parser_conf': {'rules': [{'@': 22}, {'@': 23}, {'@': 24}, {'@': 25}, {'@': 26}, {'@': 27}, {'@': 28}, {'@': 29}, {'@': 30}, {'@': 31}, {'@': 32}, {'@': 33}, {'@': 34}, {'@': 35}, {'@': 36}, {'@': 37}, {'@': 38}, {'@': 39}, {'@': 40}, {'@': 41}, {'@': 42}, {'@': 43}, {'@': 44}, {'@': 45}, {'@': 46}, {'@': 47}, {'@': 48}, {'@': 49}, {'@': 50}, {'@': 51}, {'@': 52}, {'@': 53}, {'@': 54}, {'@': 55}, {'@': 56}, {'@': 57}, {'@': 58}, {'@': 59}, {'@': 60}, {'@': 61}, {'@': 62}, {'@': 63}, {'@': 64}, {'@': 65}, {'@': 66}, {'@': 67}, {'@': 68}, {'@': 69}, {'@': 70}, {'@': 71}, {'@': 72}, {'@': 73}, {'@': 74}, {'@': 75}, {'@': 76}], 'start': ['start'], 'parser_type': 'lalr', '__type__': 'ParserConf'}, 'parser': {'tokens': {0: 'AND', 1: 'COMMA', 2: 'OR', 3: 'DOT', 4: 'RPAR', 5: 'LSQB', 6: 'DOUBLE_DOT', 7: 'COMPARE_OPERATOR', 8: 'COLON', 9: 'RSQB', 10: 'predicate', 11: 'identifier', 12: 'STRING', 13: 'CNAME', 14: '$END', 15: 'AT', 16: 'path', 17: 'NUMBER', 18: 'test_comparison', 19: 'atom', 20: 'funccall', 21: 'path_with_action', 22: 'test', 23: 'false', 24: 'first_path', 25: 'root', 26: 'value', 27: 'DOLLAR', 28: 'FALSE', 29: 'true', 30: 'test_and', 31: 'args', 32: 'LPAR', 33: 'TRUE', 34: 'NULL', 35: 'self', 36: 'null', 37: 'expr', 38: 'action_separate_with_dot', 39: '__ANON_0', 40: 'start', 41: 'STAR', 42: 'slice'}, 'states': {0: {0: (1, {'@': 38}), 1: (1, {'@': 38}), 2: (1, {'@': 38}), 3: (1, {'@': 38}), 4: (1, {'@': 38}), 5: (1, {'@': 38}), 6: (1, {'@': 38}), 7: (1, {'@': 38}), 8: (1, {'@': 38}), 9: (1, {'@': 38})}, 1: {5: (0, 42), 10: (0, 64), 11: (0, 22), 12: (0, 43), 13: (0, 33)}, 2: {0: (1, {'@': 50}), 1: (1, {'@': 50}), 2: (1, {'@': 50}), 3: (1, {'@': 50}), 4: (1, {'@': 50}), 5: (1, {'@': 50}), 6: (1, {'@': 50}), 7: (1, {'@': 50}), 8: (1, {'@': 50}), 9: (1, {'@': 50}), 14: (1, {'@': 50})}, 3: {0: (1, {'@': 49}), 1: (1, {'@': 49}), 2: (1, {'@': 49}), 3: (1, {'@': 49}), 4: (1, {'@': 49}), 5: (1, {'@': 49}), 6: (1, {'@': 49}), 7: (1, {'@': 49}), 8: (1, {'@': 49}), 9: (1, {'@': 49}), 14: (1, {'@': 49})}, 4: {15: (0, 41), 16: (0, 49), 12: (0, 18), 17: (0, 71), 13: (0, 26), 18: (0, 63), 19: (0, 60), 20: (0, 36), 21: (0, 40), 22: (0, 54), 23: (0, 27), 24: (0, 53), 25: (0, 2), 26: (0, 24), 27: (0, 68), 28: (0, 39), 29: (0, 7), 30: (0, 32), 31: (0, 31), 32: (0, 70), 33: (0, 20), 34: (0, 0), 35: (0, 3), 36: (0, 69), 37: (0, 19)}, 5: {9: (0, 21)}, 6: {4: (1, {'@': 68}), 1: (1, {'@': 68})}, 7: {0: (1, {'@': 40}), 1: (1, {'@': 40}), 2: (1, {'@': 40}), 3: (1, {'@': 40}), 4: (1, {'@': 40}), 5: (1, {'@': 40}), 6: (1, {'@': 40}), 7: (1, {'@': 40}), 8: (1, {'@': 40}), 9: (1, {'@': 40})}, 8: {14: (1, {'@': 63}), 3: (1, {'@': 63}), 5: (1, {'@': 63}), 6: (1, {'@': 63}), 0: (1, {'@': 63}), 2: (1, {'@': 63}), 4: (1, {'@': 63}), 8: (1, {'@': 63}), 1: (1, {'@': 63}), 9: (1, {'@': 63}), 7: (1, {'@': 63})}, 9: {30: (0, 59), 24: (0, 53), 15: (0, 41), 25: (0, 2), 26: (0, 24), 27: (0, 68), 16: (0, 49), 12: (0, 18), 28: (0, 39), 17: (0, 71), 29: (0, 7), 19: (0, 60), 13: (0, 26), 18: (0, 63), 32: (0, 70), 33: (0, 20), 34: (0, 0), 20: (0, 36), 21: (0, 40), 35: (0, 3), 36: (0, 69), 23: (0, 27)}, 10: {15: (0, 41), 16: (0, 49), 12: (0, 18), 17: (0, 71), 13: (0, 26), 18: (0, 63), 19: (0, 60), 20: (0, 36), 21: (0, 40), 22: (0, 54), 23: (0, 27), 24: (0, 53), 25: (0, 2), 26: (0, 24), 27: (0, 68), 28: (0, 39), 29: (0, 7), 37: (0, 51), 30: (0, 32), 32: (0, 70), 33: (0, 20), 34: (0, 0), 35: (0, 3), 36: (0, 69), 9: (1, {'@': 27})}, 11: {0: (1, {'@': 65}), 1: (1, {'@': 65}), 2: (1, {'@': 65}), 3: (1, {'@': 65}), 4: (1, {'@': 65}), 5: (1, {'@': 65}), 6: (1, {'@': 65}), 7: (1, {'@': 65}), 8: (1, {'@': 65}), 9: (1, {'@': 65}), 14: (1, {'@': 65})}, 12: {24: (0, 53), 15: (0, 41), 25: (0, 2), 26: (0, 24), 27: (0, 68), 16: (0, 49), 12: (0, 18), 28: (0, 39), 17: (0, 71), 29: (0, 7), 19: (0, 60), 13: (0, 26), 18: (0, 63), 30: (0, 32), 32: (0, 70), 37: (0, 6), 33: (0, 20), 34: (0, 0), 20: (0, 36), 21: (0, 40), 35: (0, 3), 36: (0, 69), 22: (0, 54), 23: (0, 27)}, 13: {}, 14: {0: (1, {'@': 55}), 2: (1, {'@': 55}), 4: (1, {'@': 55}), 1: (1, {'@': 55}), 8: (1, {'@': 55}), 9: (1, {'@': 55})}, 15: {15: (0, 41), 16: (0, 49), 12: (0, 18), 17: (0, 71), 13: (0, 26), 18: (0, 63), 19: (0, 60), 20: (0, 36), 21: (0, 40), 37: (0, 17), 22: (0, 54), 23: (0, 27), 8: (0, 10), 24: (0, 53), 25: (0, 2), 26: (0, 24), 27: (0, 68), 28: (0, 39), 29: (0, 7), 30: (0, 32), 32: (0, 70), 33: (0, 20), 34: (0, 0), 35: (0, 3), 36: (0, 69), 9: (1, {'@': 33})}, 16: {5: (0, 42), 38: (0, 44), 6: (0, 1), 3: (0, 56), 10: (0, 11)}, 17: {8: (0, 57), 9: (1, {'@': 32})}, 18: {0: (1, {'@': 43}), 1: (1, {'@': 43}), 2: (1, {'@': 43}), 3: (1, {'@': 43}), 4: (1, {'@': 43}), 5: (1, {'@': 43}), 6: (1, {'@': 43}), 7: (1, {'@': 43}), 8: (1, {'@': 43}), 9: (1, {'@': 43})}, 19: {4: (1, {'@': 69}), 1: (1, {'@': 69})}, 20: {0: (1, {'@': 36}), 1: (1, {'@': 36}), 2: (1, {'@': 36}), 3: (1, {'@': 36}), 4: (1, {'@': 36}), 5: (1, {'@': 36}), 6: (1, {'@': 36}), 7: (1, {'@': 36}), 8: (1, {'@': 36}), 9: (1, {'@': 36})}, 21: {0: (1, {'@': 58}), 2: (1, {'@': 58}), 3: (1, {'@': 58}), 5: (1, {'@': 58}), 8: (1, {'@': 58}), 7: (1, {'@': 58}), 9: (1, {'@': 58}), 4: (1, {'@': 58}), 6: (1, {'@': 58}), 14: (1, {'@': 58}), 1: (1, {'@': 58})}, 22: {14: (1, {'@': 61}), 3: (1, {'@': 61}), 5: (1, {'@': 61}), 6: (1, {'@': 61}), 0: (1, {'@': 61}), 2: (1, {'@': 61}), 4: (1, {'@': 61}), 8: (1, {'@': 61}), 1: (1, {'@': 61}), 9: (1, {'@': 61}), 7: (1, {'@': 61})}, 23: {9: (1, {'@': 30})}, 24: {0: (1, {'@': 72}), 1: (1, {'@': 72}), 2: (1, {'@': 72}), 3: (1, {'@': 72}), 4: (1, {'@': 72}), 5: (1, {'@': 72}), 6: (1, {'@': 72}), 7: (1, {'@': 72}), 8: (1, {'@': 72}), 9: (1, {'@': 72})}, 25: {0: (1, {'@': 71}), 1: (1, {'@': 71}), 2: (1, {'@': 71}), 3: (1, {'@': 71}), 4: (1, {'@': 71}), 5: (1, {'@': 71}), 6: (1, {'@': 71}), 7: (1, {'@': 71}), 8: (1, {'@': 71}), 9: (1, {'@': 71}), 14: (1, {'@': 71})}, 26: {32: (0, 4), 39: (0, 25), 0: (1, {'@': 48}), 1: (1, {'@': 48}), 2: (1, {'@': 48}), 3: (1, {'@': 48}), 4: (1, {'@': 48}), 5: (1, {'@': 48}), 6: (1, {'@': 48}), 7: (1, {'@': 48}), 8: (1, {'@': 48}), 9: (1, {'@': 48}), 14: (1, {'@': 48})}, 27: {0: (1, {'@': 41}), 1: (1, {'@': 41}), 2: (1, {'@': 41}), 3: (1, {'@': 41}), 4: (1, {'@': 41}), 5: (1, {'@': 41}), 6: (1, {'@': 41}), 7: (1, {'@': 41}), 8: (1, {'@': 41}), 9: (1, {'@': 41})}, 28: {8: (0, 15), 9: (0, 29)}, 29: {0: (1, {'@': 57}), 2: (1, {'@': 57}), 3: (1, {'@': 57}), 5: (1, {'@': 57}), 8: (1, {'@': 57}), 7: (1, {'@': 57}), 9: (1, {'@': 57}), 4: (1, {'@': 57}), 6: (1, {'@': 57}), 14: (1, {'@': 57}), 1: (1, {'@': 57})}, 30: {37: (0, 23), 15: (0, 41), 16: (0, 49), 12: (0, 18), 17: (0, 71), 13: (0, 26), 18: (0, 63), 19: (0, 60), 20: (0, 36), 21: (0, 40), 22: (0, 54), 23: (0, 27), 24: (0, 53), 25: (0, 2), 26: (0, 24), 27: (0, 68), 28: (0, 39), 29: (0, 7), 30: (0, 32), 32: (0, 70), 33: (0, 20), 34: (0, 0), 35: (0, 3), 36: (0, 69), 9: (1, {'@': 31})}, 31: {4: (0, 55), 1: (0, 12)}, 32: {0: (0, 52), 2: (1, {'@': 54}), 4: (1, {'@': 54}), 1: (1, {'@': 54}), 9: (1, {'@': 54}), 8: (1, {'@': 54})}, 33: {0: (1, {'@': 44}), 2: (1, {'@': 44}), 3: (1, {'@': 44}), 5: (1, {'@': 44}), 8: (1, {'@': 44}), 7: (1, {'@': 44}), 9: (1, {'@': 44}), 4: (1, {'@': 44}), 6: (1, {'@': 44}), 14: (1, {'@': 44}), 1: (1, {'@': 44})}, 34: {37: (0, 45), 15: (0, 41), 16: (0, 49), 12: (0, 18), 17: (0, 71), 13: (0, 26), 18: (0, 63), 19: (0, 60), 20: (0, 36), 21: (0, 40), 22: (0, 54), 23: (0, 27), 24: (0, 53), 25: (0, 2), 26: (0, 24), 27: (0, 68), 28: (0, 39), 29: (0, 7), 30: (0, 32), 32: (0, 70), 33: (0, 20), 34: (0, 0), 35: (0, 3), 36: (0, 69), 9: (1, {'@': 29})}, 35: {16: (0, 47), 24: (0, 53), 15: (0, 41), 25: (0, 2), 26: (0, 24), 27: (0, 68), 12: (0, 18), 28: (0, 39), 17: (0, 71), 29: (0, 7), 13: (0, 26), 19: (0, 16), 40: (0, 13), 32: (0, 70), 33: (0, 20), 34: (0, 0), 20: (0, 48), 21: (0, 40), 35: (0, 3), 36: (0, 69), 23: (0, 27)}, 36: {0: (1, {'@': 74}), 1: (1, {'@': 74}), 2: (1, {'@': 74}), 3: (1, {'@': 74}), 4: (1, {'@': 74}), 5: (1, {'@': 74}), 6: (1, {'@': 74}), 7: (1, {'@': 74}), 8: (1, {'@': 74}), 9: (1, {'@': 74})}, 37: {5: (0, 42), 38: (0, 44), 6: (0, 1), 3: (0, 56), 10: (0, 11), 0: (1, {'@': 51}), 2: (1, {'@': 51}), 4: (1, {'@': 51}), 1: (1, {'@': 51}), 8: (1, {'@': 51}), 9: (1, {'@': 51})}, 38: {4: (0, 58)}, 39: {0: (1, {'@': 37}), 1: (1, {'@': 37}), 2: (1, {'@': 37}), 3: (1, {'@': 37}), 4: (1, {'@': 37}), 5: (1, {'@': 37}), 6: (1, {'@': 37}), 7: (1, {'@': 37}), 8: (1, {'@': 37}), 9: (1, {'@': 37})}, 40: {0: (1, {'@': 66}), 1: (1, {'@': 66}), 2: (1, {'@': 66}), 3: (1, {'@': 66}), 4: (1, {'@': 66}), 5: (1, {'@': 66}), 6: (1, {'@': 66}), 7: (1, {'@': 66}), 8: (1, {'@': 66}), 9: (1, {'@': 66}), 14: (1, {'@': 66})}, 41: {0: (1, {'@': 46}), 1: (1, {'@': 46}), 2: (1, {'@': 46}), 3: (1, {'@': 46}), 4: (1, {'@': 46}), 5: (1, {'@': 46}), 6: (1, {'@': 46}), 7: (1, {'@': 46}), 8: (1, {'@': 46}), 9: (1, {'@': 46}), 14: (1, {'@': 46})}, 42: {37: (0, 28), 15: (0, 41), 30: (0, 32), 16: (0, 49), 8: (0, 61), 12: (0, 18), 17: (0, 71), 13: (0, 26), 18: (0, 63), 19: (0, 60), 20: (0, 36), 21: (0, 40), 22: (0, 54), 41: (0, 65), 23: (0, 27), 24: (0, 53), 25: (0, 2), 26: (0, 24), 27: (0, 68), 28: (0, 39), 29: (0, 7), 42: (0, 5), 32: (0, 70), 33: (0, 20), 34: (0, 0), 35: (0, 3), 36: (0, 69)}, 43: {0: (1, {'@': 45}), 2: (1, {'@': 45}), 3: (1, {'@': 45}), 5: (1, {'@': 45}), 8: (1, {'@': 45}), 7: (1, {'@': 45}), 9: (1, {'@': 45}), 4: (1, {'@': 45}), 6: (1, {'@': 45}), 14: (1, {'@': 45}), 1: (1, {'@': 45})}, 44: {0: (1, {'@': 64}), 1: (1, {'@': 64}), 2: (1, {'@': 64}), 3: (1, {'@': 64}), 4: (1, {'@': 64}), 5: (1, {'@': 64}), 6: (1, {'@': 64}), 7: (1, {'@': 64}), 8: (1, {'@': 64}), 9: (1, {'@': 64}), 14: (1, {'@': 64})}, 45: {9: (1, {'@': 28})}, 46: {9: (1, {'@': 24})}, 47: {3: (1, {'@': 73}), 5: (1, {'@': 73}), 6: (1, {'@': 73}), 14: (1, {'@': 22})}, 48: {3: (1, {'@': 74}), 5: (1, {'@': 74}), 6: (1, {'@': 74}), 14: (1, {'@': 23})}, 49: {0: (1, {'@': 73}), 1: (1, {'@': 73}), 2: (1, {'@': 73}), 3: (1, {'@': 73}), 4: (1, {'@': 73}), 5: (1, {'@': 73}), 6: (1, {'@': 73}), 7: (1, {'@': 73}), 8: (1, {'@': 73}), 9: (1, {'@': 73})}, 50: {14: (1, {'@': 62}), 3: (1, {'@': 62}), 5: (1, {'@': 62}), 6: (1, {'@': 62}), 0: (1, {'@': 62}), 2: (1, {'@': 62}), 4: (1, {'@': 62}), 8: (1, {'@': 62}), 1: (1, {'@': 62}), 9: (1, {'@': 62}), 7: (1, {'@': 62})}, 51: {9: (1, {'@': 26})}, 52: {24: (0, 53), 15: (0, 41), 25: (0, 2), 26: (0, 24), 27: (0, 68), 16: (0, 49), 12: (0, 18), 28: (0, 39), 17: (0, 71), 29: (0, 7), 19: (0, 60), 13: (0, 26), 18: (0, 14), 32: (0, 70), 33: (0, 20), 34: (0, 0), 20: (0, 36), 21: (0, 40), 35: (0, 3), 36: (0, 69), 23: (0, 27)}, 53: {0: (1, {'@': 67}), 1: (1, {'@': 67}), 2: (1, {'@': 67}), 3: (1, {'@': 67}), 4: (1, {'@': 67}), 5: (1, {'@': 67}), 6: (1, {'@': 67}), 7: (1, {'@': 67}), 8: (1, {'@': 67}), 9: (1, {'@': 67}), 14: (1, {'@': 67})}, 54: {2: (0, 9), 4: (1, {'@': 76}), 1: (1, {'@': 76}), 9: (1, {'@': 76}), 8: (1, {'@': 76})}, 55: {0: (1, {'@': 70}), 1: (1, {'@': 70}), 2: (1, {'@': 70}), 3: (1, {'@': 70}), 4: (1, {'@': 70}), 5: (1, {'@': 70}), 6: (1, {'@': 70}), 7: (1, {'@': 70}), 8: (1, {'@': 70}), 9: (1, {'@': 70}), 14: (1, {'@': 70})}, 56: {11: (0, 50), 13: (0, 33), 41: (0, 8), 12: (0, 43)}, 57: {15: (0, 41), 16: (0, 49), 12: (0, 18), 17: (0, 71), 13: (0, 26), 18: (0, 63), 19: (0, 60), 20: (0, 36), 21: (0, 40), 22: (0, 54), 23: (0, 27), 24: (0, 53), 25: (0, 2), 26: (0, 24), 27: (0, 68), 28: (0, 39), 29: (0, 7), 30: (0, 32), 32: (0, 70), 33: (0, 20), 34: (0, 0), 35: (0, 3), 36: (0, 69), 37: (0, 46), 9: (1, {'@': 25})}, 58: {0: (1, {'@': 75}), 1: (1, {'@': 75}), 2: (1, {'@': 75}), 3: (1, {'@': 75}), 4: (1, {'@': 75}), 5: (1, {'@': 75}), 6: (1, {'@': 75}), 7: (1, {'@': 75}), 8: (1, {'@': 75}), 9: (1, {'@': 75})}, 59: {0: (0, 52), 2: (1, {'@': 53}), 4: (1, {'@': 53}), 1: (1, {'@': 53}), 9: (1, {'@': 53}), 8: (1, {'@': 53})}, 60: {5: (0, 42), 38: (0, 44), 6: (0, 1), 3: (0, 56), 7: (0, 66), 10: (0, 11), 0: (1, {'@': 52}), 2: (1, {'@': 52}), 4: (1, {'@': 52}), 1: (1, {'@': 52}), 8: (1, {'@': 52}), 9: (1, {'@': 52})}, 61: {15: (0, 41), 16: (0, 49), 12: (0, 18), 17: (0, 71), 13: (0, 26), 8: (0, 30), 18: (0, 63), 19: (0, 60), 20: (0, 36), 21: (0, 40), 22: (0, 54), 37: (0, 67), 23: (0, 27), 24: (0, 53), 25: (0, 2), 26: (0, 24), 27: (0, 68), 28: (0, 39), 29: (0, 7), 30: (0, 32), 32: (0, 70), 33: (0, 20), 34: (0, 0), 35: (0, 3), 36: (0, 69), 9: (1, {'@': 35})}, 62: {0: (1, {'@': 59}), 2: (1, {'@': 59}), 3: (1, {'@': 59}), 5: (1, {'@': 59}), 8: (1, {'@': 59}), 7: (1, {'@': 59}), 9: (1, {'@': 59}), 4: (1, {'@': 59}), 6: (1, {'@': 59}), 14: (1, {'@': 59}), 1: (1, {'@': 59})}, 63: {0: (1, {'@': 56}), 2: (1, {'@': 56}), 4: (1, {'@': 56}), 1: (1, {'@': 56}), 8: (1, {'@': 56}), 9: (1, {'@': 56})}, 64: {14: (1, {'@': 60}), 3: (1, {'@': 60}), 5: (1, {'@': 60}), 6: (1, {'@': 60}), 0: (1, {'@': 60}), 2: (1, {'@': 60}), 4: (1, {'@': 60}), 8: (1, {'@': 60}), 1: (1, {'@': 60}), 9: (1, {'@': 60}), 7: (1, {'@': 60})}, 65: {9: (0, 62)}, 66: {24: (0, 53), 15: (0, 41), 25: (0, 2), 26: (0, 24), 27: (0, 68), 16: (0, 49), 12: (0, 18), 28: (0, 39), 19: (0, 37), 17: (0, 71), 29: (0, 7), 13: (0, 26), 32: (0, 70), 33: (0, 20), 34: (0, 0), 20: (0, 36), 21: (0, 40), 35: (0, 3), 36: (0, 69), 23: (0, 27)}, 67: {8: (0, 34), 9: (1, {'@': 34})}, 68: {0: (1, {'@': 47}), 1: (1, {'@': 47}), 2: (1, {'@': 47}), 3: (1, {'@': 47}), 4: (1, {'@': 47}), 5: (1, {'@': 47}), 6: (1, {'@': 47}), 7: (1, {'@': 47}), 8: (1, {'@': 47}), 9: (1, {'@': 47}), 14: (1, {'@': 47})}, 69: {0: (1, {'@': 42}), 1: (1, {'@': 42}), 2: (1, {'@': 42}), 3: (1, {'@': 42}), 4: (1, {'@': 42}), 5: (1, {'@': 42}), 6: (1, {'@': 42}), 7: (1, {'@': 42}), 8: (1, {'@': 42}), 9: (1, {'@': 42})}, 70: {24: (0, 53), 15: (0, 41), 25: (0, 2), 26: (0, 24), 37: (0, 38), 27: (0, 68), 16: (0, 49), 12: (0, 18), 28: (0, 39), 17: (0, 71), 29: (0, 7), 19: (0, 60), 13: (0, 26), 18: (0, 63), 30: (0, 32), 32: (0, 70), 33: (0, 20), 34: (0, 0), 20: (0, 36), 21: (0, 40), 35: (0, 3), 36: (0, 69), 22: (0, 54), 23: (0, 27)}, 71: {0: (1, {'@': 39}), 1: (1, {'@': 39}), 2: (1, {'@': 39}), 3: (1, {'@': 39}), 4: (1, {'@': 39}), 5: (1, {'@': 39}), 6: (1, {'@': 39}), 7: (1, {'@': 39}), 8: (1, {'@': 39}), 9: (1, {'@': 39})}}, 'start_states': {'start': 35}, 'end_states': {'start': 13}}, 'options': {'debug': False, 'keep_all_tokens': False, 'tree_class': None, 'cache': False, 'postlex': None, 'parser': 'lalr', 'lexer': 'contextual', 'transformer': None, 'start': ['start'], 'priority': 'normal', 'ambiguity': 'auto', 'regex': False, 'propagate_positions': False, 'lexer_callbacks': {}, 'maybe_placeholders': True, 'edit_terminals': None, 'g_regex_flags': 0, 'use_bytes': False, 'import_paths': [], 'source_path': None}, '__type__': 'ParsingFrontend'}, 'rules': [{'@': 22}, {'@': 23}, {'@': 24}, {'@': 25}, {'@': 26}, {'@': 27}, {'@': 28}, {'@': 29}, {'@': 30}, {'@': 31}, {'@': 32}, {'@': 33}, {'@': 34}, {'@': 35}, {'@': 36}, {'@': 37}, {'@': 38}, {'@': 39}, {'@': 40}, {'@': 41}, {'@': 42}, {'@': 43}, {'@': 44}, {'@': 45}, {'@': 46}, {'@': 47}, {'@': 48}, {'@': 49}, {'@': 50}, {'@': 51}, {'@': 52}, {'@': 53}, {'@': 54}, {'@': 55}, {'@': 56}, {'@': 57}, {'@': 58}, {'@': 59}, {'@': 60}, {'@': 61}, {'@': 62}, {'@': 63}, {'@': 64}, {'@': 65}, {'@': 66}, {'@': 67}, {'@': 68}, {'@': 69}, {'@': 70}, {'@': 71}, {'@': 72}, {'@': 73}, {'@': 74}, {'@': 75}, {'@': 76}], 'options': {'debug': False, 'keep_all_tokens': False, 'tree_class': None, 'cache': False, 'postlex': None, 'parser': 'lalr', 'lexer': 'contextual', 'transformer': None, 'start': ['start'], 'priority': 'normal', 'ambiguity': 'auto', 'regex': False, 'propagate_positions': False, 'lexer_callbacks': {}, 'maybe_placeholders': True, 'edit_terminals': None, 'g_regex_flags': 0, 'use_bytes': False, 'import_paths': [], 'source_path': None}, '__type__': 'Lark'}
+{'parser': {'lexer_conf': {'terminals': [{'@': 0}, {'@': 1}, {'@': 2}, {'@': 3}, {'@': 4}, {'@': 5}, {'@': 6}, {'@': 7}, {'@': 8}, {'@': 9}, {'@': 10}, {'@': 11}, {'@': 12}, {'@': 13}, {'@': 14}, {'@': 15}, {'@': 16}, {'@': 17}, {'@': 18}, {'@': 19}, {'@': 20}, {'@': 21}], 'ignore': ['WS_INLINE'], 'g_regex_flags': 0, 'use_bytes': False, 'lexer_type': 'contextual', '__type__': 'LexerConf'}, 'parser_conf': {'rules': [{'@': 22}, {'@': 23}, {'@': 24}, {'@': 25}, {'@': 26}, {'@': 27}, {'@': 28}, {'@': 29}, {'@': 30}, {'@': 31}, {'@': 32}, {'@': 33}, {'@': 34}, {'@': 35}, {'@': 36}, {'@': 37}, {'@': 38}, {'@': 39}, {'@': 40}, {'@': 41}, {'@': 42}, {'@': 43}, {'@': 44}, {'@': 45}, {'@': 46}, {'@': 47}, {'@': 48}, {'@': 49}, {'@': 50}, {'@': 51}, {'@': 52}, {'@': 53}, {'@': 54}, {'@': 55}, {'@': 56}, {'@': 57}, {'@': 58}, {'@': 59}, {'@': 60}, {'@': 61}, {'@': 62}, {'@': 63}, {'@': 64}, {'@': 65}, {'@': 66}, {'@': 67}, {'@': 68}, {'@': 69}, {'@': 70}, {'@': 71}, {'@': 72}, {'@': 73}, {'@': 74}, {'@': 75}, {'@': 76}], 'start': ['start'], 'parser_type': 'lalr', '__type__': 'ParserConf'}, 'parser': {'tokens': {0: 'RSQB', 1: 'RPAR', 2: 'AND', 3: 'OR', 4: 'COLON', 5: 'COMMA', 6: 'DOT', 7: 'COMPARE_OPERATOR', 8: 'LSQB', 9: 'DOUBLE_DOT', 10: '$END', 11: 'atom', 12: 'FALSE', 13: 'path_with_action', 14: 'test_comparison', 15: 'STRING', 16: 'null', 17: 'CNAME', 18: 'value', 19: 'NULL', 20: 'first_path', 21: 'path', 22: 'LPAR', 23: 'self', 24: 'func_call', 25: 'false', 26: 'DOLLAR', 27: 'TRUE', 28: 'true', 29: 'NUMBER', 30: 'root', 31: 'AT', 32: 'action_separate_with_dot', 33: 'predicate', 34: 'test_and', 35: 'test', 36: 'expr', 37: 'args', 38: 'identifier', 39: 'start', 40: '__ANON_0', 41: 'STAR', 42: 'slice'}, 'states': {0: {0: (1, {'@': 28})}, 1: {1: (0, 20)}, 2: {2: (0, 6), 3: (1, {'@': 54}), 4: (1, {'@': 54}), 0: (1, {'@': 54}), 1: (1, {'@': 54}), 5: (1, {'@': 54})}, 3: {6: (1, {'@': 70}), 7: (1, {'@': 70}), 2: (1, {'@': 70}), 5: (1, {'@': 70}), 8: (1, {'@': 70}), 4: (1, {'@': 70}), 3: (1, {'@': 70}), 1: (1, {'@': 70}), 0: (1, {'@': 70}), 9: (1, {'@': 70}), 10: (1, {'@': 70})}, 4: {5: (1, {'@': 68}), 1: (1, {'@': 68})}, 5: {6: (1, {'@': 73}), 8: (1, {'@': 73}), 9: (1, {'@': 73}), 10: (1, {'@': 22})}, 6: {11: (0, 36), 12: (0, 68), 13: (0, 32), 14: (0, 27), 15: (0, 57), 16: (0, 71), 17: (0, 47), 18: (0, 60), 19: (0, 7), 20: (0, 61), 21: (0, 42), 22: (0, 13), 23: (0, 25), 24: (0, 30), 25: (0, 49), 26: (0, 19), 27: (0, 62), 28: (0, 70), 29: (0, 33), 30: (0, 8), 31: (0, 29)}, 7: {6: (1, {'@': 38}), 7: (1, {'@': 38}), 2: (1, {'@': 38}), 5: (1, {'@': 38}), 8: (1, {'@': 38}), 4: (1, {'@': 38}), 3: (1, {'@': 38}), 1: (1, {'@': 38}), 0: (1, {'@': 38}), 9: (1, {'@': 38})}, 8: {6: (1, {'@': 50}), 7: (1, {'@': 50}), 2: (1, {'@': 50}), 5: (1, {'@': 50}), 8: (1, {'@': 50}), 4: (1, {'@': 50}), 3: (1, {'@': 50}), 1: (1, {'@': 50}), 0: (1, {'@': 50}), 9: (1, {'@': 50}), 10: (1, {'@': 50})}, 9: {9: (0, 22), 6: (0, 48), 8: (0, 64), 32: (0, 34), 33: (0, 66), 2: (1, {'@': 51}), 5: (1, {'@': 51}), 3: (1, {'@': 51}), 1: (1, {'@': 51}), 0: (1, {'@': 51}), 4: (1, {'@': 51})}, 10: {34: (0, 2), 4: (0, 50), 35: (0, 40), 17: (0, 47), 20: (0, 61), 23: (0, 25), 36: (0, 65), 24: (0, 30), 25: (0, 49), 27: (0, 62), 28: (0, 70), 11: (0, 36), 30: (0, 8), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 18: (0, 60), 19: (0, 7), 14: (0, 55), 21: (0, 42), 22: (0, 13), 26: (0, 19), 29: (0, 33), 31: (0, 29), 0: (1, {'@': 35})}, 11: {4: (0, 69), 0: (0, 58)}, 12: {34: (0, 2), 36: (0, 0), 35: (0, 40), 17: (0, 47), 20: (0, 61), 23: (0, 25), 24: (0, 30), 25: (0, 49), 27: (0, 62), 28: (0, 70), 11: (0, 36), 30: (0, 8), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 18: (0, 60), 19: (0, 7), 14: (0, 55), 21: (0, 42), 22: (0, 13), 26: (0, 19), 29: (0, 33), 31: (0, 29), 0: (1, {'@': 29})}, 13: {34: (0, 2), 11: (0, 36), 12: (0, 68), 35: (0, 40), 13: (0, 32), 15: (0, 57), 16: (0, 71), 17: (0, 47), 18: (0, 60), 19: (0, 7), 14: (0, 55), 20: (0, 61), 21: (0, 42), 22: (0, 13), 23: (0, 25), 24: (0, 30), 25: (0, 49), 26: (0, 19), 27: (0, 62), 36: (0, 1), 28: (0, 70), 29: (0, 33), 30: (0, 8), 31: (0, 29)}, 14: {}, 15: {34: (0, 2), 35: (0, 40), 17: (0, 47), 37: (0, 35), 20: (0, 61), 23: (0, 25), 24: (0, 30), 25: (0, 49), 36: (0, 56), 27: (0, 62), 28: (0, 70), 11: (0, 36), 30: (0, 8), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 18: (0, 60), 19: (0, 7), 14: (0, 55), 21: (0, 42), 22: (0, 13), 26: (0, 19), 29: (0, 33), 31: (0, 29)}, 16: {0: (1, {'@': 26})}, 17: {3: (1, {'@': 45}), 4: (1, {'@': 45}), 9: (1, {'@': 45}), 6: (1, {'@': 45}), 7: (1, {'@': 45}), 2: (1, {'@': 45}), 5: (1, {'@': 45}), 8: (1, {'@': 45}), 10: (1, {'@': 45}), 1: (1, {'@': 45}), 0: (1, {'@': 45})}, 18: {0: (1, {'@': 30})}, 19: {6: (1, {'@': 47}), 7: (1, {'@': 47}), 2: (1, {'@': 47}), 5: (1, {'@': 47}), 8: (1, {'@': 47}), 4: (1, {'@': 47}), 3: (1, {'@': 47}), 1: (1, {'@': 47}), 0: (1, {'@': 47}), 9: (1, {'@': 47}), 10: (1, {'@': 47})}, 20: {6: (1, {'@': 75}), 7: (1, {'@': 75}), 2: (1, {'@': 75}), 5: (1, {'@': 75}), 8: (1, {'@': 75}), 4: (1, {'@': 75}), 3: (1, {'@': 75}), 1: (1, {'@': 75}), 0: (1, {'@': 75}), 9: (1, {'@': 75})}, 21: {34: (0, 2), 11: (0, 36), 36: (0, 4), 12: (0, 68), 35: (0, 40), 13: (0, 32), 15: (0, 57), 16: (0, 71), 17: (0, 47), 18: (0, 60), 19: (0, 7), 14: (0, 55), 20: (0, 61), 21: (0, 42), 22: (0, 13), 23: (0, 25), 24: (0, 30), 25: (0, 49), 26: (0, 19), 27: (0, 62), 28: (0, 70), 29: (0, 33), 30: (0, 8), 31: (0, 29)}, 22: {15: (0, 17), 8: (0, 64), 33: (0, 54), 17: (0, 26), 38: (0, 67)}, 23: {6: (1, {'@': 59}), 2: (1, {'@': 59}), 5: (1, {'@': 59}), 8: (1, {'@': 59}), 4: (1, {'@': 59}), 3: (1, {'@': 59}), 1: (1, {'@': 59}), 0: (1, {'@': 59}), 9: (1, {'@': 59}), 7: (1, {'@': 59}), 10: (1, {'@': 59})}, 24: {9: (0, 22), 6: (0, 48), 8: (0, 64), 32: (0, 34), 33: (0, 66)}, 25: {6: (1, {'@': 49}), 7: (1, {'@': 49}), 2: (1, {'@': 49}), 5: (1, {'@': 49}), 8: (1, {'@': 49}), 4: (1, {'@': 49}), 3: (1, {'@': 49}), 1: (1, {'@': 49}), 0: (1, {'@': 49}), 9: (1, {'@': 49}), 10: (1, {'@': 49})}, 26: {3: (1, {'@': 44}), 4: (1, {'@': 44}), 9: (1, {'@': 44}), 6: (1, {'@': 44}), 7: (1, {'@': 44}), 2: (1, {'@': 44}), 5: (1, {'@': 44}), 8: (1, {'@': 44}), 10: (1, {'@': 44}), 1: (1, {'@': 44}), 0: (1, {'@': 44})}, 27: {3: (1, {'@': 55}), 4: (1, {'@': 55}), 0: (1, {'@': 55}), 2: (1, {'@': 55}), 1: (1, {'@': 55}), 5: (1, {'@': 55})}, 28: {11: (0, 24), 39: (0, 14), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 21: (0, 5), 17: (0, 47), 18: (0, 60), 24: (0, 52), 19: (0, 7), 20: (0, 61), 22: (0, 13), 23: (0, 25), 25: (0, 49), 26: (0, 19), 27: (0, 62), 28: (0, 70), 29: (0, 33), 30: (0, 8), 31: (0, 29)}, 29: {6: (1, {'@': 46}), 7: (1, {'@': 46}), 2: (1, {'@': 46}), 5: (1, {'@': 46}), 8: (1, {'@': 46}), 4: (1, {'@': 46}), 3: (1, {'@': 46}), 1: (1, {'@': 46}), 0: (1, {'@': 46}), 9: (1, {'@': 46}), 10: (1, {'@': 46})}, 30: {6: (1, {'@': 74}), 7: (1, {'@': 74}), 2: (1, {'@': 74}), 5: (1, {'@': 74}), 8: (1, {'@': 74}), 4: (1, {'@': 74}), 3: (1, {'@': 74}), 1: (1, {'@': 74}), 0: (1, {'@': 74}), 9: (1, {'@': 74})}, 31: {2: (0, 6), 3: (1, {'@': 53}), 4: (1, {'@': 53}), 0: (1, {'@': 53}), 1: (1, {'@': 53}), 5: (1, {'@': 53})}, 32: {6: (1, {'@': 66}), 7: (1, {'@': 66}), 2: (1, {'@': 66}), 5: (1, {'@': 66}), 8: (1, {'@': 66}), 4: (1, {'@': 66}), 3: (1, {'@': 66}), 1: (1, {'@': 66}), 0: (1, {'@': 66}), 9: (1, {'@': 66}), 10: (1, {'@': 66})}, 33: {6: (1, {'@': 39}), 7: (1, {'@': 39}), 2: (1, {'@': 39}), 5: (1, {'@': 39}), 8: (1, {'@': 39}), 4: (1, {'@': 39}), 3: (1, {'@': 39}), 1: (1, {'@': 39}), 0: (1, {'@': 39}), 9: (1, {'@': 39})}, 34: {6: (1, {'@': 64}), 7: (1, {'@': 64}), 2: (1, {'@': 64}), 5: (1, {'@': 64}), 8: (1, {'@': 64}), 4: (1, {'@': 64}), 3: (1, {'@': 64}), 1: (1, {'@': 64}), 0: (1, {'@': 64}), 9: (1, {'@': 64}), 10: (1, {'@': 64})}, 35: {5: (0, 21), 1: (0, 3)}, 36: {9: (0, 22), 6: (0, 48), 8: (0, 64), 32: (0, 34), 33: (0, 66), 7: (0, 37), 2: (1, {'@': 52}), 5: (1, {'@': 52}), 3: (1, {'@': 52}), 1: (1, {'@': 52}), 0: (1, {'@': 52}), 4: (1, {'@': 52})}, 37: {11: (0, 9), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 17: (0, 47), 18: (0, 60), 19: (0, 7), 20: (0, 61), 21: (0, 42), 22: (0, 13), 23: (0, 25), 24: (0, 30), 25: (0, 49), 26: (0, 19), 27: (0, 62), 28: (0, 70), 29: (0, 33), 30: (0, 8), 31: (0, 29)}, 38: {34: (0, 2), 35: (0, 40), 17: (0, 47), 20: (0, 61), 23: (0, 25), 36: (0, 16), 24: (0, 30), 25: (0, 49), 27: (0, 62), 28: (0, 70), 11: (0, 36), 30: (0, 8), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 18: (0, 60), 19: (0, 7), 14: (0, 55), 21: (0, 42), 22: (0, 13), 26: (0, 19), 29: (0, 33), 31: (0, 29), 0: (1, {'@': 27})}, 39: {34: (0, 2), 35: (0, 40), 17: (0, 47), 20: (0, 61), 23: (0, 25), 24: (0, 30), 25: (0, 49), 27: (0, 62), 28: (0, 70), 11: (0, 36), 30: (0, 8), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 18: (0, 60), 19: (0, 7), 14: (0, 55), 21: (0, 42), 22: (0, 13), 36: (0, 51), 26: (0, 19), 29: (0, 33), 31: (0, 29), 0: (1, {'@': 25})}, 40: {3: (0, 46), 4: (1, {'@': 76}), 0: (1, {'@': 76}), 1: (1, {'@': 76}), 5: (1, {'@': 76})}, 41: {4: (0, 39), 0: (1, {'@': 32})}, 42: {6: (1, {'@': 73}), 7: (1, {'@': 73}), 2: (1, {'@': 73}), 5: (1, {'@': 73}), 8: (1, {'@': 73}), 4: (1, {'@': 73}), 3: (1, {'@': 73}), 1: (1, {'@': 73}), 0: (1, {'@': 73}), 9: (1, {'@': 73})}, 43: {0: (0, 23)}, 44: {6: (1, {'@': 63}), 2: (1, {'@': 63}), 5: (1, {'@': 63}), 8: (1, {'@': 63}), 4: (1, {'@': 63}), 3: (1, {'@': 63}), 1: (1, {'@': 63}), 0: (1, {'@': 63}), 9: (1, {'@': 63}), 10: (1, {'@': 63}), 7: (1, {'@': 63})}, 45: {0: (0, 59)}, 46: {11: (0, 36), 34: (0, 31), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 17: (0, 47), 18: (0, 60), 19: (0, 7), 14: (0, 55), 20: (0, 61), 21: (0, 42), 22: (0, 13), 23: (0, 25), 24: (0, 30), 25: (0, 49), 26: (0, 19), 27: (0, 62), 28: (0, 70), 29: (0, 33), 30: (0, 8), 31: (0, 29)}, 47: {40: (0, 53), 22: (0, 15), 6: (1, {'@': 48}), 7: (1, {'@': 48}), 2: (1, {'@': 48}), 5: (1, {'@': 48}), 8: (1, {'@': 48}), 4: (1, {'@': 48}), 3: (1, {'@': 48}), 1: (1, {'@': 48}), 0: (1, {'@': 48}), 9: (1, {'@': 48}), 10: (1, {'@': 48})}, 48: {41: (0, 44), 15: (0, 17), 38: (0, 63), 17: (0, 26)}, 49: {6: (1, {'@': 41}), 7: (1, {'@': 41}), 2: (1, {'@': 41}), 5: (1, {'@': 41}), 8: (1, {'@': 41}), 4: (1, {'@': 41}), 3: (1, {'@': 41}), 1: (1, {'@': 41}), 0: (1, {'@': 41}), 9: (1, {'@': 41})}, 50: {34: (0, 2), 35: (0, 40), 17: (0, 47), 20: (0, 61), 23: (0, 25), 24: (0, 30), 25: (0, 49), 27: (0, 62), 28: (0, 70), 11: (0, 36), 30: (0, 8), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 36: (0, 18), 18: (0, 60), 19: (0, 7), 14: (0, 55), 21: (0, 42), 22: (0, 13), 26: (0, 19), 29: (0, 33), 31: (0, 29), 0: (1, {'@': 31})}, 51: {0: (1, {'@': 24})}, 52: {6: (1, {'@': 74}), 8: (1, {'@': 74}), 9: (1, {'@': 74}), 10: (1, {'@': 23})}, 53: {6: (1, {'@': 71}), 7: (1, {'@': 71}), 2: (1, {'@': 71}), 5: (1, {'@': 71}), 8: (1, {'@': 71}), 4: (1, {'@': 71}), 3: (1, {'@': 71}), 1: (1, {'@': 71}), 0: (1, {'@': 71}), 9: (1, {'@': 71}), 10: (1, {'@': 71})}, 54: {6: (1, {'@': 60}), 2: (1, {'@': 60}), 5: (1, {'@': 60}), 8: (1, {'@': 60}), 4: (1, {'@': 60}), 3: (1, {'@': 60}), 1: (1, {'@': 60}), 0: (1, {'@': 60}), 9: (1, {'@': 60}), 10: (1, {'@': 60}), 7: (1, {'@': 60})}, 55: {3: (1, {'@': 56}), 4: (1, {'@': 56}), 0: (1, {'@': 56}), 2: (1, {'@': 56}), 1: (1, {'@': 56}), 5: (1, {'@': 56})}, 56: {5: (1, {'@': 69}), 1: (1, {'@': 69})}, 57: {6: (1, {'@': 43}), 7: (1, {'@': 43}), 2: (1, {'@': 43}), 5: (1, {'@': 43}), 8: (1, {'@': 43}), 4: (1, {'@': 43}), 3: (1, {'@': 43}), 1: (1, {'@': 43}), 0: (1, {'@': 43}), 9: (1, {'@': 43})}, 58: {6: (1, {'@': 57}), 2: (1, {'@': 57}), 5: (1, {'@': 57}), 8: (1, {'@': 57}), 4: (1, {'@': 57}), 3: (1, {'@': 57}), 1: (1, {'@': 57}), 0: (1, {'@': 57}), 9: (1, {'@': 57}), 7: (1, {'@': 57}), 10: (1, {'@': 57})}, 59: {6: (1, {'@': 58}), 2: (1, {'@': 58}), 5: (1, {'@': 58}), 8: (1, {'@': 58}), 4: (1, {'@': 58}), 3: (1, {'@': 58}), 1: (1, {'@': 58}), 0: (1, {'@': 58}), 9: (1, {'@': 58}), 7: (1, {'@': 58}), 10: (1, {'@': 58})}, 60: {6: (1, {'@': 72}), 7: (1, {'@': 72}), 2: (1, {'@': 72}), 5: (1, {'@': 72}), 8: (1, {'@': 72}), 4: (1, {'@': 72}), 3: (1, {'@': 72}), 1: (1, {'@': 72}), 0: (1, {'@': 72}), 9: (1, {'@': 72})}, 61: {6: (1, {'@': 67}), 7: (1, {'@': 67}), 2: (1, {'@': 67}), 5: (1, {'@': 67}), 8: (1, {'@': 67}), 4: (1, {'@': 67}), 3: (1, {'@': 67}), 1: (1, {'@': 67}), 0: (1, {'@': 67}), 9: (1, {'@': 67}), 10: (1, {'@': 67})}, 62: {6: (1, {'@': 36}), 7: (1, {'@': 36}), 2: (1, {'@': 36}), 5: (1, {'@': 36}), 8: (1, {'@': 36}), 4: (1, {'@': 36}), 3: (1, {'@': 36}), 1: (1, {'@': 36}), 0: (1, {'@': 36}), 9: (1, {'@': 36})}, 63: {6: (1, {'@': 62}), 2: (1, {'@': 62}), 5: (1, {'@': 62}), 8: (1, {'@': 62}), 4: (1, {'@': 62}), 3: (1, {'@': 62}), 1: (1, {'@': 62}), 0: (1, {'@': 62}), 9: (1, {'@': 62}), 10: (1, {'@': 62}), 7: (1, {'@': 62})}, 64: {34: (0, 2), 4: (0, 10), 35: (0, 40), 36: (0, 11), 17: (0, 47), 20: (0, 61), 23: (0, 25), 24: (0, 30), 25: (0, 49), 27: (0, 62), 28: (0, 70), 11: (0, 36), 30: (0, 8), 41: (0, 43), 12: (0, 68), 13: (0, 32), 42: (0, 45), 15: (0, 57), 16: (0, 71), 18: (0, 60), 19: (0, 7), 14: (0, 55), 21: (0, 42), 22: (0, 13), 26: (0, 19), 29: (0, 33), 31: (0, 29)}, 65: {4: (0, 12), 0: (1, {'@': 34})}, 66: {6: (1, {'@': 65}), 7: (1, {'@': 65}), 2: (1, {'@': 65}), 5: (1, {'@': 65}), 8: (1, {'@': 65}), 4: (1, {'@': 65}), 3: (1, {'@': 65}), 1: (1, {'@': 65}), 0: (1, {'@': 65}), 9: (1, {'@': 65}), 10: (1, {'@': 65})}, 67: {6: (1, {'@': 61}), 2: (1, {'@': 61}), 5: (1, {'@': 61}), 8: (1, {'@': 61}), 4: (1, {'@': 61}), 3: (1, {'@': 61}), 1: (1, {'@': 61}), 0: (1, {'@': 61}), 9: (1, {'@': 61}), 10: (1, {'@': 61}), 7: (1, {'@': 61})}, 68: {6: (1, {'@': 37}), 7: (1, {'@': 37}), 2: (1, {'@': 37}), 5: (1, {'@': 37}), 8: (1, {'@': 37}), 4: (1, {'@': 37}), 3: (1, {'@': 37}), 1: (1, {'@': 37}), 0: (1, {'@': 37}), 9: (1, {'@': 37})}, 69: {34: (0, 2), 4: (0, 38), 35: (0, 40), 17: (0, 47), 36: (0, 41), 20: (0, 61), 23: (0, 25), 24: (0, 30), 25: (0, 49), 27: (0, 62), 28: (0, 70), 11: (0, 36), 30: (0, 8), 12: (0, 68), 13: (0, 32), 15: (0, 57), 16: (0, 71), 18: (0, 60), 19: (0, 7), 14: (0, 55), 21: (0, 42), 22: (0, 13), 26: (0, 19), 29: (0, 33), 31: (0, 29), 0: (1, {'@': 33})}, 70: {6: (1, {'@': 40}), 7: (1, {'@': 40}), 2: (1, {'@': 40}), 5: (1, {'@': 40}), 8: (1, {'@': 40}), 4: (1, {'@': 40}), 3: (1, {'@': 40}), 1: (1, {'@': 40}), 0: (1, {'@': 40}), 9: (1, {'@': 40})}, 71: {6: (1, {'@': 42}), 7: (1, {'@': 42}), 2: (1, {'@': 42}), 5: (1, {'@': 42}), 8: (1, {'@': 42}), 4: (1, {'@': 42}), 3: (1, {'@': 42}), 1: (1, {'@': 42}), 0: (1, {'@': 42}), 9: (1, {'@': 42})}}, 'start_states': {'start': 28}, 'end_states': {'start': 14}}, '__type__': 'ParsingFrontend'}, 'rules': [{'@': 22}, {'@': 23}, {'@': 24}, {'@': 25}, {'@': 26}, {'@': 27}, {'@': 28}, {'@': 29}, {'@': 30}, {'@': 31}, {'@': 32}, {'@': 33}, {'@': 34}, {'@': 35}, {'@': 36}, {'@': 37}, {'@': 38}, {'@': 39}, {'@': 40}, {'@': 41}, {'@': 42}, {'@': 43}, {'@': 44}, {'@': 45}, {'@': 46}, {'@': 47}, {'@': 48}, {'@': 49}, {'@': 50}, {'@': 51}, {'@': 52}, {'@': 53}, {'@': 54}, {'@': 55}, {'@': 56}, {'@': 57}, {'@': 58}, {'@': 59}, {'@': 60}, {'@': 61}, {'@': 62}, {'@': 63}, {'@': 64}, {'@': 65}, {'@': 66}, {'@': 67}, {'@': 68}, {'@': 69}, {'@': 70}, {'@': 71}, {'@': 72}, {'@': 73}, {'@': 74}, {'@': 75}, {'@': 76}], 'options': {'debug': False, 'keep_all_tokens': False, 'tree_class': None, 'cache': False, 'postlex': None, 'parser': 'lalr', 'lexer': 'contextual', 'transformer': None, 'start': ['start'], 'priority': 'normal', 'ambiguity': 'auto', 'regex': False, 'propagate_positions': False, 'lexer_callbacks': {}, 'maybe_placeholders': True, 'edit_terminals': None, 'g_regex_flags': 0, 'use_bytes': False, 'import_paths': [], 'source_path': None, '_plugins': {}}, '__type__': 'Lark'}
 )
 MEMO = (
-{0: {'name': 'NUMBER', 'pattern': {'value': '(?:(?:\\+|\\-))?(?:(?:(?:[0-9])+(?:e|E)(?:(?:\\+|\\-))?(?:[0-9])+|(?:(?:[0-9])+\\.(?:(?:[0-9])+)?|\\.(?:[0-9])+)(?:(?:e|E)(?:(?:\\+|\\-))?(?:[0-9])+)?)|(?:[0-9])+)', 'flags': [], '_width': [1, 4294967295], '__type__': 'PatternRE'}, 'priority': 1, '__type__': 'TerminalDef'}, 1: {'name': 'CNAME', 'pattern': {'value': '(?:_|(?:[A-Z]|[a-z]))(?:(?:(?:_|(?:[A-Z]|[a-z]))|[0-9]))*', 'flags': [], '_width': [1, 4294967295], '__type__': 'PatternRE'}, 'priority': 1, '__type__': 'TerminalDef'}, 2: {'name': 'WS_INLINE', 'pattern': {'value': '(?:(?:\\ |\t))+', 'flags': [], '_width': [1, 4294967295], '__type__': 'PatternRE'}, 'priority': 1, '__type__': 'TerminalDef'}, 3: {'name': 'COLON', 'pattern': {'value': ':', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 4: {'name': 'STRING', 'pattern': {'value': '`([^`\\\\]|\\\\.)*?`|\'([^\'\\\\]|\\\\.)*?\'|"([^"\\\\]|\\\\.)*?"', 'flags': ['i'], '_width': [2, 4294967295], '__type__': 'PatternRE'}, 'priority': 1, '__type__': 'TerminalDef'}, 5: {'name': 'STAR', 'pattern': {'value': '*', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 6: {'name': 'DOT', 'pattern': {'value': '.', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 7: {'name': 'DOUBLE_DOT', 'pattern': {'value': '..', 'flags': [], '__type__': 'PatternStr'}, 'priority': 2, '__type__': 'TerminalDef'}, 8: {'name': 'COMPARE_OPERATOR', 'pattern': {'value': '(?:(?:(?:(?:(?:<=|>=)|<)|>)|!=)|=)', 'flags': [], '_width': [1, 2], '__type__': 'PatternRE'}, 'priority': 1, '__type__': 'TerminalDef'}, 9: {'name': 'AND', 'pattern': {'value': 'and', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 10: {'name': 'OR', 'pattern': {'value': 'or', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 11: {'name': 'TRUE', 'pattern': {'value': 'true', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 12: {'name': 'FALSE', 'pattern': {'value': 'false', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 13: {'name': 'NULL', 'pattern': {'value': 'null', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 14: {'name': 'AT', 'pattern': {'value': '@', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 15: {'name': 'DOLLAR', 'pattern': {'value': '$', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 16: {'name': 'LSQB', 'pattern': {'value': '[', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 17: {'name': 'RSQB', 'pattern': {'value': ']', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 18: {'name': 'COMMA', 'pattern': {'value': ',', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 19: {'name': 'LPAR', 'pattern': {'value': '(', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 20: {'name': 'RPAR', 'pattern': {'value': ')', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 21: {'name': '__ANON_0', 'pattern': {'value': '()', 'flags': [], '__type__': 'PatternStr'}, 'priority': 1, '__type__': 'TerminalDef'}, 22: {'origin': {'name': 'start', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'path', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 23: {'origin': {'name': 'start', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'funccall', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 24: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 25: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 1, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [False, False, False, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 26: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 2, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [False, False, True, False, False], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 27: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 3, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [False, False, True, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 28: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 4, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, False, False, False], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 29: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 5, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, False, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 30: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 6, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, True, False, False], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 31: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 7, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, True, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 32: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 8, 'alias': 'two_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 33: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 9, 'alias': 'two_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [False, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 34: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 10, 'alias': 'two_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, False], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 35: {'origin': {'name': 'slice', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 11, 'alias': 'two_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 36: {'origin': {'name': 'true', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'TRUE', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 37: {'origin': {'name': 'false', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'FALSE', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 38: {'origin': {'name': 'null', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'NULL', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 39: {'origin': {'name': 'value', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'NUMBER', 'filter_out': False, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 40: {'origin': {'name': 'value', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'true', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 41: {'origin': {'name': 'value', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'false', '__type__': 'NonTerminal'}], 'order': 2, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 42: {'origin': {'name': 'value', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'null', '__type__': 'NonTerminal'}], 'order': 3, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 43: {'origin': {'name': 'value', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'STRING', 'filter_out': False, '__type__': 'Terminal'}], 'order': 4, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 44: {'origin': {'name': 'identifier', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'CNAME', 'filter_out': False, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 45: {'origin': {'name': 'identifier', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'STRING', 'filter_out': False, '__type__': 'Terminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 46: {'origin': {'name': 'self', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'AT', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 47: {'origin': {'name': 'root', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOLLAR', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 48: {'origin': {'name': 'first_path', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'CNAME', 'filter_out': False, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 49: {'origin': {'name': 'first_path', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'self', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 50: {'origin': {'name': 'first_path', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'root', '__type__': 'NonTerminal'}], 'order': 2, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 51: {'origin': {'name': 'test_comparison', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'atom', '__type__': 'NonTerminal'}, {'name': 'COMPARE_OPERATOR', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'atom', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'comparison_expr', 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 52: {'origin': {'name': 'test_comparison', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'atom', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 53: {'origin': {'name': 'test', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test', '__type__': 'NonTerminal'}, {'name': 'OR', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'test_and', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'or_expr', 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 54: {'origin': {'name': 'test', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test_and', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 55: {'origin': {'name': 'test_and', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test_and', '__type__': 'NonTerminal'}, {'name': 'AND', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'test_comparison', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'and_expr', 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 56: {'origin': {'name': 'test_and', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test_comparison', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 57: {'origin': {'name': 'predicate', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'LSQB', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'RSQB', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 58: {'origin': {'name': 'predicate', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'LSQB', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'slice', '__type__': 'NonTerminal'}, {'name': 'RSQB', 'filter_out': True, '__type__': 'Terminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 59: {'origin': {'name': 'predicate', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'LSQB', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'STAR', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'RSQB', 'filter_out': True, '__type__': 'Terminal'}], 'order': 2, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 60: {'origin': {'name': 'action_separate_with_dot', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOUBLE_DOT', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'predicate', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'search_with_predicate', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 61: {'origin': {'name': 'action_separate_with_dot', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOUBLE_DOT', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'identifier', '__type__': 'NonTerminal'}], 'order': 1, 'alias': 'search_with_identifier', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 62: {'origin': {'name': 'action_separate_with_dot', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOT', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'identifier', '__type__': 'NonTerminal'}], 'order': 2, 'alias': 'chain_with_identifier', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 63: {'origin': {'name': 'action_separate_with_dot', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOT', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'STAR', 'filter_out': False, '__type__': 'Terminal'}], 'order': 3, 'alias': 'chain_with_star', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 64: {'origin': {'name': 'path_with_action', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'atom', '__type__': 'NonTerminal'}, {'name': 'action_separate_with_dot', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 65: {'origin': {'name': 'path_with_action', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'atom', '__type__': 'NonTerminal'}, {'name': 'predicate', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 66: {'origin': {'name': 'path', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'path_with_action', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 67: {'origin': {'name': 'path', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'first_path', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 68: {'origin': {'name': 'args', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'args', '__type__': 'NonTerminal'}, {'name': 'COMMA', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'multi_args', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 69: {'origin': {'name': 'args', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}], 'order': 1, 'alias': 'single_arg', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 70: {'origin': {'name': 'funccall', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'CNAME', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'LPAR', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'args', '__type__': 'NonTerminal'}, {'name': 'RPAR', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 71: {'origin': {'name': 'funccall', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'CNAME', 'filter_out': False, '__type__': 'Terminal'}, {'name': '__ANON_0', 'filter_out': True, '__type__': 'Terminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 72: {'origin': {'name': 'atom', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'value', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 73: {'origin': {'name': 'atom', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'path', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 74: {'origin': {'name': 'atom', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'funccall', '__type__': 'NonTerminal'}], 'order': 2, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 75: {'origin': {'name': 'atom', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'LPAR', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'RPAR', 'filter_out': True, '__type__': 'Terminal'}], 'order': 3, 'alias': 'parenthesized_expr', 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 76: {'origin': {'name': 'expr', '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}}
+{0: {'name': 'NUMBER', 'pattern': {'value': '(?:(?:\\+|\\-))?(?:(?:(?:[0-9])+(?:e|E)(?:(?:\\+|\\-))?(?:[0-9])+|(?:(?:[0-9])+\\.(?:(?:[0-9])+)?|\\.(?:[0-9])+)(?:(?:e|E)(?:(?:\\+|\\-))?(?:[0-9])+)?)|(?:[0-9])+)', 'flags': [], '_width': [1, 4294967295], '__type__': 'PatternRE'}, 'priority': 0, '__type__': 'TerminalDef'}, 1: {'name': 'CNAME', 'pattern': {'value': '(?:(?:[A-Z]|[a-z])|_)(?:(?:(?:[A-Z]|[a-z])|[0-9]|_))*', 'flags': [], '_width': [1, 4294967295], '__type__': 'PatternRE'}, 'priority': 0, '__type__': 'TerminalDef'}, 2: {'name': 'WS_INLINE', 'pattern': {'value': '(?:(?:\\ |\t))+', 'flags': [], '_width': [1, 4294967295], '__type__': 'PatternRE'}, 'priority': 0, '__type__': 'TerminalDef'}, 3: {'name': 'COLON', 'pattern': {'value': ':', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 4: {'name': 'STRING', 'pattern': {'value': '`([^`\\\\]|\\\\.)*?`|\'([^\'\\\\]|\\\\.)*?\'|"([^"\\\\]|\\\\.)*?"', 'flags': ['i'], '_width': [2, 4294967295], '__type__': 'PatternRE'}, 'priority': 0, '__type__': 'TerminalDef'}, 5: {'name': 'STAR', 'pattern': {'value': '*', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 6: {'name': 'DOT', 'pattern': {'value': '.', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 7: {'name': 'DOUBLE_DOT', 'pattern': {'value': '..', 'flags': [], '__type__': 'PatternStr'}, 'priority': 2, '__type__': 'TerminalDef'}, 8: {'name': 'COMPARE_OPERATOR', 'pattern': {'value': '(?:<=|>=|!=|<|>|=)', 'flags': [], '_width': [1, 2], '__type__': 'PatternRE'}, 'priority': 0, '__type__': 'TerminalDef'}, 9: {'name': 'AND', 'pattern': {'value': 'and', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 10: {'name': 'OR', 'pattern': {'value': 'or', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 11: {'name': 'TRUE', 'pattern': {'value': 'true', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 12: {'name': 'FALSE', 'pattern': {'value': 'false', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 13: {'name': 'NULL', 'pattern': {'value': 'null', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 14: {'name': 'AT', 'pattern': {'value': '@', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 15: {'name': 'DOLLAR', 'pattern': {'value': '$', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 16: {'name': 'LSQB', 'pattern': {'value': '[', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 17: {'name': 'RSQB', 'pattern': {'value': ']', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 18: {'name': 'COMMA', 'pattern': {'value': ',', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 19: {'name': 'LPAR', 'pattern': {'value': '(', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 20: {'name': 'RPAR', 'pattern': {'value': ')', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 21: {'name': '__ANON_0', 'pattern': {'value': '()', 'flags': [], '__type__': 'PatternStr'}, 'priority': 0, '__type__': 'TerminalDef'}, 22: {'origin': {'name': Token('RULE', 'start'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'path', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 23: {'origin': {'name': Token('RULE', 'start'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'func_call', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 24: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 25: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 1, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [False, False, False, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 26: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 2, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [False, False, True, False, False], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 27: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 3, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [False, False, True, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 28: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 4, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, False, False, False], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 29: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 5, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, False, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 30: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 6, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, True, False, False], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 31: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 7, 'alias': 'three_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, True, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 32: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 8, 'alias': 'two_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 33: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 9, 'alias': 'two_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [False, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 34: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 10, 'alias': 'two_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, False], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 35: {'origin': {'name': Token('RULE', 'slice'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'COLON', 'filter_out': False, '__type__': 'Terminal'}], 'order': 11, 'alias': 'two_fields_slice', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': [True, False, True], '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 36: {'origin': {'name': Token('RULE', 'true'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'TRUE', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 37: {'origin': {'name': Token('RULE', 'false'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'FALSE', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 38: {'origin': {'name': Token('RULE', 'null'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'NULL', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 39: {'origin': {'name': Token('RULE', 'value'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'NUMBER', 'filter_out': False, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 40: {'origin': {'name': Token('RULE', 'value'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'true', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 41: {'origin': {'name': Token('RULE', 'value'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'false', '__type__': 'NonTerminal'}], 'order': 2, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 42: {'origin': {'name': Token('RULE', 'value'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'null', '__type__': 'NonTerminal'}], 'order': 3, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 43: {'origin': {'name': Token('RULE', 'value'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'STRING', 'filter_out': False, '__type__': 'Terminal'}], 'order': 4, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 44: {'origin': {'name': Token('RULE', 'identifier'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'CNAME', 'filter_out': False, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 45: {'origin': {'name': Token('RULE', 'identifier'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'STRING', 'filter_out': False, '__type__': 'Terminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 46: {'origin': {'name': Token('RULE', 'self'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'AT', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 47: {'origin': {'name': Token('RULE', 'root'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOLLAR', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 48: {'origin': {'name': Token('RULE', 'first_path'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'CNAME', 'filter_out': False, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 49: {'origin': {'name': Token('RULE', 'first_path'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'self', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 50: {'origin': {'name': Token('RULE', 'first_path'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'root', '__type__': 'NonTerminal'}], 'order': 2, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 51: {'origin': {'name': Token('RULE', 'test_comparison'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'atom', '__type__': 'NonTerminal'}, {'name': 'COMPARE_OPERATOR', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'atom', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'comparison_expr', 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 52: {'origin': {'name': Token('RULE', 'test_comparison'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'atom', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 53: {'origin': {'name': Token('RULE', 'test'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test', '__type__': 'NonTerminal'}, {'name': 'OR', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'test_and', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'or_expr', 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 54: {'origin': {'name': Token('RULE', 'test'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test_and', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 55: {'origin': {'name': Token('RULE', 'test_and'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test_and', '__type__': 'NonTerminal'}, {'name': 'AND', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'test_comparison', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'and_expr', 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 56: {'origin': {'name': Token('RULE', 'test_and'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test_comparison', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 57: {'origin': {'name': Token('RULE', 'predicate'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'LSQB', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'RSQB', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 58: {'origin': {'name': Token('RULE', 'predicate'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'LSQB', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'slice', '__type__': 'NonTerminal'}, {'name': 'RSQB', 'filter_out': True, '__type__': 'Terminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 59: {'origin': {'name': Token('RULE', 'predicate'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'LSQB', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'STAR', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'RSQB', 'filter_out': True, '__type__': 'Terminal'}], 'order': 2, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 60: {'origin': {'name': Token('RULE', 'action_separate_with_dot'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOUBLE_DOT', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'predicate', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'search_with_predicate', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 61: {'origin': {'name': Token('RULE', 'action_separate_with_dot'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOUBLE_DOT', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'identifier', '__type__': 'NonTerminal'}], 'order': 1, 'alias': 'search_with_identifier', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 62: {'origin': {'name': Token('RULE', 'action_separate_with_dot'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOT', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'identifier', '__type__': 'NonTerminal'}], 'order': 2, 'alias': 'chain_with_identifier', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 63: {'origin': {'name': Token('RULE', 'action_separate_with_dot'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'DOT', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'STAR', 'filter_out': False, '__type__': 'Terminal'}], 'order': 3, 'alias': 'chain_with_star', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 64: {'origin': {'name': Token('RULE', 'path_with_action'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'atom', '__type__': 'NonTerminal'}, {'name': 'action_separate_with_dot', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 65: {'origin': {'name': Token('RULE', 'path_with_action'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'atom', '__type__': 'NonTerminal'}, {'name': 'predicate', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 66: {'origin': {'name': Token('RULE', 'path'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'path_with_action', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 67: {'origin': {'name': Token('RULE', 'path'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'first_path', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 68: {'origin': {'name': Token('RULE', 'args'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'args', '__type__': 'NonTerminal'}, {'name': 'COMMA', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}], 'order': 0, 'alias': 'multi_args', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 69: {'origin': {'name': Token('RULE', 'args'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'expr', '__type__': 'NonTerminal'}], 'order': 1, 'alias': 'single_arg', 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 70: {'origin': {'name': Token('RULE', 'func_call'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'CNAME', 'filter_out': False, '__type__': 'Terminal'}, {'name': 'LPAR', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'args', '__type__': 'NonTerminal'}, {'name': 'RPAR', 'filter_out': True, '__type__': 'Terminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 71: {'origin': {'name': Token('RULE', 'func_call'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'CNAME', 'filter_out': False, '__type__': 'Terminal'}, {'name': '__ANON_0', 'filter_out': True, '__type__': 'Terminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': False, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 72: {'origin': {'name': Token('RULE', 'atom'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'value', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 73: {'origin': {'name': Token('RULE', 'atom'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'path', '__type__': 'NonTerminal'}], 'order': 1, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 74: {'origin': {'name': Token('RULE', 'atom'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'func_call', '__type__': 'NonTerminal'}], 'order': 2, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 75: {'origin': {'name': Token('RULE', 'atom'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'LPAR', 'filter_out': True, '__type__': 'Terminal'}, {'name': 'expr', '__type__': 'NonTerminal'}, {'name': 'RPAR', 'filter_out': True, '__type__': 'Terminal'}], 'order': 3, 'alias': 'parenthesized_expr', 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}, 76: {'origin': {'name': Token('RULE', 'expr'), '__type__': 'NonTerminal'}, 'expansion': [{'name': 'test', '__type__': 'NonTerminal'}], 'order': 0, 'alias': None, 'options': {'keep_all_tokens': False, 'expand1': True, 'priority': None, 'template_source': None, 'empty_indices': (), '__type__': 'RuleOptions'}, '__type__': 'Rule'}}
 )
 Shift = 0
 Reduce = 1
 def Lark_StandAlone(**kwargs):
   return Lark._load_from_dict(DATA, MEMO, **kwargs)
```

### Comparing `jsonpath-extractor-0.8.0/jsonpath/parser.py` & `jsonpath-extractor-0.9.0/jsonpath/parser.py`

 * *Files identical despite different names*

### Comparing `jsonpath-extractor-0.8.0/jsonpath/transformer.py` & `jsonpath-extractor-0.9.0/jsonpath/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 T_NO_ARG = Iterable
 T_ARGS = Union[T_NO_ARG, List[T_ARG]]
 
 
 @v_args(inline=True)
 class JSONPathTransformer(Transformer[Expr]):
     """
-    Transform JSONPath expression AST parsed by lark-parser into an executable object.
+    Transform JSONPath expression AST parsed by lark into an executable object.
     """
 
     INT = int
 
     def cdr(self, *args: Any) -> Any:
         return args[1]
 
@@ -153,15 +153,15 @@
         colon_1: Literal[":"],
         second_field: Optional[Expr],
         colon_2: Literal[":"],
         third_field: Optional[Expr],
     ) -> Slice:
         return Slice(start=first_field, stop=second_field, step=third_field)
 
-    def funccall(self, name: str, args: T_ARGS = tuple()) -> Function:
+    def func_call(self, name: str, args: T_ARGS = tuple()) -> Function:
         if name == "key":
             return Key(*args)
         elif name == "contains":
             return Contains(*args)
         elif name == "not":
             return Not(*args)
         else:
```

### Comparing `jsonpath-extractor-0.8.0/pyproject.toml` & `jsonpath-extractor-0.9.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,90 @@
 [project]
 name = "jsonpath-extractor"
-version = "0.8.0"
+authors = [
+    { name = "林玮 (Jade Lin)", email = "linw1995@icloud.com" },
+]
 description = "A selector expression for extracting data from JSON."
 readme = "README.rst"
-classifiers = [ "Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Programming Language :: Python", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Development Status :: 4 - Beta", "Operating System :: POSIX", "Operating System :: MacOS :: MacOS X", "Operating System :: Microsoft :: Windows",]
-keywords = [ "data-extractor", "data-extraction", "jsonpath", "json",]
-dependencies = [ "typing-extensions ~= 3.7",]
-requires-python = ">=3.7"
-dynamic = [ "version",]
-[[project.authors]]
-name = "林玮 (Jade Lin)"
-email = "linw1995@icloud.com"
-
-[build-system]
-requires = [ "intreehooks", "pdm-pep517", "lark-parser ~= 0.11.3",]
-build-backend = "intreehooks:loader"
+classifiers = [
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Development Status :: 4 - Beta",
+    "Operating System :: POSIX",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows",
+]
+keywords = [
+    "data-extractor",
+    "data-extraction",
+    "jsonpath",
+    "json",
+]
+dependencies = [
+    "typing-extensions ~= 4.7",
+]
+requires-python = ">=3.8"
+dynamic = []
+version = "0.9.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/linw1995/jsonpath"
 repository = "https://github.com/linw1995/jsonpath"
 documentation = "https://jsonpath.rtfd.io/en/latest/"
 
 [project.optional-dependencies]
-parser = [ "lark-parser ~= 0.11.3",]
+parser = [
+    "lark ~= 1.1.0",
+]
 
 [project.scripts]
 jp = "jsonpath.cli:main"
 
-[tool.intreehooks]
+[build-system]
+requires = [
+    "pdm-pep517",
+    "lark ~= 1.1.0",
+]
+backend-path = [
+    ".",
+]
 build-backend = "jsonpath_build"
 
 [tool.pdm]
-includes = [ "jsonpath/*.py", "jsonpath_build.py", "jsonpath/lark_parser.py", "jsonpath/py.typed",]
-excludes = [ "**/.mypy_cache",]
+includes = [
+    "jsonpath/*.py",
+    "jsonpath_build.py",
+    "jsonpath/lark_parser.py",
+    "jsonpath/py.typed",
+    "jsonpath/grammar.lark",
+]
+excludes = [
+    "**/.mypy_cache",
+]
+
+[tool.pdm.version]
+use_scm = true
 
 [tool.pdm.dev-dependencies]
-docs = [ "sphinx ~= 3.5", "livereload ~= 2.6", "lark-parser ~= 0.11.3",]
-test = [ "pytest-cov ~= 2.11", "pexpect ~= 4.8", "sybil ~= 2.0",]
-build_readme = [ "pygments ~= 2.8", "docutils >= 0.16",]
+docs = [
+    "sphinx ~= 3.5",
+    "livereload ~= 2.6",
+    "lark ~= 1.1.0",
+]
+test = [
+    "pytest-cov ~= 2.11",
+    "pexpect ~= 4.8",
+    "sybil ~= 2.0",
+]
+build_readme = [
+    "pygments ~= 2.8",
+    "docutils >= 0.16",
+]
```

### Comparing `jsonpath-extractor-0.8.0/tests/test_cli.py` & `jsonpath-extractor-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jsonpath-extractor-0.8.0/tests/test_core.py` & `jsonpath-extractor-0.9.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jsonpath-extractor-0.8.0/tests/test_lark.py` & `jsonpath-extractor-0.9.0/tests/test_lark.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     "a[*]",
     "$[@]",
     "$[$]",
     "a[b]",
     "a[b][c]",
     "(a[b])[c]",
     "a.*",
+    "a.'*'",
     "a.'b'",
     "a..[b]",
     "a..[0]",
     "a..[:3]",
     "$.goods[contains(@.category, $.targetCategory)]",
     "$.goods[@.category]",
     "$.goods[@.price > 10]",
@@ -131,14 +132,15 @@
 pytest.mark.parametrize(
     "expression, data, expect",
     [
         ("boo", {"boo": 1}, [1]),
         ("boo.bar", {"boo": {"bar": 1}}, [1]),
         ("boo.bar.boo", {"boo": {"bar": {"boo": 1}}}, [1]),
         ("$.*", {"boo": 1, "bar": 2}, [1, 2]),
+        ("$.'*'", {"boo": 1, "bar": 2, "*": 3}, [3]),
         ("boo.*", {"boo": {"boo": 1, "bar": 2}}, [1, 2]),
         ("boo.*.boo", {"boo": {"boo": {"boo": 1}, "bar": {"boo": 2}}}, [1, 2]),
         ("boo.*.boo", {"boo": {"boo": {"boo": 1}, "bar": {"bar": 2}}}, [1]),
         ("boo.*.boo", {"boo": {"boo": {"boo": 1}, "bar": 1}}, [1]),
         ("$[0]", [1, 2], [1]),
         ("$[1]", [1, 2], [2]),
         ("$[2]", [1, 2], []),
```

