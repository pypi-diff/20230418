# Comparing `tmp/opendal-0.31.1.tar.gz` & `tmp/opendal-0.32.0.tar.gz`

## Comparing `opendal-0.31.1.tar` & `opendal-0.32.0.tar`

### file list

```diff
@@ -1,242 +1,249 @@
--rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 opendal-0.31.1/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    61889 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1256 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6635 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2438 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1832 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1296 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7703 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     5243 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      982 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10794 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     4392 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    22397 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6746 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    17164 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123    10062 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    16322 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    13631 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    53159 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    32402 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    12573 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     1885 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    25213 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    37934 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    11980 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3844 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3076 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    21079 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5164 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123     9283 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1181 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1548 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     1934 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     6441 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5404 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3394 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    10427 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2025 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11951 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     2020 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     4439 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15332 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4148 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4577 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     1971 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10680 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     9260 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6861 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5968 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     4049 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6387 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    27076 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123    10124 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123     9184 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     5821 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      913 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2251 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    16478 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     9557 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     3520 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2945 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     3973 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    25021 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3744 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    15973 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4206 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     2109 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    17788 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123     9004 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3463 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10014 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     2254 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123    20553 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2584 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    17767 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     3256 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    15552 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1826 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    16810 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     8862 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     2043 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     1074 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
--rw-r--r--   0     1001      123     4713 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9954 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4228 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     3350 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     7949 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    13309 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     6561 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3443 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      896 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2229 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    18807 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    21564 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     3358 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      896 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     4256 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10492 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5615 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    39368 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    27813 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     3685 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7040 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     4758 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123     5375 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123    20468 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      531 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2532 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2275 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19326 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     4679 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     2434 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2285 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     2333 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     2494 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    10799 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     6197 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    15166 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1462 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    23925 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123     8731 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3235 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    40765 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123     9437 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9603 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     5698 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123     7267 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.31.1/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-04-16 16:24:23.000000 opendal-0.31.1/.gitignore
--rw-r--r--   0     1001      123      982 2023-04-16 16:24:23.000000 opendal-0.31.1/README.md
--rw-r--r--   0     1001      123      765 2023-04-16 16:24:23.000000 opendal-0.31.1/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-04-16 16:24:23.000000 opendal-0.31.1/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-04-16 16:24:23.000000 opendal-0.31.1/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123     1665 2023-04-16 16:24:23.000000 opendal-0.31.1/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-04-16 16:24:23.000000 opendal-0.31.1/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-04-16 16:24:23.000000 opendal-0.31.1/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123    11963 2023-04-16 16:24:23.000000 opendal-0.31.1/src/asyncio.rs
--rw-r--r--   0     1001      123     3311 2023-04-16 16:24:23.000000 opendal-0.31.1/src/layers.rs
--rw-r--r--   0     1001      123    13929 2023-04-16 16:24:23.000000 opendal-0.31.1/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-04-16 16:24:23.000000 opendal-0.31.1/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-04-16 16:24:23.000000 opendal-0.31.1/tests/steps/binding.py
--rw-r--r--   0     1001      123   113336 2023-04-16 16:24:23.000000 opendal-0.31.1/Cargo.lock
--rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.31.1/PKG-INFO
+-rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 opendal-0.32.0/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    62800 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1256 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6635 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2438 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1832 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1290 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7703 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     5241 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      982 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10798 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     4392 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    22576 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6746 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    17164 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123    10078 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    16344 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    13631 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    53193 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    12128 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    32436 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    13351 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2117 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    25253 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    37956 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    12792 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3844 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3076 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    21038 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5164 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123     9291 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1181 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1548 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     6441 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5404 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3394 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    10427 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2025 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11983 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     2020 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     4439 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15332 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4148 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4577 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     1971 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10680 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     9260 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6861 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5968 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     4077 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    11671 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6387 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123    27080 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123    10124 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123     9184 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     5821 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      913 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2251 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    16283 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123     9557 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     3520 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2945 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     3973 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    23336 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123     1424 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      884 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3744 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    15980 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123     1808 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4206 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     2109 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    18489 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    11118 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3463 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10014 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     4503 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123    20557 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2584 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    15693 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     1497 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     3256 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    15552 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1826 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    16810 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123     1871 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     8689 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     2043 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     1074 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
+-rw-r--r--   0     1001      123     4713 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9954 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4228 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      857 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     3459 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     7949 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    13398 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     7025 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3443 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2261 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    18877 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    21580 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3358 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     4256 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123    10492 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      855 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     5615 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    39372 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3395 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    27531 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     3685 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7040 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     4820 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123     5375 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      854 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123    38770 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29663 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     3712 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2844 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    20472 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      531 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2532 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2275 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19320 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     4085 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     4679 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     2452 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2285 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     2333 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     2494 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    10799 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     6197 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    15166 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1462 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    23910 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123     8731 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3235 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1098 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    40763 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123    10255 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/ops.rs
+-rw-r--r--   0     1001      123     9611 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     5852 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123     7643 2023-04-18 13:34:01.000000 opendal-0.32.0/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.32.0/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-04-18 13:34:01.000000 opendal-0.32.0/.gitignore
+-rw-r--r--   0     1001      123      982 2023-04-18 13:34:01.000000 opendal-0.32.0/README.md
+-rw-r--r--   0     1001      123      765 2023-04-18 13:34:01.000000 opendal-0.32.0/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-04-18 13:34:01.000000 opendal-0.32.0/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-04-18 13:34:01.000000 opendal-0.32.0/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123     1665 2023-04-18 13:34:01.000000 opendal-0.32.0/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-04-18 13:34:01.000000 opendal-0.32.0/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-04-18 13:34:01.000000 opendal-0.32.0/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123    11963 2023-04-18 13:34:01.000000 opendal-0.32.0/src/asyncio.rs
+-rw-r--r--   0     1001      123     3311 2023-04-18 13:34:01.000000 opendal-0.32.0/src/layers.rs
+-rw-r--r--   0     1001      123    13929 2023-04-18 13:34:01.000000 opendal-0.32.0/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-04-18 13:34:01.000000 opendal-0.32.0/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-04-18 13:34:01.000000 opendal-0.32.0/tests/steps/binding.py
+-rw-r--r--   0     1001      123   117208 2023-04-18 13:34:01.000000 opendal-0.32.0/Cargo.lock
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.32.0/PKG-INFO
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/Cargo.toml` & `opendal-0.32.0/local_dependencies/opendal/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.31.1"
+version= "0.32.0"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
@@ -70,21 +70,24 @@
 # Enable all layers.
 layers-all = [
   "layers-chaos",
   "layers-metrics",
   "layers-prometheus",
   "layers-tracing",
   "layers-minitrace",
+  "layers-madsim",
 ]
 # Enable layers chaos support
 layers-chaos = ["dep:rand"]
 # Enable layers metrics support
 layers-metrics = ["dep:metrics"]
 # Enable layers prometheus support
 layers-prometheus = ["dep:prometheus"]
+# Enable layers madsim support
+layers-madsim = ["dep:madsim"]
 # Enable layers minitrace support.
 layers-minitrace = ["dep:minitrace"]
 # Enable layers tracing support.
 layers-tracing = ["dep:tracing"]
 
 services-azblob = [
   "dep:reqsign",
@@ -126,14 +129,19 @@
 services-rocksdb = ["dep:rocksdb"]
 services-s3 = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
 services-sled = ["dep:sled"]
+services-wasabi = [
+  "dep:reqsign",
+  "reqsign?/services-aws",
+  "reqsign?/reqwest_request",
+]
 services-webdav = []
 services-webhdfs = []
 
 [lib]
 bench = false
 
 [[bench]]
@@ -154,23 +162,24 @@
 flagset = "0.4"
 futures = { version = "0.3", features = ["alloc"] }
 hdrs = { version = "0.2", optional = true, features = ["async_file"] }
 http = "0.2.5"
 hyper = "0.14"
 lazy-regex = { version = "2.5.0", optional = true }
 log = "0.4"
+madsim = { version = "0.2.21", optional = true }
 md-5 = "0.10"
 metrics = { version = "0.20", optional = true }
 minitrace = { version = "0.4.0", optional = true }
 moka = { version = "0.10", optional = true, features = ["future"] }
 once_cell = "1"
 parking_lot = "0.12"
 percent-encoding = "2"
 pin-project = "1"
-prometheus = { version = "0.13", features = ["process"], optional = true}
+prometheus = { version = "0.13", features = ["process"], optional = true }
 prost = { version = "0.11", optional = true }
 quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
 redis = { version = "0.22", features = [
   "tokio-comp",
   "connection-manager",
 ], optional = true }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.32.0/local_dependencies/opendal/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,42 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.32.0] - 2023-04-18
+
+### Added
+
+- feat: Add wasabi service implementation (#2004)
+- feat: improve the readability of oli command line error output (#2016)
+- feat: add If-Match Support for OpRead, OpWrite, OpStat (#2017)
+- feat: add behavioral test for Write::abort (#2018)
+- feat: add if-match support for obs (#2023)
+- feat: Add missing functions for trace layers (#2025)
+- feat(layer): add madsim layer (#2006)
+- feat(gcs): add support for gcs append (#1801)
+
+### Changed
+
+- refactor: Rename `Create` to `CreateDir` for its behavior changed (#2019)
+
+### Fixed
+
+- fix: Cargo lock not updated (#2027)
+- fix(services/s3): Ignore empty query to make it more compatible (#2028)
+- fix(services/oss): Fix env not loaded for oss signer (#2029)
+
+### Docs
+
+- docs: fix some typos (#2022)
+- docs: add dev dependency section (#2021)
+
 ## [v0.31.1] - 2023-04-17
 
 ### Added
 
 - feat(services/azdfs): support rename (#1929)
 - test: Increate copy/move nested path test depth (#1932)
 - feat(layers): add a basic minitrace layer (#1931)
@@ -1883,14 +1911,15 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.32.0]: https://github.com/apache/incubator-opendal/compare/v0.31.1...v0.32.0
 [v0.31.1]: https://github.com/apache/incubator-opendal/compare/v0.31.0...v0.31.1
 [v0.31.0]: https://github.com/apache/incubator-opendal/compare/v0.30.5...v0.31.0
 [v0.30.5]: https://github.com/apache/incubator-opendal/compare/v0.30.4...v0.30.5
 [v0.30.4]: https://github.com/apache/incubator-opendal/compare/v0.30.3...v0.30.4
 [v0.30.3]: https://github.com/apache/incubator-opendal/compare/v0.30.2...v0.30.3
 [v0.30.2]: https://github.com/apache/incubator-opendal/compare/v0.30.1...v0.30.2
 [v0.30.1]: https://github.com/apache/incubator-opendal/compare/v0.30.0...v0.30.1
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.32.0/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/README.md` & `opendal-0.32.0/local_dependencies/opendal/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.32.0/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.32.0/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.32.0/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.32.0/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.32.0/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/examples/object.rs` & `opendal-0.32.0/local_dependencies/opendal/examples/object.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 // under the License.
 
 //! Compare opendal with other projects to find out the differences and areas that opendal can improve.
 //!
 //! All documents listed should be treated as highly biased. Because:
 //!
 //! - OpenDAL's maintainers and contributors write them.
-//! - Writers may not be familiar with the compared projects (at least not as //!familiar as with OpenDAL)
+//! - Writers may not be familiar with the compared projects (at least not as familiar with OpenDAL)
 //!
 //! Let's see OpenDAL:
 //!
 //! - [vs `object_store`][`vs_object_store`]
 
 #[doc = include_str!("vs_object_store.md")]
 pub mod vs_object_store {}
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.32.0/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 // specific language governing permissions and limitations
 // under the License.
 
 //! The core concepts of OpenDAL's public API.
 //!
 //! OpenDAL provides a unified abstraction for all storage services.
 //!
-//! There are three core concepts in OpenDAL:
+//! There are two core concepts in OpenDAL:
 //!
 //! - [`Builder`]: Build an instance of underlying services.
 //! - [`Operator`]: A bridge between underlying implementation detail and unified abstraction.
 //!
 //! If you are interested in internal implementation details, please have a look at [`internals`][super::internals].
 //!
 //! # Builder
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/features.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.32.0/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 //! #[async_trait]
 //! ```
 //!
 //! This is an attribute from [`async_trait`](https://docs.rs/async-trait/latest/async_trait/). By using this attribute, we can write the following code without use nightly feature.
 //!
 //! ```ignore
 //! pub trait Accessor {
