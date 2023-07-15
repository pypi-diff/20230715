# Comparing `tmp/pqp-0.3.4.tar.gz` & `tmp/pqp-0.3.5.tar.gz`

## Comparing `pqp-0.3.4.tar` & `pqp-0.3.5.tar`

### file list

```diff
@@ -1,219 +1,219 @@
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 pqp-0.3.4/Cargo.toml
--rw-r--r--   0     1001      123    53248 2023-07-15 15:54:04.000000 pqp-0.3.4/.coverage
--rw-r--r--   0     1001      123     2703 2023-07-15 15:54:04.000000 pqp-0.3.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      105 2023-07-15 15:54:04.000000 pqp-0.3.4/.gitignore
--rw-r--r--   0     1001      123      579 2023-07-15 15:54:04.000000 pqp-0.3.4/CHANGELOG.md
--rw-r--r--   0     1001      123     1145 2023-07-15 15:54:04.000000 pqp-0.3.4/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1047 2023-07-15 15:54:04.000000 pqp-0.3.4/LICENSE.txt
--rw-r--r--   0     1001      123     1292 2023-07-15 15:54:04.000000 pqp-0.3.4/README.md
--rw-r--r--   0     1001      123      333 2023-07-15 15:54:04.000000 pqp-0.3.4/deployment_script.sh
--rw-r--r--   0     1001      123       10 2023-07-15 15:54:11.000000 pqp-0.3.4/dist/pqp-0.3.4.tar.gz
--rw-r--r--   0     1001      123      333 2023-07-15 15:54:04.000000 pqp-0.3.4/publish_docs.sh
--rw-r--r--   0     1001      123      853 2023-07-15 15:54:04.000000 pqp-0.3.4/pyproject.toml
--rw-r--r--   0     1001      123       38 2023-07-15 15:54:04.000000 pqp-0.3.4/python/.gitignore
--rw-r--r--   0     1001      123        0 2023-07-15 15:54:04.000000 pqp-0.3.4/python/conftest.py
--rw-r--r--   0     1001      123       12 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/.gitignore
--rw-r--r--   0     1001      123      850 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/Makefile
--rw-r--r--   0     1001      123      804 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/make.bat
--rw-r--r--   0     1001      123      280 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.BinaryDomain.rst
--rw-r--r--   0     1001      123      442 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.CategoricalDomain.rst
--rw-r--r--   0     1001      123      286 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.ContinuousDomain.rst
--rw-r--r--   0     1001      123      412 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.Data.rst
--rw-r--r--   0     1001      123      268 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.DiscreteDomain.rst
--rw-r--r--   0     1001      123      441 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.Domain.rst
--rw-r--r--   0     1001      123      478 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.IntegerDomain.rst
--rw-r--r--   0     1001      123      272 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.RealDomain.rst
--rw-r--r--   0     1001      123      102 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.infer_domain_type.rst
--rw-r--r--   0     1001      123       84 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.data.make_domain.rst
--rw-r--r--   0     1001      123      279 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.estimation.EstimationResult.rst
--rw-r--r--   0     1001      123      764 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.estimation.Estimator.rst
--rw-r--r--   0     1001      123      973 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst
--rw-r--r--   0     1001      123      307 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.expression.Expression.rst
--rw-r--r--   0     1001      123      234 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.expression.Hedge.rst
--rw-r--r--   0     1001      123      246 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.expression.Marginal.rst
--rw-r--r--   0     1001      123      218 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.expression.P.rst
--rw-r--r--   0     1001      123      242 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.expression.Product.rst
--rw-r--r--   0     1001      123      246 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.expression.Quotient.rst
--rw-r--r--   0     1001      123       87 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.expression.parse_json.rst
--rw-r--r--   0     1001      123      113 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.graph.BidirectedEdge.rst
--rw-r--r--   0     1001      123      107 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.graph.DirectedEdge.rst
--rw-r--r--   0     1001      123      435 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.graph.Graph.rst
--rw-r--r--   0     1001      123      294 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.identification.ATE.rst
--rw-r--r--   0     1001      123      310 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.identification.AbstractCausalEstimand.rst
--rw-r--r--   0     1001      123      122 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.identification.BidirectedEdge.rst
--rw-r--r--   0     1001      123      295 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.identification.CATE.rst
--rw-r--r--   0     1001      123      278 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.identification.CausalEstimand.rst
--rw-r--r--   0     1001      123      116 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.identification.DirectedEdge.rst
--rw-r--r--   0     1001      123      624 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.identification.Graph.rst
--rw-r--r--   0     1001      123      140 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.identification.IdentificationResult.rst
--rw-r--r--   0     1001      123      103 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.refutation.Operation.rst
--rw-r--r--   0     1001      123      586 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.refutation.Result.rst
--rw-r--r--   0     1001      123      408 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.refutation.Step.rst
--rw-r--r--   0     1001      123       87 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.refutation.entrypoint.rst
--rw-r--r--   0     1001      123      730 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.AbstractExpression.rst
--rw-r--r--   0     1001      123      314 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.AbstractMath.rst
--rw-r--r--   0     1001      123      522 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Difference.rst
--rw-r--r--   0     1001      123      319 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.EqualityEvent.rst
--rw-r--r--   0     1001      123      238 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Event.rst
--rw-r--r--   0     1001      123      531 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Expectation.rst
--rw-r--r--   0     1001      123      435 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Hedge.rst
--rw-r--r--   0     1001      123      397 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.InterventionEvent.rst
--rw-r--r--   0     1001      123      504 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Marginal.rst
--rw-r--r--   0     1001      123      777 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.P.rst
--rw-r--r--   0     1001      123      495 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Product.rst
--rw-r--r--   0     1001      123      504 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Quotient.rst
--rw-r--r--   0     1001      123      121 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.StatisticalEvent.rst
--rw-r--r--   0     1001      123      477 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Value.rst
--rw-r--r--   0     1001      123      243 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.Variable.rst
--rw-r--r--   0     1001      123       60 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.do.rst
--rw-r--r--   0     1001      123       81 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.make_vars.rst
--rw-r--r--   0     1001      123       84 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.symbols.parse_json.rst
--rw-r--r--   0     1001      123       95 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.attrdict.rst
--rw-r--r--   0     1001      123      127 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.exceptions.DomainValidationError.rst
--rw-r--r--   0     1001      123      127 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.exceptions.InferredDomainWarning.rst
--rw-r--r--   0     1001      123      106 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.exceptions.NumericalError.rst
--rw-r--r--   0     1001      123      121 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.exceptions.PositivityException.rst
--rw-r--r--   0     1001      123      115 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.exceptions.UnitDomainWarning.rst
--rw-r--r--   0     1001      123       85 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.order_graph.rst
--rw-r--r--   0     1001      123       94 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.recursive_sort.rst
--rw-r--r--   0     1001      123      113 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.utils.staticproperty.rst
--rw-r--r--   0     1001      123      244 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.variable.Variable.rst
--rw-r--r--   0     1001      123       82 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/api/pqp.variable.make_vars.rst
--rw-r--r--   0     1001      123     1483 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/conf.py
--rw-r--r--   0     1001      123       42 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/example_notebooks.rst
--rw-r--r--   0     1001      123   238718 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/favicon.ico
--rw-r--r--   0     1001      123    19314 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/imgs/frontdoor_estimator.png
--rw-r--r--   0     1001      123    18477 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/imgs/frontdoor_new.png
--rw-r--r--   0     1001      123    97789 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/imgs/frontdoor_viz.png
--rw-r--r--   0     1001      123    37703 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/imgs/qs_causal_estimand.png
--rw-r--r--   0     1001      123    75030 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/imgs/qs_stat_estimand.png
--rw-r--r--   0     1001      123      809 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/index.rst
--rw-r--r--   0     1001      123       24 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/data.rst
--rw-r--r--   0     1001      123       30 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/estimation.rst
--rw-r--r--   0     1001      123       36 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/exceptions.rst
--rw-r--r--   0     1001      123       30 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/expression.rst
--rw-r--r--   0     1001      123       53 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/graph.rst
--rw-r--r--   0     1001      123       34 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/identification.rst
--rw-r--r--   0     1001      123       30 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/refutation.rst
--rw-r--r--   0     1001      123       27 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/symbols.rst
--rw-r--r--   0     1001      123       28 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/module_maps/variable.rst
--rw-r--r--   0     1001      123       46 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/modules.rst
--rw-r--r--   0     1001      123      432 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/pqp.data.rst
--rw-r--r--   0     1001      123      548 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/pqp.estimation.rst
--rw-r--r--   0     1001      123      534 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/pqp.identification.rst
--rw-r--r--   0     1001      123      340 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/pqp.refutation.rst
--rw-r--r--   0     1001      123      419 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/pqp.rst
--rw-r--r--   0     1001      123     1051 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/pqp.symbols.rst
--rw-r--r--   0     1001      123      456 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/pqp.utils.rst
--rw-r--r--   0     1001      123     6082 2023-07-15 15:54:04.000000 pqp-0.3.4/python/docs/source/quickstart.rst
--rw-r--r--   0     1001      123   117134 2023-07-15 15:54:04.000000 pqp-0.3.4/python/fd_case_study.ipynb
--rw-r--r--   0     1001      123       16 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/.gitignore
--rw-r--r--   0     1001      123      268 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/__init__.py
--rw-r--r--   0     1001      123       60 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/data/__init__.py
--rw-r--r--   0     1001      123     7569 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/data/data.py
--rw-r--r--   0     1001      123     8507 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/data/domain.py
--rw-r--r--   0     1001      123      135 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/estimation/__init__.py
--rw-r--r--   0     1001      123     4072 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/estimation/estimator.py
--rw-r--r--   0     1001      123     8925 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/estimation/multinomial_estimator.py
--rw-r--r--   0     1001      123     4762 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/expression.py
--rw-r--r--   0     1001      123      589 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/fd_demo.py
--rw-r--r--   0     1001      123     3704 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/graph.py
--rw-r--r--   0     1001      123      186 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/identification/__init__.py
--rw-r--r--   0     1001      123     8977 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/identification/estimands.py
--rw-r--r--   0     1001      123    13147 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/identification/graph.py
--rw-r--r--   0     1001      123     2388 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/refutation/__init__.py
--rw-r--r--   0     1001      123     6271 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/refutation/result.py
--rw-r--r--   0     1001      123      241 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/symbols/__init__.py
--rw-r--r--   0     1001      123      396 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/symbols/abstract_math.py
--rw-r--r--   0     1001      123     3018 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/symbols/event.py
--rw-r--r--   0     1001      123     7580 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/symbols/p.py
--rw-r--r--   0     1001      123     1126 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/symbols/parse.py
--rw-r--r--   0     1001      123    20412 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/symbols/relation.py
--rw-r--r--   0     1001      123     4317 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/symbols/variable.py
--rw-r--r--   0     1001      123       29 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/utils/__init__.py
--rw-r--r--   0     1001      123      683 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/utils/exceptions.py
--rw-r--r--   0     1001      123     1473 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/utils/utils.py
--rw-r--r--   0     1001      123      324 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/utils.py
--rw-r--r--   0     1001      123     1555 2023-07-15 15:54:04.000000 pqp-0.3.4/python/pqp/variable.py
--rw-r--r--   0     1001      123    26124 2023-07-15 15:54:04.000000 pqp-0.3.4/python/scratch.ipynb
--rw-r--r--   0     1001      123       11 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/.gitignore
--rw-r--r--   0     1001      123      552 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_abstract_step.py
--rw-r--r--   0     1001      123      966 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_causal_estimand.py
--rw-r--r--   0     1001      123     3021 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_data.py
--rw-r--r--   0     1001      123     1690 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_domain.py
--rw-r--r--   0     1001      123      228 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_event.py
--rw-r--r--   0     1001      123     6346 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_examples.py
--rw-r--r--   0     1001      123     2280 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_graph.py
--rw-r--r--   0     1001      123     1538 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_id.py
--rw-r--r--   0     1001      123     7724 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_multinomial_estimator.py
--rw-r--r--   0     1001      123     2413 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_p.py
--rw-r--r--   0     1001      123      901 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_pqp.py
--rw-r--r--   0     1001      123      832 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_refutation.py
--rw-r--r--   0     1001      123     3032 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_relation.py
--rw-r--r--   0     1001      123      550 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_utils.py
--rw-r--r--   0     1001      123     1040 2023-07-15 15:54:04.000000 pqp-0.3.4/python/tests/test_variable.py
--rw-r--r--   0     1001      123       74 2023-07-15 15:54:04.000000 pqp-0.3.4/requirements.txt
--rw-r--r--   0     1001      123      574 2023-07-15 15:54:04.000000 pqp-0.3.4/src/api/functions.rs
--rw-r--r--   0     1001      123       58 2023-07-15 15:54:04.000000 pqp-0.3.4/src/api/mod.rs
--rw-r--r--   0     1001      123      651 2023-07-15 15:54:04.000000 pqp-0.3.4/src/api/python.rs
--rw-r--r--   0     1001      123     1364 2023-07-15 15:54:04.000000 pqp-0.3.4/src/api/test.rs
--rw-r--r--   0     1001      123     5453 2023-07-15 15:54:04.000000 pqp-0.3.4/src/api/wrapper.rs
--rw-r--r--   0     1001      123     9318 2023-07-15 15:54:04.000000 pqp-0.3.4/src/form/form.rs
--rw-r--r--   0     1001      123      129 2023-07-15 15:54:04.000000 pqp-0.3.4/src/form/mod.rs
--rw-r--r--   0     1001      123     5218 2023-07-15 15:54:04.000000 pqp-0.3.4/src/form/simplify.rs
--rw-r--r--   0     1001      123     4151 2023-07-15 15:54:04.000000 pqp-0.3.4/src/form/test_form.rs
--rw-r--r--   0     1001      123     6687 2023-07-15 15:54:04.000000 pqp-0.3.4/src/form/test_simplify.rs
--rw-r--r--   0     1001      123     3459 2023-07-15 15:54:04.000000 pqp-0.3.4/src/form/tikka.rs
--rw-r--r--   0     1001      123     2552 2023-07-15 15:54:04.000000 pqp-0.3.4/src/graph/bigraph.rs
--rw-r--r--   0     1001      123     4865 2023-07-15 15:54:04.000000 pqp-0.3.4/src/graph/digraph.rs
--rw-r--r--   0     1001      123      303 2023-07-15 15:54:04.000000 pqp-0.3.4/src/graph/graph.rs
--rw-r--r--   0     1001      123     2075 2023-07-15 15:54:04.000000 pqp-0.3.4/src/graph/graph_builder.rs
--rw-r--r--   0     1001      123      296 2023-07-15 15:54:04.000000 pqp-0.3.4/src/graph/mod.rs
--rw-r--r--   0     1001      123      373 2023-07-15 15:54:04.000000 pqp-0.3.4/src/graph/node.rs
--rw-r--r--   0     1001      123     5763 2023-07-15 15:54:04.000000 pqp-0.3.4/src/graph/tests.rs
--rw-r--r--   0     1001      123       64 2023-07-15 15:54:04.000000 pqp-0.3.4/src/identification/mod.rs
--rw-r--r--   0     1001      123     3689 2023-07-15 15:54:04.000000 pqp-0.3.4/src/identification/shpitser.rs
--rw-r--r--   0     1001      123     6682 2023-07-15 15:54:04.000000 pqp-0.3.4/src/identification/tests.rs
--rw-r--r--   0     1001      123      154 2023-07-15 15:54:04.000000 pqp-0.3.4/src/lib.rs
--rw-r--r--   0     1001      123      368 2023-07-15 15:54:04.000000 pqp-0.3.4/src/model/examples.rs
--rw-r--r--   0     1001      123       93 2023-07-15 15:54:04.000000 pqp-0.3.4/src/model/mod.rs
--rw-r--r--   0     1001      123     6195 2023-07-15 15:54:04.000000 pqp-0.3.4/src/model/model.rs
--rw-r--r--   0     1001      123     2565 2023-07-15 15:54:04.000000 pqp-0.3.4/src/model/order.rs
--rw-r--r--   0     1001      123     4253 2023-07-15 15:54:04.000000 pqp-0.3.4/src/model/tests.rs
--rw-r--r--   0     1001      123      795 2023-07-15 15:54:04.000000 pqp-0.3.4/src/test.rs
--rw-r--r--   0     1001      123      304 2023-07-15 15:54:04.000000 pqp-0.3.4/src/utils/defaults.rs
--rw-r--r--   0     1001      123       99 2023-07-15 15:54:04.000000 pqp-0.3.4/src/utils/mod.rs
--rw-r--r--   0     1001      123     2185 2023-07-15 15:54:04.000000 pqp-0.3.4/src/utils/set_utils.rs
--rw-r--r--   0     1001      123      987 2023-07-15 15:54:04.000000 pqp-0.3.4/src/utils/tests.rs
--rw-r--r--   0     1001      123      612 2023-07-15 15:54:04.000000 pqp-0.3.4/src/utils/utils.rs
--rw-r--r--   0     1001      123       49 2023-07-15 15:54:04.000000 pqp-0.3.4/test.sh
--rw-r--r--   0     1001      123   150084 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-01-14-13-06-10.png
--rw-r--r--   0     1001      123    51282 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-01-14-13-52-24.png
--rw-r--r--   0     1001      123    53166 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-01-14-14-22-06.png
--rw-r--r--   0     1001      123   118082 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-01-14-15-01-52.png
--rw-r--r--   0     1001      123    45879 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-02-25-09-07-36.png
--rw-r--r--   0     1001      123    50872 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-02-25-09-22-50.png
--rw-r--r--   0     1001      123   367476 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-33-14.png
--rw-r--r--   0     1001      123   325115 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-33-44.png
--rw-r--r--   0     1001      123   213508 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-34-19.png
--rw-r--r--   0     1001      123   336724 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-34-30.png
--rw-r--r--   0     1001      123   349974 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-34-44.png
--rw-r--r--   0     1001      123   407521 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-35-39.png
--rw-r--r--   0     1001      123   115292 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-36-00.png
--rw-r--r--   0     1001      123   476032 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-36-57.png
--rw-r--r--   0     1001      123   345389 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/2023-04-02-14-37-10.png
--rw-r--r--   0     1001      123   108822 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/PQP a Library for End-to-End Causal Inference.ipynb
--rw-r--r--   0     1001      123   197652 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/PQP.ipynb
--rw-r--r--   0     1001      123    36229 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/Performant Conditional Query Identification in Structural Causal Models.ipynb
--rw-r--r--   0     1001      123   117397 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/agg.ipynb
--rw-r--r--   0     1001      123      882 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/build.py
--rw-r--r--   0     1001      123    16499 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/demo.ipynb
--rw-r--r--   0     1001      123     8008 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/demo1.csv
--rw-r--r--   0     1001      123    27322 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/doctordemo.csv
--rw-r--r--   0     1001      123    14520 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/examples.ipynb
--rw-r--r--   0     1001      123     1756 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/grab_code.py
--rw-r--r--   0     1001      123     1738 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/scratch.ipynb
--rw-r--r--   0     1001      123     6485 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/speed.ipynb
--rw-r--r--   0     1001      123      678 2023-07-15 15:54:04.000000 pqp-0.3.4/writeup/supplement.py
--rw-r--r--   0     1001      123     9185 2023-07-15 15:54:04.000000 pqp-0.3.4/Cargo.lock
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 pqp-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 pqp-0.3.5/Cargo.toml
+-rw-r--r--   0     1001      123    53248 2023-07-15 21:29:55.000000 pqp-0.3.5/.coverage
+-rw-r--r--   0     1001      123     2714 2023-07-15 21:29:55.000000 pqp-0.3.5/.github/workflows/build_release.yml
+-rw-r--r--   0     1001      123      105 2023-07-15 21:29:55.000000 pqp-0.3.5/.gitignore
+-rw-r--r--   0     1001      123      579 2023-07-15 21:29:55.000000 pqp-0.3.5/CHANGELOG.md
+-rw-r--r--   0     1001      123     1192 2023-07-15 21:29:55.000000 pqp-0.3.5/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1047 2023-07-15 21:29:55.000000 pqp-0.3.5/LICENSE.txt
+-rw-r--r--   0     1001      123     1292 2023-07-15 21:29:55.000000 pqp-0.3.5/README.md
+-rw-r--r--   0     1001      123      333 2023-07-15 21:29:55.000000 pqp-0.3.5/deployment_script.sh
+-rw-r--r--   0     1001      123       10 2023-07-15 21:30:04.000000 pqp-0.3.5/dist/pqp-0.3.5.tar.gz
+-rw-r--r--   0     1001      123      333 2023-07-15 21:29:55.000000 pqp-0.3.5/publish_docs.sh
+-rw-r--r--   0     1001      123      907 2023-07-15 21:29:55.000000 pqp-0.3.5/pyproject.toml
+-rw-r--r--   0     1001      123       38 2023-07-15 21:29:55.000000 pqp-0.3.5/python/.gitignore
+-rw-r--r--   0     1001      123        0 2023-07-15 21:29:55.000000 pqp-0.3.5/python/conftest.py
+-rw-r--r--   0     1001      123       12 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/.gitignore
+-rw-r--r--   0     1001      123      862 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/Makefile
+-rw-r--r--   0     1001      123      804 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/make.bat
+-rw-r--r--   0     1001      123      280 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.BinaryDomain.rst
+-rw-r--r--   0     1001      123      442 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.CategoricalDomain.rst
+-rw-r--r--   0     1001      123      286 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.ContinuousDomain.rst
+-rw-r--r--   0     1001      123      412 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.Data.rst
+-rw-r--r--   0     1001      123      268 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.DiscreteDomain.rst
+-rw-r--r--   0     1001      123      441 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.Domain.rst
+-rw-r--r--   0     1001      123      478 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.IntegerDomain.rst
+-rw-r--r--   0     1001      123      272 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.RealDomain.rst
+-rw-r--r--   0     1001      123      102 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.infer_domain_type.rst
+-rw-r--r--   0     1001      123       84 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.data.make_domain.rst
+-rw-r--r--   0     1001      123      279 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.estimation.EstimationResult.rst
+-rw-r--r--   0     1001      123      764 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.estimation.Estimator.rst
+-rw-r--r--   0     1001      123      973 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst
+-rw-r--r--   0     1001      123      307 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.expression.Expression.rst
+-rw-r--r--   0     1001      123      234 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.expression.Hedge.rst
+-rw-r--r--   0     1001      123      246 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.expression.Marginal.rst
+-rw-r--r--   0     1001      123      218 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.expression.P.rst
+-rw-r--r--   0     1001      123      242 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.expression.Product.rst
+-rw-r--r--   0     1001      123      246 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.expression.Quotient.rst
+-rw-r--r--   0     1001      123       87 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.expression.parse_json.rst
+-rw-r--r--   0     1001      123      113 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.graph.BidirectedEdge.rst
+-rw-r--r--   0     1001      123      107 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.graph.DirectedEdge.rst
+-rw-r--r--   0     1001      123      435 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.graph.Graph.rst
+-rw-r--r--   0     1001      123      294 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.identification.ATE.rst
+-rw-r--r--   0     1001      123      310 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.identification.AbstractCausalEstimand.rst
+-rw-r--r--   0     1001      123      122 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.identification.BidirectedEdge.rst
+-rw-r--r--   0     1001      123      295 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.identification.CATE.rst
+-rw-r--r--   0     1001      123      278 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.identification.CausalEstimand.rst
+-rw-r--r--   0     1001      123      116 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.identification.DirectedEdge.rst
+-rw-r--r--   0     1001      123      624 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.identification.Graph.rst
+-rw-r--r--   0     1001      123      140 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.identification.IdentificationResult.rst
+-rw-r--r--   0     1001      123      103 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.refutation.Operation.rst
+-rw-r--r--   0     1001      123      586 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.refutation.Result.rst
+-rw-r--r--   0     1001      123      408 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.refutation.Step.rst
+-rw-r--r--   0     1001      123       87 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.refutation.entrypoint.rst
+-rw-r--r--   0     1001      123      730 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.AbstractExpression.rst
+-rw-r--r--   0     1001      123      314 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.AbstractMath.rst
+-rw-r--r--   0     1001      123      522 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Difference.rst
+-rw-r--r--   0     1001      123      319 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.EqualityEvent.rst
+-rw-r--r--   0     1001      123      238 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Event.rst
+-rw-r--r--   0     1001      123      531 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Expectation.rst
+-rw-r--r--   0     1001      123      435 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Hedge.rst
+-rw-r--r--   0     1001      123      397 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.InterventionEvent.rst
+-rw-r--r--   0     1001      123      504 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Marginal.rst
+-rw-r--r--   0     1001      123      777 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.P.rst
+-rw-r--r--   0     1001      123      495 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Product.rst
+-rw-r--r--   0     1001      123      504 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Quotient.rst
+-rw-r--r--   0     1001      123      121 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.StatisticalEvent.rst
+-rw-r--r--   0     1001      123      477 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Value.rst
+-rw-r--r--   0     1001      123      235 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.VarSet.rst
+-rw-r--r--   0     1001      123      243 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.Variable.rst
+-rw-r--r--   0     1001      123       96 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.create_literal.rst
+-rw-r--r--   0     1001      123       60 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.do.rst
+-rw-r--r--   0     1001      123       81 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.make_vars.rst
+-rw-r--r--   0     1001      123       84 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.symbols.parse_json.rst
+-rw-r--r--   0     1001      123       95 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.attrdict.rst
+-rw-r--r--   0     1001      123      112 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.exceptions.CyclicGraphError.rst
+-rw-r--r--   0     1001      123      127 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.exceptions.DomainValidationError.rst
+-rw-r--r--   0     1001      123      127 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.exceptions.InferredDomainWarning.rst
+-rw-r--r--   0     1001      123      106 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.exceptions.NumericalError.rst
+-rw-r--r--   0     1001      123      100 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.exceptions.PQPException.rst
+-rw-r--r--   0     1001      123      121 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.exceptions.PositivityException.rst
+-rw-r--r--   0     1001      123      115 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.exceptions.UnitDomainWarning.rst
+-rw-r--r--   0     1001      123       85 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.order_graph.rst
+-rw-r--r--   0     1001      123       94 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.recursive_sort.rst
+-rw-r--r--   0     1001      123      113 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.utils.staticproperty.rst
+-rw-r--r--   0     1001      123      244 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.variable.Variable.rst
+-rw-r--r--   0     1001      123       82 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/api/pqp.variable.make_vars.rst
+-rw-r--r--   0     1001      123     1510 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/conf.py
+-rw-r--r--   0     1001      123       42 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/example_notebooks.rst
+-rw-r--r--   0     1001      123   238718 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/favicon.ico
+-rw-r--r--   0     1001      123    19314 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/imgs/frontdoor_estimator.png
+-rw-r--r--   0     1001      123    18477 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/imgs/frontdoor_new.png
+-rw-r--r--   0     1001      123    97789 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/imgs/frontdoor_viz.png
+-rw-r--r--   0     1001      123    37703 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/imgs/qs_causal_estimand.png
+-rw-r--r--   0     1001      123    75030 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/imgs/qs_stat_estimand.png
+-rw-r--r--   0     1001      123      809 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/index.rst
+-rw-r--r--   0     1001      123       24 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/data.rst
+-rw-r--r--   0     1001      123       30 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/estimation.rst
+-rw-r--r--   0     1001      123       36 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/exceptions.rst
+-rw-r--r--   0     1001      123       30 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/expression.rst
+-rw-r--r--   0     1001      123       53 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/graph.rst
+-rw-r--r--   0     1001      123       34 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/identification.rst
+-rw-r--r--   0     1001      123       30 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/refutation.rst
+-rw-r--r--   0     1001      123       27 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/symbols.rst
+-rw-r--r--   0     1001      123       28 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/module_maps/variable.rst
+-rw-r--r--   0     1001      123       46 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/modules.rst
+-rw-r--r--   0     1001      123      432 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/pqp.data.rst
+-rw-r--r--   0     1001      123      548 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/pqp.estimation.rst
+-rw-r--r--   0     1001      123      534 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/pqp.identification.rst
+-rw-r--r--   0     1001      123      340 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/pqp.refutation.rst
+-rw-r--r--   0     1001      123     1031 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/pqp.rst
+-rw-r--r--   0     1001      123     1051 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/pqp.symbols.rst
+-rw-r--r--   0     1001      123      456 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/pqp.utils.rst
+-rw-r--r--   0     1001      123     6026 2023-07-15 21:29:55.000000 pqp-0.3.5/python/docs/source/quickstart.rst
+-rw-r--r--   0     1001      123   117134 2023-07-15 21:29:55.000000 pqp-0.3.5/python/fd_case_study.ipynb
+-rw-r--r--   0     1001      123       16 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/.gitignore
+-rw-r--r--   0     1001      123      130 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/__init__.py
+-rw-r--r--   0     1001      123       60 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/data/__init__.py
+-rw-r--r--   0     1001      123     8270 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/data/data.py
+-rw-r--r--   0     1001      123     9308 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/data/domain.py
+-rw-r--r--   0     1001      123      135 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/estimation/__init__.py
+-rw-r--r--   0     1001      123     4097 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/estimation/estimator.py
+-rw-r--r--   0     1001      123     8925 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/estimation/multinomial_estimator.py
+-rw-r--r--   0     1001      123      589 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/fd_demo.py
+-rw-r--r--   0     1001      123      186 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/identification/__init__.py
+-rw-r--r--   0     1001      123     9110 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/identification/estimands.py
+-rw-r--r--   0     1001      123    13337 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/identification/graph.py
+-rw-r--r--   0     1001      123     2388 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/refutation/__init__.py
+-rw-r--r--   0     1001      123     7932 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/refutation/result.py
+-rw-r--r--   0     1001      123      241 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/symbols/__init__.py
+-rw-r--r--   0     1001      123      396 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/symbols/abstract_math.py
+-rw-r--r--   0     1001      123     3018 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/symbols/event.py
+-rw-r--r--   0     1001      123     7589 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/symbols/p.py
+-rw-r--r--   0     1001      123     1126 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/symbols/parse.py
+-rw-r--r--   0     1001      123    20412 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/symbols/relation.py
+-rw-r--r--   0     1001      123     4317 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/symbols/variable.py
+-rw-r--r--   0     1001      123       73 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/utils/__init__.py
+-rw-r--r--   0     1001      123      893 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/utils/exceptions.py
+-rw-r--r--   0     1001      123     1679 2023-07-15 21:29:55.000000 pqp-0.3.5/python/pqp/utils/utils.py
+-rw-r--r--   0     1001      123    26124 2023-07-15 21:29:55.000000 pqp-0.3.5/python/scratch.ipynb
+-rw-r--r--   0     1001      123       11 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/.gitignore
+-rw-r--r--   0     1001      123      552 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_abstract_step.py
+-rw-r--r--   0     1001      123      966 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_causal_estimand.py
+-rw-r--r--   0     1001      123     3021 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_data.py
+-rw-r--r--   0     1001      123     1690 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_domain.py
+-rw-r--r--   0     1001      123      228 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_event.py
+-rw-r--r--   0     1001      123     6346 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_examples.py
+-rw-r--r--   0     1001      123     2280 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_graph.py
+-rw-r--r--   0     1001      123     1538 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_id.py
+-rw-r--r--   0     1001      123     7724 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_multinomial_estimator.py
+-rw-r--r--   0     1001      123     2462 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_p.py
+-rw-r--r--   0     1001      123      931 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_pqp.py
+-rw-r--r--   0     1001      123      832 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_refutation.py
+-rw-r--r--   0     1001      123     3032 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_relation.py
+-rw-r--r--   0     1001      123      724 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_utils.py
+-rw-r--r--   0     1001      123     1040 2023-07-15 21:29:55.000000 pqp-0.3.5/python/tests/test_variable.py
+-rw-r--r--   0     1001      123       74 2023-07-15 21:29:55.000000 pqp-0.3.5/requirements.txt
+-rw-r--r--   0     1001      123      574 2023-07-15 21:29:55.000000 pqp-0.3.5/src/api/functions.rs
+-rw-r--r--   0     1001      123       58 2023-07-15 21:29:55.000000 pqp-0.3.5/src/api/mod.rs
+-rw-r--r--   0     1001      123      651 2023-07-15 21:29:55.000000 pqp-0.3.5/src/api/python.rs
+-rw-r--r--   0     1001      123     1364 2023-07-15 21:29:55.000000 pqp-0.3.5/src/api/test.rs
+-rw-r--r--   0     1001      123     5453 2023-07-15 21:29:55.000000 pqp-0.3.5/src/api/wrapper.rs
+-rw-r--r--   0     1001      123     9318 2023-07-15 21:29:55.000000 pqp-0.3.5/src/form/form.rs
+-rw-r--r--   0     1001      123      129 2023-07-15 21:29:55.000000 pqp-0.3.5/src/form/mod.rs
+-rw-r--r--   0     1001      123     5218 2023-07-15 21:29:55.000000 pqp-0.3.5/src/form/simplify.rs
+-rw-r--r--   0     1001      123     4151 2023-07-15 21:29:55.000000 pqp-0.3.5/src/form/test_form.rs
+-rw-r--r--   0     1001      123     6687 2023-07-15 21:29:55.000000 pqp-0.3.5/src/form/test_simplify.rs
+-rw-r--r--   0     1001      123     3459 2023-07-15 21:29:55.000000 pqp-0.3.5/src/form/tikka.rs
+-rw-r--r--   0     1001      123     2552 2023-07-15 21:29:55.000000 pqp-0.3.5/src/graph/bigraph.rs
+-rw-r--r--   0     1001      123     4865 2023-07-15 21:29:55.000000 pqp-0.3.5/src/graph/digraph.rs
+-rw-r--r--   0     1001      123      303 2023-07-15 21:29:55.000000 pqp-0.3.5/src/graph/graph.rs
+-rw-r--r--   0     1001      123     2075 2023-07-15 21:29:55.000000 pqp-0.3.5/src/graph/graph_builder.rs
+-rw-r--r--   0     1001      123      296 2023-07-15 21:29:55.000000 pqp-0.3.5/src/graph/mod.rs
+-rw-r--r--   0     1001      123      373 2023-07-15 21:29:55.000000 pqp-0.3.5/src/graph/node.rs
+-rw-r--r--   0     1001      123     5763 2023-07-15 21:29:55.000000 pqp-0.3.5/src/graph/tests.rs
+-rw-r--r--   0     1001      123       64 2023-07-15 21:29:55.000000 pqp-0.3.5/src/identification/mod.rs
+-rw-r--r--   0     1001      123     3689 2023-07-15 21:29:55.000000 pqp-0.3.5/src/identification/shpitser.rs
+-rw-r--r--   0     1001      123     6682 2023-07-15 21:29:55.000000 pqp-0.3.5/src/identification/tests.rs
+-rw-r--r--   0     1001      123      154 2023-07-15 21:29:55.000000 pqp-0.3.5/src/lib.rs
+-rw-r--r--   0     1001      123      368 2023-07-15 21:29:55.000000 pqp-0.3.5/src/model/examples.rs
+-rw-r--r--   0     1001      123       93 2023-07-15 21:29:55.000000 pqp-0.3.5/src/model/mod.rs
+-rw-r--r--   0     1001      123     6195 2023-07-15 21:29:55.000000 pqp-0.3.5/src/model/model.rs
+-rw-r--r--   0     1001      123     2565 2023-07-15 21:29:55.000000 pqp-0.3.5/src/model/order.rs
+-rw-r--r--   0     1001      123     4253 2023-07-15 21:29:55.000000 pqp-0.3.5/src/model/tests.rs
+-rw-r--r--   0     1001      123      795 2023-07-15 21:29:55.000000 pqp-0.3.5/src/test.rs
+-rw-r--r--   0     1001      123      304 2023-07-15 21:29:55.000000 pqp-0.3.5/src/utils/defaults.rs
+-rw-r--r--   0     1001      123       99 2023-07-15 21:29:55.000000 pqp-0.3.5/src/utils/mod.rs
+-rw-r--r--   0     1001      123     2185 2023-07-15 21:29:55.000000 pqp-0.3.5/src/utils/set_utils.rs
+-rw-r--r--   0     1001      123      987 2023-07-15 21:29:55.000000 pqp-0.3.5/src/utils/tests.rs
+-rw-r--r--   0     1001      123      612 2023-07-15 21:29:55.000000 pqp-0.3.5/src/utils/utils.rs
+-rw-r--r--   0     1001      123       49 2023-07-15 21:29:55.000000 pqp-0.3.5/test.sh
+-rw-r--r--   0     1001      123   150084 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-01-14-13-06-10.png
+-rw-r--r--   0     1001      123    51282 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-01-14-13-52-24.png
+-rw-r--r--   0     1001      123    53166 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-01-14-14-22-06.png
+-rw-r--r--   0     1001      123   118082 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-01-14-15-01-52.png
+-rw-r--r--   0     1001      123    45879 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-02-25-09-07-36.png
+-rw-r--r--   0     1001      123    50872 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-02-25-09-22-50.png
+-rw-r--r--   0     1001      123   367476 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-33-14.png
+-rw-r--r--   0     1001      123   325115 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-33-44.png
+-rw-r--r--   0     1001      123   213508 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-34-19.png
+-rw-r--r--   0     1001      123   336724 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-34-30.png
+-rw-r--r--   0     1001      123   349974 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-34-44.png
+-rw-r--r--   0     1001      123   407521 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-35-39.png
+-rw-r--r--   0     1001      123   115292 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-36-00.png
+-rw-r--r--   0     1001      123   476032 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-36-57.png
+-rw-r--r--   0     1001      123   345389 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/2023-04-02-14-37-10.png
+-rw-r--r--   0     1001      123   108822 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/PQP a Library for End-to-End Causal Inference.ipynb
+-rw-r--r--   0     1001      123   197652 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/PQP.ipynb
+-rw-r--r--   0     1001      123    36229 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/Performant Conditional Query Identification in Structural Causal Models.ipynb
+-rw-r--r--   0     1001      123   117397 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/agg.ipynb
+-rw-r--r--   0     1001      123      882 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/build.py
+-rw-r--r--   0     1001      123    16499 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/demo.ipynb
+-rw-r--r--   0     1001      123     8008 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/demo1.csv
+-rw-r--r--   0     1001      123    27322 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/doctordemo.csv
+-rw-r--r--   0     1001      123    14520 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/examples.ipynb
+-rw-r--r--   0     1001      123     1756 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/grab_code.py
+-rw-r--r--   0     1001      123     1738 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/scratch.ipynb
+-rw-r--r--   0     1001      123     6485 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/speed.ipynb
+-rw-r--r--   0     1001      123      678 2023-07-15 21:29:55.000000 pqp-0.3.5/writeup/supplement.py
+-rw-r--r--   0     1001      123     9185 2023-07-15 21:29:55.000000 pqp-0.3.5/Cargo.lock
+-rw-r--r--   0        0        0     2286 1970-01-01 00:00:00.000000 pqp-0.3.5/PKG-INFO
```

