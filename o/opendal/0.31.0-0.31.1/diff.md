# Comparing `tmp/opendal-0.31.0.tar.gz` & `tmp/opendal-0.31.1.tar.gz`

## Comparing `opendal-0.31.0.tar` & `opendal-0.31.1.tar`

### file list

```diff
@@ -1,240 +1,242 @@
--rw-r--r--   0        0        0     5090 1970-01-01 00:00:00.000000 opendal-0.31.0/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    60180 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1256 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6663 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2438 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1832 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1296 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7703 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     5243 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      926 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10794 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     4392 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    22397 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6746 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    17164 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9976 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    16050 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    13631 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    52162 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    32204 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123     1618 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    37153 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    11794 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3844 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3113 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    21079 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5164 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123     9055 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1181 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1548 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     1934 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     6441 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5404 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3394 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    10427 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2025 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11951 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     2020 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     4439 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15332 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4148 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4577 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     1971 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10680 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     8918 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6861 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5443 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     4049 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6387 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    27076 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123    10124 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123     9145 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     5738 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      913 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2183 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    15592 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     7931 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     3437 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2877 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     3625 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    25021 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3569 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    15973 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4206 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     2041 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    16136 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123     7533 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3380 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10014 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     2186 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123    20553 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2516 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    17767 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     3081 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    13256 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1743 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    16810 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     8862 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1975 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     1074 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
--rw-r--r--   0     1001      123     4713 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9954 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     3889 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     3350 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     7949 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    13309 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     6561 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3360 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      896 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2161 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    18570 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    20500 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     3275 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      896 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     4044 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10492 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5615 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    39368 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    27213 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     3602 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7040 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     4227 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123     5093 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123    20468 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      531 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2532 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2207 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    23279 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     5211 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     1812 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2213 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     2333 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     2494 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    10546 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     6197 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    15166 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1462 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    23847 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123     8731 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     3235 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    37805 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123     9437 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9603 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     5698 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123     7267 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.31.0/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-04-12 03:51:19.000000 opendal-0.31.0/.gitignore
--rw-r--r--   0     1001      123      917 2023-04-12 03:51:19.000000 opendal-0.31.0/README.md
--rw-r--r--   0     1001      123      765 2023-04-12 03:51:19.000000 opendal-0.31.0/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-04-12 03:51:19.000000 opendal-0.31.0/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-04-12 03:51:19.000000 opendal-0.31.0/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123     1638 2023-04-12 03:51:19.000000 opendal-0.31.0/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-04-12 03:51:19.000000 opendal-0.31.0/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-04-12 03:51:19.000000 opendal-0.31.0/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123    11963 2023-04-12 03:51:19.000000 opendal-0.31.0/src/asyncio.rs
--rw-r--r--   0     1001      123     3311 2023-04-12 03:51:19.000000 opendal-0.31.0/src/layers.rs
--rw-r--r--   0     1001      123    13929 2023-04-12 03:51:19.000000 opendal-0.31.0/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-04-12 03:51:19.000000 opendal-0.31.0/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-04-12 03:51:19.000000 opendal-0.31.0/tests/steps/binding.py
--rw-r--r--   0     1001      123   110910 2023-04-12 03:51:19.000000 opendal-0.31.0/Cargo.lock
--rw-r--r--   0        0        0     2051 1970-01-01 00:00:00.000000 opendal-0.31.0/PKG-INFO
+-rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 opendal-0.31.1/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    61889 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1256 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6635 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2438 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1832 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1296 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7703 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     5243 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      982 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10794 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     4392 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    22397 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6746 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    17164 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123    10062 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    16322 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    13631 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    53159 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    32402 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    12573 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     1885 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    25213 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    37934 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    11980 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3844 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3076 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    21079 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5164 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123     9283 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1181 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1548 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     6441 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5404 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3394 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    10427 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2025 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11951 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     2020 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     4439 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15332 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4148 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4577 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     1971 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10680 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     9260 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6861 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5968 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     4049 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    11671 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6387 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123    27076 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123    10124 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123     9184 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     5821 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      913 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2251 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    16478 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123     9557 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     3520 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2945 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     3973 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    25021 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123     1424 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      884 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3744 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    15973 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123     1808 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4206 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     2109 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    17788 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123     9004 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3463 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10014 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     2254 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123    20553 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2584 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    17767 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     1497 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     3256 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    15552 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1826 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    16810 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123     1871 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     8862 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     2043 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     1074 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
+-rw-r--r--   0     1001      123     4713 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9954 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4228 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      857 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     3350 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     7949 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    13309 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     6561 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3443 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2229 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    18807 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    21564 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3358 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     4256 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123    10492 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      855 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     5615 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    39368 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3395 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    27813 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     3685 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7040 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     4758 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123     5375 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      854 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123    20468 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      531 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2532 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2275 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19326 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     4085 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     4679 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     2434 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2285 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     2333 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     2494 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    10799 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     6197 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    15166 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1462 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    23925 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123     8731 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3235 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1098 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    40765 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123     9437 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/ops.rs
+-rw-r--r--   0     1001      123     9603 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     5698 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123     7267 2023-04-16 16:24:23.000000 opendal-0.31.1/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.31.1/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-04-16 16:24:23.000000 opendal-0.31.1/.gitignore
+-rw-r--r--   0     1001      123      982 2023-04-16 16:24:23.000000 opendal-0.31.1/README.md
+-rw-r--r--   0     1001      123      765 2023-04-16 16:24:23.000000 opendal-0.31.1/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-04-16 16:24:23.000000 opendal-0.31.1/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-04-16 16:24:23.000000 opendal-0.31.1/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123     1665 2023-04-16 16:24:23.000000 opendal-0.31.1/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-04-16 16:24:23.000000 opendal-0.31.1/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-04-16 16:24:23.000000 opendal-0.31.1/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123    11963 2023-04-16 16:24:23.000000 opendal-0.31.1/src/asyncio.rs
+-rw-r--r--   0     1001      123     3311 2023-04-16 16:24:23.000000 opendal-0.31.1/src/layers.rs
+-rw-r--r--   0     1001      123    13929 2023-04-16 16:24:23.000000 opendal-0.31.1/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-04-16 16:24:23.000000 opendal-0.31.1/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-04-16 16:24:23.000000 opendal-0.31.1/tests/steps/binding.py
+-rw-r--r--   0     1001      123   113336 2023-04-16 16:24:23.000000 opendal-0.31.1/Cargo.lock
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 opendal-0.31.1/PKG-INFO
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/Cargo.toml` & `opendal-0.31.1/local_dependencies/opendal/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.31.0"
+version= "0.31.1"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
@@ -43,15 +43,14 @@
   "services-ghac",
   "services-http",
   "services-ipmfs",
   "services-memory",
   "services-obs",
   "services-oss",
   "services-s3",
-  "services-sled",
   "services-webdav",
   "services-webhdfs",
 ]
 
 # Build docs or not.
 #
 # This features is used to control whether or not to build opendal's docs.
@@ -65,19 +64,29 @@
 rustls = ["reqwest/rustls-tls-native-roots"]
 # Enable native-tls for TLS support
 native-tls = ["reqwest/native-tls"]
 # Enable vendored native-tls for TLS support
 native-tls-vendored = ["reqwest/native-tls-vendored"]
 
 # Enable all layers.
-layers-all = ["layers-chaos", "layers-metrics", "layers-tracing"]
+layers-all = [
+  "layers-chaos",
+  "layers-metrics",
+  "layers-prometheus",
+  "layers-tracing",
+  "layers-minitrace",
+]
 # Enable layers chaos support
 layers-chaos = ["dep:rand"]
 # Enable layers metrics support
 layers-metrics = ["dep:metrics"]
+# Enable layers prometheus support
+layers-prometheus = ["dep:prometheus"]
+# Enable layers minitrace support.
+layers-minitrace = ["dep:minitrace"]
 # Enable layers tracing support.
 layers-tracing = ["dep:tracing"]
 
 services-azblob = [
   "dep:reqsign",
   "reqsign?/services-azblob",
   "reqsign?/reqwest_request",
@@ -147,19 +156,21 @@
 hdrs = { version = "0.2", optional = true, features = ["async_file"] }
 http = "0.2.5"
 hyper = "0.14"
 lazy-regex = { version = "2.5.0", optional = true }
 log = "0.4"
 md-5 = "0.10"
 metrics = { version = "0.20", optional = true }
+minitrace = { version = "0.4.0", optional = true }
 moka = { version = "0.10", optional = true, features = ["future"] }
 once_cell = "1"
 parking_lot = "0.12"
 percent-encoding = "2"
 pin-project = "1"
+prometheus = { version = "0.13", features = ["process"], optional = true}
 prost = { version = "0.11", optional = true }
 quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
 redis = { version = "0.22", features = [
   "tokio-comp",
   "connection-manager",
 ], optional = true }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.31.1/local_dependencies/opendal/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,61 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.31.1] - 2023-04-17
+
+### Added
+
+- feat(services/azdfs): support rename (#1929)
+- test: Increate copy/move nested path test depth (#1932)
+- feat(layers): add a basic minitrace layer (#1931)
+- feat: add Writer::abort method (#1937)
+- feat(services/gcs): Allow setting PredefinedAcl (#1989)
+- feat(services/oss): add oss cache-control header support (#1986)
+- feat: Add PreconditionFailed Error so users can handle them (#1993)
+- feat: add http if_none_match support (#1995)
+- feat: add oss if-none-match support (#1997)
+- feat(services/gcs): Allow setting default storage_class (#1996)
+- feat(binding/C): add clang-format for c binding (#2003)
+
+### Changed
+
+- refactor: Polish the behavior of scan (#1926)
+- refactor: Polish the implementation of webhdfs (#1935)
+
+### Fixed
+
+- fix: sled should not be enabled by default (#1923)
+- fix: kv adapter's writer implementation fixed to honour empty writes (#193
+4)
+- fix(services/azblob): fix copy missing content-length (#2000)
+
+### Docs
+
+- docs: Adding docs link to python binding (#1921)
+- docs(bindings/python): fix wrong doc link (#1928)
+- docs: Add contributing for OpenDAL (#1984)
+- docs: Add explanation in contributing (#1985)
+- docs: Feel relax in community and don't hurry (#1987)
+- docs: update contributing (#1998)
+- docs(services/memory): Fix wrong explanation (#2002)
+- docs: Add OpenDAL VISION (#2007)
+- docs: update VISION and behavior tests doc (#2009)
+
+### CI
+
+- ci(bindings/nodejs): Access should be set to public before publish (#1919)
+- ci: Re-enable webhdfs test (#1925)
+- chore: add .editorconfig (#1988)
+- ci: Fix format after adding editorconfig (#1990)
+
 ## [v0.31.0] - 2023-04-12
 
 ### Added
 
 - feat(bindings/java): add cucumber test (#1809)
 - feat(bindings/java): setup Java CI (#1823)
 - feat: add if_none_match support (#1832)
@@ -1836,14 +1883,15 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.31.1]: https://github.com/apache/incubator-opendal/compare/v0.31.0...v0.31.1
 [v0.31.0]: https://github.com/apache/incubator-opendal/compare/v0.30.5...v0.31.0
 [v0.30.5]: https://github.com/apache/incubator-opendal/compare/v0.30.4...v0.30.5
 [v0.30.4]: https://github.com/apache/incubator-opendal/compare/v0.30.3...v0.30.4
 [v0.30.3]: https://github.com/apache/incubator-opendal/compare/v0.30.2...v0.30.3
 [v0.30.2]: https://github.com/apache/incubator-opendal/compare/v0.30.1...v0.30.2
 [v0.30.1]: https://github.com/apache/incubator-opendal/compare/v0.30.0...v0.30.1
 [v0.30.0]: https://github.com/apache/incubator-opendal/compare/v0.29.1...v0.30.0
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.31.1/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/README.md` & `opendal-0.31.1/local_dependencies/opendal/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [actions]: https://github.com/apache/incubator-opendal/actions?query=branch%3Amain
 [latest version]: https://img.shields.io/crates/v/opendal.svg
 [crates.io]: https://crates.io/crates/opendal
 [crate downloads]: https://img.shields.io/crates/d/opendal.svg
 [chat]: https://img.shields.io/discord/1081052318650339399
 [discord]: https://discord.gg/XQy8yGR2dg
 
-**Open** **D**ata **A**ccess **L**ayer: Access data freely, painlessly, and efficiently
+**Open** **D**ata **A**ccess **L**ayer: access data freely.
 
 - Documentation: [stable](https://docs.rs/opendal/) | [main](https://opendal.apache.org/docs/rust/opendal/)
 - [Release notes](https://docs.rs/opendal/latest/opendal/docs/changelog/index.html)
 
 ![](https://user-images.githubusercontent.com/5351546/222356748-14276998-501b-4d2a-9b09-b8cff3018204.png)
 
 ## Services
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.31.1/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.31.1/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.31.1/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.31.1/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.31.1/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/examples/object.rs` & `opendal-0.31.1/local_dependencies/opendal/examples/object.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.31.1/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/features.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/features.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ## Layer Features
 
 - `layers-all`: Enable all layers support.
 - `layers-metrics`: Enable metrics layer support.
+- `layers-prometheus`: Enable prometheus layer support.
 - `layers-tracing`: Enable tracing layer support.
 - `layers-chaos`: Enable chaos layer support.
 
 ## Service Features
 
 - `services-dashmap`: Enable dashmap service support.
 - `services-ftp`: Enable ftp service support.
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.31.1/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.31.1/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/complete.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,18 @@
         self.inner.write(bs).await
     }
 
     async fn append(&mut self, bs: Bytes) -> Result<()> {
         self.inner.append(bs).await
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        self.inner.abort().await
+    }
+
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await
     }
 }
 
 impl<R: oio::BlockingWrite> oio::BlockingWrite for ConcurrentLimitWrapper<R> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,22 @@
         self.inner.append(bs).await.map_err(|err| {
             err.with_operation(WriteOperation::Append)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        self.inner.abort().await.map_err(|err| {
+            err.with_operation(WriteOperation::Append)
+                .with_context("service", self.scheme)
+                .with_context("path", &self.path)
+        })
+    }
+
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await.map_err(|err| {
             err.with_operation(WriteOperation::Close)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1415,14 +1415,44 @@
                     )
                 }
                 Err(err)
             }
         }
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        match self.inner.abort().await {
+            Ok(_) => {
+                trace!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} path={} written={} -> abort writer",
+                    self.scheme,
+                    WriteOperation::Abort,
+                    self.path,
+                    self.written,
+                );
+                Ok(())
+            }
+            Err(err) => {
+                if let Some(lvl) = self.failure_level {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} path={} written={} -> abort writer failed: {err:?}",
+                        self.scheme,
+                        WriteOperation::Abort,
+                        self.path,
+                        self.written,
+                    )
+                }
+                Err(err)
+            }
+        }
+    }
+
     async fn close(&mut self) -> Result<()> {
         match self.inner.close().await {
             Ok(_) => Ok(()),
             Err(err) => {
                 if let Some(lvl) = self.failure_level {
                     log!(
                         target: LOGGING_TARGET,
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files 0% similar despite different names*

```diff
@@ -933,14 +933,21 @@
             .map(|_| self.bytes += size as u64)
             .map_err(|err| {
                 self.handle.increment_errors_total(self.op, err.kind());
                 err
             })
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        self.inner.abort().await.map_err(|err| {
+            self.handle.increment_errors_total(self.op, err.kind());
+            err
+        })
+    }
+
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await.map_err(|err| {
             self.handle.increment_errors_total(self.op, err.kind());
             err
         })
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -32,22 +32,32 @@
 pub use chaos::ChaosLayer;
 
 #[cfg(feature = "layers-metrics")]
 mod metrics;
 #[cfg(feature = "layers-metrics")]
 pub use self::metrics::MetricsLayer;
 
