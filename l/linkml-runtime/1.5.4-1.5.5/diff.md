# Comparing `tmp/linkml_runtime-1.5.4.tar.gz` & `tmp/linkml_runtime-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_runtime-1.5.4.tar", max compression
+gzip compressed data, was "linkml_runtime-1.5.5.tar", max compression
```

## Comparing `linkml_runtime-1.5.4.tar` & `linkml_runtime-1.5.5.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     7048 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/LICENSE
--rw-r--r--   0        0        0     1996 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/README.md
--rw-r--r--   0        0        0     1179 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/__init__.py
--rw-r--r--   0        0        0      507 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/__init__.py
--rw-r--r--   0        0        0      176 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/csv_dumper.py
--rw-r--r--   0        0        0     1418 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/delimited_file_dumper.py
--rw-r--r--   0        0        0      973 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/dumper_root.py
--rw-r--r--   0        0        0     4377 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/json_dumper.py
--rw-r--r--   0        0        0     4023 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/rdf_dumper.py
--rw-r--r--   0        0        0     7169 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/rdflib_dumper.py
--rw-r--r--   0        0        0      177 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/tsv_dumper.py
--rw-r--r--   0        0        0      901 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/yaml_dumper.py
--rw-r--r--   0        0        0        0 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/index/__init__.py
--rw-r--r--   0        0        0     8875 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/index/object_index.py
--rw-r--r--   0        0        0      119 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/README.md
--rw-r--r--   0        0        0      738 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/__init__.py
--rw-r--r--   0        0        0     3240 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/annotations.py
--rw-r--r--   0        0        0     3333 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/extensions.py
--rw-r--r--   0        0        0      114 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/graphql/README.md
--rw-r--r--   0        0        0    30306 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/graphql/meta.graphql
--rw-r--r--   0        0        0      111 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/README.md
--rw-r--r--   0        0        0    11169 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/annotations.json
--rw-r--r--   0        0        0     9306 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/extensions.json
--rw-r--r--   0        0        0    12109 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/mappings.json
--rw-r--r--   0        0        0   222072 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/meta.json
--rw-r--r--   0        0        0     6442 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/types.json
--rw-r--r--   0        0        0    22401 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/units.json
--rw-r--r--   0        0        0    14834 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/validation.json
--rw-r--r--   0        0        0      113 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/README.md
--rw-r--r--   0        0        0      648 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld
--rw-r--r--   0        0        0      648 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld
--rw-r--r--   0        0        0     7019 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/context.jsonld
--rw-r--r--   0        0        0      587 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld
--rw-r--r--   0        0        0      587 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld
--rw-r--r--   0        0        0     1615 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld
--rw-r--r--   0        0        0     1615 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld
--rw-r--r--   0        0        0    13814 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/meta.context.jsonld
--rw-r--r--   0        0        0    14266 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld
--rw-r--r--   0        0        0      610 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/types.context.jsonld
--rw-r--r--   0        0        0      610 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld
--rw-r--r--   0        0        0     2065 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/units.context.jsonld
--rw-r--r--   0        0        0     2065 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld
--rw-r--r--   0        0        0     1910 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/validation.context.jsonld
--rw-r--r--   0        0        0     1910 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld
--rw-r--r--   0        0        0      117 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/README.md
--rw-r--r--   0        0        0     4196 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/annotations.schema.json
--rw-r--r--   0        0        0     1984 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/extensions.schema.json
--rw-r--r--   0        0        0      297 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/mappings.schema.json
--rw-r--r--   0        0        0   353208 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/meta.schema.json
--rw-r--r--   0        0        0      291 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/types.schema.json
--rw-r--r--   0        0        0     5621 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/units.schema.json
--rw-r--r--   0        0        0     2291 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/validation.schema.json
--rw-r--r--   0        0        0     7126 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/linkml_files.py
--rw-r--r--   0        0        0     1821 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/mappings.py
--rw-r--r--   0        0        0   249036 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/meta.py
--rw-r--r--   0        0        0      112 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/README.md
--rw-r--r--   0        0        0      118 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/docs/credits.md
--rw-r--r--   0        0        0      141 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/docs/home.md
--rw-r--r--   0        0        0        5 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/import_map.json
--rw-r--r--   0        0        0      119 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/README.md
--rw-r--r--   0        0        0      833 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/annotations.yaml
--rw-r--r--   0        0        0     1057 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/extensions.yaml
--rw-r--r--   0        0        0     2755 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/mappings.yaml
--rw-r--r--   0        0        0    89120 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/meta.yaml
--rw-r--r--   0        0        0     3880 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/types.yaml
--rw-r--r--   0        0        0     2776 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/units.yaml
--rw-r--r--   0        0        0     2953 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/validation.yaml
--rw-r--r--   0        0        0      110 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/owl/README.md
--rw-r--r--   0        0        0   192274 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/owl/meta.owl.ttl
--rw-r--r--   0        0        0      110 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/README.md
--rw-r--r--   0        0        0    13054 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/annotations.model.ttl
--rw-r--r--   0        0        0    13054 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/annotations.ttl
--rw-r--r--   0        0        0    10932 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/extensions.model.ttl
--rw-r--r--   0        0        0    10932 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/extensions.ttl
--rw-r--r--   0        0        0    13825 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/mappings.model.ttl
--rw-r--r--   0        0        0    13825 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/mappings.ttl
--rw-r--r--   0        0        0   207795 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/meta.model.ttl
--rw-r--r--   0        0        0   207795 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/meta.ttl
--rw-r--r--   0        0        0     7565 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/types.model.ttl
--rw-r--r--   0        0        0     7565 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/types.ttl
--rw-r--r--   0        0        0    25276 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/units.model.ttl
--rw-r--r--   0        0        0    25276 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/units.ttl
--rw-r--r--   0        0        0    16810 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/validation.model.ttl
--rw-r--r--   0        0        0    16810 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/validation.ttl
--rw-r--r--   0        0        0      113 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/README.md
--rw-r--r--   0        0        0     1261 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/annotations.shex
--rw-r--r--   0        0        0     8918 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/annotations.shexj
--rw-r--r--   0        0        0      821 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/extensions.shex
--rw-r--r--   0        0        0     5303 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/extensions.shexj
--rw-r--r--   0        0        0      424 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/mappings.shex
--rw-r--r--   0        0        0     2568 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/mappings.shexj
--rw-r--r--   0        0        0    37441 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/meta.shex
--rw-r--r--   0        0        0   254576 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/meta.shexj
--rw-r--r--   0        0        0      459 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/types.shex
--rw-r--r--   0        0        0     2568 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/types.shexj
--rw-r--r--   0        0        0     1682 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/units.shex
--rw-r--r--   0        0        0    11643 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/units.shexj
--rw-r--r--   0        0        0     1519 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/validation.shex
--rw-r--r--   0        0        0     7343 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/validation.shexj
--rw-r--r--   0        0        0     4599 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/types.py
--rw-r--r--   0        0        0     3332 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/units.py
--rw-r--r--   0        0        0     6897 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/validation.py
--rw-r--r--   0        0        0      507 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/__init__.py
--rw-r--r--   0        0        0     1533 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/context_flattener.py
--rw-r--r--   0        0        0      179 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/csv_loader.py
--rw-r--r--   0        0        0     2776 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/delimited_file_loader.py
--rw-r--r--   0        0        0     1574 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/json_loader.py
--rw-r--r--   0        0        0     6855 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/loader_root.py
--rw-r--r--   0        0        0     4831 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/rdf_loader.py
--rw-r--r--   0        0        0    14214 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/rdflib_loader.py
--rw-r--r--   0        0        0     1358 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/requests_ssl_patch.py
--rw-r--r--   0        0        0      180 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/tsv_loader.py
--rw-r--r--   0        0        0     2223 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/yaml_loader.py
--rw-r--r--   0        0        0    42276 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/processing/referencevalidator.py
--rw-r--r--   0        0        0    26951 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/processing/validation_datamodel.py
--rw-r--r--   0        0        0    10253 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/processing/validation_datamodel.yaml
--rw-r--r--   0        0        0        0 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/__init__.py
--rw-r--r--   0        0        0      850 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/comparefiles.py
--rw-r--r--   0        0        0     1972 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/compile_python.py
--rw-r--r--   0        0        0     4034 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/context_utils.py
--rw-r--r--   0        0        0     2389 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/csvutils.py
--rw-r--r--   0        0        0      486 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/curienamespace.py
--rw-r--r--   0        0        0     1325 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/dataclass_extensions_376.py
--rw-r--r--   0        0        0      433 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/dictutils.py
--rw-r--r--   0        0        0     2554 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/distroutils.py
--rw-r--r--   0        0        0     3683 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/enumerations.py
--rw-r--r--   0        0        0     6755 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/eval_utils.py
--rw-r--r--   0        0        0     6594 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/formatutils.py
--rw-r--r--   0        0        0     5672 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/inference_utils.py
--rw-r--r--   0        0        0     1976 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/introspection.py
--rw-r--r--   0        0        0    11553 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/metamodelcore.py
--rw-r--r--   0        0        0    10580 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/namespaces.py
--rw-r--r--   0        0        0     2870 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/pattern.py
--rw-r--r--   0        0        0     6697 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/permissiblevalueimpl.py
--rw-r--r--   0        0        0     4720 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/ruleutils.py
--rw-r--r--   0        0        0     2287 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schema_as_dict.py
--rw-r--r--   0        0        0     9312 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schema_builder.py
--rw-r--r--   0        0        0     2815 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schemaops.py
--rw-r--r--   0        0        0    66900 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schemaview.py
--rw-r--r--   0        0        0     4327 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schemaview_cli.py
--rw-r--r--   0        0        0      368 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/slot.py
--rw-r--r--   0        0        0      641 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/strictness.py
--rw-r--r--   0        0        0     1405 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/walker_utils.py
--rw-r--r--   0        0        0    19743 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/yamlutils.py
--rw-r--r--   0        0        0     1848 2023-06-14 23:49:12.821710 linkml_runtime-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 linkml_runtime-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/LICENSE
+-rw-r--r--   0        0        0     1996 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/README.md
+-rw-r--r--   0        0        0     1179 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/__init__.py
+-rw-r--r--   0        0        0      507 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/csv_dumper.py
+-rw-r--r--   0        0        0     1418 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/delimited_file_dumper.py
+-rw-r--r--   0        0        0      973 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/dumper_root.py
+-rw-r--r--   0        0        0     4377 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/json_dumper.py
+-rw-r--r--   0        0        0     4023 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/rdf_dumper.py
+-rw-r--r--   0        0        0     7169 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/rdflib_dumper.py
+-rw-r--r--   0        0        0      177 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/tsv_dumper.py
+-rw-r--r--   0        0        0      901 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/dumpers/yaml_dumper.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/index/__init__.py
+-rw-r--r--   0        0        0     8875 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/index/object_index.py
+-rw-r--r--   0        0        0      119 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/README.md
+-rw-r--r--   0        0        0      738 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/__init__.py
+-rw-r--r--   0        0        0     3240 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/annotations.py
+-rw-r--r--   0        0        0     3333 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/extensions.py
+-rw-r--r--   0        0        0      114 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/graphql/README.md
+-rw-r--r--   0        0        0    30306 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/graphql/meta.graphql
+-rw-r--r--   0        0        0      111 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/README.md
+-rw-r--r--   0        0        0    11169 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/annotations.json
+-rw-r--r--   0        0        0     9306 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/extensions.json
+-rw-r--r--   0        0        0    12109 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/mappings.json
+-rw-r--r--   0        0        0   222072 2023-07-14 23:48:37.175908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/meta.json
+-rw-r--r--   0        0        0     6442 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/types.json
+-rw-r--r--   0        0        0    22401 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/units.json
+-rw-r--r--   0        0        0    14834 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/validation.json
+-rw-r--r--   0        0        0      113 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/README.md
+-rw-r--r--   0        0        0      648 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld
+-rw-r--r--   0        0        0      648 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld
+-rw-r--r--   0        0        0     7019 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/context.jsonld
+-rw-r--r--   0        0        0      587 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld
+-rw-r--r--   0        0        0      587 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld
+-rw-r--r--   0        0        0     1615 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld
+-rw-r--r--   0        0        0     1615 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld
+-rw-r--r--   0        0        0    13814 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/meta.context.jsonld
+-rw-r--r--   0        0        0    14266 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld
+-rw-r--r--   0        0        0      610 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/types.context.jsonld
+-rw-r--r--   0        0        0      610 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld
+-rw-r--r--   0        0        0     2065 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/units.context.jsonld
+-rw-r--r--   0        0        0     2065 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld
+-rw-r--r--   0        0        0     1910 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/validation.context.jsonld
+-rw-r--r--   0        0        0     1910 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld
+-rw-r--r--   0        0        0      117 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/README.md
+-rw-r--r--   0        0        0     4196 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/annotations.schema.json
+-rw-r--r--   0        0        0     1984 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/extensions.schema.json
+-rw-r--r--   0        0        0      297 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/mappings.schema.json
+-rw-r--r--   0        0        0   353208 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/meta.schema.json
+-rw-r--r--   0        0        0      291 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/types.schema.json
+-rw-r--r--   0        0        0     5621 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/units.schema.json
+-rw-r--r--   0        0        0     2291 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/validation.schema.json
+-rw-r--r--   0        0        0     7126 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/linkml_files.py
+-rw-r--r--   0        0        0     1821 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/mappings.py
+-rw-r--r--   0        0        0   249036 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/meta.py
+-rw-r--r--   0        0        0      112 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/README.md
+-rw-r--r--   0        0        0      118 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/docs/credits.md
+-rw-r--r--   0        0        0      141 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/docs/home.md
+-rw-r--r--   0        0        0        5 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/import_map.json
+-rw-r--r--   0        0        0      119 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/README.md
+-rw-r--r--   0        0        0      833 2023-07-14 23:48:37.179908 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/annotations.yaml
+-rw-r--r--   0        0        0     1057 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/extensions.yaml
+-rw-r--r--   0        0        0     2755 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/mappings.yaml
+-rw-r--r--   0        0        0    89120 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/meta.yaml
+-rw-r--r--   0        0        0     3880 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/types.yaml
+-rw-r--r--   0        0        0     2776 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/units.yaml
+-rw-r--r--   0        0        0     2953 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/validation.yaml
+-rw-r--r--   0        0        0      110 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/owl/README.md
+-rw-r--r--   0        0        0   192274 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/owl/meta.owl.ttl
+-rw-r--r--   0        0        0      110 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/README.md
+-rw-r--r--   0        0        0    13054 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/annotations.model.ttl
+-rw-r--r--   0        0        0    13054 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/annotations.ttl
+-rw-r--r--   0        0        0    10932 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/extensions.model.ttl
+-rw-r--r--   0        0        0    10932 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/extensions.ttl
+-rw-r--r--   0        0        0    13825 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/mappings.model.ttl
+-rw-r--r--   0        0        0    13825 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/mappings.ttl
+-rw-r--r--   0        0        0   207795 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/meta.model.ttl
+-rw-r--r--   0        0        0   207795 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/meta.ttl
+-rw-r--r--   0        0        0     7565 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/types.model.ttl
+-rw-r--r--   0        0        0     7565 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/types.ttl
+-rw-r--r--   0        0        0    25276 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/units.model.ttl
+-rw-r--r--   0        0        0    25276 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/units.ttl
+-rw-r--r--   0        0        0    16810 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/validation.model.ttl
+-rw-r--r--   0        0        0    16810 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/validation.ttl
+-rw-r--r--   0        0        0      113 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/README.md
+-rw-r--r--   0        0        0     1261 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/annotations.shex
+-rw-r--r--   0        0        0     8918 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/annotations.shexj
+-rw-r--r--   0        0        0      821 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/extensions.shex
+-rw-r--r--   0        0        0     5303 2023-07-14 23:48:37.183909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/extensions.shexj
+-rw-r--r--   0        0        0      424 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/mappings.shex
+-rw-r--r--   0        0        0     2568 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/mappings.shexj
+-rw-r--r--   0        0        0    37441 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/meta.shex
+-rw-r--r--   0        0        0   254576 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/meta.shexj
+-rw-r--r--   0        0        0      459 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/types.shex
+-rw-r--r--   0        0        0     2568 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/types.shexj
+-rw-r--r--   0        0        0     1682 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/units.shex
+-rw-r--r--   0        0        0    11643 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/units.shexj
+-rw-r--r--   0        0        0     1519 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/validation.shex
+-rw-r--r--   0        0        0     7343 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/validation.shexj
+-rw-r--r--   0        0        0     4599 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/types.py
+-rw-r--r--   0        0        0     3332 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/units.py
+-rw-r--r--   0        0        0     8885 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/linkml_model/validation.py
+-rw-r--r--   0        0        0      507 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/__init__.py
+-rw-r--r--   0        0        0     1533 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/context_flattener.py
+-rw-r--r--   0        0        0      179 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/csv_loader.py
+-rw-r--r--   0        0        0     2776 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/delimited_file_loader.py
+-rw-r--r--   0        0        0     1574 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/json_loader.py
+-rw-r--r--   0        0        0     6855 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/loader_root.py
+-rw-r--r--   0        0        0     4831 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/rdf_loader.py
+-rw-r--r--   0        0        0    14214 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/rdflib_loader.py
+-rw-r--r--   0        0        0     1358 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/requests_ssl_patch.py
+-rw-r--r--   0        0        0      180 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/tsv_loader.py
+-rw-r--r--   0        0        0     2223 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/loaders/yaml_loader.py
+-rw-r--r--   0        0        0    42276 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/processing/referencevalidator.py
+-rw-r--r--   0        0        0    26951 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/processing/validation_datamodel.py
+-rw-r--r--   0        0        0    10253 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/processing/validation_datamodel.yaml
+-rw-r--r--   0        0        0        0 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/__init__.py
+-rw-r--r--   0        0        0      850 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/comparefiles.py
+-rw-r--r--   0        0        0     1972 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/compile_python.py
+-rw-r--r--   0        0        0     4034 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/context_utils.py
+-rw-r--r--   0        0        0     2389 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/csvutils.py
+-rw-r--r--   0        0        0      486 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/curienamespace.py
+-rw-r--r--   0        0        0     1325 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/dataclass_extensions_376.py
+-rw-r--r--   0        0        0      433 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/dictutils.py
+-rw-r--r--   0        0        0     2554 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/distroutils.py
+-rw-r--r--   0        0        0     3683 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/enumerations.py
+-rw-r--r--   0        0        0     6755 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/eval_utils.py
+-rw-r--r--   0        0        0     6594 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/formatutils.py
+-rw-r--r--   0        0        0     5672 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/inference_utils.py
+-rw-r--r--   0        0        0     1976 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/introspection.py
+-rw-r--r--   0        0        0    11553 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/metamodelcore.py
+-rw-r--r--   0        0        0    10580 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/namespaces.py
+-rw-r--r--   0        0        0     2870 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/pattern.py
+-rw-r--r--   0        0        0     6697 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/permissiblevalueimpl.py
+-rw-r--r--   0        0        0     4720 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/ruleutils.py
+-rw-r--r--   0        0        0     2287 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/schema_as_dict.py
+-rw-r--r--   0        0        0     9312 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/schema_builder.py
+-rw-r--r--   0        0        0     2815 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/schemaops.py
+-rw-r--r--   0        0        0    66909 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/schemaview.py
+-rw-r--r--   0        0        0     4327 2023-07-14 23:48:37.187909 linkml_runtime-1.5.5/linkml_runtime/utils/schemaview_cli.py
+-rw-r--r--   0        0        0      368 2023-07-14 23:48:37.191909 linkml_runtime-1.5.5/linkml_runtime/utils/slot.py
+-rw-r--r--   0        0        0      641 2023-07-14 23:48:37.191909 linkml_runtime-1.5.5/linkml_runtime/utils/strictness.py
+-rw-r--r--   0        0        0     1405 2023-07-14 23:48:37.191909 linkml_runtime-1.5.5/linkml_runtime/utils/walker_utils.py
+-rw-r--r--   0        0        0    19743 2023-07-14 23:48:37.191909 linkml_runtime-1.5.5/linkml_runtime/utils/yamlutils.py
+-rw-r--r--   0        0        0     1848 2023-07-14 23:48:57.688663 linkml_runtime-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 linkml_runtime-1.5.5/PKG-INFO
```

### Comparing `linkml_runtime-1.5.4/LICENSE` & `linkml_runtime-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/README.md` & `linkml_runtime-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/__init__.py` & `linkml_runtime-1.5.5/linkml_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/dumpers/delimited_file_dumper.py` & `linkml_runtime-1.5.5/linkml_runtime/dumpers/delimited_file_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/dumpers/dumper_root.py` & `linkml_runtime-1.5.5/linkml_runtime/dumpers/dumper_root.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/dumpers/json_dumper.py` & `linkml_runtime-1.5.5/linkml_runtime/dumpers/json_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/dumpers/rdf_dumper.py` & `linkml_runtime-1.5.5/linkml_runtime/dumpers/rdf_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/dumpers/rdflib_dumper.py` & `linkml_runtime-1.5.5/linkml_runtime/dumpers/rdflib_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/dumpers/yaml_dumper.py` & `linkml_runtime-1.5.5/linkml_runtime/dumpers/yaml_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/index/object_index.py` & `linkml_runtime-1.5.5/linkml_runtime/index/object_index.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/__init__.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/annotations.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/annotations.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/extensions.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/extensions.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/graphql/meta.graphql` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/graphql/meta.graphql`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/annotations.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/annotations.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/extensions.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/extensions.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/mappings.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/mappings.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/meta.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/meta.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/types.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/types.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/units.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/units.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/validation.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/json/validation.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/meta.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/meta.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/types.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/types.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/units.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/units.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/validation.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/validation.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/annotations.schema.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/annotations.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/extensions.schema.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/extensions.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/meta.schema.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/meta.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/units.schema.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/units.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/validation.schema.json` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/jsonschema/validation.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/linkml_files.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/linkml_files.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/mappings.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/mappings.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/meta.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/meta.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/annotations.yaml` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/annotations.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/extensions.yaml` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/extensions.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/mappings.yaml` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/mappings.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/meta.yaml` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/meta.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/types.yaml` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/types.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/units.yaml` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/units.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/validation.yaml` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/model/schema/validation.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/owl/meta.owl.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/owl/meta.owl.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/annotations.model.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/annotations.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/annotations.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/annotations.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/extensions.model.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/extensions.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/extensions.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/extensions.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/mappings.model.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/mappings.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/mappings.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/mappings.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/meta.model.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/meta.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/meta.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/meta.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/types.model.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/types.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/types.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/types.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/units.model.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/units.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/units.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/units.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/validation.model.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/validation.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/validation.ttl` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/rdf/validation.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/annotations.shex` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/annotations.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/annotations.shexj` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/annotations.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/extensions.shex` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/extensions.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/extensions.shexj` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/extensions.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/mappings.shexj` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/mappings.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/meta.shex` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/meta.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/meta.shexj` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/meta.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/types.shexj` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/types.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/units.shex` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/units.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/units.shexj` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/units.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/validation.shex` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/validation.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/validation.shexj` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/shex/validation.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/types.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/types.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/units.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/units.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/linkml_model/validation.py` & `linkml_runtime-1.5.5/linkml_runtime/linkml_model/validation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Auto generated from validation.yaml by pythongen.py version: 0.9.0
-# Generation date: 2022-05-19T21:54:12
+# Generation date: 2023-06-29T10:29:33
 # Schema: reporting
 #
 # id: https://w3id.org/linkml/reporting
-# description: A datamodel for reports on data
+# description: A datamodel for reports on data, based on SHACL
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
-import sys
 import re
 from jsonasobj2 import JsonObj, as_dict
 from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
+from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions
 
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
 from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
 from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
-from .types import Nodeidentifier, String
+from linkml_runtime.linkml_model.types import Nodeidentifier, String
 from linkml_runtime.utils.metamodelcore import NodeIdentifier
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
@@ -87,15 +87,15 @@
     type: Optional[Union[str, NodeIdentifier]] = None
     severity: Optional[Union[str, "SeverityOptions"]] = None
     subject: Optional[Union[str, NodeIdentifier]] = None
     instantiates: Optional[Union[str, NodeIdentifier]] = None
     predicate: Optional[Union[str, NodeIdentifier]] = None
     object: Optional[Union[str, NodeIdentifier]] = None
     object_str: Optional[str] = None
-    source: Optional[Union[str, NodeIdentifier]] = None
+    node_source: Optional[Union[str, NodeIdentifier]] = None
     info: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.type is not None and not isinstance(self.type, NodeIdentifier):
             self.type = NodeIdentifier(self.type)
 
         if self.severity is not None and not isinstance(self.severity, SeverityOptions):
@@ -112,52 +112,92 @@
 
         if self.object is not None and not isinstance(self.object, NodeIdentifier):
             self.object = NodeIdentifier(self.object)
 
         if self.object_str is not None and not isinstance(self.object_str, str):
             self.object_str = str(self.object_str)
 
-        if self.source is not None and not isinstance(self.source, NodeIdentifier):
-            self.source = NodeIdentifier(self.source)
+        if self.node_source is not None and not isinstance(self.node_source, NodeIdentifier):
+            self.node_source = NodeIdentifier(self.node_source)
 
         if self.info is not None and not isinstance(self.info, str):
             self.info = str(self.info)
 
         super().__post_init__(**kwargs)
 
 
 # Enumerations
 class ProblemType(EnumDefinitionImpl):
 
-    undeclared_slot = PermissibleValue(text="undeclared_slot",
-                                                     description="Applies when a slot is used in data but the slot is undeclared in the datamodel")
-    inapplicable_slot = PermissibleValue(text="inapplicable_slot",
-                                                         description="Applies when a slot is used in an instance of a class where the slot is not applicable for that class")
-    missing_slot_value = PermissibleValue(text="missing_slot_value",
-                                                           description="Applies when an instance of a class has a required slot which is not filled in")
-    slot_range_violation = PermissibleValue(text="slot_range_violation",
-                                                               description="Applies when the value of a slot is inconsistent with the declared range")
-    max_count_violation = PermissibleValue(text="max_count_violation",
-                                                             meaning=SH.MaxCountConstraintComponent)
-    parsing_error = PermissibleValue(text="parsing_error",
-                                                 description="The data could not be parsed")
+    undeclared_slot = PermissibleValue(
+        text="undeclared_slot",
+        description="Applies when a slot is used in data but the slot is undeclared in the datamodel")
+    inapplicable_slot = PermissibleValue(
+        text="inapplicable_slot",
+        description="""Applies when a slot is used in an instance of a class where the slot is not applicable for that class""")
+    missing_slot_value = PermissibleValue(
+        text="missing_slot_value",
+        description="Applies when an instance of a class has a required slot which is not filled in")
+    slot_range_violation = PermissibleValue(
+        text="slot_range_violation",
+        description="Applies when the value of a slot is inconsistent with the declared range")
+    max_count_violation = PermissibleValue(
+        text="max_count_violation",
+        meaning=SH.MaxCountConstraintComponent)
+    parsing_error = PermissibleValue(
+        text="parsing_error",
+        description="The data could not be parsed")
 
     _defn = EnumDefinition(
         name="ProblemType",
     )
 
 class SeverityOptions(EnumDefinitionImpl):
 
     FATAL = PermissibleValue(text="FATAL")
-    ERROR = PermissibleValue(text="ERROR",
-                                 meaning=SH.Violation)
-    WARNING = PermissibleValue(text="WARNING",
-                                     meaning=SH.Warning)
-    INFO = PermissibleValue(text="INFO",
-                               meaning=SH.Info)
+    ERROR = PermissibleValue(
+        text="ERROR",
+        meaning=SH.Violation)
+    WARNING = PermissibleValue(
+        text="WARNING",
+        meaning=SH.Warning)
+    INFO = PermissibleValue(
+        text="INFO",
+        meaning=SH.Info)
 
     _defn = EnumDefinition(
         name="SeverityOptions",
     )
 
 # Slots
+class slots:
+    pass
 
+slots.type = Slot(uri=SH.sourceConstraintComponent, name="type", curie=SH.curie('sourceConstraintComponent'),
+                   model_uri=REPORTING.type, domain=None, range=Optional[Union[str, NodeIdentifier]])
+
+slots.subject = Slot(uri=SH.focusNode, name="subject", curie=SH.curie('focusNode'),
+                   model_uri=REPORTING.subject, domain=None, range=Optional[Union[str, NodeIdentifier]])
+
+slots.instantiates = Slot(uri=REPORTING.instantiates, name="instantiates", curie=REPORTING.curie('instantiates'),
+                   model_uri=REPORTING.instantiates, domain=None, range=Optional[Union[str, NodeIdentifier]])
+
+slots.predicate = Slot(uri=REPORTING.predicate, name="predicate", curie=REPORTING.curie('predicate'),
+                   model_uri=REPORTING.predicate, domain=None, range=Optional[Union[str, NodeIdentifier]])
+
+slots.object = Slot(uri=SH.value, name="object", curie=SH.curie('value'),
+                   model_uri=REPORTING.object, domain=None, range=Optional[Union[str, NodeIdentifier]])
+
+slots.object_str = Slot(uri=REPORTING.object_str, name="object_str", curie=REPORTING.curie('object_str'),
+                   model_uri=REPORTING.object_str, domain=None, range=Optional[str])
+
+slots.node_source = Slot(uri=REPORTING.node_source, name="node_source", curie=REPORTING.curie('node_source'),
+                   model_uri=REPORTING.node_source, domain=None, range=Optional[Union[str, NodeIdentifier]])
+
+slots.severity = Slot(uri=REPORTING.severity, name="severity", curie=REPORTING.curie('severity'),
+                   model_uri=REPORTING.severity, domain=None, range=Optional[Union[str, "SeverityOptions"]])
+
+slots.info = Slot(uri=REPORTING.info, name="info", curie=REPORTING.curie('info'),
+                   model_uri=REPORTING.info, domain=None, range=Optional[str])
+
+slots.validationReport__results = Slot(uri=REPORTING.results, name="validationReport__results", curie=REPORTING.curie('results'),
+                   model_uri=REPORTING.validationReport__results, domain=None, range=Optional[Union[Union[dict, ValidationResult], List[Union[dict, ValidationResult]]]])
```

