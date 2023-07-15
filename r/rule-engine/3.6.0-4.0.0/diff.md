# Comparing `tmp/rule-engine-3.6.0.tar.gz` & `tmp/rule-engine-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rule-engine-3.6.0.tar", last modified: Sat Jun 17 16:22:33 2023, max compression
+gzip compressed data, was "rule-engine-4.0.0.tar", last modified: Sat Jul 15 16:37:00 2023, max compression
```

## Comparing `rule-engine-3.6.0.tar` & `rule-engine-4.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:22:33.023142 rule-engine-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-17 16:22:03.000000 rule-engine-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-17 16:22:33.023142 rule-engine-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-17 16:22:03.000000 rule-engine-3.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:22:33.019142 rule-engine-3.6.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:22:33.019142 rule-engine-3.6.0/lib/rule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49596 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/debug_repl.py
--rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/suggestions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-06-17 16:22:03.000000 rule-engine-3.6.0/lib/rule_engine/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:22:33.023142 rule-engine-3.6.0/lib/rule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 16:22:32.000000 rule-engine-3.6.0/lib/rule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 16:22:33.023142 rule-engine-3.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3732 2023-06-17 16:22:03.000000 rule-engine-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:37:00.653619 rule-engine-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-15 16:36:32.000000 rule-engine-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-15 16:37:00.653619 rule-engine-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-15 16:36:32.000000 rule-engine-4.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:37:00.653619 rule-engine-4.0.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:37:00.653619 rule-engine-4.0.0/lib/rule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52126 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/debug_repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23588 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21819 2023-07-15 16:36:32.000000 rule-engine-4.0.0/lib/rule_engine/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:37:00.653619 rule-engine-4.0.0/lib/rule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 16:37:00.000000 rule-engine-4.0.0/lib/rule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:37:00.653619 rule-engine-4.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3778 2023-07-15 16:36:32.000000 rule-engine-4.0.0/setup.py
```

### Comparing `rule-engine-3.6.0/LICENSE` & `rule-engine-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rule-engine-3.6.0/PKG-INFO` & `rule-engine-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 3.6.0
+Version: 4.0.0
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
@@ -16,28 +16,25 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Rule Engine
 ===========
 |badge-build| |badge-pypi|
 
 A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 
 Documentation is available at https://zeroSteiner.github.io/rule-engine/.
 
-:Warning:
-  Version 3.6 is the last to support Python versions 3.4 and 3.5. The next version, either 3.7 or 4.0, will drop them.
-  There is currently no timeline for its release.
-
 Rule Engine expressions are written in their own language, defined as strings in Python. The syntax is most similar to
 Python with some inspiration from Ruby. Some features of this language includes:
 
 - Optional type hinting
 - Matching strings with regular expressions
 - Datetime datatypes
 - Compound datatypes (equivalents for Python dict, list and set types)
```

### Comparing `rule-engine-3.6.0/README.rst` & `rule-engine-4.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 ===========
 |badge-build| |badge-pypi|
 
 A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 
 Documentation is available at https://zeroSteiner.github.io/rule-engine/.
 
-:Warning:
-  Version 3.6 is the last to support Python versions 3.4 and 3.5. The next version, either 3.7 or 4.0, will drop them.
-  There is currently no timeline for its release.
-
 Rule Engine expressions are written in their own language, defined as strings in Python. The syntax is most similar to
 Python with some inspiration from Ruby. Some features of this language includes:
 
 - Optional type hinting
 - Matching strings with regular expressions
 - Datetime datatypes
 - Compound datatypes (equivalents for Python dict, list and set types)
```

### Comparing `rule-engine-3.6.0/lib/rule_engine/__init__.py` & `rule-engine-4.0.0/lib/rule_engine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #  LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 #  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = '3.6.0'
+__version__ = '4.0.0'
 
 from .engine import resolve_attribute
 from .engine import resolve_item
 from .engine import type_resolver_from_dict
 from .engine import Context
 from .engine import Rule
```

### Comparing `rule-engine-3.6.0/lib/rule_engine/ast.py` & `rule-engine-4.0.0/lib/rule_engine/ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,20 +34,18 @@
 import collections.abc
 import datetime
 import functools
 import operator
 import re
 
 from . import errors
-from ._utils import parse_timedelta
+from ._utils import parse_datetime, parse_float, parse_timedelta
 from .suggestions import suggest_symbol
 from .types import *
 