### Comparing `pqp-0.3.4/.coverage` & `pqp-0.3.5/.coverage`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/.github/workflows/CI.yml` & `pqp-0.3.5/.github/workflows/build_release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is autogenerated by maturin v1.1.0
 # To update, run
 #
 #    maturin generate-ci github
 #
-name: CI
+name: build_release
 
 on:
   push:
     branches:
       - main
       - master
     tags:
```

### Comparing `pqp-0.3.4/CHANGELOG.md` & `pqp-0.3.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/CONTRIBUTING.md` & `pqp-0.3.5/CONTRIBUTING.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 ```bash
 # run in root of repo
 source test.sh
 ```
 
 ## Documentation
 
-To build the documentation, use the makefile in the `docs` directory:
+To build the documentation, use the makefile in the `docs` directory. Make sure you have installed the dev dependencies.
 
 ```bash
 # run in root of repo
-cd python/pqp/docs
+cd python/docs
 
 # regenerate documentation source (only run when adding new modules)
 make autodoc
 
 # build html documentation (runs local development server)
 make livehtml
 ```
```

### Comparing `pqp-0.3.4/LICENSE.txt` & `pqp-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/README.md` & `pqp-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/pyproject.toml` & `pqp-0.3.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 [project]
 name = "pqp"
-version = "0.3.4"
+version = "0.3.5"
 description = "Subroutines for structural causal modeling"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Leo Ware"}]
 dependencies = [
     "pandas",
     "numpy",
-    "tomli",
-    "matplotlib"
+    "tomli"
 ]
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["causal inference", "causal identification"]
 
 [project.optional-dependencies]
