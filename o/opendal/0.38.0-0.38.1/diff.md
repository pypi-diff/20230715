# Comparing `tmp/opendal-0.38.0.tar.gz` & `tmp/opendal-0.38.1.tar.gz`

## Comparing `opendal-0.38.0.tar` & `opendal-0.38.1.tar`

### file list

```diff
@@ -1,340 +1,340 @@
--rw-r--r--   0        0        0     6825 1970-01-01 00:00:00.000000 opendal-0.38.0/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    89540 2023-06-27 15:43:19.000000 opendal-0.38.0/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1114 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6290 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5554 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2987 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1290 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7682 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     6142 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123     1040 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10880 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     3172 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
--rw-r--r--   0     1001      123     2687 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
--rw-r--r--   0     1001      123     2576 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md
--rw-r--r--   0     1001      123     4658 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    26469 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6622 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    32922 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9949 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    17725 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    14214 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    53997 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    13488 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    30012 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    12657 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2376 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    13222 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/oteltrace.rs
--rw-r--r--   0     1001      123    23560 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    38577 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    11611 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/throttle.rs
--rw-r--r--   0     1001      123    14179 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/timeout.rs
--rw-r--r--   0     1001      123    12198 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3644 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3571 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    18865 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5049 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123    12928 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1020 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1566 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     5407 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
--rw-r--r--   0     1001      123    12938 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
--rw-r--r--   0     1001      123     1067 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
--rw-r--r--   0     1001      123     1934 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     5928 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5735 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3415 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    11165 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2159 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123    35575 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/multipart.rs
--rw-r--r--   0     1001      123     2962 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11712 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1976 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     3018 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/append.rs
--rw-r--r--   0     1001      123     9434 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15408 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4150 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     2842 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_reader.rs
--rw-r--r--   0     1001      123     1473 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_stream.rs
--rw-r--r--   0     1001      123     1070 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/mod.rs
--rw-r--r--   0     1001      123     4579 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     2181 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10670 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     2132 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/stream.rs
--rw-r--r--   0     1001      123     9158 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6894 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5739 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     3953 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    12115 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/ops.rs
--rw-r--r--   0     1001      123    11671 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6507 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123     4514 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/appender.rs
--rw-r--r--   0     1001      123    31973 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123     5544 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123    16987 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     2304 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/docs.md
--rw-r--r--   0     1001      123     5870 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      927 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2252 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    14348 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123    10123 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     1960 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/docs.md
--rw-r--r--   0     1001      123     3519 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2909 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     4216 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cacache/backend.rs
--rw-r--r--   0     1001      123      657 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cacache/docs.md
--rw-r--r--   0     1001      123      860 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cacache/mod.rs
--rw-r--r--   0     1001      123     5727 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/appender.rs
--rw-r--r--   0     1001      123    13653 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/backend.rs
--rw-r--r--   0     1001      123     9184 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/core.rs
--rw-r--r--   0     1001      123     1314 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/docs.md
--rw-r--r--   0     1001      123     3492 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/error.rs
--rw-r--r--   0     1001      123      910 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/mod.rs
--rw-r--r--   0     1001      123     5963 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/pager.rs
--rw-r--r--   0     1001      123     2230 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/cos/writer.rs
--rw-r--r--   0     1001      123     3972 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      186 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/docs.md
--rw-r--r--   0     1001      123      859 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123     2935 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/backend.rs
--rw-r--r--   0     1001      123     4144 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/builder.rs
--rw-r--r--   0     1001      123     4854 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/core.rs
--rw-r--r--   0     1001      123     2573 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/error.rs
--rw-r--r--   0     1001      123      906 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/mod.rs
--rw-r--r--   0     1001      123     2160 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/writer.rs
--rw-r--r--   0     1001      123     1409 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/appender.rs
--rw-r--r--   0     1001      123    23158 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123      869 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/docs.md
--rw-r--r--   0     1001      123     1424 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      898 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3290 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    15921 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123      737 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/docs.md
--rw-r--r--   0     1001      123     1808 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4208 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     2098 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    23912 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    17063 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3512 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10592 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     6513 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123     3361 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/backend.rs
--rw-r--r--   0     1001      123     4276 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/builder.rs
--rw-r--r--   0     1001      123     7046 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/core.rs
--rw-r--r--   0     1001      123     1743 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/error.rs
--rw-r--r--   0     1001      123      904 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/mod.rs
--rw-r--r--   0     1001      123     2154 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/writer.rs
--rw-r--r--   0     1001      123    20868 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2573 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    13208 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     2419 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/docs.md
--rw-r--r--   0     1001      123     1497 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     2659 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    16276 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1875 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    15931 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123      867 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/docs.md
--rw-r--r--   0     1001      123     1871 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     9056 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123      186 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/docs.md
--rw-r--r--   0     1001      123     2790 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1951 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     5712 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9177 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4405 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      511 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memory/docs.md
--rw-r--r--   0     1001      123      857 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     6599 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/mini_moka/backend.rs
--rw-r--r--   0     1001      123      861 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/mini_moka/mod.rs
--rw-r--r--   0     1001      123     4625 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     8174 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123     4710 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/appender.rs
--rw-r--r--   0     1001      123    15624 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     9417 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3492 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      910 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2230 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    12480 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/backend.rs
--rw-r--r--   0     1001      123     4177 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/builder.rs
--rw-r--r--   0     1001      123     1743 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/error.rs
--rw-r--r--   0     1001      123     9228 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs
--rw-r--r--   0     1001      123      926 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/mod.rs
--rw-r--r--   0     1001      123     4874 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/pager.rs
--rw-r--r--   0     1001      123     6426 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/writer.rs
--rw-r--r--   0     1001      123     4869 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/appender.rs
--rw-r--r--   0     1001      123    21977 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    25318 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     1842 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/docs.md
--rw-r--r--   0     1001      123     3407 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      910 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     6849 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123     6613 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redb/backend.rs
--rw-r--r--   0     1001      123      677 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redb/docs.md
--rw-r--r--   0     1001      123      854 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redb/mod.rs
--rw-r--r--   0     1001      123     9658 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      856 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redis/docs.md
--rw-r--r--   0     1001      123      855 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     4241 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123     1263 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/docs.md
--rw-r--r--   0     1001      123      859 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    36080 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     4183 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    28667 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     7050 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/docs.md
--rw-r--r--   0     1001      123     4805 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7387 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     7720 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123    16132 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/backend.rs
--rw-r--r--   0     1001      123     1076 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/docs.md
--rw-r--r--   0     1001      123     2587 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/error.rs
--rw-r--r--   0     1001      123      899 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/mod.rs
--rw-r--r--   0     1001      123     2420 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/pager.rs
--rw-r--r--   0     1001      123     3641 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/utils.rs
--rw-r--r--   0     1001      123     1958 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sftp/writer.rs
--rw-r--r--   0     1001      123     5813 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      642 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sled/docs.md
--rw-r--r--   0     1001      123      854 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123     9779 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/backend.rs
--rw-r--r--   0     1001      123     8021 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/core.rs
--rw-r--r--   0     1001      123     2952 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/error.rs
--rw-r--r--   0     1001      123      894 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/mod.rs
--rw-r--r--   0     1001      123     2555 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/supabase/writer.rs
--rw-r--r--   0     1001      123     4551 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
--rw-r--r--   0     1001      123     3636 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
--rw-r--r--   0     1001      123     1743 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
--rw-r--r--   0     1001      123      912 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
--rw-r--r--   0     1001      123     2228 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
--rw-r--r--   0     1001      123    39653 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29752 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     4779 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2223 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    20966 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      990 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2560 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2239 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19002 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     1864 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/docs.md
--rw-r--r--   0     1001      123     4224 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     7373 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     4859 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2249 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     8596 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/appender.rs
--rw-r--r--   0     1001      123     2649 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     6975 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/capability.rs
--rw-r--r--   0     1001      123     2494 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    12002 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     7417 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    16556 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1614 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    26806 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123    13888 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3073 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1153 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    49498 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123     2863 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator_functions.rs
--rw-r--r--   0     1001      123    17237 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator_futures.rs
--rw-r--r--   0     1001      123     9547 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     7375 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123    13822 2023-06-27 15:43:20.000000 opendal-0.38.0/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 opendal-0.38.0/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-06-27 15:43:20.000000 opendal-0.38.0/.gitignore
--rw-r--r--   0     1001      123     2213 2023-06-27 15:43:20.000000 opendal-0.38.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1084 2023-06-27 15:43:20.000000 opendal-0.38.0/README.md
--rw-r--r--   0     1001      123      765 2023-06-27 15:43:20.000000 opendal-0.38.0/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-06-27 15:43:20.000000 opendal-0.38.0/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-06-27 15:43:20.000000 opendal-0.38.0/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123      917 2023-06-27 15:43:20.000000 opendal-0.38.0/examples/object.ipynb
--rw-r--r--   0     1001      123     1660 2023-06-27 15:43:20.000000 opendal-0.38.0/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-06-27 15:43:20.000000 opendal-0.38.0/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-06-27 15:43:20.000000 opendal-0.38.0/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123      405 2023-06-27 15:43:20.000000 opendal-0.38.0/python/opendal/layers.pyi
--rw-r--r--   0     1001      123    11963 2023-06-27 15:43:20.000000 opendal-0.38.0/src/asyncio.rs
--rw-r--r--   0     1001      123     3074 2023-06-27 15:43:20.000000 opendal-0.38.0/src/layers.rs
--rw-r--r--   0     1001      123    12218 2023-06-27 15:43:20.000000 opendal-0.38.0/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-06-27 15:43:20.000000 opendal-0.38.0/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-06-27 15:43:20.000000 opendal-0.38.0/tests/steps/binding.py
--rw-r--r--   0     1001      123   138739 2023-06-27 15:43:19.000000 opendal-0.38.0/Cargo.lock
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 opendal-0.38.0/PKG-INFO
+-rw-r--r--   0        0        0     6878 1970-01-01 00:00:00.000000 opendal-0.38.1/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    95565 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1114 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6290 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5554 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2987 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1290 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     6142 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123     1040 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10880 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     3172 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
+-rw-r--r--   0     1001      123     2687 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
+-rw-r--r--   0     1001      123     2576 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md
+-rw-r--r--   0     1001      123     6055 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2602_object_versioning.md
+-rw-r--r--   0     1001      123     4748 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    26469 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6622 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    32922 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9949 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17725 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    14214 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    53997 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13488 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    30012 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    14264 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2376 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13222 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    23560 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    38577 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    11611 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/throttle.rs
+-rw-r--r--   0     1001      123    14179 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/timeout.rs
+-rw-r--r--   0     1001      123    12198 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3644 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3571 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    18865 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123    12928 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1020 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1566 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     5407 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
+-rw-r--r--   0     1001      123    12938 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
+-rw-r--r--   0     1001      123     1067 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     5941 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5735 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3415 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    11165 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2159 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123    35575 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/multipart.rs
+-rw-r--r--   0     1001      123     2962 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11712 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1976 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     3018 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/append.rs
+-rw-r--r--   0     1001      123     9438 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3670 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15410 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4154 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     2842 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_reader.rs
+-rw-r--r--   0     1001      123     1473 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_stream.rs
+-rw-r--r--   0     1001      123     1070 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/mod.rs
+-rw-r--r--   0     1001      123     4579 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     2181 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10637 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     2132 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/stream.rs
+-rw-r--r--   0     1001      123     9158 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6894 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5739 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     3953 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    13103 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/ops.rs
+-rw-r--r--   0     1001      123    11651 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6507 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123     4514 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/appender.rs
+-rw-r--r--   0     1001      123    32011 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123     5544 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    16985 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     2304 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/docs.md
+-rw-r--r--   0     1001      123     5870 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      927 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2346 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    14348 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123    10123 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     1960 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/docs.md
+-rw-r--r--   0     1001      123     3519 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2909 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     4216 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cacache/backend.rs
+-rw-r--r--   0     1001      123      657 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cacache/docs.md
+-rw-r--r--   0     1001      123      860 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cacache/mod.rs
+-rw-r--r--   0     1001      123     5727 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/appender.rs
+-rw-r--r--   0     1001      123    13691 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/backend.rs
+-rw-r--r--   0     1001      123     9182 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/core.rs
+-rw-r--r--   0     1001      123     1314 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/docs.md
+-rw-r--r--   0     1001      123     3492 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/error.rs
+-rw-r--r--   0     1001      123      910 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/mod.rs
+-rw-r--r--   0     1001      123     5963 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/pager.rs
+-rw-r--r--   0     1001      123     2324 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/cos/writer.rs
+-rw-r--r--   0     1001      123     3972 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      186 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/docs.md
+-rw-r--r--   0     1001      123      859 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    10414 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/backend.rs
+-rw-r--r--   0     1001      123     8274 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/builder.rs
+-rw-r--r--   0     1001      123    14868 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/core.rs
+-rw-r--r--   0     1001      123     3219 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/error.rs
+-rw-r--r--   0     1001      123      906 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/mod.rs
+-rw-r--r--   0     1001      123     2160 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/writer.rs
+-rw-r--r--   0     1001      123     1409 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/appender.rs
+-rw-r--r--   0     1001      123    23196 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123      869 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/docs.md
+-rw-r--r--   0     1001      123     1424 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      898 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3541 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    15921 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123      737 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/docs.md
+-rw-r--r--   0     1001      123     1808 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4208 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     2098 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    23950 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    17061 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3512 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10592 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6539 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123     3361 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/backend.rs
+-rw-r--r--   0     1001      123     4276 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/builder.rs
+-rw-r--r--   0     1001      123     7046 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/core.rs
+-rw-r--r--   0     1001      123     1743 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/error.rs
+-rw-r--r--   0     1001      123      904 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/mod.rs
+-rw-r--r--   0     1001      123     2154 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/writer.rs
+-rw-r--r--   0     1001      123    20868 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2573 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    13208 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     3048 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/docs.md
+-rw-r--r--   0     1001      123     1497 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2659 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    16276 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1875 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    15931 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123      867 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/docs.md
+-rw-r--r--   0     1001      123     1871 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     9056 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123      186 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/docs.md
+-rw-r--r--   0     1001      123     2790 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1951 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     5712 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9058 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4405 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      511 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memory/docs.md
+-rw-r--r--   0     1001      123      857 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     6599 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/mini_moka/backend.rs
+-rw-r--r--   0     1001      123      861 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/mini_moka/mod.rs
+-rw-r--r--   0     1001      123     4625 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     8174 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123     4710 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/appender.rs
+-rw-r--r--   0     1001      123    15662 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     9415 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3492 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      910 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2324 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    12480 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/backend.rs
+-rw-r--r--   0     1001      123     4177 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/error.rs
+-rw-r--r--   0     1001      123     9228 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/graph_model.rs
+-rw-r--r--   0     1001      123      926 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/mod.rs
+-rw-r--r--   0     1001      123     4874 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/pager.rs
+-rw-r--r--   0     1001      123     6426 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/writer.rs
+-rw-r--r--   0     1001      123     4869 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/appender.rs
+-rw-r--r--   0     1001      123    22015 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    25314 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     1842 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/docs.md
+-rw-r--r--   0     1001      123     3407 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      910 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     6875 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123     6613 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redb/backend.rs
+-rw-r--r--   0     1001      123      677 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redb/docs.md
+-rw-r--r--   0     1001      123      854 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redb/mod.rs
+-rw-r--r--   0     1001      123     9658 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      856 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redis/docs.md
+-rw-r--r--   0     1001      123      855 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     4241 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123     1263 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/docs.md
+-rw-r--r--   0     1001      123      859 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    41263 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     4183 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28667 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     7050 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/docs.md
+-rw-r--r--   0     1001      123     4805 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7387 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     7720 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123    16132 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/backend.rs
+-rw-r--r--   0     1001      123     1076 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/docs.md
+-rw-r--r--   0     1001      123     2587 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/error.rs
+-rw-r--r--   0     1001      123      899 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/mod.rs
+-rw-r--r--   0     1001      123     2420 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/pager.rs
+-rw-r--r--   0     1001      123     3641 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/utils.rs
+-rw-r--r--   0     1001      123     1958 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sftp/writer.rs
+-rw-r--r--   0     1001      123     5813 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      642 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sled/docs.md
+-rw-r--r--   0     1001      123      854 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123     9779 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/backend.rs
+-rw-r--r--   0     1001      123     8021 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/core.rs
+-rw-r--r--   0     1001      123     2952 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/error.rs
+-rw-r--r--   0     1001      123      894 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/mod.rs
+-rw-r--r--   0     1001      123     2555 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/supabase/writer.rs
+-rw-r--r--   0     1001      123     4551 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
+-rw-r--r--   0     1001      123     3636 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
+-rw-r--r--   0     1001      123      912 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
+-rw-r--r--   0     1001      123     2228 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
+-rw-r--r--   0     1001      123    39653 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29752 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     4779 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2223 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    21005 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1851 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      990 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      892 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123    18302 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2337 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19002 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     1864 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/docs.md
+-rw-r--r--   0     1001      123     4224 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     7373 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     4859 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2249 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     8596 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/appender.rs
+-rw-r--r--   0     1001      123     2649 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     6975 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    12174 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     7417 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    17930 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1614 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    27602 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123    13888 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3073 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1153 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    50360 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123     3428 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator_functions.rs
+-rw-r--r--   0     1001      123    18181 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator_futures.rs
+-rw-r--r--   0     1001      123     9547 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     7375 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    13822 2023-07-15 04:02:43.000000 opendal-0.38.1/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 opendal-0.38.1/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-07-15 04:02:43.000000 opendal-0.38.1/.gitignore
+-rw-r--r--   0     1001      123     2213 2023-07-15 04:02:43.000000 opendal-0.38.1/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1084 2023-07-15 04:02:43.000000 opendal-0.38.1/README.md
+-rw-r--r--   0     1001      123      765 2023-07-15 04:02:43.000000 opendal-0.38.1/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-07-15 04:02:43.000000 opendal-0.38.1/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-07-15 04:02:43.000000 opendal-0.38.1/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-07-15 04:02:43.000000 opendal-0.38.1/examples/object.ipynb
+-rw-r--r--   0     1001      123     1660 2023-07-15 04:02:43.000000 opendal-0.38.1/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-07-15 04:02:43.000000 opendal-0.38.1/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-07-15 04:02:43.000000 opendal-0.38.1/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123      405 2023-07-15 04:02:43.000000 opendal-0.38.1/python/opendal/layers.pyi
+-rw-r--r--   0     1001      123    11963 2023-07-15 04:02:43.000000 opendal-0.38.1/src/asyncio.rs
+-rw-r--r--   0     1001      123     3074 2023-07-15 04:02:43.000000 opendal-0.38.1/src/layers.rs
+-rw-r--r--   0     1001      123    12218 2023-07-15 04:02:43.000000 opendal-0.38.1/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-07-15 04:02:43.000000 opendal-0.38.1/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-07-15 04:02:43.000000 opendal-0.38.1/tests/steps/binding.py
+-rw-r--r--   0     1001      123   140798 2023-07-15 04:02:43.000000 opendal-0.38.1/Cargo.lock
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 opendal-0.38.1/PKG-INFO
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/Cargo.toml` & `opendal-0.38.1/local_dependencies/opendal/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.38.0"
+version= "0.38.1"
+resolver = "2"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
@@ -137,14 +138,15 @@
 ]
 services-onedrive = []
 services-oss = [
   "dep:reqsign",
   "reqsign?/services-aliyun",
   "reqsign?/reqwest_request",
 ]
+services-redb = ["dep:redb"]
 services-redis = ["dep:redis"]
 services-rocksdb = ["dep:rocksdb"]
 services-s3 = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
@@ -155,53 +157,56 @@
 services-wasabi = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
 services-webdav = []
 services-webhdfs = []
-services-redb = ["dep:redb"]
 
 [lib]
 bench = false
 
 [[bench]]
 harness = false
 name = "ops"
 
 [[test]]
 harness = false
 name = "behavior"
+path = "tests/behavior/main.rs"
 
 [dependencies]
 anyhow = { version = "1.0.30", features = ["std"] }
 async-compat = "0.2"
 async-tls = { version = "0.11", optional = true }
 async-trait = "0.1.68"
 backon = "0.4.0"
 base64 = "0.21"
 bb8 = { version = "0.8", optional = true }
 bytes = "1.2"
-cacache =  { version = "11.6", default-features = false, features = ["tokio-runtime", "mmap"], optional = true }
-chrono = "0.4.24"
+cacache = { version = "11.6", default-features = false, features = [
+  "tokio-runtime",
+  "mmap",
+], optional = true }
+chrono = "0.4.26"
 dashmap = { version = "5.4", optional = true }
 dirs = { version = "5.0.1", optional = true }
 flagset = "0.4"
 futures = { version = "0.3", default-features = false, features = ["std"] }
 governor = { version = "0.5", optional = true, features = ["std"] }
 hdrs = { version = "0.2", optional = true, features = ["async_file"] }
 http = "0.2.5"
 hyper = "0.14"
 lazy-regex = { version = "2.5.0", optional = true }
 log = "0.4"
 madsim = { version = "0.2.21", optional = true }
 md-5 = "0.10"
 metrics = { version = "0.20", optional = true }
-minitrace = { version = "0.4.0", optional = true }
 mini-moka = { version = "0.10", optional = true }
+minitrace = { version = "0.4.1", optional = true }
 moka = { version = "0.10", optional = true, features = ["future"] }
 once_cell = "1"
 openssh = { version = "0.9.9", optional = true }
 openssh-sftp-client = { version = "0.13.5", optional = true, features = [
   "openssh",
   "tracing",
 ] }
@@ -209,28 +214,28 @@
 parking_lot = "0.12"
 percent-encoding = "2"
 pin-project = "1"
 prometheus = { version = "0.13", features = ["process"], optional = true }
 prost = { version = "0.11", optional = true }
 quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
-redis = { version = "0.22", features = [
+redb = { version = "1.0.0", optional = true }
+redis = { version = "0.23", features = [
   "tokio-comp",
   "connection-manager",
 ], optional = true }
 reqsign = { version = "0.13.0", default-features = false, optional = true }
 reqwest = { version = "0.11.18", features = [
   "stream",
 ], default-features = false }
 rocksdb = { version = "0.21.0", default-features = false, optional = true }
 serde = { version = "1", features = ["derive"] }
 serde_json = "1"
 sha2 = { version = "0.10", optional = true }
 sled = { version = "0.34.7", optional = true }
-redb = { version = "1.0.0", optional = true }
 suppaftp = { version = "4.5", default-features = false, features = [
   "async-secure",
   "async-rustls",
 ], optional = true }
 tokio = "1.27"
 tracing = { version = "0.1", optional = true }
 uuid = { version = "1", features = ["serde", "v4"] }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.38.1/local_dependencies/opendal/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,147 +1,243 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.38.1] - 2023-07-14
+
+### Added
+
+- feat(binding/lua): add rename and create_dir operator function by @oowl in https://github.com/apache/incubator-opendal/pull/2564
+- feat(services/azblob): support sink by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2574
+- feat(services/gcs): support sink by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2576
+- feat(services/oss): support sink by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2577
+- feat(services/obs): support sink by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2578
+- feat(services/cos): impl sink by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2587
+- feat(service): Support stat for Dropbox by @Zheaoli in https://github.com/apache/incubator-opendal/pull/2588
+- feat(services/dropbox): impl create_dir and polish error handling by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2600
+- feat(services/dropbox): Implement refresh token support by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2604
+- feat(service/dropbox): impl batch delete by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2606
+- feat(CI): set Kvrocks test for service redis by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2613
+- feat(core): object versioning APIs by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2614
+- feat(oay): actually read configuration from `oay.toml` by @messense in https://github.com/apache/incubator-opendal/pull/2615
+- feat(services/webdav): impl sink by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2622
+- feat(services/fs): impl Sink for Fs by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2626
+- feat(core): impl `delete_with` on blocking operator by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2633
+- feat(bindings/C): add support for list in C binding by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2448
+- feat(services/s3): Add detect_region support for S3Builder by @parkma99 in https://github.com/apache/incubator-opendal/pull/2634
+
+### Changed
+
+- refactor(core): Add ErrorKind InvalidInput to indicate users input error by @dqhl76 in https://github.com/apache/incubator-opendal/pull/2637
+- refactor(services/s3): Add more detect logic for detect_region by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2645
+
+### Fixed
+
+- fix(doc): fix codeblock rendering by @xxchan in https://github.com/apache/incubator-opendal/pull/2592
+- fix(service/minitrace): should set local parent by @andylokandy in https://github.com/apache/incubator-opendal/pull/2620
+- fix(service/minitrace): update doc by @andylokandy in https://github.com/apache/incubator-opendal/pull/2621
+
+### Docs
+
+- doc(bindings/haskell): add module document by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2566
+- docs: Update license related comments by @Prashanth-Chandra in https://github.com/apache/incubator-opendal/pull/2573
+- docs: add hdfs namenode High Availability related troubleshoot by @wcy-fdu in https://github.com/apache/incubator-opendal/pull/2601
+- docs: polish release doc by @PsiACE in https://github.com/apache/incubator-opendal/pull/2608
+- docs(blog): add Apache OpenDAL(Incubating): Access Data Freely by @PsiACE in https://github.com/apache/incubator-opendal/pull/2607
+- docs(RFC): Object Versioning by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2602
+
+### CI
+
+- ci: Disable bindings/java deploy for now by @tisonkun in https://github.com/apache/incubator-opendal/pull/2560
+- ci: Disable the failed stage-release job instead by @tisonkun in https://github.com/apache/incubator-opendal/pull/2561
+- ci: add haddock generator for haskell binding by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2569
+- ci(binding/lua): add luarocks package manager support by @oowl in https://github.com/apache/incubator-opendal/pull/2558
+- build(deps): bump predicates from 2.1.5 to 3.0.1 by @dependabot in https://github.com/apache/incubator-opendal/pull/2583
+- build(deps): bump tower-http from 0.4.0 to 0.4.1 by @dependabot in https://github.com/apache/incubator-opendal/pull/2582
+- build(deps): bump chrono from 0.4.24 to 0.4.26 by @dependabot in https://github.com/apache/incubator-opendal/pull/2581
+- build(deps): bump redis from 0.22.3 to 0.23.0 by @dependabot in https://github.com/apache/incubator-opendal/pull/2580
+- build(deps): bump cbindgen from 0.24.3 to 0.24.5 by @dependabot in https://github.com/apache/incubator-opendal/pull/2579
+- ci: upgrade hawkeye to v3 by @tisonkun in https://github.com/apache/incubator-opendal/pull/2585
+- ci(services/webdav): Setup integration test for nextcloud by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2631
+
+### Chore
+
+- chore: add haskell binding link to website by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2571
+- chore: fix cargo warning for resolver by @xxchan in https://github.com/apache/incubator-opendal/pull/2590
+- chore: bump log to 0.4.19 by @xxchan in https://github.com/apache/incubator-opendal/pull/2591
+- chore(deps): update deps to latest version by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2596
+- chore: Add release 0.38.0 to download by @PsiACE in https://github.com/apache/incubator-opendal/pull/2597
+- chore(service/minitrace): automatically generate span name by @andylokandy in https://github.com/apache/incubator-opendal/pull/2618
+
+## New Contributors
+
+- @Prashanth-Chandra made their first contribution in https://github.com/apache/incubator-opendal/pull/2573
+- @andylokandy made their first contribution in https://github.com/apache/incubator-opendal/pull/2618
+- @parkma99 made their first contribution in https://github.com/apache/incubator-opendal/pull/2634
+
+**Full Changelog**: https://github.com/apache/incubator-opendal/compare/v0.38.0...v0.38.1
+
 ## [v0.38.0] - 2023-06-27
 
 ### Added
-* feat(raw/http_util): Implement mixed multipart parser by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2430
-* feat(services/gcs): Add batch delete support by @wcy-fdu in https://github.com/apache/incubator-opendal/pull/2142
-* feat(core): Add Write::sink API by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2440
-* feat(services/s3): Allow retry for unexpected 499 error by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2453
-* feat(layer): add throttle layer by @morristai in https://github.com/apache/incubator-opendal/pull/2444
-* feat(bindings/haskell): init haskell binding by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2463
-* feat(core): add capability check by @unixzii in https://github.com/apache/incubator-opendal/pull/2461
-* feat(bindings/haskell): add CONTRIBUTING.md by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2466
-* feat(bindings/haskell): add CI test for haskell binding by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2468
-* feat(binding/lua): introduce opendal lua binding by @oowl in https://github.com/apache/incubator-opendal/pull/2469
-* feat(bindings/swift): add Swift binding by @unixzii in https://github.com/apache/incubator-opendal/pull/2470
-* feat(bindings/haskell): support `is_exist` `create_dir` `copy` `rename` `delete` by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2475
-* feat(bindings/haskell): add `Monad` wrapper by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2482
-* feat(bindings/dotnet): basic structure by @tisonkun in https://github.com/apache/incubator-opendal/pull/2485
-* feat(services/dropbox): Support create/read/delete for Dropbox by @Zheaoli in https://github.com/apache/incubator-opendal/pull/2264
-* feat(bindings/java): support load system lib by @tisonkun in https://github.com/apache/incubator-opendal/pull/2502
-* feat(blocking operator): add remove_all api by @infdahai in https://github.com/apache/incubator-opendal/pull/2449
-* feat(core): adopt WebHDFS LISTSTATUS_BATCH for better performance by @morristai in https://github.com/apache/incubator-opendal/pull/2499
-* feat(bindings/haskell): support stat by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2504
-* feat(adapters-kv): add rename and copy support to kv adapters by @oowl in https://github.com/apache/incubator-opendal/pull/2513
-* feat: Implement sink for services s3 by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2508
-* feat(adapters-kv): add rename and copy support to non typed kv adapters by @oowl in https://github.com/apache/incubator-opendal/pull/2515
-* feat: Implement test harness via libtest-mimic instead by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2517
-* feat(service/sled): introduce tree support by @oowl in https://github.com/apache/incubator-opendal/pull/2516
-* feat(bindings/haskell): support list and scan by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2527
-* feat(services/redb): support redb service by @oowl in https://github.com/apache/incubator-opendal/pull/2526
-* feat(core): implement service for Mini Moka by @morristai in https://github.com/apache/incubator-opendal/pull/2537
-* feat(core): add Mini Moka GitHub Action workflow job by @morristai in https://github.com/apache/incubator-opendal/pull/2539
-* feat(services): add cacache backend by @PsiACE in https://github.com/apache/incubator-opendal/pull/2548
-* feat: Implement Writer::copy so user can copy from AsyncRead by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2552
-### Changed
-* refactor(bindings/C): refactor c bindings to call all APIs using pointer by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2489
-### Fixed
-* fix(services/azblob): Fix azblob batch max operations by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2434
-* fix(services/sftp): change default root config to remote server setting by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2431
-* fix: Enable `std` feature for futures to allow `futures::AsyncRead` by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2450
-* fix(services/gcs): GCS should support create dir by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2467
-* fix(bindings/C): use copy_from_slice instead of from_static in opendal_bytes by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2473
-* fix(bindings/swift): reorg the package to correct its name by @unixzii in https://github.com/apache/incubator-opendal/pull/2479
-* fix: Fix the build for zig binding by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2493
-* fix(service/webhdfs): fix webhdfs config builder for disable_list_batch by @morristai in https://github.com/apache/incubator-opendal/pull/2509
-* fix(core/types): add missing `vercel artifacts` for `FromStr` by @cijiugechu in https://github.com/apache/incubator-opendal/pull/2519
-* fix(types/operator): fix operation limit error default size by @oowl in https://github.com/apache/incubator-opendal/pull/2536
-### Docs
-* docs: Replace `create` with `new` by @NiwakaDev in https://github.com/apache/incubator-opendal/pull/2427
-* docs(services/redis): fix redis via config example by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2443
-* docs: add rust usage example by @Young-Flash in https://github.com/apache/incubator-opendal/pull/2447
-* docs: Polish rust examples by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2456
-* docs: polish docs and fix typos by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2458
-* docs: fix a typo on the landing page by @unixzii in https://github.com/apache/incubator-opendal/pull/2460
-* docs(examples/rust): Add 01-init-operator by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2464
-* docs: update readme.md to match the output by @rrain7 in https://github.com/apache/incubator-opendal/pull/2486
-* docs: Update components for Libraries and Services by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2487
-* docs: Add OctoBase into our users list by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2506
-* docs: Fix scan not checked for sled services by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2507
-* doc(binding/lua): Improve readme doc for contribute and usage by @oowl in https://github.com/apache/incubator-opendal/pull/2511
-* doc(services/redb): add doc for redb service backend by @oowl in https://github.com/apache/incubator-opendal/pull/2538
-* doc(bindings/swift): add CONTRIBUTING.md by @unixzii in https://github.com/apache/incubator-opendal/pull/2540
-* docs: Add new rust example 02-async-io by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2541
-* docs: Fix link for CONTRIBUTING.md  by @HuSharp in https://github.com/apache/incubator-opendal/pull/2544
-* doc: polish release doc by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2531
-* docs: Move verify to upper folder by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2546
-* doc(binding/lua): add ldoc generactor for lua binding by @oowl in https://github.com/apache/incubator-opendal/pull/2549
-* docs: Add new architectural image for OpenDAL by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2553
-* docs: Polish README for core and bindings by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2554
+
+- feat(raw/http_util): Implement mixed multipart parser by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2430
+- feat(services/gcs): Add batch delete support by @wcy-fdu in https://github.com/apache/incubator-opendal/pull/2142
+- feat(core): Add Write::sink API by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2440
+- feat(services/s3): Allow retry for unexpected 499 error by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2453
+- feat(layer): add throttle layer by @morristai in https://github.com/apache/incubator-opendal/pull/2444
+- feat(bindings/haskell): init haskell binding by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2463
+- feat(core): add capability check by @unixzii in https://github.com/apache/incubator-opendal/pull/2461
+- feat(bindings/haskell): add CONTRIBUTING.md by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2466
+- feat(bindings/haskell): add CI test for haskell binding by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2468
+- feat(binding/lua): introduce opendal lua binding by @oowl in https://github.com/apache/incubator-opendal/pull/2469
+- feat(bindings/swift): add Swift binding by @unixzii in https://github.com/apache/incubator-opendal/pull/2470
+- feat(bindings/haskell): support `is_exist` `create_dir` `copy` `rename` `delete` by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2475
+- feat(bindings/haskell): add `Monad` wrapper by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2482
+- feat(bindings/dotnet): basic structure by @tisonkun in https://github.com/apache/incubator-opendal/pull/2485
+- feat(services/dropbox): Support create/read/delete for Dropbox by @Zheaoli in https://github.com/apache/incubator-opendal/pull/2264
+- feat(bindings/java): support load system lib by @tisonkun in https://github.com/apache/incubator-opendal/pull/2502
+- feat(blocking operator): add remove_all api by @infdahai in https://github.com/apache/incubator-opendal/pull/2449
+- feat(core): adopt WebHDFS LISTSTATUS_BATCH for better performance by @morristai in https://github.com/apache/incubator-opendal/pull/2499
+- feat(bindings/haskell): support stat by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2504
+- feat(adapters-kv): add rename and copy support to kv adapters by @oowl in https://github.com/apache/incubator-opendal/pull/2513
+- feat: Implement sink for services s3 by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2508
+- feat(adapters-kv): add rename and copy support to non typed kv adapters by @oowl in https://github.com/apache/incubator-opendal/pull/2515
+- feat: Implement test harness via libtest-mimic instead by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2517
+- feat(service/sled): introduce tree support by @oowl in https://github.com/apache/incubator-opendal/pull/2516
+- feat(bindings/haskell): support list and scan by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2527
+- feat(services/redb): support redb service by @oowl in https://github.com/apache/incubator-opendal/pull/2526
+- feat(core): implement service for Mini Moka by @morristai in https://github.com/apache/incubator-opendal/pull/2537
+- feat(core): add Mini Moka GitHub Action workflow job by @morristai in https://github.com/apache/incubator-opendal/pull/2539
+- feat(services): add cacache backend by @PsiACE in https://github.com/apache/incubator-opendal/pull/2548
+- feat: Implement Writer::copy so user can copy from AsyncRead by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2552
+
+### Changed
+
+- refactor(bindings/C): refactor c bindings to call all APIs using pointer by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2489
+
+### Fixed
+
+- fix(services/azblob): Fix azblob batch max operations by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2434
+- fix(services/sftp): change default root config to remote server setting by @silver-ymz in https://github.com/apache/incubator-opendal/pull/2431
+- fix: Enable `std` feature for futures to allow `futures::AsyncRead` by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2450
+- fix(services/gcs): GCS should support create dir by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2467
+- fix(bindings/C): use copy_from_slice instead of from_static in opendal_bytes by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2473
+- fix(bindings/swift): reorg the package to correct its name by @unixzii in https://github.com/apache/incubator-opendal/pull/2479
+- fix: Fix the build for zig binding by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2493
+- fix(service/webhdfs): fix webhdfs config builder for disable_list_batch by @morristai in https://github.com/apache/incubator-opendal/pull/2509
+- fix(core/types): add missing `vercel artifacts` for `FromStr` by @cijiugechu in https://github.com/apache/incubator-opendal/pull/2519
+- fix(types/operator): fix operation limit error default size by @oowl in https://github.com/apache/incubator-opendal/pull/2536
+
+### Docs
+
+- docs: Replace `create` with `new` by @NiwakaDev in https://github.com/apache/incubator-opendal/pull/2427
+- docs(services/redis): fix redis via config example by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2443
+- docs: add rust usage example by @Young-Flash in https://github.com/apache/incubator-opendal/pull/2447
+- docs: Polish rust examples by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2456
+- docs: polish docs and fix typos by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2458
+- docs: fix a typo on the landing page by @unixzii in https://github.com/apache/incubator-opendal/pull/2460
+- docs(examples/rust): Add 01-init-operator by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2464
+- docs: update readme.md to match the output by @rrain7 in https://github.com/apache/incubator-opendal/pull/2486
+- docs: Update components for Libraries and Services by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2487
+- docs: Add OctoBase into our users list by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2506
+- docs: Fix scan not checked for sled services by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2507
+- doc(binding/lua): Improve readme doc for contribute and usage by @oowl in https://github.com/apache/incubator-opendal/pull/2511
+- doc(services/redb): add doc for redb service backend by @oowl in https://github.com/apache/incubator-opendal/pull/2538
+- doc(bindings/swift): add CONTRIBUTING.md by @unixzii in https://github.com/apache/incubator-opendal/pull/2540
+- docs: Add new rust example 02-async-io by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2541
+- docs: Fix link for CONTRIBUTING.md by @HuSharp in https://github.com/apache/incubator-opendal/pull/2544
+- doc: polish release doc by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2531
+- docs: Move verify to upper folder by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2546
+- doc(binding/lua): add ldoc generactor for lua binding by @oowl in https://github.com/apache/incubator-opendal/pull/2549
+- docs: Add new architectural image for OpenDAL by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2553
+- docs: Polish README for core and bindings by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2554
+
 ### CI
-* ci: Fix append test should use copy_buf to avoid call times by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2436
-* build(bindings/ruby): fix compile rb-sys on Apple M1 by @tisonkun in https://github.com/apache/incubator-opendal/pull/2451
-* ci: Use summary for zig test to fix build by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2480
-* ci(workflow): add lua binding test workflow by @oowl in https://github.com/apache/incubator-opendal/pull/2478
-* build(deps): bump actions/setup-python from 3 to 4 by @dependabot in https://github.com/apache/incubator-opendal/pull/2481
-* ci(bindings/swift): add CI for Swift binding by @unixzii in https://github.com/apache/incubator-opendal/pull/2492
-* ci: Try to make webhdfs tests more stable by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2503
-* ci(bindings/java): auto release snapshot  by @tisonkun in https://github.com/apache/incubator-opendal/pull/2521
-* ci: Disable the stage snapshot CI by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2528
-* ci: fix opendal-java snapshot releases by @tisonkun in https://github.com/apache/incubator-opendal/pull/2532
-* ci: Fix typo in binding java CI by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2534
-* ci(bindings/swift): optimize time consumption of CI pipeline by @unixzii in https://github.com/apache/incubator-opendal/pull/2545
-* ci: Fix PR label not updated while edited by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2547
+
+- ci: Fix append test should use copy_buf to avoid call times by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2436
+- build(bindings/ruby): fix compile rb-sys on Apple M1 by @tisonkun in https://github.com/apache/incubator-opendal/pull/2451
+- ci: Use summary for zig test to fix build by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2480
+- ci(workflow): add lua binding test workflow by @oowl in https://github.com/apache/incubator-opendal/pull/2478
+- build(deps): bump actions/setup-python from 3 to 4 by @dependabot in https://github.com/apache/incubator-opendal/pull/2481
+- ci(bindings/swift): add CI for Swift binding by @unixzii in https://github.com/apache/incubator-opendal/pull/2492
+- ci: Try to make webhdfs tests more stable by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2503
+- ci(bindings/java): auto release snapshot by @tisonkun in https://github.com/apache/incubator-opendal/pull/2521
+- ci: Disable the stage snapshot CI by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2528
+- ci: fix opendal-java snapshot releases by @tisonkun in https://github.com/apache/incubator-opendal/pull/2532
+- ci: Fix typo in binding java CI by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2534
+- ci(bindings/swift): optimize time consumption of CI pipeline by @unixzii in https://github.com/apache/incubator-opendal/pull/2545
+- ci: Fix PR label not updated while edited by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2547
+
 ### Chore
-* chore: Add redis bench support by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2438
-* chore(bindings/nodejs): update index.d.ts by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2459
-* chore: Add release 0.37.0 to download by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2472
-* chore: Fix Cargo.lock not updated by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2490
-* chore: Polish some code details by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2505
-* chore(bindings/nodejs): provide more precise type for scheme by @cijiugechu in https://github.com/apache/incubator-opendal/pull/2520
+
+- chore: Add redis bench support by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2438
+- chore(bindings/nodejs): update index.d.ts by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2459
+- chore: Add release 0.37.0 to download by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2472
+- chore: Fix Cargo.lock not updated by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2490
+- chore: Polish some code details by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2505
+- chore(bindings/nodejs): provide more precise type for scheme by @cijiugechu in https://github.com/apache/incubator-opendal/pull/2520
 
 ## [v0.37.0] - 2023-06-06
 
 ### Added
-* feat(services/webdav): support redirection when get 302/307 response during read operation by @Yansongsongsong in https://github.com/apache/incubator-opendal/pull/2256
-* feat: Add Zig Bindings Module by @kassane in https://github.com/apache/incubator-opendal/pull/2374
-* feat: Implement Timeout Layer by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2395
-* feat(bindings/c): add  opendal_operator_blocking_delete method by @jiaoew1991 in https://github.com/apache/incubator-opendal/pull/2416
-* feat(services/obs): add append support by @infdahai in https://github.com/apache/incubator-opendal/pull/2422
-### Changed
-* refactor(bindings/zig): enable tests and more by @tisonkun in https://github.com/apache/incubator-opendal/pull/2375
-* refactor(bindings/zig): add errors handler and module test by @kassane in https://github.com/apache/incubator-opendal/pull/2381
-* refactor(http_util): Adopt reqwest's redirect support by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2390
-### Fixed
-* fix(bindings/zig): reflect C interface changes by @tisonkun in https://github.com/apache/incubator-opendal/pull/2378
-* fix(services/azblob): Fix batch delete doesn't work on azure by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2382
-* fix(services/oss): Fix oss batch max operations by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2414
-* fix(core): Don't wake up operator futures while not ready by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2415
-* fix(services/s3): Fix s3 batch max operations by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2418
-### Docs
-* docs: service doc for s3 by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2376
-* docs(bindings/C): The documentation for OpenDAL C binding by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2373
-* docs: add link for c binding by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2380
-* docs: docs for kv services by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2396
-* docs: docs for fs related services by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2397
-* docs(bindings/java): do not release snapshot versions anymore by @tisonkun in https://github.com/apache/incubator-opendal/pull/2398
-* docs: doc for ipmfs by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2408
-* docs: add service doc for oss by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2409
-* docs: improvement of Python binding by @ideal in https://github.com/apache/incubator-opendal/pull/2411
-* docs: doc for download by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2424
-* docs: Add release guide by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2425
+
+- feat(services/webdav): support redirection when get 302/307 response during read operation by @Yansongsongsong in https://github.com/apache/incubator-opendal/pull/2256
+- feat: Add Zig Bindings Module by @kassane in https://github.com/apache/incubator-opendal/pull/2374
+- feat: Implement Timeout Layer by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2395
+- feat(bindings/c): add opendal_operator_blocking_delete method by @jiaoew1991 in https://github.com/apache/incubator-opendal/pull/2416
+- feat(services/obs): add append support by @infdahai in https://github.com/apache/incubator-opendal/pull/2422
+
+### Changed
+
+- refactor(bindings/zig): enable tests and more by @tisonkun in https://github.com/apache/incubator-opendal/pull/2375
+- refactor(bindings/zig): add errors handler and module test by @kassane in https://github.com/apache/incubator-opendal/pull/2381
+- refactor(http_util): Adopt reqwest's redirect support by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2390
+
+### Fixed
+
+- fix(bindings/zig): reflect C interface changes by @tisonkun in https://github.com/apache/incubator-opendal/pull/2378
+- fix(services/azblob): Fix batch delete doesn't work on azure by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2382
+- fix(services/oss): Fix oss batch max operations by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2414
+- fix(core): Don't wake up operator futures while not ready by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2415
+- fix(services/s3): Fix s3 batch max operations by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2418
+
+### Docs
+
+- docs: service doc for s3 by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2376
+- docs(bindings/C): The documentation for OpenDAL C binding by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2373
+- docs: add link for c binding by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2380
+- docs: docs for kv services by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2396
+- docs: docs for fs related services by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2397
+- docs(bindings/java): do not release snapshot versions anymore by @tisonkun in https://github.com/apache/incubator-opendal/pull/2398
+- docs: doc for ipmfs by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2408
+- docs: add service doc for oss by @A-Stupid-Sun in https://github.com/apache/incubator-opendal/pull/2409
+- docs: improvement of Python binding by @ideal in https://github.com/apache/incubator-opendal/pull/2411
+- docs: doc for download by @suyanhanx in https://github.com/apache/incubator-opendal/pull/2424
+- docs: Add release guide by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2425
+
 ### CI
-* ci: Enable semantic PRs by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2370
-* ci: improve licenserc settings by @tisonkun in https://github.com/apache/incubator-opendal/pull/2377
-* build(deps): bump reqwest from 0.11.15 to 0.11.18 by @dependabot in https://github.com/apache/incubator-opendal/pull/2389
-* build(deps): bump pyo3 from 0.18.2 to 0.18.3 by @dependabot in https://github.com/apache/incubator-opendal/pull/2388
-* ci: Enable nextest for all behavior tests by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2400
-* ci: reflect ascii file rewrite by @tisonkun in https://github.com/apache/incubator-opendal/pull/2419
-* ci: Remove website from git archive by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2420
-* ci: Add integration tests for Cloudflare R2 by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2423
+
+- ci: Enable semantic PRs by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2370
+- ci: improve licenserc settings by @tisonkun in https://github.com/apache/incubator-opendal/pull/2377
+- build(deps): bump reqwest from 0.11.15 to 0.11.18 by @dependabot in https://github.com/apache/incubator-opendal/pull/2389
+- build(deps): bump pyo3 from 0.18.2 to 0.18.3 by @dependabot in https://github.com/apache/incubator-opendal/pull/2388
+- ci: Enable nextest for all behavior tests by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2400
+- ci: reflect ascii file rewrite by @tisonkun in https://github.com/apache/incubator-opendal/pull/2419
+- ci: Remove website from git archive by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2420
+- ci: Add integration tests for Cloudflare R2 by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2423
+
 ### Chore
-* chore(bindings/python): upgrade maturin to 1.0 by @messense in https://github.com/apache/incubator-opendal/pull/2369
-* chore: Fix license headers for release/labler by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2371
-* chore(bindings/C): add one simple read/write example into readme and code by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2421
+
+- chore(bindings/python): upgrade maturin to 1.0 by @messense in https://github.com/apache/incubator-opendal/pull/2369
+- chore: Fix license headers for release/labler by @Xuanwo in https://github.com/apache/incubator-opendal/pull/2371
+- chore(bindings/C): add one simple read/write example into readme and code by @Ji-Xinyou in https://github.com/apache/incubator-opendal/pull/2421
 
 ## [v0.36.0] - 2023-05-30
 
 ### Added
 
 - feat(service/fs): add append support for fs (#2296)
 - feat(services/sftp): add append support for sftp (#2297)
@@ -191,15 +287,15 @@
 - docs: add service doc for cos (#2341)
 - docs: add service doc for dashmap (#2342)
 - docs(bindings/java): for BlockingOperator (#2344)
 
 ### CI
 
 - build(bindings/java): prepare for snapshot release (#2301)
-- build(bindings/java): support multiple platform java bindings  (#2324)
+- build(bindings/java): support multiple platform java bindings (#2324)
 - ci(binding/nodejs): Use docker to build nodejs binding (#2328)
 - build(bindings/java): prepare for automatically multiple platform deploy (#2335)
 - ci: add bindings java docs and integrate with website (#2346)
 - ci: avoid copy gitignore to site folder (#2348)
 - ci(bindings/c): Add diff check (#2359)
 - ci: Cache librocksdb to speed up CI (#2360)
 - ci: Don't load rocksdb for all workflows (#2362)
@@ -216,18 +312,18 @@
 - chore: protect branch gh-pages (#2358)
 
 ## [v0.35.0] - 2023-05-23
 
 ### Added
 
 - feat(services/onedrive): Implement `list`, `create_dir`, `stat` and upload
-ing large files (#2231)
+  ing large files (#2231)
 - feat(bindings/C): Initially support stat in C binding (#2249)
 - feat(bindings/python): Enable `abi3` to avoid building on different python
- version (#2255)
+  version (#2255)
 - feat(bindings/C): support BDD tests using GTest (#2254)
 - feat(services/sftp): setup integration tests (#2192)
 - feat(core): Add trait and public API for `append` (#2260)
 - feat(services/sftp): support copy and rename for sftp (#2263)
 - feat(services/sftp): support copy and read_seek (#2267)
 - feat: Add COS service support (#2269)
 - feat(services/cos): Add support for loading from env (#2271)
@@ -282,15 +378,15 @@
 
 ### Added
 
 - feat(writer): configurable buffer size of unsized write (#2143)
 - feat(oay): Add basic s3 list_objects_v2 with start_after support (#2219)
 - feat: Add typed kv adapter and migrate moka to it (#2222)
 - feat: migrate service dashmap (#2225)
-- feat(services/memory): migrate service memory  (#2229)
+- feat(services/memory): migrate service memory (#2229)
 - feat: Add assert for public types to ensure Send + Sync (#2237)
 - feat(services/gcs): Add abort support for writer (#2242)
 
 ### Changed
 
 - refactor: Replace futures::ready with std::task::ready (#2221)
 - refactor: Use list without delimiter to replace scan (#2243)
@@ -383,15 +479,15 @@
 
 ### Docs
 
 - docs: add hdfs classpath related troubleshoot (#2130)
 
 ### CI
 
--  ci: Mark job as skipped if owner is not apache (#2128)
+- ci: Mark job as skipped if owner is not apache (#2128)
 - ci: Enable native-tls to test gcs presign for workaround (#2138)
 
 ## [v0.33.1] - 2023-04-25
 
 ### Added
 
 - feat: Add behavior test for read_with_if_match & stat_with_if_match (#2088)
@@ -509,15 +605,17 @@
 - refactor: Polish the behavior of scan (#1926)
 - refactor: Polish the implementation of webhdfs (#1935)
 
 ### Fixed
 
 - fix: sled should not be enabled by default (#1923)
 - fix: kv adapter's writer implementation fixed to honour empty writes (#193
-4)
+
+4.
+
 - fix(services/azblob): fix copy missing content-length (#2000)
 
 ### Docs
 
 - docs: Adding docs link to python binding (#1921)
 - docs(bindings/python): fix wrong doc link (#1928)
 - docs: Add contributing for OpenDAL (#1984)
@@ -574,15 +672,15 @@
 - refactor(core): Simplify the usage of BatchOperation and BatchResults (#1843)
 - refactor: Use reqwest blocking client instead of ureq (#1853)
 - refactor: Bump MSRV to 1.64 (#1864)
 - refactor: Remove not used blocking http client (#1895)
 - refactor: Change presign to async for future refactor (#1900)
 - refactor(services/gcs): Migrate to async reqsign (#1906)
 - refactor(services/azdfs): Migrate to async reqsign (#1903)
-- refactor(services/azblob): Adopt new reqsign  (#1902)
+- refactor(services/azblob): Adopt new reqsign (#1902)
 - refactor(services/s3): Migrate to async reqsign (#1909)
 - refactor(services/oss): Migrate to async reqsign (#1911)
 - refactor: Use chrono instead of time to work well with ecosystem (#1912)
 - refactor(service/obs): Migrate obs to async reqsign (#1914)
 
 ### Fixed
 
@@ -730,15 +828,15 @@
 - feat(bindings/nodejs): Migrate to BDD test (#1661)
 - feat(bindings/nodejs): Add generated `index.d.ts` (#1664)
 - feat(bindings/python): add auto-generated api docs (#1613)
 - feat(bindings/python): add `__repr__` to `Operator` and `AsyncOperator` (#1683)
 
 ### Changed
 
-- *: Change all files licenses to ASF (#1592)
+- \*: Change all files licenses to ASF (#1592)
 - refactor(bindings/python): only enable `pyo3/entension-module` feature when building with maturin (#1680)
 
 ### Fixed
 
 - fix(bindings/python): Fix the metadata for Python binding (#1568)
 - fix: Operator::remove_all behaviour on non-existing object fixed (#1587)
 - fix: reset Reader::SeekState when poll completed (#1609)
@@ -904,15 +1002,15 @@
 
 ### Changed
 
 - refactor: Promote operator as a mod for further refactor (#1479)
 
 ### Docs
 
-- docs: Add convert from m*n to m+n (#1454)
+- docs: Add convert from m\*n to m+n (#1454)
 - docs: Polish comments for public types (#1455)
 - docs: Add discord chat link (#1474)
 
 ### Chore
 
 - chore: fix typo (#1456)
 - chore: fix typo (#1459)
@@ -1186,15 +1284,14 @@
 - feat(services/hdfs): Evaluating the new async implementation (#1176)
 - feat(services/ghac): Handling too many requests error (#1181)
 
 ### Fixed
 
 - doc: fix name change in README (#1179)
 
-
 ## [v0.24.5] - 2023-01-09
 
 ### Fixed
 
 - fix(services/memcached): TcpStream should only accept host:port (#1170)
 
 ## [v0.24.4] - 2023-01-09
@@ -2366,14 +2463,15 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.38.1]: https://github.com/apache/incubator-opendal/compare/v0.38.0...v0.38.1
 [v0.38.0]: https://github.com/apache/incubator-opendal/compare/v0.37.0...v0.38.0
 [v0.37.0]: https://github.com/apache/incubator-opendal/compare/v0.36.0...v0.37.0
 [v0.36.0]: https://github.com/apache/incubator-opendal/compare/v0.35.0...v0.36.0
 [v0.35.0]: https://github.com/apache/incubator-opendal/compare/v0.34.0...v0.35.0
 [v0.34.0]: https://github.com/apache/incubator-opendal/compare/v0.33.3...v0.34.0
 [v0.33.3]: https://github.com/apache/incubator-opendal/compare/v0.33.2...v0.33.3
 [v0.33.2]: https://github.com/apache/incubator-opendal/compare/v0.33.1...v0.33.2
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.38.1/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/README.md` & `opendal-0.38.1/local_dependencies/opendal/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.38.1/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.38.1/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.38.1/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.38.1/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.38.1/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,45 +51,45 @@
 
 ### Design
 
 `object_store` exposed a trait called [`ObjectStore`](https://docs.rs/object_store/latest/object_store/trait.ObjectStore.html) to users.
 
 Users need to build a `dyn ObjectStore` and operate on it directly:
 
-```Rust
+```rust
 let object_store: Arc<dyn ObjectStore> = Arc::new(get_object_store());
 let path: Path = "data/file01.parquet".try_into()?;
 let stream = object_store
     .get(&path)
     .await?
     .into_stream();
 ```
 
 `opendal` has a similar trait called [`Accessor`][crate::raw::Accessor]
 
 But `opendal` don't expose this trait to end users directly. Instead, `opendal` expose a new struct called [`Operator`][crate::Operator] and builds public API on it.
 