-import dateutil.parser
-
 def _assert_is_integer_number(*values):
 	if not all(map(is_integer_number, values)):
 		raise errors.EvaluationError('data type mismatch (not an integer number)')
 
 def _assert_is_natural_number(*values):
 	if not all(map(is_natural_number, values)):
 		raise errors.EvaluationError('data type mismatch (not a natural number)')
@@ -58,28 +56,28 @@
 
 def _assert_is_string(*values):
 	if not all(map(isinstance, values, [str])):
 		raise errors.EvaluationError('data type mismatch (not a string value)')
 
 def _is_reduced(*values):
 	"""
-	Check if the ast expression *value* is a literal expression and if it is a compound datatype, that all of it's
+	Check if the ast expression *value* is a literal expression and if it is a compound datatype, that all of its
 	members are reduced literals. A value that causes this to evaluate to True for is able to be evaluated without a
 	*thing*.
 	"""
 	return all((isinstance(value, LiteralExpressionBase) and value.is_reduced) for value in values)
 
 def _iterable_member_value_type(value):
 	value = (
 		member.result_type if isinstance(member, ExpressionBase) else member for member in value
 	)
 	return iterable_member_value_type(value)
 
 class Assignment(object):
-	"""An internal assignment where by a symbol is populated with a value of the specified type."""
+	"""An internal assignment whereby a symbol is populated with a value of the specified type."""
 	__slots__ = ('name', 'value', 'value_type')
 	def __init__(self, name, *, value=errors.UNDEFINED, value_type=None):
 		"""
 		:param str name: The symbol name that the assignment is defining.
 		:param value: The value of the assignment.
 		:param value_type: The data type of the assignment.
 		:type value_type: :py:class:`~.DataType`
@@ -237,44 +235,39 @@
 class DatetimeExpression(LiteralExpressionBase):
 	"""
 	Literal datetime expressions representing a specific point in time. This expression type always evaluates to true.
 	"""
 	result_type = DataType.DATETIME
 	@classmethod
 	def from_string(cls, context, string):
-		try:
-			dt = dateutil.parser.isoparse(string)
-		except ValueError:
-			raise errors.DatetimeSyntaxError('invalid datetime', string)
-		if dt.tzinfo is None:
-			dt = dt.replace(tzinfo=context.default_timezone)
+		dt = parse_datetime(string, default_timezone=context.default_timezone)
 		return cls(context, dt)
 
 class TimedeltaExpression(LiteralExpressionBase):
 	"""
 	Literal timedelta expressions representing an offset from a specific point in time.
 
 	.. versionadded:: 3.5.0
 	"""
 	result_type = DataType.TIMEDELTA
 	@classmethod
 	def from_string(cls, context, string):
-		try:
-			dt = parse_timedelta(string)
-		except ValueError:
-			raise errors.TimedeltaSyntaxError('invalid timedelta', string)
-		return cls(context, dt)
+		return cls(context, parse_timedelta(string))
 
 class FloatExpression(LiteralExpressionBase):
 	"""Literal float expressions representing numerical values."""
 	result_type = DataType.FLOAT
 	def __init__(self, context, value, **kwargs):
 		value = coerce_value(value)
 		super(FloatExpression, self).__init__(context, value, **kwargs)
 
+	@classmethod
+	def from_string(cls, context, string):
+		return cls(context, parse_float(string))
+
 class MappingExpression(LiteralExpressionBase):
 	"""Literal mapping expression representing a set of associations between keys and values."""
 	result_type = DataType.MAPPING
 	def __init__(self, context, value, **kwargs):
 		if isinstance(value, dict):
 			value = tuple(value.items())
 		super(MappingExpression, self).__init__(context, value, **kwargs)
@@ -1030,14 +1023,76 @@
 			return value
 
 		raise errors.SymbolTypeError(self.name, is_value=value, is_type=value_type, expected_type=self.result_type)
 
 	def to_graphviz(self, digraph, *args, **kwargs):
 		digraph.node(str(id(self)), "{}\nname={!r}".format(self.__class__.__name__, self.name))
 
+class FunctionCallExpression(ExpressionBase):
+	__slots__ = ('function', 'arguments',)
+	def __init__(self, context, function, arguments):
+		self.context = context
+		self.function = function
+		if self.function.result_type != DataType.UNDEFINED:
+			function_type = self.function.result_type
+			self._validate_function(function_type, arguments)
+			self.result_type = function_type.return_type
+		self.arguments = arguments
+
+	@classmethod
+	def build(cls, context, function, arguments):
+		return cls(context, function.build(), tuple(argument.build() for argument in arguments)).reduce()
+
+	# because there is no syntax for defining a function, they can't be reduced until symbols can be reduced
+
+	def evaluate(self, thing):
+		function = self.function.evaluate(thing)
+		if not callable(function):
+			raise errors.EvaluationError('data type mismatch (not a callable value)')
+		arguments = tuple(argument.evaluate(thing) for argument in self.arguments)
+		function_name = function.__name__ + '?'
+		if self.function.result_type != DataType.UNDEFINED:
+			function_type = self.function.result_type
+			function_name = function_type.value_name
+			self._validate_function(function_type, arguments)
+		try:
+			result = function(*arguments)
+		except errors.FunctionCallError as error:
+			error.function_name = function_name
+			raise error
+		except Exception as error:
+			raise errors.FunctionCallError('function call failed', error=error, function_name=function_name) from None
+		return self._new_value(result)
+
+	def _validate_function(self, function_type, arguments):
+		if not isinstance(function_type, DataType.FUNCTION.__class__):
+			raise errors.EvaluationError('data type mismatch (not a callable value)')
+		if function_type.minimum_arguments is not DataType.UNDEFINED:
+			if len(arguments) < function_type.minimum_arguments:
+				raise errors.FunctionCallError(
+					"expected at least {} positional arguments".format(function_type.minimum_arguments),
+					function_name=function_type.value_name
+				)
+		if function_type.argument_types is not DataType.UNDEFINED:
+			if len(arguments) > len(function_type.argument_types):
+				raise errors.FunctionCallError(
+					"expected at most {} positional arguments".format(len(function_type.argument_types)),
+					function_name=function_type.value_name
+				)
+			for pos, (arg1, arg2_type) in enumerate(zip(arguments, function_type.argument_types), 1):
+				if isinstance(arg1, LiteralExpressionBase):
+					arg1_type = arg1.result_type
+				else:
+					arg1_type = DataType.from_value(arg1)
+				if not DataType.is_compatible(arg1_type, arg2_type):
+					raise errors.FunctionCallError(
+						"data type mismatch (argument #{})".format(pos),
+						function_name=function_type.value_name
+					)
+
 class Statement(ASTNodeBase):
 	"""A class representing the top level statement of the grammar text."""
 	__slots__ = ('context', 'expression', 'comment')
 	def __init__(self, context, expression, comment=None):
 		"""
 		:param context: The context to use for evaluating the statement.
 		:type context: :py:class:`~rule_engine.engine.Context`