-//!     async fn create(&self, path: &str) -> Result<()>;
+//!     async fn create_dir(&self, path: &str) -> Result<()>;
 //! }
 //! ```
 //!
 //! `async_trait` will transform the `async fn` into:
 //!
 //! ```ignore
 //! pub trait Accessor {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.32.0/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Upgrade to v0.32
+
+OpenDAL 0.32 doesn't have much breaking changes.
+
+We changed `Accessor::create` into `Accessor::create_dir`. Only users who implement `Layer` need to change.
+
 # Upgrade to v0.31
 
 In version v0.31 of OpenDAL, we made some internal refactoring to improve its compatibility with the ecosystem.
 
 ## MSRV Bump
 
 We increased the MSRV to 1.64 from v0.31 onwards. Although it is still possible to build OpenDAL under older rustc versions, we cannot guarantee that any issues related to them will be fixed.
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/complete.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files 4% similar despite different names*

```diff
@@ -90,22 +90,22 @@
     type Pager = ConcurrentLimitWrapper<A::Pager>;
     type BlockingPager = ConcurrentLimitWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         let _permit = self
             .semaphore
             .acquire()
             .await
             .expect("semaphore must be valid");
 
-        self.inner.create(path, args).await
+        self.inner.create_dir(path, args).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let permit = self
             .semaphore
             .clone()
             .acquire_owned()
@@ -186,21 +186,21 @@
             .acquire()
             .await
             .expect("semaphore must be valid");
 
         self.inner.batch(args).await
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         let _permit = self
             .semaphore
             .try_acquire()
             .expect("semaphore must be valid");
 
-        self.inner.blocking_create(path, args)
+        self.inner.blocking_create_dir(path, args)
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         let permit = self
             .semaphore
             .clone()
             .try_acquire_owned()
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files 2% similar despite different names*

```diff
@@ -78,19 +78,19 @@
         &self.inner
     }
 
     fn metadata(&self) -> AccessorInfo {
         self.meta.clone()
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         self.inner
-            .create(path, args)
+            .create_dir(path, args)
             .map_err(|err| {
-                err.with_operation(Operation::Create)
+                err.with_operation(Operation::CreateDir)
                     .with_context("service", self.meta.scheme())
                     .with_context("path", path)
             })
             .await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
@@ -232,17 +232,17 @@
             .map_err(|err| {
                 err.with_operation(Operation::Batch)
                     .with_context("service", self.meta.scheme())
             })
             .await
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.inner.blocking_create(path, args).map_err(|err| {
-            err.with_operation(Operation::BlockingCreate)
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.inner.blocking_create_dir(path, args).map_err(|err| {
+            err.with_operation(Operation::BlockingCreateDir)
                 .with_context("service", self.meta.scheme())
                 .with_context("path", path)
         })
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         self.inner
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 1% similar despite different names*

```diff
@@ -194,44 +194,44 @@
             Operation::Info,
             result
         );
 
         result
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         debug!(
             target: LOGGING_TARGET,
             "service={} operation={} path={} -> started",
             self.scheme,
-            Operation::Create,
+            Operation::CreateDir,
             path
         );
 
         self.inner
-            .create(path, args)
+            .create_dir(path, args)
             .await
             .map(|v| {
                 debug!(
                     target: LOGGING_TARGET,
                     "service={} operation={} path={} -> finished",
                     self.scheme,
-                    Operation::Create,
+                    Operation::CreateDir,
                     path
                 );
                 v
             })
             .map_err(|err| {
                 if let Some(lvl) = self.err_level(&err) {
                     log!(
                         target: LOGGING_TARGET,
                         lvl,
                         "service={} operation={} path={} -> {}: {err:?}",
                         self.scheme,
-                        Operation::Create,
+                        Operation::CreateDir,
                         path,
                         self.err_status(&err)
                     )
                 };
                 err
             })
     }
@@ -650,43 +650,43 @@
                     );
                 }
                 err
             })
             .await
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         debug!(
             target: LOGGING_TARGET,
             "service={} operation={} path={} -> started",
             self.scheme,
-            Operation::BlockingCreate,
+            Operation::BlockingCreateDir,
             path
         );
 
         self.inner
-            .blocking_create(path, args)
+            .blocking_create_dir(path, args)
             .map(|v| {
                 debug!(
                     target: LOGGING_TARGET,
                     "service={} operation={} path={} -> finished",
                     self.scheme,
-                    Operation::BlockingCreate,
+                    Operation::BlockingCreateDir,
                     path
                 );
                 v
             })
             .map_err(|err| {
                 if let Some(lvl) = self.err_level(&err) {
                     log!(
                         target: LOGGING_TARGET,
                         lvl,
                         "service={} operation={} path={} -> {}: {err:?}",
                         self.scheme,
-                        Operation::BlockingCreate,
+                        Operation::BlockingCreateDir,
                         path,
                         self.err_status(&err)
                     );
                 }
                 err
             })
     }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files 0% similar despite different names*

```diff
@@ -209,20 +209,20 @@
                 LABEL_SERVICE => service,
                 LABEL_OPERATION => Operation::Info.into_static(),
             ),
 
             requests_total_create: register_counter!(
                 METRIC_REQUESTS_TOTAL,
                 LABEL_SERVICE => service,
-                LABEL_OPERATION => Operation::Create.into_static(),
+                LABEL_OPERATION => Operation::CreateDir.into_static(),
             ),
             requests_duration_seconds_create: register_histogram!(
                 METRIC_REQUESTS_DURATION_SECONDS,
                 LABEL_SERVICE => service,
-                LABEL_OPERATION => Operation::Create.into_static(),
+                LABEL_OPERATION => Operation::CreateDir.into_static(),
             ),
 
             requests_total_read: register_counter!(
                 METRIC_REQUESTS_TOTAL,
                 LABEL_SERVICE => service,
                 LABEL_OPERATION => Operation::Read.into_static(),
             ),
@@ -318,20 +318,20 @@
                 LABEL_SERVICE => service,
                 LABEL_OPERATION => Operation::Batch.into_static(),
             ),
 
             requests_total_blocking_create: register_counter!(
                 METRIC_REQUESTS_TOTAL,
                 LABEL_SERVICE => service,
-                LABEL_OPERATION => Operation::BlockingCreate.into_static(),
+                LABEL_OPERATION => Operation::BlockingCreateDir.into_static(),
             ),
             requests_duration_seconds_blocking_create: register_histogram!(
                 METRIC_REQUESTS_DURATION_SECONDS,
                 LABEL_SERVICE => service,
-                LABEL_OPERATION => Operation::BlockingCreate.into_static(),
+                LABEL_OPERATION => Operation::BlockingCreateDir.into_static(),
             ),
 
             requests_total_blocking_read: register_counter!(
                 METRIC_REQUESTS_TOTAL,
                 LABEL_SERVICE => service,
                 LABEL_OPERATION => Operation::BlockingRead.into_static(),
             ),
@@ -456,29 +456,29 @@
         let dur = start.elapsed().as_secs_f64();
 
         self.handle.requests_duration_seconds_metadata.record(dur);
 
         result
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         self.handle.requests_total_create.increment(1);
 
         let start = Instant::now();
 
         self.inner
-            .create(path, args)
+            .create_dir(path, args)
             .map(|v| {
                 let dur = start.elapsed().as_secs_f64();
 
                 self.handle.requests_duration_seconds_create.record(dur);
 
                 v.map_err(|e| {
                     self.handle
-                        .increment_errors_total(Operation::Create, e.kind());
+                        .increment_errors_total(Operation::CreateDir, e.kind());
                     e
                 })
             })
             .await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
@@ -642,28 +642,28 @@
         result.map_err(|e| {
             self.handle
                 .increment_errors_total(Operation::Presign, e.kind());
             e
         })
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         self.handle.requests_total_blocking_create.increment(1);
 
         let start = Instant::now();
-        let result = self.inner.blocking_create(path, args);
+        let result = self.inner.blocking_create_dir(path, args);
         let dur = start.elapsed().as_secs_f64();
 
         self.handle
             .requests_duration_seconds_blocking_create
             .record(dur);
 
         result.map_err(|e| {
             self.handle
-                .increment_errors_total(Operation::BlockingCreate, e.kind());
+                .increment_errors_total(Operation::BlockingCreateDir, e.kind());
             e
         })
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         self.handle.requests_total_blocking_read.increment(1);
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::FutureExt;
 use minitrace::prelude::*;
 
 use crate::ops::*;
-use crate::raw::oio::{PageOperation, ReadOperation, WriteOperation};
+use crate::raw::oio::PageOperation;
+use crate::raw::oio::ReadOperation;
+use crate::raw::oio::WriteOperation;
 use crate::raw::*;
 use crate::*;
 
 /// Add [minitrace](https://docs.rs/minitrace/) for every operations.
 ///
 /// # Examples
 ///
@@ -142,16 +144,16 @@
 
     #[trace("metadata")]
     fn metadata(&self) -> AccessorInfo {
         self.inner.info()
     }
 
     #[trace("create", enter_on_poll = true)]
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.inner.create(path, args).await
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.inner.create_dir(path, args).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let span = Span::enter_with_local_parent("read");
         self.inner
             .read(path, args)
             .map(|v| v.map(|(rp, r)| (rp, MinitraceWrapper::new(span, r))))
@@ -162,14 +164,24 @@
         let span = Span::enter_with_local_parent("write");
         self.inner
             .write(path, args)
             .map(|v| v.map(|(rp, r)| (rp, MinitraceWrapper::new(span, r))))
             .await
     }
 