+#[cfg(feature = "layers-prometheus")]
+mod prometheus;
+#[cfg(feature = "layers-prometheus")]
+pub use self::prometheus::PrometheusLayer;
+
 mod retry;
 pub use self::retry::RetryLayer;
 
 #[cfg(feature = "layers-tracing")]
 mod tracing;
 #[cfg(feature = "layers-tracing")]
 pub use self::tracing::TracingLayer;
 
+#[cfg(feature = "layers-minitrace")]
+mod minitrace;
+#[cfg(feature = "layers-minitrace")]
+pub use self::minitrace::MinitraceLayer;
+
 mod type_eraser;
 pub(crate) use type_eraser::TypeEraseLayer;
 
 mod error_context;
 pub(crate) use error_context::ErrorContextLayer;
 
 mod complete;
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/retry.rs`

 * *Files 1% similar despite different names*

```diff
@@ -668,14 +668,35 @@
                         continue;
                     }
                 },
             }
         }
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        let mut backoff = self.builder.build();
+
+        loop {
+            match self.inner.abort().await {
+                Ok(v) => return Ok(v),
+                Err(e) if !e.is_temporary() => return Err(e),
+                Err(e) => match backoff.next() {
+                    None => return Err(e),
+                    Some(dur) => {
+                        warn!(target: "opendal::service",
+                              "operation={} path={} -> pager retry after {}s: error={:?}",
+                              WriteOperation::Append, self.path, dur.as_secs_f64(), e);
+                        tokio::time::sleep(dur).await;
+                        continue;
+                    }
+                },
+            }
+        }
+    }
+
     async fn close(&mut self) -> Result<()> {
         let mut backoff = self.builder.build();
 
         loop {
             match self.inner.close().await {
                 Ok(v) => return Ok(v),
                 Err(e) if !e.is_temporary() => return Err(e),
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files 1% similar despite different names*

```diff
@@ -332,14 +332,22 @@
         self.inner.append(bs).await
     }
 
     #[tracing::instrument(
         parent = &self.span,
         level = "trace",
         skip_all)]
+    async fn abort(&mut self) -> Result<()> {
+        self.inner.abort().await
+    }
+
+    #[tracing::instrument(
+        parent = &self.span,
+        level = "trace",
+        skip_all)]
     async fn close(&mut self) -> Result<()> {
         self.inner.close().await
     }
 }
 
 impl<R: oio::BlockingWrite> oio::BlockingWrite for TracingWrapper<R> {
     #[tracing::instrument(
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.31.1/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/lib.rs` & `opendal-0.31.1/local_dependencies/opendal/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-//! OpenDAL is the Open Data Access Layer to **freely**, **painlessly**, and **efficiently** access data.
+//! OpenDAL is the Open Data Access Layer to **freely** access data.
 //!
 //! - Documentation: All docs are carried byself, visit [`docs`] for more.
 //! - Services: All supported services could be found at [`services`].
 //! - Layers: All builtin layer could be found at [`layers`].
 //! - Features: All features could be found at [`features`][docs::features].
 //!
 //! # Quick Start
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files 8% similar despite different names*

```diff
@@ -205,22 +205,16 @@
 pub struct KvPager {
     root: String,
     inner: Option<Vec<String>>,
 }
 
 impl KvPager {
     fn new(root: &str, inner: Vec<String>) -> Self {
-        let root = if root == "/" {
-            "".to_string()
-        } else {
-            root.to_string()
-        };
-
         Self {
-            root,
+            root: root.to_string(),
             inner: Some(inner),
         }
     }
 
     fn inner_next_page(&mut self) -> Option<Vec<oio::Entry>> {
         let res = self
             .inner
@@ -229,19 +223,15 @@
             .map(|v| {
                 let mode = if v.ends_with('/') {
                     EntryMode::DIR
                 } else {
                     EntryMode::FILE
                 };
 
-                oio::Entry::new(
-                    v.strip_prefix(&self.root)
-                        .expect("key must start with root"),
-                    Metadata::new(mode),
-                )
+                oio::Entry::new(&build_rel_path(&self.root, &v), Metadata::new(mode))
             })
             .collect();
 
         Some(res)
     }
 }
 
@@ -259,67 +249,84 @@
 }
 
 pub struct KvWriter<S> {
     kv: Arc<S>,
     path: String,
 
     /// TODO: if kv supports append, we can use them directly.
-    buf: Vec<u8>,
+    buf: Option<Vec<u8>>,
 }
 
 impl<S> KvWriter<S> {
     fn new(kv: Arc<S>, path: String) -> Self {
         KvWriter {
             kv,
             path,
-            buf: Vec::new(),
+            buf: None,
+        }
+    }
+
+    fn extend_buf(&mut self, bs: Bytes) {
+        if let Some(buf) = self.buf.as_mut() {
+            buf.extend(bs);
+        } else {
+            self.buf = Some(bs.into())
         }
     }
 }
 
 #[async_trait]
 impl<S: Adapter> oio::Write for KvWriter<S> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.buf = bs.into();
+        self.buf = Some(bs.into());
 
         Ok(())
     }
 
     async fn append(&mut self, bs: Bytes) -> Result<()> {
         if let Err(e) = self.kv.append(&self.path, bs.to_vec().as_slice()).await {
             if e.kind() == ErrorKind::Unsupported {
-                self.buf.extend(bs);
+                self.extend_buf(bs);
             } else {
                 return Err(e);
             }
         }
         Ok(())
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "output writer doesn't support abort",
+        ))
+    }
+
     async fn close(&mut self) -> Result<()> {
-        if !self.buf.is_empty() {
-            self.kv.set(&self.path, &self.buf).await?;
+        if let Some(buf) = self.buf.as_deref() {
+            self.kv.set(&self.path, buf).await?;
         }
 
         Ok(())
     }
 }
 
 impl<S: Adapter> oio::BlockingWrite for KvWriter<S> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.buf = bs.into();
+        self.buf = Some(bs.into());
 
         Ok(())
     }
 
     fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.buf.extend(bs);
+        self.extend_buf(bs);
 
         Ok(())
     }
 
     fn close(&mut self) -> Result<()> {
-        self.kv.blocking_set(&self.path, &self.buf)?;
+        if let Some(buf) = self.buf.as_deref() {
+            self.kv.blocking_set(&self.path, buf)?;
+        }
 
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             "service doesn't support list hierarchy, it must be a bug"
         );
     }
 
     ToFlatPager {
         acc,
         size,
+        root: path.to_string(),
         dirs: VecDeque::from([oio::Entry::new(path, Metadata::new(EntryMode::DIR))]),
         pagers: vec![],
         res: Vec::with_capacity(size),
     }
 }
 
 /// ToFlatPager will walk dir in bottom up way:
@@ -83,14 +84,15 @@
 ///
 /// Especially, for storage services that can't return dirs first, ToFlatPager
 /// may output parent dirs' files before nested dirs, this is expected because files
 /// always output directly while listing.
 pub struct ToFlatPager<A: Accessor, P> {
     acc: A,
     size: usize,
+    root: String,
     dirs: VecDeque<oio::Entry>,
     pagers: Vec<(P, oio::Entry, Vec<oio::Entry>)>,
     res: Vec<oio::Entry>,
 }
 
 #[async_trait]
 impl<A, P> oio::Page for ToFlatPager<A, P>
@@ -117,15 +119,18 @@
 
             if buf.is_empty() {
                 match pager.next().await? {
                     Some(v) => {
                         buf = v;
                     }
                     None => {
-                        self.res.push(de);
+                        // Only push entry if it's not root dir
+                        if de.path() != self.root {
+                            self.res.push(de);
+                        }
                         continue;
                     }
                 }
             }
 
             let mut buf = VecDeque::from(buf);
             loop {
@@ -174,15 +179,18 @@
 
             if buf.is_empty() {
                 match pager.next()? {
                     Some(v) => {
                         buf = v;
                     }
                     None => {
-                        self.res.push(de);
+                        // Only push entry if it's not root dir
+                        if de.path() != self.root {
+                            self.res.push(de);
+                        }
                         continue;
                     }
                 }
             }
 
             let mut buf = VecDeque::from(buf);
             loop {
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 #[derive(Debug, Copy, Clone, Hash, Eq, PartialEq)]
 #[non_exhaustive]
 pub enum WriteOperation {
     /// Operation for [`Write::write`]
     Write,
     /// Operation for [`Write::append`]
     Append,
+    /// Operation for [`Write::abort`]
+    Abort,
     /// Operation for [`Write::close`]
     Close,
     /// Operation for [`BlockingWrite::write`]
     BlockingWrite,
     /// Operation for [`BlockingWrite::append`]
     BlockingAppend,
     /// Operation for [`BlockingWrite::close`]
@@ -57,14 +59,15 @@
 impl From<WriteOperation> for &'static str {
     fn from(v: WriteOperation) -> &'static str {
         use WriteOperation::*;
 
         match v {
             Write => "Writer::write",
             Append => "Writer::append",
+            Abort => "Writer::abort",
             Close => "Writer::close",
             BlockingWrite => "BlockingWriter::write",
             BlockingAppend => "BlockingWriter::append",
             BlockingClose => "BlockingWriter::close",
         }
     }
 }
@@ -83,14 +86,19 @@
     /// Append bytes to the writer.
     ///
     /// It is highly recommended to align the length of the input bytes
     /// into blocks of 4MiB (except the last block) for better performance
     /// and compatibility.
     async fn append(&mut self, bs: Bytes) -> Result<()>;
 
+    /// Abort the pending appendable writer.
+    /// #note
+    /// This method is only applicable to writers opened in append mode.
+    async fn abort(&mut self) -> Result<()>;
+
     /// Close the writer and make sure all data has been flushed.
     async fn close(&mut self) -> Result<()>;
 }
 
 #[async_trait]
 impl Write for () {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
@@ -104,14 +112,21 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "output writer doesn't support abort",
+        ))
+    }
+
     async fn close(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support close",
         ))
     }
 }