@@ -1080,30 +1135,28 @@
 		self.condition = condition
 		self.case_true = case_true
 		self.case_false = case_false
 		if self.case_true.result_type == self.case_false.result_type:
 			self.result_type = self.case_true.result_type
 		elif isinstance(self.case_true.result_type, DataType.ARRAY.__class__) and isinstance(self.case_false.result_type, DataType.ARRAY.__class__):
 			self.result_type = DataType.ARRAY
+		# todo: the other compound types should be checked here as well.
 
 	@classmethod
 	def build(cls, context, condition, case_true, case_false):
 		return cls(context, condition.build(), case_true.build(), case_false.build()).reduce()
 
 	def evaluate(self, thing):
 		case = (self.case_true if self.condition.evaluate(thing) else self.case_false)
 		return case.evaluate(thing)
 
 	def reduce(self):
-		if _is_reduced(self.condition):
-			reduced_condition = bool(self.condition.value)
-		else:
-			reduced_condition = self.condition.reduce()
-			if reduced_condition is self.condition:
-				return self
+		if not _is_reduced(self.condition):
+			return self
+		reduced_condition = bool(self.condition.value)
 		return self.case_true.reduce() if reduced_condition else self.case_false.reduce()
 
 	def to_graphviz(self, digraph, *args, **kwargs):
 		super(TernaryExpression, self).to_graphviz(digraph, *args, **kwargs)
 		self.condition.to_graphviz(digraph, *args, **kwargs)
 		self.case_true.to_graphviz(digraph, *args, **kwargs)
 		self.case_false.to_graphviz(digraph, *args, **kwargs)