+dataviz = [
+    "matplotlib",
+    "networkx"
+]
 dev = [
     "sphinx",
     "maturin",
     "sphinx-autobuild",
+    "sphinx_automodapi",
     "pytest",
     "networkx",
 ]
 
 [project.urls]
 Homepage = "https://leo-ware.github.io/capstone/"
 Source = "https://github.com/leo-ware/capstone"
```

### Comparing `pqp-0.3.4/python/docs/Makefile` & `pqp-0.3.5/python/docs/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 
 livehtml:
-	sphinx-autobuild "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	sphinx-autobuild "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O) --port 7000
 
 autodoc:
 	sphinx-apidoc -f -o "$(SOURCEDIR)" "$(PACKAGEDIR)"
 
 build:
 	sphinx-build "$(SOURCEDIR)" "$(BUILDDIR)"
```

### Comparing `pqp-0.3.4/python/docs/make.bat` & `pqp-0.3.5/python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/api/pqp.estimation.Estimator.rst` & `pqp-0.3.5/python/docs/source/api/pqp.estimation.Estimator.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst` & `pqp-0.3.5/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/api/pqp.identification.Graph.rst` & `pqp-0.3.5/python/docs/source/api/pqp.identification.Graph.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/api/pqp.refutation.Result.rst` & `pqp-0.3.5/python/docs/source/api/pqp.refutation.Result.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/api/pqp.symbols.AbstractExpression.rst` & `pqp-0.3.5/python/docs/source/api/pqp.symbols.AbstractExpression.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/api/pqp.symbols.Difference.rst` & `pqp-0.3.5/python/docs/source/api/pqp.symbols.Difference.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/api/pqp.symbols.Expectation.rst` & `pqp-0.3.5/python/docs/source/api/pqp.symbols.Expectation.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/api/pqp.symbols.P.rst` & `pqp-0.3.5/python/docs/source/api/pqp.symbols.P.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/conf.py` & `pqp-0.3.5/python/docs/source/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 import os
 import sys
 import toml
 import datetime
