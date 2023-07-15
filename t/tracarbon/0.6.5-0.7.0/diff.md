# Comparing `tmp/tracarbon-0.6.5.tar.gz` & `tmp/tracarbon-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracarbon-0.6.5.tar", max compression
+gzip compressed data, was "tracarbon-0.7.0.tar", max compression
```

## Comparing `tracarbon-0.6.5.tar` & `tracarbon-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0    10264 2023-06-07 14:21:37.910555 tracarbon-0.6.5/LICENSE.txt
--rw-r--r--   0        0        0     9707 2023-06-07 14:21:37.910555 tracarbon-0.6.5/README.md
--rw-r--r--   0        0        0     2665 2023-06-07 14:21:37.914555 tracarbon-0.6.5/pyproject.toml
--rwxr-xr-x   0        0        0      246 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/__init__.py
--rw-r--r--   0        0        0       70 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/__main__.py
--rw-r--r--   0        0        0     2225 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/builder.py
--rw-r--r--   0        0        0     4517 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/cli/__init__.py
--rwxr-xr-x   0        0        0     2320 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/conf.py
--rw-r--r--   0        0        0       51 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/emissions/__init__.py
--rw-r--r--   0        0        0     6361 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/emissions/carbon_emissions.py
--rw-r--r--   0        0        0      734 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exceptions.py
--rwxr-xr-x   0        0        0      237 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/__init__.py
--rwxr-xr-x   0        0        0     2207 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/datadog_exporter.py
--rwxr-xr-x   0        0        0     3617 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/exporter.py
--rw-r--r--   0        0        0     2126 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/json_exporter.py
--rw-r--r--   0        0        0     2524 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/prometheus_exporter.py
--rwxr-xr-x   0        0        0      886 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/stdout.py
--rw-r--r--   0        0        0    10599 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/general_metrics.py
--rwxr-xr-x   0        0        0      210 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/__init__.py
--rw-r--r--   0        0        0     1303 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/cloud_providers.py
--rw-r--r--   0        0        0     4876 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/containers.py
--rw-r--r--   0        0        0        0 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/data/__init__.py
--rw-r--r--   0        0        0   160141 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/data/aws-instances.csv
--rw-r--r--   0        0        0     4720 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/energy.py
--rw-r--r--   0        0        0     1362 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/gpu.py
--rwxr-xr-x   0        0        0     1653 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/hardware.py
--rw-r--r--   0        0        0     6166 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/rapl.py
--rw-r--r--   0        0        0     7242 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/sensors.py
--rwxr-xr-x   0        0        0       85 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/__init__.py
--rw-r--r--   0        0        0     6103 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/country.py
--rw-r--r--   0        0        0        0 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/data/__init__.py
--rw-r--r--   0        0        0     1614 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json
--rw-r--r--   0        0        0     1179 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/data/grid-emissions-factors-aws.csv
--rwxr-xr-x   0        0        0     1576 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/location.py
--rw-r--r--   0        0        0        0 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/py.typed
--rw-r--r--   0        0        0    11290 1970-01-01 00:00:00.000000 tracarbon-0.6.5/PKG-INFO
+-rwxr-xr-x   0        0        0    10265 2023-07-15 20:17:41.581233 tracarbon-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     9752 2023-07-15 20:17:41.581233 tracarbon-0.7.0/README.md
+-rw-r--r--   0        0        0     2702 2023-07-15 20:17:41.585233 tracarbon-0.7.0/pyproject.toml
+-rwxr-xr-x   0        0        0      246 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/__main__.py
+-rw-r--r--   0        0        0     3158 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/builder.py
+-rw-r--r--   0        0        0     4609 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/cli/__init__.py
+-rwxr-xr-x   0        0        0     2320 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/conf.py
+-rw-r--r--   0        0        0      111 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/emissions/__init__.py
+-rw-r--r--   0        0        0     6361 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/emissions/carbon_emissions.py
+-rw-r--r--   0        0        0      734 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exceptions.py
+-rwxr-xr-x   0        0        0      237 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/__init__.py
+-rwxr-xr-x   0        0        0     2288 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/datadog_exporter.py
+-rwxr-xr-x   0        0        0     4999 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/exporter.py
+-rw-r--r--   0        0        0     2203 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/json_exporter.py
+-rw-r--r--   0        0        0     2605 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/prometheus_exporter.py
+-rwxr-xr-x   0        0        0      963 2023-07-15 20:17:41.585233 tracarbon-0.7.0/tracarbon/exporters/stdout.py
+-rw-r--r--   0        0        0    10784 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/general_metrics.py
+-rwxr-xr-x   0        0        0      210 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/__init__.py
+-rw-r--r--   0        0        0     1303 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/cloud_providers.py
+-rw-r--r--   0        0        0     4876 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/containers.py
+-rw-r--r--   0        0        0        0 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/data/__init__.py
+-rw-r--r--   0        0        0   160142 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/data/aws-instances.csv
+-rw-r--r--   0        0        0     4720 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/energy.py
+-rw-r--r--   0        0        0     1362 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/gpu.py
+-rwxr-xr-x   0        0        0     1653 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/hardware.py
+-rw-r--r--   0        0        0     6166 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/rapl.py
+-rw-r--r--   0        0        0     7242 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/hardwares/sensors.py
+-rwxr-xr-x   0        0        0       85 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/__init__.py
+-rw-r--r--   0        0        0     6103 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/country.py
+-rw-r--r--   0        0        0        0 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/data/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json
+-rw-r--r--   0        0        0     1180 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/data/grid-emissions-factors-aws.csv
+-rwxr-xr-x   0        0        0     1576 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/locations/location.py
+-rw-r--r--   0        0        0        0 2023-07-15 20:17:41.589233 tracarbon-0.7.0/tracarbon/py.typed
+-rw-r--r--   0        0        0    11335 1970-01-01 00:00:00.000000 tracarbon-0.7.0/PKG-INFO
```

### Comparing `tracarbon-0.6.5/LICENSE.txt` & `tracarbon-0.7.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -172,8 +172,8 @@
       License. However, in accepting such obligations, You may act only
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
-   END OF TERMS AND CONDITIONS
+   END OF TERMS AND CONDITIONS
```

### Comparing `tracarbon-0.6.5/README.md` & `tracarbon-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![doc](https://img.shields.io/badge/docs-python-blue.svg?style=for-the-badgee)](https://fvaleye.github.io/tracarbon)
 [![licence](https://img.shields.io/badge/license-Apache--2.0-green)](https://github.com/fvaleye/tracarbon/blob/main/LICENSE.txt)
 
 
 ## 📌 Overview
 Tracarbon is a Python library that tracks your device's energy consumption and calculates your carbon emissions.
 
-It detects your location and your device automatically before starting to export measurements to an exporter. 
+It detects your location and your device automatically before starting to export measurements to an exporter.
 It could be used as a CLI with already defined metrics or programmatically with the API by defining the metrics that you want to have.
 
 Read more in this [article](https://medium.com/@florian.valeye/tracarbon-track-your-devices-carbon-footprint-fb051fcc9009).
 
 ## 📦 Where to get it
 
 ```sh
@@ -87,14 +87,16 @@
 tracarbon = TracarbonBuilder(configuration=configuration).build()
 tracarbon.start()
 # Your code
 tracarbon.stop()
 
 with tracarbon:
     # Your code
+
+report = tracarbon.report() # Get the report
 ```
 
 ## 💻 Development
 
 **Local: using Poetry**
 ```sh
 make init
```

### Comparing `tracarbon-0.6.5/pyproject.toml` & `tracarbon-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 [tool.poetry]
 name = "tracarbon"
 authors = ["Florian Valeye <fvaleye@github.com>"]
-version = "0.6.5"
+version = "0.7.0"
 description = "Tracarbon is a Python library that tracks your device's energy consumption and calculates your carbon emissions."
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["energy", "sustainability", "energy-consumption", "electricity-consumption", "energy-efficiency", "carbon-footprint", "carbon-emissions"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only"
 ]
 include = ["tracarbon/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 loguru = ">=0.6,<0.8"
-aiohttp = "^3.8.1"
-aiocache = "^0.12.0"
+aiohttp = "^3.8.4"
+aiocache = "^0.12.1"
 aiofiles = "^23.1.0"
 psutil = "^5.9.4"
-ujson = "^5.7.0"
+ujson = "^5.8.0"
 msgpack = "^1.0.4"
-pydantic = "^1.10.7"
+pydantic = ">=1.10.7,<3.0.0"
 typer = ">=0.7,<0.10"
-ec2-metadata = "^2.11.0"
+ec2-metadata = "^2.13.0"
 python-dotenv = ">=0.21,<1.1"
 datadog = {version = ">=0.44,<0.46", optional = true}
 prometheus-client = {version = ">=0.16,<0.18", optional = true}
 kubernetes = {version = "^26.1.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.3"
 black = "^23.3.0"
-isort = "^5.11.5"
-pytest = "^7.3.1"
-pytest-mock = "^3.7.0"
+isort = "^5.12.0"
+pytest = "^7.3.2"
+pytest-mock = "^3.11.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.3.1"
 pytest-clarity = "^1.0.1"
 sphinx = "^7.0.1"
 pydata-sphinx-theme = "^0.13.3"
 toml = "^0.10.2"
-types-ujson = "^5.7.0"
+types-ujson = "^5.8.0"
 datadog = ">=0.44,<0.46"
 prometheus-client = ">=0.16,<0.18"
 types-requests = "^2.31.0"
 bandit = "^1.7.4"
 radon = "^6.0.1"
 types-aiofiles = "^23.1.0"
 kubernetes = "^26.1.0"
+autodoc_pydantic = "1.9.0"
 
 [tool.poetry.extras]
 datadog = ["datadog"]
 prometheus = ["prometheus-client"]
 kubernetes = ["kubernetes"]
 
 [tool.poetry.scripts]
@@ -100,8 +101,8 @@
 markers = [
     "darwin",
     "windows",
     "linux"
 ]
 testpaths = [
     "tests",
-]
+]
```

### Comparing `tracarbon-0.6.5/tracarbon/builder.py` & `tracarbon-0.7.0/tracarbon/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,114 @@
-from typing import Optional
+import datetime
+from typing import Dict, Optional
 
 from pydantic import BaseModel
 
 from tracarbon.conf import TracarbonConfiguration
-from tracarbon.exporters import Exporter, StdoutExporter
+from tracarbon.exporters import Exporter, MetricGenerator, MetricReport, StdoutExporter
 from tracarbon.general_metrics import CarbonEmissionGenerator
 from tracarbon.locations import Country, Location
 
 
+class TracarbonReport(BaseModel):
+    """
+    Tracarbon report to store running statistics.
+    """
+
+    start_time: Optional[datetime.datetime] = None
+    end_time: Optional[datetime.datetime] = None
+    metric_report: Dict[str, MetricReport] = dict()
+
+    class Config:
+        """Pydantic configuration."""
+
+        arbitrary_types_allowed = True
+
+
 class Tracarbon:
     """
     Tracarbon instance.
     """
 
     configuration: TracarbonConfiguration
     exporter: Exporter
     location: Location
+    report: TracarbonReport = TracarbonReport()
 
     def __init__(
         self,
         configuration: TracarbonConfiguration,
         exporter: Optional[Exporter],
         location: Optional[Location],
     ) -> None:
         self.configuration = configuration
-        if location:
-            self.location = location
-        else:
-            self.location = Country.get_location(
-                co2signal_api_key=self.configuration.co2signal_api_key,
-                co2signal_url=self.configuration.co2signal_url,
-            )
-        if exporter:
-            self.exporter = exporter
-        else:
-            self.exporter = StdoutExporter(
-                metric_generators=[CarbonEmissionGenerator(location=self.location)]
-            )
+        self.exporter = exporter
+        self.location = location
 
     def __enter__(self) -> None:
-        self.exporter.start(interval_in_seconds=self.configuration.interval_in_seconds)
+        self.start()
 
     def __exit__(self, type, value, traceback) -> None:  # type: ignore
-        self.exporter.stop()
+        self.stop()
 
     def start(self) -> None:
         """
         Start Tracarbon.
         """
+        self.report.start_time = datetime.datetime.now()
         self.exporter.start(interval_in_seconds=self.configuration.interval_in_seconds)
 
     def stop(self) -> None:
         """
         Stop Tracarbon.
         """
+        self.report.metric_report = self.exporter.metric_report
+        self.report.end_time = datetime.datetime.now()
         self.exporter.stop()
 
 
 class TracarbonBuilder(BaseModel):
     """
     Tracarbon builder for building Tracarbon.
     """
 
+    exporter: Optional[Exporter] = None
+    location: Optional[Location] = None
     configuration: TracarbonConfiguration = TracarbonConfiguration()
 
-    def build(
-        self, exporter: Optional[Exporter] = None, location: Optional[Location] = None
-    ) -> Tracarbon:
+    def with_location(self, location: Location) -> "TracarbonBuilder":
         """
-        Build Tracarbon with its configuration.
+        Add a location to the builder.
+        :param location: the location
+        :return:
+        """
+        self.location = location
+        return self
+
+    def with_exporter(self, exporter: Exporter) -> "TracarbonBuilder":
+        """
+        Add an exporter to the builder.
+        :param exporter: the exporter
+        :return:
+        """
+        self.exporter = exporter
+        return self
 
-        :param exporter: the exporter to use
-        :param location: the location to use
+    def build(self) -> Tracarbon:
+        """
+        Build Tracarbon with its configuration.
         """
+        if not self.location:
+            self.location = Country.get_location(
+                co2signal_api_key=self.configuration.co2signal_api_key,
+                co2signal_url=self.configuration.co2signal_url,
+            )
+        if not self.exporter:
+            self.exporter = StdoutExporter(
+                metric_generators=[CarbonEmissionGenerator(location=self.location)]
+            )
 
         return Tracarbon(
             configuration=self.configuration,
-            exporter=exporter,
-            location=location,
+            exporter=self.exporter,
+            location=self.location,
         )
```

### Comparing `tracarbon-0.6.5/tracarbon/cli/__init__.py` & `tracarbon-0.7.0/tracarbon/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,26 +106,28 @@
         metric_generators.extend(add_containers_generator(location=location))
     try:
         exporter = get_exporter(
             exporter_name=exporter_name,
             metric_generators=metric_generators,
             tracarbon_builder=tracarbon_builder,
         )
-        tracarbon = tracarbon_builder.build(
-            location=location,
-            exporter=exporter,
+        tracarbon = (
+            tracarbon_builder.with_location(location=location)
+            .with_exporter(exporter=exporter)
+            .build()
         )
         from loguru import logger
 
         logger.info("Tracarbon CLI started.")
         with tracarbon:
             while running:
                 time.sleep(tracarbon_builder.configuration.interval_in_seconds)
     except KeyboardInterrupt:
-        logger.info("Tracarbon CLI exited.")
+        pass
+    logger.info(f"Tracarbon CLI exited. Tracarbon report: {tracarbon.report}")
 
 
 @app.command()
 def run(
     exporter_name: str = "Stdout",
     country_code_alpha_iso_2: Optional[str] = None,
     containers: bool = False,
```

### Comparing `tracarbon-0.6.5/tracarbon/conf.py` & `tracarbon-0.7.0/tracarbon/conf.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/emissions/carbon_emissions.py` & `tracarbon-0.7.0/tracarbon/emissions/carbon_emissions.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/exceptions.py` & `tracarbon-0.7.0/tracarbon/exceptions.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/exporters/datadog_exporter.py` & `tracarbon-0.7.0/tracarbon/exporters/datadog_exporter.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,14 +51,15 @@
                     )
                     logger.info(
                         f"Sending metric[{metric_name}] with value [{metric_value}] and tags{metric.format_tags()} to Datadog."
                     )
                     self.stats.gauge(
                         metric_name, metric_value, tags=metric.format_tags()
                     )
+                    self.add_metric_to_report(metric=metric, value=metric_value)
 
         @classmethod
         def get_name(cls) -> str:
             """
             Get the name of the exporter.
 
             :return: the Exporter's name
```

### Comparing `tracarbon-0.6.5/tracarbon/exporters/exporter.py` & `tracarbon-0.7.0/tracarbon/exporters/exporter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,115 @@
 import asyncio
+import sys
 from abc import ABCMeta, abstractmethod
 from threading import Event, Timer
-from typing import AsyncGenerator, Awaitable, Callable, List, Optional
+from typing import AsyncGenerator, Awaitable, Callable, Dict, List, Optional
 
 from loguru import logger
 from pydantic import BaseModel
 
 from tracarbon.hardwares.hardware import HardwareInfo
 from tracarbon.locations import Location
 
 
+class Tag(BaseModel):
+    """
+    Tag for a metric.
+    """
+
+    key: str
+    value: str
+
+
+class Metric(BaseModel):
+    """
+    Global metric to use for the exporters.
+    """
+
+    name: str
+    value: Callable[[], Awaitable[float]]
+    tags: List[Tag] = list()
+
+    def format_name(
+        self, metric_prefix_name: Optional[str] = None, separator: str = "."
+    ) -> str:
+        """
+        Format the name of the metric with a prefix and separator.
+
+        :param metric_prefix_name: the prefix to insert before the separator and the name.
+        :param separator: the separator to use between the prefix and the name.
+        """
+        if metric_prefix_name:
+            return f"{metric_prefix_name}{separator}{self.name}"
+        return self.name
+
+    def format_tags(self, separator: str = ":") -> List[str]:
+        """
+        Format tags with a separator.
+
+        :param separator: the separator to insert between the key and value.
+        """
+        return [f"{tag.key}{separator}{tag.value}" for tag in self.tags]
+
+
+class MetricReport(BaseModel):
+    """
+    MetricReport is a report of the generated metrics.
+    """
+
+    exporter_name: str
+    metric: "Metric"
+    total: float = 0.0
+    average: float = 0.0
+    minimum: float = sys.float_info.max
+    maximum: float = 0.0
+    call_count: int = 0
+
+    class Config:
+        """Pydantic configuration."""
+
+        arbitrary_types_allowed = True
+
+
+class MetricGenerator(BaseModel):
+    """
+    MetricGenerator generates metrics for the Exporter.
+    """
+
+    metrics: List[Metric]
+    platform: str = HardwareInfo.get_platform()
+    location: Optional[Location] = None
+
+    async def generate(self) -> AsyncGenerator[Metric, None]:
+        """
+        Generate a metric.
+        """
+        for metric in self.metrics:
+            yield metric
+
+
 class Exporter(BaseModel, metaclass=ABCMeta):
     """The Exporter interface."""
 
-    metric_generators: List["MetricGenerator"]
+    metric_generators: List[MetricGenerator]
     event: Optional[Event] = None
     stopped: bool = False
     metric_prefix_name: Optional[str] = None
+    metric_report: Dict[str, MetricReport] = dict()
 
     class Config:
         """Pydantic configuration."""
 
         arbitrary_types_allowed = True
 
     @abstractmethod
     async def launch(self, metric_generator: "MetricGenerator") -> None:
         """
         Launch the exporter.
+        Add the metric generator to the metric reporter.
 
         :param metric_generator: the metric generator
         """
         pass
 
     def start(self, interval_in_seconds: int) -> None:
         """
@@ -45,14 +124,15 @@
         def _run() -> None:
             asyncio.run(self._launch_all())
             if self.event and not self.stopped and not self.event.is_set():
                 timer = Timer(interval_in_seconds, _run, [])
                 timer.daemon = True
                 timer.start()
 
+        self.metric_report = dict()
         _run()
 
     def stop(self) -> None:
         """
         Stop the explorer and the associated timer.
 
         :return:
@@ -65,73 +145,37 @@
         """
         Launch the exporter with all the metric generators.
         """
         for metric_generator in self.metric_generators:
             logger.debug(f"Running MetricGenerator[{metric_generator}].")
             await self.launch(metric_generator=metric_generator)
 
+    def add_metric_to_report(self, metric: "Metric", value: float) -> "MetricReport":
+        """
+        Add the generated metric to the report.
+
+        :param metric: the metric to add
+        :param value: the metric value to add
+        """
+        if metric.name not in self.metric_report:
+            self.metric_report[metric.name] = MetricReport(
+                exporter_name=self.get_name(), metric=metric
+            )
+        metric_report = self.metric_report[metric.name]
+        metric_report.total += value
+        metric_report.call_count += 1
+        metric_report.average = metric_report.total / metric_report.call_count
+        if value < metric_report.minimum:
+            metric_report.minimum = value
+        if value > metric_report.maximum:
+            metric_report.maximum = value
+        return metric_report
+
     @classmethod
     @abstractmethod
     def get_name(cls) -> str:
         """
         Get the name of the exporter.
 
         :return: the Exporter's name
         """
         pass
-
-
-class Tag(BaseModel):
-    """
-    Tag for a metric.
-    """
-
-    key: str
-    value: str
-
-
-class Metric(BaseModel):
-    """
-    Global metric to use for the exporters.
-    """
-
-    name: str
-    value: Callable[[], Awaitable[float]]
-    tags: List[Tag] = list()
-
-    def format_name(
-        self, metric_prefix_name: Optional[str] = None, separator: str = "."
-    ) -> str:
-        """
-        Format the name of the metric with a prefix and separator.
-
-        :param metric_prefix_name: the prefix to insert before the separator and the name.
-        :param separator: the separator to use between the prefix and the name.
-        """
-        if metric_prefix_name:
-            return f"{metric_prefix_name}{separator}{self.name}"
-        return self.name
-
-    def format_tags(self, separator: str = ":") -> List[str]:
-        """
-        Format tags with a separator.
-
-        :param separator: the separator to insert between the key and value.
-        """
-        return [f"{tag.key}{separator}{tag.value}" for tag in self.tags]
-
-
-class MetricGenerator(BaseModel):
-    """
-    MetricGenerator generates metrics for the Exporter.
-    """
-
-    metrics: List[Metric]
-    platform: str = HardwareInfo.get_platform()
-    location: Optional[Location] = None
-
-    async def generate(self) -> AsyncGenerator[Metric, None]:
-        """
-        Generate a metric.
-        """
-        for metric in self.metrics:
-            yield metric
```

### Comparing `tracarbon-0.6.5/tracarbon/exporters/json_exporter.py` & `tracarbon-0.7.0/tracarbon/exporters/json_exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
                                 ),
                                 "metric_value": metric_value,
                                 "metric_tags": metric.format_tags(),
                             },
                             indent=self.indent,
                         )
                     )
+                self.add_metric_to_report(metric=metric, value=metric_value)
 
     @classmethod
     def get_name(cls) -> str:
         """
         Get the name of the exporter.
 
         :return: the Exporter's name
```

### Comparing `tracarbon-0.6.5/tracarbon/exporters/prometheus_exporter.py` & `tracarbon-0.7.0/tracarbon/exporters/prometheus_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
                 if metric_value:
                     logger.info(
                         f"Sending metric[{metric_name}] with value [{metric_value}] and labels{metric.format_tags()} to Prometheus."
                     )
                     self.prometheus_metrics[metric_name].labels(
                         *[tag.value for tag in metric.tags]
                     ).set(metric_value)
+                    self.add_metric_to_report(metric=metric, value=metric_value)
 
         @classmethod
         def get_name(cls) -> str:
             """
             Get the name of the exporter.
 
             :return: the Exporter's name
```

### Comparing `tracarbon-0.6.5/tracarbon/exporters/stdout.py` & `tracarbon-0.7.0/tracarbon/exporters/stdout.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         """
         async for metric in metric_generator.generate():
             metric_value = await metric.value()
             if metric_value:
                 logger.info(
                     f"Metric name[{metric.format_name(metric_prefix_name=self.metric_prefix_name)}], value[{metric_value}], tags{metric.format_tags()}"
                 )
+                self.add_metric_to_report(metric=metric, value=metric_value)
 
     @classmethod
     def get_name(cls) -> str:
         """
         Get the name of the exporter.
 
         :return: the Exporter's name
```

### Comparing `tracarbon-0.6.5/tracarbon/general_metrics.py` & `tracarbon-0.7.0/tracarbon/general_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from typing import Any, AsyncGenerator, Optional
 
 from tracarbon.conf import KUBERNETES_INSTALLED
 from tracarbon.emissions import CarbonEmission, CarbonUsageUnit
 from tracarbon.exporters import Metric, MetricGenerator, Tag
 from tracarbon.hardwares import EnergyConsumption, EnergyUsageUnit, UsageType
-from tracarbon.locations import Location
+from tracarbon.locations import Country, Location
 
 
 class EnergyConsumptionGenerator(MetricGenerator):
     """
     Energy consumption generator for energy consumption.
     """
 
     energy_consumption: EnergyConsumption
 
-    def __init__(self, location: Location, **data: Any) -> None:
+    def __init__(self, location: Optional[Location] = None, **data: Any) -> None:
         if "energy_consumption" not in data:
             data["energy_consumption"] = EnergyConsumption.from_platform()
+        if not location:
+            location = Country.get_location()
         super().__init__(location=location, metrics=[], **data)
 
     async def generate(self) -> AsyncGenerator[Metric, None]:
         """
         Generate a metric for energy consumption.
 
         :return: an async generator of the metrics
@@ -50,15 +52,17 @@
     """
     Carbon emission generator to generate carbon emissions.
     """
 
     carbon_emission: CarbonEmission
     co2signal_api_key: Optional[str] = None
 
-    def __init__(self, location: Location, **data: Any) -> None:
+    def __init__(self, location: Optional[Location] = None, **data: Any) -> None:
+        if not location:
+            location = Country.get_location()
         if "carbon_emission" not in data:
             data["carbon_emission"] = CarbonEmission(
                 co2signal_api_key=data["co2signal_api_key"]
                 if "co2signal_api_key" in data
                 else location.co2signal_api_key,
                 co2signal_url=data["co2signal_url"]
                 if "co2signal_url" in data
```

### Comparing `tracarbon-0.6.5/tracarbon/hardwares/cloud_providers.py` & `tracarbon-0.7.0/tracarbon/hardwares/cloud_providers.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/hardwares/containers.py` & `tracarbon-0.7.0/tracarbon/hardwares/containers.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/hardwares/data/aws-instances.csv` & `tracarbon-0.7.0/tracarbon/hardwares/data/aws-instances.csv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -615,8 +615,8 @@
 db.t3.xlarge,August 2018,4,96,Xeon Platinum 8175M,16,384,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"2,41","6,11","14,32","19,92","2,41","3,85","9,92","15,99","0,0","0,0","0,0","0,0","4,0","8,8","14,0","28,2","39,9",2.5 GHz Intel Scalable Processor
 db.t3.2xlarge,August 2018,8,96,Xeon Platinum 8175M,32,384,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"4,82","12,22","28,64","39,83","4,82","7,70","19,84","31,98","0,0","0,0","0,0","0,0","8,0","17,6","27,9","56,5","79,8",2.5 GHz Intel Scalable Processor
 db.t2.micro,July 2014,1,48,Xeon E5-2676 v3,1,288,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"0,60","1,72","3,54","4,85","0,20","0,30","0,40","0,60","0,0","0,0","0,0","0,0","1,0","1,8","3,0","4,9","6,4",3.3 GHz Intel Scalable Processor
 db.t2.small,July 2014,1,48,Xeon E5-2676 v3,2,288,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"0,60","1,72","3,54","4,85","0,40","0,60","0,80","1,20","0,0","0,0","0,0","0,0","1,0","2,0","3,3","5,3","7,0",3.3 GHz Intel Scalable Processor
 db.t2.medium,July 2014,2,48,Xeon E5-2676 v3,4,288,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"1,21","3,44","7,08","9,69","0,80","1,20","1,60","2,40","0,0","0,0","0,0","0,0","2,0","4,0","6,6","10,7","14,1",3.3 GHz Intel Scalable Processor
 db.t2.large,June 2015,2,48,Xeon E5-2676 v3,8,288,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"1,21","3,44","7,08","9,69","1,60","2,40","3,20","4,80","0,0","0,0","0,0","0,0","2,0","4,8","7,8","12,3","16,5",3.3 GHz Intel Scalable Processor
 db.t2.xlarge,November 2016,4,48,Xeon E5-2676 v3,16,288,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"2,41","6,89","14,16","19,39","3,20","4,80","6,40","9,60","0,0","0,0","0,0","0,0","4,0","9,6","15,7","24,6","33,0",3.3 GHz Intel Scalable Processor
-db.t2.2xlarge,November 2016,8,48,Xeon E5-2676 v3,32,288,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"4,82","13,77","28,33","38,78","6,40","9,60","12,80","19,20","0,0","0,0","0,0","0,0","8,0","19,2","31,4","49,1","66,0",3.3 GHz Intel Scalable Processor
+db.t2.2xlarge,November 2016,8,48,Xeon E5-2676 v3,32,288,EBS-Only,EBS,0,N/A,N/A,N/A,N/A,"4,82","13,77","28,33","38,78","6,40","9,60","12,80","19,20","0,0","0,0","0,0","0,0","8,0","19,2","31,4","49,1","66,0",3.3 GHz Intel Scalable Processor
```

### Comparing `tracarbon-0.6.5/tracarbon/hardwares/energy.py` & `tracarbon-0.7.0/tracarbon/hardwares/energy.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/hardwares/gpu.py` & `tracarbon-0.7.0/tracarbon/hardwares/gpu.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/hardwares/hardware.py` & `tracarbon-0.7.0/tracarbon/hardwares/hardware.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/hardwares/rapl.py` & `tracarbon-0.7.0/tracarbon/hardwares/rapl.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/hardwares/sensors.py` & `tracarbon-0.7.0/tracarbon/hardwares/sensors.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/locations/country.py` & `tracarbon-0.7.0/tracarbon/locations/country.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json` & `tracarbon-0.7.0/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 4% similar despite different names*

```diff
@@ -89,13 +89,13 @@
 00000580: 2e34 2c0a 2020 2020 2020 226e 616d 6522  .4,.      "name"
 00000590: 3a20 2265 7322 0a20 2020 207d 2c0a 2020  : "es".    },.  
 000005a0: 2020 7b0a 2020 2020 2020 2263 6f32 675f    {.      "co2g_
 000005b0: 6b77 6822 3a20 3538 2e35 2c0a 2020 2020  kwh": 58.5,.    
 000005c0: 2020 226e 616d 6522 3a20 226c 7522 0a20    "name": "lu". 
 000005d0: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
 000005e0: 2020 2263 6f32 675f 6b77 6822 3a20 3239    "co2g_kwh": 29
-000005f0: 392e 352c 200a 2020 2020 2020 226e 616d  9.5, .      "nam
-00000600: 6522 3a20 2272 6f22 0a20 2020 207d 2c0a  e": "ro".    },.
-00000610: 2020 2020 7b0a 2020 2020 2020 2263 6f32      {.      "co2
-00000620: 675f 6b77 6822 3a20 3632 302e 392c 200a  g_kwh": 620.9, .
-00000630: 2020 2020 2020 226e 616d 6522 3a20 2263        "name": "c
-00000640: 7922 0a20 2020 207d 0a20 205d 0a7d       y".    }.  ].}
+000005f0: 392e 352c 0a20 2020 2020 2022 6e61 6d65  9.5,.      "name
+00000600: 223a 2022 726f 220a 2020 2020 7d2c 0a20  ": "ro".    },. 
+00000610: 2020 207b 0a20 2020 2020 2022 636f 3267     {.      "co2g
+00000620: 5f6b 7768 223a 2036 3230 2e39 2c0a 2020  _kwh": 620.9,.  
+00000630: 2020 2020 226e 616d 6522 3a20 2263 7922      "name": "cy"
+00000640: 0a20 2020 207d 0a20 205d 0a7d 0a         .    }.  ].}.
```

### Comparing `tracarbon-0.6.5/tracarbon/locations/data/grid-emissions-factors-aws.csv` & `tracarbon-0.7.0/tracarbon/locations/data/grid-emissions-factors-aws.csv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 eu-central-1,Germany,,0.000338,EEA
 eu-west-1,Ireland,,0.000316,EEA
 eu-west-2,England,,0.000228,EEA
 eu-south-1,Italy,,0.000233,EEA
 eu-west-3,France,,0.000052,EEA
 eu-north-1,Sweden,,0.000008,EEA
 me-south-1,Bahrain,,0.000732,carbonfootprint.com
-sa-east-1,Brazil,,0.000074,carbonfootprint.com
+sa-east-1,Brazil,,0.000074,carbonfootprint.com
```

### Comparing `tracarbon-0.6.5/tracarbon/locations/location.py` & `tracarbon-0.7.0/tracarbon/locations/location.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.5/PKG-INFO` & `tracarbon-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracarbon
-Version: 0.6.5
+Version: 0.7.0
 Summary: Tracarbon is a Python library that tracks your device's energy consumption and calculates your carbon emissions.
 License: Apache-2.0
 Keywords: energy,sustainability,energy-consumption,electricity-consumption,energy-efficiency,carbon-footprint,carbon-emissions
 Author: Florian Valeye
 Author-email: fvaleye@github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,42 +14,42 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: datadog
 Provides-Extra: kubernetes
 Provides-Extra: prometheus
-Requires-Dist: aiocache (>=0.12.0,<0.13.0)
+Requires-Dist: aiocache (>=0.12.1,<0.13.0)
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: datadog (>=0.44,<0.46) ; extra == "datadog"
-Requires-Dist: ec2-metadata (>=2.11.0,<3.0.0)
+Requires-Dist: ec2-metadata (>=2.13.0,<3.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0) ; extra == "kubernetes"
 Requires-Dist: loguru (>=0.6,<0.8)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: prometheus-client (>=0.16,<0.18) ; extra == "prometheus"
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=1.10.7,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21,<1.1)
 Requires-Dist: typer (>=0.7,<0.10)
-Requires-Dist: ujson (>=5.7.0,<6.0.0)
+Requires-Dist: ujson (>=5.8.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 ![Tracarbon Logo](https://raw.githubusercontent.com/fvaleye/tracarbon/main/logo.png "Tracarbon logo")
 
 ![example workflow](https://github.com/fvaleye/tracarbon/actions/workflows/build.yml/badge.svg)
 [![pypi](https://img.shields.io/pypi/v/tracarbon.svg?style=flat-square)](https://pypi.org/project/tracarbon/)
 [![doc](https://img.shields.io/badge/docs-python-blue.svg?style=for-the-badgee)](https://fvaleye.github.io/tracarbon)
 [![licence](https://img.shields.io/badge/license-Apache--2.0-green)](https://github.com/fvaleye/tracarbon/blob/main/LICENSE.txt)
 
 
 ## 📌 Overview
 Tracarbon is a Python library that tracks your device's energy consumption and calculates your carbon emissions.
 
-It detects your location and your device automatically before starting to export measurements to an exporter. 
+It detects your location and your device automatically before starting to export measurements to an exporter.
 It could be used as a CLI with already defined metrics or programmatically with the API by defining the metrics that you want to have.
 
 Read more in this [article](https://medium.com/@florian.valeye/tracarbon-track-your-devices-carbon-footprint-fb051fcc9009).
 
 ## 📦 Where to get it
 
 ```sh
@@ -123,14 +123,16 @@
 tracarbon = TracarbonBuilder(configuration=configuration).build()
 tracarbon.start()
 # Your code
 tracarbon.stop()
 
 with tracarbon:
     # Your code
+
+report = tracarbon.report() # Get the report
 ```
 
 ## 💻 Development
 
 **Local: using Poetry**
 ```sh
 make init
```