@@ -1122,22 +1175,21 @@
 		:param str type_: The grammar type of operator to the left of the expression.
 		:param right: The expression to the right of the operator.
 		:type right: :py:class:`~.ExpressionBase`
 		"""
 		self.context = context
 		type_ = type_.lower()
 		self.type = type_
-		self._evaluator = getattr(self, '_op_' + type_)
 		if type_ == 'not':
 			self.result_type = DataType.BOOLEAN
 		elif type_ == 'uminus':
 			self.result_type = right.result_type
 		else:
-			raise errors.EvaluationError('unknown unary expression type')
-
+			raise ValueError('unknown unary expression type')
+		self._evaluator = getattr(self, '_op_' + type_)
 		self.right = right
 
 	@classmethod
 	def build(cls, context, type_, right):
 		return cls(context, type_, right.build()).reduce()
 
 	def __repr__(self):
```

### Comparing `rule-engine-3.6.0/lib/rule_engine/debug_repl.py` & `rule-engine-4.0.0/lib/rule_engine/debug_repl.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 #
 
 import argparse
 import code
 import io
 import os
 import pprint
+import re
 import sys
+import textwrap
 import traceback
 
 from . import __version__
 from . import engine
 from . import errors
 
 def _console_interact(console, *args, **kwargs):
@@ -93,32 +95,47 @@
 			_console_interact(
 				console,
 				banner='edit the \'context\' and \'thing\' objects as necessary',
 				exitmsg='exiting the edit console...'
 			)
 		context = console.locals['context']
 		thing = console.locals['thing']
+	debugging = arguments.debug
 
 	while True:
 		try:
 			rule_text = input('rule > ')
 		except (EOFError, KeyboardInterrupt):
 			break
 
+		match = re.match(r'\s*#!\s*debug\s*=\s*(\w+)', rule_text)
+		if match:
+			debugging = match.group(1).lower() != 'false'
+			print('# debugging = ' + str(debugging).lower())
+			continue
+
 		try:
 			rule = engine.Rule(rule_text, context=context)
 			result = rule.evaluate(thing)
 		except errors.EngineError as error:
 			print("{}: {}".format(error.__class__.__name__, error.message))
 			if isinstance(error, (errors.AttributeResolutionError, errors.SymbolResolutionError)) and error.suggestion:
 				print("Did you mean '{}'?".format(error.suggestion))
 			elif isinstance(error, errors.RegexSyntaxError):
 				print("  Regex:   {!r}".format(error.error.pattern))
 				print("  Details: {} at position {}".format(error.error.msg, error.error.pos))
-			if arguments.debug:
+			elif isinstance(error, errors.FunctionCallError):
+				if debugging:
+					inner_exception = ''.join(traceback.format_exception(
+						error.error,
+						error.error,
+						error.error.__traceback__
+					))
+					print(textwrap.indent(inner_exception, ' ' * 2))
+			if debugging:
 				traceback.print_exc()
 		except Exception as error:
 			traceback.print_exc()
 		else:
 			print('result: ')
 			pprint.pprint(result, indent=4)
```

### Comparing `rule-engine-3.6.0/lib/rule_engine/engine.py` & `rule-engine-4.0.0/lib/rule_engine/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,21 @@
 import decimal
 import functools
 import math
 import re
 import threading
 
 from . import ast
+from . import builtins
 from . import errors
 from . import parser
 from .suggestions import suggest_symbol
 
 import dateutil.tz
 
-def _now(builtins):
-	return datetime.datetime.now(tz=builtins.timezone)
-
-def _today(builtins):
-	return _now(builtins).replace(hour=0, minute=0, second=0, microsecond=0)
-
 def _tls_getter(thread_local, key, _builtins):
 	# a function stub to be used with functools.partial for retrieving thread-local values
 	return getattr(thread_local.storage, key)
 
 def resolve_attribute(thing, name):
 	"""
 	A replacement resolver function for looking up symbols as members of *thing*. This is effectively the same as
@@ -271,15 +266,15 @@
 
 	@attribute('as_upper', ast.DataType.STRING, result_type=ast.DataType.STRING)
 	def string_as_upper(self, value):
 		return value.upper()
 
 	@attribute('to_ary', ast.DataType.STRING, result_type=ast.DataType.ARRAY(ast.DataType.STRING))
 	def string_to_ary(self, value):
-		return value.split()
+		return tuple(value)
 
 	@attribute('to_flt', ast.DataType.STRING, result_type=ast.DataType.FLOAT)
 	def string_to_flt(self, value):
 		value = value.strip()
 		if re.match(r'-?inf', value):
 			return decimal.Decimal(value)
 		match = re.match(r'^(' + parser.Parser.get_token_regex('FLOAT') + ')$', value)