### Comparing `linkml_runtime-1.5.4/linkml_runtime/loaders/context_flattener.py` & `linkml_runtime-1.5.5/linkml_runtime/loaders/context_flattener.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/loaders/delimited_file_loader.py` & `linkml_runtime-1.5.5/linkml_runtime/loaders/delimited_file_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/loaders/json_loader.py` & `linkml_runtime-1.5.5/linkml_runtime/loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/loaders/loader_root.py` & `linkml_runtime-1.5.5/linkml_runtime/loaders/loader_root.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/loaders/rdf_loader.py` & `linkml_runtime-1.5.5/linkml_runtime/loaders/rdf_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/loaders/rdflib_loader.py` & `linkml_runtime-1.5.5/linkml_runtime/loaders/rdflib_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/loaders/requests_ssl_patch.py` & `linkml_runtime-1.5.5/linkml_runtime/loaders/requests_ssl_patch.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/loaders/yaml_loader.py` & `linkml_runtime-1.5.5/linkml_runtime/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/processing/referencevalidator.py` & `linkml_runtime-1.5.5/linkml_runtime/processing/referencevalidator.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/processing/validation_datamodel.py` & `linkml_runtime-1.5.5/linkml_runtime/processing/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/processing/validation_datamodel.yaml` & `linkml_runtime-1.5.5/linkml_runtime/processing/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/comparefiles.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/comparefiles.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/compile_python.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/compile_python.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/context_utils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/context_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/csvutils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/csvutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/dataclass_extensions_376.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/dataclass_extensions_376.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/distroutils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/distroutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/enumerations.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/enumerations.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/eval_utils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/formatutils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/formatutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/inference_utils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/introspection.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/metamodelcore.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/metamodelcore.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/namespaces.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/pattern.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/pattern.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/permissiblevalueimpl.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/permissiblevalueimpl.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/ruleutils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/ruleutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/schema_as_dict.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/schema_as_dict.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/schema_builder.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/schemaops.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/schemaops.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/schemaview.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/schemaview.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,22 +127,22 @@
     schema_map: Dict[SchemaDefinitionName, SchemaDefinition] = None
     importmap: Optional[Mapping[str, str]] = None
     """Optional mapping between schema names and local paths/URLs"""
     modifications: int = 0
     uuid: str = None
 
     def __init__(self, schema: Union[str, Path, SchemaDefinition],
-                 importmap: Optional[Mapping[str, str]] = None, merge_imports: bool = False):
+                 importmap: Optional[Dict[str, str]] = None, merge_imports: bool = False, base_dir: str = None):
         if isinstance(schema, Path):
             schema = str(schema)
         if isinstance(schema, str):
             schema = load_schema_wrap(schema)
         self.schema = schema
         self.schema_map = {schema.name: schema}