+    #[trace("copy", enter_on_poll = true)]
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.inner().copy(from, to, args).await
+    }
+
+    #[trace("rename", enter_on_poll = true)]
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.inner().rename(from, to, args).await
+    }
+
     #[trace("stat", enter_on_poll = true)]
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner.stat(path, args).await
     }
 
     #[trace("delete", enter_on_poll = true)]
     async fn delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
@@ -199,16 +211,16 @@
 
     #[trace("batch", enter_on_poll = true)]
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         self.inner.batch(args).await
     }
 
     #[trace("blocking_create")]
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.inner.blocking_create(path, args)
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.inner.blocking_create_dir(path, args)
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         let span = Span::enter_with_local_parent("blocking_read");
         self.inner.blocking_read(path, args).map(|(rp, r)| {
             (
                 rp,
@@ -223,14 +235,24 @@
             (
                 rp,
                 MinitraceWrapper::new(Span::enter_with_parent("WriteOperation", &span), r),
             )
         })
     }
 
+    #[trace("blocking_copy")]
+    fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.inner().blocking_copy(from, to, args)
+    }
+
+    #[trace("blocking_rename")]
+    fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.inner().blocking_rename(from, to, args)
+    }
+
     #[trace("blocking_stat")]
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner.blocking_stat(path, args)
     }
 
     #[trace("blocking_delete")]
     fn blocking_delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files 1% similar despite different names*

```diff
@@ -23,39 +23,38 @@
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::FutureExt;
 use futures::TryFutureExt;
 use log::debug;
-
+use prometheus::core::AtomicU64;
 use prometheus::core::GenericCounterVec;
 use prometheus::exponential_buckets;
 use prometheus::histogram_opts;
 use prometheus::register_histogram_vec_with_registry;
 use prometheus::register_int_counter_vec_with_registry;
+use prometheus::HistogramVec;
 use prometheus::Registry;
-use prometheus::{core::AtomicU64, HistogramVec};
 
 use crate::ops::*;
 use crate::raw::Accessor;
 use crate::raw::*;
 use crate::*;
 /// Add [prometheus](https://docs.rs/prometheus) for every operations.
 ///
 /// # Examples
 ///
 /// ```
 /// use log::debug;
 /// use log::info;
+/// use opendal::layers::PrometheusLayer;
 /// use opendal::services;
 /// use opendal::Operator;
 /// use opendal::Result;
-///
-/// use opendal::layers::PrometheusLayer;
 /// use prometheus::Encoder;
 ///
 /// /// Visit [`opendal::services`] for more service related config.
 /// /// Visit [`opendal::Object`] for more object level APIs.
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     // Pick a builder and configure it.
@@ -197,31 +196,31 @@
     type Pager = A::Pager;
     type BlockingPager = A::BlockingPager;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         self.stats
             .requests_total
             .with_label_values(&[&self.scheme])
             .inc();
 
         let timer = self
             .stats
             .requests_duration_seconds
-            .with_label_values(&[&self.scheme, Operation::Create.into_static()])
+            .with_label_values(&[&self.scheme, Operation::CreateDir.into_static()])
             .start_timer();
-        let create_res = self.inner.create(path, args).await;
+        let create_res = self.inner.create_dir(path, args).await;
 
         timer.observe_duration();
         create_res.map_err(|e| {
             self.stats
-                .increment_errors_total(Operation::Create, e.kind());
+                .increment_errors_total(Operation::CreateDir, e.kind());
             e
         })
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         self.stats
             .requests_total
@@ -424,32 +423,32 @@
         result.map_err(|e| {
             self.stats
                 .increment_errors_total(Operation::Presign, e.kind());
             e
         })
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         self.stats
             .requests_total
-            .with_label_values(&[&self.scheme, Operation::BlockingCreate.into_static()])
+            .with_label_values(&[&self.scheme, Operation::BlockingCreateDir.into_static()])
             .inc();
 
         let timer = self
             .stats
             .requests_duration_seconds
-            .with_label_values(&[&self.scheme, Operation::BlockingCreate.into_static()])
+            .with_label_values(&[&self.scheme, Operation::BlockingCreateDir.into_static()])
             .start_timer();
-        let result = self.inner.blocking_create(path, args);
+        let result = self.inner.blocking_create_dir(path, args);
 
         timer.observe_duration();
 
         result.map_err(|e| {
             self.stats
-                .increment_errors_total(Operation::BlockingCreate, e.kind());
+                .increment_errors_total(Operation::BlockingCreateDir, e.kind());
             e
         })
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         self.stats
             .requests_total
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/retry.rs`

 * *Files 0% similar despite different names*

```diff
@@ -164,23 +164,23 @@
     type Pager = RetryWrapper<A::Pager>;
     type BlockingPager = RetryWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        { || self.inner.create(path, args.clone()) }
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        { || self.inner.create_dir(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
                 warn!(
                     target: "opendal::service",
                     "operation={} -> retry after {}s: error={:?}",
-                    Operation::Create, dur.as_secs_f64(), err)
+                    Operation::CreateDir, dur.as_secs_f64(), err)
             })
             .map(|v| v.map_err(|e| e.set_persistent()))
             .await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         { || self.inner.read(path, args.clone()) }