-sys.path.insert(0, os.path.abspath('../..'))
+sys.path.insert(0, os.path.abspath('../pqp'))
 
 # -- Project information -----------------------------------------------------
 # DO NOT EDIT!!! This information is automatically generated from pyproject.toml
 
 with open("../../../pyproject.toml") as f:
     pyproject = toml.load(f)["project"]
 
@@ -26,15 +26,16 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.napoleon',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.githubpages',
-    'sphinx_automodapi.automodapi'
+    'sphinx_automodapi.automodapi',
+    'sphinx.ext.doctest'
 ]
 
 templates_path = ['_templates']
 exclude_patterns = []
 numpydoc_show_class_members = False
```

### Comparing `pqp-0.3.4/python/docs/source/favicon.ico` & `pqp-0.3.5/python/docs/source/favicon.ico`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/imgs/frontdoor_estimator.png` & `pqp-0.3.5/python/docs/source/imgs/frontdoor_estimator.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/imgs/frontdoor_new.png` & `pqp-0.3.5/python/docs/source/imgs/frontdoor_new.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/imgs/frontdoor_viz.png` & `pqp-0.3.5/python/docs/source/imgs/frontdoor_viz.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/imgs/qs_causal_estimand.png` & `pqp-0.3.5/python/docs/source/imgs/qs_causal_estimand.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/imgs/qs_stat_estimand.png` & `pqp-0.3.5/python/docs/source/imgs/qs_stat_estimand.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/index.rst` & `pqp-0.3.5/python/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/pqp.estimation.rst` & `pqp-0.3.5/python/docs/source/pqp.estimation.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/pqp.identification.rst` & `pqp-0.3.5/python/docs/source/pqp.identification.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/pqp.symbols.rst` & `pqp-0.3.5/python/docs/source/pqp.symbols.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/docs/source/quickstart.rst` & `pqp-0.3.5/python/docs/source/quickstart.rst`

 * *Files 18% similar despite different names*

```diff
@@ -19,27 +19,30 @@
 #. **Causal Estimand**: an algebraic expression representing the causal effect of interest
 
 Setup
 ++++++
 
 To get started, we will spoof some data to run our analysis on.
 
-.. code-block:: python
+.. testcode::
 
     import pandas as pd
 
     df = pd.DataFrame({
         "x": [0, 0, 0, 1, 1, 0],
         "z": [0, 1, 0, 1, 1, 0],
         "y": [0, 1, 0, 1, 1, 0],
     })
 
+.. testoutput::
+    print(5)
+
 We can use the ``make_vars`` function to create a list of variables.
 
-.. code-block:: python
+.. testcode::
 
     from pqp.symbols import make_vars
     x, y, z = make_vars("xyz")
 
 Note that the names of these variables match the column names in the data frame.
 
 Causal Assumptions
@@ -48,40 +51,40 @@
 We can then assemble these variables into a causal diagram using the ``Graph`` class. Here we will
 build the famous front-door model.
 
 Infix operators are used to construct causal relationships.  The ``<=`` operator is used to 
 indicate causal influence from right to left, while the ``&`` operator is used to indicate
 confounding.
 
-.. code-block:: python
+.. testcode::
 
     from pqp.identification import Graph
     g = Graph([
         x & y,
         z <= x,
         y <= z,
     ])
 
 We can use the ``.draw()`` method to visualize the causal diagram.
 
-.. code-block:: python
+.. testcode::
 
     g.draw()
 
 .. image:: imgs/frontdoor_viz.png
     :width: 400px
 
 
 Parametric Assumptions
 +++++++++++++++++++++++
 
 For the purposes of this article, we will assume that the data is drawn from a multinomial
 distribution. We can use the ``MultinomialEstimator`` class to specify the parametric assumptions.
 
-.. code-block:: python
+.. testcode::
 
     from pqp.estimation import MultinomialEstimator
     estimator = MultinomialEstimator(df, prior=1)
 
 The ``prior`` argument specifies the prior strength of the model.  The default is
 zero, in which case the model fits through maximum likelihood. We are using a nonzero
 value here because if you don't specify a prior, the model will not always give positive
@@ -92,24 +95,24 @@
 
 Causal Estimand
 ++++++++++++++++
 
 For this example, we will estimate the average treatment effect of ``x`` on ``y``. First, 
 we need to define the treatment and control conditions.
 
-.. code-block:: python
+.. testcode::
 
     treatment_condition = [x.val == 1]
     control_condition = [x.val == 0]
 
 Then, we can use the ``ATE`` class to define the causal estimand.
 
-.. code-block:: python
+.. testcode::
 
-    from pqp.estimation import ATE
+    from pqp.identification import ATE
     causal_estimand = ATE(y, treatment_condition, control_condition)
     
     #inspect the expression
     causal_estimand.expression().display()
 
 .. image:: imgs/qs_causal_estimand.png
     :width: 500px
@@ -119,25 +122,25 @@
 
 Now, we can first use the causal assumptions to identify the causal estimand, and then we can use the
 parametric assumptions to estimate the causal effect.
 
 To identify the causal relationships in the causal diagram, we can use the ``.identify()`` method.
 For example, to identify the causal relationship between ``x`` and ``y``, we can use the following:
 
-.. code-block:: python
+.. testcode::
 
     estimand = g.identify(causal_estimand).identified_estimand
     estimand.display()
 
 .. image:: imgs/qs_stat_estimand.png
     :width: 600px
 
 We can then use the ``.estimate()`` method to estimate the causal effect.
 
-.. code-block:: python
+.. testcode::
 
     effect = estimator.estimate(estimand)
     effect
     # => EstimationResult(value=0.4433808167141502)
 
 
 Interpretability and Robustness
@@ -145,15 +148,15 @@
 
 One of the most important features of ``pqp`` is its ability to provide human-interpretable explanations of the workings of the code. Many of the routines make very specific assumptions about the structure of the data or the effects of interest. It's important for users to understand these assumptions so they can understand the potential limitations of an analysis.
 
 The currency of ``pqp`` is the ``Result`` class. Any calculations that draw conclusions from the data will return instances of this class. This class tracks the transformations and assumptions made by the algorithms. As ``Results`` are assembled into successively more complex analyses of the data, ``pqp`` builds a dependency graph which tracks how different ``Result`` instances relate to each other and allows the user access to a list of steps executed in an analysis and the assumptions made.
 
 To access the list of steps, we can use the ``.explain()`` and ``explain_all()`` methods, which detail the current result only or all results in the dependency graph, respectively.
 
-.. code-block:: python
+.. testcode::
 
     estimator.estimate(estimand).explain()
 
 Output:
 
 .. code-block::
```