-```Rust
+```rust
 let op: Operator = Operator::from_env(Scheme::S3)?;
 let r = op.reader("data/file01.parquet").await?;
 ```
 
 ### Interception
 
 Both `object_store` and `opendal` provide a mechanism to intercept operations.
 
 `object_store` called `Adapters`:
 
-```Rust
+```rust
 let object_store = ThrottledStore::new(get_object_store(), ThrottleConfig::default())
 ```
 
 `opendal` called [`Layer`](crate::raw::Layer):
 
-```Rust
+```rust
 let op = op.layer(TracingLayer).layer(MetricsLayer);
 ```
 
 At the time of writing:
 
 object_store (`v0.5.0`) supports:
 
@@ -153,27 +153,27 @@
 
 ## Demo show
 
 The most straightforward complete demo how to read a file from s3:
 
 `opendal`
 
-```Rust
+```rust
 let mut builder = S3::default();
 builder.bucket("example");
 builder.access_key_id("access_key_id");
 builder.secret_access_key("secret_access_key");
 
 let store = Operator::new(builder)?.finish();
 let r = store.reader("data.parquet").await?;
 ```
 
 `object_store`
 
-```Rust
+```rust
 let mut builder = AmazonS3Builder::new()
 .with_bucket_name("example")
 .with_access_key_id("access_key_id")
 .with_secret_access_key("secret_access_key");
 
 let store = Arc::new(builder.build()?);
 let path: Path = "data.parquet".try_into().unwrap();
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.38.1/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/features.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.38.1/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/2299_chain_based_operator_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -138,7 +138,10 @@
 pub mod rfc_2083_writer_sink_api {}
 
 #[doc = include_str!("2133_append_api.md")]
 pub mod rfc_2133_append_api {}
 
 #[doc = include_str!("2299_chain_based_operator_api.md")]
 pub mod rfc_2299_chain_based_operator_api {}