@@ -318,23 +318,23 @@
                     "operation={} -> retry after {}s: error={:?}",
                     Operation::Batch, dur.as_secs_f64(), err),
             })
             .map(|v| v.unwrap_err().map_err(|e| e.set_persistent()))
             .await
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        { || self.inner.blocking_create(path, args.clone()) }
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        { || self.inner.blocking_create_dir(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
                 warn!(
                     target: "opendal::service",
                     "operation={} -> retry after {}s: error={:?}",
-                    Operation::BlockingCreate, dur.as_secs_f64(), err)
+                    Operation::BlockingCreateDir, dur.as_secs_f64(), err)
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         { || self.inner.blocking_read(path, args.clone()) }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files 6% similar despite different names*

```diff
@@ -147,16 +147,16 @@
 
     #[tracing::instrument(level = "debug")]
     fn metadata(&self) -> AccessorInfo {
         self.inner.info()
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.inner.create(path, args).await
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.inner.create_dir(path, args).await
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         self.inner
             .read(path, args)
             .map(|v| v.map(|(rp, r)| (rp, TracingWrapper::new(Span::current(), r))))
@@ -168,14 +168,24 @@
         self.inner
             .write(path, args)
             .await
             .map(|(rp, r)| (rp, TracingWrapper::new(Span::current(), r)))
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.inner().copy(from, to, args).await
+    }
+
+    #[tracing::instrument(level = "debug", skip(self))]
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.inner().rename(from, to, args).await
+    }
+
+    #[tracing::instrument(level = "debug", skip(self))]
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner.stat(path, args).await
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
     async fn delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         self.inner.delete(path, args).await
@@ -204,16 +214,16 @@
 
     #[tracing::instrument(level = "debug", skip(self))]
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         self.inner.batch(args).await
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.inner.blocking_create(path, args)
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.inner.blocking_create_dir(path, args)
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         self.inner
             .blocking_read(path, args)
             .map(|(rp, r)| (rp, TracingWrapper::new(Span::current(), r)))
@@ -223,14 +233,24 @@
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         self.inner
             .blocking_write(path, args)
             .map(|(rp, r)| (rp, TracingWrapper::new(Span::current(), r)))
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
+    fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.inner().blocking_copy(from, to, args)
+    }
+
+    #[tracing::instrument(level = "debug", skip(self))]
+    fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.inner().blocking_rename(from, to, args)
+    }
+
+    #[tracing::instrument(level = "debug", skip(self))]
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner.blocking_stat(path, args)
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
     fn blocking_delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         self.inner.blocking_delete(path, args)
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.32.0/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/lib.rs` & `opendal-0.32.0/local_dependencies/opendal/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 #[async_trait]
 pub trait Accessor: Send + Sync + Debug + Unpin + 'static {
     /// Reader is the associated reader the could return in `read` operation.
     type Reader: oio::Read;
     /// BlockingReader is the associated reader that could return in
     /// `blocking_read` operation.
     type BlockingReader: oio::BlockingRead;
-    /// Reader is the associated writer the could return in `write` operation.
+    /// Writer is the associated writer the could return in `write` operation.
     type Writer: oio::Write;
     /// BlockingWriter is the associated writer the could return in
     /// `blocking_write` operation.
     type BlockingWriter: oio::BlockingWrite;
     /// Pager is the associated page that return in `list` or `scan` operation.
     type Pager: oio::Page;
     /// BlockingPager is the associated pager that could return in
@@ -82,16 +82,15 @@
     ///
     /// Require [`AccessorCapability::Write`]
     ///
     /// # Behavior
     ///
     /// - Input path MUST match with EntryMode, DON'T NEED to check mode.
     /// - Create on existing dir SHOULD succeed.
-    /// - Create on existing file SHOULD overwrite and truncate.
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
@@ -252,15 +251,15 @@
     }
 
     /// Invoke the `blocking_create` operation on the specified path.
     ///
     /// This operation is the blocking version of [`Accessor::create`]
     ///
     /// Require [`AccessorCapability::Write`] and [`AccessorCapability::Blocking`]
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
@@ -413,16 +412,16 @@
     type Pager = T::Pager;
     type BlockingPager = T::BlockingPager;
 
     fn info(&self) -> AccessorInfo {
         self.as_ref().info()
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.as_ref().create(path, args).await
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.as_ref().create_dir(path, args).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         self.as_ref().read(path, args).await
     }
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         self.as_ref().write(path, args).await
@@ -453,16 +452,16 @@
         self.as_ref().batch(args).await
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         self.as_ref().presign(path, args).await
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.as_ref().blocking_create(path, args)
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.as_ref().blocking_create_dir(path, args)
     }
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         self.as_ref().blocking_read(path, args)
     }
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         self.as_ref().blocking_write(path, args)
     }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -64,21 +64,21 @@
         let mut am: AccessorInfo = self.kv.metadata().into();
         am.set_root(&self.root)
             .set_hints(AccessorHint::ReadStreamable | AccessorHint::ReadSeekable);
 
         am
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = build_abs_path(&self.root, path);
         self.kv.set(&p, &[]).await?;
         Ok(RpCreate::default())
     }
 
-    fn blocking_create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    fn blocking_create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = build_abs_path(&self.root, path);
         self.kv.blocking_set(&p, &[])?;
 
         Ok(RpCreate::default())
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/layer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,16 @@
 
     fn inner(&self) -> &Self::Inner;
 
     fn metadata(&self) -> AccessorInfo {
         self.inner().info()
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.inner().create(path, args).await
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.inner().create_dir(path, args).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)>;
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)>;
 
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
@@ -183,16 +183,16 @@
         self.inner().batch(args).await
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         self.inner().presign(path, args).await
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        self.inner().blocking_create(path, args)
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        self.inner().blocking_create_dir(path, args)
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)>;
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)>;
 
     fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
@@ -225,16 +225,16 @@
     type Pager = L::Pager;
     type BlockingPager = L::BlockingPager;
 
     fn info(&self) -> AccessorInfo {
         (self as &L).metadata()
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        (self as &L).create(path, args).await
+    async fn create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        (self as &L).create_dir(path, args).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         (self as &L).read(path, args).await
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
@@ -269,16 +269,16 @@
         (self as &L).batch(args).await
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         (self as &L).presign(path, args).await
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        (self as &L).blocking_create(path, args)
+    fn blocking_create_dir(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        (self as &L).blocking_create_dir(path, args)
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         (self as &L).blocking_read(path, args)
     }
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/operation.rs`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 /// Operation is the name for APIs in `Accessor`.
 #[derive(Debug, Copy, Clone, Hash, Eq, PartialEq, Default)]
 #[non_exhaustive]
 pub enum Operation {
     /// Operation for [`crate::raw::Accessor::info`]
     #[default]
     Info,
-    /// Operation for [`crate::raw::Accessor::create`]
-    Create,
+    /// Operation for [`crate::raw::Accessor::create_dir`]
+    CreateDir,
     /// Operation for [`crate::raw::Accessor::read`]
     Read,
     /// Operation for [`crate::raw::Accessor::write`]
     Write,
     /// Operation for [`crate::raw::Accessor::copy`]
     Copy,
     /// Operation for [`crate::raw::Accessor::rename`]
@@ -43,16 +43,16 @@
     List,
     /// Operation for [`crate::raw::Accessor::scan`]
     Scan,
     /// Operation for [`crate::raw::Accessor::batch`]
     Batch,
     /// Operation for [`crate::raw::Accessor::presign`]
     Presign,
-    /// Operation for [`crate::raw::Accessor::blocking_create`]
-    BlockingCreate,
+    /// Operation for [`crate::raw::Accessor::blocking_create_dir`]
+    BlockingCreateDir,
     /// Operation for [`crate::raw::Accessor::blocking_read`]
     BlockingRead,
     /// Operation for [`crate::raw::Accessor::blocking_write`]
     BlockingWrite,
     /// Operation for [`crate::raw::Accessor::blocking_copy`]
     BlockingCopy,
     /// Operation for [`crate::raw::Accessor::blocking_rename`]
@@ -80,26 +80,26 @@
     }
 }
 
 impl From<Operation> for &'static str {
     fn from(v: Operation) -> &'static str {
         match v {
             Operation::Info => "metadata",
-            Operation::Create => "create",
+            Operation::CreateDir => "create_dir",
             Operation::Read => "read",
             Operation::Write => "write",
             Operation::Copy => "copy",
             Operation::Rename => "rename",
             Operation::Stat => "stat",
             Operation::Delete => "delete",
             Operation::List => "list",
             Operation::Scan => "scan",
             Operation::Presign => "presign",
             Operation::Batch => "batch",
-            Operation::BlockingCreate => "blocking_create",
+            Operation::BlockingCreateDir => "blocking_create_dir",
             Operation::BlockingRead => "blocking_read",
             Operation::BlockingWrite => "blocking_write",
             Operation::BlockingCopy => "blocking_copy",
             Operation::BlockingMove => "blocking_rename",
             Operation::BlockingStat => "blocking_stat",
             Operation::BlockingDelete => "blocking_delete",
             Operation::BlockingList => "blocking_list",
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.32.0/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
             .set_max_batch_operations(AZBLOB_BATCH_LIMIT)
             .set_capabilities(Read | Write | List | Scan | Batch | Copy)
             .set_hints(ReadStreamable);
 
         am
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req = self
             .core
             .azblob_put_blob_request(path, Some(0), None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -315,24 +315,18 @@
                     | AccessorCapability::List,
             )
             .set_hints(AccessorHint::ReadStreamable);
 
         am
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        let resource = match args.mode() {
-            EntryMode::FILE => "file",
-            EntryMode::DIR => "directory",
-            _ => unimplemented!("not supported object mode"),
-        };
-
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req =
             self.core
-                .azdfs_create_request(path, resource, None, None, AsyncBody::Empty)?;
+                .azdfs_create_request(path, "directory", None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -309,49 +309,20 @@
                     | AccessorCapability::Blocking,
             )
             .set_hints(AccessorHint::ReadSeekable);
 
         am
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = self.root.join(path.trim_end_matches('/'));
 
-        if args.mode() == EntryMode::FILE {
-            let parent = p
-                .parent()
-                .ok_or_else(|| {
-                    Error::new(
-                        ErrorKind::Unexpected,
-                        "path should have parent but not, it must be malformed",
-                    )
-                    .with_context("input", p.to_string_lossy())
-                })?
-                .to_path_buf();
-
-            fs::create_dir_all(&parent).await.map_err(parse_io_error)?;
-
-            fs::OpenOptions::new()
-                .create(true)
-                .truncate(true)
-                .write(true)
-                .open(&p)
-                .await
-                .map_err(parse_io_error)?;
+        fs::create_dir_all(&p).await.map_err(parse_io_error)?;
 
-            return Ok(RpCreate::default());
-        }
-
-        if args.mode() == EntryMode::DIR {
-            fs::create_dir_all(&p).await.map_err(parse_io_error)?;
-
-            return Ok(RpCreate::default());
-        }
-
-        unreachable!()
+        Ok(RpCreate::default())
     }
 
     /// # Notes
     ///
     /// There are three ways to get the total file length:
     ///
     /// - call std::fs::metadata directly and than open. (400ns)
@@ -536,47 +507,20 @@
         };
 
         let rd = FsPager::new(&self.root, f, args.limit());
 
         Ok((RpList::default(), Some(rd)))
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    fn blocking_create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = self.root.join(path.trim_end_matches('/'));
 
-        if args.mode() == EntryMode::FILE {
-            let parent = p
-                .parent()
-                .ok_or_else(|| {
-                    Error::new(
-                        ErrorKind::Unexpected,
-                        "path should have parent but not, it must be malformed",
-                    )
-                    .with_context("input", p.to_string_lossy())
-                })?
-                .to_path_buf();
-
-            std::fs::create_dir_all(parent).map_err(parse_io_error)?;
-
-            std::fs::OpenOptions::new()
-                .create(true)
-                .write(true)
-                .open(&p)
-                .map_err(parse_io_error)?;
-
-            return Ok(RpCreate::default());
-        }
-
-        if args.mode() == EntryMode::DIR {
-            std::fs::create_dir_all(&p).map_err(parse_io_error)?;
-
-            return Ok(RpCreate::default());
-        }
+        std::fs::create_dir_all(p).map_err(parse_io_error)?;
 