### Comparing `pqp-0.3.4/python/fd_case_study.ipynb` & `pqp-0.3.5/python/fd_case_study.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/pqp/data/data.py` & `pqp-0.3.5/python/pqp/data/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,53 +4,55 @@
 from pqp.utils import attrdict
 from pqp.symbols.variable import Variable
 from pqp.data.domain import make_domain, Domain, CategoricalDomain
 from pqp.utils.exceptions import InferredDomainWarning, UnitDomainWarning
 from pqp.refutation import Result, Operation, Step
 
 class Data(Result):
-    def __init__(self, df, vars=None, validate_domain=True, **kwargs):
-        """Class representing datasets, wraps a pandas DataFrame and contains some metadata
+    """Class representing datasets, wraps a pandas DataFrame and contains some metadata
 
         The main job of this class is to validate/create a set of symbolic variables that 
-        align with the columns names on `df`.
+        align with the columns names on ``df``.
 
         Examples:
 
-        >> df = pd.DataFrame({"x": [1, 2, 3], "y": [4, 5, 6]})
-        >> # it can infer a discrete domain for the variables
-        >> Data(df, vars=[Variable("x"), Variable("y")])
-        >> Data(df, vars={"x": Variable("X"), "y": Variable("Y")}) # capitalizes names
-
-        >> # or you can specify the domain explicitly
-        >> Data(df, vars={"x": DiscreteDomain([1, 2, 3, 4, 6]), "y": ContinuousDomain([1, 10])})
-        >> Data(df, vars={"x": "discrete", "y": "continuous"})
-        >> Data(df, vars={"x": None, "y": None}) # specifies an unknown domain
-
-        >> # examples of invalid calls
-        >> Data(df, vars={"x": Variable("x"), "z": Variable("z")}) # z not in df
-        >> Data(df, vars={"x": Variable("x"), "y": "some name"}) # "some name" is interpreted as a domain type
+        >>> df = pd.DataFrame({"x": [1, 2, 3], "y": [4, 5, 6]})
+        >>> # it can infer a discrete domain for the variables
+        >>> Data(df, vars=[Variable("x"), Variable("y")])
+        >>> Data(df, vars={"x": Variable("X"), "y": Variable("Y")})
+
+        >>> # or you can specify the domain explicitly
+        >>> Data(df, vars={"x": DiscreteDomain([1, 2, 3, 4, 6]), "y": ContinuousDomain([1, 10])})
+        >>> Data(df, vars={"x": "discrete", "y": "continuous"})
+        >>> Data(df, vars={"x": None, "y": None}) # specifies a domain of unknown type
+        
+        >>> # examples of invalid calls
+        >>> Data(df, vars={"x": Variable("x"), "z": Variable("z")}) # z not in df
+        >>> Data(df, vars={"x": Variable("x"), "y": "some name"}) # "some name" is interpreted as a domain type
 
 
         Args:
-            df (pandas.DataFrame): the dataset
-            vars (list or dict): the variables in the dataset, either a list of `Variable` (names
-                must match columns in `df`) or a `dict` mapping column names in `df` to `Variable` 
-                or str specifying the type of the variable's domain
-            validate_domain (bool): if False, do not validate that the data conforms to the domains 
-                specified, defaults to True
-            silence_inferred_domain_warning (bool): if True, silences the default warning when
+            df (``pandas.DataFrame``): the dataset
+            vars (``list`` or ``dict``): the variables in the dataset, either a list of ``Variable`` (names
+                must match columns in ``df``) or a ``dict`` mapping column names in ``df`` to ``Variable`` 
+                or ``str`` specifying the type of the variable's domain
+            validate_domain (``bool``): if ``False``, do not validate that the data conforms to the domains 
+                specified, defaults to ``True``
+            silence_inferred_domain_warning (``bool``): if ``True``, silences the default warning when
                 the domain of a variable is inferred
-            silence_unit_domain_warning (bool): if True, silences the default warning when an inferred
+            silence_unit_domain_warning (``bool``): if ``True``, silences the default warning when an inferred
                 domain for a variable has only a single possible value
         
         Attributes:
-            df (pandas.DataFrame): the dataset
-            vars (dict): a dict mapping variable names to `Variable` objects
+            df (``pandas.DataFrame``): The dataset
+            vars (``dict``): ``dict`` mapping variable names to ``Variable`` objects
         """
+    
+    def __init__(self, df, vars=None, validate_domain=True, **kwargs):
+        
         self.step = Step("Data Processing")
         self.operation = Operation(self.__init__, [df], {"vars": vars, "validate_domain": validate_domain, **kwargs})
 
         self._silence_inferred_domain_warning = kwargs.get("silence_inferred_domain_warning", True)
         self._silence_unit_domain_warning = kwargs.get("silence_unit_domain_warning", False)
 
         if not isinstance(df, pd.DataFrame):
@@ -137,28 +139,48 @@
         for name, var in self.vars.items():
             if var.domain == None:
                 raise ValueError(f'Variable "{var}" has no domain')
             var.domain.validate_or_throw(self.df[name])
     
     @property
     def n(self):
+        """The number of rows in the dataset"""
         return self.df.shape[0]
     
     def domain_of(self, var):
+        """Get the domain of a variable
+
+        Args:
+            var (``str`` or ``Variable``): the variable whose domain to get
+        
+        Returns:
+            ``Domain``: the domain of the variable
+        """
         if isinstance(var, Variable):
             var = var.name
         try:
             return self.vars[var].domain
         except KeyError:
             raise ValueError(f'{repr(var)} not found in vars')
     
     def _domains(self):
         return {var: var.domain for var in self.vars.values()}
     
     def quantize(self, var, n_bins=2):
+        """Quantize a variable in place
+
+        Turns a continuous variable into a categorical variable by binning it into ``n_bins`` bins.
+
+        Args:
+            var (``str`` or ``Variable``): the variable to quantize
+            n_bins (``int``): the number of bins to quantize into
+        
+        Returns:
+            ``None``
+        """
         step = self.step.substep(f'Quantizing {var} into {n_bins} bins')
         if isinstance(var, Variable):
             var = var.name        
         quantized = pd.cut(self.df[var], n_bins)
         for el in np.unique(quantized):
             step.write(f"Mapping elements on ({el.left}, {el.right}] to {el.mid}")
         self.df[var] = np.array([i.mid for i in quantized])
```

### Comparing `pqp-0.3.4/python/pqp/data/domain.py` & `pqp-0.3.5/python/pqp/data/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,59 +9,83 @@
     @abc.abstractmethod
     def get_cardinality(self):
         """The number of possible values a variable can take on"""
         raise NotImplementedError
     
     @abc.abstractmethod
     def __contains__(self, value):
-        """Returns whether a value is in the domain"""
+        """Returns whether a value is in the domain
+        
+        Args:
+            value: the value to check
+        
+        Returns:
+            ``bool``: True if the value is in the domain, False otherwise
+        """
         raise NotImplementedError
     
     @abc.abstractmethod
     def describe_assumptions(self):
-        """Describes any assumptions made about the domain"""
+        """Returns a human readable description of assumptions made about the domain"""
         pass
     
     def validate(self, values):
         """Validates that a list of values is in the domain
 
         Args:
-            values (list): a list of values to validate
+            values (``list``): a list of values to validate
 
         Returns:
-            bool: True if all values are in the domain, False otherwise
+            ``bool``: ``True`` if all values are in the domain, ``False`` otherwise
         """
         return all([value in self for value in values])
     
     def validate_or_throw(self, values):
         """Validates that a list of values is in the domain, throws an error if not
 
         Args:
-            values (list): a list of values to validate
+            values (``list``): a list of values to validate
 
         Raises:
-            ValueError: if any value is not in the domain
+            ``ValueError``: if any value is not in the domain
         """
         for val in values:
             if not val in self:
                 raise DomainValidationError(f"Value {val} is not in domain {self}")
 
 class DiscreteDomain(Domain, abc.ABC):
     """Abstract base class for discrete domains"""
     @abc.abstractmethod
     def get_values(self):
-        """Returns a list of all possible values in the domain"""
+        """Returns a list of all possible values in the domain
+        
+        Returns:
+            ``list``: all possible values in the domain
+        """
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def get_cardinality(self):
+        """Calculates the cardinality of the domain
+
+        Returns:
+            ``int``: the number of possible values in the domain
+        """
         raise NotImplementedError
 
 class IntegerDomain(DiscreteDomain):
     def __init__(self, values):
         """Domain for which a variable is an integer in an (inclusive) range
 
         Args:
-            values (list): a list of integers, max and min of which are bounds of the range
+            values (``list``): a list of integers, max and min of which are bounds of the range
+        
+        Attributes:
+            min (``int``): the minimum value in the domain (inclusive)
+            max (``int``): the maximum value in the domain (inclusive)
         """
         try:
             values = list(values)
         except TypeError:
             raise ValueError("values must be an iterable")
         
         self.min = int(np.min(values))
@@ -72,14 +96,15 @@
             "We assume the variable is an integer in the range [{self.min}, {self.max}] inclusive"
         )
     
     def get_values(self):
         return list(range(self.min, self.max + 1))
     
     def check_int(self, val):
+        """Checks whether a value is an integer"""
         return int(val) == val
     
     def get_cardinality(self):
         return self.max - self.min + 1
     
     def __repr__(self):
         return f"IntegerDomain([{self.min}, {self.max}])"
@@ -94,15 +119,15 @@
 
 class CategoricalDomain(DiscreteDomain):
     """Domain of a categorical variable"""
     def __init__(self, values):
         """Represents a categorical domain for a variable, specified by a list of values
 
         Args:
-            values (list): a list, unique elements of which are possible values for the variable
+            values (``list``): a ``list``, unique elements of which are possible values for the variable
         """
         try:
             values = list(values)
         except TypeError:
             raise ValueError("Discrete domains must specify values")
         self.values = set(values)
     
@@ -158,15 +183,15 @@
     def get_cardinality(self):
         return float("inf")
 
 class RealDomain(ContinuousDomain):
     """A continuous domain for a variable, delimited by min and max values
 
     Args:
-        values (list): the min and max of this list are taken as the min and max of the domain
+        values (``list``): the min and max of this list are taken as the min and max of the domain
     """
     def __init__(self, values):
         try:
             values = list(values)
         except TypeError:
             raise ValueError("Continuous domains must specify values")
         self.min = np.min(values)
@@ -222,19 +247,19 @@
         return 'continuous'
     else:
         return 'discrete'
 
 def infer_domain_type(vals):
     """Attempts to infer the best domain type to use of a list of values
 
-    The rules for determining this are somewhat complicated. You should run this and
+    The heuristics are somewhat complicated. You should run this and
     inspect the result before use.
 
     Args:
-        vals (iterable): a list of values to infer the domain type of
+        vals (``Iterable``): a ``list`` of values to infer the domain type of
     """
     try:
         iter(vals)
     except TypeError:
         raise TypeError("vals must be iterable")
 
     if isinstance(vals, pd.Series) or isinstance(vals, np.ndarray):
@@ -242,30 +267,30 @@
     else:
         return _infer_domain_type_values(vals)
 
 def make_domain(domain_type, values=None):
     """Generates a domain object from a string and optional values
 
     Options:
-        discrete: values must be specified
-        continuous: min and max of `values` used to specify domain
-        binary: values are ignored
-        integer: min and max of `values` used to specify domain
-        infer: attempt to guess
+        * ``"discrete"``: values must be specified
+        * ``"continuous"``: min and max of ``values`` used to specify domain
+        * ``"binary"``: values are ignored
+        * ``"integer"``: min and max of ``values`` used to specify domain
+        * ``"infer"``: attempt to guess
     
     Args:
-        domain_type (str): one of 'discrete', 'continuous', 'integer', 'binary' or 'infer'
-        values (list): the values of the domain
+        domain_type (``str``): one of ``"discrete"``, ``"continuous"``, ``"binary"``, ``"integer"``, or ``"infer"``
+        values (``list``): the values of the domain
 
     """
     if domain_type == "discrete":
         return CategoricalDomain(values)
     elif domain_type == "continuous":
         return RealDomain(values)
     elif domain_type == "binary":
         return BinaryDomain()
     elif domain_type == "integer":
         return IntegerDomain(values)
     elif domain_type == "infer":
         return make_domain(infer_domain_type(values), values)
     else:
-        raise ValueError(f"Invalid domain type {domain_type}, must be one of 'discrete', 'continuous', or 'binary'")
+        raise ValueError(f"Invalid domain type {domain_type}")
```

### Comparing `pqp-0.3.4/python/pqp/estimation/estimator.py` & `pqp-0.3.5/python/pqp/estimation/estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,55 +25,55 @@
         super().__init__(op, step)
 
     @abstractmethod
     def estimate(self, expr: AbstractExpression, assignments=None):
         """Estimate the value of an expression
 
         Args:
-            expr (AbstractExpression): The expression to estimate
-            assignments (dict): dict of variable assignments (optional)
+            expr (``AbstractExpression``): The expression to estimate
+            assignments (``dict``): ``dict`` of variable assignments (optional)
         
         Returns:
             EstimationResult: the result of the estimation
         """
         pass
     
     @abstractmethod
     def get_observed(self):
         """Return the set of Variables that are considered observed in the model
         
         Returns:
-            set: the set of observed variables
+            ``set``: the observed variables
         """
         pass
 
     @abstractmethod
     def domain_of(self, var):
-        """Return the domain of a variable
+        """Return the domain of a Variable
         
         Args:
-            var (Variable or str): The variable to get the domain of
+            var (``Variable`` or ``str``): The variable to get the domain of
         
         Returns:
-            Domain: the domain of the variable
+            ``Domain``: the domain of the variable
         """
         pass
 
     def __repr__(self):
         return f"{self.__class__.__name__}(observed=[{', '.join(map(str, self.get_observed()))}])"
 
     def approx(self, expr, assignments=None):
-        """Approximated the value of an expression
+        """Approximates the value of an expression
 
         Args:
-            expr (AbstractExpression): The expression to approximate
-            assignments (dict): dict of variable assignments (optional)
+            expr (``AbstractExpression``): The expression to approximate
+            assignments (``dict``): variable assignments (optional)
         
         Returns:
-            float: the approximate value of the expression
+            ``float``: the approximate value of the expression
         """
         if not isinstance(expr, AbstractExpression) and not (isinstance(expr, Result) and hasattr(expr, "statistical_estimand")):
             raise TypeError("expr must be an AbstractExpression object or Result")
         
         if isinstance(expr, Result):
             id_result = expr
             expr = expr.statistical_estimand
```

### Comparing `pqp-0.3.4/python/pqp/estimation/multinomial_estimator.py` & `pqp-0.3.5/python/pqp/estimation/multinomial_estimator.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/pqp/fd_demo.py` & `pqp-0.3.5/python/pqp/fd_demo.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/pqp/identification/estimands.py` & `pqp-0.3.5/python/pqp/identification/estimands.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,24 +12,24 @@
         raise NotImplementedError()
     
     @abstractmethod
     def expression(self):
         """Derive the expression for the causal estimand
         
         Returns:
-            AbstractExpression: the expression for the causal estimand
+            ``AbstractExpression``: the expression for the causal estimand
         """
         raise NotImplementedError()
     
     @abstractmethod
     def literal(self):
         """The estimand represented as a function call, as an Expression
         
         Returns:
-            AbstractExpression: the literal for the causal estimand
+            ``AbstractExpression``: the literal for the causal estimand
         """
         raise NotImplementedError()
     
     def display(self):
         """Display the causal estimand"""
         from IPython.display import display, Math
         tex = self.literal().to_latex() + " = " + self.expression().to_latex()
@@ -53,32 +53,32 @@
         return self.__class__.LITERAL_CLASS(self.exp)
 
 class ATE(AbstractCausalEstimand):
     """Causal estimand for the average treatment effect
 
     To define the average treatment effect, it's necessary to specify what is meant
     by "treatment" and "control" in this context. You can do this by passing either
-    a dict or a list of StatisticalEvent objects to each of the treatment_condition
-    and control_condition arguments. If a dict is passed, the keys must be Variable
-    or string, and the values must not be Variable. If a list is passed, it must 
-    contain only instances of StatisticalEvent.
+    a ``dict`` or a list of ``StatisticalEvent`` objects to each of the ``treatment_condition``
+    and ``control_condition`` arguments. If a ``dict`` is passed, the keys must be ``Variable``
+    or ``str``, and the values must not be ``Variable``. If a ``list`` is passed, it must 
+    contain only instances of ``StatisticalEvent``.
 
     Example:
         >>> # treatment condition is x = 1, control condition is x = 0 in both of these
         >>> ATE(outcome, treatment_condition={"x": 1}, control_condition={"x": 0})
         >>> ATE(outcome, treatment_condition=[EqualityEvent("x", 1)], control_condition=[EqualityEvent("x", 0)])
         >>>
         >>> # treatment condition is x = 1 and y = "red", control condition is x = 0 and y = "blue"
         >>> ATE(outcome, treatment_condition={"x": 1, y: "red"}, control_condition={"x": 0, y: "blue"})
         
     
     Args:
-        outcome (Variable): the outcome variable
-        treatment_condition (dict or list): the treatment condition
-        control_condition (dict or list): the control condition
+        outcome (``Variable``): the outcome variable
+        treatment_condition (``dict`` or ``list``): the treatment condition
+        control_condition (``dict`` or ``list``): the control condition
     """
     LITERAL_CLASS = create_literal("ATE", arity=2, sep=" | ", name_tex="\\text{ATE}", sep_tex=" \\mid ")
 
     def __init__(self, outcome, treatment_condition, control_condition=None):
         super().__init__()
         self.name = "average treatment effect"
 
@@ -141,19 +141,19 @@
 
 class CATE(ATE):
     """Causal estimand for the conditional average treatment effect
 
     To define the conditional average treatment effect, it's necessary to specify 
     what is meant by treatment and control in this context, and you need to specify the
     subpopulation in which to measure the effect. You can 
-    do this by passing either a dict or a list of StatisticalEvent objects to 
-    each of the treatment_condition and control_condition arguments. If a dict 
-    is passed, the keys must be Variable or string, and the values must not 
-    be Variable. If a list is passed, it must contain only instances of 
-    StatisticalEvent.
+    do this by passing either a ``dict`` or a list of ``StatisticalEvent`` objects to 
+    each of the ``treatment_condition`` and ``control_condition`` arguments. If a ``dict`` 
+    is passed, the keys must be ``Variable`` or ``string``, and the values must not 
+    be ``Variable``. If a ``list`` is passed, it must contain only instances of 
+    ``StatisticalEvent``.
 
     Example:
         >>> # treatment condition is x = 1, control condition is x = 0 in both of these
         >>  # in both, we are measuring the effect in the subpopulation where z = 1
         >>> CATE(outcome, treatment_condition={"x": 1}, control_condition={"x": 0}, subpopulation={"z": 1})
         >>> CATE(
         ...     outcome,
@@ -169,18 +169,18 @@
         ...     treatment_condition={"x": 1, y: "red"},
         ...     control_condition={"x": 0, y: "blue"},
         ...     subpopulation={"z": 1}
         ... )
         
     
     Args:
-        outcome (Variable): the outcome variable
-        treatment_condition (dict or list): the treatment condition
-        control_condition (dict or list): the control condition
-        subpopulation (dict or list): the subpopulation in which to measure the effect
+        outcome (``Variable``): the outcome variable
+        treatment_condition (``dict`` or ``list``): the treatment condition
+        control_condition (``dict`` or ``list``): the control condition
+        subpopulation (``dict`` or ``list``): the subpopulation in which to measure the effect
     """
     LITERAL_CLASS = create_literal("CATE", arity=3, sep=" | ", name_tex="\\text{CATE}", sep_tex=" \\mid ")
     def __init__(self, outcome, treatment_condition, control_condition, subpopulation):
         super().__init__(outcome, treatment_condition, control_condition)
         self.name = "conditional average treatment effect"
         self.subpopulation = self._validate_condition(subpopulation, "subpopulation")
```

### Comparing `pqp-0.3.4/python/pqp/identification/graph.py` & `pqp-0.3.5/python/pqp/identification/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 from itertools import chain
 
 class IdentificationResult(Result):
     """Stores the result of identification
 
     Attributes:
-        identified_estimand (AbstractExpression): the identified causal estimand
+        identified_estimand (``AbstractExpression``): the identified causal estimand
     """
     _keys = ["identified_estimand"]
 
 
 @dataclass(frozen=True)
 class SearchNode:
     prev: Optional["SearchNode"]
@@ -33,16 +33,16 @@
         if self.prev is not None:
             self.prev.unpack(_path=_path)
 
 
 class Graph:
     """A causal graph
 
