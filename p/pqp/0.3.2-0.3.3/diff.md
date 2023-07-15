# Comparing `tmp/pqp-0.3.2.tar.gz` & `tmp/pqp-0.3.3.tar.gz`

## Comparing `pqp-0.3.2.tar` & `pqp-0.3.3.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 pqp-0.3.2/Cargo.toml
--rw-r--r--   0      501       20    53248 2023-03-17 07:12:19.000000 pqp-0.3.2/.coverage
--rw-r--r--   0      501       20      105 2023-02-01 03:34:57.000000 pqp-0.3.2/.gitignore
--rw-r--r--   0      501       20      579 2023-02-25 01:53:51.000000 pqp-0.3.2/CHANGELOG.md
--rw-r--r--   0      501       20     1145 2023-02-01 03:55:07.000000 pqp-0.3.2/CONTRIBUTING.md
--rw-r--r--   0      501       20     1047 2023-02-01 03:34:57.000000 pqp-0.3.2/LICENSE.txt
--rw-r--r--   0      501       20     1292 2023-06-24 06:06:14.000000 pqp-0.3.2/README.md
--rw-r--r--   0      501       20      333 2023-02-01 03:34:57.000000 pqp-0.3.2/publish_docs.sh
--rw-r--r--   0      501       20      827 2023-06-24 06:07:11.000000 pqp-0.3.2/pyproject.toml
--rw-r--r--   0      501       20       38 2023-03-01 09:39:53.000000 pqp-0.3.2/python/.gitignore
--rw-r--r--   0      501       20        0 2023-02-01 03:34:57.000000 pqp-0.3.2/python/conftest.py
--rw-r--r--   0      501       20       12 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/.gitignore
--rw-r--r--   0      501       20      850 2023-03-31 02:19:59.000000 pqp-0.3.2/python/docs/Makefile
--rw-r--r--   0      501       20      804 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/make.bat
--rw-r--r--   0      501       20      280 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.BinaryDomain.rst
--rw-r--r--   0      501       20      442 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.CategoricalDomain.rst
--rw-r--r--   0      501       20      286 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.ContinuousDomain.rst
--rw-r--r--   0      501       20      412 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.Data.rst
--rw-r--r--   0      501       20      268 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.DiscreteDomain.rst
--rw-r--r--   0      501       20      441 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.Domain.rst
--rw-r--r--   0      501       20      478 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.IntegerDomain.rst
--rw-r--r--   0      501       20      272 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.RealDomain.rst
--rw-r--r--   0      501       20      102 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.infer_domain_type.rst
--rw-r--r--   0      501       20       84 2023-03-31 02:41:09.000000 pqp-0.3.2/python/docs/source/api/pqp.data.make_domain.rst
--rw-r--r--   0      501       20      279 2023-03-31 03:04:18.000000 pqp-0.3.2/python/docs/source/api/pqp.estimation.EstimationResult.rst
--rw-r--r--   0      501       20      764 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.estimation.Estimator.rst
--rw-r--r--   0      501       20      973 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst
--rw-r--r--   0      501       20      307 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.expression.Expression.rst
--rw-r--r--   0      501       20      234 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.expression.Hedge.rst
--rw-r--r--   0      501       20      246 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.expression.Marginal.rst
--rw-r--r--   0      501       20      218 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.expression.P.rst
--rw-r--r--   0      501       20      242 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.expression.Product.rst
--rw-r--r--   0      501       20      246 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.expression.Quotient.rst
--rw-r--r--   0      501       20       87 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.expression.parse_json.rst
--rw-r--r--   0      501       20      113 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.graph.BidirectedEdge.rst
--rw-r--r--   0      501       20      107 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.graph.DirectedEdge.rst
--rw-r--r--   0      501       20      435 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.graph.Graph.rst
--rw-r--r--   0      501       20      294 2023-03-31 04:09:43.000000 pqp-0.3.2/python/docs/source/api/pqp.identification.ATE.rst
--rw-r--r--   0      501       20      310 2023-03-31 04:09:43.000000 pqp-0.3.2/python/docs/source/api/pqp.identification.AbstractCausalEstimand.rst
--rw-r--r--   0      501       20      122 2023-03-31 04:09:43.000000 pqp-0.3.2/python/docs/source/api/pqp.identification.BidirectedEdge.rst
--rw-r--r--   0      501       20      295 2023-03-31 04:09:43.000000 pqp-0.3.2/python/docs/source/api/pqp.identification.CATE.rst
--rw-r--r--   0      501       20      278 2023-03-31 04:09:43.000000 pqp-0.3.2/python/docs/source/api/pqp.identification.CausalEstimand.rst
--rw-r--r--   0      501       20      116 2023-03-31 04:09:43.000000 pqp-0.3.2/python/docs/source/api/pqp.identification.DirectedEdge.rst
--rw-r--r--   0      501       20      624 2023-03-31 04:09:43.000000 pqp-0.3.2/python/docs/source/api/pqp.identification.Graph.rst
--rw-r--r--   0      501       20      140 2023-03-31 04:09:43.000000 pqp-0.3.2/python/docs/source/api/pqp.identification.IdentificationResult.rst
--rw-r--r--   0      501       20      103 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.refutation.Operation.rst
--rw-r--r--   0      501       20      586 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.refutation.Result.rst
--rw-r--r--   0      501       20      408 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.refutation.Step.rst
--rw-r--r--   0      501       20       87 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.refutation.entrypoint.rst
--rw-r--r--   0      501       20      730 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.AbstractExpression.rst
--rw-r--r--   0      501       20      314 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.AbstractMath.rst
--rw-r--r--   0      501       20      522 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Difference.rst
--rw-r--r--   0      501       20      319 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.EqualityEvent.rst
--rw-r--r--   0      501       20      238 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Event.rst
--rw-r--r--   0      501       20      531 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Expectation.rst
--rw-r--r--   0      501       20      435 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Hedge.rst
--rw-r--r--   0      501       20      397 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.InterventionEvent.rst
--rw-r--r--   0      501       20      504 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Marginal.rst
--rw-r--r--   0      501       20      777 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.P.rst
--rw-r--r--   0      501       20      495 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Product.rst
--rw-r--r--   0      501       20      504 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Quotient.rst
--rw-r--r--   0      501       20      121 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.StatisticalEvent.rst
--rw-r--r--   0      501       20      477 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Value.rst
--rw-r--r--   0      501       20      243 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.Variable.rst
--rw-r--r--   0      501       20       60 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.do.rst
--rw-r--r--   0      501       20       81 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.make_vars.rst
--rw-r--r--   0      501       20       84 2023-03-31 02:27:30.000000 pqp-0.3.2/python/docs/source/api/pqp.symbols.parse_json.rst
--rw-r--r--   0      501       20       95 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.attrdict.rst
--rw-r--r--   0      501       20      127 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.exceptions.DomainValidationError.rst
--rw-r--r--   0      501       20      127 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.exceptions.InferredDomainWarning.rst
--rw-r--r--   0      501       20      106 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.exceptions.NumericalError.rst
--rw-r--r--   0      501       20      121 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.exceptions.PositivityException.rst
--rw-r--r--   0      501       20      115 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.exceptions.UnitDomainWarning.rst
--rw-r--r--   0      501       20       85 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.order_graph.rst
--rw-r--r--   0      501       20       94 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.recursive_sort.rst
--rw-r--r--   0      501       20      113 2023-03-31 02:27:29.000000 pqp-0.3.2/python/docs/source/api/pqp.utils.staticproperty.rst
--rw-r--r--   0      501       20      244 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.variable.Variable.rst
--rw-r--r--   0      501       20       82 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/api/pqp.variable.make_vars.rst
--rw-r--r--   0      501       20     1483 2023-02-01 04:08:19.000000 pqp-0.3.2/python/docs/source/conf.py
--rw-r--r--   0      501       20       42 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/example_notebooks.rst
--rw-r--r--   0      501       20   238718 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/favicon.ico
--rw-r--r--   0      501       20    19314 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/imgs/frontdoor_estimator.png
--rw-r--r--   0      501       20    18477 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/imgs/frontdoor_new.png
--rw-r--r--   0      501       20    97789 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/imgs/frontdoor_viz.png
--rw-r--r--   0      501       20    37703 2023-03-31 05:48:21.000000 pqp-0.3.2/python/docs/source/imgs/qs_causal_estimand.png
--rw-r--r--   0      501       20    75030 2023-03-31 05:55:41.000000 pqp-0.3.2/python/docs/source/imgs/qs_stat_estimand.png
--rw-r--r--   0      501       20      809 2023-03-31 06:13:18.000000 pqp-0.3.2/python/docs/source/index.rst
--rw-r--r--   0      501       20       24 2023-03-31 02:39:47.000000 pqp-0.3.2/python/docs/source/module_maps/data.rst
--rw-r--r--   0      501       20       30 2023-03-31 02:21:59.000000 pqp-0.3.2/python/docs/source/module_maps/estimation.rst
--rw-r--r--   0      501       20       36 2023-03-31 02:28:16.000000 pqp-0.3.2/python/docs/source/module_maps/exceptions.rst
--rw-r--r--   0      501       20       34 2023-03-31 02:22:26.000000 pqp-0.3.2/python/docs/source/module_maps/identification.rst
--rw-r--r--   0      501       20       30 2023-03-31 02:23:26.000000 pqp-0.3.2/python/docs/source/module_maps/refutation.rst
--rw-r--r--   0      501       20       27 2023-03-31 02:22:32.000000 pqp-0.3.2/python/docs/source/module_maps/symbols.rst
--rw-r--r--   0      501       20       46 2023-02-01 03:34:57.000000 pqp-0.3.2/python/docs/source/modules.rst
--rw-r--r--   0      501       20      432 2023-03-31 02:20:15.000000 pqp-0.3.2/python/docs/source/pqp.data.rst
--rw-r--r--   0      501       20      548 2023-03-31 02:20:15.000000 pqp-0.3.2/python/docs/source/pqp.estimation.rst
--rw-r--r--   0      501       20      534 2023-03-31 02:20:15.000000 pqp-0.3.2/python/docs/source/pqp.identification.rst
--rw-r--r--   0      501       20      340 2023-03-31 02:20:15.000000 pqp-0.3.2/python/docs/source/pqp.refutation.rst
--rw-r--r--   0      501       20      419 2023-03-31 02:20:15.000000 pqp-0.3.2/python/docs/source/pqp.rst
--rw-r--r--   0      501       20     1051 2023-03-31 02:20:16.000000 pqp-0.3.2/python/docs/source/pqp.symbols.rst
--rw-r--r--   0      501       20      456 2023-03-31 02:20:16.000000 pqp-0.3.2/python/docs/source/pqp.utils.rst
--rw-r--r--   0      501       20     6082 2023-04-01 02:03:49.000000 pqp-0.3.2/python/docs/source/quickstart.rst
--rw-r--r--   0      501       20   117134 2023-06-24 06:07:14.000000 pqp-0.3.2/python/fd_case_study.ipynb
--rw-r--r--   0      501       20       16 2023-02-01 03:34:57.000000 pqp-0.3.2/python/pqp/.gitignore
--rw-r--r--   0      501       20      269 2023-06-22 21:46:02.000000 pqp-0.3.2/python/pqp/__init__.py
--rw-r--r--   0      501       20       60 2023-03-31 02:50:56.000000 pqp-0.3.2/python/pqp/data/__init__.py
--rw-r--r--   0      501       20     7569 2023-04-01 11:23:18.000000 pqp-0.3.2/python/pqp/data/data.py
--rw-r--r--   0      501       20     8507 2023-04-01 07:52:26.000000 pqp-0.3.2/python/pqp/data/domain.py
--rw-r--r--   0      501       20      135 2023-03-31 03:00:34.000000 pqp-0.3.2/python/pqp/estimation/__init__.py
--rw-r--r--   0      501       20     4072 2023-04-01 08:03:10.000000 pqp-0.3.2/python/pqp/estimation/estimator.py
--rw-r--r--   0      501       20     8925 2023-04-01 07:57:47.000000 pqp-0.3.2/python/pqp/estimation/multinomial_estimator.py
--rw-r--r--   0      501       20      589 2023-06-22 22:02:47.000000 pqp-0.3.2/python/pqp/fd_demo.py
--rw-r--r--   0      501       20      186 2023-03-31 04:17:25.000000 pqp-0.3.2/python/pqp/identification/__init__.py
--rw-r--r--   0      501       20     8977 2023-06-23 20:53:27.000000 pqp-0.3.2/python/pqp/identification/estimands.py
--rw-r--r--   0      501       20    13147 2023-06-23 16:55:29.000000 pqp-0.3.2/python/pqp/identification/graph.py
--rw-r--r--   0      501       20     2388 2023-03-31 01:56:15.000000 pqp-0.3.2/python/pqp/refutation/__init__.py
--rw-r--r--   0      501       20     6271 2023-06-23 16:52:32.000000 pqp-0.3.2/python/pqp/refutation/result.py
--rw-r--r--   0      501       20      241 2023-03-31 04:12:37.000000 pqp-0.3.2/python/pqp/symbols/__init__.py
--rw-r--r--   0      501       20      396 2023-03-18 07:10:53.000000 pqp-0.3.2/python/pqp/symbols/abstract_math.py
--rw-r--r--   0      501       20     3018 2023-03-31 04:16:19.000000 pqp-0.3.2/python/pqp/symbols/event.py
--rw-r--r--   0      501       20     7580 2023-03-25 09:26:26.000000 pqp-0.3.2/python/pqp/symbols/p.py
--rw-r--r--   0      501       20     1126 2023-03-23 04:31:01.000000 pqp-0.3.2/python/pqp/symbols/parse.py
--rw-r--r--   0      501       20    20412 2023-06-23 21:46:53.000000 pqp-0.3.2/python/pqp/symbols/relation.py
--rw-r--r--   0      501       20     4317 2023-06-23 20:46:28.000000 pqp-0.3.2/python/pqp/symbols/variable.py
--rw-r--r--   0      501       20       29 2023-03-23 02:58:35.000000 pqp-0.3.2/python/pqp/utils/__init__.py
--rw-r--r--   0      501       20      683 2023-03-25 06:45:09.000000 pqp-0.3.2/python/pqp/utils/exceptions.py
--rw-r--r--   0      501       20     1473 2023-03-28 09:15:44.000000 pqp-0.3.2/python/pqp/utils/utils.py
--rw-r--r--   0      501       20       11 2023-02-01 03:34:57.000000 pqp-0.3.2/python/tests/.gitignore
--rw-r--r--   0      501       20      552 2023-03-26 06:08:17.000000 pqp-0.3.2/python/tests/test_abstract_step.py
--rw-r--r--   0      501       20      966 2023-06-23 20:52:53.000000 pqp-0.3.2/python/tests/test_causal_estimand.py
--rw-r--r--   0      501       20     3021 2023-03-28 07:26:00.000000 pqp-0.3.2/python/tests/test_data.py
--rw-r--r--   0      501       20     1690 2023-03-25 03:20:40.000000 pqp-0.3.2/python/tests/test_domain.py
--rw-r--r--   0      501       20      228 2023-03-23 04:38:36.000000 pqp-0.3.2/python/tests/test_event.py
--rw-r--r--   0      501       20     6346 2023-04-01 08:45:57.000000 pqp-0.3.2/python/tests/test_examples.py
--rw-r--r--   0      501       20     2280 2023-06-23 16:10:10.000000 pqp-0.3.2/python/tests/test_graph.py
--rw-r--r--   0      501       20     1538 2023-03-28 06:40:11.000000 pqp-0.3.2/python/tests/test_id.py
--rw-r--r--   0      501       20     7724 2023-04-01 04:27:39.000000 pqp-0.3.2/python/tests/test_multinomial_estimator.py
--rw-r--r--   0      501       20     2413 2023-03-25 05:57:51.000000 pqp-0.3.2/python/tests/test_p.py
--rw-r--r--   0      501       20      832 2023-03-31 01:59:17.000000 pqp-0.3.2/python/tests/test_refutation.py
--rw-r--r--   0      501       20     3032 2023-06-23 19:24:57.000000 pqp-0.3.2/python/tests/test_relation.py
--rw-r--r--   0      501       20      550 2023-03-28 09:16:20.000000 pqp-0.3.2/python/tests/test_utils.py
--rw-r--r--   0      501       20     1040 2023-06-23 20:00:53.000000 pqp-0.3.2/python/tests/test_variable.py
--rw-r--r--   0      501       20       74 2023-04-01 08:30:11.000000 pqp-0.3.2/requirements.txt
--rw-r--r--   0      501       20      574 2023-02-01 03:34:57.000000 pqp-0.3.2/src/api/functions.rs
--rw-r--r--   0      501       20       58 2023-02-25 00:17:24.000000 pqp-0.3.2/src/api/mod.rs
--rw-r--r--   0      501       20      651 2023-02-01 03:34:57.000000 pqp-0.3.2/src/api/python.rs
--rw-r--r--   0      501       20     1364 2023-02-01 03:34:57.000000 pqp-0.3.2/src/api/test.rs
--rw-r--r--   0      501       20     5453 2023-04-01 08:49:23.000000 pqp-0.3.2/src/api/wrapper.rs
--rw-r--r--   0      501       20     9318 2023-06-22 18:22:01.000000 pqp-0.3.2/src/form/form.rs
--rw-r--r--   0      501       20      129 2023-02-01 03:34:57.000000 pqp-0.3.2/src/form/mod.rs
--rw-r--r--   0      501       20     5218 2023-02-01 03:34:57.000000 pqp-0.3.2/src/form/simplify.rs
--rw-r--r--   0      501       20     4151 2023-06-22 18:25:20.000000 pqp-0.3.2/src/form/test_form.rs
--rw-r--r--   0      501       20     6687 2023-02-01 03:34:57.000000 pqp-0.3.2/src/form/test_simplify.rs
--rw-r--r--   0      501       20     3459 2023-02-01 03:34:57.000000 pqp-0.3.2/src/form/tikka.rs
--rw-r--r--   0      501       20     2552 2023-02-24 11:35:34.000000 pqp-0.3.2/src/graph/bigraph.rs
--rw-r--r--   0      501       20     4865 2023-02-24 11:35:34.000000 pqp-0.3.2/src/graph/digraph.rs
--rw-r--r--   0      501       20      303 2023-02-24 11:35:34.000000 pqp-0.3.2/src/graph/graph.rs
--rw-r--r--   0      501       20     2075 2023-02-24 11:35:34.000000 pqp-0.3.2/src/graph/graph_builder.rs
--rw-r--r--   0      501       20      296 2023-06-22 19:37:08.000000 pqp-0.3.2/src/graph/mod.rs
--rw-r--r--   0      501       20      373 2023-06-22 21:00:19.000000 pqp-0.3.2/src/graph/node.rs
--rw-r--r--   0      501       20     5763 2023-02-01 03:34:57.000000 pqp-0.3.2/src/graph/tests.rs
--rw-r--r--   0      501       20       64 2023-02-25 00:14:14.000000 pqp-0.3.2/src/identification/mod.rs
--rw-r--r--   0      501       20     3689 2023-02-25 00:13:29.000000 pqp-0.3.2/src/identification/shpitser.rs
--rw-r--r--   0      501       20     6682 2023-06-22 18:22:08.000000 pqp-0.3.2/src/identification/tests.rs
--rw-r--r--   0      501       20      154 2023-02-24 11:35:34.000000 pqp-0.3.2/src/lib.rs
--rw-r--r--   0      501       20      368 2023-02-01 03:34:57.000000 pqp-0.3.2/src/model/examples.rs
--rw-r--r--   0      501       20       93 2023-06-22 21:01:19.000000 pqp-0.3.2/src/model/mod.rs
--rw-r--r--   0      501       20     6195 2023-06-22 18:44:17.000000 pqp-0.3.2/src/model/model.rs
--rw-r--r--   0      501       20     2565 2023-02-01 03:34:57.000000 pqp-0.3.2/src/model/order.rs
--rw-r--r--   0      501       20     4253 2023-06-22 21:01:26.000000 pqp-0.3.2/src/model/tests.rs
--rw-r--r--   0      501       20      795 2023-06-22 21:01:57.000000 pqp-0.3.2/src/test.rs
--rw-r--r--   0      501       20      304 2023-02-01 03:34:57.000000 pqp-0.3.2/src/utils/defaults.rs
--rw-r--r--   0      501       20       99 2023-02-24 11:35:34.000000 pqp-0.3.2/src/utils/mod.rs
--rw-r--r--   0      501       20     2185 2023-02-01 03:34:57.000000 pqp-0.3.2/src/utils/set_utils.rs
--rw-r--r--   0      501       20      987 2023-02-01 03:34:57.000000 pqp-0.3.2/src/utils/tests.rs
--rw-r--r--   0      501       20      612 2023-02-24 11:35:34.000000 pqp-0.3.2/src/utils/utils.rs
--rw-r--r--   0      501       20       49 2023-02-01 03:34:57.000000 pqp-0.3.2/test.sh
--rw-r--r--   0      501       20   150084 2023-02-01 03:34:57.000000 pqp-0.3.2/writeup/2023-01-14-13-06-10.png
--rw-r--r--   0      501       20    51282 2023-02-01 03:34:57.000000 pqp-0.3.2/writeup/2023-01-14-13-52-24.png
--rw-r--r--   0      501       20    53166 2023-02-01 03:34:57.000000 pqp-0.3.2/writeup/2023-01-14-14-22-06.png
--rw-r--r--   0      501       20   118082 2023-02-01 03:34:57.000000 pqp-0.3.2/writeup/2023-01-14-15-01-52.png
--rw-r--r--   0      501       20    45879 2023-02-25 02:07:37.000000 pqp-0.3.2/writeup/2023-02-25-09-07-36.png
--rw-r--r--   0      501       20    50872 2023-02-25 02:22:50.000000 pqp-0.3.2/writeup/2023-02-25-09-22-50.png
--rw-r--r--   0      501       20   367476 2023-04-02 04:33:16.000000 pqp-0.3.2/writeup/2023-04-02-14-33-14.png
--rw-r--r--   0      501       20   325115 2023-04-02 04:33:45.000000 pqp-0.3.2/writeup/2023-04-02-14-33-44.png
--rw-r--r--   0      501       20   213508 2023-04-02 04:34:20.000000 pqp-0.3.2/writeup/2023-04-02-14-34-19.png
--rw-r--r--   0      501       20   336724 2023-04-02 04:34:31.000000 pqp-0.3.2/writeup/2023-04-02-14-34-30.png
--rw-r--r--   0      501       20   349974 2023-04-02 04:34:45.000000 pqp-0.3.2/writeup/2023-04-02-14-34-44.png
--rw-r--r--   0      501       20   407521 2023-04-02 04:35:40.000000 pqp-0.3.2/writeup/2023-04-02-14-35-39.png
--rw-r--r--   0      501       20   115292 2023-04-02 04:36:00.000000 pqp-0.3.2/writeup/2023-04-02-14-36-00.png
--rw-r--r--   0      501       20   476032 2023-04-02 04:36:59.000000 pqp-0.3.2/writeup/2023-04-02-14-36-57.png
--rw-r--r--   0      501       20   345389 2023-04-02 04:37:11.000000 pqp-0.3.2/writeup/2023-04-02-14-37-10.png
--rw-r--r--   0      501       20   108822 2023-04-02 04:47:11.000000 pqp-0.3.2/writeup/PQP a Library for End-to-End Causal Inference.ipynb
--rw-r--r--   0      501       20   197652 2023-04-01 03:17:51.000000 pqp-0.3.2/writeup/PQP.ipynb
--rw-r--r--   0      501       20   117397 2023-04-01 03:17:56.000000 pqp-0.3.2/writeup/agg.ipynb
--rw-r--r--   0      501       20      882 2023-02-25 16:01:13.000000 pqp-0.3.2/writeup/build.py
--rw-r--r--   0      501       20    16499 2023-03-11 07:28:34.000000 pqp-0.3.2/writeup/demo.ipynb
--rw-r--r--   0      501       20     8008 2023-04-02 04:40:20.000000 pqp-0.3.2/writeup/demo1.csv
--rw-r--r--   0      501       20    27322 2023-04-01 12:35:30.000000 pqp-0.3.2/writeup/doctordemo.csv
--rw-r--r--   0      501       20    14520 2023-06-22 21:23:55.000000 pqp-0.3.2/writeup/examples.ipynb
--rw-r--r--   0      501       20     1756 2023-02-25 15:09:55.000000 pqp-0.3.2/writeup/grab_code.py
--rw-r--r--   0      501       20     6485 2023-04-03 04:52:12.000000 pqp-0.3.2/writeup/speed.ipynb
--rw-r--r--   0      501       20      678 2023-04-01 03:08:56.000000 pqp-0.3.2/writeup/supplement.py
--rw-r--r--   0      501       20     9185 2023-02-24 11:35:34.000000 pqp-0.3.2/Cargo.lock
--rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 pqp-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 pqp-0.3.3/Cargo.toml
+-rw-r--r--   0      501       20    53248 2023-03-17 07:12:19.000000 pqp-0.3.3/.coverage
+-rw-r--r--   0      501       20      105 2023-02-01 03:34:57.000000 pqp-0.3.3/.gitignore
+-rw-r--r--   0      501       20      579 2023-02-25 01:53:51.000000 pqp-0.3.3/CHANGELOG.md
+-rw-r--r--   0      501       20     1145 2023-02-01 03:55:07.000000 pqp-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0      501       20     1047 2023-02-01 03:34:57.000000 pqp-0.3.3/LICENSE.txt
+-rw-r--r--   0      501       20     1292 2023-06-24 06:06:14.000000 pqp-0.3.3/README.md
+-rw-r--r--   0      501       20      333 2023-02-01 03:34:57.000000 pqp-0.3.3/publish_docs.sh
+-rw-r--r--   0      501       20      826 2023-06-24 06:08:54.000000 pqp-0.3.3/pyproject.toml
+-rw-r--r--   0      501       20       38 2023-03-01 09:39:53.000000 pqp-0.3.3/python/.gitignore
+-rw-r--r--   0      501       20        0 2023-02-01 03:34:57.000000 pqp-0.3.3/python/conftest.py
+-rw-r--r--   0      501       20       12 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/.gitignore
+-rw-r--r--   0      501       20      850 2023-03-31 02:19:59.000000 pqp-0.3.3/python/docs/Makefile
+-rw-r--r--   0      501       20      804 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/make.bat
+-rw-r--r--   0      501       20      280 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.BinaryDomain.rst
+-rw-r--r--   0      501       20      442 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.CategoricalDomain.rst
+-rw-r--r--   0      501       20      286 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.ContinuousDomain.rst
+-rw-r--r--   0      501       20      412 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.Data.rst
+-rw-r--r--   0      501       20      268 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.DiscreteDomain.rst
+-rw-r--r--   0      501       20      441 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.Domain.rst
+-rw-r--r--   0      501       20      478 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.IntegerDomain.rst
+-rw-r--r--   0      501       20      272 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.RealDomain.rst
+-rw-r--r--   0      501       20      102 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.infer_domain_type.rst
+-rw-r--r--   0      501       20       84 2023-03-31 02:41:09.000000 pqp-0.3.3/python/docs/source/api/pqp.data.make_domain.rst
+-rw-r--r--   0      501       20      279 2023-03-31 03:04:18.000000 pqp-0.3.3/python/docs/source/api/pqp.estimation.EstimationResult.rst
+-rw-r--r--   0      501       20      764 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.estimation.Estimator.rst
+-rw-r--r--   0      501       20      973 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst
+-rw-r--r--   0      501       20      307 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.expression.Expression.rst
+-rw-r--r--   0      501       20      234 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.expression.Hedge.rst
+-rw-r--r--   0      501       20      246 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.expression.Marginal.rst
+-rw-r--r--   0      501       20      218 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.expression.P.rst
+-rw-r--r--   0      501       20      242 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.expression.Product.rst
+-rw-r--r--   0      501       20      246 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.expression.Quotient.rst
+-rw-r--r--   0      501       20       87 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.expression.parse_json.rst
+-rw-r--r--   0      501       20      113 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.graph.BidirectedEdge.rst
+-rw-r--r--   0      501       20      107 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.graph.DirectedEdge.rst
+-rw-r--r--   0      501       20      435 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.graph.Graph.rst
+-rw-r--r--   0      501       20      294 2023-03-31 04:09:43.000000 pqp-0.3.3/python/docs/source/api/pqp.identification.ATE.rst
+-rw-r--r--   0      501       20      310 2023-03-31 04:09:43.000000 pqp-0.3.3/python/docs/source/api/pqp.identification.AbstractCausalEstimand.rst
+-rw-r--r--   0      501       20      122 2023-03-31 04:09:43.000000 pqp-0.3.3/python/docs/source/api/pqp.identification.BidirectedEdge.rst
+-rw-r--r--   0      501       20      295 2023-03-31 04:09:43.000000 pqp-0.3.3/python/docs/source/api/pqp.identification.CATE.rst
+-rw-r--r--   0      501       20      278 2023-03-31 04:09:43.000000 pqp-0.3.3/python/docs/source/api/pqp.identification.CausalEstimand.rst
+-rw-r--r--   0      501       20      116 2023-03-31 04:09:43.000000 pqp-0.3.3/python/docs/source/api/pqp.identification.DirectedEdge.rst
+-rw-r--r--   0      501       20      624 2023-03-31 04:09:43.000000 pqp-0.3.3/python/docs/source/api/pqp.identification.Graph.rst
+-rw-r--r--   0      501       20      140 2023-03-31 04:09:43.000000 pqp-0.3.3/python/docs/source/api/pqp.identification.IdentificationResult.rst
+-rw-r--r--   0      501       20      103 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.refutation.Operation.rst
+-rw-r--r--   0      501       20      586 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.refutation.Result.rst
+-rw-r--r--   0      501       20      408 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.refutation.Step.rst
+-rw-r--r--   0      501       20       87 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.refutation.entrypoint.rst
+-rw-r--r--   0      501       20      730 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.AbstractExpression.rst
+-rw-r--r--   0      501       20      314 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.AbstractMath.rst
+-rw-r--r--   0      501       20      522 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Difference.rst
+-rw-r--r--   0      501       20      319 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.EqualityEvent.rst
+-rw-r--r--   0      501       20      238 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Event.rst
+-rw-r--r--   0      501       20      531 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Expectation.rst
+-rw-r--r--   0      501       20      435 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Hedge.rst
+-rw-r--r--   0      501       20      397 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.InterventionEvent.rst
+-rw-r--r--   0      501       20      504 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Marginal.rst
+-rw-r--r--   0      501       20      777 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.P.rst
+-rw-r--r--   0      501       20      495 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Product.rst
+-rw-r--r--   0      501       20      504 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Quotient.rst
+-rw-r--r--   0      501       20      121 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.StatisticalEvent.rst
+-rw-r--r--   0      501       20      477 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Value.rst
+-rw-r--r--   0      501       20      243 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.Variable.rst
+-rw-r--r--   0      501       20       60 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.do.rst
+-rw-r--r--   0      501       20       81 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.make_vars.rst
+-rw-r--r--   0      501       20       84 2023-03-31 02:27:30.000000 pqp-0.3.3/python/docs/source/api/pqp.symbols.parse_json.rst
+-rw-r--r--   0      501       20       95 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.attrdict.rst
+-rw-r--r--   0      501       20      127 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.exceptions.DomainValidationError.rst
+-rw-r--r--   0      501       20      127 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.exceptions.InferredDomainWarning.rst
+-rw-r--r--   0      501       20      106 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.exceptions.NumericalError.rst
+-rw-r--r--   0      501       20      121 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.exceptions.PositivityException.rst
+-rw-r--r--   0      501       20      115 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.exceptions.UnitDomainWarning.rst
+-rw-r--r--   0      501       20       85 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.order_graph.rst
+-rw-r--r--   0      501       20       94 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.recursive_sort.rst
+-rw-r--r--   0      501       20      113 2023-03-31 02:27:29.000000 pqp-0.3.3/python/docs/source/api/pqp.utils.staticproperty.rst
+-rw-r--r--   0      501       20      244 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.variable.Variable.rst
+-rw-r--r--   0      501       20       82 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/api/pqp.variable.make_vars.rst
+-rw-r--r--   0      501       20     1483 2023-02-01 04:08:19.000000 pqp-0.3.3/python/docs/source/conf.py
+-rw-r--r--   0      501       20       42 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/example_notebooks.rst
+-rw-r--r--   0      501       20   238718 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/favicon.ico
+-rw-r--r--   0      501       20    19314 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/imgs/frontdoor_estimator.png
+-rw-r--r--   0      501       20    18477 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/imgs/frontdoor_new.png
+-rw-r--r--   0      501       20    97789 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/imgs/frontdoor_viz.png
+-rw-r--r--   0      501       20    37703 2023-03-31 05:48:21.000000 pqp-0.3.3/python/docs/source/imgs/qs_causal_estimand.png
+-rw-r--r--   0      501       20    75030 2023-03-31 05:55:41.000000 pqp-0.3.3/python/docs/source/imgs/qs_stat_estimand.png
+-rw-r--r--   0      501       20      809 2023-03-31 06:13:18.000000 pqp-0.3.3/python/docs/source/index.rst
+-rw-r--r--   0      501       20       24 2023-03-31 02:39:47.000000 pqp-0.3.3/python/docs/source/module_maps/data.rst
+-rw-r--r--   0      501       20       30 2023-03-31 02:21:59.000000 pqp-0.3.3/python/docs/source/module_maps/estimation.rst
+-rw-r--r--   0      501       20       36 2023-03-31 02:28:16.000000 pqp-0.3.3/python/docs/source/module_maps/exceptions.rst
+-rw-r--r--   0      501       20       34 2023-03-31 02:22:26.000000 pqp-0.3.3/python/docs/source/module_maps/identification.rst
+-rw-r--r--   0      501       20       30 2023-03-31 02:23:26.000000 pqp-0.3.3/python/docs/source/module_maps/refutation.rst
+-rw-r--r--   0      501       20       27 2023-03-31 02:22:32.000000 pqp-0.3.3/python/docs/source/module_maps/symbols.rst
+-rw-r--r--   0      501       20       46 2023-02-01 03:34:57.000000 pqp-0.3.3/python/docs/source/modules.rst
+-rw-r--r--   0      501       20      432 2023-03-31 02:20:15.000000 pqp-0.3.3/python/docs/source/pqp.data.rst
+-rw-r--r--   0      501       20      548 2023-03-31 02:20:15.000000 pqp-0.3.3/python/docs/source/pqp.estimation.rst
+-rw-r--r--   0      501       20      534 2023-03-31 02:20:15.000000 pqp-0.3.3/python/docs/source/pqp.identification.rst
+-rw-r--r--   0      501       20      340 2023-03-31 02:20:15.000000 pqp-0.3.3/python/docs/source/pqp.refutation.rst
+-rw-r--r--   0      501       20      419 2023-03-31 02:20:15.000000 pqp-0.3.3/python/docs/source/pqp.rst
+-rw-r--r--   0      501       20     1051 2023-03-31 02:20:16.000000 pqp-0.3.3/python/docs/source/pqp.symbols.rst
+-rw-r--r--   0      501       20      456 2023-03-31 02:20:16.000000 pqp-0.3.3/python/docs/source/pqp.utils.rst
+-rw-r--r--   0      501       20     6082 2023-04-01 02:03:49.000000 pqp-0.3.3/python/docs/source/quickstart.rst
+-rw-r--r--   0      501       20   117134 2023-06-24 06:07:14.000000 pqp-0.3.3/python/fd_case_study.ipynb
+-rw-r--r--   0      501       20       16 2023-02-01 03:34:57.000000 pqp-0.3.3/python/pqp/.gitignore
+-rw-r--r--   0      501       20      269 2023-06-22 21:46:02.000000 pqp-0.3.3/python/pqp/__init__.py
+-rw-r--r--   0      501       20       60 2023-03-31 02:50:56.000000 pqp-0.3.3/python/pqp/data/__init__.py
+-rw-r--r--   0      501       20     7569 2023-04-01 11:23:18.000000 pqp-0.3.3/python/pqp/data/data.py
+-rw-r--r--   0      501       20     8507 2023-04-01 07:52:26.000000 pqp-0.3.3/python/pqp/data/domain.py
+-rw-r--r--   0      501       20      135 2023-03-31 03:00:34.000000 pqp-0.3.3/python/pqp/estimation/__init__.py
+-rw-r--r--   0      501       20     4072 2023-04-01 08:03:10.000000 pqp-0.3.3/python/pqp/estimation/estimator.py
+-rw-r--r--   0      501       20     8925 2023-04-01 07:57:47.000000 pqp-0.3.3/python/pqp/estimation/multinomial_estimator.py
+-rw-r--r--   0      501       20      589 2023-06-22 22:02:47.000000 pqp-0.3.3/python/pqp/fd_demo.py
+-rw-r--r--   0      501       20      186 2023-03-31 04:17:25.000000 pqp-0.3.3/python/pqp/identification/__init__.py
+-rw-r--r--   0      501       20     8977 2023-06-23 20:53:27.000000 pqp-0.3.3/python/pqp/identification/estimands.py
+-rw-r--r--   0      501       20    13147 2023-06-23 16:55:29.000000 pqp-0.3.3/python/pqp/identification/graph.py
+-rw-r--r--   0      501       20     2388 2023-03-31 01:56:15.000000 pqp-0.3.3/python/pqp/refutation/__init__.py
+-rw-r--r--   0      501       20     6271 2023-06-23 16:52:32.000000 pqp-0.3.3/python/pqp/refutation/result.py
+-rw-r--r--   0      501       20      241 2023-03-31 04:12:37.000000 pqp-0.3.3/python/pqp/symbols/__init__.py
+-rw-r--r--   0      501       20      396 2023-03-18 07:10:53.000000 pqp-0.3.3/python/pqp/symbols/abstract_math.py
+-rw-r--r--   0      501       20     3018 2023-03-31 04:16:19.000000 pqp-0.3.3/python/pqp/symbols/event.py
+-rw-r--r--   0      501       20     7580 2023-03-25 09:26:26.000000 pqp-0.3.3/python/pqp/symbols/p.py
+-rw-r--r--   0      501       20     1126 2023-03-23 04:31:01.000000 pqp-0.3.3/python/pqp/symbols/parse.py
+-rw-r--r--   0      501       20    20412 2023-06-23 21:46:53.000000 pqp-0.3.3/python/pqp/symbols/relation.py
+-rw-r--r--   0      501       20     4317 2023-06-23 20:46:28.000000 pqp-0.3.3/python/pqp/symbols/variable.py
+-rw-r--r--   0      501       20       29 2023-03-23 02:58:35.000000 pqp-0.3.3/python/pqp/utils/__init__.py
+-rw-r--r--   0      501       20      683 2023-03-25 06:45:09.000000 pqp-0.3.3/python/pqp/utils/exceptions.py
+-rw-r--r--   0      501       20     1473 2023-03-28 09:15:44.000000 pqp-0.3.3/python/pqp/utils/utils.py
+-rw-r--r--   0      501       20       11 2023-02-01 03:34:57.000000 pqp-0.3.3/python/tests/.gitignore
+-rw-r--r--   0      501       20      552 2023-03-26 06:08:17.000000 pqp-0.3.3/python/tests/test_abstract_step.py
+-rw-r--r--   0      501       20      966 2023-06-23 20:52:53.000000 pqp-0.3.3/python/tests/test_causal_estimand.py
+-rw-r--r--   0      501       20     3021 2023-03-28 07:26:00.000000 pqp-0.3.3/python/tests/test_data.py
+-rw-r--r--   0      501       20     1690 2023-03-25 03:20:40.000000 pqp-0.3.3/python/tests/test_domain.py
+-rw-r--r--   0      501       20      228 2023-03-23 04:38:36.000000 pqp-0.3.3/python/tests/test_event.py
+-rw-r--r--   0      501       20     6346 2023-04-01 08:45:57.000000 pqp-0.3.3/python/tests/test_examples.py
+-rw-r--r--   0      501       20     2280 2023-06-23 16:10:10.000000 pqp-0.3.3/python/tests/test_graph.py
+-rw-r--r--   0      501       20     1538 2023-03-28 06:40:11.000000 pqp-0.3.3/python/tests/test_id.py
+-rw-r--r--   0      501       20     7724 2023-04-01 04:27:39.000000 pqp-0.3.3/python/tests/test_multinomial_estimator.py
+-rw-r--r--   0      501       20     2413 2023-03-25 05:57:51.000000 pqp-0.3.3/python/tests/test_p.py
+-rw-r--r--   0      501       20      832 2023-03-31 01:59:17.000000 pqp-0.3.3/python/tests/test_refutation.py
+-rw-r--r--   0      501       20     3032 2023-06-23 19:24:57.000000 pqp-0.3.3/python/tests/test_relation.py
+-rw-r--r--   0      501       20      550 2023-03-28 09:16:20.000000 pqp-0.3.3/python/tests/test_utils.py
+-rw-r--r--   0      501       20     1040 2023-06-23 20:00:53.000000 pqp-0.3.3/python/tests/test_variable.py
+-rw-r--r--   0      501       20       74 2023-04-01 08:30:11.000000 pqp-0.3.3/requirements.txt
+-rw-r--r--   0      501       20      574 2023-02-01 03:34:57.000000 pqp-0.3.3/src/api/functions.rs
+-rw-r--r--   0      501       20       58 2023-02-25 00:17:24.000000 pqp-0.3.3/src/api/mod.rs
+-rw-r--r--   0      501       20      651 2023-02-01 03:34:57.000000 pqp-0.3.3/src/api/python.rs
+-rw-r--r--   0      501       20     1364 2023-02-01 03:34:57.000000 pqp-0.3.3/src/api/test.rs
+-rw-r--r--   0      501       20     5453 2023-04-01 08:49:23.000000 pqp-0.3.3/src/api/wrapper.rs
+-rw-r--r--   0      501       20     9318 2023-06-22 18:22:01.000000 pqp-0.3.3/src/form/form.rs
+-rw-r--r--   0      501       20      129 2023-02-01 03:34:57.000000 pqp-0.3.3/src/form/mod.rs
+-rw-r--r--   0      501       20     5218 2023-02-01 03:34:57.000000 pqp-0.3.3/src/form/simplify.rs
+-rw-r--r--   0      501       20     4151 2023-06-22 18:25:20.000000 pqp-0.3.3/src/form/test_form.rs
+-rw-r--r--   0      501       20     6687 2023-02-01 03:34:57.000000 pqp-0.3.3/src/form/test_simplify.rs
+-rw-r--r--   0      501       20     3459 2023-02-01 03:34:57.000000 pqp-0.3.3/src/form/tikka.rs
+-rw-r--r--   0      501       20     2552 2023-02-24 11:35:34.000000 pqp-0.3.3/src/graph/bigraph.rs
+-rw-r--r--   0      501       20     4865 2023-02-24 11:35:34.000000 pqp-0.3.3/src/graph/digraph.rs
+-rw-r--r--   0      501       20      303 2023-02-24 11:35:34.000000 pqp-0.3.3/src/graph/graph.rs
+-rw-r--r--   0      501       20     2075 2023-02-24 11:35:34.000000 pqp-0.3.3/src/graph/graph_builder.rs
+-rw-r--r--   0      501       20      296 2023-06-22 19:37:08.000000 pqp-0.3.3/src/graph/mod.rs
+-rw-r--r--   0      501       20      373 2023-06-22 21:00:19.000000 pqp-0.3.3/src/graph/node.rs
+-rw-r--r--   0      501       20     5763 2023-02-01 03:34:57.000000 pqp-0.3.3/src/graph/tests.rs
+-rw-r--r--   0      501       20       64 2023-02-25 00:14:14.000000 pqp-0.3.3/src/identification/mod.rs
+-rw-r--r--   0      501       20     3689 2023-02-25 00:13:29.000000 pqp-0.3.3/src/identification/shpitser.rs
+-rw-r--r--   0      501       20     6682 2023-06-22 18:22:08.000000 pqp-0.3.3/src/identification/tests.rs
+-rw-r--r--   0      501       20      154 2023-02-24 11:35:34.000000 pqp-0.3.3/src/lib.rs
+-rw-r--r--   0      501       20      368 2023-02-01 03:34:57.000000 pqp-0.3.3/src/model/examples.rs
+-rw-r--r--   0      501       20       93 2023-06-22 21:01:19.000000 pqp-0.3.3/src/model/mod.rs
+-rw-r--r--   0      501       20     6195 2023-06-22 18:44:17.000000 pqp-0.3.3/src/model/model.rs
+-rw-r--r--   0      501       20     2565 2023-02-01 03:34:57.000000 pqp-0.3.3/src/model/order.rs
+-rw-r--r--   0      501       20     4253 2023-06-22 21:01:26.000000 pqp-0.3.3/src/model/tests.rs
+-rw-r--r--   0      501       20      795 2023-06-22 21:01:57.000000 pqp-0.3.3/src/test.rs
+-rw-r--r--   0      501       20      304 2023-02-01 03:34:57.000000 pqp-0.3.3/src/utils/defaults.rs
+-rw-r--r--   0      501       20       99 2023-02-24 11:35:34.000000 pqp-0.3.3/src/utils/mod.rs
+-rw-r--r--   0      501       20     2185 2023-02-01 03:34:57.000000 pqp-0.3.3/src/utils/set_utils.rs
+-rw-r--r--   0      501       20      987 2023-02-01 03:34:57.000000 pqp-0.3.3/src/utils/tests.rs
+-rw-r--r--   0      501       20      612 2023-02-24 11:35:34.000000 pqp-0.3.3/src/utils/utils.rs
+-rw-r--r--   0      501       20       49 2023-02-01 03:34:57.000000 pqp-0.3.3/test.sh
+-rw-r--r--   0      501       20   150084 2023-02-01 03:34:57.000000 pqp-0.3.3/writeup/2023-01-14-13-06-10.png
+-rw-r--r--   0      501       20    51282 2023-02-01 03:34:57.000000 pqp-0.3.3/writeup/2023-01-14-13-52-24.png
+-rw-r--r--   0      501       20    53166 2023-02-01 03:34:57.000000 pqp-0.3.3/writeup/2023-01-14-14-22-06.png
+-rw-r--r--   0      501       20   118082 2023-02-01 03:34:57.000000 pqp-0.3.3/writeup/2023-01-14-15-01-52.png
+-rw-r--r--   0      501       20    45879 2023-02-25 02:07:37.000000 pqp-0.3.3/writeup/2023-02-25-09-07-36.png
+-rw-r--r--   0      501       20    50872 2023-02-25 02:22:50.000000 pqp-0.3.3/writeup/2023-02-25-09-22-50.png
+-rw-r--r--   0      501       20   367476 2023-04-02 04:33:16.000000 pqp-0.3.3/writeup/2023-04-02-14-33-14.png
+-rw-r--r--   0      501       20   325115 2023-04-02 04:33:45.000000 pqp-0.3.3/writeup/2023-04-02-14-33-44.png
+-rw-r--r--   0      501       20   213508 2023-04-02 04:34:20.000000 pqp-0.3.3/writeup/2023-04-02-14-34-19.png
+-rw-r--r--   0      501       20   336724 2023-04-02 04:34:31.000000 pqp-0.3.3/writeup/2023-04-02-14-34-30.png
+-rw-r--r--   0      501       20   349974 2023-04-02 04:34:45.000000 pqp-0.3.3/writeup/2023-04-02-14-34-44.png
+-rw-r--r--   0      501       20   407521 2023-04-02 04:35:40.000000 pqp-0.3.3/writeup/2023-04-02-14-35-39.png
+-rw-r--r--   0      501       20   115292 2023-04-02 04:36:00.000000 pqp-0.3.3/writeup/2023-04-02-14-36-00.png
+-rw-r--r--   0      501       20   476032 2023-04-02 04:36:59.000000 pqp-0.3.3/writeup/2023-04-02-14-36-57.png
+-rw-r--r--   0      501       20   345389 2023-04-02 04:37:11.000000 pqp-0.3.3/writeup/2023-04-02-14-37-10.png
+-rw-r--r--   0      501       20   108822 2023-04-02 04:47:11.000000 pqp-0.3.3/writeup/PQP a Library for End-to-End Causal Inference.ipynb
+-rw-r--r--   0      501       20   197652 2023-04-01 03:17:51.000000 pqp-0.3.3/writeup/PQP.ipynb
+-rw-r--r--   0      501       20   117397 2023-04-01 03:17:56.000000 pqp-0.3.3/writeup/agg.ipynb
+-rw-r--r--   0      501       20      882 2023-02-25 16:01:13.000000 pqp-0.3.3/writeup/build.py
+-rw-r--r--   0      501       20    16499 2023-03-11 07:28:34.000000 pqp-0.3.3/writeup/demo.ipynb
+-rw-r--r--   0      501       20     8008 2023-04-02 04:40:20.000000 pqp-0.3.3/writeup/demo1.csv
+-rw-r--r--   0      501       20    27322 2023-04-01 12:35:30.000000 pqp-0.3.3/writeup/doctordemo.csv
+-rw-r--r--   0      501       20    14520 2023-06-22 21:23:55.000000 pqp-0.3.3/writeup/examples.ipynb
+-rw-r--r--   0      501       20     1756 2023-02-25 15:09:55.000000 pqp-0.3.3/writeup/grab_code.py
+-rw-r--r--   0      501       20     6485 2023-04-03 04:52:12.000000 pqp-0.3.3/writeup/speed.ipynb
+-rw-r--r--   0      501       20      678 2023-04-01 03:08:56.000000 pqp-0.3.3/writeup/supplement.py
+-rw-r--r--   0      501       20     9185 2023-02-24 11:35:34.000000 pqp-0.3.3/Cargo.lock
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pqp-0.3.3/PKG-INFO
```

### Comparing `pqp-0.3.2/.coverage` & `pqp-0.3.3/.coverage`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/CHANGELOG.md` & `pqp-0.3.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/CONTRIBUTING.md` & `pqp-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/LICENSE.txt` & `pqp-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/README.md` & `pqp-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/pyproject.toml` & `pqp-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "pqp"
-version = "0.3.2"
+version = "0.3.3"
 description = "Subroutines for structural causal modeling"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Leo Ware"}]
 dependencies = [
     "pandas",
     "numpy",
     "tomli",
     "matplotlib"
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["causal inference", "causal identification"]
```