+
+#[doc = include_str!("2602_object_versioning.md")]
+pub mod rfc_2602_object_versioning {}
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.38.1/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/complete.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/logging.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::FutureExt;
 use minitrace::prelude::*;
 
+use crate::raw::oio::AppendOperation;
 use crate::raw::oio::PageOperation;
 use crate::raw::oio::ReadOperation;
 use crate::raw::oio::WriteOperation;
 use crate::raw::*;
 use crate::*;
 
 /// Add [minitrace](https://docs.rs/minitrace/) for every operations.
@@ -59,40 +60,37 @@
 /// use opendal::layers::MinitraceLayer;
 /// use opendal::services;
 /// use opendal::Operator;
 ///
 /// fn main() -> Result<(), Box<dyn Error + Send + Sync + 'static>> {
 ///     let collector = {
 ///         let (span, collector) = minitrace::Span::root("op");
-///         let _g = span.set_local_parent();
 ///         let runtime = tokio::runtime::Runtime::new()?;
-///
-///         runtime.block_on(async {
-///             let _ = dotenvy::dotenv();
-///             let op = Operator::from_env::<services::Memory>()
-///                 .expect("init operator must succeed")
-///                 .layer(MinitraceLayer)
-///                 .finish();
-///
-///             op.write("test", "0".repeat(16 * 1024 * 1024).into_bytes())
-///                 .await
-///                 .expect("must succeed");
-///             op.stat("test").await.expect("must succeed");
-///             op.read("test").await.expect("must succeed");
-///         });
+///         runtime.block_on(
+///             async {
+///                 let _ = dotenvy::dotenv();
+///                 let op = Operator::from_env::<services::Memory>()
+///                     .expect("init operator must succeed")
+///                     .layer(MinitraceLayer)
+///                     .finish();
+///                 op.write("test", "0".repeat(16 * 1024 * 1024).into_bytes())
+///                     .await
+///                     .expect("must succeed");
+///                 op.stat("test").await.expect("must succeed");
+///                 op.read("test").await.expect("must succeed");
+///             }
+///             .in_span(Span::enter_with_parent("test", &span)),
+///         );
 ///         collector
 ///     };
-///
 ///     let spans = block_on(collector.collect());
-///
 ///     let bytes =
 ///         minitrace_jaeger::encode("opendal".to_owned(), rand::random(), 0, 0, &spans).unwrap();
 ///     minitrace_jaeger::report_blocking("127.0.0.1:6831".parse().unwrap(), &bytes)
 ///         .expect("report error");
-///
 ///     Ok(())
 /// }
 /// ```
 ///
 /// # Output
 ///
 /// OpenDAL is using [`minitrace`](https://docs.rs/minitrace/latest/minitrace/) for tracing internally.
@@ -130,141 +128,173 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for MinitraceAccessor<A> {
     type Inner = A;
     type Reader = MinitraceWrapper<A::Reader>;
     type BlockingReader = MinitraceWrapper<A::BlockingReader>;
     type Writer = MinitraceWrapper<A::Writer>;
     type BlockingWriter = MinitraceWrapper<A::BlockingWriter>;
-    type Appender = A::Appender;
+    type Appender = MinitraceWrapper<A::Appender>;
     type Pager = MinitraceWrapper<A::Pager>;
     type BlockingPager = MinitraceWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
-    #[trace("metadata")]
+    #[trace]
     fn metadata(&self) -> AccessorInfo {
         self.inner.info()
     }
 
     #[trace("create", enter_on_poll = true)]
     async fn create_dir(&self, path: &str, args: OpCreateDir) -> Result<RpCreateDir> {
         self.inner.create_dir(path, args).await
     }
 
+    #[trace(enter_on_poll = true)]
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let span = Span::enter_with_local_parent("read");
         self.inner
             .read(path, args)
-            .map(|v| v.map(|(rp, r)| (rp, MinitraceWrapper::new(span, r))))
+            .map(|v| {
+                v.map(|(rp, r)| {
+                    (
+                        rp,
+                        MinitraceWrapper::new(Span::enter_with_local_parent("ReadOperation"), r),
+                    )
+                })
+            })
             .await
     }
 
+    #[trace(enter_on_poll = true)]
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        let span = Span::enter_with_local_parent("write");
         self.inner
             .write(path, args)
-            .map(|v| v.map(|(rp, r)| (rp, MinitraceWrapper::new(span, r))))
+            .map(|v| {
+                v.map(|(rp, r)| {
+                    (
+                        rp,
+                        MinitraceWrapper::new(Span::enter_with_local_parent("WriteOperation"), r),
+                    )
+                })
+            })
             .await
     }
 
+    #[trace(enter_on_poll = true)]
     async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
-        self.inner.append(path, args).await
+        self.inner
+            .append(path, args)
+            .map(|v| {
+                v.map(|(rp, r)| {
+                    (
+                        rp,
+                        MinitraceWrapper::new(Span::enter_with_local_parent("AppendOperation"), r),
+                    )
+                })
+            })
+            .await
     }
 
-    #[trace("copy", enter_on_poll = true)]
+    #[trace(enter_on_poll = true)]
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         self.inner().copy(from, to, args).await
     }
 
-    #[trace("rename", enter_on_poll = true)]
+    #[trace(enter_on_poll = true)]
     async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         self.inner().rename(from, to, args).await
     }
 
-    #[trace("stat", enter_on_poll = true)]
+    #[trace(enter_on_poll = true)]
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner.stat(path, args).await
     }
 
-    #[trace("delete", enter_on_poll = true)]
+    #[trace(enter_on_poll = true)]
     async fn delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         self.inner.delete(path, args).await
     }
 
+    #[trace(enter_on_poll = true)]
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
-        let span = Span::enter_with_local_parent("list");
         self.inner
             .list(path, args)
-            .map(|v| v.map(|(rp, s)| (rp, MinitraceWrapper::new(span, s))))
+            .map(|v| {
+                v.map(|(rp, s)| {
+                    (
+                        rp,
+                        MinitraceWrapper::new(Span::enter_with_local_parent("ListOperation"), s),
+                    )
+                })
+            })
             .await
     }
 
-    #[trace("presign", enter_on_poll = true)]
+    #[trace(enter_on_poll = true)]
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         self.inner.presign(path, args).await
     }
 
-    #[trace("batch", enter_on_poll = true)]
+    #[trace(enter_on_poll = true)]
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         self.inner.batch(args).await
     }
 
-    #[trace("blocking_create")]
+    #[trace]
     fn blocking_create_dir(&self, path: &str, args: OpCreateDir) -> Result<RpCreateDir> {
         self.inner.blocking_create_dir(path, args)
     }
 
+    #[trace]
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
-        let span = Span::enter_with_local_parent("blocking_read");
         self.inner.blocking_read(path, args).map(|(rp, r)| {
             (
                 rp,
-                MinitraceWrapper::new(Span::enter_with_parent("ReadOperation", &span), r),
+                MinitraceWrapper::new(Span::enter_with_local_parent("ReadOperation"), r),
             )
         })
     }
 
+    #[trace]
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
-        let span = Span::enter_with_local_parent("blocking_write");
         self.inner.blocking_write(path, args).map(|(rp, r)| {
             (
                 rp,
-                MinitraceWrapper::new(Span::enter_with_parent("WriteOperation", &span), r),
+                MinitraceWrapper::new(Span::enter_with_local_parent("WriteOperation"), r),
             )
         })
     }
 
-    #[trace("blocking_copy")]
+    #[trace]
     fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         self.inner().blocking_copy(from, to, args)
     }
 
-    #[trace("blocking_rename")]
+    #[trace]
     fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         self.inner().blocking_rename(from, to, args)
     }
 
-    #[trace("blocking_stat")]
+    #[trace]
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner.blocking_stat(path, args)
     }
 
-    #[trace("blocking_delete")]
+    #[trace]
     fn blocking_delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         self.inner.blocking_delete(path, args)
     }
 
+    #[trace]
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
-        let span = Span::enter_with_local_parent("blocking_list");
         self.inner.blocking_list(path, args).map(|(rp, it)| {
             (
                 rp,
-                MinitraceWrapper::new(Span::enter_with_parent("PageOperation", &span), it),
+                MinitraceWrapper::new(Span::enter_with_local_parent("PageOperation"), it),
             )
         })
     }
 }
 
 pub struct MinitraceWrapper<R> {
     span: Span,
@@ -275,42 +305,48 @@
     fn new(span: Span, inner: R) -> Self {
         Self { span, inner }
     }
 }
 
 impl<R: oio::Read> oio::Read for MinitraceWrapper<R> {
     fn poll_read(&mut self, cx: &mut Context<'_>, buf: &mut [u8]) -> Poll<Result<usize>> {
-        let _span = Span::enter_with_parent(ReadOperation::Read.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(ReadOperation::Read.into_static());
         self.inner.poll_read(cx, buf)
     }
 
     fn poll_seek(&mut self, cx: &mut Context<'_>, pos: io::SeekFrom) -> Poll<Result<u64>> {
-        let _span = Span::enter_with_parent(ReadOperation::Seek.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(ReadOperation::Seek.into_static());
         self.inner.poll_seek(cx, pos)
     }
 
     fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<Bytes>>> {
-        let _span = Span::enter_with_parent(ReadOperation::Next.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(ReadOperation::Next.into_static());
         self.inner.poll_next(cx)
     }
 }
 
 impl<R: oio::BlockingRead> oio::BlockingRead for MinitraceWrapper<R> {
     fn read(&mut self, buf: &mut [u8]) -> Result<usize> {
-        let _span = Span::enter_with_parent(ReadOperation::BlockingRead.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(ReadOperation::BlockingRead.into_static());
         self.inner.read(buf)
     }
 
     fn seek(&mut self, pos: io::SeekFrom) -> Result<u64> {
-        let _span = Span::enter_with_parent(ReadOperation::BlockingSeek.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(ReadOperation::BlockingSeek.into_static());
         self.inner.seek(pos)
     }
 
     fn next(&mut self) -> Option<Result<Bytes>> {
-        let _span = Span::enter_with_parent(ReadOperation::BlockingNext.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(ReadOperation::BlockingNext.into_static());
         self.inner.next()
     }
 }
 
 #[async_trait]
 impl<R: oio::Write> oio::Write for MinitraceWrapper<R> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
@@ -352,38 +388,62 @@
             ))
             .await
     }
 }
 
 impl<R: oio::BlockingWrite> oio::BlockingWrite for MinitraceWrapper<R> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
-        let _span =
-            Span::enter_with_parent(WriteOperation::BlockingWrite.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(WriteOperation::BlockingWrite.into_static());
         self.inner.write(bs)
     }
 
     fn close(&mut self) -> Result<()> {
-        let _span =
-            Span::enter_with_parent(WriteOperation::BlockingClose.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(WriteOperation::BlockingClose.into_static());
         self.inner.close()
     }
 }
 
 #[async_trait]
+impl<R: oio::Append> oio::Append for MinitraceWrapper<R> {
+    async fn append(&mut self, bs: Bytes) -> Result<()> {
+        self.inner
+            .append(bs)
+            .in_span(Span::enter_with_parent(
+                AppendOperation::Append.into_static(),
+                &self.span,
+            ))
+            .await
+    }
+
+    async fn close(&mut self) -> Result<()> {
+        self.inner
+            .close()
+            .in_span(Span::enter_with_parent(
+                AppendOperation::Close.into_static(),
+                &self.span,
+            ))
+            .await
+    }
+}
+
+#[async_trait]
 impl<R: oio::Page> oio::Page for MinitraceWrapper<R> {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         self.inner
             .next()
             .in_span(Span::enter_with_parent(
                 PageOperation::Next.into_static(),
                 &self.span,
             ))
             .await
     }
 }
 
 impl<R: oio::BlockingPage> oio::BlockingPage for MinitraceWrapper<R> {
     fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
-        let _span = Span::enter_with_parent(PageOperation::BlockingNext.into_static(), &self.span);
+        let _g = self.span.set_local_parent();
+        let _span = LocalSpan::enter_with_local_parent(PageOperation::BlockingNext.into_static());
         self.inner.next()
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/oteltrace.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/oteltrace.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/retry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/throttle.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/throttle.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/timeout.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/timeout.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.38.1/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/lib.rs` & `opendal-0.38.1/local_dependencies/opendal/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
     /// This is not a real test case.
     ///
     /// We assert our public structs here to make sure we don't introduce
     /// unexpected struct/enum size change.
     #[test]
     fn assert_size() {
         assert_eq!(24, size_of::<Operator>());
-        assert_eq!(240, size_of::<Entry>());
-        assert_eq!(216, size_of::<Metadata>());
+        assert_eq!(264, size_of::<Entry>());
+        assert_eq!(240, size_of::<Metadata>());
         assert_eq!(1, size_of::<EntryMode>());
         assert_eq!(24, size_of::<Scheme>());
     }
 
     /// This is used to make sure our public API implement Send + Sync
     trait AssertSendSync: Send + Sync {}
     impl AssertSendSync for Entry {}
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         }
 
         Ok(())
     }
 
     /// Consume the response to bytes.
     ///
-    /// Borrowed from hyper's [`to_bytes`](https://docs.rs/hyper/latest/hyper/body/fn.to_bytes.html).
+    /// This code is Inspired from hyper's [`to_bytes`](https://docs.rs/hyper/latest/hyper/body/fn.to_bytes.html).
     pub async fn bytes(mut self) -> Result<Bytes> {
         use oio::ReadExt;
 
         // If there's only 1 chunk, we can just return Buf::to_bytes()
         let mut first = if let Some(buf) = self.next().await {
             buf?
         } else {
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/multipart.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/multipart.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/append.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/append.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             SeekFrom::Current(n) => (self.pos as i64, n),
         };
 
         let n = match base.checked_add(amt) {
             Some(n) if n >= 0 => n as u64,
             _ => {
                 return Poll::Ready(Err(Error::new(
-                    ErrorKind::Unexpected,
+                    ErrorKind::InvalidInput,
                     "invalid seek to a negative or overflowing position",
                 )))
             }
         };
         self.pos = n;
         Poll::Ready(Ok(n))
     }
@@ -123,15 +123,15 @@
             SeekFrom::Current(n) => (self.pos as i64, n),
         };
 
         let n = match base.checked_add(amt) {
             Some(n) if n >= 0 => n as u64,
             _ => {
                 return Err(Error::new(
-                    ErrorKind::Unexpected,
+                    ErrorKind::InvalidInput,
                     "invalid seek to a negative or overflowing position",
                 ))
             }
         };
         self.pos = n;
         Ok(n)
     }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files 6% similar despite different names*

```diff
@@ -86,29 +86,29 @@
             SeekFrom::Start(n) => (self.start as i64, n as i64),
             SeekFrom::End(n) => (self.end as i64, n),
             SeekFrom::Current(n) => (self.offset as i64, n),
         };
 
         match base.checked_add(offset) {
             Some(n) if n < 0 => Err(Error::new(
-                ErrorKind::Unexpected,
+                ErrorKind::InvalidInput,
                 "invalid seek to a negative or overflowing position",
             )),
             Some(n) => {
                 let cur = self.inner.seek(SeekFrom::Start(n as u64)).map_err(|err| {
                     Error::new(ErrorKind::Unexpected, "seek data from FdReader")
                         .with_context("source", "FdReader")
                         .set_source(err)
                 })?;
 
                 self.offset = cur;
                 Ok(self.offset - self.start)
             }
             None => Err(Error::new(
-                ErrorKind::Unexpected,
+                ErrorKind::InvalidInput,
                 "invalid seek to a negative or overflowing position",
             )),
         }
     }
 
     fn next(&mut self) -> Option<Result<Bytes>> {
         Some(Err(Error::new(
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             SeekFrom::Current(n) => (self.cur as i64, n),
         };
 
         let n = match base.checked_add(amt) {
             Some(n) if n >= 0 => n as u64,
             _ => {
                 return Err(Error::new(
-                    ErrorKind::Unexpected,
+                    ErrorKind::InvalidInput,
                     "invalid seek to a negative or overflowing position",
                 ))
             }
         };
         Ok(n)
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             SeekFrom::Start(n) => (self.start as i64, n as i64),
             SeekFrom::End(n) => (self.end as i64, n),
             SeekFrom::Current(n) => (self.offset as i64, n),
         };
 
         match base.checked_add(offset) {
             Some(n) if n < 0 => Poll::Ready(Err(Error::new(
-                ErrorKind::Unexpected,
+                ErrorKind::InvalidInput,
                 "invalid seek to a negative or overflowing position",
             ))),
             Some(n) => {
                 let cur =
                     ready!(Pin::new(&mut self.inner).poll_seek(cx, SeekFrom::Start(n as u64)))
                         .map_err(|err| {
                             Error::new(ErrorKind::Unexpected, "seek data from FdReader")
@@ -105,15 +105,15 @@
                                 .set_source(err)
                         })?;
 
                 self.offset = cur;
                 Poll::Ready(Ok(self.offset - self.start))
             }
             None => Poll::Ready(Err(Error::new(
-                ErrorKind::Unexpected,
+                ErrorKind::InvalidInput,
                 "invalid seek to a negative or overflowing position",
             ))),
         }
     }
 
     fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<bytes::Bytes>>> {
         let _ = cx;
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_reader.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_stream.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/from_futures_stream.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_stream/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_stream/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files 2% similar despite different names*

```diff
@@ -188,32 +188,32 @@
 /// Extension of [`Read`] to make it easier for use.
 pub trait ReadExt: Read {
     /// Build a future for `poll_read`.
     fn read<'a>(&'a mut self, buf: &'a mut [u8]) -> ReadFuture<'a, Self> {
         ReadFuture {
             reader: self,
             buf,
-            _pin: PhantomPinned::default(),
+            _pin: PhantomPinned,
         }
     }
 
     /// Build a future for `poll_seek`.
     fn seek(&mut self, pos: io::SeekFrom) -> SeekFuture<'_, Self> {
         SeekFuture {
             reader: self,
             pos,
-            _pin: PhantomPinned::default(),
+            _pin: PhantomPinned,
         }
     }
 
     /// Build a future for `poll_next`
     fn next(&mut self) -> NextFuture<'_, Self> {
         NextFuture {
             reader: self,
-            _pin: PhantomPinned::default(),
+            _pin: PhantomPinned,
         }
     }
 }
 
 #[pin_project]
 pub struct ReadFuture<'a, R: Read + Unpin + ?Sized> {
     reader: &'a mut R,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/stream.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/stream.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/operation.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/ops.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/ops.rs`

 * *Files 4% similar despite different names*

```diff
@@ -36,20 +36,35 @@
     }
 }
 
 /// Args for `delete` operation.
 ///
 /// The path must be normalized.
 #[derive(Debug, Clone, Default)]
-pub struct OpDelete {}
+pub struct OpDelete {
+    version: Option<String>,
+}
 
 impl OpDelete {
     /// Create a new `OpDelete`.
     pub fn new() -> Self {
-        Self {}
+        Self::default()
+    }
+}
+
+impl OpDelete {
+    /// Change the version of this delete operation.
+    pub fn with_version(mut self, version: &str) -> Self {
+        self.version = Some(version.into());
+        self
+    }
+
+    /// Get the version of this delete operation.
+    pub fn version(&self) -> Option<&str> {
+        self.version.as_deref()
     }
 }
 
 /// Args for `list` operation.
 #[derive(Debug, Clone)]
 pub struct OpList {
     /// The limit passed to underlying service to specify the max results
@@ -225,14 +240,15 @@
 #[derive(Debug, Clone, Default)]
 pub struct OpRead {
     br: BytesRange,
     if_match: Option<String>,
     if_none_match: Option<String>,
     override_cache_control: Option<String>,
     override_content_disposition: Option<String>,
+    version: Option<String>,
 }
 
 impl OpRead {
     /// Create a default `OpRead` which will read whole content of path.
     pub fn new() -> Self {
         Self::default()
     }
@@ -288,21 +304,33 @@
         self
     }
 
     /// Get If-None-Match from option
     pub fn if_none_match(&self) -> Option<&str> {
         self.if_none_match.as_deref()
     }
+
+    /// Set the version of the option
+    pub fn with_version(mut self, version: &str) -> Self {
+        self.version = Some(version.to_string());
+        self
+    }
+
+    /// Get version from option
+    pub fn version(&self) -> Option<&str> {
+        self.version.as_deref()
+    }
 }
 
 /// Args for `stat` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpStat {
     if_match: Option<String>,
     if_none_match: Option<String>,
+    version: Option<String>,
 }
 
 impl OpStat {
     /// Create a new `OpStat`.
     pub fn new() -> Self {
         Self::default()
     }
@@ -324,14 +352,25 @@
         self
     }
 
     /// Get If-None-Match from option
     pub fn if_none_match(&self) -> Option<&str> {
         self.if_none_match.as_deref()
     }
+
+    /// Set the version of the option
+    pub fn with_version(mut self, version: &str) -> Self {
+        self.version = Some(version.to_string());
+        self
+    }
+
+    /// Get version from option
+    pub fn version(&self) -> Option<&str> {
+        self.version.as_deref()
+    }
 }
 
 /// Args for `write` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpWrite {
     content_length: Option<u64>,
     content_type: Option<String>,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/path.rs`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,14 @@
             name
         }
         None => path,
     }
 }
 
 /// Get parent from path.