-    The best way to create a `Graph` is using the `<=` and `&` infix operators. When you use
-    these operators between `Variable`s, they create a `DirectedEdge` or `BidirectedEdge` respectively.
+    The best way to create a ``Graph`` is using the ``<=`` and ``&`` infix operators. When you use
+    these operators between ``Variable`` s, they create a ``DirectedEdge`` or ``BidirectedEdge`` respectively.
 
     Example: The Front-Door Model
         >>> x, y, m = make_vars("xym")
         >>> g = Graph([
         ...     m <= x,
         ...     y <= m,
         ...     y & x,
@@ -51,72 +51,72 @@
     Example: The Back-Door Model
         >>> x, y, z = make_vars("xyz")
         >>> g = Graph([
         ...     y <= [x, z],
         ...     x <= z,
         ... ])
 
-    You can use the `identify` method to identify a causal estimand. The estimand can either
-    be passed as an expression or as an instance of `AbstractCausalEstimand`, such as `ATE` or
-    `CATE`.
+    You can use the ``identify`` method to identify a causal estimand. The estimand can either
+    be passed as an expression or as an instance of ``AbstractCausalEstimand``, such as ``ATE`` or
+    ``CATE``.
 
     Example:
         >>> x = Variable("X")
         >>> y = Variable("Y")
         >>> g = Graph([
         ...     y <= x,
         ... ])
         >>> g.identify(ATE([y], [x]))
         P(y | x)
     
     Args:
-        edges (list of DirectedEdge or BidirectedEdge): the edges in the graph
+        edges (``list`` of ``DirectedEdge`` or ``BidirectedEdge``): the edges in the graph
     """
     def __init__(self, edges=[]):
         self.bi_edges = []
         self.directed_edges = []
         self.nodes = set()
         self.add_edges(edges)
     
     def add_node(self, node):
         """Adds a node to the graph
         
         Args:
-            node (Variable): the node to add
+            node (``Variable``): the node to add
         """
         self.nodes.add(node)
     
     def add_nodes(self, nodes):
         """Adds multiple nodes to the graph
         
         Args:
-            nodes (list of Variable): the nodes to add
+            nodes (``list`` of ``Variable``): the nodes to add
         """
         self.nodes.update(nodes)
     
     def add_edges(self, edges):
         """Add multiple edges to the graph
         
         Args:
-            edges (list of DirectedEdge or BidirectedEdge): the edges to add
+            edges (``list`` of ``DirectedEdge`` or ``BidirectedEdge``): the edges to add
         """
         while edges:
             edge = edges.pop()
             if isinstance(edge, BidirectedEdge) or isinstance(edge, DirectedEdge):
                 self.add_edge(edge)
             elif isinstance(edge, list):
                 edges.extend(edge)
             else:
                 raise TypeError(f"Cannot add edge of type {type(edge)}")
     
     def add_edge(self, edge):
         """Adds an edge to the graph
         
         Args:
-            edge (DirectedEdge or BidirectedEdge): the edge to add
+            edge (``DirectedEdge`` or ``BidirectedEdge``): the edge to add
         """
         if isinstance(edge, BidirectedEdge):
             self.bi_edges.append(edge)
             self.add_nodes([edge.a, edge.b])
         elif isinstance(edge, DirectedEdge):
             self.directed_edges.append(edge)
             self.add_nodes([edge.start, edge.end])
@@ -129,20 +129,20 @@
     def _di_edge_tuples(self):
         return [(str(edge.start), str(edge.end)) for edge in self.directed_edges]
     
     def _idc(self, y, x, z=[], step=None):
         """Identification of conditional interventional distribution.
 
         Args:
-            x (list of Variable): intervention variables
-            y (list of Variable): outcome variables
-            z (list of Variable): conditioning variables (optional)
+            x (``list`` of ``Variable``): intervention variables
+            y (``list`` of ``Variable``): outcome variables
+            z (``list`` of ``Variable``): conditioning variables (optional)
         
         Returns:
-            AbstractExpression: the expression for the interventional distribution
+            ``AbstractExpression``: the expression for the interventional distribution
         """
         
         def purify_vars(vs):
             for v in vs:
                 if isinstance(v, Variable):
                     yield v
                 elif isinstance(v, str):
@@ -177,18 +177,18 @@
     def identify(self, estimand, step):
         """Uses IDC to identify an arbitrary estimand
 
         Finds the interventional distributions in a causal estimand and replaces
         them with equivalent conditional probability expressions using IDC.
 
         Args:
-            estimand (Expression): the estimand to identify
+            estimand (``Expression``): the estimand to identify
         
         Returns:
-            AbstractExpression: the identified estimand, containing no do-operators
+            ``AbstractExpression``: the identified estimand, containing no do-operators
         """
         if isinstance(estimand, AbstractCausalEstimand):
             causal_estimand = estimand
             estimand = estimand.expression()
         else:
             causal_estimand = CausalEstimand(exp=estimand)
         
@@ -229,39 +229,39 @@
         ans = estimand.r_map(id)
         step.result("identified_estimand", ans)
     
     def identify_ate(self, outcome, treatment_condition, control_condition):
         """Identifies the average treatment effect
 
         Args:
-            outcome (Variable): the outcome variable
-            treatment_condition (dict): the treatment condition
-            control_condition (dict): the control condition
+            outcome (``Variable``): the outcome variable
+            treatment_condition (``dict``): the treatment condition
+            control_condition (``dict``): the control condition
         
         Returns:
-            AbstractExpression: the identified average treatment effect
+            ``AbstractExpression``: the identified average treatment effect
         """
         return self.identify(ATE(outcome, treatment_condition, control_condition).expression())
     
     def identify_cate(self, outcome, treatment_condition, control_condition, subpopulation):
         """Identifies the conditional average treatment effect
 
         Args:
-            outcome (Variable): the outcome variable
-            treatment_condition (dict): the treatment condition
-            control_condition (dict): the control condition
-            subpopulation (dict): the subpopulation condition
+            outcome (``Variable``): the outcome variable
+            treatment_condition (``dict``): the treatment condition
+            control_condition (``dict``): the control condition
+            subpopulation (``dict``): the subpopulation condition
         
         Returns:
-            AbstractExpression: the identified conditional average treatment effect
+            ``AbstractExpression``: the identified conditional average treatment effect
         """
         return self.identify(CATE(outcome, treatment_condition, control_condition, subpopulation).expression())
     
     def draw(self):
-        """Draws the causal diagram using networkx"""
+        """Draws the causal diagram using networkx (must be installed)."""
         import networkx as nx
 
         layout_graph = nx.Graph()
         layout_graph.add_edges_from(self._bi_edge_tuples() + self._di_edge_tuples())
         layout = nx.spring_layout(layout_graph, scale=1, k=1/len(layout_graph.nodes)**0.5)
         nx.draw_networkx_nodes(layout_graph, layout, node_size=500)
 
@@ -303,32 +303,32 @@
                     else:
                         stack.append(nxt_node)
     
     def dfs(self, start, end):
         """Performs a depth-first search over directed edges in the graph, returning a generator over paths
         
         Args:
-            start (Variable): the start of the search
-            end (Variable): the end of the search
+            start (``Variable``): the start of the search
+            end (``Variable``): the end of the search
         
         Returns:
-            Generator[List[DirectedEdge]]: the path from start to end
+            Generator[``List[DirectedEdge]``]: the path from start to end
         """
         if start not in self.nodes:
             raise ValueError(f"{start} is not in the graph")
         if end not in self.nodes:
             raise ValueError(f"{end} is not in the graph")
         return self._dfs(start, end)
 
 class DirectedEdge:
     """A directed edge between two variables, represents a causal relationship
     
     Args:
-        start (Variable): the start of the edge
-        end (Variable): the end of the edge
+        start (``Variable``): the start of the edge
+        end (``Variable``): the end of the edge
     """
     def __init__(self, start, end):
         self.start = start
         self.end = end
     
     def __repr__(self):
         return f"DirectedEdge(start={self.start}, end={self.end})"
@@ -353,16 +353,16 @@
         else:
             raise TypeError(f"Cannot add edge of type {type(other)}")
 
 class BidirectedEdge:
     """A bidirected edge between two variables, represents confounding in the causal model
     
     Args:
-        a (Variable): one of the variables
-        b (Variable): the other variable
+        a (``Variable``): one of the variables
+        b (``Variable``): the other variable
     """
     def __init__(self, a, b):
         self.a = a
         self.b = b
     
     def __repr__(self):
         return f"BidirectedEdge({self.a}, {self.b})"
```

### Comparing `pqp-0.3.4/python/pqp/refutation/__init__.py` & `pqp-0.3.5/python/pqp/refutation/__init__.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/pqp/refutation/result.py` & `pqp-0.3.5/python/pqp/refutation/result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,96 @@
 from collections import deque
 from pqp.utils import order_graph
 
 class Assumption:
+    """Class representing a modeling assumption
+    
+    Attributes:
+        name (``str``): the name of the assumption
+    """
     def __init__(self, name):
         self.name = name
     
     def __str__(self):
         return f"Assume: {self.name}"
 
 class Derived:
+    """Class representing a derived value or expression
+
+    Attributes:
+        name (``str``): the name of the derived value
+        value (``Any``): the derived value
+    """
     def __init__(self, name, value):
         self.name = name
         self.value = value
     
     def __str__(self):
         return f"Derived: {self.name} = {self.value}"
 
 # human interpretability
 class Step:
-    """Human-interpretable notes on how a result was derived"""
+    """Human-interpretable notes on how a result was derived
+    
+    Subroutes in the library should use this class to record the steps taken to 
+    derive a result. This class is not intended to be used by end-users.
+
+    Args:
+        name (``str``): the name of the step
+    """
     def __init__(self, name):
         self._name = name
         self._log = [] # list of strings, substeps, assumption, expression
         self._assumptions = []
         self._results = {}
     
     def substep(self, name):
+        """Add a substep to the derivation
+
+        Args:
+            name (``str``): the name of the substep
+        Returns:
+            ``Step``: the substep
+        """
         s = Step(name)
         self._log.append(s)
         return s
 
     def write(self, msg):
+        """Add a note about the derivation
+
+        Args:
+            msg (``str``): the message to add
+        Returns:
+            ``None``
+        """
         self._log.append(msg)
     
     def assume(self, assumption):
+        """Add an assumption to the derivation
+
+        Args:
+            assumption (``Assumption`` or ``str``): the assumption to add
+        Returns:
+            ``None``
+        """
         if not isinstance(assumption, Assumption):
             assumption = Assumption(assumption)
         self._assumptions.append(assumption)
         self._log.append(assumption)
     
     def result(self, key, value):
+        """Record the value derived during the step
+
+        Args:
+            key (``str``): the name of the derived value
+            value (``Any``): the derived value
+        Returns:
+            ``None``
+        """
         self._log.append(Derived(key, value))
         self._results[key] = value
     
     def _get_log_strings(self, pad=True):
         acc = []
         for l in self._log:
             if isinstance(l, Step):
@@ -58,17 +105,17 @@
         return self._name + "\n\t" + "\n\t".join(self._get_log_strings(pad=pad))
 
 # computer replicability
 class Operation:
     """Class used to track the computational graph of function calls which led to a result
 
     Attributes:
-        op (function): the function which was called
-        args (list): the arguments passed to the function
-        kwargs (dict): the keyword arguments passed to the function
+        op (``Callable``): the function which was called
+        args (``list``): the arguments passed to the function
+        kwargs (``dict``): the keyword arguments passed to the function
     """
     def __init__(self, op, args, kwargs):
         self.op = op
         self.args = args
         self.kwargs = kwargs
 
 class Result:
@@ -94,24 +141,34 @@
                 stuff[k] = getattr(self, k)
         return f"{self.__class__.__name__}({', '.join(f'{k}={v}' for k, v in stuff.items())})"
 
     def __hash__(self):
         return hash(str(self))
     
     def get_dependencies(self):
+        """Returns a list of all results which this result directly depends on
+        
+        Returns:
+            ``List[Result]``: the list of dependencies
+        """
         dependencies = []
         for args in self.operation.args:
             if isinstance(args, Result):
                 dependencies.append(args)
         for kwargs in self.operation.kwargs.values():
             if isinstance(kwargs, Result):
                 dependencies.append(kwargs)
         return dependencies
     
     def get_nested_dependencies(self):
+        """Returns a list of all results which this result depends on, including indirect dependencies
+
+        Returns:
+            ``List[Result]``: the list of dependencies
+        """
         d = deque([self])
         all_results = {}
         while d:
             r = d.popleft()
             deps = r.get_dependencies()
             all_results[r] = deps
             for dep in deps:
@@ -138,25 +195,25 @@
         Equivalent to calling self.explain(nested=True)"""
         self.explain(nested=True)
 
 def entrypoint(step_name, result_class=Result):
     """Wrapper for logical steps in the assumption management system
 
     Args:
-        step_name (str): the name of the step (human readable)
-        result_class (class): used to store results of the step, must be a subclass of `Result`
+        step_name (``str``): the name of the ``Step`` (human readable)
+        result_class (``class``): used to store results of the ``Step``, must be a subclass of ``Result``
     Returns:
         decorator: wrapper for functions implementing logical steps in an analysis
     
     This function returns a a decorator which can be used to wrap a method implementing a step, a 
-    `Step` instance is passed as a keyword argument ("step") to the method and should 
+    ``Step`` instance is passed as a keyword argument ("step") to the method and should 
     be used to record substeps, assumptions, and results. The method should not return a value.
 
-    The three core constructs of the assumption management system are `Assumption`a, `Step`s, and 
-    `Result`s. A step is a logical unit of work encapsulated in a single method, which may be 
+    The three core constructs of the assumption management system are ``Assumption`` s, ``Step`` s, and 
+    ``Result`` s. A step is a logical unit of work encapsulated in a single method, which may be 
     composed of multiple substeps. During the process of calculation, the method can report 
     logical substeps, assumptions it is making, results as they are computed, and notes for 
     the user. This information is consolidated into the `Step` object, which stores references
     to previous steps in the analysis in a graph representing the entire computation. This way,
     metadata about the computation is available at all times and can be used by both the user and
     automated sensitivity analysis tools.
     """
```

### Comparing `pqp-0.3.4/python/pqp/symbols/event.py` & `pqp-0.3.5/python/pqp/symbols/event.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/pqp/symbols/p.py` & `pqp-0.3.5/python/pqp/symbols/p.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         vars (list of Variable): probability variables
         given (list of Variable): conditioned variables
     
     Raises:
         ValueError: if a variable is repeated in vars or given
         TypeError: if vars or given are not a list of Variable or Event
     """
-    _unassigned = object()
+    unassigned = object()
 
     def __init__(self, vars, given=None):
         if isinstance(vars, Variable) or isinstance(vars, Event):
             vars = [vars]
         elif not isinstance(vars, list):
             vars = list(vars)
         for v in vars:
@@ -48,19 +48,19 @@
                 if v.get_var() in _present:
                     raise ValueError(f"Duplicate variable {v}")
                 _present.add(v.get_var())
         
         self.vars = vars
         self.given = given or []
     
-    @staticproperty
-    @staticmethod
-    def unassigned():
-        """Special object marker for unassigned variables, used in certain routines"""
-        return P._unassigned
+    # @staticproperty
+    # @staticmethod
+    # def unassigned():
+    #     """Special object marker for unassigned variables, used in certain routines"""
+    #     return P._unassigned
     
     def sorted(self):
         return P(
             sorted(self.vars, key=str),
             sorted(self.given, key=str)
             )
```

### Comparing `pqp-0.3.4/python/pqp/symbols/parse.py` & `pqp-0.3.5/python/pqp/symbols/parse.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/pqp/symbols/relation.py` & `pqp-0.3.5/python/pqp/symbols/relation.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/pqp/symbols/variable.py` & `pqp-0.3.5/python/pqp/symbols/variable.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/pqp/utils/exceptions.py` & `pqp-0.3.5/python/pqp/utils/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 
-class InferredDomainWarning(Warning):
+class PQPException(Exception):
+    """Base class for exceptions in this module."""
+    pass
+
+class InferredDomainWarning(PQPException):
     """Warning raised when the domain of a variable is inferred from provided examples"""
     pass
 
-class UnitDomainWarning(Warning):
+class UnitDomainWarning(PQPException):
     """Warning raised when the domain of a variable has cardinality <= 1"""
     pass
 
-class PositivityException(Exception):
+class PositivityException(PQPException):
     """Exception raised when a nonpositive distribution is used"""
     pass
 
-class DomainValidationError(Exception):
+class DomainValidationError(PQPException):
     """Exception raised when domain is used with invalid values"""
     pass
 
-class NumericalError(Exception):
+class NumericalError(PQPException):
     """Exception raised when numerical methods fail"""
     pass
 
+class CyclicGraphError(PQPException):
+    """Exception raised when a graph is cyclic"""
+    pass
+
 # class HedgeError(Exception):
 #     """Indicates that identification has failed"""
 #     pass
```

### Comparing `pqp-0.3.4/python/pqp/utils/utils.py` & `pqp-0.3.5/python/pqp/utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from collections import defaultdict
+from pqp.utils.exceptions import CyclicGraphError
 
 
 def recursive_sort(d):
+    """Recursive sorting of nested dicts, lists, and tuples--useful for semantic comparison"""
     if isinstance(d, dict):
         return {k: recursive_sort(v) for k, v in sorted(d.items())}
     elif isinstance(d, list):
         return list(sorted(recursive_sort(v) for v in d))
     elif isinstance(d, tuple):
         return tuple(sorted(recursive_sort(v) for v in d))
     else:
         return d
 
 class attrdict(dict):
+    """Dictionary subclass which allows access to keys as attributes"""
     def __getattr__(self, key):
         return self[key]
 
 class staticproperty(staticmethod):
     def __get__(self, *_):         
         return self.__func__()
 
@@ -45,8 +48,8 @@
                 ls.append(k)
                 if k in g:
                     for el in g[k]:
                         if el in incoming_counts:
                             incoming_counts[el] -= 1
             if not n:
                 return ls
-    raise Exception("Cycle detected")
+    raise CyclicGraphError
```

### Comparing `pqp-0.3.4/python/scratch.ipynb` & `pqp-0.3.5/python/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_abstract_step.py` & `pqp-0.3.5/python/tests/test_abstract_step.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_causal_estimand.py` & `pqp-0.3.5/python/tests/test_causal_estimand.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_data.py` & `pqp-0.3.5/python/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_domain.py` & `pqp-0.3.5/python/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_examples.py` & `pqp-0.3.5/python/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_graph.py` & `pqp-0.3.5/python/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_id.py` & `pqp-0.3.5/python/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_multinomial_estimator.py` & `pqp-0.3.5/python/tests/test_multinomial_estimator.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_p.py` & `pqp-0.3.5/python/tests/test_p.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,8 +62,12 @@
     x, y, z = make_vars("xyz")
     p = P(x, given=y)
     assert p._intervene(x) == P(x, given=[y]) # this seems unwise, but not sure what else to do
     assert p._intervene(y) == P(x, given=[do(y)])
     p = P(x, given=[y, z])
     assert p._intervene(x) == P(x, given=[y, z])
     assert p._intervene(y) == P(x, given=[do(y), z])
-    assert p.intervene(y)._intervene(z) == P(x, given=[do(y), do(z)])
+    assert p.intervene(y)._intervene(z) == P(x, given=[do(y), do(z)])
+
+
+def test_unassigned():
+    assert P.unassigned
```

### Comparing `pqp-0.3.4/python/tests/test_pqp.py` & `pqp-0.3.5/python/tests/test_pqp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from pqp.graph import Graph
-from pqp.variable import make_vars
-from pqp.utils import recursive_sort
-
-
-def test_create_graph():
-    x, y, z = make_vars("xyz")
-
-    g = Graph([
-        z <= x,
-        y <= z,
-        x & y
-    ])
-    assert recursive_sort(g.bi_edge_tuples()) == recursive_sort([("x", "y")])
-    assert recursive_sort(g.di_edge_tuples()) == recursive_sort([("x", "z"), ("y", "z")])
-
-    g.add_edge(x & z)
-    assert recursive_sort(g.bi_edge_tuples()) == recursive_sort([("x", "y"), ("x", "z")])
-
-def test_id():
-    x, y, z = make_vars("xyz")
-    g = Graph([
-        z <= x,
-        y <= z,
-        x & y
-    ])
-    estimand = g.idc([y], [x])    
-    assert estimand != None
-
-def test_repr_expression():
-    x, y, z = make_vars("xyz")
-    assert str(x / y) == "[x / y]"
-    assert str(x * y) == "x * y"
-    assert (x / y).to_latex() == "{x \over y}"
-    assert (x * y).to_latex() == "x y"
+# from pqp import Graph, make_vars
+# from pqp.utils import recursive_sort
+
+
+# def test_create_graph():
+#     x, y, z = make_vars("xyz")
+
+#     g = Graph([
+#         z <= x,
+#         y <= z,
+#         x & y
+#     ])
+#     assert recursive_sort(g._bi_edge_tuples()) == recursive_sort([("x", "y")])
+#     assert recursive_sort(g._di_edge_tuples()) == recursive_sort([("x", "z"), ("y", "z")])
+
+#     g.add_edge(x & z)
+#     assert recursive_sort(g._bi_edge_tuples()) == recursive_sort([("x", "y"), ("x", "z")])
+
+# def test_id():
+#     x, y, z = make_vars("xyz")
+#     g = Graph([
+#         z <= x,
+#         y <= z,
+#         x & y
+#     ])
+#     estimand = g._idc([y], [x])    
+#     assert estimand != None
+
+# def test_repr_expression():
+#     x, y, z = make_vars("xyz")
+#     assert str(x / y) == "[x / y]"
+#     assert str(x * y) == "x * y"
+#     assert (x / y).to_latex() == "{x \over y}"
+#     assert (x * y).to_latex() == "x y"
```

### Comparing `pqp-0.3.4/python/tests/test_refutation.py` & `pqp-0.3.5/python/tests/test_refutation.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_relation.py` & `pqp-0.3.5/python/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/python/tests/test_variable.py` & `pqp-0.3.5/python/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/api/functions.rs` & `pqp-0.3.5/src/api/functions.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/api/python.rs` & `pqp-0.3.5/src/api/python.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/api/test.rs` & `pqp-0.3.5/src/api/test.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/api/wrapper.rs` & `pqp-0.3.5/src/api/wrapper.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/form/form.rs` & `pqp-0.3.5/src/form/form.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/form/simplify.rs` & `pqp-0.3.5/src/form/simplify.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/form/test_form.rs` & `pqp-0.3.5/src/form/test_form.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/form/test_simplify.rs` & `pqp-0.3.5/src/form/test_simplify.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/form/tikka.rs` & `pqp-0.3.5/src/form/tikka.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/graph/bigraph.rs` & `pqp-0.3.5/src/graph/bigraph.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/graph/digraph.rs` & `pqp-0.3.5/src/graph/digraph.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/graph/graph_builder.rs` & `pqp-0.3.5/src/graph/graph_builder.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/graph/tests.rs` & `pqp-0.3.5/src/graph/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/identification/shpitser.rs` & `pqp-0.3.5/src/identification/shpitser.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/identification/tests.rs` & `pqp-0.3.5/src/identification/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/model/model.rs` & `pqp-0.3.5/src/model/model.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/model/order.rs` & `pqp-0.3.5/src/model/order.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/model/tests.rs` & `pqp-0.3.5/src/model/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/test.rs` & `pqp-0.3.5/src/test.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/utils/set_utils.rs` & `pqp-0.3.5/src/utils/set_utils.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/utils/tests.rs` & `pqp-0.3.5/src/utils/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/src/utils/utils.rs` & `pqp-0.3.5/src/utils/utils.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-01-14-13-06-10.png` & `pqp-0.3.5/writeup/2023-01-14-13-06-10.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-01-14-13-52-24.png` & `pqp-0.3.5/writeup/2023-01-14-13-52-24.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-01-14-14-22-06.png` & `pqp-0.3.5/writeup/2023-01-14-14-22-06.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-01-14-15-01-52.png` & `pqp-0.3.5/writeup/2023-01-14-15-01-52.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-02-25-09-07-36.png` & `pqp-0.3.5/writeup/2023-02-25-09-07-36.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-02-25-09-22-50.png` & `pqp-0.3.5/writeup/2023-02-25-09-22-50.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-33-14.png` & `pqp-0.3.5/writeup/2023-04-02-14-33-14.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-33-44.png` & `pqp-0.3.5/writeup/2023-04-02-14-33-44.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-34-19.png` & `pqp-0.3.5/writeup/2023-04-02-14-34-19.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-34-30.png` & `pqp-0.3.5/writeup/2023-04-02-14-34-30.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-34-44.png` & `pqp-0.3.5/writeup/2023-04-02-14-34-44.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-35-39.png` & `pqp-0.3.5/writeup/2023-04-02-14-35-39.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-36-00.png` & `pqp-0.3.5/writeup/2023-04-02-14-36-00.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-36-57.png` & `pqp-0.3.5/writeup/2023-04-02-14-36-57.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/2023-04-02-14-37-10.png` & `pqp-0.3.5/writeup/2023-04-02-14-37-10.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/PQP a Library for End-to-End Causal Inference.ipynb` & `pqp-0.3.5/writeup/PQP a Library for End-to-End Causal Inference.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/PQP.ipynb` & `pqp-0.3.5/writeup/PQP.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/Performant Conditional Query Identification in Structural Causal Models.ipynb` & `pqp-0.3.5/writeup/Performant Conditional Query Identification in Structural Causal Models.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/agg.ipynb` & `pqp-0.3.5/writeup/agg.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/build.py` & `pqp-0.3.5/writeup/build.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/demo.ipynb` & `pqp-0.3.5/writeup/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/demo1.csv` & `pqp-0.3.5/writeup/demo1.csv`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/doctordemo.csv` & `pqp-0.3.5/writeup/doctordemo.csv`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/examples.ipynb` & `pqp-0.3.5/writeup/examples.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/grab_code.py` & `pqp-0.3.5/writeup/grab_code.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/scratch.ipynb` & `pqp-0.3.5/writeup/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/speed.ipynb` & `pqp-0.3.5/writeup/speed.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/writeup/supplement.py` & `pqp-0.3.5/writeup/supplement.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/Cargo.lock` & `pqp-0.3.5/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pqp-0.3.4/PKG-INFO` & `pqp-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pqp
-Version: 0.3.4
+Version: 0.3.5
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: tomli
-Requires-Dist: matplotlib
 Requires-Dist: sphinx; extra == 'dev'
 Requires-Dist: maturin; extra == 'dev'
 Requires-Dist: sphinx-autobuild; extra == 'dev'
+Requires-Dist: sphinx_automodapi; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: networkx; extra == 'dev'
+Requires-Dist: matplotlib; extra == 'dataviz'
+Requires-Dist: networkx; extra == 'dataviz'
 Provides-Extra: dev
+Provides-Extra: dataviz
 License-File: LICENSE.txt
 Summary: Subroutines for structural causal modeling
 Keywords: causal inference,causal identification
 Author: Leo Ware
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source, https://github.com/leo-ware/capstone
```