-        unreachable!()
+        Ok(RpCreate::default())
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         use oio::BlockingRead;
 
         let p = self.root.join(path.trim_end_matches('/'));
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -319,16 +319,16 @@
             .set_capabilities(
                 AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
             );
 
         am
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let mut ftp_stream = self.ftp_connect(Operation::Create).await?;
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+        let mut ftp_stream = self.ftp_connect(Operation::CreateDir).await?;
 
         let paths: Vec<&str> = path.split_inclusive('/').collect();
 
         let mut curr_path = String::new();
 
         for path in paths {
             curr_path.push_str(path);
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
             .set_root(&self.core.root)
             .set_name(&self.core.bucket)
             .set_capabilities(Read | Write | List | Scan | Copy)
             .set_hints(ReadStreamable);
         am
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req = self
             .core
             .gcs_insert_object_request(path, Some(0), None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
@@ -406,24 +406,40 @@
             Ok((RpRead::with_metadata(meta), resp.into_body()))
         } else {
             Err(parse_error(resp).await?)
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "append write is not supported",
-            ));
-        }
+        let upload_location = if args.append() {
+            let resp = self.core.gcs_initiate_resumable_upload(path).await?;
+            let status = resp.status();
+
+            match status {
+                StatusCode::OK => {
+                    let bs = parse_location(resp.headers())
+                        .expect("Failed to retrieve location of resumable upload");
+                    if let Some(location) = bs {
+                        Some(String::from(location))
+                    } else {
+                        return Err(Error::new(
+                            ErrorKind::NotFound,
+                            "location is not in the response header",
+                        ));
+                    }
+                }
+                _ => return Err(parse_error(resp).await?),
+            }
+        } else {
+            None
+        };
 
         Ok((
             RpWrite::default(),
-            GcsWriter::new(self.core.clone(), args, path.to_string()),
+            GcsWriter::new(self.core.clone(), args, path.to_string(), upload_location),
         ))
     }
 
     async fn copy(&self, from: &str, to: &str, _: OpCopy) -> Result<RpCopy> {
         let resp = self.core.gcs_copy_object(from, to).await?;
 
         if resp.status().is_success() {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
 
 use backon::ExponentialBuilder;
 use backon::Retryable;
-use bytes::BytesMut;
-use http::header::CONTENT_LENGTH;
+use bytes::{Bytes, BytesMut};
 use http::header::CONTENT_TYPE;
+use http::header::{CONTENT_LENGTH, CONTENT_RANGE};
 use http::Request;
 use http::Response;
 use once_cell::sync::Lazy;
 use reqsign::GoogleCredentialLoader;
 use reqsign::GoogleSigner;
 use reqsign::GoogleToken;
 use reqsign::GoogleTokenLoader;
@@ -297,8 +297,81 @@
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
+
+    pub async fn gcs_initiate_resumable_upload(
+        &self,
+        path: &str,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let url = format!(
+            "{}/upload/storage/v1/b/{}/o?uploadType=resumable&name={}",
+            self.endpoint, self.bucket, p
+        );
+        let mut req = Request::post(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+        self.sign(&mut req).await?;
+        self.send(req).await
+    }
+
+    pub fn gcs_upload_in_resumable_upload(
+        &self,
+        location: &str,
+        size: u64,
+        written_bytes: u64,
+        is_last_part: bool,
+        body: AsyncBody,
+    ) -> Result<Request<AsyncBody>> {
+        let mut req = Request::put(location);
+
+        let range_header = if is_last_part {
+            format!(
+                "bytes {}-{}/{}",
+                written_bytes,
+                written_bytes + size - 1,
+                written_bytes + size
+            )
+        } else {
+            format!("bytes {}-{}/*", written_bytes, written_bytes + size - 1)
+        };
+
+        req = req
+            .header(CONTENT_LENGTH, size)
+            .header(CONTENT_RANGE, range_header);
+
+        // Set body
+        let req = req.body(body).map_err(new_request_build_error)?;
+
+        Ok(req)
+    }
+
+    pub async fn gcs_complete_resumable_upload(
+        &self,
+        location: &str,
+        written_bytes: u64,
+        bs: Bytes,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let size = bs.len() as u64;
+        let mut req = Request::post(location)
+            .header(CONTENT_LENGTH, size)
+            .header(
+                CONTENT_RANGE,
+                format!(
+                    "bytes {}-{}/{}",
+                    written_bytes,
+                    written_bytes + size - 1,
+                    written_bytes + size
+                ),
+            )
+            .body(AsyncBody::Bytes(bs))
+            .map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
 }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files 12% similar despite different names*

```diff
@@ -17,40 +17,41 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::GcsCore;
+use super::core::ObsCore;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct GcsWriter {
-    core: Arc<GcsCore>,
+pub struct ObsWriter {
+    core: Arc<ObsCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl GcsWriter {
-    pub fn new(core: Arc<GcsCore>, op: OpWrite, path: String) -> Self {
-        GcsWriter { core, op, path }
+impl ObsWriter {
+    pub fn new(core: Arc<ObsCore>, op: OpWrite, path: String) -> Self {
+        ObsWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for GcsWriter {
+impl oio::Write for ObsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.gcs_insert_object_request(
-            &percent_encode_path(&self.path),
+        let mut req = self.core.obs_put_object_request(
+            &self.path,
             Some(bs.len()),
             self.op.content_type(),
+            self.op.if_match(),
             AsyncBody::Bytes(bs),
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
             .set_root(&self.root)
             .set_name(&self.version)
             .set_capabilities(AccessorCapability::Read | AccessorCapability::Write)
             .set_hints(AccessorHint::ReadStreamable);
         am
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         // ignore creation of dir.
         if path.ends_with('/') {
             return Ok(RpCreate::default());
         }
         if !self.enable_create_simulation {
             return Err(Error::new(
                 ErrorKind::Unsupported,
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 14% similar despite different names*

```diff
@@ -239,51 +239,20 @@
                     | AccessorCapability::Blocking,
             )
             .set_hints(AccessorHint::ReadSeekable);
 
         am
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = build_rooted_abs_path(&self.root, path);
 
-        match args.mode() {
-            EntryMode::FILE => {
-                let parent = PathBuf::from(&p)
-                    .parent()
-                    .ok_or_else(|| {
-                        Error::new(
-                            ErrorKind::Unexpected,
-                            "path should have parent but not, it must be malformed",
-                        )
-                        .with_context("input", &p)
-                    })?
-                    .to_path_buf();
-
-                self.client
-                    .create_dir(&parent.to_string_lossy())
-                    .map_err(parse_io_error)?;
-
-                self.client
-                    .open_file()
-                    .create(true)
-                    .write(true)
-                    .truncate(true)
-                    .open(&p)
-                    .map_err(parse_io_error)?;
+        self.client.create_dir(&p).map_err(parse_io_error)?;
 
-                Ok(RpCreate::default())
-            }
-            EntryMode::DIR => {
-                self.client.create_dir(&p).map_err(parse_io_error)?;
-
-                Ok(RpCreate::default())
-            }
-            EntryMode::Unknown => unreachable!(),
-        }
+        Ok(RpCreate::default())
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         use oio::ReadExt;
 
         let p = build_rooted_abs_path(&self.root, path);
 
@@ -408,51 +377,20 @@
         };
 
         let rd = HdfsPager::new(&self.root, f, args.limit());
 
         Ok((RpList::default(), Some(rd)))
     }
 
-    fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+    fn blocking_create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let p = build_rooted_abs_path(&self.root, path);
 