-#[allow(dead_code)]
 pub fn get_parent(path: &str) -> &str {
     if path == "/" {
         return "/";
     }
 
     if !path.ends_with('/') {
         // The idx of first `/` if path in reserve order.
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.38.1/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/appender.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -527,14 +527,15 @@
                 read_can_next: true,
                 read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
                 read_with_override_content_disposition: true,
 
                 write: true,
+                write_can_sink: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
 
                 append: true,
                 append_with_cache_control: true,
                 append_with_content_type: true,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
         self.send(req).await
     }
 
     pub fn azblob_put_blob_request(
         &self,
         path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -33,25 +33,22 @@
     path: String,
 }
 
 impl AzblobWriter {
     pub fn new(core: Arc<AzblobCore>, op: OpWrite, path: String) -> Self {
         AzblobWriter { core, op, path }
     }
-}
 
-#[async_trait]
-impl oio::Write for AzblobWriter {
-    async fn write(&mut self, bs: Bytes) -> Result<()> {
+    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
         let mut req = self.core.azblob_put_blob_request(
             &self.path,
-            Some(bs.len()),
+            Some(size),
             self.op.content_type(),
             self.op.cache_control(),
-            AsyncBody::Bytes(bs),
+            body,
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
@@ -60,20 +57,25 @@
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
+}
+
+#[async_trait]
+impl oio::Write for AzblobWriter {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        self.write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
+            .await
+    }
 
-    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "Write::sink is not supported",
-        ))
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.write_oneshot(size, AsyncBody::Stream(s)).await
     }
 
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cacache/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cacache/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cacache/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/cacache/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cacache/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cacache/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cos/appender.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cos/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cos/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cos/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,15 @@
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
+                write_can_sink: true,
                 write_with_content_type: true,
                 write_with_cache_control: true,
 
                 append: true,
                 append_with_cache_control: true,
                 append_with_content_disposition: true,
                 append_with_content_type: true,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cos/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cos/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         Ok(req)
     }
 
     pub fn cos_put_object_request(
         &self,
         path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cos/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/cos/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cos/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cos/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cos/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cos/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cos/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cos/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/cos/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files 9% similar despite different names*

```diff
@@ -17,41 +17,38 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::CosCore;
+use super::core::ObsCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct CosWriter {
-    core: Arc<CosCore>,
+pub struct ObsWriter {
+    core: Arc<ObsCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl CosWriter {
-    pub fn new(core: Arc<CosCore>, op: OpWrite, path: String) -> Self {
-        CosWriter { core, op, path }
+impl ObsWriter {
+    pub fn new(core: Arc<ObsCore>, op: OpWrite, path: String) -> Self {
+        ObsWriter { core, op, path }
     }
-}
 
-#[async_trait]
-impl oio::Write for CosWriter {
-    async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.cos_put_object_request(
+    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
+        let mut req = self.core.obs_put_object_request(
             &self.path,
-            Some(bs.len()),
+            Some(size),
             self.op.content_type(),
             self.op.cache_control(),
-            AsyncBody::Bytes(bs),
+            body,
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
@@ -60,20 +57,25 @@
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
+}
+
+#[async_trait]
+impl oio::Write for ObsWriter {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        self.write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
+            .await
+    }
 
-    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "Write::sink is not supported",
-        ))
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.write_oneshot(size, AsyncBody::Stream(s)).await
     }
 
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files 24% similar despite different names*

```diff
@@ -11,83 +11,67 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::fmt::Debug;
-use std::sync::Arc;
+use std::str;
+use std::str::FromStr;
+use std::vec::IntoIter;
 
 use async_trait::async_trait;
-use http::StatusCode;
+use suppaftp::list::File;
 
-use super::core::DropboxCore;
-use super::error::parse_error;
-use super::writer::DropboxWriter;
 use crate::raw::*;
 use crate::*;
 
-#[derive(Clone, Debug)]
-pub struct DropboxBackend {
-    pub core: Arc<DropboxCore>,
+pub struct FtpPager {
+    path: String,
+    size: usize,
+    file_iter: IntoIter<String>,
 }
 
-#[async_trait]
-impl Accessor for DropboxBackend {
-    type Reader = IncomingAsyncBody;
-    type BlockingReader = ();
-    type Writer = DropboxWriter;
-    type BlockingWriter = ();
-    type Pager = ();
-    type BlockingPager = ();
-    type Appender = ();
-
-    fn info(&self) -> AccessorInfo {
-        let mut ma = AccessorInfo::default();
-        ma.set_scheme(Scheme::Dropbox)
-            .set_root(&self.core.root)
-            .set_capability(Capability {
-                read: true,
-                write: true,
-                delete: true,
-                ..Default::default()
-            });
-        ma
-    }
-
-    async fn read(&self, path: &str, _args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.core.dropbox_get(path).await?;
-        let status = resp.status();
-        match status {
-            StatusCode::OK => {
-                let meta = parse_into_metadata(path, resp.headers())?;
-                Ok((RpRead::with_metadata(meta), resp.into_body()))
-            }
-            _ => Err(parse_error(resp).await?),
-        }
-    }
-
-    async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.content_length().is_none() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "write without content length is not supported",
-            ));
+impl FtpPager {
+    pub fn new(path: &str, files: Vec<String>, limit: Option<usize>) -> Self {
+        Self {
+            path: path.to_string(),
+            size: limit.unwrap_or(1000),
+            file_iter: files.into_iter(),
         }
-        Ok((
-            RpWrite::default(),
-            DropboxWriter::new(self.core.clone(), args, String::from(path)),
-        ))
     }
+}
 
-    async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.core.dropbox_delete(path).await?;
-
-        let status = resp.status();
+#[async_trait]
+impl oio::Page for FtpPager {
+    async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
+        let mut oes: Vec<oio::Entry> = Vec::with_capacity(self.size);
+
+        for _ in 0..self.size {
+            let de = match self.file_iter.next() {
+                Some(file_str) => File::from_str(file_str.as_str()).map_err(|e| {
+                    Error::new(ErrorKind::Unexpected, "parse file from response").set_source(e)
+                })?,
+                None => break,
+            };
+
+            let path = self.path.to_string() + de.name();
+
+            let d = if de.is_file() {
+                oio::Entry::new(
+                    &path,
+                    Metadata::new(EntryMode::FILE)
+                        .with_content_length(de.size() as u64)
+                        .with_last_modified(de.modified().into()),
+                )
+            } else if de.is_directory() {
+                oio::Entry::new(&format!("{}/", &path), Metadata::new(EntryMode::DIR))
+            } else {
+                oio::Entry::new(&path, Metadata::new(EntryMode::Unknown))
+            };
 
-        match status {
-            StatusCode::OK => Ok(RpDelete::default()),
-            _ => Err(parse_error(resp).await?),
+            oes.push(d)
         }
+
+        Ok(if oes.is_empty() { None } else { Some(oes) })
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/builder.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/builder.rs`

 * *Files 12% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
-use std::sync::Arc;
 
-use super::backend::DropboxBackend;
-use super::core::DropboxCore;
-use crate::raw::*;
+use log::debug;
+
+use super::backend::GdriveBackend;
+use crate::raw::normalize_root;
+use crate::raw::HttpClient;
+use crate::Scheme;
 use crate::*;
 
-/// [Dropbox](https://www.dropbox.com/) backend support.
+/// [GoogleDrive](https://drive.google.com/) backend support.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
@@ -43,58 +45,63 @@
 ///
 ///
 /// # Configuration
 ///
 /// - `access_token`: set the access_token for google drive api
 /// - `root`: Set the work directory for backend
 ///
-/// You can refer to [`DropboxBuilder`]'s docs for more information
+/// You can refer to [`GdriveBuilder`]'s docs for more information
 ///
 /// # Example
 ///
 /// ## Via Builder
 ///
-/// ```
+/// ```no_run
 /// use anyhow::Result;
-/// use opendal::raw::OpWrite;
-/// use opendal::services::Dropbox;
+/// use opendal::services::Gdrive;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     // create backend builder
-///     let mut builder = Dropbox::default();
-///     builder.access_token("<token>");
+///     let mut builder = Gdrive::default();
+///
+///     builder.access_token("xxx").root("/path/to/root");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
+///
+///     let write = op.write("abc.txt", "who are you").await?;
+///     let read = op.read("abc.txt").await?;
+///     let s = String::from_utf8(read).unwrap();
+///     println!("{}", s);
+///     let delete = op.delete("abc.txt").await?;
 ///     Ok(())
 /// }
 /// ```
-
 #[derive(Default)]
-pub struct DropboxBuilder {
+pub struct GdriveBuilder {
     access_token: Option<String>,
     root: Option<String>,
     http_client: Option<HttpClient>,
 }
 
-impl Debug for DropboxBuilder {
+impl Debug for GdriveBuilder {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("Builder").finish()
+        f.debug_struct("Backend").field("root", &self.root).finish()
     }
 }
 
-impl DropboxBuilder {
+impl GdriveBuilder {
     /// default: no access token, which leads to failure
     pub fn access_token(&mut self, access_token: &str) -> &mut Self {
         self.access_token = Some(access_token.to_string());
         self
     }
 
-    /// default: no root path, which leads to failure
+    /// Set root path of GoogleDrive folder.
     pub fn root(&mut self, root: &str) -> &mut Self {
         self.root = Some(root.to_string());
         self
     }
 
     /// Specify the http client that used by this service.
     ///
@@ -104,46 +111,40 @@
     /// during minor updates.
     pub fn http_client(&mut self, http_client: HttpClient) -> &mut Self {
         self.http_client = Some(http_client);
         self
     }
 }
 
-impl Builder for DropboxBuilder {
-    const SCHEME: Scheme = Scheme::Dropbox;
-    type Accessor = DropboxBackend;
+impl Builder for GdriveBuilder {
+    const SCHEME: Scheme = Scheme::Gdrive;
+
+    type Accessor = GdriveBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
         let mut builder = Self::default();
+
+        map.get("root").map(|v| builder.root(v));
         map.get("access_token").map(|v| builder.access_token(v));
+
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         let root = normalize_root(&self.root.take().unwrap_or_default());
+        debug!("backend use root {}", root);
+
         let client = if let Some(client) = self.http_client.take() {
             client
         } else {
             HttpClient::new().map_err(|err| {
                 err.with_operation("Builder::build")
-                    .with_context("service", Scheme::Dropbox)
+                    .with_context("service", Scheme::Gdrive)
             })?
         };
-        let token = match self.access_token.clone() {
-            Some(access_token) => access_token,
-            None => {
-                return Err(Error::new(
-                    ErrorKind::ConfigInvalid,
-                    "access_token is required",
-                ))
-            }
-        };
 
-        Ok(DropboxBackend {
-            core: Arc::new(DropboxCore {
-                root,
-                token,
-                client,
-            }),
-        })
+        match self.access_token.clone() {
+            Some(access_token) => Ok(GdriveBackend::new(root, access_token, client)),
+            None => Err(Error::new(ErrorKind::ConfigInvalid, "access_token not set")),
+        }
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files 27% similar despite different names*

```diff
@@ -11,140 +11,117 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::default::Default;
-use std::fmt::Debug;
-use std::fmt::Formatter;
-
-use bytes::Bytes;
-use http::header;
-use http::request::Builder;
-use http::Request;
-use http::Response;
-use serde::Deserialize;
-use serde::Serialize;
-
-use crate::raw::build_rooted_abs_path;
-use crate::raw::new_json_serialize_error;
-use crate::raw::new_request_build_error;
-use crate::raw::AsyncBody;
-use crate::raw::HttpClient;
-use crate::raw::IncomingAsyncBody;
-use crate::types::Result;
-
-pub struct DropboxCore {
-    pub token: String,
-    pub client: HttpClient,
-    pub root: String,
-}
+use std::path::Path;
+use std::path::PathBuf;
+
+use async_trait::async_trait;
 
-impl Debug for DropboxCore {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        let mut de = f.debug_struct("DropboxCore");
-        de.finish()
+use super::error::parse_io_error;
+use crate::raw::*;
+use crate::EntryMode;
+use crate::Metadata;
+use crate::Result;
+
+pub struct FsPager<P> {
+    root: PathBuf,
+
+    size: usize,
+    rd: P,
+}
+
+impl<P> FsPager<P> {
+    pub fn new(root: &Path, rd: P, limit: Option<usize>) -> Self {
+        Self {
+            root: root.to_owned(),
+            size: limit.unwrap_or(1000),
+            rd,
+        }
     }
 }
 
-impl DropboxCore {
-    pub async fn dropbox_get(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let url: String = "https://content.dropboxapi.com/2/files/download".to_string();
-        let download_args = DropboxDownloadArgs {
-            path: build_rooted_abs_path(&self.root, path),
-        };
-        let request_payload =
-            serde_json::to_string(&download_args).map_err(new_json_serialize_error)?;
-        let request = self
-            .build_auth_header(Request::post(&url))
-            .header("Dropbox-API-Arg", request_payload)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-        self.client.send(request).await
-    }
+#[async_trait]
+impl oio::Page for FsPager<tokio::fs::ReadDir> {
+    async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
+        let mut oes: Vec<oio::Entry> = Vec::with_capacity(self.size);
+
+        for _ in 0..self.size {
+            let de = match self.rd.next_entry().await.map_err(parse_io_error)? {
+                Some(de) => de,
+                None => break,
+            };
+
+            let entry_path = de.path();
+            let rel_path = normalize_path(
+                &entry_path
+                    .strip_prefix(&self.root)
+                    .expect("cannot fail because the prefix is iterated")
+                    .to_string_lossy()
+                    .replace('\\', "/"),
+            );
+
+            // On Windows and most Unix platforms this function is free
+            // (no extra system calls needed), but some Unix platforms may
+            // require the equivalent call to symlink_metadata to learn about
+            // the target file type.
+            let file_type = de.file_type().await.map_err(parse_io_error)?;
+
+            let d = if file_type.is_file() {
+                oio::Entry::new(&rel_path, Metadata::new(EntryMode::FILE))
+            } else if file_type.is_dir() {
+                // Make sure we are returning the correct path.
+                oio::Entry::new(&format!("{rel_path}/"), Metadata::new(EntryMode::DIR))
+            } else {
+                oio::Entry::new(&rel_path, Metadata::new(EntryMode::Unknown))
+            };
 
-    pub async fn dropbox_update(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let url = "https://content.dropboxapi.com/2/files/upload".to_string();
-        let args = DropboxUploadArgs {
-            path: build_rooted_abs_path(&self.root, path),
-            ..Default::default()
-        };
-        let mut request_builder = Request::post(&url);
-        if let Some(size) = size {
-            request_builder = request_builder.header(header::CONTENT_LENGTH, size);
+            oes.push(d)
         }
-        if let Some(mime) = content_type {
-            request_builder = request_builder.header(header::CONTENT_TYPE, mime);
-        }
-        let request = self
-            .build_auth_header(request_builder)
-            .header(
-                "Dropbox-API-Arg",
-                serde_json::to_string(&args).map_err(new_json_serialize_error)?,
-            )
-            .body(body)
-            .map_err(new_request_build_error)?;
-
-        self.client.send(request).await
-    }
 
-    pub async fn dropbox_delete(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let url = "https://api.dropboxapi.com/2/files/delete_v2".to_string();
-        let args = DropboxDeleteArgs {
-            path: build_rooted_abs_path(&self.root, path),
-        };
-
-        let bs = Bytes::from(serde_json::to_string(&args).map_err(new_json_serialize_error)?);
-
-        let request = self
-            .build_auth_header(Request::post(&url))
-            .header(header::CONTENT_TYPE, "application/json")
-            .body(AsyncBody::Bytes(bs))
-            .map_err(new_request_build_error)?;
-        self.client.send(request).await
+        Ok(if oes.is_empty() { None } else { Some(oes) })
     }
-
-    fn build_auth_header(&self, mut req: Builder) -> Builder {
-        let auth_header_content = format!("Bearer {}", self.token);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
-        req
-    }
-}
-
-#[derive(Clone, Debug, Deserialize, Serialize)]
-struct DropboxDownloadArgs {
-    path: String,
 }
 
-#[derive(Clone, Debug, Deserialize, Serialize)]
-struct DropboxUploadArgs {
-    path: String,
-    mode: String,
-    mute: bool,
-    autorename: bool,
-    strict_conflict: bool,
-}
+impl oio::BlockingPage for FsPager<std::fs::ReadDir> {
+    fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
+        let mut oes: Vec<oio::Entry> = Vec::with_capacity(self.size);
+
+        for _ in 0..self.size {
+            let de = match self.rd.next() {
+                Some(de) => de.map_err(parse_io_error)?,
+                None => break,
+            };
+
+            let entry_path = de.path();
+            let rel_path = normalize_path(
+                &entry_path
+                    .strip_prefix(&self.root)
+                    .expect("cannot fail because the prefix is iterated")
+                    .to_string_lossy()
+                    .replace('\\', "/"),
+            );
+
+            // On Windows and most Unix platforms this function is free
+            // (no extra system calls needed), but some Unix platforms may
+            // require the equivalent call to symlink_metadata to learn about
+            // the target file type.
+            let file_type = de.file_type().map_err(parse_io_error)?;
+
+            let d = if file_type.is_file() {
+                oio::Entry::new(&rel_path, Metadata::new(EntryMode::FILE))
+            } else if file_type.is_dir() {
+                // Make sure we are returning the correct path.
+                oio::Entry::new(&format!("{rel_path}/"), Metadata::new(EntryMode::DIR))
+            } else {
+                oio::Entry::new(&rel_path, Metadata::new(EntryMode::Unknown))
+            };
 
-#[derive(Clone, Debug, Deserialize, Serialize)]
-struct DropboxDeleteArgs {
-    path: String,
-}
-
-impl Default for DropboxUploadArgs {
-    fn default() -> Self {
-        DropboxUploadArgs {
-            mode: "overwrite".to_string(),
-            path: "".to_string(),
-            mute: true,
-            autorename: false,
-            strict_conflict: false,
+            oes.push(d)
         }
+
+        Ok(if oes.is_empty() { None } else { Some(oes) })
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/error.rs`

 * *Files 25% similar despite different names*

```diff
@@ -13,67 +13,74 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use http::Response;
 use http::StatusCode;
+use http::Uri;
 use serde::Deserialize;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
 #[derive(Default, Debug, Deserialize)]
 #[serde(default)]
-struct DropboxError {
-    error_summary: String,
-    error: DropboxErrorDetail,
-}
-
-#[derive(Default, Debug, Deserialize)]
-#[serde(default)]
-struct DropboxErrorDetail {
-    #[serde(rename(deserialize = ".tag"))]
-    tag: String,
+pub struct DropboxErrorResponse {
+    pub error_summary: String,
 }
 
 /// Parse error response into Error.
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
-    let (kind, retryable) = match parts.status {
+    let (mut kind, mut retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
-    let dropbox_error =
-        serde_json::from_slice::<DropboxError>(&bs).map_err(new_json_deserialize_error);
-    match dropbox_error {
-        Ok(dropbox_error) => {
-            let mut err = Error::new(kind, dropbox_error.error_summary.as_ref())
-                .with_context("response", format!("{parts:?}"));
-
-            if retryable {
-                err = err.set_temporary();
-            }
-
-            Ok(err)
-        }
-        Err(_err) => {
-            let mut err = Error::new(kind, &String::from_utf8_lossy(&bs))
-                .with_context("response", format!("{parts:?}"));
-
-            if retryable {
-                err = err.set_temporary();
-            }
 
-            Ok(err)
-        }
+    let (message, dropbox_err) = serde_json::from_slice::<DropboxErrorResponse>(&bs)
+        .map(|dropbox_err| (format!("{dropbox_err:?}"), Some(dropbox_err)))
+        .unwrap_or_else(|_| (String::from_utf8_lossy(&bs).into_owned(), None));
+
+    if let Some(dropbox_err) = dropbox_err {
+        (kind, retryable) =
+            parse_dropbox_error_summary(&dropbox_err.error_summary).unwrap_or((kind, retryable));
+    }
+
+    let mut err = Error::new(kind, &message).with_context("response", format!("{parts:?}"));
+
+    if retryable {
+        err = err.set_temporary();
+    }
+
+    if let Some(uri) = parts.extensions.get::<Uri>() {
+        err = err.with_context("uri", uri.to_string());
+    }
+
+    Ok(err)
+}
+
+/// We cannot get the error type from the response header when the status code is 409.
+/// Because Dropbox API v2 will put error summary in the response body,
+/// we need to parse it to get the correct error type and then error kind.
+///
+/// See <https://www.dropbox.com/developers/documentation/http/documentation#error-handling>
+pub fn parse_dropbox_error_summary(summary: &str) -> Option<(ErrorKind, bool)> {
+    if summary.starts_with("path/not_found") || summary.starts_with("path_lookup/not_found") {
+        Some((ErrorKind::NotFound, false))
+    } else if summary.starts_with("path/conflict") {
+        Some((ErrorKind::AlreadyExists, false))
+    } else if summary.starts_with("too_many_write_operations") {
+        Some((ErrorKind::RateLimited, true))
+    } else {
+        None
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/dropbox/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/dropbox/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/fs/appender.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/fs/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,15 @@
                 stat: true,
 
                 read: true,
                 read_can_seek: true,
                 read_with_range: true,
 
                 write: true,
+                write_can_sink: true,
                 write_without_content_length: true,
                 create_dir: true,
                 delete: true,
 
                 append: true,
 
                 list: true,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/fs/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/fs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 use std::io::Seek;
 use std::io::SeekFrom;
 use std::io::Write;
 use std::path::PathBuf;
 
 use async_trait::async_trait;
 use bytes::Bytes;
+use futures::StreamExt;
 use tokio::io::AsyncSeekExt;
 use tokio::io::AsyncWriteExt;
 
 use super::error::parse_io_error;
 use crate::raw::*;
 use crate::*;
 
@@ -60,19 +61,26 @@
             .map_err(parse_io_error)?;
         self.f.write_all(&bs).await.map_err(parse_io_error)?;
         self.pos += bs.len() as u64;
 
         Ok(())
     }
 
-    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "Write::sink is not supported",
-        ))
+    async fn sink(&mut self, _size: u64, mut s: oio::Streamer) -> Result<()> {
+        while let Some(bs) = s.next().await {
+            let bs = bs?;
+            self.f
+                .seek(SeekFrom::Start(self.pos))
+                .await
+                .map_err(parse_io_error)?;
+            self.f.write_all(&bs).await.map_err(parse_io_error)?;
+            self.pos += bs.len() as u64;
+        }
+
+        Ok(())
     }
 
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
         ))
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/pager.rs`

 * *Files 22% similar despite different names*

```diff
@@ -11,67 +11,75 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::str;
-use std::str::FromStr;
-use std::vec::IntoIter;
+use std::pin::Pin;
 
 use async_trait::async_trait;
-use suppaftp::list::File;
-
-use crate::raw::*;
-use crate::*;
-
-pub struct FtpPager {
-    path: String,
-    size: usize,
-    file_iter: IntoIter<String>,
+use futures::StreamExt;
+use openssh_sftp_client::fs::DirEntry;
+use openssh_sftp_client::fs::ReadDir;
+
+use crate::raw::oio;
+use crate::Result;
+
+pub struct SftpPager {
+    dir: Pin<Box<ReadDir>>,
+    prefix: String,
+    limit: usize,
 }
 
-impl FtpPager {
-    pub fn new(path: &str, files: Vec<String>, limit: Option<usize>) -> Self {
-        Self {
-            path: path.to_string(),
-            size: limit.unwrap_or(1000),
-            file_iter: files.into_iter(),
+impl SftpPager {
+    pub fn new(dir: ReadDir, path: String, limit: Option<usize>) -> Self {
+        let prefix = if path == "/" { "".to_owned() } else { path };
+
+        let limit = limit.unwrap_or(usize::MAX);
+
+        SftpPager {
+            dir: Box::pin(dir),
+            prefix,
+            limit,
         }
     }
 }
 
 #[async_trait]
-impl oio::Page for FtpPager {
+impl oio::Page for SftpPager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
-        let mut oes: Vec<oio::Entry> = Vec::with_capacity(self.size);
+        if self.limit == 0 {
+            return Ok(None);
+        }
 
-        for _ in 0..self.size {
-            let de = match self.file_iter.next() {
-                Some(file_str) => File::from_str(file_str.as_str()).map_err(|e| {
-                    Error::new(ErrorKind::Unexpected, "parse file from response").set_source(e)
-                })?,
-                None => break,
-            };
-
-            let path = self.path.to_string() + de.name();
-
-            let d = if de.is_file() {
-                oio::Entry::new(
-                    &path,
-                    Metadata::new(EntryMode::FILE)
-                        .with_content_length(de.size() as u64)
-                        .with_last_modified(de.modified().into()),
-                )
-            } else if de.is_directory() {
-                oio::Entry::new(&format!("{}/", &path), Metadata::new(EntryMode::DIR))
-            } else {
-                oio::Entry::new(&path, Metadata::new(EntryMode::Unknown))
-            };
+        let item = self.dir.next().await;
 
-            oes.push(d)
+        match item {
+            Some(Ok(e)) => {
+                if e.filename().to_str() == Some(".") || e.filename().to_str() == Some("..") {
+                    self.next().await
+                } else {
+                    self.limit -= 1;
+                    Ok(Some(vec![map_entry(self.prefix.as_str(), e.clone())]))
+                }
+            }
+            Some(Err(e)) => Err(e.into()),
+            None => Ok(None),
         }
-
-        Ok(if oes.is_empty() { None } else { Some(oes) })
     }
 }
+
+fn map_entry(prefix: &str, value: DirEntry) -> oio::Entry {
+    let path = format!(
+        "{}{}{}",
+        prefix,
+        value.filename().to_str().unwrap(),
+        if value.file_type().unwrap().is_dir() {
+            "/"
+        } else {
+            ""
+        }
+    );
+
+    oio::Entry::new(path.as_str(), value.metadata().into())
+}
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -414,14 +414,15 @@
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
+                write_can_sink: true,
                 write_with_content_type: true,
                 write_without_content_length: true,
                 delete: true,
                 copy: true,
 
                 list: true,
                 list_with_limit: true,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub fn gcs_insert_object_request(
         &self,
         path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
             "{}/upload/storage/v1/b/{}/o?uploadType={}&name={}",
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -48,20 +48,20 @@
             location: None,
             written: 0,
             buffer: oio::VectorCursor::new(),
             write_fixed_size,
         }
     }
 
-    async fn write_oneshot(&self, bs: Bytes) -> Result<()> {
+    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
         let mut req = self.core.gcs_insert_object_request(
             &percent_encode_path(&self.path),
-            Some(bs.len()),
+            Some(size),
             self.op.content_type(),
-            AsyncBody::Bytes(bs),
+            body,
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
@@ -121,15 +121,17 @@
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let location = match &self.location {
             Some(location) => location,
             None => {
                 if self.op.content_length().unwrap_or_default() == bs.len() as u64
                     && self.written == 0
                 {
-                    return self.write_oneshot(bs).await;
+                    return self
+                        .write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
+                        .await;
                 } else {
                     let location = self.initiate_upload().await?;
                     self.location = Some(location);
                     self.location.as_deref().unwrap()
                 }
             }
         };
@@ -158,19 +160,16 @@
                 // write is re-enter safe.
                 self.buffer.pop();
                 Err(e)
             }
         }
     }
 
-    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "Write::sink is not supported",
-        ))
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.write_oneshot(size, AsyncBody::Stream(s)).await
     }
 
     async fn abort(&mut self) -> Result<()> {
         let location = if let Some(location) = &self.location {
             location
         } else {
             return Ok(());
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/builder.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files 20% similar despite different names*

```diff
@@ -12,139 +12,134 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
-use std::fmt::Debug;
-use std::fmt::Formatter;
 
 use log::debug;
 
-use super::backend::GdriveBackend;
-use crate::raw::normalize_root;
-use crate::raw::HttpClient;
-use crate::Scheme;
+use super::backend::IpmfsBackend;
+use crate::raw::*;
 use crate::*;
 
-/// [GoogleDrive](https://drive.google.com/) backend support.
+/// IPFS file system support based on [IPFS MFS](https://docs.ipfs.tech/concepts/file-systems/) API.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
-/// - [x] delete
-/// - [ ] copy
-/// - [ ] create
-/// - [ ] list
-/// - [ ] rename
-///
-/// # Notes
-///
+/// - [x] list
+/// - [ ] ~~scan~~
+/// - [ ] presign
+/// - [ ] blocking
 ///
 /// # Configuration
 ///
-/// - `access_token`: set the access_token for google drive api
 /// - `root`: Set the work directory for backend
+/// - `endpoint`: Customizable endpoint setting
 ///
-/// You can refer to [`GdriveBuilder`]'s docs for more information
+/// You can refer to [`IpmfsBuilder`]'s docs for more information
 ///
 /// # Example
 ///
 /// ## Via Builder
 ///
 /// ```no_run
 /// use anyhow::Result;
-/// use opendal::services::Gdrive;
+/// use opendal::services::Ipmfs;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     // create backend builder
-///     let mut builder = Gdrive::default();
+///     let mut builder = Ipmfs::default();
 ///
-///     builder.access_token("xxx").root("/path/to/root");
+///     // set the storage bucket for OpenDAL
+///     builder.endpoint("http://127.0.0.1:5001");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
 ///
-///     let write = op.write("abc.txt", "who are you").await?;
-///     let read = op.read("abc.txt").await?;
-///     let s = String::from_utf8(read).unwrap();
-///     println!("{}", s);
-///     let delete = op.delete("abc.txt").await?;
 ///     Ok(())
 /// }
 /// ```
-#[derive(Default)]
-pub struct GdriveBuilder {
-    access_token: Option<String>,
+#[derive(Default, Debug)]
+pub struct IpmfsBuilder {
     root: Option<String>,
+    endpoint: Option<String>,
     http_client: Option<HttpClient>,
 }
 
-impl Debug for GdriveBuilder {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("Backend").field("root", &self.root).finish()
-    }
-}
+impl IpmfsBuilder {
+    /// Set root for ipfs.
+    pub fn root(&mut self, root: &str) -> &mut Self {
+        self.root = if root.is_empty() {
+            None
+        } else {
+            Some(root.to_string())
+        };
 
-impl GdriveBuilder {
-    /// default: no access token, which leads to failure
-    pub fn access_token(&mut self, access_token: &str) -> &mut Self {
-        self.access_token = Some(access_token.to_string());
         self
     }
 
-    /// Set root path of GoogleDrive folder.
-    pub fn root(&mut self, root: &str) -> &mut Self {
-        self.root = Some(root.to_string());
+    /// Set endpoint for ipfs.
+    ///
+    /// Default: http://localhost:5001
+    pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
+        self.endpoint = if endpoint.is_empty() {
+            None
+        } else {
+            Some(endpoint.to_string())
+        };
         self
     }
 
     /// Specify the http client that used by this service.
     ///
     /// # Notes
     ///
     /// This API is part of OpenDAL's Raw API. `HttpClient` could be changed
     /// during minor updates.
-    pub fn http_client(&mut self, http_client: HttpClient) -> &mut Self {
-        self.http_client = Some(http_client);
+    pub fn http_client(&mut self, client: HttpClient) -> &mut Self {
+        self.http_client = Some(client);
         self
     }
 }
 
-impl Builder for GdriveBuilder {
-    const SCHEME: Scheme = Scheme::Gdrive;
-
-    type Accessor = GdriveBackend;
+impl Builder for IpmfsBuilder {
+    const SCHEME: Scheme = Scheme::Ipmfs;
+    type Accessor = IpmfsBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
-        let mut builder = Self::default();
+        let mut builder = IpmfsBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
-        map.get("access_token").map(|v| builder.access_token(v));
+        map.get("endpoint").map(|v| builder.endpoint(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         let root = normalize_root(&self.root.take().unwrap_or_default());
         debug!("backend use root {}", root);
 
+        let endpoint = self
+            .endpoint
+            .clone()
+            .unwrap_or_else(|| "http://localhost:5001".to_string());
+
         let client = if let Some(client) = self.http_client.take() {
             client
         } else {
             HttpClient::new().map_err(|err| {
                 err.with_operation("Builder::build")
-                    .with_context("service", Scheme::Gdrive)
+                    .with_context("service", Scheme::Ipmfs)
             })?
         };
 
-        match self.access_token.clone() {
-            Some(access_token) => Ok(GdriveBackend::new(root, access_token, client)),
-            None => Err(Error::new(ErrorKind::ConfigInvalid, "access_token not set")),
-        }
+        debug!("backend build finished: {:?}", &self);
+        Ok(IpmfsBackend::new(root, client, endpoint))
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/gdrive/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/gdrive/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/docs.md`

 * *Files 16% similar despite different names*

```diff
@@ -63,14 +63,29 @@
 `CLASSPATH` is not set correctly or your hadoop installation is incorrect.
 
 To set `CLASSPATH`:
 ```shell
 export CLASSPATH=$(find $HADOOP_HOME -iname "*.jar" | xargs echo | tr ' ' ':'):${CLASSPATH}
 ```
 
+- If HDFS has High Availability (HA) enabled with multiple available NameNodes, some configuration is required:
+1. Obtain the entire HDFS config folder (usually located at HADOOP_HOME/etc/hadoop).
+2. Set the environment variable HADOOP_CONF_DIR to the path of this folder.
+```shell
+export HADOOP_CONF_DIR=<path of the config folder>
+```
+3. Append the HADOOP_CONF_DIR to the `CLASSPATH`
+```shell
+export CLASSPATH=$CLASSPATH:$HADOOP_CONF_DIR
+```
+4. Use the `cluster_name` specified in the `core-site.xml` file (located in the HADOOP_CONF_DIR folder) to replace namenode:port.
+
+```rust
+builder.name_node("hdfs://cluster_name");
+```
 ## Example
 
 ### Via Builder
 
 ```rust
 use std::sync::Arc;
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/http/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs`

 * *Files 22% similar despite different names*

```diff
@@ -13,133 +13,114 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
 
-use log::debug;
-
-use super::backend::IpmfsBackend;
-use crate::raw::*;
+use super::backend::VercelArtifactsBackend;
+use crate::raw::HttpClient;
+use crate::Scheme;
 use crate::*;
 
-/// IPFS file system support based on [IPFS MFS](https://docs.ipfs.tech/concepts/file-systems/) API.
+/// [Vercel Cache](https://vercel.com/docs/concepts/monorepos/remote-caching) backend support.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
+/// - [ ] stat
 /// - [x] read
 /// - [x] write
-/// - [x] list
+/// - [x] create_dir
+/// - [x] delete
+/// - [ ] ~~copy~~
+/// - [ ] ~~rename~~
+/// - [ ] ~~list~~
 /// - [ ] ~~scan~~
-/// - [ ] presign
+/// - [ ] ~~presign~~
 /// - [ ] blocking
 ///
+/// # Notes
 /// # Configuration
 ///
-/// - `root`: Set the work directory for backend
-/// - `endpoint`: Customizable endpoint setting
+/// - `access_token`: set the access_token for Rest API
 ///
-/// You can refer to [`IpmfsBuilder`]'s docs for more information
+/// You can refer to [`VercelArtifactsBuilder`]'s docs for more information
 ///
 /// # Example
 ///
 /// ## Via Builder
 ///
 /// ```no_run
 /// use anyhow::Result;
-/// use opendal::services::Ipmfs;
+/// use opendal::services::VercelArtifacts;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     // create backend builder
-///     let mut builder = Ipmfs::default();
+///     let mut builder = VercelArtifacts::default();
 ///
-///     // set the storage bucket for OpenDAL
-///     builder.endpoint("http://127.0.0.1:5001");
+///     builder.access_token("xxx");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
-///
 ///     Ok(())
 /// }
 /// ```
-#[derive(Default, Debug)]
-pub struct IpmfsBuilder {
-    root: Option<String>,
-    endpoint: Option<String>,
+#[derive(Default)]
+pub struct VercelArtifactsBuilder {
+    access_token: Option<String>,
     http_client: Option<HttpClient>,
 }
 
-impl IpmfsBuilder {
-    /// Set root for ipfs.
-    pub fn root(&mut self, root: &str) -> &mut Self {
-        self.root = if root.is_empty() {
-            None
-        } else {
-            Some(root.to_string())
-        };
-
-        self
-    }
-
-    /// Set endpoint for ipfs.
+impl VercelArtifactsBuilder {
+    /// set the bearer access token for Vercel
     ///
-    /// Default: http://localhost:5001
-    pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
-        self.endpoint = if endpoint.is_empty() {
-            None
-        } else {
-            Some(endpoint.to_string())
-        };
+    /// default: no access token, which leads to failure
+    pub fn access_token(&mut self, access_token: &str) -> &mut Self {
+        self.access_token = Some(access_token.to_string());
         self
     }
 
     /// Specify the http client that used by this service.
     ///
     /// # Notes
     ///
     /// This API is part of OpenDAL's Raw API. `HttpClient` could be changed
     /// during minor updates.
-    pub fn http_client(&mut self, client: HttpClient) -> &mut Self {
-        self.http_client = Some(client);
+    pub fn http_client(&mut self, http_client: HttpClient) -> &mut Self {
+        self.http_client = Some(http_client);
         self
     }
 }
 
-impl Builder for IpmfsBuilder {
-    const SCHEME: Scheme = Scheme::Ipmfs;
-    type Accessor = IpmfsBackend;
-
-    fn from_map(map: HashMap<String, String>) -> Self {
-        let mut builder = IpmfsBuilder::default();
+impl Builder for VercelArtifactsBuilder {
+    const SCHEME: Scheme = Scheme::VercelArtifacts;
 
-        map.get("root").map(|v| builder.root(v));
-        map.get("endpoint").map(|v| builder.endpoint(v));
+    type Accessor = VercelArtifactsBackend;
 
+    fn from_map(map: HashMap<String, String>) -> Self {
+        let mut builder = Self::default();
+        map.get("access_token").map(|v| builder.access_token(v));
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
-        let root = normalize_root(&self.root.take().unwrap_or_default());
-        debug!("backend use root {}", root);
-
-        let endpoint = self
-            .endpoint
-            .clone()
-            .unwrap_or_else(|| "http://localhost:5001".to_string());
-
         let client = if let Some(client) = self.http_client.take() {
             client
         } else {
             HttpClient::new().map_err(|err| {
                 err.with_operation("Builder::build")
-                    .with_context("service", Scheme::Ipmfs)
+                    .with_context("service", Scheme::VercelArtifacts)
             })?
         };
 
-        debug!("backend build finished: {:?}", &self);
-        Ok(IpmfsBackend::new(root, client, endpoint))
+        match self.access_token.clone() {
+            Some(access_token) => Ok(VercelArtifactsBackend {
+                access_token,
+                client,
+            }),
+            None => Err(Error::new(ErrorKind::ConfigInvalid, "access_token not set")),
+        }
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,14 @@
         let mut conn = self.conn().await?;
 
         conn.delete(&percent_encode_path(key)).await
     }
 }
 
 /// A `bb8::ManageConnection` for `memcache_async::ascii::Protocol`.
-///
-/// Most code is borrowed from [bb8-memcached](https://github.com/dqminh/bb8-memcached/blob/master/src/client.rs).
 #[derive(Clone, Debug)]
 struct MemcacheConnectionManager {
     address: String,
 }
 
 impl MemcacheConnectionManager {
     fn new(address: &str) -> Self {
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/mini_moka/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/mini_moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/mini_moka/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/mini_moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/obs/appender.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/obs/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,15 @@
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
+                write_can_sink: true,
                 write_with_content_type: true,
                 write_with_cache_control: true,
 
                 append: true,
                 append_with_cache_control: true,
                 append_with_content_type: true,
                 append_with_content_disposition: true,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         Ok(req)
     }
 
     pub fn obs_put_object_request(
         &self,
         path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/cos/writer.rs`

 * *Files 13% similar despite different names*

```diff
@@ -17,41 +17,38 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::ObsCore;
+use super::core::CosCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct ObsWriter {
-    core: Arc<ObsCore>,
+pub struct CosWriter {
+    core: Arc<CosCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl ObsWriter {
-    pub fn new(core: Arc<ObsCore>, op: OpWrite, path: String) -> Self {
-        ObsWriter { core, op, path }
+impl CosWriter {
+    pub fn new(core: Arc<CosCore>, op: OpWrite, path: String) -> Self {
+        CosWriter { core, op, path }
     }
-}
 
-#[async_trait]
-impl oio::Write for ObsWriter {
-    async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.obs_put_object_request(
+    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
+        let mut req = self.core.cos_put_object_request(
             &self.path,
-            Some(bs.len()),
+            Some(size),
             self.op.content_type(),
             self.op.cache_control(),
-            AsyncBody::Bytes(bs),
+            body,
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
@@ -60,20 +57,25 @@
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
+}
+
+#[async_trait]
+impl oio::Write for CosWriter {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        self.write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
+            .await
+    }
 
-    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "Write::sink is not supported",
-        ))
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.write_oneshot(size, AsyncBody::Stream(s)).await
     }
 
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/builder.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/graph_model.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/onedrive/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/onedrive/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/oss/appender.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/oss/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -404,14 +404,15 @@
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
                 read_with_if_match: true,
                 read_with_if_none_match: true,
 
                 write: true,
+                write_can_sink: true,
                 write_with_cache_control: true,
                 write_with_content_type: true,
                 write_without_content_length: true,
                 delete: true,
                 create_dir: true,
                 copy: true,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 }
 
 impl OssCore {
     #[allow(clippy::too_many_arguments)]
     pub fn oss_put_object_request(
         &self,
         path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
         is_presign: bool,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
@@ -372,15 +372,15 @@
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub async fn oss_put_object(
         &self,
         path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Response<IncomingAsyncBody>> {
         let mut req = self.oss_put_object_request(
             path,
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/oss/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/oss/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -50,22 +50,22 @@
             upload_id: None,
             parts: vec![],
             buffer: oio::VectorCursor::new(),
             buffer_size,
         }
     }
 
-    async fn write_oneshot(&self, bs: Bytes) -> Result<()> {
+    async fn write_oneshot(&self, size: u64, body: AsyncBody) -> Result<()> {
         let mut req = self.core.oss_put_object_request(
             &self.path,
-            Some(bs.len()),
+            Some(size),
             self.op.content_type(),
             self.op.content_disposition(),
             self.op.cache_control(),
-            AsyncBody::Bytes(bs),
+            body,
             false,
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
@@ -132,15 +132,17 @@
 #[async_trait]
 impl oio::Write for OssWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let upload_id = match &self.upload_id {
             Some(upload_id) => upload_id,
             None => {
                 if self.op.content_length().unwrap_or_default() == bs.len() as u64 {
-                    return self.write_oneshot(bs).await;
+                    return self
+                        .write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
+                        .await;
                 } else {
                     let upload_id = self.initiate_upload().await?;
                     self.upload_id = Some(upload_id);
                     self.upload_id.as_deref().unwrap()
                 }
             }
         };
@@ -170,19 +172,16 @@
                 // write is re-enter safe.
                 self.buffer.pop();
                 Err(e)
             }
         }
     }
 
-    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "Write::sink is not supported",
-        ))
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.write_oneshot(size, AsyncBody::Stream(s)).await
     }
 
     // TODO: we can cancel the upload by sending an abort request.
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support abort",
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/redb/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/redb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/redb/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/redb/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/redb/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/redb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/redis/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/redis/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 use async_trait::async_trait;
 use base64::prelude::BASE64_STANDARD;
 use base64::Engine;
 use bytes::Buf;
 use http::StatusCode;
 use log::debug;
+use log::warn;
 use md5::Digest;
 use md5::Md5;
 use once_cell::sync::Lazy;
 use reqsign::AwsConfig;
 use reqsign::AwsCredentialLoad;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
@@ -52,14 +53,15 @@
         "https://s3.{region}.amazonaws.com",
     );
     m
 });
 
 const DEFAULT_WRITE_MIN_SIZE: usize = 8 * 1024 * 1024;
 const DEFAULT_BATCH_MAX_OPERATIONS: usize = 1000;
+
 /// Aws S3 and compatible services (including minio, digitalocean space, Tencent Cloud Object Storage(COS) and so on) support.
 /// For more information about s3-compatible services, refer to [Compatible Services](#compatible-services).
 #[doc = include_str!("docs.md")]
 #[doc = include_str!("compatible_services.md")]
 #[derive(Default)]
 pub struct S3Builder {
     root: Option<String>,
@@ -513,14 +515,124 @@
     }
     /// Set maximum batch operations of this backend.
     pub fn batch_max_operations(&mut self, batch_max_operations: usize) -> &mut Self {
         self.batch_max_operations = Some(batch_max_operations);
 
         self
     }
+
+    /// Detect region of S3 bucket.
+    ///
+    /// # Args
+    ///
+    /// - endpoint: the endpoint of S3 service
+    /// - bucket: the bucket of S3 service
+    ///
+    /// # Return
+    ///
+    /// - `Some(region)` means we detect the region successfully
+    /// - `None` means we can't detect the region or meeting errors.
+    ///
+    /// # Notes
+    ///
+    /// We will try to detect region by the following methods.
+    ///
+    /// - Match endpoint with given rules to get region
+    ///   - Cloudflare R2
+    ///   - AWS S3
+    ///   - Aliyun OSS
+    /// - Send a `HEAD` request to endpoint with bucket name to get `x-amz-bucket-region`.
+    ///
+    /// # Examples
+    ///
+    /// ```no_run
+    /// use opendal::services::S3;
+    ///
+    /// # async fn example() {
+    /// let builder = S3::default();
+    /// let region: Option<String> = builder.detect_region("https://s3.amazonaws.com", "example").await;
+    /// # }
+    /// ```
+    ///
+    /// # Reference
+    ///
+    /// - [Amazon S3 HeadBucket API](https://docs.aws.amazon.com/zh_cn/AmazonS3/latest/API/API_HeadBucket.html)
+    pub async fn detect_region(&self, endpoint: &str, bucket: &str) -> Option<String> {
+        let mut endpoint = if endpoint.starts_with("http") {
+            endpoint.to_string()
+        } else {
+            // Prefix https if endpoint doesn't start with scheme.
+            format!("https://{}", endpoint)
+        };
+
+        // Remove bucket name from endpoint.
+        endpoint = endpoint.replace(&format!("//{bucket}."), "//");
+        let url = format!("{endpoint}/{bucket}");
+
+        debug!("detect region with url: {url}");
+
+        // Try to detect region by endpoint.
+
+        // If this bucket is R2, we can return auto directly.
+        //
+        // Reference: <https://developers.cloudflare.com/r2/api/s3/api/>
+        if endpoint.ends_with("r2.cloudflarestorage.com") {
+            return Some("auto".to_string());
+        }
+
+        // If this bucket is AWS, we can try to match the endpoint.
+        if let Some(v) = endpoint.strip_prefix("https://s3.") {
+            if let Some(region) = v.strip_suffix(".amazonaws.com") {
+                return Some(region.to_string());
+            }
+        }
+
+        // If this bucket is OSS, we can try to match the endpoint.
+        //
+        // - `oss-ap-southeast-1.aliyuncs.com` => `oss-ap-southeast-1`
+        // - `oss-cn-hangzhou-internal.aliyuncs.com` => `oss-cn-hangzhou`
+        if let Some(v) = endpoint.strip_prefix("https://") {
+            if let Some(region) = v.strip_suffix(".aliyuncs.com") {
+                return Some(region.to_string());
+            }
+
+            if let Some(region) = v.strip_suffix("-internal.aliyuncs.com") {
+                return Some(region.to_string());
+            }
+        }
+
+        // Try to detect region by HeadBucket.
+        let req = http::Request::head(&url).body(AsyncBody::Empty).ok()?;
+
+        let client = HttpClient::new().ok()?;
+        let res = client
+            .send(req)
+            .await
+            .map_err(|err| warn!("detect region failed for: {err:?}"))
+            .ok()?;
+
+        debug!(
+            "auto detect region got response: status {:?}, header: {:?}",
+            res.status(),
+            res.headers()
+        );
+
+        match res.status() {
+            StatusCode::OK | StatusCode::FORBIDDEN | StatusCode::MOVED_PERMANENTLY => {
+                let region = res.headers().get("x-amz-bucket-region")?;
+                if let Ok(regin) = region.to_str() {
+                    Some(regin.to_string())
+                } else {
+                    None
+                }
+            }
+            // Unexpected status code
+            _ => None,
+        }
+    }
 }
 
 impl Builder for S3Builder {
     const SCHEME: Scheme = Scheme::S3;
     type Accessor = S3Backend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
@@ -1045,8 +1157,57 @@
                 b.endpoint(endpoint);
             }
 
             let endpoint = b.build_endpoint("us-east-2");
             assert_eq!(endpoint, "https://test.s3.us-east-2.amazonaws.com");
         }
     }
+
+    #[tokio::test]
+    async fn test_detect_region() {
+        let cases = vec![
+            (
+                "aws s3 without region in endpoint",
+                "https://s3.amazonaws.com",
+                "example",
+                Some("us-east-1"),
+            ),
+            (
+                "aws s3 with region in endpoint",
+                "https://s3.us-east-1.amazonaws.com",
+                "example",
+                Some("us-east-1"),
+            ),
+            (
+                "oss with public endpoint",
+                "https://oss-ap-southeast-1.aliyuncs.com",
+                "example",
+                Some("oss-ap-southeast-1"),
+            ),
+            (
+                "oss with internal endpoint",
+                "https://oss-cn-hangzhou-internal.aliyuncs.com",
+                "example",
+                Some("oss-cn-hangzhou-internal"),
+            ),
+            (
+                "r2",
+                "https://abc.xxxxx.r2.cloudflarestorage.com",
+                "example",
+                Some("auto"),
+            ),
+            (
+                "invalid service",
+                "https://opendal.apache.org",
+                "example",
+                None,
+            ),
+        ];
+
+        let b = S3Builder::default();
+
+        for (name, endpoint, bucket, expected) in cases {
+            let region = b.detect_region(endpoint, bucket).await;
+            assert_eq!(region.as_deref(), expected, "{}", name);
+        }
+    }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/s3/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/s3/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/writer.rs`

 * *Files 21% similar despite different names*

```diff
@@ -11,75 +11,85 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::pin::Pin;
+use std::sync::Arc;
 
 use async_trait::async_trait;
-use futures::StreamExt;
-use openssh_sftp_client::fs::DirEntry;
-use openssh_sftp_client::fs::ReadDir;
-
-use crate::raw::oio;
-use crate::Result;
-
-pub struct SftpPager {
-    dir: Pin<Box<ReadDir>>,
-    prefix: String,
-    limit: usize,
+use bytes::Bytes;
+use http::StatusCode;
+
+use super::core::*;
+use super::error::parse_error;
+use crate::raw::*;
+use crate::*;
+
+pub struct SupabaseWriter {
+    core: Arc<SupabaseCore>,
+
+    op: OpWrite,
+    path: String,
 }
 
-impl SftpPager {
-    pub fn new(dir: ReadDir, path: String, limit: Option<usize>) -> Self {
-        let prefix = if path == "/" { "".to_owned() } else { path };
-
-        let limit = limit.unwrap_or(usize::MAX);
-
-        SftpPager {
-            dir: Box::pin(dir),
-            prefix,
-            limit,
+impl SupabaseWriter {
+    pub fn new(core: Arc<SupabaseCore>, path: &str, op: OpWrite) -> Self {
+        SupabaseWriter {
+            core,
+            op,
+            path: path.to_string(),
+        }
+    }
+
+    pub async fn upload(&self, bytes: Bytes) -> Result<()> {
+        let size = bytes.len();
+        let mut req = self.core.supabase_upload_object_request(
+            &self.path,
+            Some(size),
+            self.op.content_type(),
+            AsyncBody::Bytes(bytes),
+        )?;
+
+        self.core.sign(&mut req)?;
+
+        let resp = self.core.send(req).await?;
+
+        match resp.status() {
+            StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(())
+            }
+            _ => Err(parse_error(resp).await?),
         }
     }
 }
 
 #[async_trait]
-impl oio::Page for SftpPager {
-    async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
-        if self.limit == 0 {
-            return Ok(None);
+impl oio::Write for SupabaseWriter {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        if bs.is_empty() {
+            return Ok(());
         }
 
-        let item = self.dir.next().await;
+        self.upload(bs).await
+    }
 
-        match item {
-            Some(Ok(e)) => {
-                if e.filename().to_str() == Some(".") || e.filename().to_str() == Some("..") {
-                    self.next().await
-                } else {
-                    self.limit -= 1;
-                    Ok(Some(vec![map_entry(self.prefix.as_str(), e.clone())]))
-                }
-            }
-            Some(Err(e)) => Err(e.into()),
-            None => Ok(None),
-        }
+    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "Write::sink is not supported",
+        ))
     }
-}
 
-fn map_entry(prefix: &str, value: DirEntry) -> oio::Entry {
-    let path = format!(
-        "{}{}{}",
-        prefix,
-        value.filename().to_str().unwrap(),
-        if value.file_type().unwrap().is_dir() {
-            "/"
-        } else {
-            ""
-        }
-    );
+    async fn abort(&mut self) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "The abort operation is not yet supported for Supabase backend",
+        ))
+    }
 
-    oio::Entry::new(path.as_str(), value.metadata().into())
+    async fn close(&mut self) -> Result<()> {
+        Ok(())
+    }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/utils.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sftp/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/sftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sled/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/sled/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/supabase/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/supabase/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files 14% similar despite different names*

```diff
@@ -22,74 +22,59 @@
 use http::StatusCode;
 
 use super::core::*;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct SupabaseWriter {
-    core: Arc<SupabaseCore>,
+pub struct WasabiWriter {
+    core: Arc<WasabiCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl SupabaseWriter {
-    pub fn new(core: Arc<SupabaseCore>, path: &str, op: OpWrite) -> Self {
-        SupabaseWriter {
-            core,
-            op,
-            path: path.to_string(),
-        }
+impl WasabiWriter {
+    pub fn new(core: Arc<WasabiCore>, op: OpWrite, path: String) -> Self {
+        WasabiWriter { core, op, path }
     }
+}
 
-    pub async fn upload(&self, bytes: Bytes) -> Result<()> {
-        let size = bytes.len();
-        let mut req = self.core.supabase_upload_object_request(
-            &self.path,
-            Some(size),
-            self.op.content_type(),
-            AsyncBody::Bytes(bytes),
-        )?;
-
-        self.core.sign(&mut req)?;
-
-        let resp = self.core.send(req).await?;
+#[async_trait]
+impl oio::Write for WasabiWriter {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        let resp = self
+            .core
+            .put_object(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                self.op.content_disposition(),
+                self.op.cache_control(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
         match resp.status() {
-            StatusCode::OK => {
+            StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
-}
-
-#[async_trait]
-impl oio::Write for SupabaseWriter {
-    async fn write(&mut self, bs: Bytes) -> Result<()> {
-        if bs.is_empty() {
-            return Ok(());
-        }
-
-        self.upload(bs).await
-    }
 
     async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "Write::sink is not supported",
         ))
     }
 
     async fn abort(&mut self) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "The abort operation is not yet supported for Supabase backend",
-        ))
+        Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 18% similar despite different names*

```diff
@@ -11,54 +11,53 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::sync::Arc;
-
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::*;
+use super::backend::WebhdfsBackend;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct WasabiWriter {
-    core: Arc<WasabiCore>,
+pub struct WebhdfsWriter {
+    backend: WebhdfsBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl WasabiWriter {
-    pub fn new(core: Arc<WasabiCore>, op: OpWrite, path: String) -> Self {
-        WasabiWriter { core, op, path }
+impl WebhdfsWriter {
+    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
+        WebhdfsWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WasabiWriter {
+impl oio::Write for WebhdfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let resp = self
-            .core
-            .put_object(
+        let req = self
+            .backend
+            .webhdfs_create_object_request(
                 &self.path,
                 Some(bs.len()),
                 self.op.content_type(),
-                self.op.content_disposition(),
-                self.op.cache_control(),
                 AsyncBody::Bytes(bs),
             )
             .await?;
 
-        match resp.status() {
+        let resp = self.backend.client.send(req).await?;
+
+        let status = resp.status();
+        match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
+use std::collections::VecDeque;
 use std::fmt::Debug;
 use std::fmt::Formatter;
+use std::str::FromStr;
 
 use async_trait::async_trait;
 use bytes::Buf;
 use http::header;
 use http::HeaderMap;
 use http::Request;
 use http::Response;
 use http::StatusCode;
 use log::debug;
 
 use super::error::parse_error;
-use super::list_response::Multistatus;
+use super::pager::Multistatus;
 use super::pager::WebdavPager;
 use super::writer::WebdavWriter;
 use crate::raw::*;
 use crate::*;
 
 /// [WebDAV](https://datatracker.ietf.org/doc/html/rfc4918) backend support.
 ///
@@ -198,14 +200,23 @@
             Some(v) => v,
             None => {
                 return Err(Error::new(ErrorKind::ConfigInvalid, "endpoint is empty")
                     .with_context("service", Scheme::Webdav));
             }
         };
 
+        let uri = http::Uri::from_str(endpoint).map_err(|err| {
+            Error::new(ErrorKind::ConfigInvalid, "endpoint is invalid")
+                .set_source(err)
+                .with_context("service", Scheme::Webdav)
+        })?;
+        // Some webdav server may have base dir like `/remote.php/webdav/`
+        // returned in the `href`.
+        let base_dir = uri.path().trim_end_matches('/');
+
         let root = normalize_root(&self.root.take().unwrap_or_default());
         debug!("backend use root {}", root);
 
         let client = if let Some(client) = self.http_client.take() {
             client
         } else {
             HttpClient::new().map_err(|err| {
@@ -224,25 +235,27 @@
         if let Some(token) = &self.token {
             auth = Some(format_authorization_by_bearer(token)?)
         }
 
         debug!("backend build finished: {:?}", &self);
         Ok(WebdavBackend {
             endpoint: endpoint.to_string(),
+            base_dir: base_dir.to_string(),
             authorization: auth,
             root,
             client,
         })
     }
 }
 
 /// Backend is used to serve `Accessor` support for http.
 #[derive(Clone)]
 pub struct WebdavBackend {
     endpoint: String,
+    base_dir: String,
     root: String,
     client: HttpClient,
 
     authorization: Option<String>,
 }
 
 impl Debug for WebdavBackend {
@@ -258,48 +271,52 @@
 #[async_trait]
 impl Accessor for WebdavBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = WebdavWriter;
     type BlockingWriter = ();
     type Appender = ();
-    type Pager = WebdavPager;
+    type Pager = Option<WebdavPager>;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Webdav)
             .set_root(&self.root)
             .set_capability(Capability {
                 stat: true,
 
                 read: true,
                 read_can_next: true,
                 read_with_range: true,
 
                 write: true,
+                write_can_sink: true,
+
                 create_dir: true,
                 delete: true,
+
                 copy: true,
+
                 rename: true,
 
                 list: true,
                 list_with_delimiter_slash: true,
 
                 ..Default::default()
             });
 
         ma
     }
 
     async fn create_dir(&self, path: &str, _: OpCreateDir) -> Result<RpCreateDir> {
         self.ensure_parent_path(path).await?;
+        self.create_dir_internal(path).await?;
 
-        let abs_path = build_abs_path(&self.root, path);
-        self.create_internal(&abs_path).await
+        Ok(RpCreateDir::default())
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self.webdav_get(path, args.range()).await?;
         let status = resp.status();
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
@@ -314,14 +331,16 @@
         if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
                 "write without content length is not supported",
             ));
         }
 
+        self.ensure_parent_path(path).await?;
+
         let p = build_abs_path(&self.root, path);
 
         Ok((RpWrite::default(), WebdavWriter::new(self.clone(), args, p)))
     }
 
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
         self.ensure_parent_path(to).await?;
@@ -420,27 +439,18 @@
             StatusCode::OK | StatusCode::MULTI_STATUS => {
                 let bs = resp.into_body().bytes().await?;
                 let result: Multistatus =
                     quick_xml::de::from_reader(bs.reader()).map_err(new_xml_deserialize_error)?;
 
                 Ok((
                     RpList::default(),
-                    WebdavPager::new(&self.root, path, result),
+                    Some(WebdavPager::new(&self.base_dir, &self.root, path, result)),
                 ))
             }
-            StatusCode::NOT_FOUND if path.ends_with('/') => Ok((
-                RpList::default(),
-                WebdavPager::new(
-                    &self.root,
-                    path,
-                    Multistatus {
-                        response: Vec::new(),
-                    },
-                ),
-            )),
+            StatusCode::NOT_FOUND if path.ends_with('/') => Ok((RpList::default(), None)),
             _ => Err(parse_error(resp).await?),
         }
     }
 }
 
 impl WebdavBackend {
     async fn webdav_get(
@@ -467,15 +477,15 @@
 
         self.client.send(req).await
     }
 
     pub async fn webdav_put(
         &self,
         abs_path: &str,
-        size: Option<usize>,
+        size: Option<u64>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
         body: AsyncBody,
     ) -> Result<Response<IncomingAsyncBody>> {
         let url = format!("{}/{}", self.endpoint, percent_encode_path(abs_path));
 
         let mut req = Request::put(&url);
@@ -498,37 +508,27 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
 
-    async fn webdav_mkcol(
-        &self,
-        abs_path: &str,
-        content_type: Option<&str>,
-        content_disposition: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(abs_path));
+    async fn webdav_mkcol(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::builder().method("MKCOL").uri(&url);
         if let Some(auth) = &self.authorization {
             req = req.header(header::AUTHORIZATION, auth);
         }
 
-        if let Some(mime) = content_type {
-            req = req.header(header::CONTENT_TYPE, mime)
-        }
-
-        if let Some(cd) = content_disposition {
-            req = req.header(header::CONTENT_DISPOSITION, cd)
-        }
-
-        let req = req.body(body).map_err(new_request_build_error)?;
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
 
     async fn webdav_propfind(
         &self,
         path: &str,
@@ -632,57 +632,55 @@
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
 
-    async fn create_internal(&self, abs_path: &str) -> Result<RpCreateDir> {
-        let resp = if abs_path.ends_with('/') {
-            self.webdav_mkcol(abs_path, None, None, AsyncBody::Empty)
-                .await?
-        } else {
-            self.webdav_put(abs_path, Some(0), None, None, AsyncBody::Empty)
-                .await?
-        };
+    async fn create_dir_internal(&self, path: &str) -> Result<()> {
+        let resp = self.webdav_mkcol(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED
-            | StatusCode::OK
-            // `File exists` will return `Method Not Allowed`
-            | StatusCode::METHOD_NOT_ALLOWED
-            // create existing dir will return conflict
-            | StatusCode::CONFLICT
-            // create existing file will return no_content
-            | StatusCode::NO_CONTENT => {
+            // Allow multiple status
+            | StatusCode::MULTI_STATUS
+            // The MKCOL method can only be performed on a deleted or non-existent resource.
+            // This error means the directory already exists which is allowed by create_dir.
+            | StatusCode::METHOD_NOT_ALLOWED => {
                 resp.into_body().consume().await?;
-                Ok(RpCreateDir::default())
+                Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn ensure_parent_path(&self, path: &str) -> Result<()> {
-        if path == "/" {
-            return Ok(());
-        }
+    async fn ensure_parent_path(&self, mut path: &str) -> Result<()> {
+        let mut dirs = VecDeque::default();
 
-        // create dir recursively, split path by `/` and create each dir except the last one
-        let abs_path = build_abs_path(&self.root, path);
-        let abs_path = abs_path.as_str();
-        let mut parts: Vec<&str> = abs_path.split('/').filter(|x| !x.is_empty()).collect();
-        if !parts.is_empty() {
-            parts.pop();
-        }
-
-        let mut sub_path = String::new();
-        for sub_part in parts {
-            let sub_path_with_slash = sub_part.to_owned() + "/";
-            sub_path.push_str(&sub_path_with_slash);
-            self.create_internal(&sub_path).await?;
+        while path != "/" {
+            // check path first.
+            let parent = get_parent(path);
+
+            let mut header_map = HeaderMap::new();
+            // not include children
+            header_map.insert("Depth", "0".parse().unwrap());
+            header_map.insert(header::ACCEPT, "application/xml".parse().unwrap());
+
+            let resp = self.webdav_propfind(parent, Some(header_map)).await?;
+            match resp.status() {
+                StatusCode::OK | StatusCode::MULTI_STATUS => break,
+                StatusCode::NOT_FOUND => {
+                    dirs.push_front(parent);
+                    path = parent
+                }
+                _ => return Err(parse_error(resp).await?),
+            }
         }
 
+        for dir in dirs {
+            self.create_dir_internal(dir).await?;
+        }
         Ok(())
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        // Allowing retry for resource locked.
+        StatusCode::LOCKED => (ErrorKind::Unexpected, true),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,73 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::mem;
+
+use async_trait::async_trait;
 use serde::Deserialize;
 
-use crate::raw::parse_datetime_from_rfc2822;
-use crate::EntryMode;
-use crate::Error;
-use crate::ErrorKind;
-use crate::Metadata;
-use crate::Result;
+use crate::raw::*;
+use crate::*;
+pub struct WebdavPager {
+    base_dir: String,
+    root: String,
+    path: String,
+    multistates: Multistatus,
+}
+
+impl WebdavPager {
+    pub fn new(base_dir: &str, root: &str, path: &str, multistates: Multistatus) -> Self {
+        Self {
+            base_dir: base_dir.to_string(),
+            root: root.into(),
+            path: path.into(),
+            multistates,
+        }
+    }
+}
+
+#[async_trait]
+impl oio::Page for WebdavPager {
+    async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
+        if self.multistates.response.is_empty() {
+            return Ok(None);
+        };
+        let oes = mem::take(&mut self.multistates.response);
+
+        let mut entries = Vec::with_capacity(oes.len());
+
+        for res in oes {
+            let path = res
+                .href
+                .strip_prefix(&self.base_dir)
+                .unwrap_or(res.href.as_str());
+
+            // Ignore the root path itself.
+            if self.root == path {
+                continue;
+            }
+
+            let normalized_path = build_rel_path(&self.root, path);
+            if normalized_path == self.path {
+                // WebDav server may return the current path as an entry.
+                continue;
+            }
+
+            let meta = res.parse_into_metadata()?;
+            entries.push(oio::Entry::new(&normalized_path, meta))
+        }
+
+        Ok(Some(entries))
+    }
+}
 
 #[derive(Deserialize, Debug, PartialEq, Eq)]
 pub struct Multistatus {
     pub response: Vec<ListOpResponse>,
 }
 
 #[derive(Deserialize, Debug, PartialEq, Eq)]
@@ -59,15 +110,15 @@
                 return Err(Error::new(
                     ErrorKind::Unexpected,
                     &format!("Invalid response: {} {}", code, text),
                 ));
             }
         }
 
-        let mode = if href.ends_with('/') {
+        let mode: EntryMode = if href.ends_with('/') {
             EntryMode::DIR
         } else {
             EntryMode::FILE
         };
         let mut m = Metadata::new(mode);
 
         if let Some(v) = getcontentlength {
@@ -77,14 +128,15 @@
         if let Some(v) = getcontenttype {
             m.set_content_type(v);
         }
 
         if let Some(v) = getetag {
             m.set_etag(v);
         }
+
         // https://www.rfc-editor.org/rfc/rfc4918#section-14.18
         m.set_last_modified(parse_datetime_from_rfc2822(getlastmodified)?);
         Ok(m)
     }
 }
 
 #[derive(Deserialize, Debug, PartialEq, Eq)]
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -15,10 +15,9 @@
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
 pub use backend::WebdavBuilder as Webdav;
 
 mod error;
-mod list_response;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/entry.rs`

 * *Files 26% similar despite different names*

```diff
@@ -11,73 +11,70 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::mem;
+use crate::raw::*;
+use crate::*;
 
-use async_trait::async_trait;
-
-use super::list_response::Multistatus;
-use crate::raw::build_rel_path;
-use crate::raw::oio;
-use crate::EntryMode;
-use crate::Metadata;
-use crate::Result;
-
-pub struct WebdavPager {
-    root: String,
+/// Entry is the file/dir entry returned by `Lister`.
+#[derive(Clone, Debug)]
+pub struct Entry {
+    /// Path of the entry.
     path: String,
-    multistates: Multistatus,
+
+    /// Optional cached metadata
+    metadata: Option<Metadata>,
 }
 
-impl WebdavPager {
-    pub fn new(root: &str, path: &str, multistates: Multistatus) -> Self {
+impl Entry {
+    /// Create an entry with .
+    ///
+    /// # Notes
+    ///
+    /// This function is crate internal only. Users don't have public
+    /// methods to construct an entry with arbitrary cached metadata.
+    ///
+    /// The only way to get an entry with associated cached metadata
+    /// is `Operator::list` or `Operator::scan`.
+    pub(crate) fn new_with(path: String, metadata: Metadata) -> Self {
         Self {
-            root: root.into(),
-            path: path.into(),
-            multistates,
+            path,
+            metadata: Some(metadata),
         }
     }
-}
 
-#[async_trait]
-impl oio::Page for WebdavPager {
-    async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
-        if self.multistates.response.is_empty() {
-            return Ok(None);
-        };
-        let oes = mem::take(&mut self.multistates.response);
-
-        let oes = oes
-            .into_iter()
-            .filter_map(|de| {
-                let path = de.href;
-
-                // Ignore the root path itself.
-                if self.root == path {
-                    return None;
-                }
-
-                let normalized_path = build_rel_path(&self.root, &path);
-                if normalized_path == self.path {
-                    // WebDav server may return the current path as an entry.
-                    return None;
-                }
-
-                let entry = if de.propstat.prop.resourcetype.value
-                    == Some(super::list_response::ResourceType::Collection)
-                {
-                    oio::Entry::new(&normalized_path, Metadata::new(EntryMode::DIR))
-                } else {
-                    oio::Entry::new(&normalized_path, Metadata::new(EntryMode::FILE))
-                };
-
-                Some(entry)
-            })
-            .collect();
+    /// Create an [`Entry`] with empty cached metadata.
+    pub fn new(path: &str) -> Self {
+        Self {
+            path: normalize_path(path),
+            metadata: None,
+        }
+    }
+
+    /// Path of entry. Path is relative to operator's root.
+    /// Only valid in current operator.
+    pub fn path(&self) -> &str {
+        &self.path
+    }
+
+    /// Name of entry. Name is the last segment of path.
+    ///
+    /// If this entry is a dir, `Name` MUST endswith `/`
+    /// Otherwise, `Name` MUST NOT endswith `/`.
+    pub fn name(&self) -> &str {
+        get_basename(&self.path)
+    }
 
-        Ok(Some(oes))
+    /// Get the cached metadata of entry.
+    ///
+    /// # Notes
+    ///
+    /// This function is crate internal only. Because the returning
+    /// metadata could be incomplete. Users must use `Operator::metadata`
+    /// to query the cached metadata instead.
+    pub(crate) fn metadata(&self) -> &Option<Metadata> {
+        &self.metadata
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files 13% similar despite different names*

```diff
@@ -31,46 +31,48 @@
     path: String,
 }
 
 impl WebdavWriter {
     pub fn new(backend: WebdavBackend, op: OpWrite, path: String) -> Self {
         WebdavWriter { backend, op, path }
     }
-}
 
-#[async_trait]
-impl oio::Write for WebdavWriter {
-    async fn write(&mut self, bs: Bytes) -> Result<()> {
+    async fn write_oneshot(&mut self, size: u64, body: AsyncBody) -> Result<()> {
         let resp = self
             .backend
             .webdav_put(
                 &self.path,
-                Some(bs.len()),
+                Some(size),
                 self.op.content_type(),
                 self.op.content_disposition(),
-                AsyncBody::Bytes(bs),
+                body,
             )
             .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
+}
+
+#[async_trait]
+impl oio::Write for WebdavWriter {
+    async fn write(&mut self, bs: Bytes) -> Result<()> {
+        self.write_oneshot(bs.len() as u64, AsyncBody::Bytes(bs))
+            .await
+    }
 
-    async fn sink(&mut self, _size: u64, _s: oio::Streamer) -> Result<()> {
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "Write::sink is not supported",
-        ))
+    async fn sink(&mut self, size: u64, s: oio::Streamer) -> Result<()> {
+        self.write_oneshot(size, AsyncBody::Stream(s)).await
     }
 
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/docs.md` & `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/docs.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.38.1/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/appender.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/appender.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/capability.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/capability.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/error.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,18 @@
     /// This error kind means expect content length is not reached.
     ///
     /// For examples:
     ///
     /// - Users expected to read 1024 bytes, but service returned less bytes.
     /// - Service expected to write 1024 bytes, but users write less bytes.
     ContentIncomplete,
+    /// The input is invalid.
+    ///
+    /// For example, user try to seek to a negative position
+    InvalidInput,
 }
 
 impl ErrorKind {
     /// Convert self into static str.
     pub fn into_static(self) -> &'static str {
         self.into()
     }
@@ -126,14 +130,15 @@
             ErrorKind::NotADirectory => "NotADirectory",
             ErrorKind::AlreadyExists => "AlreadyExists",
             ErrorKind::RateLimited => "RateLimited",
             ErrorKind::IsSameFile => "IsSameFile",
             ErrorKind::ConditionNotMatch => "ConditionNotMatch",
             ErrorKind::ContentTruncated => "ContentTruncated",
             ErrorKind::ContentIncomplete => "ContentIncomplete",
+            ErrorKind::InvalidInput => "InvalidInput",
         }
     }
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
 enum ErrorStatus {
     /// Permanent means without external changes, the error never changes.
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/list.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/metadata.rs`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     content_disposition: Option<String>,
     content_length: Option<u64>,
     content_md5: Option<String>,
     content_range: Option<BytesContentRange>,
     content_type: Option<String>,
     etag: Option<String>,
     last_modified: Option<DateTime<Utc>>,
+    version: Option<String>,
 }
 
 impl Metadata {
     /// Create a new metadata
     pub fn new(mode: EntryMode) -> Self {
         // Mode is required to be set for metadata.
         let mut bit: FlagSet<Metakey> = Metakey::Mode.into();
@@ -65,14 +66,15 @@
             content_length: None,
             content_md5: None,
             content_type: None,
             content_range: None,
             last_modified: None,
             etag: None,
             content_disposition: None,
+            version: None,
         }
     }
 
     /// Get the bit from metadata.
     pub(crate) fn bit(&self) -> FlagSet<Metakey> {
         self.bit
     }
@@ -414,14 +416,50 @@
     /// - "attachment"
     /// - "attachment; filename=\"filename.jpg\""
     pub fn set_content_disposition(&mut self, v: &str) -> &mut Self {
         self.content_disposition = Some(v.to_string());
         self.bit |= Metakey::ContentDisposition;
         self
     }
+
+    /// Version of this entry.
+    ///
+    /// Version is a string that can be used to identify the version of this entry.
+    ///
+    /// This field may come out from the version control system, like object versioning in AWS S3.
+    pub fn version(&self) -> Option<&str> {
+        debug_assert!(
+            self.bit.contains(Metakey::Version) || self.bit.contains(Metakey::Complete),
+            "visiting not set metadata: version, maybe a bug"
+        );
+
+        self.version.as_deref()
+    }
+
+    /// Set version of this entry.
+    ///
+    /// Version is a string that can be used to identify the version of this entry.
+    ///
+    /// This field may come out from the version control system, like object versioning in AWS S3.
+    pub fn with_version(mut self, v: String) -> Self {
+        self.version = Some(v);
+        self.bit |= Metakey::Version;
+        self
+    }
+
+    /// Set version of this entry.
+    ///
+    /// Version is a string that can be used to identify the version of this entry.
+    ///
+    /// This field may come out from the version control system, like object versioning in AWS S3.
+    pub fn set_version(&mut self, v: &str) -> &mut Self {
+        self.version = Some(v.to_string());
+        self.bit |= Metakey::Version;
+        self
+    }
 }
 
 flags! {
     /// Metakey describes the metadata keys that can be stored
     /// or queried.
     ///
     /// ## For store
@@ -453,9 +491,11 @@
         ContentRange,
         /// Key for content type.
         ContentType,
         /// Key for etag.
         Etag,
         /// Key for last last modified.
         LastModified,
+        /// Key for version.
+        Version,
     }
 }
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -669,19 +669,51 @@
     /// # use opendal::BlockingOperator;
     /// # fn test(op: BlockingOperator) -> Result<()> {
     /// op.delete("path/to/file")?;
     /// # Ok(())
     /// # }
     /// ```
     pub fn delete(&self, path: &str) -> Result<()> {
+        self.delete_with(path).call()?;
+
+        Ok(())
+    }
+
+    /// Delete given path with options.
+    ///
+    /// # Notes
+    ///
+    /// - Delete not existing error won't return errors.
+    ///
+    /// # Examples
+    ///
+    /// ```no_run
+    /// # use anyhow::Result;
+    /// # use futures::io;
+    /// # use opendal::BlockingOperator;
+    /// # fn test(op: BlockingOperator) -> Result<()> {
+    /// let _ = op
+    ///     .delete_with("path/to/file")
+    ///     .version("example_version").call()?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub fn delete_with(&self, path: &str) -> FunctionDelete {
         let path = normalize_path(path);
 
-        let _ = self.inner().blocking_delete(&path, OpDelete::new())?;
+        FunctionDelete(OperatorFunction::new(
+            self.inner().clone(),
+            path,
+            OpDelete::new(),
+            |inner, path, args| {
+                let _ = inner.blocking_delete(&path, args)?;
 
-        Ok(())
+                Ok(())
+            },
+        ))
     }
 
     /// remove will remove files via the given paths.
     ///
     /// remove_via will remove files via the given vector iterators.
     ///
     /// # Notes
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1069,19 +1069,54 @@
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// op.delete("test").await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn delete(&self, path: &str) -> Result<()> {
+        self.delete_with(path).await
+    }
+
+    /// Delete the given path with extra options.
+    ///
+    /// # Notes
+    ///
+    /// - Deleting a file that does not exist won't return errors.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use anyhow::Result;
+    /// # use futures::io;
+    /// # use opendal::Operator;
+    ///
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// op.delete_with("test").await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub fn delete_with(&self, path: &str) -> FutureDelete {
         let path = normalize_path(path);
 
-        let _ = self.inner().delete(&path, OpDelete::new()).await?;
+        let fut = FutureDelete(OperatorFuture::new(
+            self.inner().clone(),
+            path,
+            OpDelete::default(),
+            |inner, path, args| {
+                let fut = async move {
+                    let _ = inner.delete(&path, args).await?;
+                    Ok(())
+                };
+
+                Box::pin(fut)
+            },
+        ));
 
-        Ok(())
+        fut
     }
 
     ///
     /// # Notes
     ///
     /// If underlying services support delete in batch, we will use batch
     /// delete instead.
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator_functions.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator_functions.rs`

 * *Files 13% similar despite different names*

```diff
@@ -91,7 +91,26 @@
 
     /// Call the function to consume all the input and generate a
     /// result.
     pub fn call(self) -> Result<()> {
         self.0.call()
     }
 }
+
+/// Function that generated by [`BlockingOperator::delete_with`].
+///
+/// Users can add more options by public functions provided by this struct.
+pub struct FunctionDelete(pub(crate) OperatorFunction<OpDelete, ()>);
+
+impl FunctionDelete {
+    /// Set the version for this operation.
+    pub fn version(mut self, v: &str) -> Self {
+        self.0 = self.0.map_args(|args| args.with_version(v));
+        self
+    }
+
+    /// Call the function to consume all the input and generate a
+    /// result.
+    pub fn call(self) -> Result<()> {
+        self.0.call()
+    }
+}
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/operator/operator_futures.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/operator/operator_futures.rs`

 * *Files 3% similar despite different names*

```diff
@@ -127,14 +127,20 @@
     }
 
     /// Set the If-None-Match for this operation.
     pub fn if_none_match(mut self, v: &str) -> Self {
         self.0 = self.0.map_args(|args| args.with_if_none_match(v));
         self
     }
+
+    /// Set the version for this operation.
+    pub fn version(mut self, v: &str) -> Self {
+        self.0 = self.0.map_args(|args| args.with_version(v));
+        self
+    }
 }
 
 impl Future for FutureStat {
     type Output = Result<Metadata>;
 
     fn poll(mut self: Pin<&mut Self>, cx: &mut Context<'_>) -> Poll<Self::Output> {
         self.0.poll_unpin(cx)
@@ -353,14 +359,20 @@
     }
 
     /// Set the If-None-Match for this operation.
     pub fn if_none_match(mut self, v: &str) -> Self {
         self.0 = self.0.map_args(|args| args.with_if_none_match(v));
         self
     }
+
+    /// Set the version for this operation.
+    pub fn version(mut self, v: &str) -> Self {
+        self.0 = self.0.map_args(|args| args.with_version(v));
+        self
+    }
 }
 
 impl Future for FutureRead {
     type Output = Result<Vec<u8>>;
 
     fn poll(mut self: Pin<&mut Self>, cx: &mut Context<'_>) -> Poll<Self::Output> {
         self.0.poll_unpin(cx)
@@ -504,14 +516,35 @@
     type Output = Result<Writer>;
 
     fn poll(mut self: Pin<&mut Self>, cx: &mut Context<'_>) -> Poll<Self::Output> {
         self.0.poll_unpin(cx)
     }
 }
 
+/// Future that generated by [`Operator::delete_with`].
+///
+/// Users can add more options by public functions provided by this struct.
+pub struct FutureDelete(pub(crate) OperatorFuture<OpDelete, ()>);
+
+impl FutureDelete {
+    /// Change the version of this delete operation.
+    pub fn version(mut self, v: &str) -> Self {
+        self.0 = self.0.map_args(|args| args.with_version(v));
+        self
+    }
+}
+
+impl Future for FutureDelete {
+    type Output = Result<()>;
+
+    fn poll(mut self: Pin<&mut Self>, cx: &mut Context<'_>) -> Poll<Self::Output> {
+        self.0.poll_unpin(cx)
+    }
+}
+
 /// Future that generated by [`Operator::list_with`].
 ///
 /// Users can add more options by public functions provided by this struct.
 pub struct FutureList(pub(crate) OperatorFuture<OpList, Lister>);
 
 impl FutureList {
     /// Change the limit of this list operation.
```

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/scheme.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.38.1/local_dependencies/opendal/src/types/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/Cargo.toml` & `opendal-0.38.1/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.38.0"
+version= "0.38.1"
+resolver = "2"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 futures = "0.3.28"
```

### Comparing `opendal-0.38.0/.gitignore` & `opendal-0.38.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/CONTRIBUTING.md` & `opendal-0.38.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/README.md` & `opendal-0.38.1/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/benchmark/README.md` & `opendal-0.38.1/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/benchmark/async_opendal_benchmark.py` & `opendal-0.38.1/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.38.1/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/examples/object.ipynb` & `opendal-0.38.1/examples/object.ipynb`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/pyproject.toml` & `opendal-0.38.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/python/opendal/__init__.py` & `opendal-0.38.1/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/python/opendal/__init__.pyi` & `opendal-0.38.1/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/src/asyncio.rs` & `opendal-0.38.1/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/src/layers.rs` & `opendal-0.38.1/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/src/lib.rs` & `opendal-0.38.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/tests/binding.feature` & `opendal-0.38.1/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/tests/steps/binding.py` & `opendal-0.38.1/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.38.0/Cargo.lock` & `opendal-0.38.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
 name = "ahash"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.10",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -35,44 +56,38 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstream"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
- "anstyle 1.0.0",
+ "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23ea9e81bd02e310c216d080f6223c179012256e5151c41db88d12c88a1684d2"
-
-[[package]]
-name = "anstyle"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
+checksum = "938874ff5980b03a87c5524b3ae5b59cf99b1d6bc836848df7bc5ada9643c333"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
 version = "1.0.0"
@@ -84,15 +99,15 @@
 
 [[package]]
 name = "anstyle-wincon"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
- "anstyle 1.0.0",
+ "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -101,20 +116,14 @@
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
-name = "array-init"
-version = "2.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d62b7694a562cdf5a74227903507c56ab2cc8bdd1f781ed5cb4cf9c9f810bfc"
-
-[[package]]
 name = "assert-json-diff"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "47e4f2b81832e72834d7518d8487a0396a28cc408186a2e8854c0f98011faf12"
 dependencies = [
  "serde",
  "serde_json",
@@ -122,18 +131,18 @@
 
 [[package]]
 name = "assert_cmd"
 version = "2.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86d6b683edf8d1119fe420a94f8a7e389239666aa72e65495d91c00462510151"
 dependencies = [
- "anstyle 1.0.0",
- "bstr 1.4.0",
+ "anstyle",
+ "bstr 1.5.0",
  "doc-comment",
- "predicates 3.0.1",
+ "predicates",
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "async-channel"
@@ -157,17 +166,17 @@
  "once_cell",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.5.0"
+version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17adb73da160dfb475c183343c8cccd80721ea5a605d3eb57125f0a7b7a92d0b"
+checksum = "6fa3dc5f2a8564f07759c008b9109dc0d39de92a88d5588b8a5036d286383afb"
 dependencies = [
  "async-lock",
  "async-task",
  "concurrent-queue",
  "fastrand",
  "futures-lite",
  "slab",
@@ -186,30 +195,30 @@
  "blocking",
  "futures-lite",
  "once_cell",
 ]
 
 [[package]]
 name = "async-io"
-version = "1.12.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c374dda1ed3e7d8f0d9ba58715f924862c63eae6849c92d3a18e7fbde9e2794"
+checksum = "0fc5b45d93ef0529756f812ca52e44c221b35341892d3dcc34132ac02f3dd2af"
 dependencies = [
  "async-lock",
  "autocfg",
+ "cfg-if",
  "concurrent-queue",
  "futures-lite",
- "libc",
  "log",
  "parking",
  "polling",
+ "rustix 0.37.22",
  "slab",
- "socket2",
+ "socket2 0.4.9",
  "waker-fn",
- "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "async-lock"
 version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa24f727524730b077666307f2734b4a1a1c57acb79193127dcc8914d5242dd7"
@@ -258,15 +267,15 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "async-task"
 version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ecc7ab41815b3c653ccd2978ec3255c81349336702dfdf62ee6f7069b12a3aae"
@@ -282,28 +291,28 @@
  "rustls 0.19.1",
  "webpki",
  "webpki-roots",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "7b2d0f03b3640e3a630367e40c468cb7f309529c708ed1d88597047b0e7c6ef7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "atomic-waker"
-version = "1.1.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "debc29dde2e69f9e47506b525f639ed42300fc014a3e007832592448fa8e4599"
+checksum = "1181e1e0d1fce796a03db1ae795d67167da795f9cf4a39c37589e85ef57f26d3"
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
@@ -381,47 +390,62 @@
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
 name = "backon"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f34fac4d7cdaefa2deded0eda2d5d59dbfd43370ff3f856209e72340ae84c294"
+checksum = "0c1a6197b2120bb2185a267f6515038558b019e92b832bb0320e96d66268dcf9"
 dependencies = [
- "futures",
+ "fastrand",
+ "futures-core",
  "pin-project",
- "rand 0.8.5",
  "tokio",
 ]
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
 [[package]]
 name = "bb8"
-version = "0.8.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1627eccf3aa91405435ba240be23513eeca466b5dc33866422672264de061582"
+checksum = "98b4b0f25f18bcdc3ac72bdb486ed0acf7e185221fd4dc985bc15db5800b0ba2"
 dependencies = [
  "async-trait",
  "futures-channel",
  "futures-util",
  "parking_lot 0.12.1",
  "tokio",
 ]
@@ -469,78 +493,79 @@
  "peeking_take_while",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.0.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "487f1e0fcbe47deb8b0574e646def1c903389d95241dd1bbcc6ce4a715dfc0c1"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "blocking"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c67b173a56acffd6d2326fb7ab938ba0b00a71480e14902b2591c87bc5741e8"
+checksum = "77231a1c8f801696fc0123ec6150ce92cffb8e164a02afb9c8ddee0e9b65ad65"
 dependencies = [
  "async-channel",
  "async-lock",
  "async-task",
  "atomic-waker",
  "fastrand",
  "futures-lite",
+ "log",
 ]
 
 [[package]]
 name = "bstr"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "bstr"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d4260bcc2e8fc9df1eac4919a720effeb63a3f0952f5bf4944adfa18897f09"
+checksum = "a246e68bb43f6cd9db24bea052a53e40405417c5fb372e3d1a8a7f770a564ef5"
 dependencies = [
  "memchr",
  "once_cell",
  "regex-automata",
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bytecount"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c676a478f63e9fa2dd5368a42f28bba0d6c560b775f38583c8bbaa7fcd67c9c"
 
@@ -629,21 +654,21 @@
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cbindgen"
-version = "0.24.3"
+version = "0.24.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6358dedf60f4d9b8db43ad187391afe959746101346fe51bb978126bec61dfb"
+checksum = "4b922faaf31122819ec80c4047cc684c6979a087366c069611e33649bf98e18d"
 dependencies = [
- "clap 3.2.23",
+ "clap 3.2.25",
  "heck",
- "indexmap",
+ "indexmap 1.9.3",
  "log",
  "proc-macro2",
  "quote",
  "serde",
  "serde_json",
  "syn 1.0.109",
  "tempfile",
@@ -678,141 +703,130 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clang-sys"
-version = "1.6.0"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ed9a53e5d4d9c573ae844bfac6872b159cb1d1585a83b29e7a64b7eef7332a"
+checksum = "c688fc74432808e3eb684cae8830a86be1d66a2bd58e1f248ed0960a590baf6f"
 dependencies = [
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
  "bitflags 1.3.2",
  "clap_lex 0.2.4",
- "indexmap",
+ "indexmap 1.9.3",
  "strsim",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap"
-version = "4.2.5"
+version = "4.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a1f23fa97e1d1641371b51f35535cb26959b8e27ab50d167a8b996b5bada819"
+checksum = "384e169cc618c613d5e3ca6404dda77a8685a63e08660dcc64abaf7da7cb0c7a"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.5"
+version = "4.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fdc5d93c358224b4d6867ef1356d740de2303e9892edc06c5340daeccd96bab"
+checksum = "ef137bbe35aab78bdb468ccfba75a5f4d8321ae011d34063770780545176af2d"
 dependencies = [
  "anstream",
- "anstyle 1.0.0",
- "bitflags 1.3.2",
- "clap_lex 0.4.1",
+ "anstyle",
+ "clap_lex 0.5.0",
  "once_cell",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.2.0"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
+checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
-
-[[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
@@ -828,39 +842,37 @@
  "pin-project-lite",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "concurrent-queue"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c278839b831783b70278b14df4d45e1beb1aad306c07bb796637de9a0e323e8e"
+checksum = "62ec6771ecfa0762d24683ee5a32ad78487a3d3afdc0fb8cae19d2c5deb50b7c"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "concurrent_arena"
-version = "0.1.7"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24bfeb060a299f86521bb3940344800fc861cc506356e44a273a42cb552afde5"
+checksum = "c529c2d4ecc249ae15d317c9a8b9e7d86f87e80d4417de6cfa8f4d6030f37daf"
 dependencies = [
  "arc-swap",
- "array-init",
- "const_fn_assert",
  "parking_lot 0.12.1",
  "triomphe",
 ]
 
 [[package]]
 name = "const-oid"
-version = "0.9.2"
+version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "520fbf3c07483f94e3e3ca9d0cfd913d7718ef2483d2cfd91c0d9e91474ab913"
+checksum = "6340df57935414636969091153f35f68d9f00bbc8fb4a9c6054706c213e6c6bc"
 
 [[package]]
 name = "const-random"
 version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "368a7a772ead6ce7e1de82bfb04c485f3db8ec744f72925af5735e29a22cc18e"
 dependencies = [
@@ -870,27 +882,21 @@
 
 [[package]]
 name = "const-random-macro"
 version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d7d6ab3c3a2282db210df5f02c4dab6e0a7057af0fb7ebd4070f30fe05c0ddb"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.10",
  "once_cell",
  "proc-macro-hack",
  "tiny-keccak",
 ]
 
 [[package]]
-name = "const_fn_assert"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "27d614f23f34f7b5165a77dc1591f497e2518f9cec4b4f4b92bfc4dc6cf7a190"
-
-[[package]]
 name = "convert_case"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
 dependencies = [
  "unicode-segmentation",
 ]
@@ -903,23 +909,23 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -935,15 +941,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
 dependencies = [
  "anes",
  "atty",
  "cast",
  "ciborium",
- "clap 3.2.23",
+ "clap 3.2.25",
  "criterion-plot",
  "futures",
  "itertools",
  "lazy_static",
  "num-traits",
  "oorandom",
  "plotters",
@@ -965,17 +971,17 @@
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -986,30 +992,30 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
@@ -1033,55 +1039,21 @@
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "cxx"
-version = "1.0.93"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c00419335c41018365ddf7e4d5f1c12ee3659ddcf3e01974650ba1de73d038"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.93"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb8307ad413a98fff033c8545ecf133e3257747b3bae935e7602aab8aa92d4ca"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn 2.0.16",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.93"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "edc52e2eb08915cb12596d29d55f0b5384f00d697a646dbd269b6ecb0fbd9d31"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.93"
+name = "ctor"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "631569015d0d8d54e6c241733f944042623ab6df7bc3be7466874b05fcdb1c5f"
+checksum = "eed5fff0d93c7559121e9c72bf9c242295869396255071ff2cb1617147b608c5"
 dependencies = [
- "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
@@ -1121,22 +1093,22 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
  "hashbrown 0.12.3",
  "lock_api",
  "once_cell",
- "parking_lot_core 0.9.7",
+ "parking_lot_core 0.9.8",
 ]
 
 [[package]]
 name = "data-encoding"
-version = "2.3.3"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23d8666cb01533c39dde32bcbab8e227b4ed6679b2c925eba05feabea39508fb"
+checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
 
 [[package]]
 name = "deadpool"
 version = "0.9.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "421fe0f90f2ab22016f32a9881be5134fdd71c65298917084b0c7477cbc3856e"
 dependencies = [
@@ -1151,17 +1123,17 @@
 name = "deadpool-runtime"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eaa37046cc0f6c3cc6090fbdbf73ef0b8ef4cfcc37f6befc0020f63e8cf121e1"
 
 [[package]]
 name = "der"
-version = "0.7.6"
+version = "0.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56acb310e15652100da43d130af8d97b509e95af61aab1c5a7939ef24337ee17"
+checksum = "0c7ed52955ce76b1554f509074bb357d3fb8ac9b51288a65a3fd480d1dfba946"
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
@@ -1185,17 +1157,17 @@
 name = "difflib"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6184e33543162437515c2e2b48714794e37845ec9851711914eec9d308f6ebe8"
 
 [[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "const-oid",
  "crypto-common",
  "subtle",
 ]
 
@@ -1253,17 +1225,17 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "dotenvy"
-version = "0.15.6"
+version = "0.15.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03d8c417d7a8cb362e0c37e5d815f5eb7c37f79ff93707329d5a194e42e54ca0"
+checksum = "1aaf95b3e5c8f23aa320147307562d361db0ae0d51242340f558153b4eb2439b"
 
 [[package]]
 name = "downcast-rs"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
 
@@ -1304,25 +1276,42 @@
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88bffebc5d80432c9b140ee17875ff173a8ab62faad5b257da912bd2f6c1c0a1"
+
+[[package]]
 name = "errno"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
  "cc",
  "libc",
@@ -1386,17 +1375,17 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "fs2"
 version = "0.4.3"
@@ -1453,17 +1442,17 @@
 name = "futures-io"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-lite"
-version = "1.12.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7694489acd39452c77daa48516b894c153f192c3578d5a839b62c58099fcbf48"
+checksum = "49a9d51ce47660b1e808d3c990b4709f2f415d928835a17dfd16991515c46bce"
 dependencies = [
  "fastrand",
  "futures-core",
  "futures-io",
  "memchr",
  "parking",
  "pin-project-lite",
@@ -1474,15 +1463,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1524,17 +1513,17 @@
 checksum = "c31b6d751ae2c7f11320402d34e41349dd1016f8d5d45e48c4312bc8625af50c"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
@@ -1545,24 +1534,30 @@
  "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "gloo-timers"
@@ -1592,25 +1587,25 @@
  "quanta 0.9.3",
  "rand 0.8.5",
  "smallvec",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.16"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5be7b54589b581f624f566bf5d8eb2bab1db736c51528720b6bd36b96b55924d"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap",
+ "indexmap 1.9.3",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
@@ -1628,14 +1623,20 @@
 [[package]]
 name = "hashbrown"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 
 [[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+
+[[package]]
 name = "hdfs-sys"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73dcfda0dbca0569e98b8bfb87028d83d2f07705587bac1fddea7dc9ee1eca13"
 dependencies = [
  "cc",
 ]
@@ -1644,15 +1645,15 @@
 name = "hdrs"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "70a8d6dab41a27fd3825810f6413f16f15733c84114504e41955516e4156676c"
 dependencies = [
  "async-lock",
  "blocking",
- "errno",
+ "errno 0.2.8",
  "futures",
  "hdfs-sys",
  "libc",
  "log",
 ]
 
 [[package]]
@@ -1668,23 +1669,14 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
@@ -1785,45 +1777,45 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "0.14.25"
+version = "0.14.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc5e554ff619822309ffd57d8734d77cd5ce6238bc956f037ea06c58238c9899"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2",
+ "socket2 0.4.9",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
 name = "hyper-rustls"
 version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0646026eb1b3eea4cd9ba47912ea5ce9cc07713d105b1a14698f4e6433d348b7"
 dependencies = [
  "http",
  "hyper",
- "rustls 0.21.1",
+ "rustls 0.21.2",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
 name = "hyper-tls"
 version = "0.5.0"
@@ -1835,34 +1827,33 @@
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.54"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
@@ -1876,33 +1867,43 @@
  "matches",
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+dependencies = [
+ "equivalent",
+ "hashbrown 0.14.0",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "infer"
@@ -1923,67 +1924,66 @@
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09270fd4fa1111bc614ed2246c7ef56239a3063d5be0d1ec3b589c505d400aeb"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipconfig"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd302af1b90f2463a98fa5ad469fc212c8e3175a41c3068601bfa2727591c5be"
+checksum = "b58db92f96b720de98181bbbe63c831e87005ab460c1bf306eb2622b4707997f"
 dependencies = [
- "socket2",
+ "socket2 0.5.3",
  "widestring",
- "winapi",
- "winreg",
+ "windows-sys 0.48.0",
+ "winreg 0.50.0",
 ]
 
 [[package]]
 name = "ipnet"
-version = "2.7.1"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30e22bd8629359895450b59ea7a776c850561b96a3b1d31321c1949d9e6c9146"
+checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.5"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8687c819457e979cc940d09cb16e42a1bf70aa6b60a549de6d3a62a0ee90c69e"
+checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
 dependencies = [
  "hermit-abi 0.3.1",
- "io-lifetimes",
- "rustix",
- "windows-sys 0.45.0",
+ "rustix 0.38.2",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "jni"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a87aa2bb7d2af34197c04845522473242e1aa17c12f4935d5856491a7fb8c97"
 dependencies = [
@@ -2010,28 +2010,28 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "jsonwebtoken"
 version = "8.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6971da4d9c3aa03c3d8f3ff0f4155b534aad021292003895a469716b2a230378"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.2",
  "pem",
  "ring",
  "serde",
  "serde_json",
  "simple_asn1",
 ]
 
@@ -2096,17 +2096,17 @@
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "librocksdb-sys"
 version = "0.11.0+8.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3386f101bcb4bd252d8e9d2fb41ec3b0862a15a62b478c355b2982efa469e3e"
 dependencies = [
@@ -2120,133 +2120,127 @@
 
 [[package]]
 name = "libtest-mimic"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d8de370f98a6cb8a4606618e53e802f93b094ddec0f96988eaec2c27e6e9ce7"
 dependencies = [
- "clap 4.2.5",
+ "clap 4.3.10",
  "termcolor",
  "threadpool",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.8"
+version = "1.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9702761c3935f8cc2f101793272e202c72b99da8f4224a19ddcf1279a6450bbf"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
 dependencies = [
  "cc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+
+[[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+
+[[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 dependencies = [
- "cfg-if",
  "value-bag",
 ]
 
 [[package]]
 name = "lru-cache"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e24f1ad8321ca0e8a1e0ac13f23cb668e6f5466c2c57319f6a5cf1cc8e3b1c"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
-name = "lua-src"
-version = "546.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cb00c1380f1b4b4928dd211c07301ffa34872a239e590bd3219d9e5b213face"
-dependencies = [
- "cc",
-]
-
-[[package]]
-name = "luajit-src"
-version = "210.4.5+resty2cf5186"
+name = "mach"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "27b7992a40e602786272d84c6f2beca44a588ededcfd57b48ec6f82008a7cb97"
+checksum = "b823e83b2affd8f40a9ee8c29dbc56404c1e34cd2710921f2801e2cf29527afa"
 dependencies = [
- "cc",
+ "libc",
 ]
 
 [[package]]
-name = "mach"
-version = "0.3.2"
+name = "mach2"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b823e83b2affd8f40a9ee8c29dbc56404c1e34cd2710921f2801e2cf29527afa"
+checksum = "6d0d1830bcd151a6fc4aea1369af235b36c1528fe976b8ff678683c9995eade8"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "madsim"
-version = "0.2.21"
+version = "0.2.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d3f6f28042419b0a63a7db6a8b4f74db021453d567f76cdbfd81494eeec0b22"
+checksum = "7777a8bc4e68878b6e5433ac7b9bc196d9ccdfeef1f7cb3d23193cb997a520c9"
 dependencies = [
  "ahash",
  "async-channel",
  "async-stream",
  "async-task",
  "bincode",
  "bytes",
  "downcast-rs",
  "futures-util",
  "lazy_static",
  "libc",
  "madsim-macros",
  "naive-timer",
+ "panic-message",
  "rand 0.8.5",
  "rand_xoshiro",
  "rustversion",
  "serde",
  "spin 0.9.8",
  "tokio",
  "tokio-util",
- "toml 0.7.3",
+ "toml 0.7.5",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "madsim-macros"
 version = "0.2.12"
@@ -2257,29 +2251,29 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "magnus"
-version = "0.5.2"
+version = "0.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3fda351681130b40996b3e40592565b5e44ef1a677c45ea3768ed223b5918a5"
+checksum = "b560c3c0284c9ec7c30b7ba823896387423225add3f107213a794b73853c7505"
 dependencies = [
  "bytes",
  "magnus-macros",
  "rb-sys",
  "rb-sys-env",
 ]
 
 [[package]]
 name = "magnus-macros"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85aa71c9891b2732ff1157e1860a1ee578459fd25811fd3d72cc6e32b3fbdfea"
+checksum = "6cc17af1d45442c011aa579d727ec6cff8a69aea8a6bbad26736e7112d749bfb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -2339,22 +2333,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "metrics"
 version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b9b8653cec6897f73b519a43fba5ee3d50f62fe9af80b428accdcc093b4a849"
 dependencies = [
  "ahash",
  "metrics-macros",
- "portable-atomic",
+ "portable-atomic 0.3.20",
 ]
 
 [[package]]
 name = "metrics-macros"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "731f8ecebd9f3a4aa847dfe75455e4757a45da40a7793d2f0b1f9b6ed18b23f3"
@@ -2380,15 +2383,15 @@
 name = "miette-derive"
 version = "5.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4901771e1d44ddb37964565c654a3223ba41a594d02b8da471cc4464912b5cfa"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
@@ -2437,46 +2440,52 @@
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
 name = "minstant"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc5dcfca9a0725105ac948b84cfeb69c3942814c696326743797215413f854b9"
 dependencies = [
- "ctor",
+ "ctor 0.1.26",
  "libc",
  "wasi 0.7.0",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
- "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mlua"
 version = "0.8.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07366ed2cd22a3b000aed076e2b68896fb46f06f1f5786c5962da73c0af01577"
 dependencies = [
  "bstr 0.2.17",
  "cc",
- "lua-src",
- "luajit-src",
  "mlua_derive",
  "num-traits",
  "once_cell",
  "pkg-config",
  "rustc-hash",
 ]
 
@@ -2489,28 +2498,28 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "moka"
-version = "0.10.0"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b6446f16d504e3d575df79cabb11bfbe9f24b17e9562d964a815db7b28ae3ec"
+checksum = "e0d3b8e76a2e4b17de765db9432e377a171c42fbe0512b8bc860ff1bfe2e273b"
 dependencies = [
  "async-io",
  "async-lock",
  "crossbeam-channel",
  "crossbeam-epoch",
  "crossbeam-utils",
  "futures-util",
  "num_cpus",
  "once_cell",
  "parking_lot 0.12.1",
- "quanta 0.10.1",
+ "quanta 0.11.1",
  "rustc_version",
  "scheduled-thread-pool",
  "skeptic",
  "smallvec",
  "tagptr",
  "thiserror",
  "triomphe",
@@ -2521,50 +2530,51 @@
 name = "naive-timer"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "034a0ad7deebf0c2abcf2435950a6666c3c15ea9d8fad0c0f48efa8a7f843fed"
 
 [[package]]
 name = "napi"
-version = "2.12.0"
+version = "2.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "564ad12389dd08b0f5e95b9e8b5e88e5e42a234d326639cfa7b0fe643562e0d7"
+checksum = "0ede2d12cd6fce44da537a4be1f5510c73be2506c2e32dfaaafd1f36968f3a0e"
 dependencies = [
- "bitflags 2.0.2",
- "ctor",
+ "bitflags 2.3.3",
+ "ctor 0.2.3",
  "napi-derive",
  "napi-sys",
  "once_cell",
  "tokio",
 ]
 
 [[package]]
 name = "napi-build"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "882a73d9ef23e8dc2ebbffb6a6ae2ef467c0f18ac10711e4cc59c5485d41df0e"
 
 [[package]]
 name = "napi-derive"
-version = "2.12.2"
+version = "2.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6bd0beb0ac7e8576bc92d293361a461b42eaf41740bbdec7e0cbf64d8dc89f7"
+checksum = "da1c6a8fa84d549aa8708fcd062372bf8ec6e849de39016ab921067d21bde367"
 dependencies = [
+ "cfg-if",
  "convert_case",
  "napi-derive-backend",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "napi-derive-backend"
-version = "1.0.48"
+version = "1.0.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c713ff9ff5baa6d6ad9aedc46fad73c91e2f16ebe5ece0f41983d4e70e020c7c"
+checksum = "20bbc7c69168d06a848f925ec5f0e0997f98e8c8d4f2cc30157f0da51c009e17"
 dependencies = [
  "convert_case",
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
  "semver",
@@ -2645,17 +2655,17 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint-dig"
-version = "0.8.2"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2399c9463abc5f909349d8aa9ba080e0b88b3ce2885389b60b993f39b1a56905"
+checksum = "dc84195820f291c7697304f3cbdadd1cb7199c0efc917ff5eafd71225c136151"
 dependencies = [
  "byteorder",
  "lazy_static",
  "libm",
  "num-integer",
  "num-iter",
  "num-traits",
@@ -2704,50 +2714,59 @@
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi 0.3.1",
  "libc",
 ]
 
 [[package]]
 name = "oay"
-version = "0.38.0"
+version = "0.38.1"
 dependencies = [
  "anyhow",
  "axum",
  "chrono",
- "clap 4.2.5",
+ "clap 4.3.10",
  "dirs 5.0.1",
  "futures",
  "opendal",
  "quick-xml 0.27.1",
  "serde",
  "tokio",
- "toml 0.7.3",
+ "toml 0.7.5",
  "tower",
  "tower-http",
  "tracing",
  "tracing-subscriber",
  "url",
  "uuid",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "object_store"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1ea8f683b4f89a64181393742c041520a1a87e9775e6b4c0dd5a3281af05fc6"
+checksum = "ec9cd6ca25e796a49fa242876d1c4de36a24a6da5258e9f0bc062dbf5e81c53b"
 dependencies = [
  "async-trait",
  "bytes",
  "chrono",
  "futures",
  "itertools",
  "parking_lot 0.12.1",
@@ -2757,65 +2776,65 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.38.0"
+version = "0.38.1"
 dependencies = [
  "async-trait",
  "bytes",
  "futures",
  "object_store",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "oli"
-version = "0.38.0"
+version = "0.38.1"
 dependencies = [
  "anyhow",
  "assert_cmd",
- "clap 4.2.5",
+ "clap 4.3.10",
  "dirs 5.0.1",
  "env_logger",
  "futures",
  "log",
  "opendal",
- "predicates 2.1.5",
+ "predicates",
  "serde",
  "tokio",
- "toml 0.7.3",
+ "toml 0.7.5",
  "url",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.38.0"
+version = "0.38.1"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
- "base64 0.21.0",
+ "base64 0.21.2",
  "bb8",
  "bytes",
  "cacache",
  "chrono",
  "criterion",
  "dashmap",
  "dirs 5.0.1",
@@ -2866,15 +2885,15 @@
  "tracing-subscriber",
  "uuid",
  "wiremock",
 ]
 
 [[package]]
 name = "opendal-c"
-version = "0.38.0"
+version = "0.38.1"
 dependencies = [
  "bytes",
  "cbindgen",
  "opendal",
 ]
 
 [[package]]
@@ -2890,15 +2909,15 @@
 dependencies = [
  "chrono",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-java"
-version = "0.38.0"
+version = "0.38.1"
 dependencies = [
  "anyhow",
  "jni",
  "num_cpus",
  "once_cell",
  "opendal",
  "tokio",
@@ -2910,26 +2929,26 @@
 dependencies = [
  "mlua",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.38.0"
+version = "0.38.1"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.38.0"
+version = "0.38.1"
 dependencies = [
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
 ]
@@ -2958,17 +2977,17 @@
  "thiserror",
  "tokio",
  "tokio-pipe",
 ]
 
 [[package]]
 name = "openssh-sftp-client"
-version = "0.13.5"
+version = "0.13.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "866d0eab409a2fcb6b8c3838fdbf10d7399d486548c19179a80f1c1142e93348"
+checksum = "1a88d72ccea61738948673f736b3c7f0abef0c268e61622ef61f069c963aba46"
 dependencies = [
  "bytes",
  "derive_destructure2",
  "futures-core",
  "once_cell",
  "openssh",
  "openssh-sftp-client-lowlevel",
@@ -3014,15 +3033,15 @@
 
 [[package]]
 name = "openssh-sftp-protocol"
 version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf38532d784978966f95d241226223823f351d5bb2a4bebcf6b20b9cb1e393e0"
 dependencies = [
- "bitflags 2.0.2",
+ "bitflags 2.3.3",
  "num-derive",
  "num-traits",
  "openssh-sftp-protocol-error",
  "serde",
  "ssh_format",
  "vec-strings",
 ]
@@ -3036,60 +3055,59 @@
  "serde",
  "thiserror",
  "vec-strings",
 ]
 
 [[package]]
 name = "openssl"
-version = "0.10.47"
+version = "0.10.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8b277f87dacc05a6b709965d1cbafac4649d6ce9f3ce9ceb88508b5666dfec9"
+checksum = "345df152bc43501c5eb9e4654ff05f794effb78d4efe3d53abc158baddc0703d"
 dependencies = [
  "bitflags 1.3.2",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.25.2+1.1.1t"
+version = "111.26.0+1.1.1u"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "320708a054ad9b3bf314688b5db87cf4d6683d64cfc835e2337924ae62bf4431"
+checksum = "efc62c9f12b22b8f5208c23a7200a442b2e5999f8bdf80233852122b5a4f6f37"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.82"
+version = "0.9.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a95792af3c4e0153c3914df2261bedd30a98476f94dc892b67dfe1d89d433a04"
+checksum = "374533b0e45f3a7ced10fcaeccca020e66656bc03dac384f852e4e5a7a8104a6"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -3151,15 +3169,15 @@
 name = "opentelemetry_api"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed41783a5bf567688eb38372f2b7a8530f5a607a4b49d38dd7573236c23ca7e2"
 dependencies = [
  "futures-channel",
  "futures-util",
- "indexmap",
+ "indexmap 1.9.3",
  "once_cell",
  "pin-project-lite",
  "thiserror",
  "urlencoding",
 ]
 
 [[package]]
@@ -3203,17 +3221,17 @@
 dependencies = [
  "dlv-list",
  "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "os_str_bytes"
-version = "6.5.0"
+version = "6.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
+checksum = "4d5d9eb14b174ee9aa2ef96dc2b94637a2d4b6e7cb873c7e171f0c20c6cf3eac"
 
 [[package]]
 name = "output_vt100"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "628223faebab4e3e40667ee0b2336d34a5b960ff60ea743ddfdbcf7770bcfb66"
 dependencies = [
@@ -3223,18 +3241,24 @@
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
+name = "panic-message"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "384e52fd8fbd4cbe3c317e8216260c21a0f9134de108cea8a4dd4e7e152c472d"
+
+[[package]]
 name = "parking"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
+checksum = "14f2252c834a40ed9bb5422029649578e63aa341ac401f74e719dd1afda8394e"
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
 dependencies = [
@@ -3246,49 +3270,49 @@
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core 0.9.7",
+ "parking_lot_core 0.9.8",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
 dependencies = [
  "cfg-if",
  "instant",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+checksum = "b4b27ab7be369122c218afc2079489cdcb4b517c0a3fc386ff11e1fedfcc2b35"
 
 [[package]]
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
@@ -3308,43 +3332,43 @@
 checksum = "88b39c9bfcfc231068454382784bb460aae594343fb030d46e9f50a645418412"
 dependencies = [
  "base64ct",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -3367,101 +3391,99 @@
 dependencies = [
  "der",
  "spki",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "plotters"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2538b639e642295546c50fcd545198c9d64ee2a38620a628724a3b266d5fbf97"
+checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "193228616381fecdc1224c62e96946dfbc73ff4384fba576e052ff8c1bea8142"
+checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a81d2759aae1dae668f783c308bc5c8ebd191ff4184aaa1b37f65a6ae5a56f"
+checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
 name = "polling"
-version = "2.6.0"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e1f879b2998099c2d69ab9605d145d5b661195627eccc680002c4918a7fb6fa"
+checksum = "4b2d323e8ca7996b3e23126511a523f7e62924d93ecd5ae73b333815b0eb3dce"
 dependencies = [
  "autocfg",
  "bitflags 1.3.2",
  "cfg-if",
  "concurrent-queue",
  "libc",
  "log",
  "pin-project-lite",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "portable-atomic"
+version = "0.3.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e30165d31df606f5726b090ec7592c308a0eaf61721ff64c9a3018e344a8753e"
+dependencies = [
+ "portable-atomic 1.3.3",
 ]
 
 [[package]]
 name = "portable-atomic"
-version = "0.3.19"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26f6a7b87c2e435a3241addceeeff740ff8b7e76b74c13bf9acb17fa454ea00b"
+checksum = "767eb9f07d4a5ebcb39bbf2d452058a93c011373abf6832e24194a1c3f004794"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "predicates"
-version = "2.1.5"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59230a63c37f3e18569bdb90e4a89cbf5bf8b06fea0b84e65ea10cc4df47addd"
+checksum = "09963355b9f467184c04017ced4a2ba2d75cbcb4e7462690d388233253d4b1a9"
 dependencies = [
+ "anstyle",
  "difflib",
  "float-cmp",
  "itertools",
  "normalize-line-endings",
  "predicates-core",
  "regex",
 ]
 
 [[package]]
-name = "predicates"
-version = "3.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba7d6ead3e3966038f68caa9fc1f860185d95a793180bbcfe0d0da47b3961ed"
-dependencies = [
- "anstyle 0.3.5",
- "difflib",
- "itertools",
- "predicates-core",
-]
-
-[[package]]
 name = "predicates-core"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b794032607612e7abeb4db69adb4e33590fa6cf1149e95fd7cb00e634b92f174"
 
 [[package]]
 name = "predicates-tree"
@@ -3475,28 +3497,28 @@
 
 [[package]]
 name = "pretty_assertions"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a25e9bcb20aa780fd0bb16b72403a9064d6b3f22f026946029acb941a50af755"
 dependencies = [
- "ctor",
+ "ctor 0.1.26",
  "diff",
  "output_vt100",
  "yansi",
 ]
 
 [[package]]
 name = "prettyplease"
-version = "0.2.6"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b69d39aab54d069e7f2fe8cb970493e7834601ca2d8c65fd7bbd183578080d1"
+checksum = "9825a04601d60621feed79c4e6b56d65db77cdca55cef43b46b0de1096d1c282"
 dependencies = [
  "proc-macro2",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
@@ -3523,32 +3545,32 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "procfs"
 version = "0.14.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1de8dacb0873f77e6aefc6d71e044761fcc68060290f5b1089fcdf84626bb69"
 dependencies = [
  "bitflags 1.3.2",
  "byteorder",
  "hex",
  "lazy_static",
- "rustix",
+ "rustix 0.36.14",
 ]
 
 [[package]]
 name = "prometheus"
 version = "0.13.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "449811d15fbdf5ceb5c1144416066429cf82316e2ec8ce0c1f6f8a02e7bbcf8c"
@@ -3562,27 +3584,27 @@
  "procfs",
  "protobuf",
  "thiserror",
 ]
 
 [[package]]
 name = "prost"
-version = "0.11.8"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e48e50df39172a3e7eb17e14642445da64996989bc212b583015435d39a58537"
+checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
 name = "prost-derive"
-version = "0.11.8"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ea9b0f8cbe5e15a8a042d030bd96668db28ecb567ec37d691971ff5731d2b1b"
+checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
 dependencies = [
  "anyhow",
  "itertools",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
@@ -3591,17 +3613,17 @@
 name = "protobuf"
 version = "2.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "106dd99e98437432fed6519dedecfade6a06a73bb7b2a1e019fdd2bee5778d94"
 
 [[package]]
 name = "pulldown-cmark"
-version = "0.9.2"
+version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d9cc634bc78768157b5cbfe988ffcd1dcba95cd2b2f03a88316c08c6d00ed63"
+checksum = "77a1a2f1f0a7ecff9c31abbe177637be0e97a0aef46cf8738ece09327985d998"
 dependencies = [
  "bitflags 1.3.2",
  "memchr",
  "unicase",
 ]
 
 [[package]]
@@ -3609,15 +3631,15 @@
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot 0.12.1",
  "pyo3-build-config 0.18.3",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
@@ -3642,17 +3664,17 @@
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
@@ -3701,24 +3723,24 @@
  "wasi 0.10.0+wasi-snapshot-preview1",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "quanta"
-version = "0.10.1"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e31331286705f455e56cca62e0e717158474ff02b7936c1fa596d983f4ae27"
+checksum = "a17e662a7a8291a865152364c20c7abc5e60486ab2001e8ec10b24862de0b9ab"
 dependencies = [
  "crossbeam-utils",
  "libc",
- "mach",
+ "mach2",
  "once_cell",
  "raw-cpuid",
- "wasi 0.10.0+wasi-snapshot-preview1",
+ "wasi 0.11.0+wasi-snapshot-preview1",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
@@ -3733,27 +3755,27 @@
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quick-xml"
-version = "0.28.1"
+version = "0.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5c1a97b1bc42b1d550bfb48d4262153fe400a12bab1511821736f7eac76d7e2"
+checksum = "0ce5e73202a820a31f8a0ee32ada5e21029c81fd9e3ebf668a40832e4219d9d1"
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
@@ -3809,15 +3831,15 @@
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.10",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
@@ -3863,26 +3885,26 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "rb-sys"
-version = "0.9.78"
+version = "0.9.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91447d8cbb45afb5c915bad4dd44bd4b4e9be37648122409ceca75302cb81683"
+checksum = "939fb78db3e4f26665c1d4c7b91ca66d3578335a19aba552d4a6445811d07072"
 dependencies = [
  "rb-sys-build",
 ]
 
 [[package]]
 name = "rb-sys-build"
-version = "0.9.78"
+version = "0.9.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20673c1cfbd57b2db6c066b796352f07d241c45b210fd15b269dec54fa240380"
+checksum = "335a95eb0420d52fa94ef12019df3c2c250c6b19cbb3c60bd05cb7e9c362072c"
 dependencies = [
  "bindgen 0.62.0",
  "lazy_static",
  "proc-macro2",
  "quote",
  "regex",
  "shell-words",
@@ -3893,27 +3915,27 @@
 name = "rb-sys-env"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a35802679f07360454b418a5d1735c89716bde01d35b1560fc953c1415a0b3bb"
 
 [[package]]
 name = "redb"
-version = "1.0.0"
+version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89ccfb694235b9b5214d32756192abe324083e49363f29bc7c91a69854effe4c"
+checksum = "5b48b6e8001eaa7ac3793fbfc7444ade76fc51efa3629dee8c66629425d39595"
 dependencies = [
  "libc",
- "pyo3-build-config 0.19.0",
+ "pyo3-build-config 0.19.1",
 ]
 
 [[package]]
 name = "redis"
-version = "0.22.3"
+version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa8455fa3621f6b41c514946de66ea0531f57ca017b2e6c7cc368035ea5b46df"
+checksum = "3ea8c51b5dc1d8e5fd3350ec8167f464ec0995e79f2e90a075b63371500d557f"
 dependencies = [
  "arc-swap",
  "async-trait",
  "bytes",
  "combine",
  "futures",
  "futures-util",
@@ -3933,21 +3955,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags 1.3.2",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
- "getrandom 0.2.8",
- "redox_syscall",
+ "getrandom 0.2.10",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "reflink"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3955,58 +3986,64 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.2",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "reqsign"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6cb65eb3405f9c2de5c18bfc37338d6bbdb2c35eb8eb0e946208cbb564e4833"
 dependencies = [
  "anyhow",
  "async-trait",
- "base64 0.21.0",
+ "base64 0.21.2",
  "chrono",
  "form_urlencoded",
  "hex",
  "hmac",
  "home",
  "http",
  "jsonwebtoken",
  "log",
  "once_cell",
  "percent-encoding",
- "quick-xml 0.28.1",
+ "quick-xml 0.28.2",
  "rand 0.8.5",
  "reqwest",
  "rsa",
  "rust-ini",
  "serde",
  "serde_json",
  "sha1",
@@ -4016,15 +4053,15 @@
 
 [[package]]
 name = "reqwest"
 version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.2",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -4035,15 +4072,15 @@
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.21.1",
+ "rustls 0.21.2",
  "rustls-native-certs",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "tokio",
  "tokio-native-tls",
@@ -4052,15 +4089,15 @@
  "tower-service",
  "trust-dns-resolver",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "wasm-streams",
  "web-sys",
- "winreg",
+ "winreg 0.10.1",
 ]
 
 [[package]]
 name = "resolv-conf"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52e44394d2086d010551b14b53b1f24e31647570cd1deb0379e2c21b329aba00"
@@ -4129,14 +4166,20 @@
 checksum = "7e2a3bcec1f113553ef1c88aae6c020a369d03d55b58de9869a0908930385091"
 dependencies = [
  "cfg-if",
  "ordered-multimap",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustc_version"
@@ -4145,110 +4188,137 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.11"
+version = "0.36.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db4165c9963ab29e422d6c26fbc1d37f15bace6b2810221f9d925023480fcf0e"
+checksum = "14e4d67015953998ad0eb82887a0eb0129e18a7e2f3b7b0f6c422fddcd503d62"
 dependencies = [
  "bitflags 1.3.2",
- "errno",
+ "errno 0.3.1",
  "io-lifetimes",
  "libc",
- "linux-raw-sys",
+ "linux-raw-sys 0.1.4",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "rustix"
+version = "0.37.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8818fa822adcc98b18fedbb3632a6a33213c070556b5aa7c4c8cc21cff565c4c"
+dependencies = [
+ "bitflags 1.3.2",
+ "errno 0.3.1",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys 0.3.8",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "rustix"
+version = "0.38.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aabcb0461ebd01d6b79945797c27f8529082226cb630a9865a71870ff63532a4"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno 0.3.1",
+ "libc",
+ "linux-raw-sys 0.4.3",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "rustls"
 version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35edb675feee39aec9c99fa5ff985081995a06d594114ae14cbe797ad7b7a6d7"
 dependencies = [
  "base64 0.13.1",
  "log",
  "ring",
  "sct 0.6.1",
  "webpki",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
+checksum = "e32ca28af694bc1bbf399c33a516dbdf1c90090b8ab23c2bc24f834aa2247f5f"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct 0.7.0",
 ]
 
 [[package]]
 name = "rustls-native-certs"
-version = "0.6.2"
+version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0167bac7a9f490495f3c33013e7722b53cb087ecbe082fb0c6387c96f634ea50"
+checksum = "a9aace74cb666635c918e9c12bc0d348266037aa8eb599b5cba565709a8dff00"
 dependencies = [
  "openssl-probe",
  "rustls-pemfile",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
+checksum = "2d3987094b1d07b653b7dfdc3f70ce9a1da9c51ac18c1b06b662e4f9a0e9f4b2"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.2",
 ]
 
 [[package]]
 name = "rustls-webpki"
 version = "0.100.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "dc31bd9b61a32c31f9650d18add92aa83a49ba979c143eefd27fe7177b05bd5f"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "schannel"
-version = "0.1.21"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
 dependencies = [
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "scheduled-thread-pool"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3cbc66816425a074528352f5789333ecff06ca41b36b0b0efdfbb29edc391a19"
@@ -4259,20 +4329,14 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
-
-[[package]]
 name = "sct"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b362b83898e0e69f38515b82ee15aa80636befe47c3b6d3d89a911e78fc228ce"
 dependencies = [
  "ring",
  "untrusted",
@@ -4286,30 +4350,30 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.8.2"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a332be01508d814fed64bf28f798a146d73792121129962fdf335bb3c49a4254"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.8.0"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c9bb296072e961fcbd8853511dd39c2d8be2deb1e17c6860b1d30732b323b4"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
@@ -4318,49 +4382,50 @@
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.158"
+version = "1.0.166"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
+checksum = "d01b7404f9d441d3ad40e6a636a7782c377d2abdbe4fa2440e2edcc2f4f10db8"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.158"
+version = "1.0.166"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e801c1712f48475582b7696ac71e0ca34ebb30e09338425384269d9717c62cad"
+checksum = "5dd83d6dde2b6b2d466e14d9d1acce8816dedee94f735eac6395808b3483c6d6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_path_to_error"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7f05c1d5476066defcdfacce1f52fc3cae3af1d3089727100c02ae92e5abbe0"
+checksum = "0b1b6471d7496b051e03f1958802a73f88b947866f5146f329e47e36554f4e55"
 dependencies = [
+ "itoa",
  "serde",
 ]
 
 [[package]]
 name = "serde_qs"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4369,17 +4434,17 @@
  "percent-encoding",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.1"
+version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0efd8caf556a6cebd3b285caf480045fcc1ac04f6bd786b09a6f11af30c4fcf4"
+checksum = "96426c9936fd7a0124915f9185ea1d20aa9445cc9821142f0a73bc9207a2e186"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -4418,17 +4483,17 @@
 name = "sha1_smol"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae1a47186c03a32177042e55dbc5fd5aee900b8e0069a8d70fba96a9375cd012"
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -4465,32 +4530,32 @@
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "signature"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fe458c98333f9c8152221191a77e2a44e8325d0193484af2e9421a53019e57d"
+checksum = "5e1788eed21689f9cf370582dfc467ef36ed9c707f073528ddafa8d83e3b8500"
 dependencies = [
  "digest",
  "rand_core 0.6.4",
 ]
 
 [[package]]
 name = "simple_asn1"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adc4e5204eb1910f40f9cfa375f6f05b68c3abac4b6fd879c8ff5e7ae8a0a085"
 dependencies = [
  "num-bigint",
  "num-traits",
  "thiserror",
- "time 0.3.20",
+ "time 0.3.22",
 ]
 
 [[package]]
 name = "size"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fed904c7fb2856d868b92464fc8fa597fce366edea1a9cbfaa8cb5fe080bd6d"
@@ -4570,14 +4635,24 @@
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "socket2"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2538b18701741680e0322a2302176d3253a35388e2e62f172f64f4f16605f877"
+dependencies = [
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
 name = "spin"
@@ -4620,15 +4695,15 @@
 
 [[package]]
 name = "ssri"
 version = "9.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5327a6eb28e137e180380169adeae3ac6128438ca1e8a8dc80118f3d1812cbd"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.2",
  "digest",
  "hex",
  "miette",
  "serde",
  "sha-1",
  "sha2",
  "thiserror",
@@ -4645,17 +4720,17 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "subtle"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "suppaftp"
 version = "4.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d865bcb2d4bfea8c0ab4ca6c3f79d011ad04db5ef1fc693e720299bb60c58018"
 dependencies = [
@@ -4677,17 +4752,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -4700,29 +4775,30 @@
 name = "tagptr"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b2093cf4c8eb1e67749a6762251bc9cd836b6fc171623bd0a9d324d37af2417"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
+ "autocfg",
  "cfg-if",
  "fastrand",
- "redox_syscall",
- "rustix",
- "windows-sys 0.42.0",
+ "redox_syscall 0.3.5",
+ "rustix 0.37.22",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
@@ -4761,15 +4837,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -4809,35 +4885,35 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
@@ -4870,27 +4946,28 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.1"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
- "socket2",
+ "socket2 0.4.9",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-io-utility"
 version = "0.7.6"
@@ -4905,15 +4982,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -4930,19 +5007,19 @@
 dependencies = [
  "libc",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-rustls"
-version = "0.24.0"
+version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0d409377ff5b1e3ca6437aa86c1eb7d40c134bfec254e44c830defa92669db5"
+checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls 0.21.1",
+ "rustls 0.21.2",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4974,40 +5051,40 @@
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml"
-version = "0.7.3"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b403acf6f2bb0859c93c7f0d967cb4a75a7ac552100f9322faf64dc047669b21"
+checksum = "1ebafdf5ad1220cb59e7d17cf4d2c72015297b75b19a10472f99b89225089240"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.1"
+version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.7"
+version = "0.19.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc18466501acd8ac6a3f615dd29a3438f8ca6bb3b19537138b3106e575621274"
+checksum = "266f016b7f039eec8a1a80dfe6156b633d208b9fccca5e4db1d6775b0c4e34a7"
 dependencies = [
- "indexmap",
+ "indexmap 2.0.0",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
@@ -5024,19 +5101,19 @@
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "tower-http"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d1d42a9b3f3ec46ba828e8d376aec14592ea199f70a06a548587ecd1c4ab658"
+checksum = "a8bd22a874a2d0b70452d5597b12c537331d49060824a95f49f108994f94aa4c"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.3.3",
  "bytes",
  "futures-core",
  "futures-util",
  "http",
  "http-body",
  "http-range-header",
  "pin-project-lite",
@@ -5068,28 +5145,28 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
 name = "tracing-log"
@@ -5114,17 +5191,17 @@
  "tracing-core",
  "tracing-log",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6176eae26dd70d0c919749377897b54a9276bd7061339665dd68777926b5a70"
+checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
 dependencies = [
  "matchers",
  "nu-ansi-term",
  "once_cell",
  "regex",
  "sharded-slab",
  "smallvec",
@@ -5215,17 +5292,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -5254,20 +5331,20 @@
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
- "idna 0.3.0",
+ "idna 0.4.0",
  "percent-encoding",
  "serde",
 ]
 
 [[package]]
 name = "urlencoding"
 version = "2.1.2"
@@ -5278,38 +5355,34 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
+checksum = "d023da39d1fde5a8a3fe1f3e01ca9632ada0a63e9797de55a879d6e2236277be"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.10",
  "rand 0.8.5",
  "serde",
 ]
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
 [[package]]
 name = "value-bag"
-version = "1.0.0-alpha.9"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2209b78d1249f7e6f3293657c9779fe31ced465df091bbd433a1cf88e916ec55"
-dependencies = [
- "ctor",
- "version_check",
-]
+checksum = "d92ccd67fb88503048c01b59152a04effd0782d035a83a6d256ce6085f08f4a3"
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
@@ -5352,19 +5425,18 @@
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -5386,77 +5458,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.23",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.34"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.23",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "wasm-streams"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bbae3363c08332cadccd13b67db371814cd214c2524020932f0804b8cf7c078"
 dependencies = [
@@ -5465,17 +5537,17 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -5494,17 +5566,17 @@
 checksum = "aabe153544e473b775453675851ecc86863d2a81d786d741f6b76778f2a48940"
 dependencies = [
  "webpki",
 ]
 
 [[package]]
 name = "widestring"
-version = "0.5.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17882f045410753661207383517a6f62ec3dbeb6a4ed2acce01f0728238d1983"
+checksum = "653f141f39ec16bba3c5abe400a0c60da7468261cc2cbf36805022876bc721a8"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -5531,34 +5603,19 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
-version = "0.46.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
-dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
@@ -5568,15 +5625,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
@@ -5588,17 +5645,17 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm 0.48.0",
  "windows_aarch64_msvc 0.48.0",
  "windows_i686_gnu 0.48.0",
  "windows_i686_msvc 0.48.0",
  "windows_x86_64_gnu 0.48.0",
  "windows_x86_64_gnullvm 0.48.0",
@@ -5687,39 +5744,49 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.3.6"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23d020b441f92996c80d94ae9166e8501e59c7bb56121189dc9eab3bd8216966"
+checksum = "ca0ace3845f0d96209f0375e6d367e3eb87eb65d27d445bdc9f1843a26f39448"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
+name = "winreg"
+version = "0.50.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
+dependencies = [
+ "cfg-if",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "wiremock"
-version = "0.5.17"
+version = "0.5.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12316b50eb725e22b2f6b9c4cbede5b7b89984274d113a7440c86e5c3fc6f99b"
+checksum = "c6f71803d3a1c80377a06221e0530be02035d5b3e854af56c6ece7ac20ac441d"
 dependencies = [
  "assert-json-diff",
  "async-trait",
- "base64 0.13.1",
+ "base64 0.21.2",
  "deadpool",
  "futures",
  "futures-timer",
  "http-types",
  "hyper",
  "log",
  "once_cell",
@@ -5739,10 +5806,10 @@
 name = "yansi"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
```

### Comparing `opendal-0.38.0/PKG-INFO` & `opendal-0.38.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.38.0
+Version: 0.38.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: gevent ; extra == 'benchmark'
 Requires-Dist: greenify ; extra == 'benchmark'
 Requires-Dist: greenlet ; extra == 'benchmark'
 Requires-Dist: boto3 ; extra == 'benchmark'
```