@@ -124,14 +139,18 @@
         (**self).write(bs).await
     }
 
     async fn append(&mut self, bs: Bytes) -> Result<()> {
         (**self).append(bs).await
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        (**self).abort().await
+    }
+
     async fn close(&mut self) -> Result<()> {
         (**self).close().await
     }
 }
 
 /// BlockingWriter is a type erased [`BlockingWrite`]
 pub type BlockingWriter = Box<dyn BlockingWrite>;
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/operation.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/rps.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.31.1/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
             self.endpoint,
             self.container,
             percent_encode_path(&target)
         );
 
         let mut req = Request::put(&target)
             .header(X_MS_COPY_SOURCE, source)
+            .header(CONTENT_LENGTH, 0)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -70,11 +70,15 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Ok(())
+    }
+
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
+/// - [x] rename
 /// - [x] list
 /// - [ ] ~~scan~~
 /// - [ ] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
@@ -304,15 +305,18 @@
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azdfs)
             .set_root(&self.core.root)
             .set_name(&self.core.filesystem)
             .set_capabilities(
-                AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
+                AccessorCapability::Read
+                    | AccessorCapability::Write
+                    | AccessorCapability::Rename
+                    | AccessorCapability::List,
             )
             .set_hints(AccessorHint::ReadStreamable);
 
         am
     }
 
     async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