-        match args.mode() {
-            EntryMode::FILE => {
-                let parent = PathBuf::from(&p)
-                    .parent()
-                    .ok_or_else(|| {
-                        Error::new(
-                            ErrorKind::Unexpected,
-                            "path should have parent but not, it must be malformed",
-                        )
-                        .with_context("input", &p)
-                    })?
-                    .to_path_buf();
-
-                self.client
-                    .create_dir(&parent.to_string_lossy())
-                    .map_err(parse_io_error)?;
-
-                self.client
-                    .open_file()
-                    .create(true)
-                    .write(true)
-                    .truncate(true)
-                    .open(&p)
-                    .map_err(parse_io_error)?;
+        self.client.create_dir(&p).map_err(parse_io_error)?;
 
-                Ok(RpCreate::default())
-            }
-            EntryMode::DIR => {
-                self.client.create_dir(&p).map_err(parse_io_error)?;
-
-                Ok(RpCreate::default())
-            }
-            EntryMode::Unknown => unreachable!(),
-        }
+        Ok(RpCreate::default())
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         use oio::BlockingRead;
 
         let p = build_rooted_abs_path(&self.root, path);
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/http/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -77,20 +77,16 @@
                 AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
             )
             .set_hints(AccessorHint::ReadStreamable);
 
         am
     }
 
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        let resp = match args.mode() {
-            EntryMode::DIR => self.ipmfs_mkdir(path).await?,
-            EntryMode::FILE => self.ipmfs_write(path, AsyncBody::Empty).await?,
-            _ => unreachable!(),
-        };
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+        let resp = self.ipmfs_mkdir(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(RpCreate::default())
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt` & `opendal-0.32.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,19 @@
 pub use s3::S3;
 
 #[cfg(feature = "services-sled")]
 mod sled;
 #[cfg(feature = "services-sled")]
 pub use self::sled::Sled;
 
+#[cfg(feature = "services-wasabi")]
+mod wasabi;
+#[cfg(feature = "services-wasabi")]
+pub use wasabi::Wasabi;
+
 #[cfg(feature = "services-webdav")]
 mod webdav;
 #[cfg(feature = "services-webdav")]
 pub use webdav::Webdav;
 
 #[cfg(feature = "services-webhdfs")]
 mod webhdfs;
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -310,18 +310,18 @@
             .set_name(&self.core.bucket)
             .set_capabilities(Read | Write | Copy | List | Scan)
             .set_hints(ReadStreamable);
 
         am
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let mut req = self
-            .core
-            .obs_put_object_request(path, Some(0), None, AsyncBody::Empty)?;
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+        let mut req =
+            self.core
+                .obs_put_object_request(path, Some(0), None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
@@ -331,15 +331,18 @@
                 Ok(RpCreate::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.core.obs_get_object(path, args.range()).await?;
+        let resp = self
+            .core
+            .obs_get_object(path, args.range(), args.if_match())
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
@@ -372,21 +375,21 @@
                 resp.into_body().consume().await?;
                 Ok(RpCopy::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
+    async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.core.obs_get_head_object(path).await?;
+        let resp = self.core.obs_get_head_object(path, args.if_match()).await?;
 
         let status = resp.status();
 
         // The response is very similar to azblob.
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files 20% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 
-use crate::raw::*;
-use crate::*;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::header::IF_MATCH;
 use http::Request;
 use http::Response;
 use reqsign::HuaweicloudObsCredential;
 use reqsign::HuaweicloudObsCredentialLoader;
 use reqsign::HuaweicloudObsSigner;
 
+use crate::raw::*;
+use crate::*;
+
 pub struct ObsCore {
     pub bucket: String,
     pub root: String,
     pub endpoint: String,
 
     pub signer: HuaweicloudObsSigner,
     pub loader: HuaweicloudObsCredentialLoader,
@@ -80,21 +82,26 @@
 }
 
 impl ObsCore {
     pub async fn obs_get_object(
         &self,
         path: &str,
         range: BytesRange,
+        if_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::get(&url);
 
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
         if !range.is_full() {
             req = req.header(http::header::RANGE, range.to_header())
         }
 
         let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
@@ -105,44 +112,57 @@
     }
 
     pub fn obs_put_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
+        if_match: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::put(&url);
 
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
         if let Some(size) = size {
             req = req.header(CONTENT_LENGTH, size)
         }
 
         if let Some(mime) = content_type {
             req = req.header(CONTENT_TYPE, mime)
         }
 
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn obs_get_head_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn obs_get_head_object(
+        &self,
+        path: &str,
+        if_match: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         // The header 'Origin' is optional for API calling, the doc has mistake, confirmed with customer service of huaweicloud.
         // https://support.huaweicloud.com/intl/en-us/api-obs/obs_04_0084.html
 
-        let req = Request::head(&url);
+        let mut req = Request::head(&url);
+
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
 
         let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 11% similar despite different names*

```diff
@@ -11,55 +11,53 @@
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
 
-use super::core::ObsCore;
+use super::backend::WebhdfsBackend;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct ObsWriter {
-    core: Arc<ObsCore>,
+pub struct WebhdfsWriter {
+    backend: WebhdfsBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl ObsWriter {
-    pub fn new(core: Arc<ObsCore>, op: OpWrite, path: String) -> Self {
-        ObsWriter { core, op, path }
+impl WebhdfsWriter {
+    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
+        WebhdfsWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for ObsWriter {
+impl oio::Write for WebhdfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.core.obs_put_object_request(
-            &self.path,
-            Some(bs.len()),
-            self.op.content_type(),
-            AsyncBody::Bytes(bs),
-        )?;
-
-        self.core.sign(&mut req).await?;
+        let req = self
+            .backend
+            .webhdfs_create_object_request(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
-        let resp = self.core.send(req).await?;
+        let resp = self.backend.client.send(req).await?;
 
         let status = resp.status();
-
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -307,14 +307,16 @@
             self.parse_endpoint(&self.presign_endpoint, bucket)?.0
         } else {
             endpoint.clone()
         };
         debug!("backend use presign_endpoint: {}", &presign_endpoint);
 
         let mut cfg = AliyunConfig::default();
+        // Load cfg from env first.
+        cfg = cfg.from_env();
 
         if let Some(v) = self.access_key_id.take() {
             cfg.access_key_id = Some(v);
         }
 
         if let Some(v) = self.access_key_secret.take() {
             cfg.access_key_secret = Some(v);
@@ -367,15 +369,15 @@
             .set_max_batch_operations(1000)
             .set_capabilities(Read | Write | Copy | List | Scan | Presign | Batch)
             .set_hints(ReadStreamable);
 
         am
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let resp = self
             .core
             .oss_put_object(path, None, None, None, None, AsyncBody::Empty)
             .await?;
         let status = resp.status();
 
         match status {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::time::Duration;
 
 use bytes::Bytes;
+use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::header::IF_NONE_MATCH;
 use http::header::RANGE;
-use http::header::{CACHE_CONTROL, IF_NONE_MATCH};
 use http::Request;
 use http::Response;
 use reqsign::AliyunCredential;
 use reqsign::AliyunLoader;
 use reqsign::AliyunOssSigner;
 use serde::Deserialize;
 use serde::Serialize;
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -917,15 +917,15 @@
             .set_max_batch_operations(1000)
             .set_capabilities(Read | Write | List | Scan | Presign | Batch | Copy)
             .set_hints(ReadStreamable);
 
         am
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let mut req =
             self.core
                 .s3_put_object_request(path, Some(0), None, None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.32.0/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 use std::fmt::Formatter;
 use std::fmt::Write;
 use std::time::Duration;
 
 use backon::ExponentialBuilder;
 use backon::Retryable;
 use bytes::Bytes;
+use http::header::HeaderName;
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
-use http::header::{HeaderName, IF_NONE_MATCH};
+use http::header::IF_NONE_MATCH;
 use http::HeaderValue;
 use http::Request;
 use http::Response;
 use once_cell::sync::Lazy;
 use reqsign::AwsCredential;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
@@ -338,30 +339,15 @@
     }
 
     pub async fn s3_head_object(
         &self,
         path: &str,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        let mut req = Request::head(&url);
-
-        // Set SSE headers.
-        req = self.insert_sse_headers(req, false);
-
-        if let Some(if_none_match) = if_none_match {
-            req = req.header(IF_NONE_MATCH, if_none_match);
-        }
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+        let mut req = self.s3_head_object_request(path, if_none_match)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     pub async fn s3_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
@@ -448,18 +434,21 @@
         continuation_token: &str,
         delimiter: &str,
         limit: Option<usize>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let mut url = format!(
-            "{}?list-type=2&delimiter={delimiter}&prefix={}",
+            "{}?list-type=2&prefix={}",
             self.endpoint,
             percent_encode_path(&p)
         );
+        if !delimiter.is_empty() {
+            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
+        }
         if let Some(limit) = limit {
             write!(url, "&max-keys={limit}").expect("write into string must succeed");
         }
         if !continuation_token.is_empty() {
             // AWS S3 could return continuation-token that contains `=`
             // which could lead `reqsign` parse query wrongly.
             // URL encode continuation-token before starting signing so that
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,16 @@
         };
 
         let resp = self
             .core
             .s3_abort_multipart_upload(&self.path, upload_id)
             .await?;
         match resp.status() {
-            StatusCode::OK => {
+            // s3 returns code 204 if abort succeeds.
+            StatusCode::NO_CONTENT => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
                     | AccessorCapability::List,
             )
             .set_hints(AccessorHint::ReadStreamable);
 
         ma
     }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         self.ensure_parent_path(path).await?;
 
         let abs_path = build_abs_path(&self.root, path);
         self.create_internal(&abs_path).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -440,15 +440,15 @@
                     return Err(Error::new(
                         ErrorKind::ConfigInvalid,
                         "root path must be dir",
                     ));
                 }
             }
             StatusCode::NOT_FOUND => {
-                self.create("/", OpCreate::new(EntryMode::DIR)).await?;
+                self.create_dir("/", OpCreate::new()).await?;
             }
             _ => return Err(parse_error(resp).await?),
         }
         Ok(())
     }
 }
 
@@ -469,15 +469,15 @@
                 AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
             )
             .set_hints(AccessorHint::ReadStreamable);
         am
     }
 
     /// Create a file or directory
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
+    async fn create_dir(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let req = self
             .webhdfs_create_object_request(path, Some(0), None, AsyncBody::Empty)
             .await?;
 
         let resp = self.client.send(req).await?;
 
         let status = resp.status();
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
 
-use super::message::{FileStatus, FileStatusType};
+use super::message::FileStatus;
+use super::message::FileStatusType;
 use crate::raw::*;
 use crate::*;
 
 pub struct WebhdfsPager {
     path: String,
     statuses: Vec<FileStatus>,
 }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files 20% similar despite different names*

```diff
@@ -11,69 +11,94 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::WebhdfsBackend;
+use super::core::*;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct WebhdfsWriter {
-    backend: WebhdfsBackend,
+pub struct WasabiWriter {
+    core: Arc<WasabiCore>,
 
     op: OpWrite,
     path: String,
+
+    upload_id: Option<String>,
 }
 
-impl WebhdfsWriter {
-    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
-        WebhdfsWriter { backend, op, path }
+impl WasabiWriter {
+    pub fn new(
+        core: Arc<WasabiCore>,
+        op: OpWrite,
+        path: String,
+        upload_id: Option<String>,
+    ) -> Self {
+        WasabiWriter {
+            core,
+
+            op,
+            path,
+            upload_id,
+        }
     }
 }
 
 #[async_trait]
-impl oio::Write for WebhdfsWriter {
+impl oio::Write for WasabiWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let req = self
-            .backend
-            .webhdfs_create_object_request(
+        debug_assert!(
+            self.upload_id.is_none(),
+            "Writer initiated with upload id, but users trying to call write, must be buggy"
+        );
+
+        let resp = self
+            .core
+            .put_object(
                 &self.path,
                 Some(bs.len()),
                 self.op.content_type(),
+                self.op.content_disposition(),
+                self.op.cache_control(),
                 AsyncBody::Bytes(bs),
             )
             .await?;
 
-        let resp = self.backend.client.send(req).await?;
-
-        let status = resp.status();
-        match status {
+        match resp.status() {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn append(&mut self, bs: Bytes) -> Result<()> {
-        let _ = bs;
+        let resp = self
+            .core
+            .append_object(&self.path, Some(bs.len()), AsyncBody::Bytes(bs))
+            .await?;
 
-        Err(Error::new(
-            ErrorKind::Unsupported,
-            "output writer doesn't support append",
-        ))
+        match resp.status() {
+            StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
+                resp.into_body().consume().await?;
+                Ok(())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
     }
 
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
     async fn close(&mut self) -> Result<()> {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/error.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/list.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files 0% similar despite different names*

```diff
@@ -299,16 +299,15 @@
                 "the path trying to create should end with `/`",
             )
             .with_operation("create_dir")
             .with_context("service", self.inner().info().scheme())
             .with_context("path", &path));
         }
 
-        self.inner()
-            .blocking_create(&path, OpCreate::new(EntryMode::DIR))?;
+        self.inner().blocking_create_dir(&path, OpCreate::new())?;
 
         Ok(())
     }
 
     /// Read the whole path into a bytes.
     ///
     /// This function will allocate a new bytes internally. For more precise memory control or
@@ -416,15 +415,15 @@
                     .with_context("service", self.info().scheme().into_static())
                     .with_context("path", &path),
             );
         }
 
         let op = OpRead::new().with_range(range.into());
 
-        BlockingReader::create(self.inner().clone(), &path, op)
+        BlockingReader::create_dir(self.inner().clone(), &path, op)
     }
 
     /// Write bytes into given path.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
@@ -634,15 +633,15 @@
                     .with_operation("BlockingOperator::writer")
                     .with_context("service", self.info().scheme().into_static())
                     .with_context("path", &path),
             );
         }
 
         let op = OpWrite::default().with_append();
-        BlockingWriter::create(self.inner().clone(), &path, op)
+        BlockingWriter::create_dir(self.inner().clone(), &path, op)
     }
 
     /// Delete given path.
     ///
     /// # Notes
     ///
     /// - Delete not existing error won't return errors.
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 0% similar despite different names*

```diff
@@ -386,17 +386,15 @@
                 "the path trying to create should end with `/`",
             )
             .with_operation("create_dir")
             .with_context("service", self.inner().info().scheme())
             .with_context("path", &path));
         }
 
-        self.inner()
-            .create(&path, OpCreate::new(EntryMode::DIR))
-            .await?;
+        self.inner().create_dir(&path, OpCreate::new()).await?;
 
         Ok(())
     }
 
     /// Read the whole path into a bytes.
     ///
     /// This function will allocate a new bytes internally. For more precise memory control or
@@ -480,15 +478,17 @@
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// # use opendal::ops::OpRead;
     /// # use futures::TryStreamExt;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// let bs = op.range_read_with("path/to/file", 1024..2048, OpRead::new()).await?;
+    /// let bs = op
+    ///     .range_read_with("path/to/file", 1024..2048, OpRead::new())
+    ///     .await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn range_read_with(
         &self,
         path: &str,
         range: impl RangeBounds<u64>,
@@ -602,15 +602,15 @@
                 Error::new(ErrorKind::IsADirectory, "read path is a directory")
                     .with_operation("Operator::range_reader")
                     .with_context("service", self.info().scheme())
                     .with_context("path", path),
             );
         }
 
-        Reader::create(self.inner().clone(), &path, args).await
+        Reader::create_dir(self.inner().clone(), &path, args).await
     }
 
     /// Write bytes into path.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
@@ -813,15 +813,15 @@
                 Error::new(ErrorKind::IsADirectory, "write path is a directory")
                     .with_operation("Operator::writer")
                     .with_context("service", self.inner().info().scheme().into_static())
                     .with_context("path", &path),
             );
         }
 
-        Writer::create(self.inner().clone(), &path, args.with_append()).await
+        Writer::create_dir(self.inner().clone(), &path, args.with_append()).await
     }
 
     /// Write data with extra options.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/ops.rs`

 * *Files 7% similar despite different names*

```diff
@@ -18,33 +18,25 @@
 //! Ops provides the operation args struct like [`OpRead`] for user.
 //!
 //! By using ops, users can add more context for operation.
 
 use std::time::Duration;
 
 use crate::raw::*;
-use crate::*;
 
 /// Args for `create` operation.
 ///
 /// The path must be normalized.
 #[derive(Debug, Clone, Default)]
-pub struct OpCreate {
-    mode: EntryMode,
-}
+pub struct OpCreate {}
 
 impl OpCreate {
     /// Create a new `OpCreate`.
-    pub fn new(mode: EntryMode) -> Self {
-        Self { mode }
-    }
-
-    /// Get mode from option.
-    pub fn mode(&self) -> EntryMode {
-        self.mode
+    pub fn new() -> Self {
+        Self::default()
     }
 }
 
 /// Args for `delete` operation.
 ///
 /// The path must be normalized.
 #[derive(Debug, Clone, Default)]
@@ -218,14 +210,15 @@
 
 /// Args for `read` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpRead {
     br: BytesRange,
     override_content_disposition: Option<String>,
     override_cache_control: Option<String>,
+    if_match: Option<String>,
     if_none_match: Option<String>,
 }
 
 impl OpRead {
     /// Create a default `OpRead` which will read whole content of path.
     pub fn new() -> Self {
         Self::default()
@@ -261,14 +254,25 @@
     }
 
     /// Returns the cache-control header that should be send back by the remote read operation.
     pub fn override_cache_control(&self) -> Option<&str> {
         self.override_cache_control.as_deref()
     }
 
+    /// Set the If-Match of the option
+    pub fn with_if_match(mut self, if_match: &str) -> Self {
+        self.if_match = Some(if_match.to_string());
+        self
+    }
+
+    /// Get If-Match from option
+    pub fn if_match(&self) -> Option<&str> {
+        self.if_match.as_deref()
+    }
+
     /// Set the If-None-Match of the option
     pub fn with_if_none_match(mut self, if_none_match: &str) -> Self {
         self.if_none_match = Some(if_none_match.to_string());
         self
     }
 
     /// Get If-None-Match from option
@@ -276,23 +280,35 @@
         self.if_none_match.as_deref()
     }
 }
 
 /// Args for `stat` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpStat {
+    if_match: Option<String>,
     if_none_match: Option<String>,
 }
 
 impl OpStat {
     /// Create a new `OpStat`.
     pub fn new() -> Self {
         Self::default()
     }
 
+    /// Set the If-Match of the option
+    pub fn with_if_match(mut self, if_match: &str) -> Self {
+        self.if_match = Some(if_match.to_string());
+        self
+    }
+
+    /// Get If-Match from option
+    pub fn if_match(&self) -> Option<&str> {
+        self.if_match.as_deref()
+    }
+
     /// Set the If-None-Match of the option
     pub fn with_if_none_match(mut self, if_none_match: &str) -> Self {
         self.if_none_match = Some(if_none_match.to_string());
         self
     }
 
     /// Get If-None-Match from option
@@ -305,14 +321,15 @@
 #[derive(Debug, Clone, Default)]
 pub struct OpWrite {
     append: bool,
 
     content_type: Option<String>,
     content_disposition: Option<String>,
     cache_control: Option<String>,
+    if_match: Option<String>,
 }
 
 impl OpWrite {
     /// Create a new `OpWrite`.
     ///
     /// If input path is not a file path, an error will be returned.
     pub fn new() -> Self {
@@ -356,14 +373,25 @@
     }
 
     /// Set the content type of option
     pub fn with_cache_control(mut self, cache_control: &str) -> Self {
         self.cache_control = Some(cache_control.to_string());
         self
     }
+
+    /// Set the If-Match of the option
+    pub fn with_if_match(mut self, if_match: &str) -> Self {
+        self.if_match = Some(if_match.to_string());
+        self
+    }
+
+    /// Get If-Match from option
+    pub fn if_match(&self) -> Option<&str> {
+        self.if_match.as_deref()
+    }
 }
 
 /// Args for `copy` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpCopy {}
 
 impl OpCopy {
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/reader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     /// Create a new reader.
     ///
     /// Create will use internal information to decide the most suitable
     /// implementation for users.
     ///
     /// We don't want to expose those details to users so keep this function
     /// in crate only.
-    pub(crate) async fn create(acc: FusedAccessor, path: &str, op: OpRead) -> Result<Self> {
+    pub(crate) async fn create_dir(acc: FusedAccessor, path: &str, op: OpRead) -> Result<Self> {
         let (_, r) = acc.read(path, op).await?;
 
         Ok(Reader {
             inner: r,
             seek_state: SeekState::Init,
         })
     }
@@ -188,15 +188,15 @@
     /// Create a new blocking reader.
     ///
     /// Create will use internal information to decide the most suitable
     /// implementation for users.
     ///
     /// We don't want to expose those details to users so keep this function
     /// in crate only.
-    pub(crate) fn create(acc: FusedAccessor, path: &str, op: OpRead) -> Result<Self> {
+    pub(crate) fn create_dir(acc: FusedAccessor, path: &str, op: OpRead) -> Result<Self> {
         let acc_meta = acc.info();
 
         let r = if acc_meta.hints().contains(AccessorHint::ReadSeekable) {
             let (_, r) = acc.blocking_read(path, op)?;
             r
         } else {
             return Err(Error::new(
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/scheme.rs`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     Redis,
     /// [rocksdb][crate::services::Rocksdb]: RocksDB services
     Rocksdb,
     /// [s3][crate::services::S3]: AWS S3 alike services.
     S3,
     /// [sled][crate::services::Sled]: Sled services
     Sled,
+    /// [wasabi][crate::services::Wasabi]: Wasabi service
+    Wasabi,
     /// [webdav][crate::services::Webdav]: WebDAV support.
     Webdav,
     /// [webhdfs][crate::services::Webhdfs]: WebHDFS RESTful API Services
     Webhdfs,
     /// Custom that allow users to implement services outside of OpenDAL.
     ///
     /// # NOTE
@@ -125,14 +127,15 @@
             "moka" => Ok(Scheme::Moka),
             "obs" => Ok(Scheme::Obs),
             "redis" => Ok(Scheme::Redis),
             "rocksdb" => Ok(Scheme::Rocksdb),
             "s3" => Ok(Scheme::S3),
             "sled" => Ok(Scheme::Sled),
             "oss" => Ok(Scheme::Oss),
+            "wasabi" => Ok(Scheme::Wasabi),
             "webdav" => Ok(Scheme::Webdav),
             "webhdfs" => Ok(Scheme::Webhdfs),
             _ => Ok(Scheme::Custom(Box::leak(s.into_boxed_str()))),
         }
     }
 }
 
@@ -155,14 +158,15 @@
             Scheme::Moka => "moka",
             Scheme::Obs => "obs",
             Scheme::Redis => "redis",
             Scheme::Rocksdb => "rocksdb",
             Scheme::S3 => "s3",
             Scheme::Sled => "sled",
             Scheme::Oss => "oss",
+            Scheme::Wasabi => "wasabi",
             Scheme::Webdav => "webdav",
             Scheme::Webhdfs => "webhdfs",
             Scheme::Custom(v) => v,
         }
     }
 }
