# Comparing `tmp/prometheus_fastapi_instrumentator-6.0.0.tar.gz` & `tmp/prometheus_fastapi_instrumentator-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_fastapi_instrumentator-6.0.0.tar", max compression
+gzip compressed data, was "prometheus_fastapi_instrumentator-6.1.0.tar", max compression
```

## Comparing `prometheus_fastapi_instrumentator-6.0.0.tar` & `prometheus_fastapi_instrumentator-6.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      762 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/LICENSE
--rw-r--r--   0        0        0    12631 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/README.md
--rw-r--r--   0        0        0     1290 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/pyproject.toml
--rw-r--r--   0        0        0      134 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/__init__.py
--rw-r--r--   0        0        0    12605 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/instrumentation.py
--rw-r--r--   0        0        0    26494 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/metrics.py
--rw-r--r--   0        0        0     8658 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/middleware.py
--rw-r--r--   0        0        0        0 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/py.typed
--rw-r--r--   0        0        0     4014 2023-03-20 19:58:09.312835 prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/routing.py
--rw-r--r--   0        0        0    13802 1970-01-01 00:00:00.000000 prometheus_fastapi_instrumentator-6.0.0/setup.py
--rw-r--r--   0        0        0    13554 1970-01-01 00:00:00.000000 prometheus_fastapi_instrumentator-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0      762 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/LICENSE
+-rw-r--r--   0        0        0    12774 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/README.md
+-rw-r--r--   0        0        0     1304 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/__init__.py
+-rw-r--r--   0        0        0    12605 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/instrumentation.py
+-rw-r--r--   0        0        0    26608 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/metrics.py
+-rw-r--r--   0        0        0     8658 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/py.typed
+-rw-r--r--   0        0        0     4014 2023-07-15 09:40:03.961577 prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/routing.py
+-rw-r--r--   0        0        0    13950 1970-01-01 00:00:00.000000 prometheus_fastapi_instrumentator-6.1.0/setup.py
+-rw-r--r--   0        0        0    13697 1970-01-01 00:00:00.000000 prometheus_fastapi_instrumentator-6.1.0/PKG-INFO
```

### Comparing `prometheus_fastapi_instrumentator-6.0.0/LICENSE` & `prometheus_fastapi_instrumentator-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_fastapi_instrumentator-6.0.0/README.md` & `prometheus_fastapi_instrumentator-6.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
 - Counter `http_requests_total` with `handler`, `status` and `method`. Total
   number of requests.
 - Summary `http_request_size_bytes` with `handler`. Added up total of the
   content lengths of all incoming requests.
 - Summary `http_response_size_bytes` with `handler`. Added up total of the
   content lengths of all outgoing responses.
-- Histogram `http_request_duration_seconds` with `handler`. Only a few buckets
-  to keep cardinality low.
+- Histogram `http_request_duration_seconds` with `handler` and `method`. Only a
+  few buckets to keep cardinality low.
 - Histogram `http_request_duration_highr_seconds` without any labels. Large
   number of buckets (>20).
 
 In addition, following behavior is active:
 
 - Status codes are grouped into `2xx`, `3xx` and so on.
 - Requests without a matching template are grouped into the handler `none`.