@@ -365,14 +369,38 @@
 
         Ok((
             RpWrite::default(),
             AzdfsWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
+    async fn rename(&self, from: &str, to: &str, _args: OpRename) -> Result<RpRename> {
+        if let Some(resp) = self.core.azdfs_ensure_parent_path(to).await? {
+            let status = resp.status();
+            match status {
+                StatusCode::CREATED | StatusCode::CONFLICT => {
+                    resp.into_body().consume().await?;
+                }
+                _ => return Err(parse_error(resp).await?),
+            }
+        }
+
+        let resp = self.core.azdfs_rename(from, to).await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::CREATED => {
+                resp.into_body().consume().await?;
+                Ok(RpRename::default())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
         let resp = self.core.azdfs_get_properties(path).await?;
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 use reqsign::AzureStorageCredential;
 use reqsign::AzureStorageLoader;
 use reqsign::AzureStorageSigner;
 
 use crate::raw::*;
 use crate::*;
 
+const X_MS_RENAME_SOURCE: &str = "x-ms-rename-source";
+
 pub struct AzdfsCore {
     pub filesystem: String,
     pub root: String,
     pub endpoint: String,
 
     pub client: HttpClient,
     pub loader: AzureStorageLoader,
@@ -157,14 +159,38 @@
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
+    pub async fn azdfs_rename(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
+        let source = build_abs_path(&self.root, from);
+        let target = build_abs_path(&self.root, to);
+
+        let url = format!(
+            "{}/{}/{}",
+            self.endpoint,
+            self.filesystem,
+            percent_encode_path(&target)
+        );
+
+        let mut req = Request::put(&url)
+            .header(
+                X_MS_RENAME_SOURCE,
+                format!("/{}/{}", self.filesystem, percent_encode_path(&source)),
+            )
+            .header(CONTENT_LENGTH, 0)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.sign(&mut req).await?;
+        self.send(req).await
+    }
+
     /// ref: https://learn.microsoft.com/en-us/rest/api/storageservices/datalakestoragegen2/path/update
     pub fn azdfs_update_request(
         &self,
         path: &str,
         size: Option<usize>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
@@ -263,8 +289,36 @@
         let mut req = Request::get(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
+
+    pub async fn azdfs_ensure_parent_path(
+        &self,
+        path: &str,
+    ) -> Result<Option<Response<IncomingAsyncBody>>> {
+        let abs_target_path = path.trim_end_matches('/').to_string();
+        let abs_target_path = abs_target_path.as_str();
+        let mut parts: Vec<&str> = abs_target_path
+            .split('/')
+            .filter(|x| !x.is_empty())
+            .collect();
+
+        if !parts.is_empty() {
+            parts.pop();
+        }
+
+        if !parts.is_empty() {
+            let parent_path = parts.join("/");
+            let mut req =
+                self.azdfs_create_request(&parent_path, "directory", None, None, AsyncBody::Empty)?;
+
+            self.sign(&mut req).await?;
+
+            Ok(Some(self.send(req).await?))
+        } else {
+            Ok(None)
+        }
+    }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -92,11 +92,15 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Ok(())
+    }
+
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files 11% similar despite different names*

```diff
@@ -34,28 +34,43 @@
 /// - [x] read
 /// - [x] write
 /// - [ ] ~~list~~
 /// - [x] scan
 /// - [ ] ~~presign~~
 /// - [x] blocking
 #[derive(Default)]
-pub struct DashmapBuilder {}
+pub struct DashmapBuilder {
+    root: Option<String>,
+}
+
+impl DashmapBuilder {
+    /// Set the root for dashmap.
+    pub fn root(&mut self, path: &str) -> &mut Self {
+        self.root = Some(path.into());
+        self
+    }
+}
 
 impl Builder for DashmapBuilder {
     const SCHEME: Scheme = Scheme::Dashmap;
     type Accessor = DashmapBackend;
 
-    fn from_map(_: HashMap<String, String>) -> Self {
-        Self::default()
+    fn from_map(map: HashMap<String, String>) -> Self {
+        let mut builder = Self::default();
+
+        map.get("root").map(|v| builder.root(v));
+
+        builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         Ok(DashmapBackend::new(Adapter {
             inner: DashMap::default(),
-        }))
+        })
+        .with_root(self.root.as_deref().unwrap_or_default()))
     }
 }
 
 /// Backend is used to serve `Accessor` support in dashmap.
 pub type DashmapBackend = kv::Backend<Adapter>;
 
 #[derive(Debug, Clone)]
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files 9% similar despite different names*

```diff
@@ -14,51 +14,46 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::io::Seek;
 use std::io::SeekFrom;
 use std::io::Write;
-use std::path::PathBuf;
 
 use async_trait::async_trait;
 use bytes::Bytes;
-use tokio::io::AsyncSeekExt;
-use tokio::io::AsyncWriteExt;
+use futures::AsyncSeekExt;
+use futures::AsyncWriteExt;
 
 use super::error::parse_io_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct FsWriter<F> {
-    target_path: PathBuf,
-    tmp_path: Option<PathBuf>,
+pub struct HdfsWriter<F> {
     f: F,
     pos: u64,
 }
 
-impl<F> FsWriter<F> {
-    pub fn new(target_path: PathBuf, tmp_path: Option<PathBuf>, f: F) -> Self {
-        Self {
-            target_path,
-            tmp_path,
-            f,
-            pos: 0,
-        }
+impl<F> HdfsWriter<F> {
+    pub fn new(f: F) -> Self {
+        Self { f, pos: 0 }
     }
 }
 
 #[async_trait]
-impl oio::Write for FsWriter<tokio::fs::File> {
+impl oio::Write for HdfsWriter<hdrs::AsyncFile> {
     /// # Notes
     ///
     /// File could be partial written, so we will seek to start to make sure
     /// we write the same content.
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.f.rewind().await.map_err(parse_io_error)?;
+        self.f
+            .seek(SeekFrom::Start(0))
+            .await
+            .map_err(parse_io_error)?;
         self.f.write_all(&bs).await.map_err(parse_io_error)?;
 
         Ok(())
     }
 
     /// # Notes
     ///
@@ -71,28 +66,29 @@
             .map_err(parse_io_error)?;
         self.f.write_all(&bs).await.map_err(parse_io_error)?;
         self.pos += bs.len() as u64;
 
         Ok(())
     }
 
-    async fn close(&mut self) -> Result<()> {
-        self.f.sync_all().await.map_err(parse_io_error)?;
+    async fn abort(&mut self) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "output writer doesn't support abort",
+        ))
+    }
 
-        if let Some(tmp_path) = &self.tmp_path {
-            tokio::fs::rename(tmp_path, &self.target_path)
-                .await
-                .map_err(parse_io_error)?;
-        }
+    async fn close(&mut self) -> Result<()> {
+        self.f.close().await.map_err(parse_io_error)?;
 
         Ok(())
     }
 }
 
-impl oio::BlockingWrite for FsWriter<std::fs::File> {
+impl oio::BlockingWrite for HdfsWriter<hdrs::File> {
     /// # Notes
     ///
     /// File could be partial written, so we will seek to start to make sure
     /// we write the same content.
     fn write(&mut self, bs: Bytes) -> Result<()> {
         self.f.rewind().map_err(parse_io_error)?;
         self.f.write_all(&bs).map_err(parse_io_error)?;
@@ -111,16 +107,12 @@
         self.f.write_all(&bs).map_err(parse_io_error)?;
         self.pos += bs.len() as u64;
 
         Ok(())
     }
 
     fn close(&mut self) -> Result<()> {
-        self.f.sync_all().map_err(parse_io_error)?;
-
-        if let Some(tmp_path) = &self.tmp_path {
-            std::fs::rename(tmp_path, &self.target_path).map_err(parse_io_error)?;
-        }
+        self.f.flush().map_err(parse_io_error)?;
 
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -58,11 +58,15 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Ok(())
+    }
+
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 ///
 /// # Configuration
 ///
 /// - `root`: Set the work directory for backend
 /// - `bucket`: Set the container name for backend
 /// - `endpoint`: Customizable endpoint setting
 /// - `credentials`: Credential string for GCS OAuth2
+/// - `predefined_acl`: Predefined ACL for GCS
+/// - `default_storage_class`: Default storage class for GCS
 ///
 /// You can refer to [`GcsBuilder`]'s docs for more information
 ///
 /// # Example
 ///
 /// ## Via Builder
 ///
@@ -81,14 +83,18 @@
 ///     // set the storage bucket for OpenDAL
 ///     builder.bucket("test");
 ///     // set the working directory root for GCS
 ///     // all operations will happen within it
 ///     builder.root("/path/to/dir");
 ///     // set the credentials for GCS OAUTH2 authentication
 ///     builder.credential("authentication token");
+///     // set the predefined ACL for GCS
+///     builder.predefined_acl("publicRead");
+///     // set the default storage class for GCS
+///     builder.default_storage_class("STANDARD");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
 ///     Ok(())
 /// }
 /// ```
 #[derive(Default)]
 pub struct GcsBuilder {
@@ -107,14 +113,16 @@
     /// credential string for GCS service
     credential: Option<String>,
     /// credential path for GCS service.
     credential_path: Option<String>,
 
     http_client: Option<HttpClient>,
     customed_token_loader: Option<Box<dyn GoogleTokenLoad>>,
+    predefined_acl: Option<String>,
+    default_storage_class: Option<String>,
 }
 
 impl GcsBuilder {
     /// set the working directory root of backend
     pub fn root(&mut self, root: &str) -> &mut Self {
         if !root.is_empty() {
             self.root = Some(root.to_string())
@@ -194,26 +202,60 @@
     }
 
     /// Specify the customed token loader used by this service.
     pub fn customed_token_loader(&mut self, token_load: Box<dyn GoogleTokenLoad>) -> &mut Self {
         self.customed_token_loader = Some(token_load);
         self
     }
+
+    /// Set the predefined acl for GCS.
+    ///
+    /// Available values are:
+    /// - `authenticatedRead`
+    /// - `bucketOwnerFullControl`
+    /// - `bucketOwnerRead`
+    /// - `private`
+    /// - `projectPrivate`
+    /// - `publicRead`
+    pub fn predefined_acl(&mut self, acl: &str) -> &mut Self {
+        if !acl.is_empty() {
+            self.predefined_acl = Some(acl.to_string())
+        };
+        self
+    }
+
+    /// Set the default storage class for GCS.
+    ///
+    /// Available values are:
+    /// - `STANDARD`
+    /// - `NEARLINE`
+    /// - `COLDLINE`
+    /// - `ARCHIVE`
+    pub fn default_storage_class(&mut self, class: &str) -> &mut Self {
+        if !class.is_empty() {
+            self.default_storage_class = Some(class.to_string())
+        };
+        self
+    }
 }
 
 impl Debug for GcsBuilder {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let mut ds = f.debug_struct("Builder");
 
         ds.field("root", &self.root)
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint);
         if self.credential.is_some() {
             ds.field("credentials", &"<redacted>");
         }
+        if self.predefined_acl.is_some() {
+            ds.field("predefined_acl", &self.predefined_acl);
+        }
+        ds.field("default_storage_class", &self.default_storage_class);
         ds.finish()
     }
 }
 
 impl Builder for GcsBuilder {
     const SCHEME: Scheme = Scheme::Gcs;
     type Accessor = GcsBackend;
@@ -222,14 +264,17 @@
         let mut builder = GcsBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
         map.get("bucket").map(|v| builder.bucket(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
         map.get("credential").map(|v| builder.credential(v));
         map.get("scope").map(|v| builder.scope(v));
+        map.get("predefined_acl").map(|v| builder.predefined_acl(v));
+        map.get("default_storage_class")
+            .map(|v| builder.default_storage_class(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         debug!("backend build started: {:?}", self);
 
@@ -295,14 +340,16 @@
                 endpoint,
                 bucket: bucket.to_string(),
                 root,
                 client,
                 signer,
                 token_loader,
                 credential_loader: cred_loader,
+                predefined_acl: self.predefined_acl.clone(),
+                default_storage_class: self.default_storage_class.clone(),
             }),
         };
 
         Ok(backend)
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
 use std::fmt::Write;
 
 use backon::ExponentialBuilder;
 use backon::Retryable;
+use bytes::BytesMut;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::Request;
 use http::Response;
 use once_cell::sync::Lazy;
 use reqsign::GoogleCredentialLoader;
 use reqsign::GoogleSigner;
@@ -40,14 +41,17 @@
     pub bucket: String,
     pub root: String,
 
     pub client: HttpClient,
     pub signer: GoogleSigner,
     pub token_loader: GoogleTokenLoader,
     pub credential_loader: GoogleCredentialLoader,
+
+    pub predefined_acl: Option<String>,
+    pub default_storage_class: Option<String>,
 }
 
 impl Debug for GcsCore {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let mut de = f.debug_struct("Backend");
         de.field("endpoint", &self.endpoint)
             .field("bucket", &self.bucket)
@@ -132,35 +136,68 @@
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
-        let url = format!(
-            "{}/upload/storage/v1/b/{}/o?uploadType=media&name={}",
+        let mut url = format!(
+            "{}/upload/storage/v1/b/{}/o?uploadType={}&name={}",
             self.endpoint,
             self.bucket,
+            if self.default_storage_class.is_some() {
+                "multipart"
+            } else {
+                "media"
+            },
             percent_encode_path(&p)
         );
 
+        if let Some(acl) = &self.predefined_acl {
+            write!(&mut url, "&predefinedAcl={}", acl).unwrap();
+        }
+
         let mut req = Request::post(&url);
 
         if let Some(size) = size {
             req = req.header(CONTENT_LENGTH, size)
         }
 
-        if let Some(mime) = content_type {
-            req = req.header(CONTENT_TYPE, mime)
-        }
+        if let Some(storage_class) = &self.default_storage_class {
+            req = req.header(CONTENT_TYPE, "multipart/related; boundary=my-boundary");
 
-        // Set body
-        let req = req.body(body).map_err(new_request_build_error)?;
+            let mut req_body = BytesMut::with_capacity(100);
+            write!(
+                &mut req_body,
+                "--my-boundary\nContent-Type: application/json; charset=UTF-8\n\n{{\"storageClass\": \"{}\"}}\n\n--my-boundary\n",
+                storage_class
+            ).unwrap();
+
+            if let Some(mime) = content_type {
+                write!(&mut req_body, "Content-Type: {}\n\n", mime).unwrap();
+            } else {
+                write!(&mut req_body, "Content-Type: application/octet-stream\n\n").unwrap();
+            }
+
+            if let AsyncBody::Bytes(bytes) = body {
+                req_body.extend_from_slice(&bytes);
+            }
+            write!(&mut req_body, "\n--my-boundary").unwrap();
+
+            let req_body = AsyncBody::Bytes(req_body.freeze());
+            let req = req.body(req_body).map_err(new_request_build_error)?;
+            Ok(req)
+        } else {
+            if let Some(content_type) = content_type {
+                req = req.header(CONTENT_TYPE, content_type);
+            }
 
-        Ok(req)
+            let req = req.body(body).map_err(new_request_build_error)?;
+            Ok(req)
+        }
     }
 
     pub async fn gcs_get_object_metadata(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!(
             "{}/storage/v1/b/{}/o/{}",
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -70,11 +70,15 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Ok(())
+    }
+
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,18 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Ok(())
+    }
+
     async fn close(&mut self) -> Result<()> {
         let req = self.backend.ghac_commit(self.cache_id, self.size).await?;
         let resp = self.backend.client.send(req).await?;
 
         if resp.status().is_success() {
             resp.into_body().consume().await?;
             Ok(())
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files 25% similar despite different names*

```diff
@@ -11,101 +11,64 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::io::Seek;
-use std::io::SeekFrom;
-use std::io::Write;
-
 use async_trait::async_trait;
 use bytes::Bytes;
-use futures::AsyncSeekExt;
-use futures::AsyncWriteExt;
+use http::StatusCode;
 
-use super::error::parse_io_error;
+use super::backend::IpmfsBackend;
+use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
-pub struct HdfsWriter<F> {
-    f: F,
-    pos: u64,
+pub struct IpmfsWriter {
+    backend: IpmfsBackend,
+
+    path: String,
 }
 
-impl<F> HdfsWriter<F> {
-    pub fn new(f: F) -> Self {
-        Self { f, pos: 0 }
+impl IpmfsWriter {
+    pub fn new(backend: IpmfsBackend, path: String) -> Self {
+        IpmfsWriter { backend, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for HdfsWriter<hdrs::AsyncFile> {
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
+impl oio::Write for IpmfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.f
-            .seek(SeekFrom::Start(0))
-            .await
-            .map_err(parse_io_error)?;
-        self.f.write_all(&bs).await.map_err(parse_io_error)?;
-
-        Ok(())
+        let resp = self
+            .backend
+            .ipmfs_write(&self.path, AsyncBody::Multipart("data".to_string(), bs))
+            .await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::CREATED | StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
     }
 
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
     async fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.f
-            .seek(SeekFrom::Start(self.pos))
-            .await
-            .map_err(parse_io_error)?;
-        self.f.write_all(&bs).await.map_err(parse_io_error)?;
-        self.pos += bs.len() as u64;
-
-        Ok(())
-    }
-
-    async fn close(&mut self) -> Result<()> {
-        self.f.close().await.map_err(parse_io_error)?;
+        let _ = bs;
 
-        Ok(())
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "output writer doesn't support append",
+        ))
     }
-}
-
-impl oio::BlockingWrite for HdfsWriter<hdrs::File> {
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
-    fn write(&mut self, bs: Bytes) -> Result<()> {
-        self.f.rewind().map_err(parse_io_error)?;
-        self.f.write_all(&bs).map_err(parse_io_error)?;
 
+    async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
 
-    /// # Notes
-    ///
-    /// File could be partial written, so we will seek to start to make sure
-    /// we write the same content.
-    fn append(&mut self, bs: Bytes) -> Result<()> {
-        self.f
-            .seek(SeekFrom::Start(self.pos))
-            .map_err(parse_io_error)?;
-        self.f.write_all(&bs).map_err(parse_io_error)?;
-        self.pos += bs.len() as u64;
-
-        Ok(())
-    }
-
-    fn close(&mut self) -> Result<()> {
-        self.f.flush().map_err(parse_io_error)?;
-
+    async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 
 use async_trait::async_trait;
 use http::header;
+use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
 use http::StatusCode;
 use log::debug;
 
 use super::error::parse_error;
 use crate::ops::*;
@@ -259,34 +260,36 @@
             .set_capabilities(AccessorCapability::Read)
             .set_hints(AccessorHint::ReadStreamable);
 
         ma
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.http_get(path, args.range()).await?;
+        let resp = self
+            .http_get(path, args.range(), args.if_none_match())
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
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
 
-        let resp = self.http_head(path).await?;
+        let resp = self.http_head(path, args.if_none_match()).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             // HTTP Server like nginx could return FORBIDDEN if auto-index
             // is not enabled, we should ignore them.
@@ -295,21 +298,30 @@
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 }
 
 impl HttpBackend {
-    async fn http_get(&self, path: &str, range: BytesRange) -> Result<Response<IncomingAsyncBody>> {
+    async fn http_get(
+        &self,
+        path: &str,
+        range: BytesRange,
+        if_none_match: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::get(&url);
 
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
         if let Some(auth) = &self.authorization {
             req = req.header(header::AUTHORIZATION, auth.clone())
         }
 
         if !range.is_full() {
             req = req.header(header::RANGE, range.to_header());
         }
@@ -317,21 +329,29 @@
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
 
-    async fn http_head(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    async fn http_head(
+        &self,
+        path: &str,
+        if_none_match: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
 
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
         if let Some(auth) = &self.authorization {
             req = req.header(header::AUTHORIZATION, auth.clone())
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
@@ -341,14 +361,15 @@
 }
 
 #[cfg(test)]
 mod tests {
     use anyhow::Result;
     use wiremock::matchers::basic_auth;
     use wiremock::matchers::bearer_token;
+    use wiremock::matchers::headers;
     use wiremock::matchers::method;
     use wiremock::matchers::path;
     use wiremock::Mock;
     use wiremock::MockServer;
     use wiremock::ResponseTemplate;
 
     use super::*;
@@ -457,8 +478,62 @@
         let op = Operator::new(builder)?.finish();
         let bs = op.stat("hello").await?;
 
         assert_eq!(bs.mode(), EntryMode::FILE);
         assert_eq!(bs.content_length(), 128);
         Ok(())
     }
+
+    #[tokio::test]
+    async fn test_read_with() -> Result<()> {
+        let _ = env_logger::builder().is_test(true).try_init();
+
+        let mock_server = MockServer::start().await;
+        Mock::given(method("GET"))
+            .and(path("/hello"))
+            .and(headers("if-none-match", vec!["*"]))
+            .respond_with(
+                ResponseTemplate::new(200)
+                    .insert_header("content-length", "13")
+                    .set_body_string("Hello, World!"),
+            )
+            .mount(&mock_server)
+            .await;
+
+        let mut builder = HttpBuilder::default();
+        builder.endpoint(&mock_server.uri());
+        builder.root("/");
+        let op = Operator::new(builder)?.finish();
+
+        let match_bs = op
+            .read_with("hello", OpRead::new().with_if_none_match("*"))
+            .await?;
+        assert_eq!(match_bs, b"Hello, World!");
+
+        Ok(())
+    }
+
+    #[tokio::test]
+    async fn test_stat_with() -> Result<()> {
+        let _ = env_logger::builder().is_test(true).try_init();
+
+        let mock_server = MockServer::start().await;
+        Mock::given(method("HEAD"))
+            .and(path("/hello"))
+            .and(headers("if-none-match", vec!["*"]))
+            .respond_with(ResponseTemplate::new(200).insert_header("content-length", "128"))
+            .mount(&mock_server)
+            .await;
+
+        let mut builder = HttpBuilder::default();
+        builder.endpoint(&mock_server.uri());
+        builder.root("/");
+        let op = Operator::new(builder)?.finish();
+        let bs = op
+            .stat_with("hello", OpStat::new().with_if_none_match("*"))
+            .await?;
+
+        assert_eq!(bs.mode(), EntryMode::FILE);
+        assert_eq!(bs.content_length(), 128);
+        Ok(())
+    }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 16% similar despite different names*

```diff
@@ -15,41 +15,49 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::IpmfsBackend;
+use super::backend::WebhdfsBackend;
 use super::error::parse_error;
+use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct IpmfsWriter {
-    backend: IpmfsBackend,
+pub struct WebhdfsWriter {
+    backend: WebhdfsBackend,
 
+    op: OpWrite,
     path: String,
 }
 
-impl IpmfsWriter {
-    pub fn new(backend: IpmfsBackend, path: String) -> Self {
-        IpmfsWriter { backend, path }
+impl WebhdfsWriter {
+    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
+        WebhdfsWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for IpmfsWriter {
+impl oio::Write for WebhdfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let resp = self
+        let req = self
             .backend
-            .ipmfs_write(&self.path, AsyncBody::Multipart("data".to_string(), bs))
+            .webhdfs_create_object_request(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                AsyncBody::Bytes(bs),
+            )
             .await?;
 
-        let status = resp.status();
+        let resp = self.backend.client.send(req).await?;
 
+        let status = resp.status();
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
@@ -60,11 +68,15 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Ok(())
+    }
+
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt` & `opendal-0.31.1/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files 7% similar despite different names*

```diff
@@ -22,43 +22,57 @@
 use async_trait::async_trait;
 use parking_lot::Mutex;
 
 use crate::raw::adapters::kv;
 use crate::raw::*;
 use crate::*;
 
-/// In memory service support. (HashMap Based)
+/// In memory service support. (BTreeMap Based)
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
 /// - [ ] ~~list~~
 /// - [x] scan
 /// - [ ] ~~presign~~
 /// - [x] blocking
 #[derive(Default)]
-pub struct MemoryBuilder {}
+pub struct MemoryBuilder {
+    root: Option<String>,
+}
+
+impl MemoryBuilder {
+    /// Set the root for dashmap.
+    pub fn root(&mut self, path: &str) -> &mut Self {
+        self.root = Some(path.into());
+        self
+    }
+}
 
 impl Builder for MemoryBuilder {
     const SCHEME: Scheme = Scheme::Memory;
     type Accessor = MemoryBackend;
 
-    fn from_map(_: HashMap<String, String>) -> Self {
-        Self::default()
+    fn from_map(map: HashMap<String, String>) -> Self {
+        let mut builder = Self::default();
+
+        map.get("root").map(|v| builder.root(v));
+
+        builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         let adapter = Adapter {
             inner: Arc::new(Mutex::new(BTreeMap::default())),
         };
 
-        Ok(MemoryBackend::new(adapter))
+        Ok(MemoryBackend::new(adapter).with_root(self.root.as_deref().unwrap_or_default()))
     }
 }
 
 /// Backend is used to serve `Accessor` support in memory.
 pub type MemoryBackend = kv::Backend<Adapter>;
 
 #[derive(Debug, Clone)]
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         // OBS could return `520 Origin Error` errors which should be retried.
         v if v.as_u16() == 520 => (ErrorKind::Unexpected, true),
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -70,11 +70,15 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Ok(())
+    }
+
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -370,44 +370,47 @@
 
         am
     }
 
     async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let resp = self
             .core
-            .oss_put_object(path, None, None, None, AsyncBody::Empty)
+            .oss_put_object(path, None, None, None, None, AsyncBody::Empty)
             .await?;
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(RpCreate::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.core.oss_get_object(path, args.range()).await?;
+        let resp = self
+            .core
+            .oss_get_object(path, args.range(), args.if_none_match())
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         let upload_id = if args.append() {
-            let resp = self.core.oss_initiate_upload(path).await?;
+            let resp = self.core.oss_initiate_upload(path, &args).await?;
             match resp.status() {
                 StatusCode::OK => {
                     let bs = resp.into_body().bytes().await?;
                     let result: InitiateMultipartUploadResult =
                         quick_xml::de::from_reader(bs.reader())
                             .map_err(new_xml_deserialize_error)?;
                     Some(result.upload_id)
@@ -433,21 +436,24 @@
                 resp.into_body().consume().await?;
                 Ok(RpCopy::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
+    async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         if path == "/" {
             let m = Metadata::new(EntryMode::DIR);
             return Ok(RpStat::new(m));
         }
 
-        let resp = self.core.oss_head_object(path).await?;
+        let resp = self
+            .core
+            .oss_head_object(path, args.if_none_match())
+            .await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 let m = Metadata::new(EntryMode::DIR);
@@ -483,21 +489,25 @@
             OssPager::new(self.core.clone(), path, "", args.limit()),
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
-            PresignOperation::Stat(_) => self.core.oss_head_object_request(path, true)?,
-            PresignOperation::Read(v) => self.core.oss_get_object_request(path, v.range(), true)?,
+            PresignOperation::Stat(_) => self.core.oss_head_object_request(path, true, None)?,
+            PresignOperation::Read(v) => {
+                self.core
+                    .oss_get_object_request(path, v.range(), true, None)?
+            }
             PresignOperation::Write(v) => self.core.oss_put_object_request(
                 path,
                 None,
                 v.content_type(),
                 v.content_disposition(),
+                v.cache_control(),
                 AsyncBody::Empty,
                 true,
             )?,
         };
 
         self.core.sign_query(&mut req, args.expire()).await?;
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 use std::time::Duration;
 
 use bytes::Bytes;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::RANGE;
+use http::header::{CACHE_CONTROL, IF_NONE_MATCH};
 use http::Request;
 use http::Response;
 use reqsign::AliyunCredential;
 use reqsign::AliyunLoader;
 use reqsign::AliyunOssSigner;
 use serde::Deserialize;
 use serde::Serialize;
 
+use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct OssCore {
     pub root: String,
     pub bucket: String,
     /// buffered host string
@@ -101,20 +103,22 @@
     #[inline]
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
 }
 
 impl OssCore {
+    #[allow(clippy::too_many_arguments)]
     pub fn oss_put_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
+        cache_control: Option<&str>,
         body: AsyncBody,
         is_presign: bool,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
         let url = format!("{}/{}", endpoint, percent_encode_path(&p));
 
@@ -126,23 +130,28 @@
             req = req.header(CONTENT_TYPE, mime);
         }
 
         if let Some(pos) = content_disposition {
             req = req.header(CONTENT_DISPOSITION, pos);
         }
 
+        if let Some(cache_control) = cache_control {
+            req = req.header(CACHE_CONTROL, cache_control)
+        }
+
         let req = req.body(body).map_err(new_request_build_error)?;
         Ok(req)
     }
 
     pub fn oss_get_object_request(
         &self,
         path: &str,
         range: BytesRange,
         is_presign: bool,
+        if_none_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
         let url = format!("{}/{}", endpoint, percent_encode_path(&p));
 
         let mut req = Request::get(&url);
         req = req.header(CONTENT_TYPE, "application/octet-stream");
@@ -150,14 +159,18 @@
         if !range.is_full() {
             req = req.header(RANGE, range.to_header());
             // Adding `x-oss-range-behavior` header to use standard behavior.
             // ref: https://help.aliyun.com/document_detail/39571.html
             req = req.header("x-oss-range-behavior", "standard");
         }
 
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
+
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
@@ -174,20 +187,24 @@
         Ok(req)
     }
 
     pub fn oss_head_object_request(
         &self,
         path: &str,
         is_presign: bool,
+        if_none_match: Option<&str>,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
         let url = format!("{}/{}", endpoint, percent_encode_path(&p));
 
-        let req = Request::head(&url);
+        let mut req = Request::head(&url);
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
+        }
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
@@ -217,41 +234,48 @@
         Ok(req)
     }
 
     pub async fn oss_get_object(
         &self,
         path: &str,
         range: BytesRange,
+        if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_get_object_request(path, range, false)?;
+        let mut req = self.oss_get_object_request(path, range, false, if_none_match)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
-    pub async fn oss_head_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_head_object_request(path, false)?;
+    pub async fn oss_head_object(
+        &self,
+        path: &str,
+        if_none_match: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.oss_head_object_request(path, false, if_none_match)?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
 
     pub async fn oss_put_object(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
+        cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Response<IncomingAsyncBody>> {
         let mut req = self.oss_put_object_request(
             path,
             size,
             content_type,
             content_disposition,
+            cache_control,
             body,
             false,
         )?;
 
         self.sign(&mut req).await?;
         self.send(req).await
     }
@@ -337,40 +361,49 @@
         if is_presign {
             &self.presign_endpoint
         } else {
             &self.endpoint
         }
     }
 
-    pub async fn oss_initiate_upload(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn oss_initiate_upload(
+        &self,
+        path: &str,
+        args: &OpWrite,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let cache_control = args.cache_control();
         let req = self
-            .oss_initiate_upload_request(path, None, None, AsyncBody::Empty, false)
+            .oss_initiate_upload_request(path, None, None, cache_control, AsyncBody::Empty, false)
             .await?;
         self.send(req).await
     }
 
     /// Creates a request that initiates multipart upload
     async fn oss_initiate_upload_request(
         &self,
         path: &str,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
+        cache_control: Option<&str>,
         body: AsyncBody,
         is_presign: bool,
     ) -> Result<Request<AsyncBody>> {
         let path = build_abs_path(&self.root, path);
         let endpoint = self.get_endpoint(is_presign);
         let url = format!("{}/{}?uploads", endpoint, percent_encode_path(&path));
         let mut req = Request::post(&url);
         if let Some(mime) = content_type {
             req = req.header(CONTENT_TYPE, mime);
         }
         if let Some(disposition) = content_disposition {
             req = req.header(CONTENT_DISPOSITION, disposition);
         }
+        if let Some(cache_control) = cache_control {
+            req = req.header(CACHE_CONTROL, cache_control);
+        }
 
         let mut req = req.body(body).map_err(new_request_build_error)?;
         self.sign(&mut req).await?;
         Ok(req)
     }
 
     /// Creates a request to upload a part
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 impl oio::Write for OssWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let mut req = self.core.oss_put_object_request(
             &self.path,
             Some(bs.len()),
             self.op.content_type(),
             self.op.content_disposition(),
+            self.op.cache_control(),
             AsyncBody::Bytes(bs),
             false,
         )?;
 
         self.core.sign(&mut req).await?;
 
         let resp = self.core.send(req).await?;
@@ -110,14 +111,21 @@
                 self.parts.push(MultipartUploadPart { part_number, etag });
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "output writer doesn't support abort",
+        ))
+    }
+
     async fn close(&mut self) -> Result<()> {
         let upload_id = if let Some(upload_id) = &self.upload_id {
             upload_id
         } else {
             return Ok(());
         };
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.31.1/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 use std::fmt::Formatter;
 use std::fmt::Write;
 use std::time::Duration;
 
 use backon::ExponentialBuilder;
 use backon::Retryable;
 use bytes::Bytes;
-use http::header::HeaderName;
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
+use http::header::{HeaderName, IF_NONE_MATCH};
 use http::HeaderValue;
 use http::Request;
 use http::Response;
 use once_cell::sync::Lazy;
 use reqsign::AwsCredential;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
@@ -211,15 +211,15 @@
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
 
         req = self.insert_sse_headers(req, false);
 
         if let Some(if_none_match) = if_none_match {
-            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
+            req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
@@ -261,15 +261,15 @@
         let mut req = Request::get(&url);
 
         if !range.is_full() {
             req = req.header(http::header::RANGE, range.to_header());
         }
 
         if let Some(if_none_match) = if_none_match {
-            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
+            req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         // Set SSE headers.
         // TODO: how will this work with presign?
         req = self.insert_sse_headers(req, false);
 
         let req = req
@@ -348,15 +348,15 @@
 
         let mut req = Request::head(&url);
 
         // Set SSE headers.
         req = self.insert_sse_headers(req, false);
 
         if let Some(if_none_match) = if_none_match {
-            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
+            req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
         let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
@@ -590,14 +590,36 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
+    /// Abort an on-going multipart upload.
+    pub async fn s3_abort_multipart_upload(
+        &self,
+        path: &str,
+        upload_id: &str,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!(
+            "{}/{}?uploadId={}",
+            self.endpoint,
+            percent_encode_path(&p),
+            percent_encode_path(upload_id)
+        );
+
+        let mut req = Request::delete(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+        self.sign(&mut req).await?;
+        self.send(req).await
+    }
+
     pub async fn s3_delete_objects(
         &self,
         paths: Vec<String>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let url = format!("{}/?delete", self.endpoint);
 
         let req = Request::post(&url);
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (mut kind, mut retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -121,14 +121,34 @@
 
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        let upload_id = if let Some(upload_id) = &self.upload_id {
+            upload_id
+        } else {
+            return Ok(());
+        };
+
+        let resp = self
+            .core
+            .s3_abort_multipart_upload(&self.path, upload_id)
+            .await?;
+        match resp.status() {
+            StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
     async fn close(&mut self) -> Result<()> {
         let upload_id = if let Some(upload_id) = &self.upload_id {
             upload_id
         } else {
             return Ok(());
         };
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files 4% similar despite different names*

```diff
@@ -66,32 +66,40 @@
 ///     Ok(())
 /// }
 /// ```
 #[derive(Default)]
 pub struct SledBuilder {
     /// That path to the sled data directory.
     datadir: Option<String>,
+    root: Option<String>,
 }
 
 impl SledBuilder {
     /// Set the path to the sled data directory. Will create if not exists.
     pub fn datadir(&mut self, path: &str) -> &mut Self {
         self.datadir = Some(path.into());
         self
     }
+
+    /// Set the root for sled.
+    pub fn root(&mut self, path: &str) -> &mut Self {
+        self.root = Some(path.into());
+        self
+    }
 }
 
 impl Builder for SledBuilder {
     const SCHEME: Scheme = Scheme::Sled;
     type Accessor = SledBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
         let mut builder = SledBuilder::default();
 
         map.get("datadir").map(|v| builder.datadir(v));
+        map.get("root").map(|v| builder.root(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
         let datadir_path = self.datadir.take().ok_or_else(|| {
             Error::new(ErrorKind::ConfigInvalid, "datadir is required but not set")
@@ -104,15 +112,16 @@
                 .with_context("datadir", datadir_path.clone())
                 .set_source(e)
         })?;
 
         Ok(SledBackend::new(Adapter {
             datadir: datadir_path,
             db,
-        }))
+        })
+        .with_root(self.root.as_deref().unwrap_or_default()))
     }
 }
 
 /// Backend for sled services.
 pub type SledBackend = kv::Backend<Adapter>;
 
 #[derive(Clone)]
@@ -170,14 +179,15 @@
 
     fn blocking_scan(&self, path: &str) -> Result<Vec<String>> {
         let it = self.db.scan_prefix(path).keys();
         let mut res = Vec::default();
 
         for i in it {
             let bs = i.map_err(parse_error)?.to_vec();
+
             res.push(String::from_utf8(bs).map_err(|err| {
                 Error::new(ErrorKind::Unexpected, "store key is not valid utf-8 string")
                     .set_source(err)
             })?);
         }
 
         Ok(res)
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/http/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (kind, retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
+        StatusCode::PRECONDITION_FAILED => (ErrorKind::PreconditionFailed, false),
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -68,11 +68,15 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
+    async fn abort(&mut self) -> Result<()> {
+        Ok(())
+    }
+
     async fn close(&mut self) -> Result<()> {
         Ok(())
     }
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,20 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use core::fmt::Debug;
 use std::collections::HashMap;
 
 use async_trait::async_trait;
-use bytes::Buf;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
-use http::response::Parts;
 use http::Request;
 use http::Response;
 use http::StatusCode;
 use log::debug;
-use log::error;
 use tokio::sync::OnceCell;
 
 use super::error::parse_error;
 use super::message::BooleanResp;
 use super::message::FileStatusType;
 use super::message::FileStatusWrapper;
 use super::message::FileStatusesWrapper;
@@ -72,14 +69,15 @@
 /// - `delegation`: The delegation token for WebHDFS.
 ///
 /// Refer to [`Builder`]'s public API docs for more information
 ///
 /// # Examples
 ///
 /// ## Via Builder
+///
 /// ```no_run
 /// use std::sync::Arc;
 ///
 /// use anyhow::Result;
 /// use opendal::services::Webhdfs;
 /// use opendal::Operator;
 ///
@@ -110,37 +108,33 @@
     root: Option<String>,
     endpoint: Option<String>,
     delegation: Option<String>,
 }
 
 impl Debug for WebhdfsBuilder {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        let mut ds = f.debug_struct("Builder");
-        ds.field("root", &self.root)
-            .field("endpoint", &self.endpoint);
-        if self.delegation.is_some() {
-            ds.field("delegation", &"<redacted>");
-        }
-        ds.finish()
+        f.debug_struct("Builder")
+            .field("root", &self.root)
+            .field("endpoint", &self.endpoint)
+            .finish_non_exhaustive()
     }
 }
 
 impl WebhdfsBuilder {
     /// Set the working directory of this backend
     ///
     /// All operations will happen under this root
+    ///
     /// # Note
+    ///
     /// The root will be automatically created if not exists.
-    /// If the root is occupied by a file, building of directory will fail
     pub fn root(&mut self, root: &str) -> &mut Self {
-        self.root = if root.is_empty() {
-            None
-        } else {
-            Some(root.to_string())
-        };
+        if !root.is_empty() {
+            self.root = Some(root.to_string())
+        }
 
         self
     }
 
     /// Set the remote address of this backend
     /// default to `http://127.0.0.1:9870`
     ///
@@ -157,63 +151,49 @@
             self.endpoint = Some(endpoint.trim_end_matches('/').to_string());
         }
         self
     }
 
     /// Set the delegation token of this backend,
     /// used for authentication
+    ///
     /// # Note
     /// The builder prefers using delegation token over username.
     /// If both are set, delegation token will be used.
     pub fn delegation(&mut self, delegation: &str) -> &mut Self {
         if !delegation.is_empty() {
             self.delegation = Some(delegation.to_string());
         }
         self
     }
 }
 
-impl WebhdfsBuilder {
-    fn auth_str(&mut self) -> Option<String> {
-        if let Some(dt) = self.delegation.take() {
-            return Some(format!("delegation_token={dt}"));
-        }
-        None
-    }
-}
-
 impl Builder for WebhdfsBuilder {
     const SCHEME: Scheme = Scheme::Webhdfs;
     type Accessor = WebhdfsBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
         let mut builder = WebhdfsBuilder::default();
 
-        for (k, v) in map.iter() {
-            let v = v.as_str();
-            match k.as_str() {
-                "root" => builder.root(v),
-                "endpoint" => builder.endpoint(v),
-                "delegation" => builder.delegation(v),
-                _ => continue,
-            };
-        }
+        map.get("root").map(|v| builder.root(v));
+        map.get("endpoint").map(|v| builder.endpoint(v));
+        map.get("delegation").map(|v| builder.delegation(v));
 
         builder
     }
 
     /// build the backend
     ///
-    /// # Note:
+    /// # Note
+    ///
     /// when building backend, the built backend will check if the root directory
     /// exits.
     /// if the directory does not exits, the directory will be automatically created
-    /// if the root path is occupied by a file, a failure will be returned
     fn build(&mut self) -> Result<Self::Accessor> {
-        debug!("building backend: {:?}", self);
+        debug!("start building backend: {:?}", self);
 
         let root = normalize_root(&self.root.take().unwrap_or_default());
         debug!("backend use root {root}");
 
         // check scheme
         let endpoint = match self.endpoint.take() {
             Some(endpoint) => {
@@ -223,44 +203,49 @@
                     format!("http://{endpoint}")
                 }
             }
             None => WEBHDFS_DEFAULT_ENDPOINT.to_string(),
         };
         debug!("backend use endpoint {}", endpoint);
 
-        let auth = self.auth_str();
+        let auth = self
+            .delegation
+            .take()
+            .map(|dt| format!("delegation_token={dt}"));
+
         let client = HttpClient::new()?;
 
         let backend = WebhdfsBackend {
-            root: root.clone(),
+            root,
             endpoint,
             auth,
             client,
             root_checker: OnceCell::new(),
         };
 
-        debug!("checking working directory: {}", root);
-
         Ok(backend)
     }
 }
 
 /// Backend for WebHDFS service
 #[derive(Debug, Clone)]
 pub struct WebhdfsBackend {
     root: String,
     endpoint: String,
-    pub client: HttpClient,
     auth: Option<String>,
     root_checker: OnceCell<()>,
+
+    pub client: HttpClient,
 }
 
 impl WebhdfsBackend {
-    // create object or make a directory
-    pub async fn webhdfs_create_object_req(
+    /// create object or make a directory
+    ///
+    /// TODO: we should split it into mkdir and create
+    pub async fn webhdfs_create_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
@@ -303,231 +288,170 @@
         if let Some(content_type) = content_type {
             re_builder = re_builder.header(CONTENT_TYPE, content_type);
         }
 
         re_builder.body(body).map_err(new_request_build_error)
     }
 
-    async fn webhdfs_open_req(&self, path: &str, range: &BytesRange) -> Result<Request<AsyncBody>> {
+    async fn webhdfs_open_request(
+        &self,
+        path: &str,
+        range: &BytesRange,
+    ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let mut url = format!(
             "{}/webhdfs/v1/{}?op=OPEN",
             self.endpoint,
             percent_encode_path(&p),
         );
         if let Some(auth) = &self.auth {
-            url += format!("&{auth}").as_str();
+            url += &format!("&{auth}");
         }
 
-        // make a Webhdfs compatible bytes range
-        //
-        // Webhdfs does not support read from end
-        // have to solve manually
-        let range = match (range.offset(), range.size()) {
-            // avoiding reading the whole file
-            (None, Some(size)) => {
-                debug!("converting bytes range to webhdfs compatible");
-                let status = self.stat(path, OpStat::default()).await?;
-                let total_size = status.into_metadata().content_length();
-                let offset = total_size - size;
-                BytesRange::new(Some(offset), Some(size))
-            }
-            _ => *range,
-        };
-
-        let (offset, size) = (range.offset(), range.size());
+        if !range.is_full() {
+            // Webhdfs does not support read from end
+            if range.offset().is_none() && range.size().is_some() {
+                return Err(Error::new(
+                    ErrorKind::Unsupported,
+                    "webhdfs doesn't support read with suffix range",
+                ));
+            };
 
-        match (offset, size) {
-            (Some(offset), Some(size)) => {
-                url += format!("&offset={offset}&length={size}").as_str();
+            if let Some(offset) = range.offset() {
+                url += &format!("&offset={offset}");
             }
-            (Some(offset), None) => {
-                url += format!("&offset={offset}").as_str();
-            }
-            (None, None) => {
-                // read all, do nothing
-            }
-            (None, Some(_)) => {
-                // already handled
-                unreachable!()
+            if let Some(size) = range.size() {
+                url += &format!("&length={size}")
             }
         }
 
         let req = Request::get(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    fn webhdfs_list_status_req(&self, path: &str) -> Result<Request<AsyncBody>> {
+    fn webhdfs_list_status_request(&self, path: &str) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let mut url = format!(
             "{}/webhdfs/v1/{}?op=LISTSTATUS",
             self.endpoint,
             percent_encode_path(&p),
         );
         if let Some(auth) = &self.auth {
             url += format!("&{auth}").as_str();
         }
 
-        let req = Request::get(&url);
-        let req = req
+        let req = Request::get(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
         Ok(req)
     }
-}
 
-impl WebhdfsBackend {
-    /// get object from webhdfs
-    ///
-    /// # Notes
-    ///
-    /// looks like webhdfs doesn't support range request from file end.
-    /// so if we want to read the tail of object, the whole object should be transferred.
-    async fn webhdfs_get_object(
+    async fn webhdfs_read_file(
         &self,
         path: &str,
         range: BytesRange,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let req = self.webhdfs_open_req(path, &range).await?;
+        let req = self.webhdfs_open_request(path, &range).await?;
         let resp = self.client.send(req).await?;
 
-        // this should be a 307 redirect
+        // webhdfs namenode will redirect us to datanode for data transfer.
         if resp.status() != StatusCode::TEMPORARY_REDIRECT {
             return Err(parse_error(resp).await?);
         }
 
-        let re_url = self.follow_redirect(resp)?;
-        let re_req = Request::get(&re_url)
+        let location = self.follow_redirect(resp)?;
+        let req = Request::get(&location)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
-        self.client.send(re_req).await
+        self.client.send(req).await
     }
 
-    async fn webhdfs_status_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    async fn webhdfs_get_file_status(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let mut url = format!(
             "{}/webhdfs/v1/{}?op=GETFILESTATUS",
             self.endpoint,
             percent_encode_path(&p),
         );
-        debug!("webhdfs status url: {}", url);
+
         if let Some(auth) = &self.auth {
             url += format!("&{auth}").as_str();
         }
 
-        let req = Request::get(&url);
-        let req = req
+        let req = Request::get(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
 
-    async fn webhdfs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    async fn webhdfs_delete(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
         let mut url = format!(
             "{}/webhdfs/v1/{}?op=DELETE&recursive=false",
             self.endpoint,
             percent_encode_path(&p),
         );
         if let Some(auth) = &self.auth {
             url += format!("&{auth}").as_str();
         }
 
-        let req = Request::delete(&url);
-        let req = req
+        let req = Request::delete(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
-}
 
-impl WebhdfsBackend {
     /// get redirect destination from 307 TEMPORARY_REDIRECT http response
     fn follow_redirect(&self, resp: Response<IncomingAsyncBody>) -> Result<String> {
-        let loc = match parse_location(resp.headers())? {
-            Some(p) => {
-                if !p.starts_with('/') {
-                    // is not relative path
-                    p.to_string()
-                } else {
-                    // is relative path
-                    // prefix with endpoint url
-                    let url = self.endpoint.clone();
-                    format!("{url}/{p}")
-                }
-            }
-            None => {
-                let err = Error::new(
-                    ErrorKind::Unexpected,
-                    "redirection fail: no location header",
-                );
-                return Err(err);
-            }
-        };
-        Ok(loc)
-    }
-
-    fn consume_success_mkdir(&self, path: &str, parts: Parts, body: &str) -> Result<RpCreate> {
-        let mkdir_rsp = serde_json::from_str::<BooleanResp>(body).map_err(|e| {
-            Error::new(ErrorKind::Unexpected, "cannot parse mkdir response")
-                .set_temporary()
-                .with_context("service", Scheme::Webhdfs)
-                .with_context("response", format!("{parts:?}"))
-                .set_source(e)
+        let location = parse_location(resp.headers())?.ok_or_else(|| {
+            Error::new(
+                ErrorKind::Unexpected,
+                "webhdfs expect to have redirect location but got none",
+            )
         })?;
 
-        if mkdir_rsp.boolean {
-            Ok(RpCreate::default())
+        let location = if location.starts_with('/') {
+            // location starts with `/` means it's a relative path to current
+            // endpoint. We should prepend the endpoint to it so that we can
+            // send request to the correct location.
+            format!("{}/{location}", self.endpoint)
         } else {
-            Err(Error::new(
-                ErrorKind::Unexpected,
-                &format!("mkdir failed: {path}"),
-            ))
-        }
+            location.to_string()
+        };
+
+        Ok(location)
     }
 
     async fn check_root(&self) -> Result<()> {
-        let resp = self.webhdfs_status_object("/").await?;
+        let resp = self.webhdfs_get_file_status("/").await?;
         match resp.status() {
             StatusCode::OK => {
-                let body_bs = resp.into_body().bytes().await?;
+                let bs = resp.into_body().bytes().await?;
 
-                let file_status = serde_json::from_reader::<_, FileStatusWrapper>(body_bs.reader())
-                    .map_err(|e| {
-                        Error::new(ErrorKind::Unexpected, "cannot parse returned json")
-                            .with_context("service", Scheme::Webhdfs)
-                            .set_source(e)
-                    })?
+                let file_status = serde_json::from_slice::<FileStatusWrapper>(&bs)
+                    .map_err(new_json_deserialize_error)?
                     .file_status;
 
-                match file_status.ty {
-                    FileStatusType::File => {
-                        error!("working directory is occupied!");
-                        return Err(Error::new(ErrorKind::ConfigInvalid, "root is occupied!")
-                            .with_context("service", Scheme::Webhdfs));
-                    }
-                    FileStatusType::Directory => {
-                        debug!("working directory exists, do nothing");
-                    }
+                if file_status.ty == FileStatusType::File {
+                    return Err(Error::new(
+                        ErrorKind::ConfigInvalid,
+                        "root path must be dir",
+                    ));
                 }
             }
-
             StatusCode::NOT_FOUND => {
-                debug!("working directory does not exists, creating...");
                 self.create("/", OpCreate::new(EntryMode::DIR)).await?;
             }
-
             _ => return Err(parse_error(resp).await?),
         }
-        debug!("working directory is ready!");
         Ok(())
     }
 }
 
 #[async_trait]
 impl Accessor for WebhdfsBackend {
     type Reader = IncomingAsyncBody;
@@ -545,63 +469,55 @@
                 AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
             )
             .set_hints(AccessorHint::ReadStreamable);
         am
     }
 
     /// Create a file or directory
-    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
-        // if the path ends with '/', it will be treated as a directory
-        // otherwise, it will be treated as a file
-        let path = if args.mode().is_file() && path.ends_with('/') {
-            path.trim_end_matches('/').to_owned()
-        } else if args.mode().is_dir() && !path.ends_with('/') {
-            path.to_owned() + "/"
-        } else {
-            path.to_owned()
-        };
-
+    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
         let req = self
-            .webhdfs_create_object_req(&path, Some(0), None, AsyncBody::Empty)
+            .webhdfs_create_object_request(path, Some(0), None, AsyncBody::Empty)
             .await?;
 
         let resp = self.client.send(req).await?;
 
         let status = resp.status();
 
         // WebHDFS's has a two-step create/append to prevent clients to send out
         // data before creating it.
         // According to the redirect policy of `reqwest` HTTP Client we are using,
         // the redirection should be done automatically.
         match status {
             StatusCode::CREATED | StatusCode::OK => {
-                if !path.ends_with('/') {
-                    // create file's http resp could be ignored
-                    resp.into_body().consume().await?;
-                    return Ok(RpCreate::default());
+                let bs = resp.into_body().bytes().await?;
+
+                let resp = serde_json::from_slice::<BooleanResp>(&bs)
+                    .map_err(new_json_deserialize_error)?;
+
+                if resp.boolean {
+                    Ok(RpCreate::default())
+                } else {
+                    Err(Error::new(
+                        ErrorKind::Unexpected,
+                        "webhdfs create dir failed",
+                    ))
                 }
-                let (parts, body) = resp.into_parts();
-                let bs = body.bytes().await?;
-                let s = String::from_utf8_lossy(&bs);
-                self.consume_success_mkdir(&path, parts, &s)
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let range = args.range();
-        let resp = self.webhdfs_get_object(path, range).await?;
+        let resp = self.webhdfs_read_file(path, range).await?;
         match resp.status() {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
-            StatusCode::NOT_FOUND => Err(Error::new(ErrorKind::NotFound, "object not found")
-                .with_context("service", Scheme::Webhdfs)),
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         if args.append() {
             return Err(Error::new(
@@ -618,71 +534,64 @@
 
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         // if root exists and is a directory, stat will be ok
         self.root_checker
             .get_or_try_init(|| async { self.check_root().await })
             .await?;
 
-        let resp = self.webhdfs_status_object(path).await?;
+        let resp = self.webhdfs_get_file_status(path).await?;
         let status = resp.status();
         match status {
             StatusCode::OK => {
-                debug!("stat object: {} ok", path);
-                let mut meta = parse_into_metadata(path, resp.headers())?;
-                let body_bs = resp.into_body().bytes().await?;
-
-                let file_status = serde_json::from_reader::<_, FileStatusWrapper>(body_bs.reader())
-                    .map_err(|e| {
-                        Error::new(ErrorKind::Unexpected, "cannot parse returned json")
-                            .with_context("service", Scheme::Webhdfs)
-                            .set_source(e)
-                    })?
+                let bs = resp.into_body().bytes().await?;
+
+                let file_status = serde_json::from_slice::<FileStatusWrapper>(&bs)
+                    .map_err(new_json_deserialize_error)?
                     .file_status;
-                debug!("file status: {:?}", file_status);
-                let status_meta: Metadata = file_status.try_into()?;
 
-                // is ok to unwrap here
-                // all metadata field of status meta is present and checked by `TryFrom`
-                meta.set_last_modified(status_meta.last_modified().unwrap())
-                    .set_content_length(status_meta.content_length());
+                let meta = match file_status.ty {
+                    FileStatusType::Directory => Metadata::new(EntryMode::DIR),
+                    FileStatusType::File => Metadata::new(EntryMode::FILE)
+                        .with_content_length(file_status.length)
+                        .with_last_modified(parse_datetime_from_from_timestamp_millis(
+                            file_status.modification_time,
+                        )?),
+                };
+
                 Ok(RpStat::new(meta))
             }
 
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.webhdfs_delete_object(path).await?;
+        let resp = self.webhdfs_delete(path).await?;
+
         match resp.status() {
             StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(RpDelete::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, _: OpList) -> Result<(RpList, Self::Pager)> {
         let path = path.trim_end_matches('/');
-        let req = self.webhdfs_list_status_req(path)?;
+        let req = self.webhdfs_list_status_request(path)?;
 
         let resp = self.client.send(req).await?;
         match resp.status() {
             StatusCode::OK => {
-                let body_bs = resp.into_body().bytes().await?;
-                let file_statuses =
-                    serde_json::from_reader::<_, FileStatusesWrapper>(body_bs.reader())
-                        .map_err(|e| {
-                            Error::new(ErrorKind::Unexpected, "cannot parse returned json")
-                                .with_context("service", Scheme::Webhdfs)
-                                .set_source(e)
-                        })?
-                        .file_statuses
-                        .file_status;
+                let bs = resp.into_body().bytes().await?;
+                let file_statuses = serde_json::from_slice::<FileStatusesWrapper>(&bs)
+                    .map_err(new_json_deserialize_error)?
+                    .file_statuses
+                    .file_status;
 
                 let objects = WebhdfsPager::new(path, file_statuses);
                 Ok((RpList::default(), objects))
             }
             StatusCode::NOT_FOUND => {
                 let objects = WebhdfsPager::new(path, vec![]);
                 Ok((RpList::default(), objects))
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,18 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-//! HTTP response messages
+//! WebHDFS response messages
 
 use serde::Deserialize;
 
-use crate::raw::*;
-use crate::*;
-
 #[derive(Debug, Deserialize)]
 pub(super) struct BooleanResp {
     pub boolean: bool,
 }
 
 #[derive(Debug, Deserialize)]
 #[serde(rename_all = "PascalCase")]
@@ -52,30 +49,14 @@
     pub modification_time: i64,
 
     pub path_suffix: String,
     #[serde(rename = "type")]
     pub ty: FileStatusType,
 }
 
-impl TryFrom<FileStatus> for Metadata {
-    type Error = Error;
-    fn try_from(value: FileStatus) -> Result<Self> {
-        let mut meta = match value.ty {
-            FileStatusType::Directory => Metadata::new(EntryMode::DIR),
-            FileStatusType::File => Metadata::new(EntryMode::FILE),
-        };
-
-        meta.set_last_modified(parse_datetime_from_from_timestamp_millis(
-            value.modification_time,
-        )?)
-        .set_content_length(value.length);
-        Ok(meta)
-    }
-}
-
 #[derive(Debug, Deserialize, PartialEq, Eq)]
 #[serde(rename_all = "UPPERCASE")]
 pub enum FileStatusType {
     Directory,
     File,
 }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.31.1/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
 
-use super::message::FileStatus;
+use super::message::{FileStatus, FileStatusType};
 use crate::raw::*;
 use crate::*;
 
 pub struct WebhdfsPager {
     path: String,
     statuses: Vec<FileStatus>,
 }
@@ -41,17 +41,32 @@
         if self.statuses.is_empty() {
             return Ok(None);
         }
 
         let mut entries = Vec::with_capacity(self.statuses.len());
 
         while let Some(status) = self.statuses.pop() {
-            let mut path = format!("{}/{}", &self.path, status.path_suffix);
+            let mut path = if self.path.is_empty() {
+                status.path_suffix.to_string()
+            } else {
+                format!("{}/{}", self.path, status.path_suffix)
+            };
+
+            let meta = match status.ty {
+                FileStatusType::Directory => Metadata::new(EntryMode::DIR),
+                FileStatusType::File => Metadata::new(EntryMode::FILE)
+                    .with_content_length(status.length)
+                    .with_last_modified(parse_datetime_from_from_timestamp_millis(
+                        status.modification_time,
+                    )?),
+            };
 
-            let meta: Metadata = status.try_into()?;
+            if meta.mode().is_file() {
+                path = path.trim_end_matches('/').to_string();
+            }
             if meta.mode().is_dir() {
                 path += "/"
             }
             let entry = oio::Entry::new(&path, meta);
             entries.push(entry);
         }
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/error.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,19 @@
     NotADirectory,
     /// The given path already exists thus we failed to the specified operation on it.
     AlreadyExists,
     /// Requests that sent to this path is over the limit, please slow down.
     RateLimited,
     /// The given file paths are same.
     IsSameFile,
+    /// The preconfition of this operation is not met.
+    ///
+    /// For example, reading a file with If-Match header but the file's ETag
+    /// is not match.
+    PreconditionFailed,
 }
 
 impl ErrorKind {
     /// Convert self into static str.
     pub fn into_static(self) -> &'static str {
         self.into()
     }
@@ -94,14 +99,15 @@
             ErrorKind::NotFound => "NotFound",
             ErrorKind::PermissionDenied => "PermissionDenied",
             ErrorKind::IsADirectory => "IsADirectory",
             ErrorKind::NotADirectory => "NotADirectory",
             ErrorKind::AlreadyExists => "AlreadyExists",
             ErrorKind::RateLimited => "RateLimited",
             ErrorKind::IsSameFile => "IsSameFile",
+            ErrorKind::PreconditionFailed => "PreconditionFailed",
         }
     }
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
 enum ErrorStatus {
     /// Permanent means without external changes, the error never changes.
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/list.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -714,18 +714,22 @@
 
         let (_, pager) = self.inner().blocking_list(&path, OpList::new())?;
         Ok(BlockingLister::new(pager))
     }
 
     /// List dir in flat way.
     ///
-    /// This function will create a new handle to list entries.
+    /// Also, this function can be used to list a prefix.
     ///
     /// An error will be returned if given path doesn't end with `/`.
     ///
+    /// # Notes
+    ///
+    /// - `scan` will not return the prefix itself.
+    ///
     /// # Examples
     ///
     /// ```no_run
     /// # use opendal::Result;
     /// # use futures::io;
     /// # use opendal::BlockingOperator;
     /// # use opendal::EntryMode;
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -176,17 +176,53 @@
     ///         println!("file not exist")
     ///     }
     /// }
     /// # Ok(())
     /// # }
     /// ```
     pub async fn stat(&self, path: &str) -> Result<Metadata> {
+        self.stat_with(path, OpStat::new()).await
+    }
+
+    /// Get current path's metadata **without cache** directly with extra options.
+    ///
+    /// # Notes
+    ///
+    /// Use `stat` if you:
+    ///
+    /// - Want detect the outside changes of path.
+    /// - Don't want to read from cached metadata.
+    ///
+    /// You may want to use `metadata` if you are working with entries
+    /// returned by [`Lister`]. It's highly possible that metadata
+    /// you want has already been cached.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use anyhow::Result;
+    /// # use futures::io;
+    /// # use opendal::Operator;
+    /// # use opendal::ops::OpStat;
+    /// use opendal::ErrorKind;
+    /// #
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// if let Err(e) = op.stat_with("test", OpStat::new()).await {
+    ///     if e.kind() == ErrorKind::NotFound {
+    ///         println!("file not exist")
+    ///     }
+    /// }
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn stat_with(&self, path: &str, args: OpStat) -> Result<Metadata> {
         let path = normalize_path(path);
 
-        let rp = self.inner().stat(&path, OpStat::new()).await?;
+        let rp = self.inner().stat(&path, args).await?;
         let meta = rp.into_metadata();
 
         Ok(meta)
     }
 
     /// Get current metadata with cache.
     ///
@@ -378,52 +414,104 @@
     /// # Ok(())
     /// # }
     /// ```
     pub async fn read(&self, path: &str) -> Result<Vec<u8>> {
         self.range_read(path, ..).await
     }
 
+    /// Read the whole path into a bytes with extra options.
+    ///
+    /// This function will allocate a new bytes internally. For more precise memory control or
+    /// reading data lazily, please use [`Operator::reader`]
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::Operator;
+    /// # use opendal::ops::OpRead;
+    /// # use futures::TryStreamExt;
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// let bs = op.read_with("path/to/file", OpRead::new()).await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn read_with(&self, path: &str, args: OpRead) -> Result<Vec<u8>> {
+        self.range_read_with(path, .., args).await
+    }
+
     /// Read the specified range of path into a bytes.
     ///
     /// This function will allocate a new bytes internally. For more precise memory control or
     /// reading data lazily, please use [`Operator::range_reader`]
     ///
     /// # Notes
     ///
     /// - The returning content's length may be smaller than the range specified.
     ///
     /// # Examples
     ///
     /// ```
     /// # use std::io::Result;
     /// # use opendal::Operator;
+    /// # use opendal::ops::OpRead;
     /// # use futures::TryStreamExt;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
     /// let bs = op.range_read("path/to/file", 1024..2048).await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn range_read(&self, path: &str, range: impl RangeBounds<u64>) -> Result<Vec<u8>> {
+        self.range_read_with(path, range, OpRead::new()).await
+    }
+
+    /// Read the specified range of path into a bytes with extra options..
+    ///
+    /// This function will allocate a new bytes internally. For more precise memory control or
+    /// reading data lazily, please use [`Operator::range_reader`]
+    ///
+    /// # Notes
+    ///
+    /// - The returning content's length may be smaller than the range specified.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::Operator;
+    /// # use opendal::ops::OpRead;
+    /// # use futures::TryStreamExt;
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// let bs = op.range_read_with("path/to/file", 1024..2048, OpRead::new()).await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn range_read_with(
+        &self,
+        path: &str,
+        range: impl RangeBounds<u64>,
+        args: OpRead,
+    ) -> Result<Vec<u8>> {
         let path = normalize_path(path);
 
         if !validate_path(&path, EntryMode::FILE) {
             return Err(
                 Error::new(ErrorKind::IsADirectory, "read path is a directory")
                     .with_operation("range_read")
                     .with_context("service", self.inner().info().scheme())
                     .with_context("path", &path),
             );
         }
 
         let br = BytesRange::from(range);
 
-        let op = OpRead::new().with_range(br);
-
-        let (rp, mut s) = self.inner().read(&path, op).await?;
+        let (rp, mut s) = self.inner().read(&path, args.with_range(br)).await?;
 
         let length = rp.into_metadata().content_length() as usize;
         let mut buffer = Vec::with_capacity(length);
 
         let dst = buffer.spare_capacity_mut();
         let mut buf = ReadBuf::uninit(dst);
 
@@ -940,14 +1028,17 @@
                 }
             }
         } else {
             obs.try_for_each(|v| async move { self.delete(v.path()).await })
                 .await?;
         }
 
+        // Remove the directory itself.
+        self.delete(path).await?;
+
         Ok(())
     }
 
     /// List given path.
     ///
     /// This function will create a new handle to list entries.
     ///
@@ -996,18 +1087,22 @@
         let (_, pager) = self.inner().list(&path, OpList::new()).await?;
 
         Ok(Lister::new(pager))
     }
 
     /// List dir in flat way.
     ///
-    /// This function will create a new handle to list entries.
+    /// Also, this function can be used to list a prefix.
     ///
     /// An error will be returned if given path doesn't end with `/`.
     ///
+    /// # Notes
+    ///
+    /// - `scan` will not return the prefix itself.
+    ///
     /// # Examples
     ///
     /// ```no_run
     /// # use anyhow::Result;
     /// # use futures::io;
     /// use futures::TryStreamExt;
     /// use opendal::EntryMode;
```

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/ops.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/scheme.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.31.1/local_dependencies/opendal/src/types/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/Cargo.toml` & `opendal-0.31.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.64"
-version= "0.31.0"
+version= "0.31.1"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 chrono = { version = "0.4.24", default-features = false, features = ["std"] }
```

### Comparing `opendal-0.31.0/.gitignore` & `opendal-0.31.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/README.md` & `opendal-0.31.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # OpenDAL Python Binding
 
+Documentation: [main](https://opendal.apache.org/docs/python/)
+
 This crate intends to build a native python binding.
 
 ## Installation
 
 ```bash
 pip install opendal
 ```
@@ -66,8 +68,8 @@
 ```
 
 Build API docs:
 
 ```shell
 maturin develop -E docs
 pdoc opendal
-```
+```
```

### Comparing `opendal-0.31.0/benchmark/README.md` & `opendal-0.31.1/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/benchmark/async_opendal_benchmark.py` & `opendal-0.31.1/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.31.1/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/pyproject.toml` & `opendal-0.31.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
   "pydantic",
   "boto3-stubs[essential]",
 ]
 docs = ["pdoc"]
 test = ["behave"]
 
 [project.urls]
-Documentation = "https://docs.rs/opendal/"
+Documentation = "https://opendal.apache.org/docs/python/opendal.html"
 Homepage = "https://opendal.apache.org/"
 Repository = "https://github.com/apache/incubator-opendal"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 module-name = "opendal._opendal"
 python-source = "python"
```

### Comparing `opendal-0.31.0/python/opendal/__init__.py` & `opendal-0.31.1/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/python/opendal/__init__.pyi` & `opendal-0.31.1/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/src/asyncio.rs` & `opendal-0.31.1/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/src/layers.rs` & `opendal-0.31.1/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/src/lib.rs` & `opendal-0.31.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/tests/binding.feature` & `opendal-0.31.1/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/tests/steps/binding.py` & `opendal-0.31.1/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.31.0/Cargo.lock` & `opendal-0.31.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1917,14 +1917,51 @@
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
+name = "minitrace"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "317e28b8c337ada2fd437611c241ce053d5b7f5480b79e945597996b87b1de96"
+dependencies = [
+ "futures",
+ "minitrace-macro",
+ "minstant",
+ "once_cell",
+ "parking_lot 0.12.1",
+ "pin-project",
+]
+
+[[package]]
+name = "minitrace-macro"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77814d165883613a1846517efdc50b88fabd9c210b7ff4d3745b38b99d539652"
+dependencies = [
+ "proc-macro-error",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "minstant"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc5dcfca9a0725105ac948b84cfeb69c3942814c696326743797215413f854b9"
+dependencies = [
+ "ctor",
+ "libc",
+ "wasi 0.7.0",
+]
+
+[[package]]
 name = "mio"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
@@ -2146,27 +2183,27 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.31.0"
+version = "0.31.1"
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
-version = "0.31.0"
+version = "0.31.1"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.1.11",
  "dirs",
  "env_logger",
  "futures",
@@ -2189,15 +2226,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.31.0"
+version = "0.31.1"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
@@ -2214,23 +2251,25 @@
  "hdrs",
  "http",
  "hyper",
  "lazy-regex",
  "log",
  "md-5",
  "metrics",
+ "minitrace",
  "moka",
  "once_cell",
  "opentelemetry 0.19.0",
  "opentelemetry-jaeger",
  "parking_lot 0.12.1",
  "paste",
  "percent-encoding",
  "pin-project",
  "pretty_assertions",
+ "prometheus",
  "prost",
  "quick-xml 0.27.1",
  "rand 0.8.5",
  "redis",
  "reqsign",
  "reqwest",
  "rocksdb",
@@ -2263,26 +2302,26 @@
 dependencies = [
  "jni",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.31.0"
+version = "0.31.1"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.31.0"
+version = "0.31.1"
 dependencies = [
  "chrono",
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
@@ -2735,23 +2774,77 @@
  "ctor",
  "diff",
  "output_vt100",
  "yansi",
 ]
 
 [[package]]
+name = "proc-macro-error"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
+dependencies = [
+ "proc-macro-error-attr",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "version_check",
+]
+
+[[package]]
+name = "proc-macro-error-attr"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "version_check",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "procfs"
+version = "0.14.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1de8dacb0873f77e6aefc6d71e044761fcc68060290f5b1089fcdf84626bb69"
+dependencies = [
+ "bitflags 1.3.2",
+ "byteorder",
+ "hex",
+ "lazy_static",
+ "rustix",
+]
+
+[[package]]
+name = "prometheus"
+version = "0.13.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "449811d15fbdf5ceb5c1144416066429cf82316e2ec8ce0c1f6f8a02e7bbcf8c"
+dependencies = [
+ "cfg-if",
+ "fnv",
+ "lazy_static",
+ "libc",
+ "memchr",
+ "parking_lot 0.12.1",
+ "procfs",
+ "protobuf",
+ "thiserror",
+]
+
+[[package]]
 name = "prost"
 version = "0.11.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e48e50df39172a3e7eb17e14642445da64996989bc212b583015435d39a58537"
 dependencies = [
  "bytes",
  "prost-derive",
@@ -2767,14 +2860,20 @@
  "itertools",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "protobuf"
+version = "2.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "106dd99e98437432fed6519dedecfade6a06a73bb7b2a1e019fdd2bee5778d94"
+
+[[package]]
 name = "pulldown-cmark"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d9cc634bc78768157b5cbfe988ffcd1dcba95cd2b2f03a88316c08c6d00ed63"
 dependencies = [
  "bitflags 1.3.2",
  "memchr",
@@ -4267,14 +4366,20 @@
 dependencies = [
  "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b89c3ce4ce14bdc6fb6beaf9ec7928ca331de5df7e5ea278375642a2f478570d"
+
+[[package]]
+name = "wasi"
 version = "0.9.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cccddf32554fecc6acb585f82a32a72e28b48f8c4c1883ddfeeeaa96f7d8e519"
 
 [[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
```

### Comparing `opendal-0.31.0/PKG-INFO` & `opendal-0.31.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.31.0
+Version: 0.31.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: behave; extra == 'test'
 Requires-Dist: gevent; extra == 'benchmark'
 Requires-Dist: greenify; extra == 'benchmark'
 Requires-Dist: greenlet; extra == 'benchmark'
 Requires-Dist: boto3; extra == 'benchmark'
 Requires-Dist: pydantic; extra == 'benchmark'
 Requires-Dist: boto3-stubs[essential]; extra == 'benchmark'
-Requires-Dist: behave; extra == 'test'
 Requires-Dist: pdoc; extra == 'docs'
-Provides-Extra: benchmark
 Provides-Extra: test
+Provides-Extra: benchmark
 Provides-Extra: docs
 Summary: OpenDAL Python Binding
 Home-Page: https://opendal.apache.org/
 Author: OpenDAL Contributors <dev@opendal.apache.org>
 Author-email: OpenDAL Contributors <dev@opendal.apache.org>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://docs.rs/opendal/
+Project-URL: Documentation, https://opendal.apache.org/docs/python/opendal.html
 Project-URL: Homepage, https://opendal.apache.org/
 Project-URL: Repository, https://github.com/apache/incubator-opendal
 
 # OpenDAL Python Binding
 
+Documentation: [main](https://opendal.apache.org/docs/python/)
+
 This crate intends to build a native python binding.
 
 ## Installation
 
 ```bash
 pip install opendal
 ```
@@ -95,7 +97,8 @@
 
 Build API docs:
 
 ```shell
 maturin develop -E docs
 pdoc opendal
 ```
+
```