```

### Comparing `opendal-0.31.1/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.32.0/local_dependencies/opendal/src/types/writer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 use bytes::Bytes;
 use futures::future::BoxFuture;
 use futures::ready;
 use futures::AsyncWrite;
 use futures::FutureExt;
 
 use crate::ops::OpWrite;
+use crate::raw::oio::Write;
 use crate::raw::*;
 use crate::*;
 
 /// Writer is designed to write data into given path in an asynchronous
 /// manner.
 ///
 /// # Notes
@@ -47,15 +48,15 @@
     /// Create a new writer.
     ///
     /// Create will use internal information to decide the most suitable
     /// implementation for users.
     ///
     /// We don't want to expose those details to users so keep this function
     /// in crate only.
-    pub(crate) async fn create(acc: FusedAccessor, path: &str, op: OpWrite) -> Result<Self> {
+    pub(crate) async fn create_dir(acc: FusedAccessor, path: &str, op: OpWrite) -> Result<Self> {
         let (_, w) = acc.write(path, op).await?;
 
         Ok(Writer {
             state: State::Idle(Some(w)),
         })
     }
 
@@ -71,14 +72,26 @@
             unreachable!(
                 "writer state invalid while append, expect Idle, actual {}",
                 self.state
             );
         }
     }
 
+    /// Abort inner writer.
+    pub async fn abort(&mut self) -> Result<()> {
+        if let State::Idle(Some(w)) = &mut self.state {
+            w.abort().await
+        } else {
+            unreachable!(
+                "writer state invalid while abort, expect Idle, actual {}",
+                self.state
+            );
+        }
+    }
+
     /// Close the writer and make sure all data have been stored.
     pub async fn close(&mut self) -> Result<()> {
         if let State::Idle(Some(w)) = &mut self.state {
             w.close().await
         } else {
             unreachable!(
                 "writer state invalid while close, expect Idle, actual {}",
@@ -181,15 +194,15 @@
     /// Create a new writer.
     ///
     /// Create will use internal information to decide the most suitable
     /// implementation for users.
     ///
     /// We don't want to expose those details to users so keep this function
     /// in crate only.
-    pub(crate) fn create(acc: FusedAccessor, path: &str, op: OpWrite) -> Result<Self> {
+    pub(crate) fn create_dir(acc: FusedAccessor, path: &str, op: OpWrite) -> Result<Self> {
         let (_, w) = acc.blocking_write(path, op)?;
 
         Ok(BlockingWriter { inner: w })
     }
 
     /// Append data into writer.
     ///
```

### Comparing `opendal-0.31.1/Cargo.toml` & `opendal-0.32.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.31.1"
+version= "0.32.0"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 chrono = { version = "0.4.24", default-features = false, features = ["std"] }
```

### Comparing `opendal-0.31.1/.gitignore` & `opendal-0.32.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/README.md` & `opendal-0.32.0/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/benchmark/README.md` & `opendal-0.32.0/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/benchmark/async_opendal_benchmark.py` & `opendal-0.32.0/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.32.0/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/pyproject.toml` & `opendal-0.32.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/python/opendal/__init__.py` & `opendal-0.32.0/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/python/opendal/__init__.pyi` & `opendal-0.32.0/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/src/asyncio.rs` & `opendal-0.32.0/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/src/layers.rs` & `opendal-0.32.0/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/src/lib.rs` & `opendal-0.32.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/tests/binding.feature` & `opendal-0.32.0/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/tests/steps/binding.py` & `opendal-0.32.0/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.31.1/Cargo.lock` & `opendal-0.32.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -185,18 +185,40 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
+name = "async-stream"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
+dependencies = [
+ "async-stream-impl",
+ "futures-core",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "async-stream-impl"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.12",
+]
+
+[[package]]
 name = "async-task"
-version = "4.3.0"
+version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a40729d2133846d9ed0ea60a8b9541bccddab49cd30f0715a1da672fe9a2524"
+checksum = "ecc7ab41815b3c653ccd2978ec3255c81349336702dfdf62ee6f7069b12a3aae"
 
 [[package]]
 name = "async-tls"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f23d769dbf1838d5df5156e7b1ad404f4c463d1ac2c6aeb6cd943630f8a8400"
 dependencies = [
@@ -281,14 +303,23 @@
  "futures-channel",
  "futures-util",
  "parking_lot 0.12.1",
  "tokio",
 ]
 
 [[package]]
+name = "bincode"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "bindgen"
 version = "0.60.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "062dddbc1ba4aca46de6338e2bf87771414c335f7b2f2036e8f3e9befebf88e6"
 dependencies = [
  "bitflags 1.3.2",
  "cexpr",
@@ -815,14 +846,49 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.12",
 ]
 
 [[package]]
+name = "darling"
+version = "0.14.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+dependencies = [
+ "darling_core",
+ "darling_macro",
+]
+
+[[package]]
+name = "darling_core"
+version = "0.14.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
+dependencies = [
+ "fnv",
+ "ident_case",
+ "proc-macro2",
+ "quote",
+ "strsim",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "darling_macro"
+version = "0.14.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+dependencies = [
+ "darling_core",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
  "hashbrown",
@@ -926,14 +992,20 @@
 [[package]]
 name = "dotenvy"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03d8c417d7a8cb362e0c37e5d815f5eb7c37f79ff93707329d5a194e42e54ca0"
 
 [[package]]
+name = "downcast-rs"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
+
+[[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "encoding_rs"
@@ -1484,14 +1556,20 @@
 checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
+name = "ident_case"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
+
+[[package]]
 name = "idna"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "418a0a6fab821475f634efe3ccc45c013f742efe03d853e8d3355d5cb850ecf8"
 dependencies = [
  "matches",
  "unicode-bidi",
@@ -1689,15 +1767,15 @@
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 dependencies = [
- "spin",
+ "spin 0.5.2",
 ]
 
 [[package]]
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
@@ -1805,14 +1883,56 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b823e83b2affd8f40a9ee8c29dbc56404c1e34cd2710921f2801e2cf29527afa"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "madsim"
+version = "0.2.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d3f6f28042419b0a63a7db6a8b4f74db021453d567f76cdbfd81494eeec0b22"
+dependencies = [
+ "ahash",
+ "async-channel",
+ "async-stream",
+ "async-task",
+ "bincode",
+ "bytes",
+ "downcast-rs",
+ "futures-util",
+ "lazy_static",
+ "libc",
+ "madsim-macros",
+ "naive-timer",
+ "rand 0.8.5",
+ "rand_xoshiro",
+ "rustversion",
+ "serde",
+ "spin 0.9.8",
+ "tokio",
+ "tokio-util",
+ "toml 0.7.3",
+ "tracing",
+ "tracing-subscriber",
+]
+
+[[package]]
+name = "madsim-macros"
+version = "0.2.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f3d248e97b1a48826a12c3828d921e8548e714394bf17274dd0a93910dc946e1"
+dependencies = [
+ "darling",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "magnus"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3fda351681130b40996b3e40592565b5e44ef1a677c45ea3768ed223b5918a5"
 dependencies = [
  "bytes",
  "magnus-macros",
@@ -1992,14 +2112,20 @@
  "tagptr",
  "thiserror",
  "triomphe",
  "uuid",
 ]
 
 [[package]]
+name = "naive-timer"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "034a0ad7deebf0c2abcf2435950a6666c3c15ea9d8fad0c0f48efa8a7f843fed"
+
+[[package]]
 name = "napi"
 version = "2.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "564ad12389dd08b0f5e95b9e8b5e88e5e42a234d326639cfa7b0fe643562e0d7"
 dependencies = [
  "bitflags 2.0.2",
  "ctor",
@@ -2183,27 +2309,27 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.31.1"
+version = "0.32.0"
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
-version = "0.31.1"
+version = "0.32.0"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.1.11",
  "dirs",
  "env_logger",
  "futures",
@@ -2226,15 +2352,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.31.1"
+version = "0.32.0"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
@@ -2249,14 +2375,15 @@
  "flagset",
  "futures",
  "hdrs",
  "http",
  "hyper",
  "lazy-regex",
  "log",
+ "madsim",
  "md-5",
  "metrics",
  "minitrace",
  "moka",
  "once_cell",
  "opentelemetry 0.19.0",
  "opentelemetry-jaeger",
@@ -2302,26 +2429,26 @@
 dependencies = [
  "jni",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.31.1"
+version = "0.32.0"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.31.1"
+version = "0.32.0"
 dependencies = [
  "chrono",
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
@@ -3073,14 +3200,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
 dependencies = [
  "rand_core 0.5.1",
 ]
 
 [[package]]
+name = "rand_xoshiro"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f97cdb2a36ed4183de61b2f824cc45c9f1037f28afe0a322e9fff4c108b5aaa"
+dependencies = [
+ "rand_core 0.6.4",
+]
+
+[[package]]
 name = "raw-cpuid"
 version = "10.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c297679cb867470fa8c9f67dbba74a78d78e3e98d7cf2b08d6d71540f797332"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -3304,15 +3440,15 @@
 version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
  "cc",
  "libc",
  "once_cell",
- "spin",
+ "spin 0.5.2",
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rocksdb"
@@ -3427,14 +3563,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
 dependencies = [
  "base64 0.21.0",
 ]
 
 [[package]]
+name = "rustversion"
+version = "1.0.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+
+[[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
@@ -3636,14 +3778,23 @@
 [[package]]
 name = "shlex"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
 
 [[package]]
+name = "signal-hook-registry"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "signature"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8fe458c98333f9c8152221191a77e2a44e8325d0193484af2e9421a53019e57d"
 dependencies = [
  "digest",
  "rand_core 0.6.4",
@@ -3748,14 +3899,23 @@
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
+name = "spin"
+version = "0.9.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
+dependencies = [
+ "lock_api",
+]
+
+[[package]]
 name = "spki"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67cf02bbac7a337dc36e4f5a693db6c21e7863f45070f7064577eb4367a3212b"
 dependencies = [
  "base64ct",
  "der",
@@ -3980,14 +4140,15 @@
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot 0.12.1",
  "pin-project-lite",
+ "signal-hook-registry",
  "socket2",
  "tokio-macros",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "tokio-macros"
```

### Comparing `opendal-0.31.1/PKG-INFO` & `opendal-0.32.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.31.1
+Version: 0.32.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: behave; extra == 'test'
+Requires-Dist: pdoc; extra == 'docs'
 Requires-Dist: gevent; extra == 'benchmark'
 Requires-Dist: greenify; extra == 'benchmark'
 Requires-Dist: greenlet; extra == 'benchmark'
 Requires-Dist: boto3; extra == 'benchmark'
 Requires-Dist: pydantic; extra == 'benchmark'
 Requires-Dist: boto3-stubs[essential]; extra == 'benchmark'
-Requires-Dist: pdoc; extra == 'docs'
-Provides-Extra: test
-Provides-Extra: benchmark
+Requires-Dist: behave; extra == 'test'
 Provides-Extra: docs
+Provides-Extra: benchmark
+Provides-Extra: test
 Summary: OpenDAL Python Binding
 Home-Page: https://opendal.apache.org/
 Author: OpenDAL Contributors <dev@opendal.apache.org>
 Author-email: OpenDAL Contributors <dev@opendal.apache.org>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Repository, https://github.com/apache/incubator-opendal
 Project-URL: Documentation, https://opendal.apache.org/docs/python/opendal.html
 Project-URL: Homepage, https://opendal.apache.org/
-Project-URL: Repository, https://github.com/apache/incubator-opendal
 
 # OpenDAL Python Binding
 
 Documentation: [main](https://opendal.apache.org/docs/python/)
 
 This crate intends to build a native python binding.
```