### Comparing `pqp-0.3.2/python/docs/Makefile` & `pqp-0.3.3/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/make.bat` & `pqp-0.3.3/python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/api/pqp.estimation.Estimator.rst` & `pqp-0.3.3/python/docs/source/api/pqp.estimation.Estimator.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst` & `pqp-0.3.3/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/api/pqp.identification.Graph.rst` & `pqp-0.3.3/python/docs/source/api/pqp.identification.Graph.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/api/pqp.refutation.Result.rst` & `pqp-0.3.3/python/docs/source/api/pqp.refutation.Result.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/api/pqp.symbols.AbstractExpression.rst` & `pqp-0.3.3/python/docs/source/api/pqp.symbols.AbstractExpression.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/api/pqp.symbols.Difference.rst` & `pqp-0.3.3/python/docs/source/api/pqp.symbols.Difference.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/api/pqp.symbols.Expectation.rst` & `pqp-0.3.3/python/docs/source/api/pqp.symbols.Expectation.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/api/pqp.symbols.P.rst` & `pqp-0.3.3/python/docs/source/api/pqp.symbols.P.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/conf.py` & `pqp-0.3.3/python/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/favicon.ico` & `pqp-0.3.3/python/docs/source/favicon.ico`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/imgs/frontdoor_estimator.png` & `pqp-0.3.3/python/docs/source/imgs/frontdoor_estimator.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/imgs/frontdoor_new.png` & `pqp-0.3.3/python/docs/source/imgs/frontdoor_new.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/imgs/frontdoor_viz.png` & `pqp-0.3.3/python/docs/source/imgs/frontdoor_viz.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/imgs/qs_causal_estimand.png` & `pqp-0.3.3/python/docs/source/imgs/qs_causal_estimand.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/imgs/qs_stat_estimand.png` & `pqp-0.3.3/python/docs/source/imgs/qs_stat_estimand.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/index.rst` & `pqp-0.3.3/python/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/pqp.estimation.rst` & `pqp-0.3.3/python/docs/source/pqp.estimation.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/pqp.identification.rst` & `pqp-0.3.3/python/docs/source/pqp.identification.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/pqp.symbols.rst` & `pqp-0.3.3/python/docs/source/pqp.symbols.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/docs/source/quickstart.rst` & `pqp-0.3.3/python/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/fd_case_study.ipynb` & `pqp-0.3.3/python/fd_case_study.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/data/data.py` & `pqp-0.3.3/python/pqp/data/data.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/data/domain.py` & `pqp-0.3.3/python/pqp/data/domain.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/estimation/estimator.py` & `pqp-0.3.3/python/pqp/estimation/estimator.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/estimation/multinomial_estimator.py` & `pqp-0.3.3/python/pqp/estimation/multinomial_estimator.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/fd_demo.py` & `pqp-0.3.3/python/pqp/fd_demo.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/identification/estimands.py` & `pqp-0.3.3/python/pqp/identification/estimands.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/identification/graph.py` & `pqp-0.3.3/python/pqp/identification/graph.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/refutation/__init__.py` & `pqp-0.3.3/python/pqp/refutation/__init__.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/refutation/result.py` & `pqp-0.3.3/python/pqp/refutation/result.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/symbols/event.py` & `pqp-0.3.3/python/pqp/symbols/event.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/symbols/p.py` & `pqp-0.3.3/python/pqp/symbols/p.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/symbols/parse.py` & `pqp-0.3.3/python/pqp/symbols/parse.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/symbols/relation.py` & `pqp-0.3.3/python/pqp/symbols/relation.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/symbols/variable.py` & `pqp-0.3.3/python/pqp/symbols/variable.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/utils/exceptions.py` & `pqp-0.3.3/python/pqp/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/pqp/utils/utils.py` & `pqp-0.3.3/python/pqp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_abstract_step.py` & `pqp-0.3.3/python/tests/test_abstract_step.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_causal_estimand.py` & `pqp-0.3.3/python/tests/test_causal_estimand.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_data.py` & `pqp-0.3.3/python/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_domain.py` & `pqp-0.3.3/python/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_examples.py` & `pqp-0.3.3/python/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_graph.py` & `pqp-0.3.3/python/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_id.py` & `pqp-0.3.3/python/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_multinomial_estimator.py` & `pqp-0.3.3/python/tests/test_multinomial_estimator.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_p.py` & `pqp-0.3.3/python/tests/test_p.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_refutation.py` & `pqp-0.3.3/python/tests/test_refutation.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_relation.py` & `pqp-0.3.3/python/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_utils.py` & `pqp-0.3.3/python/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/python/tests/test_variable.py` & `pqp-0.3.3/python/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/api/functions.rs` & `pqp-0.3.3/src/api/functions.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/api/python.rs` & `pqp-0.3.3/src/api/python.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/api/test.rs` & `pqp-0.3.3/src/api/test.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/api/wrapper.rs` & `pqp-0.3.3/src/api/wrapper.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/form/form.rs` & `pqp-0.3.3/src/form/form.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/form/simplify.rs` & `pqp-0.3.3/src/form/simplify.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/form/test_form.rs` & `pqp-0.3.3/src/form/test_form.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/form/test_simplify.rs` & `pqp-0.3.3/src/form/test_simplify.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/form/tikka.rs` & `pqp-0.3.3/src/form/tikka.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/graph/bigraph.rs` & `pqp-0.3.3/src/graph/bigraph.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/graph/digraph.rs` & `pqp-0.3.3/src/graph/digraph.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/graph/graph_builder.rs` & `pqp-0.3.3/src/graph/graph_builder.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/graph/tests.rs` & `pqp-0.3.3/src/graph/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/identification/shpitser.rs` & `pqp-0.3.3/src/identification/shpitser.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/identification/tests.rs` & `pqp-0.3.3/src/identification/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/model/model.rs` & `pqp-0.3.3/src/model/model.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/model/order.rs` & `pqp-0.3.3/src/model/order.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/model/tests.rs` & `pqp-0.3.3/src/model/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/test.rs` & `pqp-0.3.3/src/test.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/utils/set_utils.rs` & `pqp-0.3.3/src/utils/set_utils.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/utils/tests.rs` & `pqp-0.3.3/src/utils/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/src/utils/utils.rs` & `pqp-0.3.3/src/utils/utils.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-01-14-13-06-10.png` & `pqp-0.3.3/writeup/2023-01-14-13-06-10.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-01-14-13-52-24.png` & `pqp-0.3.3/writeup/2023-01-14-13-52-24.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-01-14-14-22-06.png` & `pqp-0.3.3/writeup/2023-01-14-14-22-06.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-01-14-15-01-52.png` & `pqp-0.3.3/writeup/2023-01-14-15-01-52.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-02-25-09-07-36.png` & `pqp-0.3.3/writeup/2023-02-25-09-07-36.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-02-25-09-22-50.png` & `pqp-0.3.3/writeup/2023-02-25-09-22-50.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-33-14.png` & `pqp-0.3.3/writeup/2023-04-02-14-33-14.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-33-44.png` & `pqp-0.3.3/writeup/2023-04-02-14-33-44.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-34-19.png` & `pqp-0.3.3/writeup/2023-04-02-14-34-19.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-34-30.png` & `pqp-0.3.3/writeup/2023-04-02-14-34-30.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-34-44.png` & `pqp-0.3.3/writeup/2023-04-02-14-34-44.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-35-39.png` & `pqp-0.3.3/writeup/2023-04-02-14-35-39.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-36-00.png` & `pqp-0.3.3/writeup/2023-04-02-14-36-00.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-36-57.png` & `pqp-0.3.3/writeup/2023-04-02-14-36-57.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/2023-04-02-14-37-10.png` & `pqp-0.3.3/writeup/2023-04-02-14-37-10.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/PQP a Library for End-to-End Causal Inference.ipynb` & `pqp-0.3.3/writeup/PQP a Library for End-to-End Causal Inference.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/PQP.ipynb` & `pqp-0.3.3/writeup/PQP.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/agg.ipynb` & `pqp-0.3.3/writeup/agg.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/build.py` & `pqp-0.3.3/writeup/build.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/demo.ipynb` & `pqp-0.3.3/writeup/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/demo1.csv` & `pqp-0.3.3/writeup/demo1.csv`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/doctordemo.csv` & `pqp-0.3.3/writeup/doctordemo.csv`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/examples.ipynb` & `pqp-0.3.3/writeup/examples.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/grab_code.py` & `pqp-0.3.3/writeup/grab_code.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/speed.ipynb` & `pqp-0.3.3/writeup/speed.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/writeup/supplement.py` & `pqp-0.3.3/writeup/supplement.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/Cargo.lock` & `pqp-0.3.3/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pqp-0.3.2/PKG-INFO` & `pqp-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqp
-Version: 0.3.2
+Version: 0.3.3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: tomli
 Requires-Dist: matplotlib
@@ -14,15 +14,15 @@
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: networkx ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE.txt
 Summary: Subroutines for structural causal modeling
 Keywords: causal inference,causal identification
 Author: Leo Ware
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://leo-ware.github.io/capstone/
 Project-URL: Source, https://github.com/leo-ware/capstone
 
 # PQP
 
 The name `pqp` is short for *Pourquoi pas?*. This phrase is French for *why not?*, because "Why not?" was the question we asked ourselves when we found there was no maintained, open-source package for structural causal modeling in Python. The package provides a convenient interface for causal modeling along with routines for identification, estimation, and visualization.
```