@@ -58,35 +58,40 @@
   [`metrics`](./src/prometheus_fastapi_instrumentator/metrics.py) and pass it to
   the instrumentator instance. See [here](#adding-metrics) how to do that.
 - Create your own instrumentation function that you can pass to an
   instrumentator instance. See [here](#creating-new-metrics) to learn how more.
 - Don't use this package at all and just use the source code as inspiration on
   how to instrument your FastAPI.
 
-Important: This package is not made for generic Prometheus instrumentation in
-Python. Use the Prometheus client library for that. This packages uses it as
-well.
-
 ## Table of Contents <!-- omit in toc -->
 
 <!--TOC-->
 
+- [Disclaimer](#disclaimer)
 - [Features](#features)
 - [Advanced Usage](#advanced-usage)
   - [Creating the Instrumentator](#creating-the-instrumentator)
   - [Adding metrics](#adding-metrics)
   - [Creating new metrics](#creating-new-metrics)
   - [Perform instrumentation](#perform-instrumentation)
   - [Specify namespace and subsystem](#specify-namespace-and-subsystem)
   - [Exposing endpoint](#exposing-endpoint)
 - [Contributing](#contributing)
 - [Licensing](#licensing)
 
 <!--TOC-->
 
+## Disclaimer
+
+Not made for generic Prometheus instrumentation in Python. Use the Prometheus
+client library for that. This packages uses it as well.
+
+All the generic middleware and instrumentation code comes with a cost in
+performance that can become noticeable.
+
 ## Features
 
 Beyond the fast track, this instrumentator is **highly configurable** and it is
 very easy to customize and adapt to your specific use case. Here is a list of
 some of these options you may opt-in to:
 
 - Regex patterns to ignore certain routes.
```

### Comparing `prometheus_fastapi_instrumentator-6.0.0/pyproject.toml` & `prometheus_fastapi_instrumentator-6.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "prometheus-fastapi-instrumentator"
-version = "6.0.0"
+version = "6.1.0"
 description = "Instrument your FastAPI with Prometheus metrics."
 authors = ["Tim Schwenke <tim@trallnag.com>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/trallnag/prometheus-fastapi-instrumentator"
 keywords = ["prometheus", "instrumentation", "fastapi", "exporter", "metrics"]
 
@@ -25,17 +25,17 @@
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 rope = "^1.7.0"
 isort = "^5.11.3"
 mypy = "^1.1.1"
 devtools = "^0.10.0"
 asgiref = "^3.6.0"
-uvicorn = "^0.20.0"
+uvicorn = ">=0.20,<0.23"
 gunicorn = "^20.1.0"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = ">=0.20.3,<0.22.0"
 
 [tool.black]
 line-length = 90
 
 [tool.isort]
 profile = "black"
```

### Comparing `prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/instrumentation.py` & `prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/instrumentation.py`

 * *Files identical despite different names*

### Comparing `prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/metrics.py` & `prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,15 +705,18 @@
         LATENCY_LOWR = Histogram(
             name="http_request_duration_seconds",
             documentation=(
                 "Latency with only few buckets by handler. "
                 "Made to be only used if aggregation by handler is important. "
             ),
             buckets=latency_lowr_buckets,
-            labelnames=("handler",),
+            labelnames=(
+                "method",
+                "handler",
+            ),
             namespace=metric_namespace,
             subsystem=metric_subsystem,
             registry=registry,
         )
 
         def instrumentation(info: Info) -> None:
             TOTAL.labels(info.method, info.modified_status, info.modified_handler).inc()
@@ -730,15 +733,17 @@
                 OUT_SIZE.labels(info.modified_handler).observe(0)
 
             if not should_only_respect_2xx_for_highr or info.modified_status.startswith(
                 "2"
             ):
                 LATENCY_HIGHR.observe(info.modified_duration)
 
-            LATENCY_LOWR.labels(info.modified_handler).observe(info.modified_duration)
+            LATENCY_LOWR.labels(
+                handler=info.modified_handler, method=info.method
+            ).observe(info.modified_duration)
 
         return instrumentation
 
     except ValueError as e:
         if not _is_duplicated_time_series(e):
             raise e
```

### Comparing `prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/middleware.py` & `prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/middleware.py`

 * *Files identical despite different names*

### Comparing `prometheus_fastapi_instrumentator-6.0.0/src/prometheus_fastapi_instrumentator/routing.py` & `prometheus_fastapi_instrumentator-6.1.0/src/prometheus_fastapi_instrumentator/routing.py`

 * *Files identical despite different names*

### Comparing `prometheus_fastapi_instrumentator-6.0.0/setup.py` & `prometheus_fastapi_instrumentator-6.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['fastapi>=0.38.1,<1.0.0', 'prometheus-client>=0.8.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'prometheus-fastapi-instrumentator',
-    'version': '6.0.0',
+    'version': '6.1.0',
     'description': 'Instrument your FastAPI with Prometheus metrics.',
-    'long_description': '# Prometheus FastAPI Instrumentator <!-- omit in toc -->\n\n[![pypi-version](https://badge.fury.io/py/prometheus-fastapi-instrumentator.svg)](https://pypi.python.org/pypi/prometheus-fastapi-instrumentator)\n[![python-versions](https://img.shields.io/pypi/pyversions/prometheus-fastapi-instrumentator.svg)](https://pypi.python.org/pypi/prometheus-fastapi-instrumentator)\n[![downloads](https://pepy.tech/badge/prometheus-fastapi-instrumentator/month)](https://pepy.tech/project/prometheus-fastapi-instrumentator/month)\n[![build](https://img.shields.io/github/actions/workflow/status/trallnag/kubestatus2cloudwatch/ci.yaml?branch=master)](https://github.com/trallnag/kubestatus2cloudwatch/actions)\n[![codecov](https://codecov.io/gh/trallnag/prometheus-fastapi-instrumentator/branch/master/graph/badge.svg)](https://codecov.io/gh/trallnag/prometheus-fastapi-instrumentator)\n\nA configurable and modular Prometheus Instrumentator for your FastAPI. Install\n`prometheus-fastapi-instrumentator` from\n[PyPI](https://pypi.python.org/pypi/prometheus-fastapi-instrumentator/). Here is\nthe fast track to get started with a pre-configured instrumentator. Import the\ninstrumentator class:\n\n```python\nfrom prometheus_fastapi_instrumentator import Instrumentator\n```\n\nInstrument your app with default metrics and expose the metrics:\n\n```python\nInstrumentator().instrument(app).expose(app)\n```\n\nDepending on your code you might have to use the following instead:\n\n```python\ninstrumentator = Instrumentator().instrument(app)\n\n@app.on_event("startup")\nasync def _startup():\n    instrumentator.expose(app)\n```\n\nWith this, your FastAPI is instrumented and metrics are ready to be scraped. The\ndefaults give you:\n\n- Counter `http_requests_total` with `handler`, `status` and `method`. Total\n  number of requests.\n- Summary `http_request_size_bytes` with `handler`. Added up total of the\n  content lengths of all incoming requests.\n- Summary `http_response_size_bytes` with `handler`. Added up total of the\n  content lengths of all outgoing responses.\n- Histogram `http_request_duration_seconds` with `handler`. Only a few buckets\n  to keep cardinality low.\n- Histogram `http_request_duration_highr_seconds` without any labels. Large\n  number of buckets (>20).\n\nIn addition, following behavior is active:\n\n- Status codes are grouped into `2xx`, `3xx` and so on.\n- Requests without a matching template are grouped into the handler `none`.\n\nIf one of these presets does not suit your needs you can do one of multiple\nthings:\n\n- Pick one of the already existing closures from\n  [`metrics`](./src/prometheus_fastapi_instrumentator/metrics.py) and pass it to\n  the instrumentator instance. See [here](#adding-metrics) how to do that.\n- Create your own instrumentation function that you can pass to an\n  instrumentator instance. See [here](#creating-new-metrics) to learn how more.\n- Don\'t use this package at all and just use the source code as inspiration on\n  how to instrument your FastAPI.\n\nImportant: This package is not made for generic Prometheus instrumentation in\nPython. Use the Prometheus client library for that. This packages uses it as\nwell.\n\n## Table of Contents <!-- omit in toc -->\n\n<!--TOC-->\n\n- [Features](#features)\n- [Advanced Usage](#advanced-usage)\n  - [Creating the Instrumentator](#creating-the-instrumentator)\n  - [Adding metrics](#adding-metrics)\n  - [Creating new metrics](#creating-new-metrics)\n  - [Perform instrumentation](#perform-instrumentation)\n  - [Specify namespace and subsystem](#specify-namespace-and-subsystem)\n  - [Exposing endpoint](#exposing-endpoint)\n- [Contributing](#contributing)\n- [Licensing](#licensing)\n\n<!--TOC-->\n\n## Features\n\nBeyond the fast track, this instrumentator is **highly configurable** and it is\nvery easy to customize and adapt to your specific use case. Here is a list of\nsome of these options you may opt-in to:\n\n- Regex patterns to ignore certain routes.\n- Completely ignore untemplated routes.\n- Control instrumentation and exposition with an env var.\n- Rounding of latencies to a certain decimal number.\n- Renaming of labels and the metric.\n- Metrics endpoint can compress data with gzip.\n- Opt-in metric to monitor the number of requests in progress.\n\nIt also features a **modular approach to metrics** that should instrument all\nFastAPI endpoints. You can either choose from a set of already existing metrics\nor create your own. And every metric function by itself can be configured as\nwell. You can see ready to use metrics\n[here](https://trallnag.github.io/prometheus-fastapi-instrumentator/metrics.html).\n\n## Advanced Usage\n\nThis chapter contains an example on the advanced usage of the Prometheus FastAPI\nInstrumentator to showcase most of it\'s features. Fore more concrete info check\nout the\n[automatically generated documentation](https://trallnag.github.io/prometheus-fastapi-instrumentator/).\n\n### Creating the Instrumentator\n\nWe start by creating an instance of the Instrumentator. Notice the additional\n`metrics` import. This will come in handy later.\n\n```python\nfrom prometheus_fastapi_instrumentator import Instrumentator, metrics\n\ninstrumentator = Instrumentator(\n    should_group_status_codes=False,\n    should_ignore_untemplated=True,\n    should_respect_env_var=True,\n    should_instrument_requests_inprogress=True,\n    excluded_handlers=[".*admin.*", "/metrics"],\n    env_var_name="ENABLE_METRICS",\n    inprogress_name="inprogress",\n    inprogress_labels=True,\n)\n```\n\nUnlike in the fast track example, now the instrumentation and exposition will\nonly take place if the environment variable `ENABLE_METRICS` is `true` at\nrun-time. This can be helpful in larger deployments with multiple services\ndepending on the same base FastAPI.\n\n### Adding metrics\n\nLet\'s say we also want to instrument the size of requests and responses. For\nthis we use the `add()` method. This method does nothing more than taking a\nfunction and adding it to a list. Then during run-time every time FastAPI\nhandles a request all functions in this list will be called while giving them a\nsingle argument that stores useful information like the request and response\nobjects. If no `add()` at all is used, the default metric gets added in the\nbackground. This is what happens in the fast track example.\n\nAll instrumentation functions are stored as closures in the `metrics` module.\nFore more concrete info check out the\n[automatically generated documentation](https://trallnag.github.io/prometheus-fastapi-instrumentator/).\n\nClosures come in handy here because it allows us to configure the functions\nwithin.\n\n```python\ninstrumentator.add(metrics.latency(buckets=(1, 2, 3,)))\n```\n\nThis simply adds the metric you also get in the fast track example with a\nmodified buckets argument. But we would also like to record the size of all\nrequests and responses.\n\n```python\ninstrumentator.add(\n    metrics.request_size(\n        should_include_handler=True,\n        should_include_method=False,\n        should_include_status=True,\n        metric_namespace="a",\n        metric_subsystem="b",\n    )\n).add(\n    metrics.response_size(\n        should_include_handler=True,\n        should_include_method=False,\n        should_include_status=True,\n        metric_namespace="namespace",\n        metric_subsystem="subsystem",\n    )\n)\n```\n\nYou can add as many metrics you like to the instrumentator.\n\n### Creating new metrics\n\nAs already mentioned, it is possible to create custom functions to pass on to\n`add()`. This is also how the default metrics are implemented. The documentation\nand code\n[here](https://trallnag.github.io/prometheus-fastapi-instrumentator/metrics.html)\nis helpful to get an overview.\n\nThe basic idea is that the instrumentator creates an `info` object that contains\neverything necessary for instrumentation based on the configuration of the\ninstrumentator. This includes the raw request and response objects but also the\nmodified handler, grouped status code and duration. Next, all registered\ninstrumentation functions are called. They get `info` as their single argument.\n\nLet\'s say we want to count the number of times a certain language has been\nrequested.\n\n```python\nfrom typing import Callable\nfrom prometheus_fastapi_instrumentator.metrics import Info\nfrom prometheus_client import Counter\n\ndef http_requested_languages_total() -> Callable[[Info], None]:\n    METRIC = Counter(\n        "http_requested_languages_total",\n        "Number of times a certain language has been requested.",\n        labelnames=("langs",)\n    )\n\n    def instrumentation(info: Info) -> None:\n        langs = set()\n        lang_str = info.request.headers["Accept-Language"]\n        for element in lang_str.split(","):\n            element = element.split(";")[0].strip().lower()\n            langs.add(element)\n        for language in langs:\n            METRIC.labels(language).inc()\n\n    return instrumentation\n```\n\nThe function `http_requested_languages_total` is used for persistent elements\nthat are stored between all instrumentation executions (for example the metric\ninstance itself). Next comes the closure. This function must adhere to the shown\ninterface. It will always get an `Info` object that contains the request,\nresponse and a few other modified informations. For example the (grouped) status\ncode or the handler. Finally, the closure is returned.\n\n**Important:** The response object inside `info` can either be the response\nobject or `None`. In addition, errors thrown in the handler are not caught by\nthe instrumentator. I recommend to check the documentation and/or the source\ncode before creating your own metrics.\n\nTo use it, we hand over the closure to the instrumentator object.\n\n```python\ninstrumentator.add(http_requested_languages_total())\n```\n\n### Perform instrumentation\n\nUp to this point, the FastAPI has not been touched at all. Everything has been\nstored in the `instrumentator` only. To actually register the instrumentation\nwith FastAPI, the `instrument()` method has to be called.\n\n```python\ninstrumentator.instrument(app)\n```\n\nNotice that this will do nothing if `should_respect_env_var` has been set during\nconstruction of the instrumentator object and the respective env var is not\nfound.\n\n### Specify namespace and subsystem\n\nYou can specify the namespace and subsystem of the metrics by passing them in\nthe instrument method.\n\n```python\nfrom prometheus_fastapi_instrumentator import Instrumentator\n\n@app.on_event("startup")\nasync def startup():\n    Instrumentator().instrument(app, metric_namespace=\'myproject\', metric_subsystem=\'myservice\').expose(app)\n```\n\nThen your metrics will contain the namespace and subsystem in the metric name.\n\n```sh\n# TYPE myproject_myservice_http_request_duration_highr_seconds histogram\nmyproject_myservice_http_request_duration_highr_seconds_bucket{le="0.01"} 0.0\n```\n\n### Exposing endpoint\n\nTo expose an endpoint for the metrics either follow\n[Prometheus Python Client](https://github.com/prometheus/client_python) and add\nthe endpoint manually to the FastAPI or serve it on a separate server. You can\nalso use the included `expose` method. It will add an endpoint to the given\nFastAPI. With `should_gzip` you can instruct the endpoint to compress the data\nas long as the client accepts gzip encoding. Prometheus for example does by\ndefault. Beware that network bandwith is often cheaper than CPU cycles.\n\n```python\ninstrumentator.expose(app, include_in_schema=False, should_gzip=True)\n```\n\nNotice that this will to nothing if `should_respect_env_var` has been set during\nconstruction of the instrumentator object and the respective env var is not\nfound.\n\n## Contributing\n\nPlease refer to [`CONTRIBUTING.md`](CONTRIBUTING).\n\nConsult [`DEVELOPMENT.md`](DEVELOPMENT.md) for guidance regarding development.\n\nRead [`RELEASE.md`](RELEASE.md) for details about the release process.\n\n## Licensing\n\nThe default license for this project is the\n[ISC License](https://choosealicense.com/licenses/isc). A permissive license\nfunctionally equivalent to the BSD 2-Clause and MIT licenses, removing some\nlanguage that is no longer necessary. See [`LICENSE`](LICENSE) for the license\ntext.\n\nThe [BSD 3-Clause License](https://choosealicense.com/licenses/bsd-3-clause) is\nused as the license for the\n[`routing`](src/prometheus_fastapi_instrumentator/routing.py) module. This is\ndue to it containing code from\n[elastic/apm-agent-python](https://github.com/elastic/apm-agent-python). BSD\n3-Clause is a permissive license similar to the BSD 2-Clause License, but with a\n3rd clause that prohibits others from using the name of the copyright holder or\nits contributors to promote derived products without written consent. The\nlicense text is included in the module itself.\n',
+    'long_description': '# Prometheus FastAPI Instrumentator <!-- omit in toc -->\n\n[![pypi-version](https://badge.fury.io/py/prometheus-fastapi-instrumentator.svg)](https://pypi.python.org/pypi/prometheus-fastapi-instrumentator)\n[![python-versions](https://img.shields.io/pypi/pyversions/prometheus-fastapi-instrumentator.svg)](https://pypi.python.org/pypi/prometheus-fastapi-instrumentator)\n[![downloads](https://pepy.tech/badge/prometheus-fastapi-instrumentator/month)](https://pepy.tech/project/prometheus-fastapi-instrumentator/month)\n[![build](https://img.shields.io/github/actions/workflow/status/trallnag/kubestatus2cloudwatch/ci.yaml?branch=master)](https://github.com/trallnag/kubestatus2cloudwatch/actions)\n[![codecov](https://codecov.io/gh/trallnag/prometheus-fastapi-instrumentator/branch/master/graph/badge.svg)](https://codecov.io/gh/trallnag/prometheus-fastapi-instrumentator)\n\nA configurable and modular Prometheus Instrumentator for your FastAPI. Install\n`prometheus-fastapi-instrumentator` from\n[PyPI](https://pypi.python.org/pypi/prometheus-fastapi-instrumentator/). Here is\nthe fast track to get started with a pre-configured instrumentator. Import the\ninstrumentator class:\n\n```python\nfrom prometheus_fastapi_instrumentator import Instrumentator\n```\n\nInstrument your app with default metrics and expose the metrics:\n\n```python\nInstrumentator().instrument(app).expose(app)\n```\n\nDepending on your code you might have to use the following instead:\n\n```python\ninstrumentator = Instrumentator().instrument(app)\n\n@app.on_event("startup")\nasync def _startup():\n    instrumentator.expose(app)\n```\n\nWith this, your FastAPI is instrumented and metrics are ready to be scraped. The\ndefaults give you:\n\n- Counter `http_requests_total` with `handler`, `status` and `method`. Total\n  number of requests.\n- Summary `http_request_size_bytes` with `handler`. Added up total of the\n  content lengths of all incoming requests.\n- Summary `http_response_size_bytes` with `handler`. Added up total of the\n  content lengths of all outgoing responses.\n- Histogram `http_request_duration_seconds` with `handler` and `method`. Only a\n  few buckets to keep cardinality low.\n- Histogram `http_request_duration_highr_seconds` without any labels. Large\n  number of buckets (>20).\n\nIn addition, following behavior is active:\n\n- Status codes are grouped into `2xx`, `3xx` and so on.\n- Requests without a matching template are grouped into the handler `none`.\n\nIf one of these presets does not suit your needs you can do one of multiple\nthings:\n\n- Pick one of the already existing closures from\n  [`metrics`](./src/prometheus_fastapi_instrumentator/metrics.py) and pass it to\n  the instrumentator instance. See [here](#adding-metrics) how to do that.\n- Create your own instrumentation function that you can pass to an\n  instrumentator instance. See [here](#creating-new-metrics) to learn how more.\n- Don\'t use this package at all and just use the source code as inspiration on\n  how to instrument your FastAPI.\n\n## Table of Contents <!-- omit in toc -->\n\n<!--TOC-->\n\n- [Disclaimer](#disclaimer)\n- [Features](#features)\n- [Advanced Usage](#advanced-usage)\n  - [Creating the Instrumentator](#creating-the-instrumentator)\n  - [Adding metrics](#adding-metrics)\n  - [Creating new metrics](#creating-new-metrics)\n  - [Perform instrumentation](#perform-instrumentation)\n  - [Specify namespace and subsystem](#specify-namespace-and-subsystem)\n  - [Exposing endpoint](#exposing-endpoint)\n- [Contributing](#contributing)\n- [Licensing](#licensing)\n\n<!--TOC-->\n\n## Disclaimer\n\nNot made for generic Prometheus instrumentation in Python. Use the Prometheus\nclient library for that. This packages uses it as well.\n\nAll the generic middleware and instrumentation code comes with a cost in\nperformance that can become noticeable.\n\n## Features\n\nBeyond the fast track, this instrumentator is **highly configurable** and it is\nvery easy to customize and adapt to your specific use case. Here is a list of\nsome of these options you may opt-in to:\n\n- Regex patterns to ignore certain routes.\n- Completely ignore untemplated routes.\n- Control instrumentation and exposition with an env var.\n- Rounding of latencies to a certain decimal number.\n- Renaming of labels and the metric.\n- Metrics endpoint can compress data with gzip.\n- Opt-in metric to monitor the number of requests in progress.\n\nIt also features a **modular approach to metrics** that should instrument all\nFastAPI endpoints. You can either choose from a set of already existing metrics\nor create your own. And every metric function by itself can be configured as\nwell. You can see ready to use metrics\n[here](https://trallnag.github.io/prometheus-fastapi-instrumentator/metrics.html).\n\n## Advanced Usage\n\nThis chapter contains an example on the advanced usage of the Prometheus FastAPI\nInstrumentator to showcase most of it\'s features. Fore more concrete info check\nout the\n[automatically generated documentation](https://trallnag.github.io/prometheus-fastapi-instrumentator/).\n\n### Creating the Instrumentator\n\nWe start by creating an instance of the Instrumentator. Notice the additional\n`metrics` import. This will come in handy later.\n\n```python\nfrom prometheus_fastapi_instrumentator import Instrumentator, metrics\n\ninstrumentator = Instrumentator(\n    should_group_status_codes=False,\n    should_ignore_untemplated=True,\n    should_respect_env_var=True,\n    should_instrument_requests_inprogress=True,\n    excluded_handlers=[".*admin.*", "/metrics"],\n    env_var_name="ENABLE_METRICS",\n    inprogress_name="inprogress",\n    inprogress_labels=True,\n)\n```\n\nUnlike in the fast track example, now the instrumentation and exposition will\nonly take place if the environment variable `ENABLE_METRICS` is `true` at\nrun-time. This can be helpful in larger deployments with multiple services\ndepending on the same base FastAPI.\n\n### Adding metrics\n\nLet\'s say we also want to instrument the size of requests and responses. For\nthis we use the `add()` method. This method does nothing more than taking a\nfunction and adding it to a list. Then during run-time every time FastAPI\nhandles a request all functions in this list will be called while giving them a\nsingle argument that stores useful information like the request and response\nobjects. If no `add()` at all is used, the default metric gets added in the\nbackground. This is what happens in the fast track example.\n\nAll instrumentation functions are stored as closures in the `metrics` module.\nFore more concrete info check out the\n[automatically generated documentation](https://trallnag.github.io/prometheus-fastapi-instrumentator/).\n\nClosures come in handy here because it allows us to configure the functions\nwithin.\n\n```python\ninstrumentator.add(metrics.latency(buckets=(1, 2, 3,)))\n```\n\nThis simply adds the metric you also get in the fast track example with a\nmodified buckets argument. But we would also like to record the size of all\nrequests and responses.\n\n```python\ninstrumentator.add(\n    metrics.request_size(\n        should_include_handler=True,\n        should_include_method=False,\n        should_include_status=True,\n        metric_namespace="a",\n        metric_subsystem="b",\n    )\n).add(\n    metrics.response_size(\n        should_include_handler=True,\n        should_include_method=False,\n        should_include_status=True,\n        metric_namespace="namespace",\n        metric_subsystem="subsystem",\n    )\n)\n```\n\nYou can add as many metrics you like to the instrumentator.\n\n### Creating new metrics\n\nAs already mentioned, it is possible to create custom functions to pass on to\n`add()`. This is also how the default metrics are implemented. The documentation\nand code\n[here](https://trallnag.github.io/prometheus-fastapi-instrumentator/metrics.html)\nis helpful to get an overview.\n\nThe basic idea is that the instrumentator creates an `info` object that contains\neverything necessary for instrumentation based on the configuration of the\ninstrumentator. This includes the raw request and response objects but also the\nmodified handler, grouped status code and duration. Next, all registered\ninstrumentation functions are called. They get `info` as their single argument.\n\nLet\'s say we want to count the number of times a certain language has been\nrequested.\n\n```python\nfrom typing import Callable\nfrom prometheus_fastapi_instrumentator.metrics import Info\nfrom prometheus_client import Counter\n\ndef http_requested_languages_total() -> Callable[[Info], None]:\n    METRIC = Counter(\n        "http_requested_languages_total",\n        "Number of times a certain language has been requested.",\n        labelnames=("langs",)\n    )\n\n    def instrumentation(info: Info) -> None:\n        langs = set()\n        lang_str = info.request.headers["Accept-Language"]\n        for element in lang_str.split(","):\n            element = element.split(";")[0].strip().lower()\n            langs.add(element)\n        for language in langs:\n            METRIC.labels(language).inc()\n\n    return instrumentation\n```\n\nThe function `http_requested_languages_total` is used for persistent elements\nthat are stored between all instrumentation executions (for example the metric\ninstance itself). Next comes the closure. This function must adhere to the shown\ninterface. It will always get an `Info` object that contains the request,\nresponse and a few other modified informations. For example the (grouped) status\ncode or the handler. Finally, the closure is returned.\n\n**Important:** The response object inside `info` can either be the response\nobject or `None`. In addition, errors thrown in the handler are not caught by\nthe instrumentator. I recommend to check the documentation and/or the source\ncode before creating your own metrics.\n\nTo use it, we hand over the closure to the instrumentator object.\n\n```python\ninstrumentator.add(http_requested_languages_total())\n```\n\n### Perform instrumentation\n\nUp to this point, the FastAPI has not been touched at all. Everything has been\nstored in the `instrumentator` only. To actually register the instrumentation\nwith FastAPI, the `instrument()` method has to be called.\n\n```python\ninstrumentator.instrument(app)\n```\n\nNotice that this will do nothing if `should_respect_env_var` has been set during\nconstruction of the instrumentator object and the respective env var is not\nfound.\n\n### Specify namespace and subsystem\n\nYou can specify the namespace and subsystem of the metrics by passing them in\nthe instrument method.\n\n```python\nfrom prometheus_fastapi_instrumentator import Instrumentator\n\n@app.on_event("startup")\nasync def startup():\n    Instrumentator().instrument(app, metric_namespace=\'myproject\', metric_subsystem=\'myservice\').expose(app)\n```\n\nThen your metrics will contain the namespace and subsystem in the metric name.\n\n```sh\n# TYPE myproject_myservice_http_request_duration_highr_seconds histogram\nmyproject_myservice_http_request_duration_highr_seconds_bucket{le="0.01"} 0.0\n```\n\n### Exposing endpoint\n\nTo expose an endpoint for the metrics either follow\n[Prometheus Python Client](https://github.com/prometheus/client_python) and add\nthe endpoint manually to the FastAPI or serve it on a separate server. You can\nalso use the included `expose` method. It will add an endpoint to the given\nFastAPI. With `should_gzip` you can instruct the endpoint to compress the data\nas long as the client accepts gzip encoding. Prometheus for example does by\ndefault. Beware that network bandwith is often cheaper than CPU cycles.\n\n```python\ninstrumentator.expose(app, include_in_schema=False, should_gzip=True)\n```\n\nNotice that this will to nothing if `should_respect_env_var` has been set during\nconstruction of the instrumentator object and the respective env var is not\nfound.\n\n## Contributing\n\nPlease refer to [`CONTRIBUTING.md`](CONTRIBUTING).\n\nConsult [`DEVELOPMENT.md`](DEVELOPMENT.md) for guidance regarding development.\n\nRead [`RELEASE.md`](RELEASE.md) for details about the release process.\n\n## Licensing\n\nThe default license for this project is the\n[ISC License](https://choosealicense.com/licenses/isc). A permissive license\nfunctionally equivalent to the BSD 2-Clause and MIT licenses, removing some\nlanguage that is no longer necessary. See [`LICENSE`](LICENSE) for the license\ntext.\n\nThe [BSD 3-Clause License](https://choosealicense.com/licenses/bsd-3-clause) is\nused as the license for the\n[`routing`](src/prometheus_fastapi_instrumentator/routing.py) module. This is\ndue to it containing code from\n[elastic/apm-agent-python](https://github.com/elastic/apm-agent-python). BSD\n3-Clause is a permissive license similar to the BSD 2-Clause License, but with a\n3rd clause that prohibits others from using the name of the copyright holder or\nits contributors to promote derived products without written consent. The\nlicense text is included in the module itself.\n',
     'author': 'Tim Schwenke',
     'author_email': 'tim@trallnag.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/trallnag/prometheus-fastapi-instrumentator',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `prometheus_fastapi_instrumentator-6.0.0/PKG-INFO` & `prometheus_fastapi_instrumentator-6.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-fastapi-instrumentator
-Version: 6.0.0
+Version: 6.1.0
 Summary: Instrument your FastAPI with Prometheus metrics.
 Home-page: https://github.com/trallnag/prometheus-fastapi-instrumentator
 License: ISC
 Keywords: prometheus,instrumentation,fastapi,exporter,metrics
 Author: Tim Schwenke
 Author-email: tim@trallnag.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -59,16 +59,16 @@
 
 - Counter `http_requests_total` with `handler`, `status` and `method`. Total
   number of requests.
 - Summary `http_request_size_bytes` with `handler`. Added up total of the
   content lengths of all incoming requests.
 - Summary `http_response_size_bytes` with `handler`. Added up total of the
   content lengths of all outgoing responses.
-- Histogram `http_request_duration_seconds` with `handler`. Only a few buckets
-  to keep cardinality low.
+- Histogram `http_request_duration_seconds` with `handler` and `method`. Only a
+  few buckets to keep cardinality low.
 - Histogram `http_request_duration_highr_seconds` without any labels. Large
   number of buckets (>20).
 
 In addition, following behavior is active:
 
 - Status codes are grouped into `2xx`, `3xx` and so on.
 - Requests without a matching template are grouped into the handler `none`.
@@ -80,35 +80,40 @@
   [`metrics`](./src/prometheus_fastapi_instrumentator/metrics.py) and pass it to
   the instrumentator instance. See [here](#adding-metrics) how to do that.
 - Create your own instrumentation function that you can pass to an
   instrumentator instance. See [here](#creating-new-metrics) to learn how more.
 - Don't use this package at all and just use the source code as inspiration on
   how to instrument your FastAPI.
 
-Important: This package is not made for generic Prometheus instrumentation in
-Python. Use the Prometheus client library for that. This packages uses it as
-well.
-
 ## Table of Contents <!-- omit in toc -->
 
 <!--TOC-->
 
+- [Disclaimer](#disclaimer)
 - [Features](#features)
 - [Advanced Usage](#advanced-usage)
   - [Creating the Instrumentator](#creating-the-instrumentator)
   - [Adding metrics](#adding-metrics)
   - [Creating new metrics](#creating-new-metrics)
   - [Perform instrumentation](#perform-instrumentation)
   - [Specify namespace and subsystem](#specify-namespace-and-subsystem)
   - [Exposing endpoint](#exposing-endpoint)
 - [Contributing](#contributing)
 - [Licensing](#licensing)
 
 <!--TOC-->
 
+## Disclaimer
+
+Not made for generic Prometheus instrumentation in Python. Use the Prometheus
+client library for that. This packages uses it as well.
+
+All the generic middleware and instrumentation code comes with a cost in
+performance that can become noticeable.
+
 ## Features
 
 Beyond the fast track, this instrumentator is **highly configurable** and it is
 very easy to customize and adapt to your specific use case. Here is a list of
 some of these options you may opt-in to:
 
 - Regex patterns to ignore certain routes.
```