@@ -302,89 +297,14 @@
 	def value_length(self, value):
 		return len(value)
 
 	@attribute('to_set', ast.DataType.ARRAY, ast.DataType.STRING, result_type=ast.DataType.SET)
 	def value_to_set(self, value):
 		return set(value)
 
-class Builtins(collections.abc.Mapping):
-	"""
-	A class to define and provide variables to within the builtin context of rules. These can be accessed by specifying
-	a symbol name with the ``$`` prefix.
-	"""
-	scope_name = 'built-in'
-	"""The identity name of the scope for builtin symbols."""
-	def __init__(self, values, namespace=None, timezone=None, value_types=None):
-		"""
-		:param dict values: A mapping of string keys to be used as symbol names with values of either Python literals or
-			a function which will be called when the symbol is accessed. When using a function, it will be passed a
-			single argument, which is the instance of :py:class:`Builtins`.
-		:param str namespace: The namespace of the variables to resolve.
-		:param timezone: A timezone to use when resolving timestamps.
-		:type timezone: :py:class:`~datetime.tzinfo`
-		:param dict value_types: A mapping of the values to their datatypes.
-
-		.. versionchanged:: 2.3.0
-			Added the *value_types* parameter.
-		"""
-		self.__values = values
-		self.__value_types = value_types or {}
-		self.namespace = namespace
-		self.timezone = timezone or dateutil.tz.tzlocal()
-
-	def resolve_type(self, name):
-		"""
-		The method to use for resolving the data type of a builtin symbol.
-
-		:param str name: The name of the symbol to retrieve the data type of.
-		:return: The data type of the symbol or :py:attr:`~rule_engine.ast.DataType.UNDEFINED`.
-		"""
-		return self.__value_types.get(name, ast.DataType.UNDEFINED)
-
-	def __repr__(self):
-		return "<{} namespace={!r} keys={!r} timezone={!r} >".format(self.__class__.__name__, self.namespace, tuple(self.keys()), self.timezone)
-
-	def __getitem__(self, name):
-		value = self.__values[name]
-		if isinstance(value, collections.abc.Mapping):
-			if self.namespace is None:
-				namespace = name
-			else:
-				namespace = self.namespace + '.' + name
-			return self.__class__(value, namespace=namespace, timezone=self.timezone)
-		elif callable(value):
-			value = value(self)
-		return value
-
-	def __iter__(self):
-		return iter(self.__values)
-
-	def __len__(self):
-		return len(self.__values)
-
-	@classmethod
-	def from_defaults(cls, values=None, **kwargs):
-		"""Initialize a :py:class:`Builtins` instance with a set of default values."""
-		# there may be errors here if the decimal.Context precision exceeds what is provided by the math constants
-		default_values = {
-			'e': decimal.Decimal(repr(math.e)),
-			'pi': decimal.Decimal(repr(math.pi)),
-			'now': _now,
-			'today': _today
-		}
-		default_values.update(values or {})
-		default_value_types = {
-			'e': ast.DataType.FLOAT,
-			'pi': ast.DataType.FLOAT,
-			'now': ast.DataType.DATETIME,
-			'today': ast.DataType.DATETIME
-		}
-		default_value_types.update(kwargs.pop('value_types', {}))
-		return cls(default_values, value_types=default_value_types, **kwargs)
-
 class _ThreadLocalStorage(object):
 	"""
 	An object whose attributes are required to be tracked separately among multiple threads. This is to guarantee that
 	if a context is used by one or more rules that are being evaluated simultaneously in multiple threads, that the
 	states are kept isolated.
 	"""
 	__slots__ = ('assignment_scopes', 'regex_groups')
@@ -399,14 +319,15 @@
 class Context(object):
 	"""
 	An object defining the context for a rule's evaluation. This can be used to change the behavior of certain aspects
 	of the rule such as how symbols are resolved and what regex flags should be used.
 	"""
 	def __init__(
 			self,
+			*,
 			regex_flags=0,
 			resolver=None,
 			type_resolver=None,
 			default_timezone='local',
 			default_value=errors.UNDEFINED,
 			decimal_context=None
 	):