-        self.importmap = parse_import_map(importmap, self.base_dir) if self.importmap is not None else dict()
+        self.importmap = parse_import_map(importmap, base_dir) if importmap is not None else dict()
         if merge_imports:
             self.merge_imports()
         self.uuid = str(uuid.uuid4())
 
     def __key(self):
         return self.schema.id, self.uuid, self.modifications
```

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/schemaview_cli.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/schemaview_cli.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/strictness.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/strictness.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/walker_utils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/walker_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/linkml_runtime/utils/yamlutils.py` & `linkml_runtime-1.5.5/linkml_runtime/utils/yamlutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.4/pyproject.toml` & `linkml_runtime-1.5.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml-runtime"
-version = "v1.5.4"
+version = "v1.5.5"
 description = "Runtime environment for LinkML, the Linked open data modeling language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sierra Moxon <smoxon@lbl.gov>",
     "Bill Duncan <wdduncan@gmail.com>",
     "Harshad Hegde <hhegde@lbl.gov>"
```

### Comparing `linkml_runtime-1.5.4/PKG-INFO` & `linkml_runtime-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-runtime
-Version: 1.5.4
+Version: 1.5.5
 Summary: Runtime environment for LinkML, the Linked open data modeling language
 Home-page: https://github.com/linkml/linkml-runtime
 Keywords: linkml,metamodel,schema visualization,rdf,owl,yaml
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