@@ -456,35 +377,35 @@
 		elif not isinstance(default_timezone, datetime.tzinfo):
 			raise TypeError('invalid default_timezone type')
 		self._thread_local = threading.local()
 		self.default_timezone = default_timezone
 		"""The *default_timezone* parameter from :py:meth:`~__init__`"""
 		self.default_value = default_value
 		"""The *default_value* parameter from :py:meth:`~__init__`"""
-		self.builtins = Builtins.from_defaults(
-			values={'re_groups': functools.partial(_tls_getter, self._thread_local, 'regex_groups')},
+		self.builtins = builtins.Builtins.from_defaults(
+			values={'re_groups': builtins.BuiltinValueGenerator(functools.partial(_tls_getter, self._thread_local, 'regex_groups'))},
 			value_types={'re_groups': ast.DataType.ARRAY(ast.DataType.STRING)},
 			timezone=default_timezone
 		)
-		"""An instance of :py:class:`Builtins` to provided a default set of builtin symbol values."""
+		"""An instance of :py:class:`~rule_engine.builtins.Builtins` to provided a default set of builtin symbol values."""
 		self.decimal_context = decimal_context or decimal.getcontext()
 		"""The *decimal_context* parameter from :py:meth:`~__init__`"""
 		if isinstance(type_resolver, collections.abc.Mapping):
 			type_resolver = type_resolver_from_dict(type_resolver)
 		self.__type_resolver = type_resolver or (lambda _: ast.DataType.UNDEFINED)
 		self.__resolver = resolver or resolve_item
 
 	@contextlib.contextmanager
 	def assignments(self, *assignments):
 		"""
 		Add the specified assignments to a thread-specific scope. This is used when an assignment originates from an
 		expression.
 
-		:param assignment: The one or more assignments to define.
-		:type assignment: :py:class:`~rule_engine.ast.Assignment`
+		:param assignments: The one or more assignments to define.
+		:type assignments: :py:class:`~rule_engine.ast.Assignment`
 		"""
 		self._tls.assignment_scopes.append({assign.name: assign for assign in assignments})
 		try:
 			yield
 		finally:
 			self._tls.assignment_scopes.pop()
 
@@ -504,17 +425,17 @@
 		If *name* fails to resolve, this method will raise :py:exc:`~rule_engine.errors.SymbolResolutionError`. It is
 		then up to the caller to determine whether or not it is appropriate to use :py:attr:`.default_value`.
 
 		:param thing: The object from which the *name* item will be accessed.
 		:param str name: The symbol name that is being resolved.
 		:return: The value for the corresponding symbol *name*.
 		"""
-		if scope == Builtins.scope_name:
+		if scope == builtins.Builtins.scope_name:
 			thing = self.builtins
-		if isinstance(thing, Builtins):
+		if isinstance(thing, builtins.Builtins):
 			return resolve_item(thing, name)
 		if scope is None:
 			for assignments in self._tls.assignment_scopes:
 				if name in assignments:
 					return assignments[name].value
 			return self.__resolver(thing, name)
 		raise errors.SymbolResolutionError(name, symbol_scope=scope, thing=thing)
@@ -543,15 +464,15 @@
 		of the compatible data type constants if the symbol is valid or raise an exception. The default behavior is to
 		return :py:data:`~rule_engine.ast.DataType.UNDEFINED` for all symbols.
 
 		:param str name: The symbol name to provide a type hint for.
 		:param str scope: An optional scope name that identifies from where to resolve the name.
 		:return: The type of the specified symbol.
 		"""
-		if scope == Builtins.scope_name:
+		if scope == builtins.Builtins.scope_name:
 			return self.builtins.resolve_type(name)
 		for assignments in self._tls.assignment_scopes:
 			if name in assignments:
 				return assignments[name].value_type
 		return self.__type_resolver(name)
 
 class Rule(object):
```

### Comparing `rule-engine-3.6.0/lib/rule_engine/errors.py` & `rule-engine-4.0.0/lib/rule_engine/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,16 +73,35 @@
 		:param str message: A text description of what error occurred.
 		:param str value: The datetime value which contains the syntax error which caused this exception to be raised.
 		"""
 		super(DatetimeSyntaxError, self).__init__(message)
 		self.value = value
 		"""The datetime value which contains the syntax error which caused this exception to be raised."""
 
+class FloatSyntaxError(SyntaxError):
+	"""
+	An error raised for issues regarding the use of improperly formatted float expressions.
+
+	.. versionadded:: 4.0.0
+	"""
+	def __init__(self, message, value):
+		"""
+		:param str message: A text description of what error occurred.
+		:param str value: The float value which contains the syntax error which caused this exception to be raised.
+		"""
+		super(FloatSyntaxError, self).__init__(message)
+		self.value = value
+		"""The float value which contains the syntax error which caused this exception to be raised."""
+
 class TimedeltaSyntaxError(SyntaxError):
-	"""An error raised for issues regarding the use of improperly formatted timedelta expressions."""
+	"""
+	An error raised for issues regarding the use of improperly formatted timedelta expressions.
+
+	.. versionadded:: 3.5.0
+	"""
 	def __init__(self, message, value):
 		"""
 		:param str message: A text description of what error occurred.
 		:param str value: The timedelta value which contains the syntax error which caused this exception to be raised.
 		"""
 		super(TimedeltaSyntaxError, self).__init__(message)
 		self.value = value
@@ -101,15 +120,15 @@
 		super(RegexSyntaxError, self).__init__(message)
 		self.error = error
 		"""The :py:exc:`re.error` exception from which this error was triggered."""
 		self.value = value
 		"""The regular expression value which contains the syntax error which caused this exception to be raised."""
 
 class RuleSyntaxError(SyntaxError):
-	"""An error raised for issues identified in while parsing the grammar of the rule text."""
+	"""An error raised for issues identified while parsing the grammar of the rule text."""
 	def __init__(self, message, token=None):
 		"""
 		:param str message: A text description of what error occurred.
 		:param token: The PLY token (if available) which is related to the syntax error.
 		"""
 		if token is None:
 			position = 'EOF'
@@ -244,7 +263,19 @@
 		"""The :py:class:`rule-engine type<rule_engine.ast.DataType>` that was expected for this symbol."""
 		message = "symbol {0!r} resolved to incorrect datatype (is: {1}, expected: {2})".format(
 			symbol_name,
 			is_type.name,
 			expected_type.name
 		)
 		super(SymbolTypeError, self).__init__(message)
+
+class FunctionCallError(EvaluationError):
+	"""
+	An error raised when there is an issue calling a function.
+
+	.. versionadded:: 4.0.0
+	"""
+	def __init__(self, message, error=None, function_name=None):
+		super(FunctionCallError, self).__init__(message)
+		self.error = error
+		"""The exception from which this error was triggered."""
+		self.function_name = function_name
```

### Comparing `rule-engine-3.6.0/lib/rule_engine/parser.py` & `rule-engine-4.0.0/lib/rule_engine/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 #  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 import ast as pyast
 import collections
-import re
 import threading
 import types as pytypes
 
 from . import ast
 from . import errors
 from ._utils import timedelta_regex
 
@@ -457,31 +456,21 @@
 		p[0] = _DeferredAstNode(ast.DatetimeExpression, args=(self.context, literal_eval(p[1])), method='from_string')
 
 	def p_expression_timedelta(self, p):
 		'object : TIMEDELTA'
 		p[0] = _DeferredAstNode(ast.TimedeltaExpression, args=(self.context, p[1]), method='from_string')
 
 	def p_expression_float(self, p):
-		'expression : FLOAT'
+		"""
+		expression : FLOAT
+				   | FLOAT_NAN
+				   | FLOAT_INF
+		"""
 		str_val = p[1]
-		if re.match('^0[0-9]', str_val):
-			raise errors.RuleSyntaxError('invalid floating point literal: ' + str_val + ' (leading zeros in decimal literals are not permitted)')
-		try:
-			val = literal_eval(str_val)
-		except SyntaxError:
-			raise errors.RuleSyntaxError('invalid floating point literal: ' + str_val)
-		p[0] = _DeferredAstNode(ast.FloatExpression, args=(self.context, float(val)))
-
-	def p_expression_float_nan(self, p):
-		'expression : FLOAT_NAN'
-		p[0] = _DeferredAstNode(ast.FloatExpression, args=(self.context, float('nan')))
-
-	def p_expression_float_inf(self, p):
-		'expression : FLOAT_INF'
-		p[0] = _DeferredAstNode(ast.FloatExpression, args=(self.context, float('inf')))
+		p[0] = _DeferredAstNode(ast.FloatExpression, args=(self.context, str_val), method='from_string')
 
 	def p_expression_null(self, p):
 		'object : NULL'
 		# null is an object because of the safe operator
 		p[0] = _DeferredAstNode(ast.NullExpression, args=(self.context,))
 
 	def p_expression_set(self, p):
@@ -577,7 +566,21 @@
 		elif colon_index == 3 and len(p) == 6:
 			start, stop = p[3], None
 		elif colon_index == 3 and len(p) == 7:
 			start, _, stop = p[3:6]
 		else:
 			raise errors.RuleSyntaxError('invalid get slice expression')
 		p[0] = _DeferredAstNode(ast.GetSliceExpression, args=(self.context, container, start, stop), kwargs={'safe': safe})
+
+	def p_expression_function_call(self, p):
+		"""
+		object : expression LPAREN RPAREN
+		       | expression LPAREN ary_members RPAREN
+		"""
+		function = p[1]
+		if len(p) == 4:
+			arguments = collections.deque()
+		elif len(p) == 5:
+			arguments = p[3]
+		else:
+			raise errors.RuleSyntaxError('invalid function call expression')
+		p[0] = _DeferredAstNode(ast.FunctionCallExpression, args=(self.context, function, arguments))
```

### Comparing `rule-engine-3.6.0/lib/rule_engine/suggestions.py` & `rule-engine-4.0.0/lib/rule_engine/suggestions.py`

 * *Files identical despite different names*

### Comparing `rule-engine-3.6.0/lib/rule_engine.egg-info/PKG-INFO` & `rule-engine-4.0.0/lib/rule_engine.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 3.6.0
+Version: 4.0.0
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
@@ -16,28 +16,25 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Rule Engine
 ===========
 |badge-build| |badge-pypi|
 
 A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 
 Documentation is available at https://zeroSteiner.github.io/rule-engine/.
 
-:Warning:
-  Version 3.6 is the last to support Python versions 3.4 and 3.5. The next version, either 3.7 or 4.0, will drop them.
-  There is currently no timeline for its release.
-
 Rule Engine expressions are written in their own language, defined as strings in Python. The syntax is most similar to
 Python with some inspiration from Ruby. Some features of this language includes:
 
 - Optional type hinting
 - Matching strings with regular expressions
 - Datetime datatypes
 - Compound datatypes (equivalents for Python dict, list and set types)
```

### Comparing `rule-engine-3.6.0/setup.py` & `rule-engine-4.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 	with open(os.path.join(base_directory, 'README.rst')) as file_h:
 		long_description = file_h.read()
 except OSError:
 	sys.stderr.write('README.rst is unavailable, can not generate the long description\n')
 	long_description = None
 
 with open(os.path.join(base_directory, 'lib', 'rule_engine', '__init__.py')) as file_h:
-	match = re.search(r'^__version__\s*=\s*([\'"])(?P<version>\d+(\.\d)*)\1$', file_h.read(), flags=re.MULTILINE)
+	match = re.search(r'^__version__\s*=\s*([\'"])(?P<version>\d+(\.\d+)*)\1$', file_h.read(), flags=re.MULTILINE)
 if match is None:
 	raise RuntimeError('Unable to find the version information')
 version = match.group('version')
 
 DESCRIPTION = """\
 A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.\
 """
@@ -65,14 +65,15 @@
 	version=version,
 	author='Spencer McIntyre',
 	author_email='zeroSteiner@gmail.com',
 	maintainer='Spencer McIntyre',
 	maintainer_email='zeroSteiner@gmail.com',
 	description=DESCRIPTION,
 	long_description=long_description,
+	long_description_content_type='text/x-rst',
 	url='https://github.com/zeroSteiner/rule-engine',
 	license='BSD',
 	# these are duplicated in requirements.txt
 	install_requires=[
 		'ply>=3.9',
 		'python-dateutil~=2.7'
 	],
@@ -80,16 +81,16 @@
 	packages=find_packages('lib'),
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: Console',
 		'Intended Audience :: Developers',
 		'License :: OSI Approved :: BSD License',
 		'Operating System :: OS Independent',
-		#'Programming Language :: Python :: 3.4',  # dropped in v3.6
-		#'Programming Language :: Python :: 3.5',  # dropped in v3.6
+		#'Programming Language :: Python :: 3.4',  # dropped in v4.0
+		#'Programming Language :: Python :: 3.5',  # dropped in v4.0
 		'Programming Language :: Python :: 3.6',
 		'Programming Language :: Python :: 3.7',
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Topic :: Software Development :: Libraries :: Python Modules'
```

