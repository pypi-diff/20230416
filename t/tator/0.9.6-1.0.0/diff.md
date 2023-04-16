# Comparing `tmp/tator-0.9.6.tar.gz` & `tmp/tator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tator-0.9.6.tar", last modified: Thu Feb 11 02:59:37 2021, max compression
+gzip compressed data, was "tator-1.0.0.tar", last modified: Sun Apr 16 18:09:50 2023, max compression
```

## Comparing `tator-0.9.6.tar` & `tator-1.0.0.tar`

### file list

```diff
@@ -1,213 +1,292 @@
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.886551 tator-0.9.6/
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)       34 2020-10-20 18:49:46.000000 tator-0.9.6/MANIFEST.in
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      321 2021-02-11 02:59:37.886551 tator-0.9.6/PKG-INFO
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      692 2020-10-20 18:49:46.000000 tator-0.9.6/README.md
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)       51 2020-12-31 04:18:03.000000 tator-0.9.6/pyproject.toml
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)       38 2021-02-11 02:59:37.886551 tator-0.9.6/setup.cfg
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     3654 2021-01-04 02:48:34.000000 tator-0.9.6/setup.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.870551 tator-0.9.6/tator/
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      600 2020-10-20 18:49:46.000000 tator-0.9.6/tator/__init__.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.870551 tator-0.9.6/tator/extractor/
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)        0 2020-12-23 02:59:42.000000 tator-0.9.6/tator/extractor/__init__.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     3621 2020-12-23 02:59:42.000000 tator-0.9.6/tator/extractor/__main__.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1564 2020-12-23 02:59:42.000000 tator-0.9.6/tator/extractor/env_launcher.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)    12359 2020-12-23 02:59:42.000000 tator-0.9.6/tator/extractor/extractor.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.870551 tator-0.9.6/tator/openapi/
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)       61 2020-10-20 18:49:46.000000 tator-0.9.6/tator/openapi/__init__.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.870551 tator-0.9.6/tator/openapi/tator_openapi/
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     8814 2021-02-11 02:59:36.000000 tator-0.9.6/tator/openapi/tator_openapi/__init__.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.870551 tator-0.9.6/tator/openapi/tator_openapi/api/
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)      150 2021-02-11 02:59:36.000000 tator-0.9.6/tator/openapi/tator_openapi/api/__init__.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)  1177621 2021-02-11 02:59:36.000000 tator-0.9.6/tator/openapi/tator_openapi/api/tator_api.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    26191 2021-02-11 02:59:36.000000 tator-0.9.6/tator/openapi/tator_openapi/api_client.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    13218 2021-02-11 02:59:36.000000 tator-0.9.6/tator/openapi/tator_openapi/configuration.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3713 2021-02-11 02:59:36.000000 tator-0.9.6/tator/openapi/tator_openapi/exceptions.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.882551 tator-0.9.6/tator/openapi/tator_openapi/models/
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     8224 2021-02-11 02:59:36.000000 tator-0.9.6/tator/openapi/tator_openapi/models/__init__.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5781 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/affiliation.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4305 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/affiliation_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3513 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/affiliation_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     7451 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/algorithm.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4241 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_launch.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5664 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_launch_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3019 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_manifest.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3747 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3905 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_parameter.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6932 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4152 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/analysis.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3980 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/analysis_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4242 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/archive_config.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3375 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/attribute_bulk_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    12453 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4013 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type_delete.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3763 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5602 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    13117 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type_update_new_attribute_type.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     8058 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/audio_definition.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3160 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/autocomplete_service.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3705 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/bad_request_response.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5353 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/bookmark.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3479 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/bookmark_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3495 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/bookmark_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5302 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/clone_media_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6713 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/color_map.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3677 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/create_list_response.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3615 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/create_response.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3931 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/credentials.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3485 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/download_info.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3069 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/download_info_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3850 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/email_attachment_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5904 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/email_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6278 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/encode_config.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6525 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/favorite.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5491 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/favorite_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     2983 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/favorite_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3854 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/fill.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6525 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/image_definition.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     7272 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/job.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5756 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/job_node.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6316 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/leaf.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4346 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/leaf_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4165 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/leaf_suggestion.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6121 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/leaf_type.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4419 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/leaf_type_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3653 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/leaf_type_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3633 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/leaf_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    17815 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/localization.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    12732 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/localization_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    10285 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/localization_type.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     9751 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/localization_type_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6781 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/localization_type_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    11181 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/localization_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    14874 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     7743 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_files.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3141 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_next.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3141 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_prev.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    12155 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5697 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_stats.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    11350 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_type.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    10587 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_type_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6548 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_type_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     9586 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/media_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6467 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/membership.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5693 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/membership_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4593 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/membership_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3057 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/message_response.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4259 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/multi_definition.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3077 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/not_found_response.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3902 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/notify_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3513 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/organization.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3157 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/organization_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    10090 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/project.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5648 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/project_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4972 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/project_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5524 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/resolution_config.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4639 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/s3_storage_config.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     8258 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/section.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     7302 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/section_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     7180 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/section_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    10403 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/state.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3465 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/state_merge_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5964 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/state_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4604 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/state_trim_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    11623 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/state_type.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    10531 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/state_type_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     6301 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/state_type_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5561 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/state_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     7383 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/temporary_file.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5689 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/temporary_file_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     2925 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/token.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4093 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/transcode.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    10545 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/transcode_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4532 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/upload_completion_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4577 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/upload_info.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     3883 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/upload_part.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5217 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/user.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4791 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/user_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     7326 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/version.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5150 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/version_spec.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     5020 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/version_update.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     4827 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/video_clip.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)     9726 2021-02-11 02:59:35.000000 tator-0.9.6/tator/openapi/tator_openapi/models/video_definition.py
--rw-r--r--   0 transcoder  (1007) transcoder  (1009)    12246 2021-02-11 02:59:36.000000 tator-0.9.6/tator/openapi/tator_openapi/rest.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.882551 tator-0.9.6/tator/transcode/
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)        0 2020-10-20 18:49:46.000000 tator-0.9.6/tator/transcode/__init__.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     4458 2021-01-22 05:20:01.000000 tator-0.9.6/tator/transcode/__main__.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2105 2020-10-20 18:49:46.000000 tator-0.9.6/tator/transcode/black.mp4
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2151 2020-10-20 18:49:46.000000 tator-0.9.6/tator/transcode/create_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      993 2020-10-20 18:49:46.000000 tator-0.9.6/tator/transcode/delete_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     5676 2021-02-01 17:03:08.000000 tator-0.9.6/tator/transcode/determine_transcode.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2316 2020-10-20 18:49:46.000000 tator-0.9.6/tator/transcode/make_fragment_info.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     4951 2021-02-01 17:02:53.000000 tator-0.9.6/tator/transcode/make_thumbnails.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     3603 2021-02-01 21:37:54.000000 tator-0.9.6/tator/transcode/prepare.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)    14530 2021-02-01 21:37:54.000000 tator-0.9.6/tator/transcode/transcode.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.886551 tator-0.9.6/tator/util/
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1588 2020-12-18 13:07:48.000000 tator-0.9.6/tator/util/__init__.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2012 2021-01-07 02:49:29.000000 tator-0.9.6/tator/util/_download_file.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     3951 2021-01-30 22:01:31.000000 tator-0.9.6/tator/util/_upload_file.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      711 2020-11-21 03:03:20.000000 tator-0.9.6/tator/util/chunked_create.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      955 2020-10-20 18:49:46.000000 tator-0.9.6/tator/util/chunked_file_list.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     4521 2021-01-28 03:45:03.000000 tator-0.9.6/tator/util/clone_leaf_list.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1544 2020-12-03 04:40:52.000000 tator-0.9.6/tator/util/clone_leaf_type.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     7444 2021-02-06 06:04:24.000000 tator-0.9.6/tator/util/clone_localization_list.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2504 2020-12-03 04:40:52.000000 tator-0.9.6/tator/util/clone_localization_type.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)    10818 2021-02-09 02:34:59.000000 tator-0.9.6/tator/util/clone_media_list.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1999 2020-12-13 02:46:15.000000 tator-0.9.6/tator/util/clone_media_type.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2099 2020-12-03 04:40:52.000000 tator-0.9.6/tator/util/clone_membership.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1834 2020-12-03 04:40:52.000000 tator-0.9.6/tator/util/clone_section.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     6495 2021-01-28 03:45:03.000000 tator-0.9.6/tator/util/clone_state_list.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2486 2020-12-03 04:40:52.000000 tator-0.9.6/tator/util/clone_state_type.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2140 2020-12-03 04:40:52.000000 tator-0.9.6/tator/util/clone_version.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     4048 2021-02-11 02:53:26.000000 tator-0.9.6/tator/util/download_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2002 2020-10-20 18:49:46.000000 tator-0.9.6/tator/util/download_temporary_file.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1072 2020-10-20 18:49:46.000000 tator-0.9.6/tator/util/full_state_graphic.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      603 2020-10-20 18:49:46.000000 tator-0.9.6/tator/util/get_api.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2448 2020-11-14 02:49:46.000000 tator-0.9.6/tator/util/get_images.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      464 2020-10-20 18:49:46.000000 tator-0.9.6/tator/util/get_parser.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     4476 2021-02-02 21:53:16.000000 tator-0.9.6/tator/util/import_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1776 2021-01-30 22:01:31.000000 tator-0.9.6/tator/util/md5sum.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     6675 2021-02-09 02:34:59.000000 tator-0.9.6/tator/util/multi_stream.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2266 2021-01-04 02:48:34.000000 tator-0.9.6/tator/util/register_algorithm.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      530 2020-10-20 18:49:46.000000 tator-0.9.6/tator/util/to_dataframe.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2923 2021-01-29 16:56:00.000000 tator-0.9.6/tator/util/upload_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2076 2021-01-04 02:48:34.000000 tator-0.9.6/tator/util/upload_media_archive.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1813 2021-01-04 02:48:34.000000 tator-0.9.6/tator/util/upload_temporary_file.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      160 2020-10-20 18:49:46.000000 tator-0.9.6/tator/version.py
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.870551 tator-0.9.6/tator.egg-info/
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      321 2021-02-11 02:59:37.000000 tator-0.9.6/tator.egg-info/PKG-INFO
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     8294 2021-02-11 02:59:37.000000 tator-0.9.6/tator.egg-info/SOURCES.txt
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)        1 2021-02-11 02:59:37.000000 tator-0.9.6/tator.egg-info/dependency_links.txt
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)       77 2021-02-11 02:59:37.000000 tator-0.9.6/tator.egg-info/requires.txt
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)        6 2021-02-11 02:59:37.000000 tator-0.9.6/tator.egg-info/top_level.txt
-drwxrwxr-x   0 transcoder  (1007) transcoder  (1009)        0 2021-02-11 02:59:37.886551 tator-0.9.6/test/
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)    13714 2021-01-04 02:48:34.000000 tator-0.9.6/test/test_algorithm.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)    11251 2021-01-04 02:48:34.000000 tator-0.9.6/test/test_algorithm_launch.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1835 2020-10-20 18:49:46.000000 tator-0.9.6/test/test_analysis.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     9936 2021-01-21 04:19:28.000000 tator-0.9.6/test/test_attribute_addition.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2772 2021-01-16 03:05:55.000000 tator-0.9.6/test/test_attribute_deletion.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     8105 2021-02-09 02:34:59.000000 tator-0.9.6/test/test_attribute_mutation.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      568 2020-12-03 04:40:52.000000 tator-0.9.6/test/test_clone_leaf_type.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1517 2020-12-03 04:40:52.000000 tator-0.9.6/test/test_clone_localization_type.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     7204 2021-01-04 02:48:34.000000 tator-0.9.6/test/test_clone_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      576 2020-12-03 04:40:52.000000 tator-0.9.6/test/test_clone_media_type.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1209 2021-02-09 02:34:59.000000 tator-0.9.6/test/test_clone_membership.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      797 2020-12-03 04:40:52.000000 tator-0.9.6/test/test_clone_section.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1083 2020-12-03 04:40:52.000000 tator-0.9.6/test/test_clone_state_type.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      797 2020-12-03 04:40:52.000000 tator-0.9.6/test/test_clone_version.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     6098 2021-02-11 02:53:26.000000 tator-0.9.6/test/test_download_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2123 2021-01-30 22:01:31.000000 tator-0.9.6/test/test_extract.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      531 2020-10-20 18:49:46.000000 tator-0.9.6/test/test_getframe.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      928 2021-01-04 02:48:34.000000 tator-0.9.6/test/test_import_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2469 2021-01-04 02:48:34.000000 tator-0.9.6/test/test_job_cancel.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     3093 2021-01-16 03:05:55.000000 tator-0.9.6/test/test_leaf.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1091 2021-01-16 03:05:55.000000 tator-0.9.6/test/test_local_transcode.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     7623 2021-01-26 04:26:59.000000 tator-0.9.6/test/test_localization.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)    17595 2020-10-20 18:49:46.000000 tator-0.9.6/test/test_localization_graphic.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      981 2021-01-12 03:39:30.000000 tator-0.9.6/test/test_media.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      397 2021-01-08 03:01:15.000000 tator-0.9.6/test/test_project_thumbnail.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     7310 2021-01-26 04:26:59.000000 tator-0.9.6/test/test_state.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1580 2021-01-04 02:48:34.000000 tator-0.9.6/test/test_stategraphic.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     1197 2020-10-20 18:49:46.000000 tator-0.9.6/test/test_temporary_file.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     2252 2020-11-21 03:03:20.000000 tator-0.9.6/test/test_transcode.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)     4240 2021-01-04 02:48:34.000000 tator-0.9.6/test/test_upload_archive.py
--rw-rw-r--   0 transcoder  (1007) transcoder  (1009)      912 2020-10-20 18:49:46.000000 tator-0.9.6/test/test_version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.686529 tator-1.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-04-16 17:59:22.000000 tator-1.0.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-04-16 18:09:50.682529 tator-1.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2023-04-16 17:59:22.000000 tator-1.0.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-04-16 17:59:22.000000 tator-1.0.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-16 18:09:50.686529 tator-1.0.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3663 2023-04-16 17:59:22.000000 tator-1.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.646529 tator-1.0.0/tator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-04-16 17:59:22.000000 tator-1.0.0/tator/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.650529 tator-1.0.0/tator/extractor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 17:59:22.000000 tator-1.0.0/tator/extractor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2023-04-16 17:59:22.000000 tator-1.0.0/tator/extractor/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2023-04-16 17:59:22.000000 tator-1.0.0/tator/extractor/env_launcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12295 2023-04-16 17:59:22.000000 tator-1.0.0/tator/extractor/extractor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.650529 tator-1.0.0/tator/openapi/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-04-16 17:59:22.000000 tator-1.0.0/tator/openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.650529 tator-1.0.0/tator/openapi/tator_openapi/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12710 2023-04-16 18:09:48.000000 tator-1.0.0/tator/openapi/tator_openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.650529 tator-1.0.0/tator/openapi/tator_openapi/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-04-16 18:09:48.000000 tator-1.0.0/tator/openapi/tator_openapi/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1846052 2023-04-16 18:09:48.000000 tator-1.0.0/tator/openapi/tator_openapi/api/tator_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2023-04-16 18:09:48.000000 tator-1.0.0/tator/openapi/tator_openapi/api_client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2023-04-16 18:09:48.000000 tator-1.0.0/tator/openapi/tator_openapi/configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-04-16 18:09:48.000000 tator-1.0.0/tator/openapi/tator_openapi/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.670529 tator-1.0.0/tator/openapi/tator_openapi/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12120 2023-04-16 18:09:48.000000 tator-1.0.0/tator/openapi/tator_openapi/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8163 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/affiliation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/affiliation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/affiliation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/algorithm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/algorithm_manifest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/algorithm_parameter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/algorithm_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4152 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/analysis.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/analysis_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/announcement.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/applet.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/applet_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/archive_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10745 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/attribute_filter_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12407 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/attribute_operation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14079 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/audio_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4042 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/autocomplete_service.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bad_request_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bookmark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bookmark_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bookmark_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bucket.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bucket_gcp_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bucket_oci_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bucket_s3_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bucket_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/bucket_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/change_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/change_log_description_of_change.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5302 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/clone_media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/color_map.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/concat_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/create_list_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/create_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/credentials.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/download_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/download_info_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/email_attachment_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/email_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6900 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/encode_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/favorite.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/favorite_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/favorite_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/feed_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/file_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/file_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/file_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/file_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/fill.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/float_array_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/generic_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/generic_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/get_cloned_media_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/image_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/invitation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/invitation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/invitation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/job.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/job_cluster.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/job_cluster_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/job_node.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4849 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/job_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf_suggestion.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-04-16 18:09:46.000000 tator-1.0.0/tator/openapi/tator_openapi/models/leaf_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/live_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/live_update_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9386 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/localization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18245 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_files.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_next.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_prev.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14774 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_stats.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/media_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/membership.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/membership_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/membership_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/message_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/multi_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/not_found_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/notify_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/organization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/organization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/organization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/password_reset_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/project.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/project_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/project_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6157 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/resolution_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/s3_storage_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7613 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/section.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6657 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/section_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/section_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10960 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_merge_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_trim_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/state_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/temporary_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/temporary_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/token.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/transcode.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10545 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/transcode_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/upload_completion_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/upload_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/upload_part.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/user_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7852 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/user_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/version_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/version_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/video_clip.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9722 2023-04-16 18:09:47.000000 tator-1.0.0/tator/openapi/tator_openapi/models/video_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13486 2023-04-16 18:09:48.000000 tator-1.0.0/tator/openapi/tator_openapi/rest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.674529 tator-1.0.0/tator/transcode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6547 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/black.mp4
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/create_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/delete_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8534 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/determine_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/make_fragment_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/make_thumbnails.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/prepare.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16774 2023-04-16 17:59:22.000000 tator-1.0.0/tator/transcode/transcode.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.678529 tator-1.0.0/tator/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/_download_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6959 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/_upload_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/chunked_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/chunked_file_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4470 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_leaf_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7441 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_localization_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11100 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_media_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6560 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_state_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4489 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/concat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/download_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/download_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/find_single_change.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/full_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/get_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/get_images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2219 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/get_paginator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      508 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/get_parser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1729 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/live_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/md5sum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17897 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7283 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/multi_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/register_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/register_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/tator-symbol.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/to_dataframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/update_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/upload_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3315 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/upload_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2023-04-16 17:59:22.000000 tator-1.0.0/tator/util/upload_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-04-16 17:59:22.000000 tator-1.0.0/tator/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.650529 tator-1.0.0/tator.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-04-16 18:09:50.000000 tator-1.0.0/tator.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11773 2023-04-16 18:09:50.000000 tator-1.0.0/tator.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-16 18:09:50.000000 tator-1.0.0/tator.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2023-04-16 18:09:50.000000 tator-1.0.0/tator.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-04-16 18:09:50.000000 tator-1.0.0/tator.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 18:09:50.682529 tator-1.0.0/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4863 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_a_float_array.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_algorithm_launch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_archive_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8615 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_attribute_type_addition.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_attribute_type_deletion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_attribute_type_mutation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_attributes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23749 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_change_log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7204 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_clone_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_collection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12346 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_file_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_get_clip.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_getframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_job_cancel.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_job_cluster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_leaf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_local_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9199 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_localization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_localization_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6973 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_poly.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_project_thumbnail.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9638 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_stategraphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_tracks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5487 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_util_media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_util_media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2023-04-16 17:59:22.000000 tator-1.0.0/test/test_version.py
```

### Comparing `tator-0.9.6/README.md` & `tator-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 python3 setup.py install --user
 ```
 
 ## Example usage
 ```
 import tator
 
-api = tator.get_api('https://www.tatorapp.com', 'MY_TOKEN')
+api = tator.get_api('https://cloud.tator.io', 'MY_TOKEN')
 api.get_media_list(1) # Pass a project ID
 ```
 
 Visit the [examples](examples) for more.
 
 ## API documentation
 
-Documentation for all API functions and models can be found in the [OpenAPI documentation](https://tatorapp.com/docs/tator-py/api.html).
+Documentation for all API functions and models can be found in the [OpenAPI documentation](https://tator.io/api).
 
 ## Authors
 
 Tator and tator-py are developed by [CVision AI](https://www.cvisionai.com).
```

### Comparing `tator-0.9.6/setup.py` & `tator-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from distutils.cmd import Command
 from setuptools import setup, find_packages  # noqa: H301
 from setuptools.command.dist_info import dist_info
 import requests
 import yaml
 import json
 
-REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil",
-            "requests", "pyyaml", "progressbar2"]
+REQUIRES = ["urllib3 >= 1.26", "six >= 1.10", "certifi", "python-dateutil",
+            "requests >= 2.25", "pyyaml", "progressbar2", "pillow"]
 
 SCHEMA_FILENAME = 'schema.yaml'
 CONFIG_FILENAME = 'config.json'
 
 def get_version():
     with open(CONFIG_FILENAME, 'r') as f:
         config = json.load(f)
@@ -32,40 +32,40 @@
     return data
 
 class NoAliasDumper(yaml.Dumper):
     def ignore_aliases(self, data):
         return True
 
 def codegen():
-    """ Fetches a schema from tatorapp.com if one does not exist, then 
+    """ Fetches a schema from cloud.tator.io if one does not exist, then 
         use openapi-generator to generate openapi code from it.
     """
     # Retrieve schema if it does not exist.
     if not os.path.exists(SCHEMA_FILENAME):
-        response = requests.get("https://www.tatorapp.com/schema")
+        response = requests.get("https://cloud.tator.io/schema")
         assert response.status_code == 200
         with open(SCHEMA_FILENAME, 'wb') as f:
             f.write(response.content)
 
     # Remove any oneOf entries from the schema, as they are not handled
     # well by openapi generator.
     with open(SCHEMA_FILENAME, 'r') as f:
-        schema = yaml.load(f)
+        schema = yaml.safe_load(f)
     schema = remove_oneof(schema)
     with open(SCHEMA_FILENAME, 'w') as f:
         yaml.dump(schema, f, Dumper=NoAliasDumper)
 
     # Get the git SHA ID.
     cmd = ['git', 'rev-parse', 'HEAD']
     git_rev = subprocess.check_output(cmd).strip().decode('utf-8')
 
     # Generate code using openapi generator docker image.
     pwd = os.path.dirname(os.path.abspath(__file__))
     cmd = [
-        'docker', 'run', '-it', '--rm',
+        'docker', 'run', '--rm',
         '-v', f"{pwd}:/pwd",
         '-v', f"{pwd}/out:/out",
         'openapitools/openapi-generator-cli:v4.3.1', 'generate',
         '-c', f'/pwd/{CONFIG_FILENAME}',
         '-i', f'/pwd/{SCHEMA_FILENAME}',
         '-g', 'python',
         '-o', f'/out/tator-py-{git_rev}',
@@ -88,15 +88,15 @@
             if os.path.exists(dst):
                 shutil.rmtree(dst)
             shutil.copytree(src, dst)
     pwd = os.path.dirname(os.path.abspath(__file__))
 
     # need to delete from within docker
     cmd = [
-        'docker', 'run', '-it', '--rm',
+        'docker', 'run', '--rm',
         '-v', f"{pwd}/out:/out",
          'openapitools/openapi-generator-cli:v4.3.1',
         'rm', '-fr',
         '/out/*'
     ]
     subprocess.run(cmd, check=True)
```

### Comparing `tator-0.9.6/tator/__init__.py` & `tator-1.0.0/tator/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/extractor/__main__.py` & `tator-1.0.0/tator/extractor/__main__.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/extractor/env_launcher.py` & `tator-1.0.0/tator/extractor/env_launcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """ Uses ENV variables to dispatch the frame extractor 
 
 Generic TATOR workflow env variables this module expects:
 
-TATOR_API_SERVICE : URL to host, e.g. https://www.tatorapp.com
+TATOR_API_SERVICE : URL to host, e.g. https://cloud.tator.io
 TATOR_AUTH_TOKEN : Token to use for authentication
 TATOR_PROJECT_ID : numerical id of the project this algorithm is being run
 TATOR_MEDIA_IDS : Comma-seperated list of media ids to process
 
 :Workflow variables:
 `python3 -m tator.extractor --help` for more information on the following
 options:
```

### Comparing `tator-0.9.6/tator/extractor/extractor.py` & `tator-1.0.0/tator/extractor/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,25 @@
                  path,
                  fname,
                  section,
                  upload_gid,
                  work_dir):
 
     md5sum = tator.util.md5sum(path)
-    response = api.create_media(project,
-                                {'type': media_type_id,
-                                 'section': section,
-                                 'name': fname,
-                                 'md5': md5sum,
-                                 'gid': upload_gid,
-                                 'uid': str(uuid.uuid1())})
+    media_spec = [
+        {
+            "type": media_type_id,
+            "section": section,
+            "name": fname,
+            "md5": md5sum,
+            "gid": upload_gid,
+            "uid": str(uuid.uuid1()),
+        },
+    ]
+    response = api.create_media_list(project, media_spec)
     assert isinstance(response, CreateResponse)
     media_id = response.id
 
     # Peel apart api to get host/token combo (TODO: not great)
     host = api.api_client.configuration.host
     token = api.api_client.configuration.api_key['Authorization']
     with tempfile.TemporaryDirectory(dir=work_dir) as td:
@@ -119,15 +123,15 @@
     :param upload_gid: str representation of a unique task id (optional)
     """
     grouped_by_frame = defaultdict(lambda: [])
     if mode == "track_thumbnail":
 
         # First get the localization_type id
         random_local = api.get_localization(metadata[0].localizations[0])
-        localization_type = random_local.meta
+        localization_type = random_local.type
         localizations = api.get_localization_list(project,
                                                   media_id=[media_el.id],
                                                   type=localization_type)
         localizations = [x.to_dict() for x in localizations]
         for l in localizations:
             found = False
             for entry in metadata:
@@ -247,15 +251,15 @@
                     media_id = resp.id
                     frame_str = os.path.splitext(fp.split('_')[-1])[0]
                     frame = int(frame_str)
                     new_meta=[]
                     for metadata in grouped_by_frame[frame]:
                         new_obj = {
                             'frame': 0,
-                            'type': metadata['meta'],
+                            'type': metadata['type'],
                             **metadata['attributes']
                         }
                         if mode == 'state':
                             new_obj.update({'media_ids':[media_id]})
                         else:
                             new_obj.update({'media_id':media_id,
                                             'x': metadata['x'],
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/__init__.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,122 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Tator REST API
 
     Interface to the Tator backend.  # noqa: E501
 
     The version of the OpenAPI document: v1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.9.6"
-
-# import apis into sdk package
-from tator.openapi.tator_openapi.api.tator_api import TatorApi
-
-# import ApiClient
-from tator.openapi.tator_openapi.api_client import ApiClient
-from tator.openapi.tator_openapi.configuration import Configuration
-from tator.openapi.tator_openapi.exceptions import OpenApiException
-from tator.openapi.tator_openapi.exceptions import ApiTypeError
-from tator.openapi.tator_openapi.exceptions import ApiValueError
-from tator.openapi.tator_openapi.exceptions import ApiKeyError
-from tator.openapi.tator_openapi.exceptions import ApiException
-# import models into sdk package
+# import models into model package
 from tator.openapi.tator_openapi.models.affiliation import Affiliation
 from tator.openapi.tator_openapi.models.affiliation_spec import AffiliationSpec
 from tator.openapi.tator_openapi.models.affiliation_update import AffiliationUpdate
 from tator.openapi.tator_openapi.models.algorithm import Algorithm
-from tator.openapi.tator_openapi.models.algorithm_launch import AlgorithmLaunch
-from tator.openapi.tator_openapi.models.algorithm_launch_spec import AlgorithmLaunchSpec
 from tator.openapi.tator_openapi.models.algorithm_manifest import AlgorithmManifest
 from tator.openapi.tator_openapi.models.algorithm_manifest_spec import AlgorithmManifestSpec
 from tator.openapi.tator_openapi.models.algorithm_parameter import AlgorithmParameter
 from tator.openapi.tator_openapi.models.algorithm_spec import AlgorithmSpec
 from tator.openapi.tator_openapi.models.analysis import Analysis
 from tator.openapi.tator_openapi.models.analysis_spec import AnalysisSpec
+from tator.openapi.tator_openapi.models.announcement import Announcement
+from tator.openapi.tator_openapi.models.applet import Applet
+from tator.openapi.tator_openapi.models.applet_spec import AppletSpec
 from tator.openapi.tator_openapi.models.archive_config import ArchiveConfig
-from tator.openapi.tator_openapi.models.attribute_bulk_update import AttributeBulkUpdate
+from tator.openapi.tator_openapi.models.attribute_combinator_spec import AttributeCombinatorSpec
+from tator.openapi.tator_openapi.models.attribute_filter_spec import AttributeFilterSpec
+from tator.openapi.tator_openapi.models.attribute_operation_spec import AttributeOperationSpec
 from tator.openapi.tator_openapi.models.attribute_type import AttributeType
 from tator.openapi.tator_openapi.models.attribute_type_delete import AttributeTypeDelete
 from tator.openapi.tator_openapi.models.attribute_type_spec import AttributeTypeSpec
 from tator.openapi.tator_openapi.models.attribute_type_update import AttributeTypeUpdate
-from tator.openapi.tator_openapi.models.attribute_type_update_new_attribute_type import AttributeTypeUpdateNewAttributeType
+from tator.openapi.tator_openapi.models.attribute_type_update_attribute_type_update import AttributeTypeUpdateAttributeTypeUpdate
 from tator.openapi.tator_openapi.models.audio_definition import AudioDefinition
 from tator.openapi.tator_openapi.models.autocomplete_service import AutocompleteService
+from tator.openapi.tator_openapi.models.auxiliary_file_definition import AuxiliaryFileDefinition
 from tator.openapi.tator_openapi.models.bad_request_response import BadRequestResponse
 from tator.openapi.tator_openapi.models.bookmark import Bookmark
 from tator.openapi.tator_openapi.models.bookmark_spec import BookmarkSpec
 from tator.openapi.tator_openapi.models.bookmark_update import BookmarkUpdate
+from tator.openapi.tator_openapi.models.bucket import Bucket
+from tator.openapi.tator_openapi.models.bucket_gcp_config import BucketGCPConfig
+from tator.openapi.tator_openapi.models.bucket_oci_config import BucketOCIConfig
+from tator.openapi.tator_openapi.models.bucket_oci_native_config import BucketOCINativeConfig
+from tator.openapi.tator_openapi.models.bucket_s3_config import BucketS3Config
+from tator.openapi.tator_openapi.models.bucket_spec import BucketSpec
+from tator.openapi.tator_openapi.models.bucket_update import BucketUpdate
+from tator.openapi.tator_openapi.models.change_log import ChangeLog
+from tator.openapi.tator_openapi.models.change_log_description_of_change import ChangeLogDescriptionOfChange
+from tator.openapi.tator_openapi.models.change_log_description_of_change_new import ChangeLogDescriptionOfChangeNew
 from tator.openapi.tator_openapi.models.clone_media_spec import CloneMediaSpec
 from tator.openapi.tator_openapi.models.color_map import ColorMap
+from tator.openapi.tator_openapi.models.concat_definition import ConcatDefinition
 from tator.openapi.tator_openapi.models.create_list_response import CreateListResponse
 from tator.openapi.tator_openapi.models.create_response import CreateResponse
 from tator.openapi.tator_openapi.models.credentials import Credentials
 from tator.openapi.tator_openapi.models.download_info import DownloadInfo
 from tator.openapi.tator_openapi.models.download_info_spec import DownloadInfoSpec
 from tator.openapi.tator_openapi.models.email_attachment_spec import EmailAttachmentSpec
 from tator.openapi.tator_openapi.models.email_spec import EmailSpec
 from tator.openapi.tator_openapi.models.encode_config import EncodeConfig
 from tator.openapi.tator_openapi.models.favorite import Favorite
 from tator.openapi.tator_openapi.models.favorite_spec import FavoriteSpec
 from tator.openapi.tator_openapi.models.favorite_update import FavoriteUpdate
+from tator.openapi.tator_openapi.models.feed_definition import FeedDefinition
+from tator.openapi.tator_openapi.models.file import File
+from tator.openapi.tator_openapi.models.file_spec import FileSpec
+from tator.openapi.tator_openapi.models.file_type import FileType
+from tator.openapi.tator_openapi.models.file_type_spec import FileTypeSpec
+from tator.openapi.tator_openapi.models.file_type_update import FileTypeUpdate
+from tator.openapi.tator_openapi.models.file_update import FileUpdate
 from tator.openapi.tator_openapi.models.fill import Fill
+from tator.openapi.tator_openapi.models.float_array_query import FloatArrayQuery
+from tator.openapi.tator_openapi.models.generic_file import GenericFile
+from tator.openapi.tator_openapi.models.generic_file_spec import GenericFileSpec
+from tator.openapi.tator_openapi.models.get_cloned_media_response import GetClonedMediaResponse
 from tator.openapi.tator_openapi.models.image_definition import ImageDefinition
+from tator.openapi.tator_openapi.models.invitation import Invitation
+from tator.openapi.tator_openapi.models.invitation_spec import InvitationSpec
+from tator.openapi.tator_openapi.models.invitation_update import InvitationUpdate
 from tator.openapi.tator_openapi.models.job import Job
+from tator.openapi.tator_openapi.models.job_cluster import JobCluster
+from tator.openapi.tator_openapi.models.job_cluster_spec import JobClusterSpec
 from tator.openapi.tator_openapi.models.job_node import JobNode
+from tator.openapi.tator_openapi.models.job_spec import JobSpec
 from tator.openapi.tator_openapi.models.leaf import Leaf
+from tator.openapi.tator_openapi.models.leaf_bulk_update import LeafBulkUpdate
+from tator.openapi.tator_openapi.models.leaf_id_query import LeafIdQuery
 from tator.openapi.tator_openapi.models.leaf_spec import LeafSpec
 from tator.openapi.tator_openapi.models.leaf_suggestion import LeafSuggestion
 from tator.openapi.tator_openapi.models.leaf_type import LeafType
 from tator.openapi.tator_openapi.models.leaf_type_spec import LeafTypeSpec
 from tator.openapi.tator_openapi.models.leaf_type_update import LeafTypeUpdate
 from tator.openapi.tator_openapi.models.leaf_update import LeafUpdate
+from tator.openapi.tator_openapi.models.live_definition import LiveDefinition
+from tator.openapi.tator_openapi.models.live_update_definition import LiveUpdateDefinition
 from tator.openapi.tator_openapi.models.localization import Localization
+from tator.openapi.tator_openapi.models.localization_bulk_delete import LocalizationBulkDelete
+from tator.openapi.tator_openapi.models.localization_bulk_update import LocalizationBulkUpdate
+from tator.openapi.tator_openapi.models.localization_delete import LocalizationDelete
+from tator.openapi.tator_openapi.models.localization_id_query import LocalizationIdQuery
 from tator.openapi.tator_openapi.models.localization_spec import LocalizationSpec
 from tator.openapi.tator_openapi.models.localization_type import LocalizationType
 from tator.openapi.tator_openapi.models.localization_type_spec import LocalizationTypeSpec
 from tator.openapi.tator_openapi.models.localization_type_update import LocalizationTypeUpdate
 from tator.openapi.tator_openapi.models.localization_update import LocalizationUpdate
 from tator.openapi.tator_openapi.models.media import Media
+from tator.openapi.tator_openapi.models.media_bulk_update import MediaBulkUpdate
 from tator.openapi.tator_openapi.models.media_files import MediaFiles
+from tator.openapi.tator_openapi.models.media_id_query import MediaIdQuery
 from tator.openapi.tator_openapi.models.media_next import MediaNext
 from tator.openapi.tator_openapi.models.media_prev import MediaPrev
 from tator.openapi.tator_openapi.models.media_spec import MediaSpec
 from tator.openapi.tator_openapi.models.media_stats import MediaStats
 from tator.openapi.tator_openapi.models.media_type import MediaType
 from tator.openapi.tator_openapi.models.media_type_spec import MediaTypeSpec
 from tator.openapi.tator_openapi.models.media_type_update import MediaTypeUpdate
@@ -98,23 +126,29 @@
 from tator.openapi.tator_openapi.models.membership_update import MembershipUpdate
 from tator.openapi.tator_openapi.models.message_response import MessageResponse
 from tator.openapi.tator_openapi.models.multi_definition import MultiDefinition
 from tator.openapi.tator_openapi.models.not_found_response import NotFoundResponse
 from tator.openapi.tator_openapi.models.notify_spec import NotifySpec
 from tator.openapi.tator_openapi.models.organization import Organization
 from tator.openapi.tator_openapi.models.organization_spec import OrganizationSpec
+from tator.openapi.tator_openapi.models.organization_update import OrganizationUpdate
+from tator.openapi.tator_openapi.models.password_reset_spec import PasswordResetSpec
 from tator.openapi.tator_openapi.models.project import Project
 from tator.openapi.tator_openapi.models.project_spec import ProjectSpec
 from tator.openapi.tator_openapi.models.project_update import ProjectUpdate
 from tator.openapi.tator_openapi.models.resolution_config import ResolutionConfig
 from tator.openapi.tator_openapi.models.s3_storage_config import S3StorageConfig
 from tator.openapi.tator_openapi.models.section import Section
 from tator.openapi.tator_openapi.models.section_spec import SectionSpec
 from tator.openapi.tator_openapi.models.section_update import SectionUpdate
 from tator.openapi.tator_openapi.models.state import State
+from tator.openapi.tator_openapi.models.state_bulk_delete import StateBulkDelete
+from tator.openapi.tator_openapi.models.state_bulk_update import StateBulkUpdate
+from tator.openapi.tator_openapi.models.state_delete import StateDelete
+from tator.openapi.tator_openapi.models.state_id_query import StateIdQuery
 from tator.openapi.tator_openapi.models.state_merge_update import StateMergeUpdate
 from tator.openapi.tator_openapi.models.state_spec import StateSpec
 from tator.openapi.tator_openapi.models.state_trim_update import StateTrimUpdate
 from tator.openapi.tator_openapi.models.state_type import StateType
 from tator.openapi.tator_openapi.models.state_type_spec import StateTypeSpec
 from tator.openapi.tator_openapi.models.state_type_update import StateTypeUpdate
 from tator.openapi.tator_openapi.models.state_update import StateUpdate
@@ -123,14 +157,14 @@
 from tator.openapi.tator_openapi.models.token import Token
 from tator.openapi.tator_openapi.models.transcode import Transcode
 from tator.openapi.tator_openapi.models.transcode_spec import TranscodeSpec
 from tator.openapi.tator_openapi.models.upload_completion_spec import UploadCompletionSpec
 from tator.openapi.tator_openapi.models.upload_info import UploadInfo
 from tator.openapi.tator_openapi.models.upload_part import UploadPart
 from tator.openapi.tator_openapi.models.user import User
+from tator.openapi.tator_openapi.models.user_spec import UserSpec
 from tator.openapi.tator_openapi.models.user_update import UserUpdate
 from tator.openapi.tator_openapi.models.version import Version
 from tator.openapi.tator_openapi.models.version_spec import VersionSpec
 from tator.openapi.tator_openapi.models.version_update import VersionUpdate
 from tator.openapi.tator_openapi.models.video_clip import VideoClip
 from tator.openapi.tator_openapi.models.video_definition import VideoDefinition
-
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/api_client.py` & `tator-1.0.0/tator/openapi/tator_openapi/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.9.6/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -119,15 +119,15 @@
         self.default_headers[header_name] = header_value
 
     def __call_api(
             self, resource_path, method, path_params=None,
             query_params=None, header_params=None, body=None, post_params=None,
             files=None, response_type=None, auth_settings=None,
             _return_http_data_only=None, collection_formats=None,
-            _preload_content=True, _request_timeout=None, _host=None):
+            _preload_content=True, _request_timeout=300, _host=None):
 
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
@@ -320,15 +320,15 @@
             return self.__deserialize_model(data, klass)
 
     def call_api(self, resource_path, method,
                  path_params=None, query_params=None, header_params=None,
                  body=None, post_params=None, files=None,
                  response_type=None, auth_settings=None, async_req=None,
                  _return_http_data_only=None, collection_formats=None,
-                 _preload_content=True, _request_timeout=None, _host=None):
+                 _preload_content=True, _request_timeout=300, _host=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
@@ -338,26 +338,26 @@
         :param body: Request body.
         :param post_params dict: Request post form parameters,
             for `application/x-www-form-urlencoded`, `multipart/form-data`.
         :param auth_settings list: Auth Settings names for the request.
         :param response: Response data type.
         :param files dict: key -> filename, value -> filepath,
             for `multipart/form-data`.
-        :param async_req bool: execute request asynchronously
+        :param bool async_req: execute request asynchronously
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param collection_formats: dict of collection formats for path, query,
             header, and post parameters.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
+                                 (connection, read) timeouts. Default is 300.
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
         """
@@ -380,15 +380,15 @@
                                                        collection_formats,
                                                        _preload_content,
                                                        _request_timeout,
                                                        _host))
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
-                _request_timeout=None):
+                _request_timeout=300):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
             return self.rest_client.GET(url,
                                         query_params=query_params,
                                         _preload_content=_preload_content,
                                         _request_timeout=_request_timeout,
                                         headers=headers)
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/configuration.py` & `tator-1.0.0/tator/openapi/tator_openapi/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     The following cookie will be added to the HTTP request:
        Cookie: JSESSIONID abc123
     """
 
     _default = None
 
-    def __init__(self, host="http://localhost",
+    def __init__(self, host="http://None",
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
                  discard_unknown_keys=False,
                  ):
         """Constructor
         """
         self.host = host
@@ -330,14 +330,21 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
+        if 'X-CSRFToken' in self.api_key:
+            auth['SessionAuth'] = {
+                'type': 'api_key',
+                'in': 'header',
+                'key': 'X-CSRFToken',
+                'value': self.get_api_key_with_prefix('X-CSRFToken')
+            }
         if 'Authorization' in self.api_key:
             auth['TokenAuth'] = {
                 'type': 'api_key',
                 'in': 'header',
                 'key': 'Authorization',
                 'value': self.get_api_key_with_prefix('Authorization')
             }
@@ -348,25 +355,25 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 0.9.6".\
+               "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "/",
+                'url': "http://None",
                 'description': "No description provided",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/exceptions.py` & `tator-1.0.0/tator/openapi/tator_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/affiliation.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/organization_spec.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,155 +14,124 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Affiliation(object):
+class OrganizationSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'int',
-        'organization': 'int',
-        'permission': 'str',
-        'user': 'int'
+        'default_membership_permission': 'str',
+        'name': 'str',
+        'thumb': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
-        'organization': 'organization',
-        'permission': 'permission',
-        'user': 'user'
+        'default_membership_permission': 'default_membership_permission',
+        'name': 'name',
+        'thumb': 'thumb'
     }
 
-    def __init__(self, id=None, organization=None, permission=None, user=None, local_vars_configuration=None):  # noqa: E501
-        """Affiliation - a model defined in OpenAPI"""
+    def __init__(self, default_membership_permission=None, name=None, thumb=None, local_vars_configuration=None):  # noqa: E501
+        """OrganizationSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._organization = None
-        self._permission = None
-        self._user = None
+        self._default_membership_permission = None
+        self._name = None
+        self._thumb = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
-        if organization is not None:
-            self.organization = organization
-        if permission is not None:
-            self.permission = permission
-        if user is not None:
-            self.user = user
+        if default_membership_permission is not None:
+            self.default_membership_permission = default_membership_permission
+        self.name = name
+        if thumb is not None:
+            self.thumb = thumb
 
     @property
-    def id(self):
+    def default_membership_permission(self):
         """
-        Unique integer identifying a affiliation.
+        Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
 
-        :return: The id of this Affiliation. 
-        :rtype: int
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """
-        Unique integer identifying a affiliation.
-
-        :param id: The id of this Affiliation.
-        :type: int
-        """
-
-        self._id = id
-
-    @property
-    def organization(self):
-        """
-        Unique integer identifying an organization.
-
-        :return: The organization of this Affiliation. 
-        :rtype: int
+        :return: The default_membership_permission of this OrganizationSpec. 
+        :rtype: str
         """
-        return self._organization
+        return self._default_membership_permission
 
-    @organization.setter
-    def organization(self, organization):
+    @default_membership_permission.setter
+    def default_membership_permission(self, default_membership_permission):
         """
-        Unique integer identifying an organization.
+        Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
 
-        :param organization: The organization of this Affiliation.
-        :type: int
+        :param default_membership_permission: The default_membership_permission of this OrganizationSpec.
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                organization is not None and organization < 1):  # noqa: E501
-            raise ValueError("Invalid value for `organization`, must be a value greater than or equal to `1`")  # noqa: E501
+        allowed_values = ["No Access", "View Only", "Can Edit", "Can Transfer", "Can Execute", "Full Control"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and default_membership_permission not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `default_membership_permission` ({0}), must be one of {1}"  # noqa: E501
+                .format(default_membership_permission, allowed_values)
+            )
 
-        self._organization = organization
+        self._default_membership_permission = default_membership_permission
 
     @property
-    def permission(self):
+    def name(self):
         """
-        User permission level for the organization.
+        Name of the organization.
 
-        :return: The permission of this Affiliation. 
+        :return: The name of this OrganizationSpec. 
         :rtype: str
         """
-        return self._permission
+        return self._name
 
-    @permission.setter
-    def permission(self, permission):
+    @name.setter
+    def name(self, name):
         """
-        User permission level for the organization.
+        Name of the organization.
 
-        :param permission: The permission of this Affiliation.
+        :param name: The name of this OrganizationSpec.
         :type: str
         """
-        allowed_values = ["Member", "Admin"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and permission not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `permission` ({0}), must be one of {1}"  # noqa: E501
-                .format(permission, allowed_values)
-            )
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._permission = permission
+        self._name = name
 
     @property
-    def user(self):
+    def thumb(self):
         """
-        Unique integer identifying a user.
+        S3 key of thumbnail used to represent the organization.
 
-        :return: The user of this Affiliation. 
-        :rtype: int
+        :return: The thumb of this OrganizationSpec. 
+        :rtype: str
         """
-        return self._user
+        return self._thumb
 
-    @user.setter
-    def user(self, user):
+    @thumb.setter
+    def thumb(self, thumb):
         """
-        Unique integer identifying a user.
+        S3 key of thumbnail used to represent the organization.
 
-        :param user: The user of this Affiliation.
-        :type: int
+        :param thumb: The thumb of this OrganizationSpec.
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                user is not None and user < 1):  # noqa: E501
-            raise ValueError("Invalid value for `user`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._user = user
+        self._thumb = thumb
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -190,18 +159,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Affiliation):
+        if not isinstance(other, OrganizationSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Affiliation):
+        if not isinstance(other, OrganizationSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/affiliation_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/affiliation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/affiliation_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/affiliation_update.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/algorithm.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/job.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,243 +14,265 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Algorithm(object):
+class Job(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'cluster': 'int',
-        'description': 'str',
-        'files_per_job': 'int',
-        'id': 'int',
-        'manifest': 'str',
-        'name': 'str',
+        'gid': 'str',
+        'id': 'str',
+        'nodes': 'list[JobNode]',
         'project': 'int',
+        'start_time': 'datetime',
+        'status': 'str',
+        'stop_time': 'datetime',
+        'uid': 'str',
         'user': 'int'
     }
 
     attribute_map = {
-        'cluster': 'cluster',
-        'description': 'description',
-        'files_per_job': 'files_per_job',
+        'gid': 'gid',
         'id': 'id',
-        'manifest': 'manifest',
-        'name': 'name',
+        'nodes': 'nodes',
         'project': 'project',
+        'start_time': 'start_time',
+        'status': 'status',
+        'stop_time': 'stop_time',
+        'uid': 'uid',
         'user': 'user'
     }
 
-    def __init__(self, cluster=None, description=None, files_per_job=None, id=None, manifest=None, name=None, project=None, user=None, local_vars_configuration=None):  # noqa: E501
-        """Algorithm - a model defined in OpenAPI"""
+    def __init__(self, gid=None, id=None, nodes=None, project=None, start_time=None, status=None, stop_time=None, uid=None, user=None, local_vars_configuration=None):  # noqa: E501
+        """Job - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._cluster = None
-        self._description = None
-        self._files_per_job = None
+        self._gid = None
         self._id = None
-        self._manifest = None
-        self._name = None
+        self._nodes = None
         self._project = None
+        self._start_time = None
+        self._status = None
+        self._stop_time = None
+        self._uid = None
         self._user = None
         self.discriminator = None
 
-        if cluster is not None:
-            self.cluster = cluster
-        if description is not None:
-            self.description = description
-        if files_per_job is not None:
-            self.files_per_job = files_per_job
+        if gid is not None:
+            self.gid = gid
         if id is not None:
             self.id = id
-        if manifest is not None:
-            self.manifest = manifest
-        if name is not None:
-            self.name = name
+        if nodes is not None:
+            self.nodes = nodes
         if project is not None:
             self.project = project
+        self.start_time = start_time
+        if status is not None:
+            self.status = status
+        self.stop_time = stop_time
+        if uid is not None:
+            self.uid = uid
         if user is not None:
             self.user = user
 
     @property
-    def cluster(self):
+    def gid(self):
         """
-        Unique integer identifying the job cluster.
+        Group ID of the job.
 
-        :return: The cluster of this Algorithm. 
-        :rtype: int
+        :return: The gid of this Job. 
+        :rtype: str
         """
-        return self._cluster
+        return self._gid
 
-    @cluster.setter
-    def cluster(self, cluster):
+    @gid.setter
+    def gid(self, gid):
         """
-        Unique integer identifying the job cluster.
+        Group ID of the job.
 
-        :param cluster: The cluster of this Algorithm.
-        :type: int
+        :param gid: The gid of this Job.
+        :type: str
         """
 
-        self._cluster = cluster
+        self._gid = gid
 
     @property
-    def description(self):
+    def id(self):
         """
-        Description of the algorithm.
+        Unique identifier of the job generated by Argo.
 
-        :return: The description of this Algorithm. 
+        :return: The id of this Job. 
         :rtype: str
         """
-        return self._description
+        return self._id
 
-    @description.setter
-    def description(self, description):
+    @id.setter
+    def id(self, id):
         """
-        Description of the algorithm.
+        Unique identifier of the job generated by Argo.
 
-        :param description: The description of this Algorithm.
+        :param id: The id of this Job.
         :type: str
         """
 
-        self._description = description
+        self._id = id
 
     @property
-    def files_per_job(self):
+    def nodes(self):
         """
-        Number of media files to be submitted to each workflow.
 
-        :return: The files_per_job of this Algorithm. 
-        :rtype: int
+        :return: The nodes of this Job. 
+        :rtype: list[JobNode]
         """
-        return self._files_per_job
+        return self._nodes
 
-    @files_per_job.setter
-    def files_per_job(self, files_per_job):
+    @nodes.setter
+    def nodes(self, nodes):
         """
-        Number of media files to be submitted to each workflow.
 
-        :param files_per_job: The files_per_job of this Algorithm.
-        :type: int
+        :param nodes: The nodes of this Job.
+        :type: list[JobNode]
         """
 
-        self._files_per_job = files_per_job
+        self._nodes = nodes
 
     @property
-    def id(self):
+    def project(self):
         """
-        Unique integer identifying the registered algorithm.
+        Unique integer identifying a project.
 
-        :return: The id of this Algorithm. 
+        :return: The project of this Job. 
         :rtype: int
         """
-        return self._id
+        return self._project
 
-    @id.setter
-    def id(self, id):
+    @project.setter
+    def project(self, project):
         """
-        Unique integer identifying the registered algorithm.
+        Unique integer identifying a project.
 
-        :param id: The id of this Algorithm.
+        :param project: The project of this Job.
         :type: int
         """
 
-        self._id = id
+        self._project = project
 
     @property
-    def manifest(self):
+    def start_time(self):
         """
-        Server URL to argo manifest file (.yaml)
+        Start time of this job.
 
-        :return: The manifest of this Algorithm. 
-        :rtype: str
+        :return: The start_time of this Job. 
+        :rtype: datetime
         """
-        return self._manifest
+        return self._start_time
 
-    @manifest.setter
-    def manifest(self, manifest):
+    @start_time.setter
+    def start_time(self, start_time):
         """
-        Server URL to argo manifest file (.yaml)
+        Start time of this job.
 
-        :param manifest: The manifest of this Algorithm.
-        :type: str
+        :param start_time: The start_time of this Job.
+        :type: datetime
         """
 
-        self._manifest = manifest
+        self._start_time = start_time
 
     @property
-    def name(self):
+    def status(self):
         """
-        Unique name of the algorithm workflow.
+        Status of this job.
 
-        :return: The name of this Algorithm. 
+        :return: The status of this Job. 
         :rtype: str
         """
-        return self._name
+        return self._status
 
-    @name.setter
-    def name(self, name):
+    @status.setter
+    def status(self, status):
         """
-        Unique name of the algorithm workflow.
+        Status of this job.
 
-        :param name: The name of this Algorithm.
+        :param status: The status of this Job.
         :type: str
         """
 
-        self._name = name
+        self._status = status
 
     @property
-    def project(self):
+    def stop_time(self):
         """
-        Unique integer identifying the project associated with the algorithm.
+        Stop time of this job.
 
-        :return: The project of this Algorithm. 
-        :rtype: int
+        :return: The stop_time of this Job. 
+        :rtype: datetime
         """
-        return self._project
+        return self._stop_time
 
-    @project.setter
-    def project(self, project):
+    @stop_time.setter
+    def stop_time(self, stop_time):
         """
-        Unique integer identifying the project associated with the algorithm.
+        Stop time of this job.
 
-        :param project: The project of this Algorithm.
-        :type: int
+        :param stop_time: The stop_time of this Job.
+        :type: datetime
         """
 
-        self._project = project
+        self._stop_time = stop_time
+
+    @property
+    def uid(self):
+        """
+        Unique ID of the job.
+
+        :return: The uid of this Job. 
+        :rtype: str
+        """
+        return self._uid
+
+    @uid.setter
+    def uid(self, uid):
+        """
+        Unique ID of the job.
+
+        :param uid: The uid of this Job.
+        :type: str
+        """
+
+        self._uid = uid
 
     @property
     def user(self):
         """
-        Unique integer identifying the user registering the algorithm.
+        Unique integer identifying user who submitted the job.
 
-        :return: The user of this Algorithm. 
+        :return: The user of this Job. 
         :rtype: int
         """
         return self._user
 
     @user.setter
     def user(self, user):
         """
-        Unique integer identifying the user registering the algorithm.
+        Unique integer identifying user who submitted the job.
 
-        :param user: The user of this Algorithm.
+        :param user: The user of this Job.
         :type: int
         """
 
         self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -282,18 +304,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Algorithm):
+        if not isinstance(other, Job):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Algorithm):
+        if not isinstance(other, Job):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_launch.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/upload_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,117 +14,117 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class AlgorithmLaunch(object):
+class UploadInfo(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'gid': 'str',
-        'message': 'str',
-        'uid': 'list[str]'
+        'key': 'str',
+        'upload_id': 'str',
+        'urls': 'list[str]'
     }
 
     attribute_map = {
-        'gid': 'gid',
-        'message': 'message',
-        'uid': 'uid'
+        'key': 'key',
+        'upload_id': 'upload_id',
+        'urls': 'urls'
     }
 
-    def __init__(self, gid=None, message=None, uid=None, local_vars_configuration=None):  # noqa: E501
-        """AlgorithmLaunch - a model defined in OpenAPI"""
+    def __init__(self, key=None, upload_id=None, urls=None, local_vars_configuration=None):  # noqa: E501
+        """UploadInfo - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._gid = None
-        self._message = None
-        self._uid = None
+        self._key = None
+        self._upload_id = None
+        self._urls = None
         self.discriminator = None
 
-        if gid is not None:
-            self.gid = gid
-        if message is not None:
-            self.message = message
-        if uid is not None:
-            self.uid = uid
+        if key is not None:
+            self.key = key
+        if upload_id is not None:
+            self.upload_id = upload_id
+        if urls is not None:
+            self.urls = urls
 
     @property
-    def gid(self):
+    def key(self):
         """
-        A uuid string identifying the group of jobs started.
+        An object key that can be supplied to the `Transcode` or `Media` or `File` endpoint after the file has been uploaded.
 
-        :return: The gid of this AlgorithmLaunch. 
+        :return: The key of this UploadInfo. 
         :rtype: str
         """
-        return self._gid
+        return self._key
 
-    @gid.setter
-    def gid(self, gid):
+    @key.setter
+    def key(self, key):
         """
-        A uuid string identifying the group of jobs started.
+        An object key that can be supplied to the `Transcode` or `Media` or `File` endpoint after the file has been uploaded.
 
-        :param gid: The gid of this AlgorithmLaunch.
+        :param key: The key of this UploadInfo.
         :type: str
         """
 
-        self._gid = gid
+        self._key = key
 
     @property
-    def message(self):
+    def upload_id(self):
         """
-        Message indicating successful launch.
+        An upload ID that can be supplied to the `UploadCompletion` endpoint after the file has been uploaded. Only contains a value if `num_parts` > 1.
 
-        :return: The message of this AlgorithmLaunch. 
+        :return: The upload_id of this UploadInfo. 
         :rtype: str
         """
-        return self._message
+        return self._upload_id
 
-    @message.setter
-    def message(self, message):
+    @upload_id.setter
+    def upload_id(self, upload_id):
         """
-        Message indicating successful launch.
+        An upload ID that can be supplied to the `UploadCompletion` endpoint after the file has been uploaded. Only contains a value if `num_parts` > 1.
 
-        :param message: The message of this AlgorithmLaunch.
+        :param upload_id: The upload_id of this UploadInfo.
         :type: str
         """
 
-        self._message = message
+        self._upload_id = upload_id
 
     @property
-    def uid(self):
+    def urls(self):
         """
-        A list of uuid strings identifying each job started.
+        One or more URLs for upload via one PUT request per URL.
 
-        :return: The uid of this AlgorithmLaunch. 
+        :return: The urls of this UploadInfo. 
         :rtype: list[str]
         """
-        return self._uid
+        return self._urls
 
-    @uid.setter
-    def uid(self, uid):
+    @urls.setter
+    def urls(self, urls):
         """
-        A list of uuid strings identifying each job started.
+        One or more URLs for upload via one PUT request per URL.
 
-        :param uid: The uid of this AlgorithmLaunch.
+        :param urls: The urls of this UploadInfo.
         :type: list[str]
         """
 
-        self._uid = uid
+        self._urls = urls
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -152,18 +152,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AlgorithmLaunch):
+        if not isinstance(other, UploadInfo):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AlgorithmLaunch):
+        if not isinstance(other, UploadInfo):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_launch_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state_id_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,145 +14,194 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class AlgorithmLaunchSpec(object):
+class StateIdQuery(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'algorithm_name': 'str',
-        'extra_params': 'list[AlgorithmParameter]',
+        'float_array': 'list[FloatArrayQuery]',
+        'ids': 'list[int]',
+        'localization_ids': 'list[int]',
         'media_ids': 'list[int]',
-        'media_query': 'str'
+        'media_query': 'str',
+        'object_search': 'AttributeOperationSpec'
     }
 
     attribute_map = {
-        'algorithm_name': 'algorithm_name',
-        'extra_params': 'extra_params',
+        'float_array': 'float_array',
+        'ids': 'ids',
+        'localization_ids': 'localization_ids',
         'media_ids': 'media_ids',
-        'media_query': 'media_query'
+        'media_query': 'media_query',
+        'object_search': 'object_search'
     }
 
-    def __init__(self, algorithm_name=None, extra_params=None, media_ids=None, media_query=None, local_vars_configuration=None):  # noqa: E501
-        """AlgorithmLaunchSpec - a model defined in OpenAPI"""
+    def __init__(self, float_array=None, ids=None, localization_ids=None, media_ids=None, media_query=None, object_search=None, local_vars_configuration=None):  # noqa: E501
+        """StateIdQuery - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._algorithm_name = None
-        self._extra_params = None
+        self._float_array = None
+        self._ids = None
+        self._localization_ids = None
         self._media_ids = None
         self._media_query = None
+        self._object_search = None
         self.discriminator = None
 
-        self.algorithm_name = algorithm_name
-        if extra_params is not None:
-            self.extra_params = extra_params
+        if float_array is not None:
+            self.float_array = float_array
+        if ids is not None:
+            self.ids = ids
+        if localization_ids is not None:
+            self.localization_ids = localization_ids
         if media_ids is not None:
             self.media_ids = media_ids
         if media_query is not None:
             self.media_query = media_query
+        if object_search is not None:
+            self.object_search = object_search
 
     @property
-    def algorithm_name(self):
+    def float_array(self):
         """
-        Name of the algorithm to execute.
+        Searches on `float_array` attributes.
 
-        :return: The algorithm_name of this AlgorithmLaunchSpec. 
-        :rtype: str
+        :return: The float_array of this StateIdQuery. 
+        :rtype: list[FloatArrayQuery]
         """
-        return self._algorithm_name
+        return self._float_array
 
-    @algorithm_name.setter
-    def algorithm_name(self, algorithm_name):
+    @float_array.setter
+    def float_array(self, float_array):
         """
-        Name of the algorithm to execute.
+        Searches on `float_array` attributes.
 
-        :param algorithm_name: The algorithm_name of this AlgorithmLaunchSpec.
-        :type: str
+        :param float_array: The float_array of this StateIdQuery.
+        :type: list[FloatArrayQuery]
+        """
+
+        self._float_array = float_array
+
+    @property
+    def ids(self):
+        """
+        Array of state IDs to retrieve.
+
+        :return: The ids of this StateIdQuery. 
+        :rtype: list[int]
+        """
+        return self._ids
+
+    @ids.setter
+    def ids(self, ids):
+        """
+        Array of state IDs to retrieve.
+
+        :param ids: The ids of this StateIdQuery.
+        :type: list[int]
         """
-        if self.local_vars_configuration.client_side_validation and algorithm_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `algorithm_name`, must not be `None`")  # noqa: E501
 
-        self._algorithm_name = algorithm_name
+        self._ids = ids
 
     @property
-    def extra_params(self):
+    def localization_ids(self):
         """
-        Extra parameters to pass into the algorithm
+        Array of child localization IDs for which states should be retrieved.
 
-        :return: The extra_params of this AlgorithmLaunchSpec. 
-        :rtype: list[AlgorithmParameter]
+        :return: The localization_ids of this StateIdQuery. 
+        :rtype: list[int]
         """
-        return self._extra_params
+        return self._localization_ids
 
-    @extra_params.setter
-    def extra_params(self, extra_params):
+    @localization_ids.setter
+    def localization_ids(self, localization_ids):
         """
-        Extra parameters to pass into the algorithm
+        Array of child localization IDs for which states should be retrieved.
 
-        :param extra_params: The extra_params of this AlgorithmLaunchSpec.
-        :type: list[AlgorithmParameter]
+        :param localization_ids: The localization_ids of this StateIdQuery.
+        :type: list[int]
         """
 
-        self._extra_params = extra_params
+        self._localization_ids = localization_ids
 
     @property
     def media_ids(self):
         """
-        List of media IDs. Must supply media_query or media_ids.
+        Array of parent media IDs for which states should be retrieved.
 
-        :return: The media_ids of this AlgorithmLaunchSpec. 
+        :return: The media_ids of this StateIdQuery. 
         :rtype: list[int]
         """
         return self._media_ids
 
     @media_ids.setter
     def media_ids(self, media_ids):
         """
-        List of media IDs. Must supply media_query or media_ids.
+        Array of parent media IDs for which states should be retrieved.
 
-        :param media_ids: The media_ids of this AlgorithmLaunchSpec.
+        :param media_ids: The media_ids of this StateIdQuery.
         :type: list[int]
         """
 
         self._media_ids = media_ids
 
     @property
     def media_query(self):
         """
-        Query string used to filter media IDs. If supplied, media_ids will be ignored.
+        Query string used to filter media IDs. This can be used to avoid serialization and download of a media ID list.
 
-        :return: The media_query of this AlgorithmLaunchSpec. 
+        :return: The media_query of this StateIdQuery. 
         :rtype: str
         """
         return self._media_query
 
     @media_query.setter
     def media_query(self, media_query):
         """
-        Query string used to filter media IDs. If supplied, media_ids will be ignored.
+        Query string used to filter media IDs. This can be used to avoid serialization and download of a media ID list.
 
-        :param media_query: The media_query of this AlgorithmLaunchSpec.
+        :param media_query: The media_query of this StateIdQuery.
         :type: str
         """
 
         self._media_query = media_query
 
+    @property
+    def object_search(self):
+        """
+
+        :return: The object_search of this StateIdQuery. 
+        :rtype: AttributeOperationSpec
+        """
+        return self._object_search
+
+    @object_search.setter
+    def object_search(self, object_search):
+        """
+
+        :param object_search: The object_search of this StateIdQuery.
+        :type: AttributeOperationSpec
+        """
+
+        self._object_search = object_search
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -179,18 +228,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AlgorithmLaunchSpec):
+        if not isinstance(other, StateIdQuery):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AlgorithmLaunchSpec):
+        if not isinstance(other, StateIdQuery):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_manifest.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/algorithm_manifest.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,25 +74,25 @@
         """
 
         self._name = name
 
     @property
     def upload_url(self):
         """
-        URL of the uploaded file returned from tus upload
+        URL of the uploaded file
 
         :return: The upload_url of this AlgorithmManifestSpec. 
         :rtype: str
         """
         return self._upload_url
 
     @upload_url.setter
     def upload_url(self, upload_url):
         """
-        URL of the uploaded file returned from tus upload
+        URL of the uploaded file
 
         :param upload_url: The upload_url of this AlgorithmManifestSpec.
         :type: str
         """
 
         self._upload_url = upload_url
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_parameter.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/algorithm_parameter.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/algorithm_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/algorithm_spec.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,55 +26,85 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'categories': 'list[str]',
         'cluster': 'int',
         'description': 'str',
         'files_per_job': 'int',
         'manifest': 'str',
         'name': 'str',
+        'parameters': 'list[AlgorithmParameter]',
         'user': 'int'
     }
 
     attribute_map = {
+        'categories': 'categories',
         'cluster': 'cluster',
         'description': 'description',
         'files_per_job': 'files_per_job',
         'manifest': 'manifest',
         'name': 'name',
+        'parameters': 'parameters',
         'user': 'user'
     }
 
-    def __init__(self, cluster=None, description=None, files_per_job=None, manifest=None, name=None, user=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, categories=None, cluster=None, description=None, files_per_job=None, manifest=None, name=None, parameters=None, user=None, local_vars_configuration=None):  # noqa: E501
         """AlgorithmSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._categories = None
         self._cluster = None
         self._description = None
         self._files_per_job = None
         self._manifest = None
         self._name = None
+        self._parameters = None
         self._user = None
         self.discriminator = None
 
-        if cluster is not None:
-            self.cluster = cluster
+        if categories is not None:
+            self.categories = categories
+        self.cluster = cluster
         if description is not None:
             self.description = description
         self.files_per_job = files_per_job
         self.manifest = manifest
         self.name = name
+        if parameters is not None:
+            self.parameters = parameters
         self.user = user
 
     @property
+    def categories(self):
+        """
+        List of categories the algorithm workflow belongs to
+
+        :return: The categories of this AlgorithmSpec. 
+        :rtype: list[str]
+        """
+        return self._categories
+
+    @categories.setter
+    def categories(self, categories):
+        """
+        List of categories the algorithm workflow belongs to
+
+        :param categories: The categories of this AlgorithmSpec.
+        :type: list[str]
+        """
+
+        self._categories = categories
+
+    @property
     def cluster(self):
         """
         Unique integer identifying the job cluster.
 
         :return: The cluster of this AlgorithmSpec. 
         :rtype: int
         """
@@ -178,14 +208,35 @@
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
+    def parameters(self):
+        """
+        List of algorithm workflow parameters
+
+        :return: The parameters of this AlgorithmSpec. 
+        :rtype: list[AlgorithmParameter]
+        """
+        return self._parameters
+
+    @parameters.setter
+    def parameters(self, parameters):
+        """
+        List of algorithm workflow parameters
+
+        :param parameters: The parameters of this AlgorithmSpec.
+        :type: list[AlgorithmParameter]
+        """
+
+        self._parameters = parameters
+
+    @property
     def user(self):
         """
         Unique integer identifying the user registering the algorithm.
 
         :return: The user of this AlgorithmSpec. 
         :rtype: int
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/analysis.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/analysis.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/analysis_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/analysis_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/archive_config.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/archive_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         self.local_vars_configuration = local_vars_configuration
 
         self._encode = None
         self._name = None
         self._s3_storage = None
         self.discriminator = None
 
-        if encode is not None:
-            self.encode = encode
+        self.encode = encode
         if name is not None:
             self.name = name
         if s3_storage is not None:
             self.s3_storage = s3_storage
 
     @property
     def encode(self):
@@ -71,14 +70,16 @@
     @encode.setter
     def encode(self, encode):
         """
 
         :param encode: The encode of this ArchiveConfig.
         :type: EncodeConfig
         """
+        if self.local_vars_configuration.client_side_validation and encode is None:  # noqa: E501
+            raise ValueError("Invalid value for `encode`, must not be `None`")  # noqa: E501
 
         self._encode = encode
 
     @property
     def name(self):
         """
         Name of this archive config, used for retrieval in case of multiple archive configs.
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/attribute_bulk_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_prev.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,66 +14,66 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class AttributeBulkUpdate(object):
+class MediaPrev(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'attributes': 'dict(str, object)'
+        'prev': 'int'
     }
 
     attribute_map = {
-        'attributes': 'attributes'
+        'prev': 'prev'
     }
 
-    def __init__(self, attributes=None, local_vars_configuration=None):  # noqa: E501
-        """AttributeBulkUpdate - a model defined in OpenAPI"""
+    def __init__(self, prev=None, local_vars_configuration=None):  # noqa: E501
+        """MediaPrev - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._attributes = None
+        self._prev = None
         self.discriminator = None
 
-        self.attributes = attributes
+        if prev is not None:
+            self.prev = prev
 
     @property
-    def attributes(self):
+    def prev(self):
         """
-        Attribute values to bulk update an entity list.
 
-        :return: The attributes of this AttributeBulkUpdate. 
-        :rtype: dict(str, object)
+        :return: The prev of this MediaPrev. 
+        :rtype: int
         """
-        return self._attributes
+        return self._prev
 
-    @attributes.setter
-    def attributes(self, attributes):
+    @prev.setter
+    def prev(self, prev):
         """
-        Attribute values to bulk update an entity list.
 
-        :param attributes: The attributes of this AttributeBulkUpdate.
-        :type: dict(str, object)
+        :param prev: The prev of this MediaPrev.
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and attributes is None:  # noqa: E501
-            raise ValueError("Invalid value for `attributes`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                prev is not None and prev < 0):  # noqa: E501
+            raise ValueError("Invalid value for `prev`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._attributes = attributes
+        self._prev = prev
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -101,18 +101,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AttributeBulkUpdate):
+        if not isinstance(other, MediaPrev):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AttributeBulkUpdate):
+        if not isinstance(other, MediaPrev):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,35 +37,39 @@
         'dtype': 'str',
         'labels': 'list[str]',
         'maximum': 'float',
         'minimum': 'float',
         'name': 'str',
         'order': 'int',
         'required': 'bool',
+        'size': 'int',
         'style': 'str',
-        'use_current': 'bool'
+        'use_current': 'bool',
+        'visible': 'bool'
     }
 
     attribute_map = {
         'autocomplete': 'autocomplete',
         'choices': 'choices',
         'default': 'default',
         'description': 'description',
         'dtype': 'dtype',
         'labels': 'labels',
         'maximum': 'maximum',
         'minimum': 'minimum',
         'name': 'name',
         'order': 'order',
         'required': 'required',
+        'size': 'size',
         'style': 'style',
-        'use_current': 'use_current'
+        'use_current': 'use_current',
+        'visible': 'visible'
     }
 
-    def __init__(self, autocomplete=None, choices=None, default=None, description='', dtype=None, labels=None, maximum=None, minimum=None, name=None, order=0, required=False, style=None, use_current=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, autocomplete=None, choices=None, default=None, description='', dtype=None, labels=None, maximum=None, minimum=None, name=None, order=0, required=False, size=None, style=None, use_current=None, visible=None, local_vars_configuration=None):  # noqa: E501
         """AttributeType - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._autocomplete = None
         self._choices = None
@@ -74,16 +78,18 @@
         self._dtype = None
         self._labels = None
         self._maximum = None
         self._minimum = None
         self._name = None
         self._order = None
         self._required = None
+        self._size = None
         self._style = None
         self._use_current = None
+        self._visible = None
         self.discriminator = None
 
         self.autocomplete = autocomplete
         if choices is not None:
             self.choices = choices
         self.default = default
         if description is not None:
@@ -98,18 +104,22 @@
             self.minimum = minimum
         if name is not None:
             self.name = name
         if order is not None:
             self.order = order
         if required is not None:
             self.required = required
+        if size is not None:
+            self.size = size
         if style is not None:
             self.style = style
         if use_current is not None:
             self.use_current = use_current
+        if visible is not None:
+            self.visible = visible
 
     @property
     def autocomplete(self):
         """
 
         :return: The autocomplete of this AttributeType. 
         :rtype: AutocompleteService
@@ -146,25 +156,25 @@
         """
 
         self._choices = choices
 
     @property
     def default(self):
         """
-        Boolean, integer, float, string, datetime, or [lon, lat].
+        Boolean, integer, float, string, datetime, [lon, lat], float array.
 
         :return: The default of this AttributeType. 
         :rtype: object
         """
         return self._default
 
     @default.setter
     def default(self, default):
         """
-        Boolean, integer, float, string, datetime, or [lon, lat].
+        Boolean, integer, float, string, datetime, [lon, lat], float array.
 
         :param default: The default of this AttributeType.
         :type: object
         """
 
         self._default = default
 
@@ -203,15 +213,15 @@
     def dtype(self, dtype):
         """
         Data type of the attribute.
 
         :param dtype: The dtype of this AttributeType.
         :type: str
         """
-        allowed_values = ["bool", "int", "float", "enum", "string", "datetime", "geopos"]  # noqa: E501
+        allowed_values = ["bool", "int", "float", "enum", "string", "datetime", "geopos", "float_array"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and dtype not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `dtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(dtype, allowed_values)
             )
 
         self._dtype = dtype
@@ -278,25 +288,25 @@
         """
 
         self._minimum = minimum
 
     @property
     def name(self):
         """
-        Name of the attribute.
+        Name of the attribute. The first character must not be '$', which is a reserved character for system usage.
 
         :return: The name of this AttributeType. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Name of the attribute.
+        Name of the attribute. The first character must not be '$', which is a reserved character for system usage.
 
         :param name: The name of this AttributeType.
         :type: str
         """
 
         self._name = name
 
@@ -339,14 +349,38 @@
         :param required: The required of this AttributeType.
         :type: bool
         """
 
         self._required = required
 
     @property
+    def size(self):
+        """
+        Number of elements for `float_array` dtype.
+
+        :return: The size of this AttributeType. 
+        :rtype: int
+        """
+        return self._size
+
+    @size.setter
+    def size(self, size):
+        """
+        Number of elements for `float_array` dtype.
+
+        :param size: The size of this AttributeType.
+        :type: int
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                size is not None and size < 1):  # noqa: E501
+            raise ValueError("Invalid value for `size`, must be a value greater than or equal to `1`")  # noqa: E501
+
+        self._size = size
+
+    @property
     def style(self):
         """
         Available options: disabled|long_string|start_frame|end_frame|start_frame_check|end_frame_check   Multiple options can be chained together separated by white space. \"disabled\" will not allow the user to edit the attribute in the Tator GUI. Create a text area string if \"long_string\" is combined with \"string\" dtype. \"start_frame\" and \"end_frame\" used in conjunction with \"attr_style_range\" interpolation. \"start_frame_check and \"end_frame_check\" are used in conjunction with \"attr_style_range\" interpolation. \"range_set and in_video_check\" is used in conjunction with \"attr_style_range\" interpolation. When associated with a bool, these checks will result in Tator GUI changes with the corresponding start_frame and end_frame attributes.
 
         :return: The style of this AttributeType. 
         :rtype: str
         """
@@ -380,14 +414,35 @@
 
         :param use_current: The use_current of this AttributeType.
         :type: bool
         """
 
         self._use_current = use_current
 
+    @property
+    def visible(self):
+        """
+        True to make attribute visible.
+
+        :return: The visible of this AttributeType. 
+        :rtype: bool
+        """
+        return self._visible
+
+    @visible.setter
+    def visible(self, visible):
+        """
+        True to make attribute visible.
+
+        :param visible: The visible of this AttributeType.
+        :type: bool
+        """
+
+        self._visible = visible
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type_delete.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type_delete.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,79 +26,79 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'attribute_to_delete': 'str',
-        'entity_type': 'str'
+        'entity_type': 'str',
+        'name': 'str'
     }
 
     attribute_map = {
-        'attribute_to_delete': 'attribute_to_delete',
-        'entity_type': 'entity_type'
+        'entity_type': 'entity_type',
+        'name': 'name'
     }
 
-    def __init__(self, attribute_to_delete=None, entity_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, entity_type=None, name=None, local_vars_configuration=None):  # noqa: E501
         """AttributeTypeDelete - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._attribute_to_delete = None
         self._entity_type = None
+        self._name = None
         self.discriminator = None
 
-        if attribute_to_delete is not None:
-            self.attribute_to_delete = attribute_to_delete
         if entity_type is not None:
             self.entity_type = entity_type
+        if name is not None:
+            self.name = name
 
     @property
-    def attribute_to_delete(self):
+    def entity_type(self):
         """
-        The attribute to delete.
+        The entity type containing the attribute to rename.
 
-        :return: The attribute_to_delete of this AttributeTypeDelete. 
+        :return: The entity_type of this AttributeTypeDelete. 
         :rtype: str
         """
-        return self._attribute_to_delete
+        return self._entity_type
 
-    @attribute_to_delete.setter
-    def attribute_to_delete(self, attribute_to_delete):
+    @entity_type.setter
+    def entity_type(self, entity_type):
         """
-        The attribute to delete.
+        The entity type containing the attribute to rename.
 
-        :param attribute_to_delete: The attribute_to_delete of this AttributeTypeDelete.
+        :param entity_type: The entity_type of this AttributeTypeDelete.
         :type: str
         """
 
-        self._attribute_to_delete = attribute_to_delete
+        self._entity_type = entity_type
 
     @property
-    def entity_type(self):
+    def name(self):
         """
-        The entity type containing the attribute to rename.
+        The attribute to delete.
 
-        :return: The entity_type of this AttributeTypeDelete. 
+        :return: The name of this AttributeTypeDelete. 
         :rtype: str
         """
-        return self._entity_type
+        return self._name
 
-    @entity_type.setter
-    def entity_type(self, entity_type):
+    @name.setter
+    def name(self, name):
         """
-        The entity type containing the attribute to rename.
+        The attribute to delete.
 
-        :param entity_type: The entity_type of this AttributeTypeDelete.
+        :param name: The name of this AttributeTypeDelete.
         :type: str
         """
 
-        self._entity_type = entity_type
+        self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/leaf_update.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,141 +14,143 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class AttributeTypeUpdate(object):
+class LeafUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'entity_type': 'str',
-        '_global': 'str',
-        'new_attribute_type': 'AttributeTypeUpdateNewAttributeType',
-        'old_attribute_type_name': 'str'
+        'attributes': 'dict(str, object)',
+        'name': 'str',
+        'null_attributes': 'list[str]',
+        'reset_attributes': 'list[str]'
     }
 
     attribute_map = {
-        'entity_type': 'entity_type',
-        '_global': 'global',
-        'new_attribute_type': 'new_attribute_type',
-        'old_attribute_type_name': 'old_attribute_type_name'
+        'attributes': 'attributes',
+        'name': 'name',
+        'null_attributes': 'null_attributes',
+        'reset_attributes': 'reset_attributes'
     }
 
-    def __init__(self, entity_type=None, _global=None, new_attribute_type=None, old_attribute_type_name=None, local_vars_configuration=None):  # noqa: E501
-        """AttributeTypeUpdate - a model defined in OpenAPI"""
+    def __init__(self, attributes=None, name=None, null_attributes=None, reset_attributes=None, local_vars_configuration=None):  # noqa: E501
+        """LeafUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._entity_type = None
-        self.__global = None
-        self._new_attribute_type = None
-        self._old_attribute_type_name = None
+        self._attributes = None
+        self._name = None
+        self._null_attributes = None
+        self._reset_attributes = None
         self.discriminator = None
 
-        if entity_type is not None:
-            self.entity_type = entity_type
-        if _global is not None:
-            self._global = _global
-        if new_attribute_type is not None:
-            self.new_attribute_type = new_attribute_type
-        if old_attribute_type_name is not None:
-            self.old_attribute_type_name = old_attribute_type_name
+        if attributes is not None:
+            self.attributes = attributes
+        if name is not None:
+            self.name = name
+        if null_attributes is not None:
+            self.null_attributes = null_attributes
+        if reset_attributes is not None:
+            self.reset_attributes = reset_attributes
 
     @property
-    def entity_type(self):
+    def attributes(self):
         """
-        The entity type containing the attribute to rename.
+        Attribute values to update.
 
-        :return: The entity_type of this AttributeTypeUpdate. 
-        :rtype: str
+        :return: The attributes of this LeafUpdate. 
+        :rtype: dict(str, object)
         """
-        return self._entity_type
+        return self._attributes
 
-    @entity_type.setter
-    def entity_type(self, entity_type):
+    @attributes.setter
+    def attributes(self, attributes):
         """
-        The entity type containing the attribute to rename.
+        Attribute values to update.
 
-        :param entity_type: The entity_type of this AttributeTypeUpdate.
-        :type: str
+        :param attributes: The attributes of this LeafUpdate.
+        :type: dict(str, object)
         """
 
-        self._entity_type = entity_type
+        self._attributes = attributes
 
     @property
-    def _global(self):
+    def name(self):
         """
-        If 'true', applies dtype mutation to all attributes with the same name.
+        Name of the leaf.
 
-        :return: The _global of this AttributeTypeUpdate. 
+        :return: The name of this LeafUpdate. 
         :rtype: str
         """
-        return self.__global
+        return self._name
 
-    @_global.setter
-    def _global(self, _global):
+    @name.setter
+    def name(self, name):
         """
-        If 'true', applies dtype mutation to all attributes with the same name.
+        Name of the leaf.
 
-        :param _global: The _global of this AttributeTypeUpdate.
+        :param name: The name of this LeafUpdate.
         :type: str
         """
 
-        self.__global = _global
+        self._name = name
 
     @property
-    def new_attribute_type(self):
+    def null_attributes(self):
         """
+        Null a value in the attributes body
 
-        :return: The new_attribute_type of this AttributeTypeUpdate. 
-        :rtype: AttributeTypeUpdateNewAttributeType
+        :return: The null_attributes of this LeafUpdate. 
+        :rtype: list[str]
         """
-        return self._new_attribute_type
+        return self._null_attributes
 
-    @new_attribute_type.setter
-    def new_attribute_type(self, new_attribute_type):
+    @null_attributes.setter
+    def null_attributes(self, null_attributes):
         """
+        Null a value in the attributes body
 
-        :param new_attribute_type: The new_attribute_type of this AttributeTypeUpdate.
-        :type: AttributeTypeUpdateNewAttributeType
+        :param null_attributes: The null_attributes of this LeafUpdate.
+        :type: list[str]
         """
 
-        self._new_attribute_type = new_attribute_type
+        self._null_attributes = null_attributes
 
     @property
-    def old_attribute_type_name(self):
+    def reset_attributes(self):
         """
-        The attribute to rename.
+        Reset an attribute to the default value specified in the Type object
 
-        :return: The old_attribute_type_name of this AttributeTypeUpdate. 
-        :rtype: str
+        :return: The reset_attributes of this LeafUpdate. 
+        :rtype: list[str]
         """
-        return self._old_attribute_type_name
+        return self._reset_attributes
 
-    @old_attribute_type_name.setter
-    def old_attribute_type_name(self, old_attribute_type_name):
+    @reset_attributes.setter
+    def reset_attributes(self, reset_attributes):
         """
-        The attribute to rename.
+        Reset an attribute to the default value specified in the Type object
 
-        :param old_attribute_type_name: The old_attribute_type_name of this AttributeTypeUpdate.
-        :type: str
+        :param reset_attributes: The reset_attributes of this LeafUpdate.
+        :type: list[str]
         """
 
-        self._old_attribute_type_name = old_attribute_type_name
+        self._reset_attributes = reset_attributes
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -176,18 +178,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AttributeTypeUpdate):
+        if not isinstance(other, LeafUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AttributeTypeUpdate):
+        if not isinstance(other, LeafUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/attribute_type_update_new_attribute_type.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class AttributeTypeUpdateNewAttributeType(object):
+class AttributeTypeUpdateAttributeTypeUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
@@ -37,36 +37,40 @@
         'dtype': 'str',
         'labels': 'list[str]',
         'maximum': 'float',
         'minimum': 'float',
         'name': 'str',
         'order': 'int',
         'required': 'bool',
+        'size': 'int',
         'style': 'str',
-        'use_current': 'bool'
+        'use_current': 'bool',
+        'visible': 'bool'
     }
 
     attribute_map = {
         'autocomplete': 'autocomplete',
         'choices': 'choices',
         'default': 'default',
         'description': 'description',
         'dtype': 'dtype',
         'labels': 'labels',
         'maximum': 'maximum',
         'minimum': 'minimum',
         'name': 'name',
         'order': 'order',
         'required': 'required',
+        'size': 'size',
         'style': 'style',
-        'use_current': 'use_current'
+        'use_current': 'use_current',
+        'visible': 'visible'
     }
 
-    def __init__(self, autocomplete=None, choices=None, default=None, description=None, dtype=None, labels=None, maximum=None, minimum=None, name=None, order=None, required=None, style=None, use_current=None, local_vars_configuration=None):  # noqa: E501
-        """AttributeTypeUpdateNewAttributeType - a model defined in OpenAPI"""
+    def __init__(self, autocomplete=None, choices=None, default=None, description=None, dtype=None, labels=None, maximum=None, minimum=None, name=None, order=None, required=None, size=None, style=None, use_current=None, visible=None, local_vars_configuration=None):  # noqa: E501
+        """AttributeTypeUpdateAttributeTypeUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._autocomplete = None
         self._choices = None
         self._default = None
@@ -74,16 +78,18 @@
         self._dtype = None
         self._labels = None
         self._maximum = None
         self._minimum = None
         self._name = None
         self._order = None
         self._required = None
+        self._size = None
         self._style = None
         self._use_current = None
+        self._visible = None
         self.discriminator = None
 
         self.autocomplete = autocomplete
         if choices is not None:
             self.choices = choices
         self.default = default
         if description is not None:
@@ -98,296 +104,345 @@
             self.minimum = minimum
         if name is not None:
             self.name = name
         if order is not None:
             self.order = order
         if required is not None:
             self.required = required
+        if size is not None:
+            self.size = size
         if style is not None:
             self.style = style
         if use_current is not None:
             self.use_current = use_current
+        if visible is not None:
+            self.visible = visible
 
     @property
     def autocomplete(self):
         """
 
-        :return: The autocomplete of this AttributeTypeUpdateNewAttributeType. 
+        :return: The autocomplete of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: AutocompleteService
         """
         return self._autocomplete
 
     @autocomplete.setter
     def autocomplete(self, autocomplete):
         """
 
-        :param autocomplete: The autocomplete of this AttributeTypeUpdateNewAttributeType.
+        :param autocomplete: The autocomplete of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: AutocompleteService
         """
 
         self._autocomplete = autocomplete
 
     @property
     def choices(self):
         """
         Array of possible values; required for enum dtype.
 
-        :return: The choices of this AttributeTypeUpdateNewAttributeType. 
+        :return: The choices of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: list[str]
         """
         return self._choices
 
     @choices.setter
     def choices(self, choices):
         """
         Array of possible values; required for enum dtype.
 
-        :param choices: The choices of this AttributeTypeUpdateNewAttributeType.
+        :param choices: The choices of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: list[str]
         """
 
         self._choices = choices
 
     @property
     def default(self):
         """
-        Boolean, integer, float, string, datetime, or [lon, lat].
+        Boolean, integer, float, string, datetime, [lon, lat], float array.
 
-        :return: The default of this AttributeTypeUpdateNewAttributeType. 
+        :return: The default of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: object
         """
         return self._default
 
     @default.setter
     def default(self, default):
         """
-        Boolean, integer, float, string, datetime, or [lon, lat].
+        Boolean, integer, float, string, datetime, [lon, lat], float array.
 
-        :param default: The default of this AttributeTypeUpdateNewAttributeType.
+        :param default: The default of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: object
         """
 
         self._default = default
 
     @property
     def description(self):
         """
         Description of the attribute.
 
-        :return: The description of this AttributeTypeUpdateNewAttributeType. 
+        :return: The description of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
         Description of the attribute.
 
-        :param description: The description of this AttributeTypeUpdateNewAttributeType.
+        :param description: The description of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: str
         """
 
         self._description = description
 
     @property
     def dtype(self):
         """
         Data type of the attribute.
 
-        :return: The dtype of this AttributeTypeUpdateNewAttributeType. 
+        :return: The dtype of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: str
         """
         return self._dtype
 
     @dtype.setter
     def dtype(self, dtype):
         """
         Data type of the attribute.
 
-        :param dtype: The dtype of this AttributeTypeUpdateNewAttributeType.
+        :param dtype: The dtype of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: str
         """
-        allowed_values = ["bool", "int", "float", "enum", "string", "datetime", "geopos"]  # noqa: E501
+        allowed_values = ["bool", "int", "float", "enum", "string", "datetime", "geopos", "float_array"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and dtype not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `dtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(dtype, allowed_values)
             )
 
         self._dtype = dtype
 
     @property
     def labels(self):
         """
         Array of labels for enum dtype.
 
-        :return: The labels of this AttributeTypeUpdateNewAttributeType. 
+        :return: The labels of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: list[str]
         """
         return self._labels
 
     @labels.setter
     def labels(self, labels):
         """
         Array of labels for enum dtype.
 
-        :param labels: The labels of this AttributeTypeUpdateNewAttributeType.
+        :param labels: The labels of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: list[str]
         """
 
         self._labels = labels
 
     @property
     def maximum(self):
         """
         Upper bound for int or float dtype.
 
-        :return: The maximum of this AttributeTypeUpdateNewAttributeType. 
+        :return: The maximum of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: float
         """
         return self._maximum
 
     @maximum.setter
     def maximum(self, maximum):
         """
         Upper bound for int or float dtype.
 
-        :param maximum: The maximum of this AttributeTypeUpdateNewAttributeType.
+        :param maximum: The maximum of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: float
         """
 
         self._maximum = maximum
 
     @property
     def minimum(self):
         """
         Lower bound for int or float dtype.
 
-        :return: The minimum of this AttributeTypeUpdateNewAttributeType. 
+        :return: The minimum of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: float
         """
         return self._minimum
 
     @minimum.setter
     def minimum(self, minimum):
         """
         Lower bound for int or float dtype.
 
-        :param minimum: The minimum of this AttributeTypeUpdateNewAttributeType.
+        :param minimum: The minimum of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: float
         """
 
         self._minimum = minimum
 
     @property
     def name(self):
         """
-        Name of the attribute.
+        Name of the attribute. The first character must not be '$', which is a reserved character for system usage.
 
-        :return: The name of this AttributeTypeUpdateNewAttributeType. 
+        :return: The name of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Name of the attribute.
+        Name of the attribute. The first character must not be '$', which is a reserved character for system usage.
 
-        :param name: The name of this AttributeTypeUpdateNewAttributeType.
+        :param name: The name of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: str
         """
 
         self._name = name
 
     @property
     def order(self):
         """
         Integer specifying relative order this attribute is displayed in the UI. Negative values are hidden by default.
 
-        :return: The order of this AttributeTypeUpdateNewAttributeType. 
+        :return: The order of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: int
         """
         return self._order
 
     @order.setter
     def order(self, order):
         """
         Integer specifying relative order this attribute is displayed in the UI. Negative values are hidden by default.
 
-        :param order: The order of this AttributeTypeUpdateNewAttributeType.
+        :param order: The order of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: int
         """
 
         self._order = order
 
     @property
     def required(self):
         """
         True if this attribute is required for POST requests.
 
-        :return: The required of this AttributeTypeUpdateNewAttributeType. 
+        :return: The required of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: bool
         """
         return self._required
 
     @required.setter
     def required(self, required):
         """
         True if this attribute is required for POST requests.
 
-        :param required: The required of this AttributeTypeUpdateNewAttributeType.
+        :param required: The required of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: bool
         """
 
         self._required = required
 
     @property
+    def size(self):
+        """
+        Number of elements for `float_array` dtype.
+
+        :return: The size of this AttributeTypeUpdateAttributeTypeUpdate. 
+        :rtype: int
+        """
+        return self._size
+
+    @size.setter
+    def size(self, size):
+        """
+        Number of elements for `float_array` dtype.
+
+        :param size: The size of this AttributeTypeUpdateAttributeTypeUpdate.
+        :type: int
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                size is not None and size < 1):  # noqa: E501
+            raise ValueError("Invalid value for `size`, must be a value greater than or equal to `1`")  # noqa: E501
+
+        self._size = size
+
+    @property
     def style(self):
         """
         Available options: disabled|long_string|start_frame|end_frame|start_frame_check|end_frame_check   Multiple options can be chained together separated by white space. \"disabled\" will not allow the user to edit the attribute in the Tator GUI. Create a text area string if \"long_string\" is combined with \"string\" dtype. \"start_frame\" and \"end_frame\" used in conjunction with \"attr_style_range\" interpolation. \"start_frame_check and \"end_frame_check\" are used in conjunction with \"attr_style_range\" interpolation. \"range_set and in_video_check\" is used in conjunction with \"attr_style_range\" interpolation. When associated with a bool, these checks will result in Tator GUI changes with the corresponding start_frame and end_frame attributes.
 
-        :return: The style of this AttributeTypeUpdateNewAttributeType. 
+        :return: The style of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: str
         """
         return self._style
 
     @style.setter
     def style(self, style):
         """
         Available options: disabled|long_string|start_frame|end_frame|start_frame_check|end_frame_check   Multiple options can be chained together separated by white space. \"disabled\" will not allow the user to edit the attribute in the Tator GUI. Create a text area string if \"long_string\" is combined with \"string\" dtype. \"start_frame\" and \"end_frame\" used in conjunction with \"attr_style_range\" interpolation. \"start_frame_check and \"end_frame_check\" are used in conjunction with \"attr_style_range\" interpolation. \"range_set and in_video_check\" is used in conjunction with \"attr_style_range\" interpolation. When associated with a bool, these checks will result in Tator GUI changes with the corresponding start_frame and end_frame attributes.
 
-        :param style: The style of this AttributeTypeUpdateNewAttributeType.
+        :param style: The style of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: str
         """
 
         self._style = style
 
     @property
     def use_current(self):
         """
         True to use current datetime as default for datetime dtype.
 
-        :return: The use_current of this AttributeTypeUpdateNewAttributeType. 
+        :return: The use_current of this AttributeTypeUpdateAttributeTypeUpdate. 
         :rtype: bool
         """
         return self._use_current
 
     @use_current.setter
     def use_current(self, use_current):
         """
         True to use current datetime as default for datetime dtype.
 
-        :param use_current: The use_current of this AttributeTypeUpdateNewAttributeType.
+        :param use_current: The use_current of this AttributeTypeUpdateAttributeTypeUpdate.
         :type: bool
         """
 
         self._use_current = use_current
 
+    @property
+    def visible(self):
+        """
+        True to make attribute visible.
+
+        :return: The visible of this AttributeTypeUpdateAttributeTypeUpdate. 
+        :rtype: bool
+        """
+        return self._visible
+
+    @visible.setter
+    def visible(self, visible):
+        """
+        True to make attribute visible.
+
+        :param visible: The visible of this AttributeTypeUpdateAttributeTypeUpdate.
+        :type: bool
+        """
+
+        self._visible = visible
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -414,18 +469,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AttributeTypeUpdateNewAttributeType):
+        if not isinstance(other, AttributeTypeUpdateAttributeTypeUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AttributeTypeUpdateNewAttributeType):
+        if not isinstance(other, AttributeTypeUpdateAttributeTypeUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/audio_definition.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/audio_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,25 +188,25 @@
         """
 
         self._host = host
 
     @property
     def http_auth(self):
         """
-        If specified will be used for HTTP authorization in request for media, i.e. \"bearer <token>\".
+        If specified will be used for HTTP authorization in request for media, i.e. \"bearer TOKEN\".
 
         :return: The http_auth of this AudioDefinition. 
         :rtype: str
         """
         return self._http_auth
 
     @http_auth.setter
     def http_auth(self, http_auth):
         """
-        If specified will be used for HTTP authorization in request for media, i.e. \"bearer <token>\".
+        If specified will be used for HTTP authorization in request for media, i.e. \"bearer TOKEN\".
 
         :param http_auth: The http_auth of this AudioDefinition.
         :type: str
         """
 
         self._http_auth = http_auth
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/autocomplete_service.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/autocomplete_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,34 +26,60 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'match_any': 'bool',
         'service_url': 'str'
     }
 
     attribute_map = {
+        'match_any': 'match_any',
         'service_url': 'serviceUrl'
     }
 
-    def __init__(self, service_url=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, match_any=False, service_url=None, local_vars_configuration=None):  # noqa: E501
         """AutocompleteService - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._match_any = None
         self._service_url = None
         self.discriminator = None
 
+        if match_any is not None:
+            self.match_any = match_any
         if service_url is not None:
             self.service_url = service_url
 
     @property
+    def match_any(self):
+        """
+        If true, autocomplete will find leaves with any part of name matching the query. Otherwise only leaf names that start with the query are returned.
+
+        :return: The match_any of this AutocompleteService. 
+        :rtype: bool
+        """
+        return self._match_any
+
+    @match_any.setter
+    def match_any(self, match_any):
+        """
+        If true, autocomplete will find leaves with any part of name matching the query. Otherwise only leaf names that start with the query are returned.
+
+        :param match_any: The match_any of this AutocompleteService.
+        :type: bool
+        """
+
+        self._match_any = match_any
+
+    @property
     def service_url(self):
         """
         URL of the autocomplete service.
 
         :return: The service_url of this AutocompleteService. 
         :rtype: str
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/bad_request_response.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/bad_request_response.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/bookmark.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/bookmark_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/bookmark_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/bookmark_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/bookmark_update.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/clone_media_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/clone_media_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/color_map.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/color_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         'map': 'dict(str, object)',
         'version': 'dict(str, object)'
     }
 
     attribute_map = {
         'alpha_ranges': 'alpha_ranges',
         'default': 'default',
-        'default_fill': 'defaultFill',
-        'fill_map': 'fillMap',
+        'default_fill': 'default_fill',
+        'fill_map': 'fill_map',
         'key': 'key',
         'map': 'map',
         'version': 'version'
     }
 
     def __init__(self, alpha_ranges=None, default=None, default_fill=None, fill_map=None, key=None, map=None, version=None, local_vars_configuration=None):  # noqa: E501
         """ColorMap - a model defined in OpenAPI"""
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/create_list_response.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/get_cloned_media_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,87 +14,87 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class CreateListResponse(object):
+class GetClonedMediaResponse(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'list[int]',
+        'ids': 'list[int]',
         'message': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
+        'ids': 'ids',
         'message': 'message'
     }
 
-    def __init__(self, id=None, message=None, local_vars_configuration=None):  # noqa: E501
-        """CreateListResponse - a model defined in OpenAPI"""
+    def __init__(self, ids=None, message=None, local_vars_configuration=None):  # noqa: E501
+        """GetClonedMediaResponse - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
+        self._ids = None
         self._message = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
+        if ids is not None:
+            self.ids = ids
         if message is not None:
             self.message = message
 
     @property
-    def id(self):
+    def ids(self):
         """
-        List of unique integers identifying created objects.
+        List of unique integers identifying cloned objects.
 
-        :return: The id of this CreateListResponse. 
+        :return: The ids of this GetClonedMediaResponse. 
         :rtype: list[int]
         """
-        return self._id
+        return self._ids
 
-    @id.setter
-    def id(self, id):
+    @ids.setter
+    def ids(self, ids):
         """
-        List of unique integers identifying created objects.
+        List of unique integers identifying cloned objects.
 
-        :param id: The id of this CreateListResponse.
+        :param ids: The ids of this GetClonedMediaResponse.
         :type: list[int]
         """
 
-        self._id = id
+        self._ids = ids
 
     @property
     def message(self):
         """
-        Message indicating successful creation.
+        Message indicating return of cloned media list.
 
-        :return: The message of this CreateListResponse. 
+        :return: The message of this GetClonedMediaResponse. 
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
         """
-        Message indicating successful creation.
+        Message indicating return of cloned media list.
 
-        :param message: The message of this CreateListResponse.
+        :param message: The message of this GetClonedMediaResponse.
         :type: str
         """
 
         self._message = message
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -126,18 +126,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateListResponse):
+        if not isinstance(other, GetClonedMediaResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateListResponse):
+        if not isinstance(other, GetClonedMediaResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/create_response.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/notify_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,91 +14,92 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class CreateResponse(object):
+class NotifySpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'int',
-        'message': 'str'
+        'message': 'str',
+        'send_as_file': 'int'
     }
 
     attribute_map = {
-        'id': 'id',
-        'message': 'message'
+        'message': 'message',
+        'send_as_file': 'send_as_file'
     }
 
-    def __init__(self, id=None, message=None, local_vars_configuration=None):  # noqa: E501
-        """CreateResponse - a model defined in OpenAPI"""
+    def __init__(self, message=None, send_as_file=None, local_vars_configuration=None):  # noqa: E501
+        """NotifySpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
         self._message = None
+        self._send_as_file = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
-        if message is not None:
-            self.message = message
+        self.message = message
+        if send_as_file is not None:
+            self.send_as_file = send_as_file
 
     @property
-    def id(self):
+    def message(self):
         """
-        Unique integer identifying the created object.
+        Message to send to administrators.
 
-        :return: The id of this CreateResponse. 
-        :rtype: int
+        :return: The message of this NotifySpec. 
+        :rtype: str
         """
-        return self._id
+        return self._message
 
-    @id.setter
-    def id(self, id):
+    @message.setter
+    def message(self, message):
         """
-        Unique integer identifying the created object.
+        Message to send to administrators.
 
-        :param id: The id of this CreateResponse.
-        :type: int
+        :param message: The message of this NotifySpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and message is None:  # noqa: E501
+            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
-        self._id = id
+        self._message = message
 
     @property
-    def message(self):
+    def send_as_file(self):
         """
-        Message indicating successful creation.
+        Whether to send message as a file. (0 or 1)
 
-        :return: The message of this CreateResponse. 
-        :rtype: str
+        :return: The send_as_file of this NotifySpec. 
+        :rtype: int
         """
-        return self._message
+        return self._send_as_file
 
-    @message.setter
-    def message(self, message):
+    @send_as_file.setter
+    def send_as_file(self, send_as_file):
         """
-        Message indicating successful creation.
+        Whether to send message as a file. (0 or 1)
 
-        :param message: The message of this CreateResponse.
-        :type: str
+        :param send_as_file: The send_as_file of this NotifySpec.
+        :type: int
         """
 
-        self._message = message
+        self._send_as_file = send_as_file
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -126,18 +127,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateResponse):
+        if not isinstance(other, NotifySpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateResponse):
+        if not isinstance(other, NotifySpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/credentials.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,33 +27,38 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'password': 'str',
+        'refresh': 'bool',
         'username': 'str'
     }
 
     attribute_map = {
         'password': 'password',
+        'refresh': 'refresh',
         'username': 'username'
     }
 
-    def __init__(self, password=None, username=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, password=None, refresh=None, username=None, local_vars_configuration=None):  # noqa: E501
         """Credentials - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._password = None
+        self._refresh = None
         self._username = None
         self.discriminator = None
 
         self.password = password
+        if refresh is not None:
+            self.refresh = refresh
         self.username = username
 
     @property
     def password(self):
         """
         Account password.
 
@@ -72,14 +77,35 @@
         """
         if self.local_vars_configuration.client_side_validation and password is None:  # noqa: E501
             raise ValueError("Invalid value for `password`, must not be `None`")  # noqa: E501
 
         self._password = password
 
     @property
+    def refresh(self):
+        """
+        If true, forces generation of new token.
+
+        :return: The refresh of this Credentials. 
+        :rtype: bool
+        """
+        return self._refresh
+
+    @refresh.setter
+    def refresh(self, refresh):
+        """
+        If true, forces generation of new token.
+
+        :param refresh: The refresh of this Credentials.
+        :type: bool
+        """
+
+        self._refresh = refresh
+
+    @property
     def username(self):
         """
         Account username.
 
         :return: The username of this Credentials. 
         :rtype: str
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/download_info.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/download_info.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/download_info_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/download_info_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,15 @@
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._keys = None
         self.discriminator = None
 
-        if keys is not None:
-            self.keys = keys
+        self.keys = keys
 
     @property
     def keys(self):
         """
         Array of object keys for download info retrieval.
 
         :return: The keys of this DownloadInfoSpec. 
@@ -63,14 +62,16 @@
     def keys(self, keys):
         """
         Array of object keys for download info retrieval.
 
         :param keys: The keys of this DownloadInfoSpec.
         :type: list[str]
         """
+        if self.local_vars_configuration.client_side_validation and keys is None:  # noqa: E501
+            raise ValueError("Invalid value for `keys`, must not be `None`")  # noqa: E501
 
         self._keys = keys
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/email_attachment_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/email_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/email_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/email_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/encode_config.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/encode_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,40 +27,45 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'crf': 'int',
+        'movflags': 'str',
         'preset': 'str',
         'tune': 'str',
         'vcodec': 'str'
     }
 
     attribute_map = {
         'crf': 'crf',
+        'movflags': 'movflags',
         'preset': 'preset',
         'tune': 'tune',
         'vcodec': 'vcodec'
     }
 
-    def __init__(self, crf=23, preset='fast', tune='fastdecode', vcodec='hevc', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, crf=23, movflags='', preset='fast', tune='fastdecode', vcodec='hevc', local_vars_configuration=None):  # noqa: E501
         """EncodeConfig - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._crf = None
+        self._movflags = None
         self._preset = None
         self._tune = None
         self._vcodec = None
         self.discriminator = None
 
         if crf is not None:
             self.crf = crf
+        if movflags is not None:
+            self.movflags = movflags
         if preset is not None:
             self.preset = preset
         if tune is not None:
             self.tune = tune
         if vcodec is not None:
             self.vcodec = vcodec
 
@@ -88,14 +93,35 @@
         if (self.local_vars_configuration.client_side_validation and
                 crf is not None and crf < 0):  # noqa: E501
             raise ValueError("Invalid value for `crf`, must be a value greater than or equal to `0`")  # noqa: E501
 
         self._crf = crf
 
     @property
+    def movflags(self):
+        """
+        Movflags to specify to packager
+
+        :return: The movflags of this EncodeConfig. 
+        :rtype: str
+        """
+        return self._movflags
+
+    @movflags.setter
+    def movflags(self, movflags):
+        """
+        Movflags to specify to packager
+
+        :param movflags: The movflags of this EncodeConfig.
+        :type: str
+        """
+
+        self._movflags = movflags
+
+    @property
     def preset(self):
         """
         Preset for ffmpeg encoding.
 
         :return: The preset of this EncodeConfig. 
         :rtype: str
         """
@@ -159,15 +185,15 @@
     def vcodec(self, vcodec):
         """
         Video codec.
 
         :param vcodec: The vcodec of this EncodeConfig.
         :type: str
         """
-        allowed_values = ["h264", "hevc"]  # noqa: E501
+        allowed_values = ["copy", "h264", "hevc"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and vcodec not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `vcodec` ({0}), must be one of {1}"  # noqa: E501
                 .format(vcodec, allowed_values)
             )
 
         self._vcodec = vcodec
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/favorite.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/temporary_file_spec.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,204 +14,152 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Favorite(object):
+class TemporaryFileSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'int',
-        'meta': 'int',
+        'hours': 'int',
+        'lookup': 'str',
         'name': 'str',
-        'page': 'int',
-        'user': 'int',
-        'values': 'dict(str, object)'
+        'url': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
-        'meta': 'meta',
+        'hours': 'hours',
+        'lookup': 'lookup',
         'name': 'name',
-        'page': 'page',
-        'user': 'user',
-        'values': 'values'
+        'url': 'url'
     }
 
-    def __init__(self, id=None, meta=None, name=None, page=1, user=None, values=None, local_vars_configuration=None):  # noqa: E501
-        """Favorite - a model defined in OpenAPI"""
+    def __init__(self, hours=24, lookup=None, name=None, url=None, local_vars_configuration=None):  # noqa: E501
+        """TemporaryFileSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._meta = None
+        self._hours = None
+        self._lookup = None
         self._name = None
-        self._page = None
-        self._user = None
-        self._values = None
+        self._url = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
-        if meta is not None:
-            self.meta = meta
-        if name is not None:
-            self.name = name
-        if page is not None:
-            self.page = page
-        if user is not None:
-            self.user = user
-        if values is not None:
-            self.values = values
+        if hours is not None:
+            self.hours = hours
+        self.lookup = lookup
+        self.name = name
+        self.url = url
 
     @property
-    def id(self):
+    def hours(self):
         """
-        Unique integer identifying a favorite.
+        Number of hours file is to be kept alive
 
-        :return: The id of this Favorite. 
+        :return: The hours of this TemporaryFileSpec. 
         :rtype: int
         """
-        return self._id
+        return self._hours
 
-    @id.setter
-    def id(self, id):
+    @hours.setter
+    def hours(self, hours):
         """
-        Unique integer identifying a favorite.
+        Number of hours file is to be kept alive
 
-        :param id: The id of this Favorite.
+        :param hours: The hours of this TemporaryFileSpec.
         :type: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                hours is not None and hours > 24):  # noqa: E501
+            raise ValueError("Invalid value for `hours`, must be a value less than or equal to `24`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                hours is not None and hours < 1):  # noqa: E501
+            raise ValueError("Invalid value for `hours`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._id = id
+        self._hours = hours
 
     @property
-    def meta(self):
+    def lookup(self):
         """
-        Unique integer identifying entity type of this localization.
+        md5hash of lookup parameters
 
-        :return: The meta of this Favorite. 
-        :rtype: int
+        :return: The lookup of this TemporaryFileSpec. 
+        :rtype: str
         """
-        return self._meta
+        return self._lookup
 
-    @meta.setter
-    def meta(self, meta):
+    @lookup.setter
+    def lookup(self, lookup):
         """
-        Unique integer identifying entity type of this localization.
+        md5hash of lookup parameters
 
-        :param meta: The meta of this Favorite.
-        :type: int
+        :param lookup: The lookup of this TemporaryFileSpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and lookup is None:  # noqa: E501
+            raise ValueError("Invalid value for `lookup`, must not be `None`")  # noqa: E501
 
-        self._meta = meta
+        self._lookup = lookup
 
     @property
     def name(self):
         """
-        Name of the favorite.
+        Unique name for the temporary file
 
-        :return: The name of this Favorite. 
+        :return: The name of this TemporaryFileSpec. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Name of the favorite.
+        Unique name for the temporary file
 
-        :param name: The name of this Favorite.
+        :param name: The name of this TemporaryFileSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def page(self):
-        """
-        Integer specifying page to display on. Should be 1-10.
-
-        :return: The page of this Favorite. 
-        :rtype: int
+    def url(self):
         """
-        return self._page
+        URL for the temporary file
 
-    @page.setter
-    def page(self, page):
-        """
-        Integer specifying page to display on. Should be 1-10.
-
-        :param page: The page of this Favorite.
-        :type: int
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                page is not None and page > 10):  # noqa: E501
-            raise ValueError("Invalid value for `page`, must be a value less than or equal to `10`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                page is not None and page < 1):  # noqa: E501
-            raise ValueError("Invalid value for `page`, must be a value greater than or equal to `1`")  # noqa: E501
-
-        self._page = page
-
-    @property
-    def user(self):
-        """
-        Unique integer identifying a user.
-
-        :return: The user of this Favorite. 
-        :rtype: int
-        """
-        return self._user
-
-    @user.setter
-    def user(self, user):
-        """
-        Unique integer identifying a user.
-
-        :param user: The user of this Favorite.
-        :type: int
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                user is not None and user < 1):  # noqa: E501
-            raise ValueError("Invalid value for `user`, must be a value greater than or equal to `1`")  # noqa: E501
-
-        self._user = user
-
-    @property
-    def values(self):
-        """
-        Attribute name/value pairs.
-
-        :return: The values of this Favorite. 
-        :rtype: dict(str, object)
+        :return: The url of this TemporaryFileSpec. 
+        :rtype: str
         """
-        return self._values
+        return self._url
 
-    @values.setter
-    def values(self, values):
+    @url.setter
+    def url(self, url):
         """
-        Attribute name/value pairs.
+        URL for the temporary file
 
-        :param values: The values of this Favorite.
-        :type: dict(str, object)
+        :param url: The url of this TemporaryFileSpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and url is None:  # noqa: E501
+            raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
 
-        self._values = values
+        self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -239,18 +187,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Favorite):
+        if not isinstance(other, TemporaryFileSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Favorite):
+        if not isinstance(other, TemporaryFileSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/favorite_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/multi_definition.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,152 +14,143 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class FavoriteSpec(object):
+class MultiDefinition(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'page': 'int',
-        'type': 'int',
-        'values': 'dict(str, object)'
+        'frame_offset': 'list[int]',
+        'ids': 'list[int]',
+        'layout': 'list[int]',
+        'quality': 'int'
     }
 
     attribute_map = {
-        'name': 'name',
-        'page': 'page',
-        'type': 'type',
-        'values': 'values'
+        'frame_offset': 'frameOffset',
+        'ids': 'ids',
+        'layout': 'layout',
+        'quality': 'quality'
     }
 
-    def __init__(self, name=None, page=1, type=None, values=None, local_vars_configuration=None):  # noqa: E501
-        """FavoriteSpec - a model defined in OpenAPI"""
+    def __init__(self, frame_offset=None, ids=None, layout=None, quality=None, local_vars_configuration=None):  # noqa: E501
+        """MultiDefinition - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._page = None
-        self._type = None
-        self._values = None
+        self._frame_offset = None
+        self._ids = None
+        self._layout = None
+        self._quality = None
         self.discriminator = None
 
-        if name is not None:
-            self.name = name
-        if page is not None:
-            self.page = page
-        if type is not None:
-            self.type = type
-        if values is not None:
-            self.values = values
+        if frame_offset is not None:
+            self.frame_offset = frame_offset
+        if ids is not None:
+            self.ids = ids
+        if layout is not None:
+            self.layout = layout
+        if quality is not None:
+            self.quality = quality
 
     @property
-    def name(self):
+    def frame_offset(self):
         """
-        Name of the favorite.
+        Frame of sub-video, offset from media in slot 0.
 
-        :return: The name of this FavoriteSpec. 
-        :rtype: str
+        :return: The frame_offset of this MultiDefinition. 
+        :rtype: list[int]
         """
-        return self._name
+        return self._frame_offset
 
-    @name.setter
-    def name(self, name):
+    @frame_offset.setter
+    def frame_offset(self, frame_offset):
         """
-        Name of the favorite.
+        Frame of sub-video, offset from media in slot 0.
 
-        :param name: The name of this FavoriteSpec.
-        :type: str
+        :param frame_offset: The frame_offset of this MultiDefinition.
+        :type: list[int]
         """
 
-        self._name = name
+        self._frame_offset = frame_offset
 
     @property
-    def page(self):
+    def ids(self):
         """
-        Integer specifying page to display on. Should be 1-10.
+        If multi-stream list of ids of sub-videos
 
-        :return: The page of this FavoriteSpec. 
-        :rtype: int
+        :return: The ids of this MultiDefinition. 
+        :rtype: list[int]
         """
-        return self._page
+        return self._ids
 
-    @page.setter
-    def page(self, page):
+    @ids.setter
+    def ids(self, ids):
         """
-        Integer specifying page to display on. Should be 1-10.
+        If multi-stream list of ids of sub-videos
 
-        :param page: The page of this FavoriteSpec.
-        :type: int
+        :param ids: The ids of this MultiDefinition.
+        :type: list[int]
         """
-        if (self.local_vars_configuration.client_side_validation and
-                page is not None and page > 10):  # noqa: E501
-            raise ValueError("Invalid value for `page`, must be a value less than or equal to `10`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                page is not None and page < 1):  # noqa: E501
-            raise ValueError("Invalid value for `page`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._page = page
+        self._ids = ids
 
     @property
-    def type(self):
+    def layout(self):
         """
-        Unique integer identifying a localization type.
+        2-element array to define rxc layout
 
-        :return: The type of this FavoriteSpec. 
-        :rtype: int
+        :return: The layout of this MultiDefinition. 
+        :rtype: list[int]
         """
-        return self._type
+        return self._layout
 
-    @type.setter
-    def type(self, type):
+    @layout.setter
+    def layout(self, layout):
         """
-        Unique integer identifying a localization type.
+        2-element array to define rxc layout
 
-        :param type: The type of this FavoriteSpec.
-        :type: int
+        :param layout: The layout of this MultiDefinition.
+        :type: list[int]
         """
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and type < 1):  # noqa: E501
-            raise ValueError("Invalid value for `type`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._type = type
+        self._layout = layout
 
     @property
-    def values(self):
+    def quality(self):
         """
-        Attribute name/value pairs.
+        Resolution to fetch on each sub-video
 
-        :return: The values of this FavoriteSpec. 
-        :rtype: dict(str, object)
+        :return: The quality of this MultiDefinition. 
+        :rtype: int
         """
-        return self._values
+        return self._quality
 
-    @values.setter
-    def values(self, values):
+    @quality.setter
+    def quality(self, quality):
         """
-        Attribute name/value pairs.
+        Resolution to fetch on each sub-video
 
-        :param values: The values of this FavoriteSpec.
-        :type: dict(str, object)
+        :param quality: The quality of this MultiDefinition.
+        :type: int
         """
 
-        self._values = values
+        self._quality = quality
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -187,18 +178,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FavoriteSpec):
+        if not isinstance(other, MultiDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FavoriteSpec):
+        if not isinstance(other, MultiDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/favorite_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/not_found_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,65 +14,65 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class FavoriteUpdate(object):
+class NotFoundResponse(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str'
+        'message': 'str'
     }
 
     attribute_map = {
-        'name': 'name'
+        'message': 'message'
     }
 
-    def __init__(self, name=None, local_vars_configuration=None):  # noqa: E501
-        """FavoriteUpdate - a model defined in OpenAPI"""
+    def __init__(self, message=None, local_vars_configuration=None):  # noqa: E501
+        """NotFoundResponse - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
+        self._message = None
         self.discriminator = None
 
-        if name is not None:
-            self.name = name
+        if message is not None:
+            self.message = message
 
     @property
-    def name(self):
+    def message(self):
         """
-        Name of the favorite.
+        Message explaining not found error.
 
-        :return: The name of this FavoriteUpdate. 
+        :return: The message of this NotFoundResponse. 
         :rtype: str
         """
-        return self._name
+        return self._message
 
-    @name.setter
-    def name(self, name):
+    @message.setter
+    def message(self, message):
         """
-        Name of the favorite.
+        Message explaining not found error.
 
-        :param name: The name of this FavoriteUpdate.
+        :param message: The message of this NotFoundResponse.
         :type: str
         """
 
-        self._name = name
+        self._message = message
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -100,18 +100,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FavoriteUpdate):
+        if not isinstance(other, NotFoundResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FavoriteUpdate):
+        if not isinstance(other, NotFoundResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/fill.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/fill.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/image_definition.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/image_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,25 +92,25 @@
         """
 
         self._host = host
 
     @property
     def http_auth(self):
         """
-        If specified will be used for HTTP authorization in request for media, i.e. \"bearer <token>\".
+        If specified will be used for HTTP authorization in request for media, i.e. \"bearer TOKEN\".
 
         :return: The http_auth of this ImageDefinition. 
         :rtype: str
         """
         return self._http_auth
 
     @http_auth.setter
     def http_auth(self, http_auth):
         """
-        If specified will be used for HTTP authorization in request for media, i.e. \"bearer <token>\".
+        If specified will be used for HTTP authorization in request for media, i.e. \"bearer TOKEN\".
 
         :param http_auth: The http_auth of this ImageDefinition.
         :type: str
         """
 
         self._http_auth = http_auth
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/job.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/temporary_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,265 +14,243 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Job(object):
+class TemporaryFile(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'gid': 'str',
-        'id': 'str',
-        'nodes': 'list[JobNode]',
+        'created_datetime': 'str',
+        'eol_datetime': 'str',
+        'id': 'int',
+        'lookup': 'str',
+        'name': 'str',
+        'path': 'str',
         'project': 'int',
-        'start_time': 'datetime',
-        'status': 'str',
-        'stop_time': 'datetime',
-        'uid': 'str',
         'user': 'int'
     }
 
     attribute_map = {
-        'gid': 'gid',
+        'created_datetime': 'created_datetime',
+        'eol_datetime': 'eol_datetime',
         'id': 'id',
-        'nodes': 'nodes',
+        'lookup': 'lookup',
+        'name': 'name',
+        'path': 'path',
         'project': 'project',
-        'start_time': 'start_time',
-        'status': 'status',
-        'stop_time': 'stop_time',
-        'uid': 'uid',
         'user': 'user'
     }
 
-    def __init__(self, gid=None, id=None, nodes=None, project=None, start_time=None, status=None, stop_time=None, uid=None, user=None, local_vars_configuration=None):  # noqa: E501
-        """Job - a model defined in OpenAPI"""
+    def __init__(self, created_datetime=None, eol_datetime=None, id=None, lookup=None, name=None, path=None, project=None, user=None, local_vars_configuration=None):  # noqa: E501
+        """TemporaryFile - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._gid = None
+        self._created_datetime = None
+        self._eol_datetime = None
         self._id = None
-        self._nodes = None
+        self._lookup = None
+        self._name = None
+        self._path = None
         self._project = None
-        self._start_time = None
-        self._status = None
-        self._stop_time = None
-        self._uid = None
         self._user = None
         self.discriminator = None
 
-        if gid is not None:
-            self.gid = gid
+        if created_datetime is not None:
+            self.created_datetime = created_datetime
+        if eol_datetime is not None:
+            self.eol_datetime = eol_datetime
         if id is not None:
             self.id = id
-        if nodes is not None:
-            self.nodes = nodes
+        if lookup is not None:
+            self.lookup = lookup
+        if name is not None:
+            self.name = name
+        if path is not None:
+            self.path = path
         if project is not None:
             self.project = project
-        self.start_time = start_time
-        if status is not None:
-            self.status = status
-        self.stop_time = stop_time
-        if uid is not None:
-            self.uid = uid
         if user is not None:
             self.user = user
 
     @property
-    def gid(self):
+    def created_datetime(self):
         """
-        Group ID of the job.
+        Datetime when this temporary file was created.
 
-        :return: The gid of this Job. 
+        :return: The created_datetime of this TemporaryFile. 
         :rtype: str
         """
-        return self._gid
+        return self._created_datetime
 
-    @gid.setter
-    def gid(self, gid):
+    @created_datetime.setter
+    def created_datetime(self, created_datetime):
         """
-        Group ID of the job.
+        Datetime when this temporary file was created.
 
-        :param gid: The gid of this Job.
+        :param created_datetime: The created_datetime of this TemporaryFile.
         :type: str
         """
 
-        self._gid = gid
+        self._created_datetime = created_datetime
 
     @property
-    def id(self):
+    def eol_datetime(self):
         """
-        Unique identifier of the job generated by Argo.
+        Datetime when this temporary file may be deleted.
 
-        :return: The id of this Job. 
+        :return: The eol_datetime of this TemporaryFile. 
         :rtype: str
         """
-        return self._id
+        return self._eol_datetime
 
-    @id.setter
-    def id(self, id):
+    @eol_datetime.setter
+    def eol_datetime(self, eol_datetime):
         """
-        Unique identifier of the job generated by Argo.
+        Datetime when this temporary file may be deleted.
 
-        :param id: The id of this Job.
+        :param eol_datetime: The eol_datetime of this TemporaryFile.
         :type: str
         """
 
-        self._id = id
+        self._eol_datetime = eol_datetime
 
     @property
-    def nodes(self):
-        """
-
-        :return: The nodes of this Job. 
-        :rtype: list[JobNode]
-        """
-        return self._nodes
-
-    @nodes.setter
-    def nodes(self, nodes):
-        """
-
-        :param nodes: The nodes of this Job.
-        :type: list[JobNode]
-        """
-
-        self._nodes = nodes
-
-    @property
-    def project(self):
+    def id(self):
         """
-        Unique integer identifying a project.
+        Unique integer identifying a temporary file.
 
-        :return: The project of this Job. 
+        :return: The id of this TemporaryFile. 
         :rtype: int
         """
-        return self._project
+        return self._id
 
-    @project.setter
-    def project(self, project):
+    @id.setter
+    def id(self, id):
         """
-        Unique integer identifying a project.
+        Unique integer identifying a temporary file.
 
-        :param project: The project of this Job.
+        :param id: The id of this TemporaryFile.
         :type: int
         """
 
-        self._project = project
+        self._id = id
 
     @property
-    def start_time(self):
+    def lookup(self):
         """
-        Start time of this job.
+        md5hash of lookup parameters
 
-        :return: The start_time of this Job. 
-        :rtype: datetime
+        :return: The lookup of this TemporaryFile. 
+        :rtype: str
         """
-        return self._start_time
+        return self._lookup
 
-    @start_time.setter
-    def start_time(self, start_time):
+    @lookup.setter
+    def lookup(self, lookup):
         """
-        Start time of this job.
+        md5hash of lookup parameters
 
-        :param start_time: The start_time of this Job.
-        :type: datetime
+        :param lookup: The lookup of this TemporaryFile.
+        :type: str
         """
 
-        self._start_time = start_time
+        self._lookup = lookup
 
     @property
-    def status(self):
+    def name(self):
         """
-        Status of this job.
+        Unique name for the temporary file
 
-        :return: The status of this Job. 
+        :return: The name of this TemporaryFile. 
         :rtype: str
         """
-        return self._status
+        return self._name
 
-    @status.setter
-    def status(self, status):
+    @name.setter
+    def name(self, name):
         """
-        Status of this job.
+        Unique name for the temporary file
 
-        :param status: The status of this Job.
+        :param name: The name of this TemporaryFile.
         :type: str
         """
 
-        self._status = status
+        self._name = name
 
     @property
-    def stop_time(self):
+    def path(self):
         """
-        Stop time of this job.
+        Full URL to the temporary file.
 
-        :return: The stop_time of this Job. 
-        :rtype: datetime
+        :return: The path of this TemporaryFile. 
+        :rtype: str
         """
-        return self._stop_time
+        return self._path
 
-    @stop_time.setter
-    def stop_time(self, stop_time):
+    @path.setter
+    def path(self, path):
         """
-        Stop time of this job.
+        Full URL to the temporary file.
 
-        :param stop_time: The stop_time of this Job.
-        :type: datetime
+        :param path: The path of this TemporaryFile.
+        :type: str
         """
 
-        self._stop_time = stop_time
+        self._path = path
 
     @property
-    def uid(self):
+    def project(self):
         """
-        Unique ID of the job.
+        Unique integer identifying a project.
 
-        :return: The uid of this Job. 
-        :rtype: str
+        :return: The project of this TemporaryFile. 
+        :rtype: int
         """
-        return self._uid
+        return self._project
 
-    @uid.setter
-    def uid(self, uid):
+    @project.setter
+    def project(self, project):
         """
-        Unique ID of the job.
+        Unique integer identifying a project.
 
-        :param uid: The uid of this Job.
-        :type: str
+        :param project: The project of this TemporaryFile.
+        :type: int
         """
 
-        self._uid = uid
+        self._project = project
 
     @property
     def user(self):
         """
-        Unique integer identifying user who submitted the job.
+        Unique integer identifying user who created this file.
 
-        :return: The user of this Job. 
+        :return: The user of this TemporaryFile. 
         :rtype: int
         """
         return self._user
 
     @user.setter
     def user(self, user):
         """
-        Unique integer identifying user who submitted the job.
+        Unique integer identifying user who created this file.
 
-        :param user: The user of this Job.
+        :param user: The user of this TemporaryFile.
         :type: int
         """
 
         self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -304,18 +282,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Job):
+        if not isinstance(other, TemporaryFile):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Job):
+        if not isinstance(other, TemporaryFile):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/job_node.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/job_node.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/leaf.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/leaf.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,59 +28,59 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'attributes': 'dict(str, object)',
         'id': 'int',
-        'meta': 'int',
         'name': 'str',
         'parent': 'int',
         'path': 'str',
-        'project': 'int'
+        'project': 'int',
+        'type': 'int'
     }
 
     attribute_map = {
         'attributes': 'attributes',
         'id': 'id',
-        'meta': 'meta',
         'name': 'name',
         'parent': 'parent',
         'path': 'path',
-        'project': 'project'
+        'project': 'project',
+        'type': 'type'
     }
 
-    def __init__(self, attributes=None, id=None, meta=None, name=None, parent=None, path=None, project=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, id=None, name=None, parent=None, path=None, project=None, type=None, local_vars_configuration=None):  # noqa: E501
         """Leaf - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
         self._id = None
-        self._meta = None
         self._name = None
         self._parent = None
         self._path = None
         self._project = None
+        self._type = None
         self.discriminator = None
 
         if attributes is not None:
             self.attributes = attributes
         if id is not None:
             self.id = id
-        if meta is not None:
-            self.meta = meta
         if name is not None:
             self.name = name
         self.parent = parent
         if path is not None:
             self.path = path
         if project is not None:
             self.project = project
+        if type is not None:
+            self.type = type
 
     @property
     def attributes(self):
         """
         Object containing attribute values.
 
         :return: The attributes of this Leaf. 
@@ -117,35 +117,14 @@
         :param id: The id of this Leaf.
         :type: int
         """
 
         self._id = id
 
     @property
-    def meta(self):
-        """
-        Unique integer identifying the entity type.
-
-        :return: The meta of this Leaf. 
-        :rtype: int
-        """
-        return self._meta
-
-    @meta.setter
-    def meta(self, meta):
-        """
-        Unique integer identifying the entity type.
-
-        :param meta: The meta of this Leaf.
-        :type: int
-        """
-
-        self._meta = meta
-
-    @property
     def name(self):
         """
         Name of the leaf.
 
         :return: The name of this Leaf. 
         :rtype: str
         """
@@ -221,14 +200,35 @@
 
         :param project: The project of this Leaf.
         :type: int
         """
 
         self._project = project
 
+    @property
+    def type(self):
+        """
+        Unique integer identifying the entity type.
+
+        :return: The type of this Leaf. 
+        :rtype: int
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """
+        Unique integer identifying the entity type.
+
+        :param type: The type of this Leaf.
+        :type: int
+        """
+
+        self._type = type
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/leaf_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/leaf_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,41 +26,67 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'attributes': 'dict(str, object)',
         'name': 'str',
         'parent': 'int',
         'type': 'int'
     }
 
     attribute_map = {
+        'attributes': 'attributes',
         'name': 'name',
         'parent': 'parent',
         'type': 'type'
     }
 
-    def __init__(self, name=None, parent=None, type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, name=None, parent=None, type=None, local_vars_configuration=None):  # noqa: E501
         """LeafSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._attributes = None
         self._name = None
         self._parent = None
         self._type = None
         self.discriminator = None
 
+        if attributes is not None:
+            self.attributes = attributes
         self.name = name
         self.parent = parent
         self.type = type
 
     @property
+    def attributes(self):
+        """
+        Object containing attribute values.
+
+        :return: The attributes of this LeafSpec. 
+        :rtype: dict(str, object)
+        """
+        return self._attributes
+
+    @attributes.setter
+    def attributes(self, attributes):
+        """
+        Object containing attribute values.
+
+        :param attributes: The attributes of this LeafSpec.
+        :type: dict(str, object)
+        """
+
+        self._attributes = attributes
+
+    @property
     def name(self):
         """
         Name of the leaf.
 
         :return: The name of this LeafSpec. 
         :rtype: str
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/leaf_suggestion.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/leaf_suggestion.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/leaf_type.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/leaf_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,48 +29,52 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'attribute_types': 'list[AttributeType]',
         'description': 'str',
         'dtype': 'str',
+        'elemental_id': 'str',
         'id': 'int',
         'name': 'str',
         'project': 'int'
     }
 
     attribute_map = {
         'attribute_types': 'attribute_types',
         'description': 'description',
         'dtype': 'dtype',
+        'elemental_id': 'elemental_id',
         'id': 'id',
         'name': 'name',
         'project': 'project'
     }
 
-    def __init__(self, attribute_types=None, description='', dtype=None, id=None, name=None, project=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attribute_types=None, description='', dtype=None, elemental_id=None, id=None, name=None, project=None, local_vars_configuration=None):  # noqa: E501
         """LeafType - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attribute_types = None
         self._description = None
         self._dtype = None
+        self._elemental_id = None
         self._id = None
         self._name = None
         self._project = None
         self.discriminator = None
 
         if attribute_types is not None:
             self.attribute_types = attribute_types
         if description is not None:
             self.description = description
         if dtype is not None:
             self.dtype = dtype
+        self.elemental_id = elemental_id
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
         if project is not None:
             self.project = project
 
@@ -134,14 +138,35 @@
         :param dtype: The dtype of this LeafType.
         :type: str
         """
 
         self._dtype = dtype
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this LeafType. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this LeafType.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def id(self):
         """
         Unique integer identifying a leaf type.
 
         :return: The id of this LeafType. 
         :rtype: int
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/leaf_type_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/file_type_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,113 +14,138 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class LeafTypeSpec(object):
+class FileTypeSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'attribute_types': 'list[AttributeType]',
         'description': 'str',
+        'elemental_id': 'str',
         'name': 'str'
     }
 
     attribute_map = {
         'attribute_types': 'attribute_types',
         'description': 'description',
+        'elemental_id': 'elemental_id',
         'name': 'name'
     }
 
-    def __init__(self, attribute_types=None, description='', name=None, local_vars_configuration=None):  # noqa: E501
-        """LeafTypeSpec - a model defined in OpenAPI"""
+    def __init__(self, attribute_types=None, description='', elemental_id=None, name=None, local_vars_configuration=None):  # noqa: E501
+        """FileTypeSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attribute_types = None
         self._description = None
+        self._elemental_id = None
         self._name = None
         self.discriminator = None
 
         if attribute_types is not None:
             self.attribute_types = attribute_types
         if description is not None:
             self.description = description
+        self.elemental_id = elemental_id
         if name is not None:
             self.name = name
 
     @property
     def attribute_types(self):
         """
         Attribute type definitions.
 
-        :return: The attribute_types of this LeafTypeSpec. 
+        :return: The attribute_types of this FileTypeSpec. 
         :rtype: list[AttributeType]
         """
         return self._attribute_types
 
     @attribute_types.setter
     def attribute_types(self, attribute_types):
         """
         Attribute type definitions.
 
-        :param attribute_types: The attribute_types of this LeafTypeSpec.
+        :param attribute_types: The attribute_types of this FileTypeSpec.
         :type: list[AttributeType]
         """
 
         self._attribute_types = attribute_types
 
     @property
     def description(self):
         """
-        Description of the leaf type.
+        Description of the file type.
 
-        :return: The description of this LeafTypeSpec. 
+        :return: The description of this FileTypeSpec. 
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
-        Description of the leaf type.
+        Description of the file type.
 
-        :param description: The description of this LeafTypeSpec.
+        :param description: The description of this FileTypeSpec.
         :type: str
         """
 
         self._description = description
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this FileTypeSpec. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this FileTypeSpec.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def name(self):
         """
-        Name of the leaf type.
+        Name of the file type.
 
-        :return: The name of this LeafTypeSpec. 
+        :return: The name of this FileTypeSpec. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Name of the leaf type.
+        Name of the file type.
 
-        :param name: The name of this LeafTypeSpec.
+        :param name: The name of this FileTypeSpec.
         :type: str
         """
 
         self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -152,18 +177,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LeafTypeSpec):
+        if not isinstance(other, FileTypeSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LeafTypeSpec):
+        if not isinstance(other, FileTypeSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/leaf_type_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/leaf_type_update.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,34 +27,38 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'description': 'str',
+        'elemental_id': 'str',
         'name': 'str'
     }
 
     attribute_map = {
         'description': 'description',
+        'elemental_id': 'elemental_id',
         'name': 'name'
     }
 
-    def __init__(self, description='', name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, description=None, elemental_id=None, name=None, local_vars_configuration=None):  # noqa: E501
         """LeafTypeUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._description = None
+        self._elemental_id = None
         self._name = None
         self.discriminator = None
 
         if description is not None:
             self.description = description
+        self.elemental_id = elemental_id
         if name is not None:
             self.name = name
 
     @property
     def description(self):
         """
         Description of the leaf type.
@@ -72,14 +76,35 @@
         :param description: The description of this LeafTypeUpdate.
         :type: str
         """
 
         self._description = description
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this LeafTypeUpdate. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this LeafTypeUpdate.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def name(self):
         """
         Name of the leaf type.
 
         :return: The name of this LeafTypeUpdate. 
         :rtype: str
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/leaf_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/password_reset_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,91 +14,66 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class LeafUpdate(object):
+class PasswordResetSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'attributes': 'dict(str, object)',
-        'name': 'str'
+        'email': 'str'
     }
 
     attribute_map = {
-        'attributes': 'attributes',
-        'name': 'name'
+        'email': 'email'
     }
 
-    def __init__(self, attributes=None, name=None, local_vars_configuration=None):  # noqa: E501
-        """LeafUpdate - a model defined in OpenAPI"""
+    def __init__(self, email=None, local_vars_configuration=None):  # noqa: E501
+        """PasswordResetSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._attributes = None
-        self._name = None
+        self._email = None
         self.discriminator = None
 
-        if attributes is not None:
-            self.attributes = attributes
-        if name is not None:
-            self.name = name
+        self.email = email
 
     @property
-    def attributes(self):
+    def email(self):
         """
-        Attribute values to update.
+        Email address registered for user requesting reset.
 
-        :return: The attributes of this LeafUpdate. 
-        :rtype: dict(str, object)
-        """
-        return self._attributes
-
-    @attributes.setter
-    def attributes(self, attributes):
-        """
-        Attribute values to update.
-
-        :param attributes: The attributes of this LeafUpdate.
-        :type: dict(str, object)
-        """
-
-        self._attributes = attributes
-
-    @property
-    def name(self):
-        """
-        Name of the leaf.
-
-        :return: The name of this LeafUpdate. 
+        :return: The email of this PasswordResetSpec. 
         :rtype: str
         """
-        return self._name
+        return self._email
 
-    @name.setter
-    def name(self, name):
+    @email.setter
+    def email(self, email):
         """
-        Name of the leaf.
+        Email address registered for user requesting reset.
 
-        :param name: The name of this LeafUpdate.
+        :param email: The email of this PasswordResetSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and email is None:  # noqa: E501
+            raise ValueError("Invalid value for `email`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._email = email
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -126,18 +101,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LeafUpdate):
+        if not isinstance(other, PasswordResetSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LeafUpdate):
+        if not isinstance(other, PasswordResetSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/localization.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/localization.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,109 +27,127 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'attributes': 'dict(str, object)',
+        'created_by': 'int',
         'created_datetime': 'datetime',
+        'elemental_id': 'str',
         'frame': 'int',
         'height': 'float',
         'id': 'int',
         'media': 'int',
-        'meta': 'int',
         'modified_by': 'int',
         'modified_datetime': 'datetime',
         'parent': 'float',
+        'points': 'list[list[float]]',
         'project': 'int',
         'thumbnail_image': 'str',
+        'type': 'int',
         'u': 'float',
         'user': 'int',
         'v': 'float',
+        'variant_deleted': 'bool',
         'version': 'int',
         'width': 'float',
         'x': 'float',
         'y': 'float'
     }
 
     attribute_map = {
         'attributes': 'attributes',
+        'created_by': 'created_by',
         'created_datetime': 'created_datetime',
+        'elemental_id': 'elemental_id',
         'frame': 'frame',
         'height': 'height',
         'id': 'id',
         'media': 'media',
-        'meta': 'meta',
         'modified_by': 'modified_by',
         'modified_datetime': 'modified_datetime',
         'parent': 'parent',
+        'points': 'points',
         'project': 'project',
         'thumbnail_image': 'thumbnail_image',
+        'type': 'type',
         'u': 'u',
         'user': 'user',
         'v': 'v',
+        'variant_deleted': 'variant_deleted',
         'version': 'version',
         'width': 'width',
         'x': 'x',
         'y': 'y'
     }
 
-    def __init__(self, attributes=None, created_datetime=None, frame=None, height=None, id=None, media=None, meta=None, modified_by=None, modified_datetime=None, parent=None, project=None, thumbnail_image=None, u=None, user=None, v=None, version=None, width=None, x=None, y=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, created_by=None, created_datetime=None, elemental_id=None, frame=None, height=None, id=None, media=None, modified_by=None, modified_datetime=None, parent=None, points=None, project=None, thumbnail_image=None, type=None, u=None, user=None, v=None, variant_deleted=None, version=None, width=None, x=None, y=None, local_vars_configuration=None):  # noqa: E501
         """Localization - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
+        self._created_by = None
         self._created_datetime = None
+        self._elemental_id = None
         self._frame = None
         self._height = None
         self._id = None
         self._media = None
-        self._meta = None
         self._modified_by = None
         self._modified_datetime = None
         self._parent = None
+        self._points = None
         self._project = None
         self._thumbnail_image = None
+        self._type = None
         self._u = None
         self._user = None
         self._v = None
+        self._variant_deleted = None
         self._version = None
         self._width = None
         self._x = None
         self._y = None
         self.discriminator = None
 
         if attributes is not None:
             self.attributes = attributes
+        if created_by is not None:
+            self.created_by = created_by
         if created_datetime is not None:
             self.created_datetime = created_datetime
+        self.elemental_id = elemental_id
         if frame is not None:
             self.frame = frame
         self.height = height
         if id is not None:
             self.id = id
         if media is not None:
             self.media = media
-        if meta is not None:
-            self.meta = meta
         if modified_by is not None:
             self.modified_by = modified_by
         if modified_datetime is not None:
             self.modified_datetime = modified_datetime
         self.parent = parent
+        self.points = points
         if project is not None:
             self.project = project
         if thumbnail_image is not None:
             self.thumbnail_image = thumbnail_image
+        if type is not None:
+            self.type = type
         self.u = u
         if user is not None:
             self.user = user
         self.v = v
+        if variant_deleted is not None:
+            self.variant_deleted = variant_deleted
         if version is not None:
             self.version = version
         self.width = width
         self.x = x
         self.y = y
 
     @property
@@ -150,14 +168,35 @@
         :param attributes: The attributes of this Localization.
         :type: dict(str, object)
         """
 
         self._attributes = attributes
 
     @property
+    def created_by(self):
+        """
+        Unique integer identifying the user who created this localization.
+
+        :return: The created_by of this Localization. 
+        :rtype: int
+        """
+        return self._created_by
+
+    @created_by.setter
+    def created_by(self, created_by):
+        """
+        Unique integer identifying the user who created this localization.
+
+        :param created_by: The created_by of this Localization.
+        :type: int
+        """
+
+        self._created_by = created_by
+
+    @property
     def created_datetime(self):
         """
         Datetime this localization was created.
 
         :return: The created_datetime of this Localization. 
         :rtype: datetime
         """
@@ -171,14 +210,35 @@
         :param created_datetime: The created_datetime of this Localization.
         :type: datetime
         """
 
         self._created_datetime = created_datetime
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this Localization. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this Localization.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def frame(self):
         """
         Frame number of this localization if it is in a video.
 
         :return: The frame of this Localization. 
         :rtype: int
         """
@@ -261,35 +321,14 @@
         :param media: The media of this Localization.
         :type: int
         """
 
         self._media = media
 
     @property
-    def meta(self):
-        """
-        Unique integer identifying entity type of this localization.
-
-        :return: The meta of this Localization. 
-        :rtype: int
-        """
-        return self._meta
-
-    @meta.setter
-    def meta(self, meta):
-        """
-        Unique integer identifying entity type of this localization.
-
-        :param meta: The meta of this Localization.
-        :type: int
-        """
-
-        self._meta = meta
-
-    @property
     def modified_by(self):
         """
         Unique integer identifying the user who last modified this localization.
 
         :return: The modified_by of this Localization. 
         :rtype: int
         """
@@ -345,14 +384,35 @@
         :param parent: The parent of this Localization.
         :type: float
         """
 
         self._parent = parent
 
     @property
+    def points(self):
+        """
+        List of normalized [x, y] pairs for `poly` localization types.
+
+        :return: The points of this Localization. 
+        :rtype: list[list[float]]
+        """
+        return self._points
+
+    @points.setter
+    def points(self, points):
+        """
+        List of normalized [x, y] pairs for `poly` localization types.
+
+        :param points: The points of this Localization.
+        :type: list[list[float]]
+        """
+
+        self._points = points
+
+    @property
     def project(self):
         """
         Unique integer identifying project of this localization.
 
         :return: The project of this Localization. 
         :rtype: int
         """
@@ -387,14 +447,35 @@
         :param thumbnail_image: The thumbnail_image of this Localization.
         :type: str
         """
 
         self._thumbnail_image = thumbnail_image
 
     @property
+    def type(self):
+        """
+        Unique integer identifying entity type of this localization.
+
+        :return: The type of this Localization. 
+        :rtype: int
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """
+        Unique integer identifying entity type of this localization.
+
+        :param type: The type of this Localization.
+        :type: int
+        """
+
+        self._type = type
+
+    @property
     def u(self):
         """
         Horizontal vector component for `line` localization types.
 
         :return: The u of this Localization. 
         :rtype: float
         """
@@ -462,14 +543,35 @@
         if (self.local_vars_configuration.client_side_validation and
                 v is not None and v < -1.0):  # noqa: E501
             raise ValueError("Invalid value for `v`, must be a value greater than or equal to `-1.0`")  # noqa: E501
 
         self._v = v
 
     @property
+    def variant_deleted(self):
+        """
+        Unique integer identifying the user who created this localization.
+
+        :return: The variant_deleted of this Localization. 
+        :rtype: bool
+        """
+        return self._variant_deleted
+
+    @variant_deleted.setter
+    def variant_deleted(self, variant_deleted):
+        """
+        Unique integer identifying the user who created this localization.
+
+        :param variant_deleted: The variant_deleted of this Localization.
+        :type: bool
+        """
+
+        self._variant_deleted = variant_deleted
+
+    @property
     def version(self):
         """
         Unique integer identifying a version.
 
         :return: The version of this Localization. 
         :rtype: int
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/localization_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/localization_spec.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,74 +26,134 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'attributes': 'dict(str, object)',
+        'elemental_id': 'str',
         'frame': 'int',
         'height': 'float',
         'media_id': 'int',
         'parent': 'float',
+        'points': 'list[list[float]]',
         'type': 'int',
         'u': 'float',
+        'user_elemental_id': 'str',
         'v': 'float',
         'version': 'int',
         'width': 'float',
         'x': 'float',
         'y': 'float'
     }
 
     attribute_map = {
+        'attributes': 'attributes',
+        'elemental_id': 'elemental_id',
         'frame': 'frame',
         'height': 'height',
         'media_id': 'media_id',
         'parent': 'parent',
+        'points': 'points',
         'type': 'type',
         'u': 'u',
+        'user_elemental_id': 'user_elemental_id',
         'v': 'v',
         'version': 'version',
         'width': 'width',
         'x': 'x',
         'y': 'y'
     }
 
-    def __init__(self, frame=None, height=None, media_id=None, parent=None, type=None, u=None, v=None, version=None, width=None, x=None, y=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, elemental_id=None, frame=None, height=None, media_id=None, parent=None, points=None, type=None, u=None, user_elemental_id=None, v=None, version=None, width=None, x=None, y=None, local_vars_configuration=None):  # noqa: E501
         """LocalizationSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._attributes = None
+        self._elemental_id = None
         self._frame = None
         self._height = None
         self._media_id = None
         self._parent = None
+        self._points = None
         self._type = None
         self._u = None
+        self._user_elemental_id = None
         self._v = None
         self._version = None
         self._width = None
         self._x = None
         self._y = None
         self.discriminator = None
 
+        if attributes is not None:
+            self.attributes = attributes
+        self.elemental_id = elemental_id
         self.frame = frame
         self.height = height
         self.media_id = media_id
         self.parent = parent
+        self.points = points
         self.type = type
         self.u = u
+        if user_elemental_id is not None:
+            self.user_elemental_id = user_elemental_id
         self.v = v
         if version is not None:
             self.version = version
         self.width = width
         self.x = x
         self.y = y
 
     @property
+    def attributes(self):
+        """
+        Object containing attribute values.
+
+        :return: The attributes of this LocalizationSpec. 
+        :rtype: dict(str, object)
+        """
+        return self._attributes
+
+    @attributes.setter
+    def attributes(self, attributes):
+        """
+        Object containing attribute values.
+
+        :param attributes: The attributes of this LocalizationSpec.
+        :type: dict(str, object)
+        """
+
+        self._attributes = attributes
+
+    @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this LocalizationSpec. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this LocalizationSpec.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def frame(self):
         """
         Frame number of this localization if it is in a video.
 
         :return: The frame of this LocalizationSpec. 
         :rtype: int
         """
@@ -180,14 +240,35 @@
         :param parent: The parent of this LocalizationSpec.
         :type: float
         """
 
         self._parent = parent
 
     @property
+    def points(self):
+        """
+        List of normalized [x, y] pairs for `poly` localization types.
+
+        :return: The points of this LocalizationSpec. 
+        :rtype: list[list[float]]
+        """
+        return self._points
+
+    @points.setter
+    def points(self, points):
+        """
+        List of normalized [x, y] pairs for `poly` localization types.
+
+        :param points: The points of this LocalizationSpec.
+        :type: list[list[float]]
+        """
+
+        self._points = points
+
+    @property
     def type(self):
         """
         Unique integer identifying a localization type.
 
         :return: The type of this LocalizationSpec. 
         :rtype: int
         """
@@ -230,14 +311,35 @@
         if (self.local_vars_configuration.client_side_validation and
                 u is not None and u < -1.0):  # noqa: E501
             raise ValueError("Invalid value for `u`, must be a value greater than or equal to `-1.0`")  # noqa: E501
 
         self._u = u
 
     @property
+    def user_elemental_id(self):
+        """
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
+
+        :return: The user_elemental_id of this LocalizationSpec. 
+        :rtype: str
+        """
+        return self._user_elemental_id
+
+    @user_elemental_id.setter
+    def user_elemental_id(self, user_elemental_id):
+        """
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
+
+        :param user_elemental_id: The user_elemental_id of this LocalizationSpec.
+        :type: str
+        """
+
+        self._user_elemental_id = user_elemental_id
+
+    @property
     def v(self):
         """
         Vertical vector component for `line` localization types.
 
         :return: The v of this LocalizationSpec. 
         :rtype: float
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/localization_type.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/localization_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,65 +29,73 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'attribute_types': 'list[AttributeType]',
         'color_map': 'ColorMap',
         'description': 'str',
+        'drawable': 'bool',
         'dtype': 'str',
+        'elemental_id': 'str',
         'grouping_default': 'bool',
         'id': 'int',
         'line_width': 'int',
         'media': 'list[int]',
         'name': 'str',
         'project': 'int',
         'visible': 'bool'
     }
 
     attribute_map = {
         'attribute_types': 'attribute_types',
-        'color_map': 'colorMap',
+        'color_map': 'color_map',
         'description': 'description',
+        'drawable': 'drawable',
         'dtype': 'dtype',
+        'elemental_id': 'elemental_id',
         'grouping_default': 'grouping_default',
         'id': 'id',
         'line_width': 'line_width',
         'media': 'media',
         'name': 'name',
         'project': 'project',
         'visible': 'visible'
     }
 
-    def __init__(self, attribute_types=None, color_map=None, description=None, dtype=None, grouping_default=True, id=None, line_width=None, media=None, name=None, project=None, visible=True, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attribute_types=None, color_map=None, description=None, drawable=True, dtype=None, elemental_id=None, grouping_default=True, id=None, line_width=None, media=None, name=None, project=None, visible=True, local_vars_configuration=None):  # noqa: E501
         """LocalizationType - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attribute_types = None
         self._color_map = None
         self._description = None
+        self._drawable = None
         self._dtype = None
+        self._elemental_id = None
         self._grouping_default = None
         self._id = None
         self._line_width = None
         self._media = None
         self._name = None
         self._project = None
         self._visible = None
         self.discriminator = None
 
         if attribute_types is not None:
             self.attribute_types = attribute_types
-        if color_map is not None:
-            self.color_map = color_map
+        self.color_map = color_map
         if description is not None:
             self.description = description
+        if drawable is not None:
+            self.drawable = drawable
         if dtype is not None:
             self.dtype = dtype
+        self.elemental_id = elemental_id
         if grouping_default is not None:
             self.grouping_default = grouping_default
         if id is not None:
             self.id = id
         if line_width is not None:
             self.line_width = line_width
         if media is not None:
@@ -157,14 +165,35 @@
         :param description: The description of this LocalizationType.
         :type: str
         """
 
         self._description = description
 
     @property
+    def drawable(self):
+        """
+        Whether this type can be drawn in the UI. Must also be visible.
+
+        :return: The drawable of this LocalizationType. 
+        :rtype: bool
+        """
+        return self._drawable
+
+    @drawable.setter
+    def drawable(self, drawable):
+        """
+        Whether this type can be drawn in the UI. Must also be visible.
+
+        :param drawable: The drawable of this LocalizationType.
+        :type: bool
+        """
+
+        self._drawable = drawable
+
+    @property
     def dtype(self):
         """
         Shape of this localization type.
 
         :return: The dtype of this LocalizationType. 
         :rtype: str
         """
@@ -174,24 +203,45 @@
     def dtype(self, dtype):
         """
         Shape of this localization type.
 
         :param dtype: The dtype of this LocalizationType.
         :type: str
         """
-        allowed_values = ["box", "line", "dot"]  # noqa: E501
+        allowed_values = ["box", "line", "dot", "poly"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and dtype not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `dtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(dtype, allowed_values)
             )
 
         self._dtype = dtype
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this LocalizationType. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this LocalizationType.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def grouping_default(self):
         """
         Whether to group elements in the UI by default.
 
         :return: The grouping_default of this LocalizationType. 
         :rtype: bool
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/localization_type_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state_spec.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,283 +14,273 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class LocalizationTypeSpec(object):
+class StateSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'attribute_types': 'list[AttributeType]',
-        'color_map': 'ColorMap',
-        'description': 'str',
-        'dtype': 'str',
-        'grouping_default': 'bool',
-        'line_width': 'int',
-        'media_types': 'list[int]',
-        'name': 'str',
-        'visible': 'bool'
+        'attributes': 'dict(str, object)',
+        'elemental_id': 'str',
+        'frame': 'int',
+        'localization_ids': 'list[int]',
+        'media_ids': 'list[int]',
+        'parent': 'float',
+        'type': 'int',
+        'user_elemental_id': 'str',
+        'version': 'int'
     }
 
     attribute_map = {
-        'attribute_types': 'attribute_types',
-        'color_map': 'colorMap',
-        'description': 'description',
-        'dtype': 'dtype',
-        'grouping_default': 'grouping_default',
-        'line_width': 'line_width',
-        'media_types': 'media_types',
-        'name': 'name',
-        'visible': 'visible'
+        'attributes': 'attributes',
+        'elemental_id': 'elemental_id',
+        'frame': 'frame',
+        'localization_ids': 'localization_ids',
+        'media_ids': 'media_ids',
+        'parent': 'parent',
+        'type': 'type',
+        'user_elemental_id': 'user_elemental_id',
+        'version': 'version'
     }
 
-    def __init__(self, attribute_types=None, color_map=None, description=None, dtype=None, grouping_default=True, line_width=None, media_types=None, name=None, visible=True, local_vars_configuration=None):  # noqa: E501
-        """LocalizationTypeSpec - a model defined in OpenAPI"""
+    def __init__(self, attributes=None, elemental_id=None, frame=None, localization_ids=None, media_ids=None, parent=None, type=None, user_elemental_id=None, version=None, local_vars_configuration=None):  # noqa: E501
+        """StateSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._attribute_types = None
-        self._color_map = None
-        self._description = None
-        self._dtype = None
-        self._grouping_default = None
-        self._line_width = None
-        self._media_types = None
-        self._name = None
-        self._visible = None
+        self._attributes = None
+        self._elemental_id = None
+        self._frame = None
+        self._localization_ids = None
+        self._media_ids = None
+        self._parent = None
+        self._type = None
+        self._user_elemental_id = None
+        self._version = None
         self.discriminator = None
 
-        if attribute_types is not None:
-            self.attribute_types = attribute_types
-        if color_map is not None:
-            self.color_map = color_map
-        if description is not None:
-            self.description = description
-        self.dtype = dtype
-        if grouping_default is not None:
-            self.grouping_default = grouping_default
-        if line_width is not None:
-            self.line_width = line_width
-        self.media_types = media_types
-        self.name = name
-        if visible is not None:
-            self.visible = visible
+        if attributes is not None:
+            self.attributes = attributes
+        self.elemental_id = elemental_id
+        if frame is not None:
+            self.frame = frame
+        if localization_ids is not None:
+            self.localization_ids = localization_ids
+        self.media_ids = media_ids
+        self.parent = parent
+        self.type = type
+        if user_elemental_id is not None:
+            self.user_elemental_id = user_elemental_id
+        if version is not None:
+            self.version = version
 
     @property
-    def attribute_types(self):
+    def attributes(self):
         """
-        Attribute type definitions.
+        Object containing attribute values.
 
-        :return: The attribute_types of this LocalizationTypeSpec. 
-        :rtype: list[AttributeType]
+        :return: The attributes of this StateSpec. 
+        :rtype: dict(str, object)
         """
-        return self._attribute_types
+        return self._attributes
 
-    @attribute_types.setter
-    def attribute_types(self, attribute_types):
+    @attributes.setter
+    def attributes(self, attributes):
         """
-        Attribute type definitions.
+        Object containing attribute values.
 
-        :param attribute_types: The attribute_types of this LocalizationTypeSpec.
-        :type: list[AttributeType]
+        :param attributes: The attributes of this StateSpec.
+        :type: dict(str, object)
         """
 
-        self._attribute_types = attribute_types
+        self._attributes = attributes
 
     @property
-    def color_map(self):
+    def elemental_id(self):
         """
+        The elemental ID of the object.
 
-        :return: The color_map of this LocalizationTypeSpec. 
-        :rtype: ColorMap
+        :return: The elemental_id of this StateSpec. 
+        :rtype: str
         """
-        return self._color_map
+        return self._elemental_id
 
-    @color_map.setter
-    def color_map(self, color_map):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
+        The elemental ID of the object.
 
-        :param color_map: The color_map of this LocalizationTypeSpec.
-        :type: ColorMap
+        :param elemental_id: The elemental_id of this StateSpec.
+        :type: str
         """
 
-        self._color_map = color_map
+        self._elemental_id = elemental_id
 
     @property
-    def description(self):
+    def frame(self):
         """
-        Description of the localization type.
+        Frame number this state applies to.
 
-        :return: The description of this LocalizationTypeSpec. 
-        :rtype: str
+        :return: The frame of this StateSpec. 
+        :rtype: int
         """
-        return self._description
+        return self._frame
 
-    @description.setter
-    def description(self, description):
+    @frame.setter
+    def frame(self, frame):
         """
-        Description of the localization type.
+        Frame number this state applies to.
 
-        :param description: The description of this LocalizationTypeSpec.
-        :type: str
+        :param frame: The frame of this StateSpec.
+        :type: int
         """
 
-        self._description = description
+        self._frame = frame
 
     @property
-    def dtype(self):
+    def localization_ids(self):
         """
-        Shape of this localization type.
+        List of localization IDs that this state applies to.
 
-        :return: The dtype of this LocalizationTypeSpec. 
-        :rtype: str
+        :return: The localization_ids of this StateSpec. 
+        :rtype: list[int]
         """
-        return self._dtype
+        return self._localization_ids
 
-    @dtype.setter
-    def dtype(self, dtype):
+    @localization_ids.setter
+    def localization_ids(self, localization_ids):
         """
-        Shape of this localization type.
+        List of localization IDs that this state applies to.
 
-        :param dtype: The dtype of this LocalizationTypeSpec.
-        :type: str
+        :param localization_ids: The localization_ids of this StateSpec.
+        :type: list[int]
         """
-        if self.local_vars_configuration.client_side_validation and dtype is None:  # noqa: E501
-            raise ValueError("Invalid value for `dtype`, must not be `None`")  # noqa: E501
-        allowed_values = ["box", "line", "dot"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and dtype not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `dtype` ({0}), must be one of {1}"  # noqa: E501
-                .format(dtype, allowed_values)
-            )
 
-        self._dtype = dtype
+        self._localization_ids = localization_ids
 
     @property
-    def grouping_default(self):
+    def media_ids(self):
         """
-        Whether to group elements in the UI by default.
+        List of media IDs that this state applies to.
 
-        :return: The grouping_default of this LocalizationTypeSpec. 
-        :rtype: bool
+        :return: The media_ids of this StateSpec. 
+        :rtype: list[int]
         """
-        return self._grouping_default
+        return self._media_ids
 
-    @grouping_default.setter
-    def grouping_default(self, grouping_default):
+    @media_ids.setter
+    def media_ids(self, media_ids):
         """
-        Whether to group elements in the UI by default.
+        List of media IDs that this state applies to.
 
-        :param grouping_default: The grouping_default of this LocalizationTypeSpec.
-        :type: bool
+        :param media_ids: The media_ids of this StateSpec.
+        :type: list[int]
         """
+        if self.local_vars_configuration.client_side_validation and media_ids is None:  # noqa: E501
+            raise ValueError("Invalid value for `media_ids`, must not be `None`")  # noqa: E501
 
-        self._grouping_default = grouping_default
+        self._media_ids = media_ids
 
     @property
-    def line_width(self):
+    def parent(self):
         """
-        Width of the line used to draw the localization.
+        If a clone, the pk of the parent.
 
-        :return: The line_width of this LocalizationTypeSpec. 
-        :rtype: int
+        :return: The parent of this StateSpec. 
+        :rtype: float
         """
-        return self._line_width
+        return self._parent
 
-    @line_width.setter
-    def line_width(self, line_width):
+    @parent.setter
+    def parent(self, parent):
         """
-        Width of the line used to draw the localization.
+        If a clone, the pk of the parent.
 
-        :param line_width: The line_width of this LocalizationTypeSpec.
-        :type: int
+        :param parent: The parent of this StateSpec.
+        :type: float
         """
-        if (self.local_vars_configuration.client_side_validation and
-                line_width is not None and line_width < 1):  # noqa: E501
-            raise ValueError("Invalid value for `line_width`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._line_width = line_width
+        self._parent = parent
 
     @property
-    def media_types(self):
+    def type(self):
         """
-        List of integers identifying media types that this localization type may apply to.
+        Unique integer identifying a state type.
 
-        :return: The media_types of this LocalizationTypeSpec. 
-        :rtype: list[int]
+        :return: The type of this StateSpec. 
+        :rtype: int
         """
-        return self._media_types
+        return self._type
 
-    @media_types.setter
-    def media_types(self, media_types):
+    @type.setter
+    def type(self, type):
         """
-        List of integers identifying media types that this localization type may apply to.
+        Unique integer identifying a state type.
 
-        :param media_types: The media_types of this LocalizationTypeSpec.
-        :type: list[int]
+        :param type: The type of this StateSpec.
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and media_types is None:  # noqa: E501
-            raise ValueError("Invalid value for `media_types`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
-        self._media_types = media_types
+        self._type = type
 
     @property
-    def name(self):
+    def user_elemental_id(self):
         """
-        Name of the localization type.
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
 
-        :return: The name of this LocalizationTypeSpec. 
+        :return: The user_elemental_id of this StateSpec. 
         :rtype: str
         """
-        return self._name
+        return self._user_elemental_id
 
-    @name.setter
-    def name(self, name):
+    @user_elemental_id.setter
+    def user_elemental_id(self, user_elemental_id):
         """
-        Name of the localization type.
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
 
-        :param name: The name of this LocalizationTypeSpec.
+        :param user_elemental_id: The user_elemental_id of this StateSpec.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._user_elemental_id = user_elemental_id
 
     @property
-    def visible(self):
+    def version(self):
         """
-        Whether this type should be displayed in the UI.
+        Unique integer identifying the version.
 
-        :return: The visible of this LocalizationTypeSpec. 
-        :rtype: bool
+        :return: The version of this StateSpec. 
+        :rtype: int
         """
-        return self._visible
+        return self._version
 
-    @visible.setter
-    def visible(self, visible):
+    @version.setter
+    def version(self, version):
         """
-        Whether this type should be displayed in the UI.
+        Unique integer identifying the version.
 
-        :param visible: The visible of this LocalizationTypeSpec.
-        :type: bool
+        :param version: The version of this StateSpec.
+        :type: int
         """
 
-        self._visible = visible
+        self._version = version
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -318,18 +308,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LocalizationTypeSpec):
+        if not isinstance(other, StateSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LocalizationTypeSpec):
+        if not isinstance(other, StateSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/localization_type_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state_type_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,192 +14,190 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class LocalizationTypeUpdate(object):
+class StateTypeUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'color_map': 'ColorMap',
+        'delete_child_localizations': 'bool',
         'description': 'str',
+        'elemental_id': 'str',
         'grouping_default': 'bool',
-        'line_width': 'int',
         'name': 'str',
         'visible': 'bool'
     }
 
     attribute_map = {
-        'color_map': 'colorMap',
+        'delete_child_localizations': 'delete_child_localizations',
         'description': 'description',
+        'elemental_id': 'elemental_id',
         'grouping_default': 'grouping_default',
-        'line_width': 'line_width',
         'name': 'name',
         'visible': 'visible'
     }
 
-    def __init__(self, color_map=None, description=None, grouping_default=True, line_width=None, name=None, visible=True, local_vars_configuration=None):  # noqa: E501
-        """LocalizationTypeUpdate - a model defined in OpenAPI"""
+    def __init__(self, delete_child_localizations=None, description=None, elemental_id=None, grouping_default=None, name=None, visible=None, local_vars_configuration=None):  # noqa: E501
+        """StateTypeUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._color_map = None
+        self._delete_child_localizations = None
         self._description = None
+        self._elemental_id = None
         self._grouping_default = None
-        self._line_width = None
         self._name = None
         self._visible = None
         self.discriminator = None
 
-        if color_map is not None:
-            self.color_map = color_map
+        if delete_child_localizations is not None:
+            self.delete_child_localizations = delete_child_localizations
         if description is not None:
             self.description = description
+        self.elemental_id = elemental_id
         if grouping_default is not None:
             self.grouping_default = grouping_default
-        if line_width is not None:
-            self.line_width = line_width
         if name is not None:
             self.name = name
         if visible is not None:
             self.visible = visible
 
     @property
-    def color_map(self):
+    def delete_child_localizations(self):
         """
+        True if child localizations should be deleted when this state is deleted. Localizations will only be deleted if they are not associated with another state. 
 
-        :return: The color_map of this LocalizationTypeUpdate. 
-        :rtype: ColorMap
+        :return: The delete_child_localizations of this StateTypeUpdate. 
+        :rtype: bool
         """
-        return self._color_map
+        return self._delete_child_localizations
 
-    @color_map.setter
-    def color_map(self, color_map):
+    @delete_child_localizations.setter
+    def delete_child_localizations(self, delete_child_localizations):
         """
+        True if child localizations should be deleted when this state is deleted. Localizations will only be deleted if they are not associated with another state. 
 
-        :param color_map: The color_map of this LocalizationTypeUpdate.
-        :type: ColorMap
+        :param delete_child_localizations: The delete_child_localizations of this StateTypeUpdate.
+        :type: bool
         """
 
-        self._color_map = color_map
+        self._delete_child_localizations = delete_child_localizations
 
     @property
     def description(self):
         """
-        Description of the localization type.
+        Description of the state type.
 
-        :return: The description of this LocalizationTypeUpdate. 
+        :return: The description of this StateTypeUpdate. 
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
-        Description of the localization type.
+        Description of the state type.
 
-        :param description: The description of this LocalizationTypeUpdate.
+        :param description: The description of this StateTypeUpdate.
         :type: str
         """
 
         self._description = description
 
     @property
-    def grouping_default(self):
+    def elemental_id(self):
         """
-        Whether to group elements in the UI by default.
+        The elemental ID of the object.
 
-        :return: The grouping_default of this LocalizationTypeUpdate. 
-        :rtype: bool
+        :return: The elemental_id of this StateTypeUpdate. 
+        :rtype: str
         """
-        return self._grouping_default
+        return self._elemental_id
 
-    @grouping_default.setter
-    def grouping_default(self, grouping_default):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        Whether to group elements in the UI by default.
+        The elemental ID of the object.
 
-        :param grouping_default: The grouping_default of this LocalizationTypeUpdate.
-        :type: bool
+        :param elemental_id: The elemental_id of this StateTypeUpdate.
+        :type: str
         """
 
-        self._grouping_default = grouping_default
+        self._elemental_id = elemental_id
 
     @property
-    def line_width(self):
+    def grouping_default(self):
         """
-        Width of the line used to draw the localization.
+        Whether to group elements in the UI by default.
 
-        :return: The line_width of this LocalizationTypeUpdate. 
-        :rtype: int
+        :return: The grouping_default of this StateTypeUpdate. 
+        :rtype: bool
         """
-        return self._line_width
+        return self._grouping_default
 
-    @line_width.setter
-    def line_width(self, line_width):
+    @grouping_default.setter
+    def grouping_default(self, grouping_default):
         """
-        Width of the line used to draw the localization.
+        Whether to group elements in the UI by default.
 
-        :param line_width: The line_width of this LocalizationTypeUpdate.
-        :type: int
+        :param grouping_default: The grouping_default of this StateTypeUpdate.
+        :type: bool
         """
-        if (self.local_vars_configuration.client_side_validation and
-                line_width is not None and line_width < 1):  # noqa: E501
-            raise ValueError("Invalid value for `line_width`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._line_width = line_width
+        self._grouping_default = grouping_default
 
     @property
     def name(self):
         """
-        Name of the localization type.
+        Name of the state type.
 
-        :return: The name of this LocalizationTypeUpdate. 
+        :return: The name of this StateTypeUpdate. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Name of the localization type.
+        Name of the state type.
 
-        :param name: The name of this LocalizationTypeUpdate.
+        :param name: The name of this StateTypeUpdate.
         :type: str
         """
 
         self._name = name
 
     @property
     def visible(self):
         """
-        Whether this type should be displayed in the UI.
+        Whether this state type should be displayed.
 
-        :return: The visible of this LocalizationTypeUpdate. 
+        :return: The visible of this StateTypeUpdate. 
         :rtype: bool
         """
         return self._visible
 
     @visible.setter
     def visible(self, visible):
         """
-        Whether this type should be displayed in the UI.
+        Whether this state type should be displayed.
 
-        :param visible: The visible of this LocalizationTypeUpdate.
+        :param visible: The visible of this StateTypeUpdate.
         :type: bool
         """
 
         self._visible = visible
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -231,18 +229,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LocalizationTypeUpdate):
+        if not isinstance(other, StateTypeUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LocalizationTypeUpdate):
+        if not isinstance(other, StateTypeUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/localization_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/localization_update.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,60 +27,83 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'attributes': 'dict(str, object)',
+        'elemental_id': 'str',
         'frame': 'int',
         'height': 'float',
+        'null_attributes': 'list[str]',
         'parent': 'float',
+        'points': 'list[list[float]]',
+        'reset_attributes': 'list[str]',
         'u': 'float',
+        'user_elemental_id': 'str',
         'v': 'float',
         'width': 'float',
         'x': 'float',
         'y': 'float'
     }
 
     attribute_map = {
         'attributes': 'attributes',
+        'elemental_id': 'elemental_id',
         'frame': 'frame',
         'height': 'height',
+        'null_attributes': 'null_attributes',
         'parent': 'parent',
+        'points': 'points',
+        'reset_attributes': 'reset_attributes',
         'u': 'u',
+        'user_elemental_id': 'user_elemental_id',
         'v': 'v',
         'width': 'width',
         'x': 'x',
         'y': 'y'
     }
 
-    def __init__(self, attributes=None, frame=None, height=None, parent=None, u=None, v=None, width=None, x=None, y=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, elemental_id=None, frame=None, height=None, null_attributes=None, parent=None, points=None, reset_attributes=None, u=None, user_elemental_id=None, v=None, width=None, x=None, y=None, local_vars_configuration=None):  # noqa: E501
         """LocalizationUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
+        self._elemental_id = None
         self._frame = None
         self._height = None
+        self._null_attributes = None
         self._parent = None
+        self._points = None
+        self._reset_attributes = None
         self._u = None
+        self._user_elemental_id = None
         self._v = None
         self._width = None
         self._x = None
         self._y = None
         self.discriminator = None
 
         if attributes is not None:
             self.attributes = attributes
+        self.elemental_id = elemental_id
         if frame is not None:
             self.frame = frame
         self.height = height
+        if null_attributes is not None:
+            self.null_attributes = null_attributes
         self.parent = parent
+        self.points = points
+        if reset_attributes is not None:
+            self.reset_attributes = reset_attributes
         self.u = u
+        if user_elemental_id is not None:
+            self.user_elemental_id = user_elemental_id
         self.v = v
         self.width = width
         self.x = x
         self.y = y
 
     @property
     def attributes(self):
@@ -100,14 +123,35 @@
         :param attributes: The attributes of this LocalizationUpdate.
         :type: dict(str, object)
         """
 
         self._attributes = attributes
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this LocalizationUpdate. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this LocalizationUpdate.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def frame(self):
         """
         Frame number of this localization if it is in a video.
 
         :return: The frame of this LocalizationUpdate. 
         :rtype: int
         """
@@ -148,14 +192,35 @@
         if (self.local_vars_configuration.client_side_validation and
                 height is not None and height < 0.0):  # noqa: E501
             raise ValueError("Invalid value for `height`, must be a value greater than or equal to `0.0`")  # noqa: E501
 
         self._height = height
 
     @property
+    def null_attributes(self):
+        """
+        Null a value in the attributes body
+
+        :return: The null_attributes of this LocalizationUpdate. 
+        :rtype: list[str]
+        """
+        return self._null_attributes
+
+    @null_attributes.setter
+    def null_attributes(self, null_attributes):
+        """
+        Null a value in the attributes body
+
+        :param null_attributes: The null_attributes of this LocalizationUpdate.
+        :type: list[str]
+        """
+
+        self._null_attributes = null_attributes
+
+    @property
     def parent(self):
         """
         If a clone, the pk of the parent.
 
         :return: The parent of this LocalizationUpdate. 
         :rtype: float
         """
@@ -169,14 +234,56 @@
         :param parent: The parent of this LocalizationUpdate.
         :type: float
         """
 
         self._parent = parent
 
     @property
+    def points(self):
+        """
+        List of normalized [x, y] pairs for `poly` localization types.
+
+        :return: The points of this LocalizationUpdate. 
+        :rtype: list[list[float]]
+        """
+        return self._points
+
+    @points.setter
+    def points(self, points):
+        """
+        List of normalized [x, y] pairs for `poly` localization types.
+
+        :param points: The points of this LocalizationUpdate.
+        :type: list[list[float]]
+        """
+
+        self._points = points
+
+    @property
+    def reset_attributes(self):
+        """
+        Reset an attribute to the default value specified in the Type object
+
+        :return: The reset_attributes of this LocalizationUpdate. 
+        :rtype: list[str]
+        """
+        return self._reset_attributes
+
+    @reset_attributes.setter
+    def reset_attributes(self, reset_attributes):
+        """
+        Reset an attribute to the default value specified in the Type object
+
+        :param reset_attributes: The reset_attributes of this LocalizationUpdate.
+        :type: list[str]
+        """
+
+        self._reset_attributes = reset_attributes
+
+    @property
     def u(self):
         """
         Horizontal vector component for `line` localization types.
 
         :return: The u of this LocalizationUpdate. 
         :rtype: float
         """
@@ -196,14 +303,35 @@
         if (self.local_vars_configuration.client_side_validation and
                 u is not None and u < -1.0):  # noqa: E501
             raise ValueError("Invalid value for `u`, must be a value greater than or equal to `-1.0`")  # noqa: E501
 
         self._u = u
 
     @property
+    def user_elemental_id(self):
+        """
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
+
+        :return: The user_elemental_id of this LocalizationUpdate. 
+        :rtype: str
+        """
+        return self._user_elemental_id
+
+    @user_elemental_id.setter
+    def user_elemental_id(self, user_elemental_id):
+        """
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
+
+        :param user_elemental_id: The user_elemental_id of this LocalizationUpdate.
+        :type: str
+        """
+
+        self._user_elemental_id = user_elemental_id
+
+    @property
     def v(self):
         """
         Vertical vector component for `line` localization types.
 
         :return: The v of this LocalizationUpdate. 
         :rtype: float
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,95 +26,112 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'archive_state': 'str',
+        'archive_status_date': 'datetime',
         'attributes': 'dict(str, object)',
         'codec': 'str',
         'created_by': 'int',
         'created_datetime': 'str',
-        'fps': 'int',
+        'elemental_id': 'str',
+        'fps': 'float',
         'gid': 'str',
         'height': 'int',
         'id': 'int',
         'last_edit_end': 'datetime',
         'last_edit_start': 'datetime',
         'md5': 'str',
         'media_files': 'MediaFiles',
-        'meta': 'int',
         'modified_by': 'int',
         'modified_datetime': 'str',
         'name': 'str',
         'num_frames': 'int',
         'project': 'int',
+        'summary_level': 'int',
+        'type': 'int',
         'uid': 'str',
         'width': 'int'
     }
 
     attribute_map = {
+        'archive_state': 'archive_state',
+        'archive_status_date': 'archive_status_date',
         'attributes': 'attributes',
         'codec': 'codec',
         'created_by': 'created_by',
         'created_datetime': 'created_datetime',
+        'elemental_id': 'elemental_id',
         'fps': 'fps',
         'gid': 'gid',
         'height': 'height',
         'id': 'id',
         'last_edit_end': 'last_edit_end',
         'last_edit_start': 'last_edit_start',
         'md5': 'md5',
         'media_files': 'media_files',
-        'meta': 'meta',
         'modified_by': 'modified_by',
         'modified_datetime': 'modified_datetime',
         'name': 'name',
         'num_frames': 'num_frames',
         'project': 'project',
+        'summary_level': 'summary_level',
+        'type': 'type',
         'uid': 'uid',
         'width': 'width'
     }
 
-    def __init__(self, attributes=None, codec=None, created_by=None, created_datetime=None, fps=None, gid=None, height=None, id=None, last_edit_end=None, last_edit_start=None, md5=None, media_files=None, meta=None, modified_by=None, modified_datetime=None, name=None, num_frames=None, project=None, uid=None, width=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, archive_state=None, archive_status_date=None, attributes=None, codec=None, created_by=None, created_datetime=None, elemental_id=None, fps=None, gid=None, height=None, id=None, last_edit_end=None, last_edit_start=None, md5=None, media_files=None, modified_by=None, modified_datetime=None, name=None, num_frames=None, project=None, summary_level=None, type=None, uid=None, width=None, local_vars_configuration=None):  # noqa: E501
         """Media - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._archive_state = None
+        self._archive_status_date = None
         self._attributes = None
         self._codec = None
         self._created_by = None
         self._created_datetime = None
+        self._elemental_id = None
         self._fps = None
         self._gid = None
         self._height = None
         self._id = None
         self._last_edit_end = None
         self._last_edit_start = None
         self._md5 = None
         self._media_files = None
-        self._meta = None
         self._modified_by = None
         self._modified_datetime = None
         self._name = None
         self._num_frames = None
         self._project = None
+        self._summary_level = None
+        self._type = None
         self._uid = None
         self._width = None
         self.discriminator = None
 
+        if archive_state is not None:
+            self.archive_state = archive_state
+        if archive_status_date is not None:
+            self.archive_status_date = archive_status_date
         if attributes is not None:
             self.attributes = attributes
         if codec is not None:
             self.codec = codec
         if created_by is not None:
             self.created_by = created_by
         if created_datetime is not None:
             self.created_datetime = created_datetime
+        self.elemental_id = elemental_id
         if fps is not None:
             self.fps = fps
         if gid is not None:
             self.gid = gid
         if height is not None:
             self.height = height
         if id is not None:
@@ -123,32 +140,82 @@
             self.last_edit_end = last_edit_end
         if last_edit_start is not None:
             self.last_edit_start = last_edit_start
         if md5 is not None:
             self.md5 = md5
         if media_files is not None:
             self.media_files = media_files
-        if meta is not None:
-            self.meta = meta
         if modified_by is not None:
             self.modified_by = modified_by
         if modified_datetime is not None:
             self.modified_datetime = modified_datetime
         if name is not None:
             self.name = name
         if num_frames is not None:
             self.num_frames = num_frames
         if project is not None:
             self.project = project
+        if summary_level is not None:
+            self.summary_level = summary_level
+        if type is not None:
+            self.type = type
         if uid is not None:
             self.uid = uid
         if width is not None:
             self.width = width
 
     @property
+    def archive_state(self):
+        """
+        The current archival state of the media.
+
+        :return: The archive_state of this Media. 
+        :rtype: str
+        """
+        return self._archive_state
+
+    @archive_state.setter
+    def archive_state(self, archive_state):
+        """
+        The current archival state of the media.
+
+        :param archive_state: The archive_state of this Media.
+        :type: str
+        """
+        allowed_values = ["archived", "to_archive", "live", "to_live"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and archive_state not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `archive_state` ({0}), must be one of {1}"  # noqa: E501
+                .format(archive_state, allowed_values)
+            )
+
+        self._archive_state = archive_state
+
+    @property
+    def archive_status_date(self):
+        """
+        Datetime of the last change to the `archive_state` field.
+
+        :return: The archive_status_date of this Media. 
+        :rtype: datetime
+        """
+        return self._archive_status_date
+
+    @archive_status_date.setter
+    def archive_status_date(self, archive_status_date):
+        """
+        Datetime of the last change to the `archive_state` field.
+
+        :param archive_status_date: The archive_status_date of this Media.
+        :type: datetime
+        """
+
+        self._archive_status_date = archive_status_date
+
+    @property
     def attributes(self):
         """
         Object containing attribute values.
 
         :return: The attributes of this Media. 
         :rtype: dict(str, object)
         """
@@ -225,30 +292,51 @@
         :param created_datetime: The created_datetime of this Media.
         :type: str
         """
 
         self._created_datetime = created_datetime
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this Media. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this Media.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def fps(self):
         """
         Frame rate for videos.
 
         :return: The fps of this Media. 
-        :rtype: int
+        :rtype: float
         """
         return self._fps
 
     @fps.setter
     def fps(self, fps):
         """
         Frame rate for videos.
 
         :param fps: The fps of this Media.
-        :type: int
+        :type: float
         """
 
         self._fps = fps
 
     @property
     def gid(self):
         """
@@ -391,35 +479,14 @@
         :param media_files: The media_files of this Media.
         :type: MediaFiles
         """
 
         self._media_files = media_files
 
     @property
-    def meta(self):
-        """
-        Unique integer identifying entity type of this media.
-
-        :return: The meta of this Media. 
-        :rtype: int
-        """
-        return self._meta
-
-    @meta.setter
-    def meta(self, meta):
-        """
-        Unique integer identifying entity type of this media.
-
-        :param meta: The meta of this Media.
-        :type: int
-        """
-
-        self._meta = meta
-
-    @property
     def modified_by(self):
         """
         Unique integer identifying user who last modified this media.
 
         :return: The modified_by of this Media. 
         :rtype: int
         """
@@ -517,14 +584,56 @@
         :param project: The project of this Media.
         :type: int
         """
 
         self._project = project
 
     @property
+    def summary_level(self):
+        """
+        If supplied, this video is best summarized at this frame interval
+
+        :return: The summary_level of this Media. 
+        :rtype: int
+        """
+        return self._summary_level
+
+    @summary_level.setter
+    def summary_level(self, summary_level):
+        """
+        If supplied, this video is best summarized at this frame interval
+
+        :param summary_level: The summary_level of this Media.
+        :type: int
+        """
+
+        self._summary_level = summary_level
+
+    @property
+    def type(self):
+        """
+        Unique integer identifying entity type of this media.
+
+        :return: The type of this Media. 
+        :rtype: int
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """
+        Unique integer identifying entity type of this media.
+
+        :param type: The type of this Media.
+        :type: int
+        """
+
+        self._type = type
+
+    @property
     def uid(self):
         """
         Unique ID for the upload of this media.
 
         :return: The uid of this Media. 
         :rtype: str
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_files.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,63 +27,83 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'archival': 'list[VideoDefinition]',
+        'attachment': 'list[AuxiliaryFileDefinition]',
         'audio': 'list[AudioDefinition]',
+        'concat': 'list[ConcatDefinition]',
+        'frame_offset': 'list[int]',
         'ids': 'list[int]',
         'image': 'list[ImageDefinition]',
         'layout': 'list[int]',
+        'live': 'list[LiveDefinition]',
         'quality': 'int',
         'streaming': 'list[VideoDefinition]',
         'thumbnail': 'list[ImageDefinition]',
         'thumbnail_gif': 'list[ImageDefinition]'
     }
 
     attribute_map = {
         'archival': 'archival',
+        'attachment': 'attachment',
         'audio': 'audio',
+        'concat': 'concat',
+        'frame_offset': 'frameOffset',
         'ids': 'ids',
         'image': 'image',
         'layout': 'layout',
+        'live': 'live',
         'quality': 'quality',
         'streaming': 'streaming',
         'thumbnail': 'thumbnail',
         'thumbnail_gif': 'thumbnail_gif'
     }
 
-    def __init__(self, archival=None, audio=None, ids=None, image=None, layout=None, quality=None, streaming=None, thumbnail=None, thumbnail_gif=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, archival=None, attachment=None, audio=None, concat=None, frame_offset=None, ids=None, image=None, layout=None, live=None, quality=None, streaming=None, thumbnail=None, thumbnail_gif=None, local_vars_configuration=None):  # noqa: E501
         """MediaFiles - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._archival = None
+        self._attachment = None
         self._audio = None
+        self._concat = None
+        self._frame_offset = None
         self._ids = None
         self._image = None
         self._layout = None
+        self._live = None
         self._quality = None
         self._streaming = None
         self._thumbnail = None
         self._thumbnail_gif = None
         self.discriminator = None
 
         if archival is not None:
             self.archival = archival
+        if attachment is not None:
+            self.attachment = attachment
         if audio is not None:
             self.audio = audio
+        if concat is not None:
+            self.concat = concat
+        if frame_offset is not None:
+            self.frame_offset = frame_offset
         if ids is not None:
             self.ids = ids
         if image is not None:
             self.image = image
         if layout is not None:
             self.layout = layout
+        if live is not None:
+            self.live = live
         if quality is not None:
             self.quality = quality
         if streaming is not None:
             self.streaming = streaming
         if thumbnail is not None:
             self.thumbnail = thumbnail
         if thumbnail_gif is not None:
@@ -105,14 +125,33 @@
         :param archival: The archival of this MediaFiles.
         :type: list[VideoDefinition]
         """
 
         self._archival = archival
 
     @property
+    def attachment(self):
+        """
+
+        :return: The attachment of this MediaFiles. 
+        :rtype: list[AuxiliaryFileDefinition]
+        """
+        return self._attachment
+
+    @attachment.setter
+    def attachment(self, attachment):
+        """
+
+        :param attachment: The attachment of this MediaFiles.
+        :type: list[AuxiliaryFileDefinition]
+        """
+
+        self._attachment = attachment
+
+    @property
     def audio(self):
         """
 
         :return: The audio of this MediaFiles. 
         :rtype: list[AudioDefinition]
         """
         return self._audio
@@ -124,14 +163,54 @@
         :param audio: The audio of this MediaFiles.
         :type: list[AudioDefinition]
         """
 
         self._audio = audio
 
     @property
+    def concat(self):
+        """
+
+        :return: The concat of this MediaFiles. 
+        :rtype: list[ConcatDefinition]
+        """
+        return self._concat
+
+    @concat.setter
+    def concat(self, concat):
+        """
+
+        :param concat: The concat of this MediaFiles.
+        :type: list[ConcatDefinition]
+        """
+
+        self._concat = concat
+
+    @property
+    def frame_offset(self):
+        """
+        Frame of sub-video, offset from media in slot 0.
+
+        :return: The frame_offset of this MediaFiles. 
+        :rtype: list[int]
+        """
+        return self._frame_offset
+
+    @frame_offset.setter
+    def frame_offset(self, frame_offset):
+        """
+        Frame of sub-video, offset from media in slot 0.
+
+        :param frame_offset: The frame_offset of this MediaFiles.
+        :type: list[int]
+        """
+
+        self._frame_offset = frame_offset
+
+    @property
     def ids(self):
         """
         If multi-stream list of ids of sub-videos
 
         :return: The ids of this MediaFiles. 
         :rtype: list[int]
         """
@@ -185,14 +264,33 @@
         :param layout: The layout of this MediaFiles.
         :type: list[int]
         """
 
         self._layout = layout
 
     @property
+    def live(self):
+        """
+
+        :return: The live of this MediaFiles. 
+        :rtype: list[LiveDefinition]
+        """
+        return self._live
+
+    @live.setter
+    def live(self, live):
+        """
+
+        :param live: The live of this MediaFiles.
+        :type: list[LiveDefinition]
+        """
+
+        self._live = live
+
+    @property
     def quality(self):
         """
         Resolution to fetch on each sub-video
 
         :return: The quality of this MediaFiles. 
         :rtype: int
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_next.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_next.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_prev.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/token.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,66 +14,65 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class MediaPrev(object):
+class Token(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'prev': 'int'
+        'token': 'str'
     }
 
     attribute_map = {
-        'prev': 'prev'
+        'token': 'token'
     }
 
-    def __init__(self, prev=None, local_vars_configuration=None):  # noqa: E501
-        """MediaPrev - a model defined in OpenAPI"""
+    def __init__(self, token=None, local_vars_configuration=None):  # noqa: E501
+        """Token - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._prev = None
+        self._token = None
         self.discriminator = None
 
-        if prev is not None:
-            self.prev = prev
+        if token is not None:
+            self.token = token
 
     @property
-    def prev(self):
+    def token(self):
         """
+        API token.
 
-        :return: The prev of this MediaPrev. 
-        :rtype: int
+        :return: The token of this Token. 
+        :rtype: str
         """
-        return self._prev
+        return self._token
 
-    @prev.setter
-    def prev(self, prev):
+    @token.setter
+    def token(self, token):
         """
+        API token.
 
-        :param prev: The prev of this MediaPrev.
-        :type: int
+        :param token: The token of this Token.
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                prev is not None and prev < 0):  # noqa: E501
-            raise ValueError("Invalid value for `prev`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._prev = prev
+        self._token = token
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -101,18 +100,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MediaPrev):
+        if not isinstance(other, Token):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MediaPrev):
+        if not isinstance(other, Token):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,110 +26,125 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'attributes': 'object',
+        'attributes': 'dict(str, object)',
         'codec': 'str',
-        'fps': 'int',
+        'elemental_id': 'str',
+        'fps': 'float',
         'gid': 'str',
         'height': 'int',
         'md5': 'str',
         'name': 'str',
         'num_frames': 'int',
         'section': 'str',
+        'summary_level': 'int',
         'thumbnail_gif_url': 'str',
         'thumbnail_url': 'str',
         'type': 'int',
         'uid': 'str',
         'url': 'str',
+        'user_elemental_id': 'str',
         'width': 'int'
     }
 
     attribute_map = {
         'attributes': 'attributes',
         'codec': 'codec',
+        'elemental_id': 'elemental_id',
         'fps': 'fps',
         'gid': 'gid',
         'height': 'height',
         'md5': 'md5',
         'name': 'name',
         'num_frames': 'num_frames',
         'section': 'section',
+        'summary_level': 'summary_level',
         'thumbnail_gif_url': 'thumbnail_gif_url',
         'thumbnail_url': 'thumbnail_url',
         'type': 'type',
         'uid': 'uid',
         'url': 'url',
+        'user_elemental_id': 'user_elemental_id',
         'width': 'width'
     }
 
-    def __init__(self, attributes=None, codec=None, fps=None, gid=None, height=None, md5=None, name=None, num_frames=None, section=None, thumbnail_gif_url=None, thumbnail_url=None, type=None, uid=None, url=None, width=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, codec=None, elemental_id=None, fps=None, gid=None, height=None, md5=None, name=None, num_frames=None, section=None, summary_level=None, thumbnail_gif_url=None, thumbnail_url=None, type=None, uid=None, url=None, user_elemental_id=None, width=None, local_vars_configuration=None):  # noqa: E501
         """MediaSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
         self._codec = None
+        self._elemental_id = None
         self._fps = None
         self._gid = None
         self._height = None
         self._md5 = None
         self._name = None
         self._num_frames = None
         self._section = None
+        self._summary_level = None
         self._thumbnail_gif_url = None
         self._thumbnail_url = None
         self._type = None
         self._uid = None
         self._url = None
+        self._user_elemental_id = None
         self._width = None
         self.discriminator = None
 
         self.attributes = attributes
         self.codec = codec
+        if elemental_id is not None:
+            self.elemental_id = elemental_id
         self.fps = fps
         if gid is not None:
             self.gid = gid
         self.height = height
         self.md5 = md5
         self.name = name
         self.num_frames = num_frames
         self.section = section
+        if summary_level is not None:
+            self.summary_level = summary_level
         if thumbnail_gif_url is not None:
             self.thumbnail_gif_url = thumbnail_gif_url
         if thumbnail_url is not None:
             self.thumbnail_url = thumbnail_url
         self.type = type
         if uid is not None:
             self.uid = uid
         if url is not None:
             self.url = url
+        if user_elemental_id is not None:
+            self.user_elemental_id = user_elemental_id
         self.width = width
 
     @property
     def attributes(self):
         """
-        Attributes for the media
+        Object containing attribute values.
 
         :return: The attributes of this MediaSpec. 
-        :rtype: object
+        :rtype: dict(str, object)
         """
         return self._attributes
 
     @attributes.setter
     def attributes(self, attributes):
         """
-        Attributes for the media
+        Object containing attribute values.
 
         :param attributes: The attributes of this MediaSpec.
-        :type: object
+        :type: dict(str, object)
         """
 
         self._attributes = attributes
 
     @property
     def codec(self):
         """
@@ -148,30 +163,51 @@
         :param codec: The codec of this MediaSpec.
         :type: str
         """
 
         self._codec = codec
 
     @property
+    def elemental_id(self):
+        """
+        Unique ID of an element
+
+        :return: The elemental_id of this MediaSpec. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        Unique ID of an element
+
+        :param elemental_id: The elemental_id of this MediaSpec.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def fps(self):
         """
         Frame rate for videos.
 
         :return: The fps of this MediaSpec. 
-        :rtype: int
+        :rtype: float
         """
         return self._fps
 
     @fps.setter
     def fps(self, fps):
         """
         Frame rate for videos.
 
         :param fps: The fps of this MediaSpec.
-        :type: int
+        :type: float
         """
 
         self._fps = fps
 
     @property
     def gid(self):
         """
@@ -301,14 +337,35 @@
         """
         if self.local_vars_configuration.client_side_validation and section is None:  # noqa: E501
             raise ValueError("Invalid value for `section`, must not be `None`")  # noqa: E501
 
         self._section = section
 
     @property
+    def summary_level(self):
+        """
+        If supplied, this video is best summarized at this frame interval
+
+        :return: The summary_level of this MediaSpec. 
+        :rtype: int
+        """
+        return self._summary_level
+
+    @summary_level.setter
+    def summary_level(self, summary_level):
+        """
+        If supplied, this video is best summarized at this frame interval
+
+        :param summary_level: The summary_level of this MediaSpec.
+        :type: int
+        """
+
+        self._summary_level = summary_level
+
+    @property
     def thumbnail_gif_url(self):
         """
         Upload URL for the video gif thumbnail if already generated.
 
         :return: The thumbnail_gif_url of this MediaSpec. 
         :rtype: str
         """
@@ -392,33 +449,54 @@
         """
 
         self._uid = uid
 
     @property
     def url(self):
         """
-        Upload URL for the image if this is an image type. If not an image, this field is ignored.
+        Upload URL for the image if this is an image type, URL of hosted original media if this is a video type. For video types this field is just for reference.
 
         :return: The url of this MediaSpec. 
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
         """
-        Upload URL for the image if this is an image type. If not an image, this field is ignored.
+        Upload URL for the image if this is an image type, URL of hosted original media if this is a video type. For video types this field is just for reference.
 
         :param url: The url of this MediaSpec.
         :type: str
         """
 
         self._url = url
 
     @property
+    def user_elemental_id(self):
+        """
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
+
+        :return: The user_elemental_id of this MediaSpec. 
+        :rtype: str
+        """
+        return self._user_elemental_id
+
+    @user_elemental_id.setter
+    def user_elemental_id(self, user_elemental_id):
+        """
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
+
+        :param user_elemental_id: The user_elemental_id of this MediaSpec.
+        :type: str
+        """
+
+        self._user_elemental_id = user_elemental_id
+
+    @property
     def width(self):
         """
         Horizontal resolution in pixels.
 
         :return: The width of this MediaSpec. 
         :rtype: int
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_stats.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_stats.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_type.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_type_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,153 +14,228 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class MediaType(object):
+class MediaTypeSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'archive_config': 'list[ArchiveConfig]',
         'attribute_types': 'list[AttributeType]',
+        'default_box': 'int',
+        'default_dot': 'int',
+        'default_line': 'int',
         'default_volume': 'int',
         'description': 'str',
         'dtype': 'str',
+        'elemental_id': 'str',
         'file_format': 'str',
-        'id': 'int',
         'name': 'str',
         'overlay_config': 'dict(str, object)',
-        'project': 'int',
-        'streaming_config': 'list[ResolutionConfig]'
+        'streaming_config': 'list[ResolutionConfig]',
+        'visible': 'bool'
     }
 
     attribute_map = {
         'archive_config': 'archive_config',
         'attribute_types': 'attribute_types',
+        'default_box': 'default_box',
+        'default_dot': 'default_dot',
+        'default_line': 'default_line',
         'default_volume': 'default_volume',
         'description': 'description',
         'dtype': 'dtype',
+        'elemental_id': 'elemental_id',
         'file_format': 'file_format',
-        'id': 'id',
         'name': 'name',
         'overlay_config': 'overlay_config',
-        'project': 'project',
-        'streaming_config': 'streaming_config'
+        'streaming_config': 'streaming_config',
+        'visible': 'visible'
     }
 
-    def __init__(self, archive_config=None, attribute_types=None, default_volume=None, description='', dtype=None, file_format=None, id=None, name=None, overlay_config=None, project=None, streaming_config=None, local_vars_configuration=None):  # noqa: E501
-        """MediaType - a model defined in OpenAPI"""
+    def __init__(self, archive_config=None, attribute_types=None, default_box=None, default_dot=None, default_line=None, default_volume=None, description='', dtype=None, elemental_id=None, file_format=None, name=None, overlay_config=None, streaming_config=None, visible=None, local_vars_configuration=None):  # noqa: E501
+        """MediaTypeSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._archive_config = None
         self._attribute_types = None
+        self._default_box = None
+        self._default_dot = None
+        self._default_line = None
         self._default_volume = None
         self._description = None
         self._dtype = None
+        self._elemental_id = None
         self._file_format = None
-        self._id = None
         self._name = None
         self._overlay_config = None
-        self._project = None
         self._streaming_config = None
+        self._visible = None
         self.discriminator = None
 
         if archive_config is not None:
             self.archive_config = archive_config
         if attribute_types is not None:
             self.attribute_types = attribute_types
+        if default_box is not None:
+            self.default_box = default_box
+        if default_dot is not None:
+            self.default_dot = default_dot
+        if default_line is not None:
+            self.default_line = default_line
         if default_volume is not None:
             self.default_volume = default_volume
         if description is not None:
             self.description = description
-        if dtype is not None:
-            self.dtype = dtype
+        self.dtype = dtype
+        self.elemental_id = elemental_id
         if file_format is not None:
             self.file_format = file_format
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
+        self.name = name
         if overlay_config is not None:
             self.overlay_config = overlay_config
-        if project is not None:
-            self.project = project
         if streaming_config is not None:
             self.streaming_config = streaming_config
+        if visible is not None:
+            self.visible = visible
 
     @property
     def archive_config(self):
         """
         Archive config definitions. If null, the raw file will be uploaded to Tator.
 
-        :return: The archive_config of this MediaType. 
+        :return: The archive_config of this MediaTypeSpec. 
         :rtype: list[ArchiveConfig]
         """
         return self._archive_config
 
     @archive_config.setter
     def archive_config(self, archive_config):
         """
         Archive config definitions. If null, the raw file will be uploaded to Tator.
 
-        :param archive_config: The archive_config of this MediaType.
+        :param archive_config: The archive_config of this MediaTypeSpec.
         :type: list[ArchiveConfig]
         """
 
         self._archive_config = archive_config
 
     @property
     def attribute_types(self):
         """
         Attribute type definitions.
 
-        :return: The attribute_types of this MediaType. 
+        :return: The attribute_types of this MediaTypeSpec. 
         :rtype: list[AttributeType]
         """
         return self._attribute_types
 
     @attribute_types.setter
     def attribute_types(self, attribute_types):
         """
         Attribute type definitions.
 
-        :param attribute_types: The attribute_types of this MediaType.
+        :param attribute_types: The attribute_types of this MediaTypeSpec.
         :type: list[AttributeType]
         """
 
         self._attribute_types = attribute_types
 
     @property
+    def default_box(self):
+        """
+        Unique integer identifying default box type for drawing.
+
+        :return: The default_box of this MediaTypeSpec. 
+        :rtype: int
+        """
+        return self._default_box
+
+    @default_box.setter
+    def default_box(self, default_box):
+        """
+        Unique integer identifying default box type for drawing.
+
+        :param default_box: The default_box of this MediaTypeSpec.
+        :type: int
+        """
+
+        self._default_box = default_box
+
+    @property
+    def default_dot(self):
+        """
+        Unique integer identifying default dot type for drawing.
+
+        :return: The default_dot of this MediaTypeSpec. 
+        :rtype: int
+        """
+        return self._default_dot
+
+    @default_dot.setter
+    def default_dot(self, default_dot):
+        """
+        Unique integer identifying default dot type for drawing.
+
+        :param default_dot: The default_dot of this MediaTypeSpec.
+        :type: int
+        """
+
+        self._default_dot = default_dot
+
+    @property
+    def default_line(self):
+        """
+        Unique integer identifying default line type for drawing.
+
+        :return: The default_line of this MediaTypeSpec. 
+        :rtype: int
+        """
+        return self._default_line
+
+    @default_line.setter
+    def default_line(self, default_line):
+        """
+        Unique integer identifying default line type for drawing.
+
+        :param default_line: The default_line of this MediaTypeSpec.
+        :type: int
+        """
+
+        self._default_line = default_line
+
+    @property
     def default_volume(self):
         """
         Default audio volume for this media type.
 
-        :return: The default_volume of this MediaType. 
+        :return: The default_volume of this MediaTypeSpec. 
         :rtype: int
         """
         return self._default_volume
 
     @default_volume.setter
     def default_volume(self, default_volume):
         """
         Default audio volume for this media type.
 
-        :param default_volume: The default_volume of this MediaType.
+        :param default_volume: The default_volume of this MediaTypeSpec.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 default_volume is not None and default_volume > 100):  # noqa: E501
             raise ValueError("Invalid value for `default_volume`, must be a value less than or equal to `100`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 default_volume is not None and default_volume < 0):  # noqa: E501
@@ -169,185 +244,189 @@
         self._default_volume = default_volume
 
     @property
     def description(self):
         """
         Description of the media type.
 
-        :return: The description of this MediaType. 
+        :return: The description of this MediaTypeSpec. 
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
         Description of the media type.
 
-        :param description: The description of this MediaType.
+        :param description: The description of this MediaTypeSpec.
         :type: str
         """
 
         self._description = description
 
     @property
     def dtype(self):
         """
         Type of the media, image or video.
 
-        :return: The dtype of this MediaType. 
+        :return: The dtype of this MediaTypeSpec. 
         :rtype: str
         """
         return self._dtype
 
     @dtype.setter
     def dtype(self, dtype):
         """
         Type of the media, image or video.
 
-        :param dtype: The dtype of this MediaType.
+        :param dtype: The dtype of this MediaTypeSpec.
         :type: str
         """
-        allowed_values = ["image", "video", "multi"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and dtype is None:  # noqa: E501
+            raise ValueError("Invalid value for `dtype`, must not be `None`")  # noqa: E501
+        allowed_values = ["image", "video", "multi", "live"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and dtype not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `dtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(dtype, allowed_values)
             )
 
         self._dtype = dtype
 
     @property
-    def file_format(self):
+    def elemental_id(self):
         """
-        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
+        The elemental ID of the object.
 
-        :return: The file_format of this MediaType. 
+        :return: The elemental_id of this MediaTypeSpec. 
         :rtype: str
         """
-        return self._file_format
+        return self._elemental_id
 
-    @file_format.setter
-    def file_format(self, file_format):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
+        The elemental ID of the object.
 
-        :param file_format: The file_format of this MediaType.
+        :param elemental_id: The elemental_id of this MediaTypeSpec.
         :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                file_format is not None and len(file_format) > 4):
-            raise ValueError("Invalid value for `file_format`, length must be less than or equal to `4`")  # noqa: E501
 
-        self._file_format = file_format
+        self._elemental_id = elemental_id
 
     @property
-    def id(self):
+    def file_format(self):
         """
-        Unique integer identifying a media type.
+        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
 
-        :return: The id of this MediaType. 
-        :rtype: int
+        :return: The file_format of this MediaTypeSpec. 
+        :rtype: str
         """
-        return self._id
+        return self._file_format
 
-    @id.setter
-    def id(self, id):
+    @file_format.setter
+    def file_format(self, file_format):
         """
-        Unique integer identifying a media type.
+        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
 
-        :param id: The id of this MediaType.
-        :type: int
+        :param file_format: The file_format of this MediaTypeSpec.
+        :type: str
         """
+        if (self.local_vars_configuration.client_side_validation and
+                file_format is not None and len(file_format) > 4):
+            raise ValueError("Invalid value for `file_format`, length must be less than or equal to `4`")  # noqa: E501
 
-        self._id = id
+        self._file_format = file_format
 
     @property
     def name(self):
         """
         Name of the media type.
 
-        :return: The name of this MediaType. 
+        :return: The name of this MediaTypeSpec. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
         Name of the media type.
 
-        :param name: The name of this MediaType.
+        :param name: The name of this MediaTypeSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def overlay_config(self):
         """
         Overlay configuration
 
-        :return: The overlay_config of this MediaType. 
+        :return: The overlay_config of this MediaTypeSpec. 
         :rtype: dict(str, object)
         """
         return self._overlay_config
 
     @overlay_config.setter
     def overlay_config(self, overlay_config):
         """
         Overlay configuration
 
-        :param overlay_config: The overlay_config of this MediaType.
+        :param overlay_config: The overlay_config of this MediaTypeSpec.
         :type: dict(str, object)
         """
 
         self._overlay_config = overlay_config
 
     @property
-    def project(self):
+    def streaming_config(self):
         """
-        Unique integer identifying project for this media type.
+        Streaming config definition. If null, the default will be used.
 
-        :return: The project of this MediaType. 
-        :rtype: int
+        :return: The streaming_config of this MediaTypeSpec. 
+        :rtype: list[ResolutionConfig]
         """
-        return self._project
+        return self._streaming_config
 
-    @project.setter
-    def project(self, project):
+    @streaming_config.setter
+    def streaming_config(self, streaming_config):
         """
-        Unique integer identifying project for this media type.
+        Streaming config definition. If null, the default will be used.
 
-        :param project: The project of this MediaType.
-        :type: int
+        :param streaming_config: The streaming_config of this MediaTypeSpec.
+        :type: list[ResolutionConfig]
         """
 
-        self._project = project
+        self._streaming_config = streaming_config
 
     @property
-    def streaming_config(self):
+    def visible(self):
         """
-        Streaming config defintion. If null, the default will be used.
+        Visible configuration
 
-        :return: The streaming_config of this MediaType. 
-        :rtype: list[ResolutionConfig]
+        :return: The visible of this MediaTypeSpec. 
+        :rtype: bool
         """
-        return self._streaming_config
+        return self._visible
 
-    @streaming_config.setter
-    def streaming_config(self, streaming_config):
+    @visible.setter
+    def visible(self, visible):
         """
-        Streaming config defintion. If null, the default will be used.
+        Visible configuration
 
-        :param streaming_config: The streaming_config of this MediaType.
-        :type: list[ResolutionConfig]
+        :param visible: The visible of this MediaTypeSpec.
+        :type: bool
         """
 
-        self._streaming_config = streaming_config
+        self._visible = visible
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -375,18 +454,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MediaType):
+        if not isinstance(other, MediaTypeSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MediaType):
+        if not isinstance(other, MediaTypeSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_type_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/localization_type_spec.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,290 +14,333 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class MediaTypeSpec(object):
+class LocalizationTypeSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'archive_config': 'list[ArchiveConfig]',
         'attribute_types': 'list[AttributeType]',
-        'default_volume': 'int',
+        'color_map': 'ColorMap',
         'description': 'str',
+        'drawable': 'bool',
         'dtype': 'str',
-        'file_format': 'str',
+        'elemental_id': 'str',
+        'grouping_default': 'bool',
+        'line_width': 'int',
+        'media_types': 'list[int]',
         'name': 'str',
-        'overlay_config': 'dict(str, object)',
-        'streaming_config': 'list[ResolutionConfig]'
+        'visible': 'bool'
     }
 
     attribute_map = {
-        'archive_config': 'archive_config',
         'attribute_types': 'attribute_types',
-        'default_volume': 'default_volume',
+        'color_map': 'color_map',
         'description': 'description',
+        'drawable': 'drawable',
         'dtype': 'dtype',
-        'file_format': 'file_format',
+        'elemental_id': 'elemental_id',
+        'grouping_default': 'grouping_default',
+        'line_width': 'line_width',
+        'media_types': 'media_types',
         'name': 'name',
-        'overlay_config': 'overlay_config',
-        'streaming_config': 'streaming_config'
+        'visible': 'visible'
     }
 
-    def __init__(self, archive_config=None, attribute_types=None, default_volume=None, description='', dtype=None, file_format=None, name=None, overlay_config=None, streaming_config=None, local_vars_configuration=None):  # noqa: E501
-        """MediaTypeSpec - a model defined in OpenAPI"""
+    def __init__(self, attribute_types=None, color_map=None, description=None, drawable=True, dtype=None, elemental_id=None, grouping_default=True, line_width=None, media_types=None, name=None, visible=True, local_vars_configuration=None):  # noqa: E501
+        """LocalizationTypeSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._archive_config = None
         self._attribute_types = None
-        self._default_volume = None
+        self._color_map = None
         self._description = None
+        self._drawable = None
         self._dtype = None
-        self._file_format = None
+        self._elemental_id = None
+        self._grouping_default = None
+        self._line_width = None
+        self._media_types = None
         self._name = None
-        self._overlay_config = None
-        self._streaming_config = None
+        self._visible = None
         self.discriminator = None
 
-        if archive_config is not None:
-            self.archive_config = archive_config
         if attribute_types is not None:
             self.attribute_types = attribute_types
-        if default_volume is not None:
-            self.default_volume = default_volume
+        self.color_map = color_map
         if description is not None:
             self.description = description
+        if drawable is not None:
+            self.drawable = drawable
         self.dtype = dtype
-        if file_format is not None:
-            self.file_format = file_format
+        self.elemental_id = elemental_id
+        if grouping_default is not None:
+            self.grouping_default = grouping_default
+        if line_width is not None:
+            self.line_width = line_width
+        self.media_types = media_types
         self.name = name
-        if overlay_config is not None:
-            self.overlay_config = overlay_config
-        if streaming_config is not None:
-            self.streaming_config = streaming_config
-
-    @property
-    def archive_config(self):
-        """
-        Archive config definitions. If null, the raw file will be uploaded to Tator.
-
-        :return: The archive_config of this MediaTypeSpec. 
-        :rtype: list[ArchiveConfig]
-        """
-        return self._archive_config
-
-    @archive_config.setter
-    def archive_config(self, archive_config):
-        """
-        Archive config definitions. If null, the raw file will be uploaded to Tator.
-
-        :param archive_config: The archive_config of this MediaTypeSpec.
-        :type: list[ArchiveConfig]
-        """
-
-        self._archive_config = archive_config
+        if visible is not None:
+            self.visible = visible
 
     @property
     def attribute_types(self):
         """
         Attribute type definitions.
 
-        :return: The attribute_types of this MediaTypeSpec. 
+        :return: The attribute_types of this LocalizationTypeSpec. 
         :rtype: list[AttributeType]
         """
         return self._attribute_types
 
     @attribute_types.setter
     def attribute_types(self, attribute_types):
         """
         Attribute type definitions.
 
-        :param attribute_types: The attribute_types of this MediaTypeSpec.
+        :param attribute_types: The attribute_types of this LocalizationTypeSpec.
         :type: list[AttributeType]
         """
 
         self._attribute_types = attribute_types
 
     @property
-    def default_volume(self):
+    def color_map(self):
         """
-        Default audio volume for this media type.
 
-        :return: The default_volume of this MediaTypeSpec. 
-        :rtype: int
+        :return: The color_map of this LocalizationTypeSpec. 
+        :rtype: ColorMap
         """
-        return self._default_volume
+        return self._color_map
 
-    @default_volume.setter
-    def default_volume(self, default_volume):
+    @color_map.setter
+    def color_map(self, color_map):
         """
-        Default audio volume for this media type.
 
-        :param default_volume: The default_volume of this MediaTypeSpec.
-        :type: int
+        :param color_map: The color_map of this LocalizationTypeSpec.
+        :type: ColorMap
         """
-        if (self.local_vars_configuration.client_side_validation and
-                default_volume is not None and default_volume > 100):  # noqa: E501
-            raise ValueError("Invalid value for `default_volume`, must be a value less than or equal to `100`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                default_volume is not None and default_volume < 0):  # noqa: E501
-            raise ValueError("Invalid value for `default_volume`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._default_volume = default_volume
+        self._color_map = color_map
 
     @property
     def description(self):
         """
-        Description of the media type.
+        Description of the localization type.
 
-        :return: The description of this MediaTypeSpec. 
+        :return: The description of this LocalizationTypeSpec. 
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
-        Description of the media type.
+        Description of the localization type.
 
-        :param description: The description of this MediaTypeSpec.
+        :param description: The description of this LocalizationTypeSpec.
         :type: str
         """
 
         self._description = description
 
     @property
+    def drawable(self):
+        """
+        Whether this type can be drawn in the UI. Must also be visible.
+
+        :return: The drawable of this LocalizationTypeSpec. 
+        :rtype: bool
+        """
+        return self._drawable
+
+    @drawable.setter
+    def drawable(self, drawable):
+        """
+        Whether this type can be drawn in the UI. Must also be visible.
+
+        :param drawable: The drawable of this LocalizationTypeSpec.
+        :type: bool
+        """
+
+        self._drawable = drawable
+
+    @property
     def dtype(self):
         """
-        Type of the media, image or video.
+        Shape of this localization type.
 
-        :return: The dtype of this MediaTypeSpec. 
+        :return: The dtype of this LocalizationTypeSpec. 
         :rtype: str
         """
         return self._dtype
 
     @dtype.setter
     def dtype(self, dtype):
         """
-        Type of the media, image or video.
+        Shape of this localization type.
 
-        :param dtype: The dtype of this MediaTypeSpec.
+        :param dtype: The dtype of this LocalizationTypeSpec.
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and dtype is None:  # noqa: E501
             raise ValueError("Invalid value for `dtype`, must not be `None`")  # noqa: E501
-        allowed_values = ["image", "video", "multi"]  # noqa: E501
+        allowed_values = ["box", "line", "dot", "poly"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and dtype not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `dtype` ({0}), must be one of {1}"  # noqa: E501
                 .format(dtype, allowed_values)
             )
 
         self._dtype = dtype
 
     @property
-    def file_format(self):
+    def elemental_id(self):
         """
-        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
+        The elemental ID of the object.
 
-        :return: The file_format of this MediaTypeSpec. 
+        :return: The elemental_id of this LocalizationTypeSpec. 
         :rtype: str
         """
-        return self._file_format
+        return self._elemental_id
 
-    @file_format.setter
-    def file_format(self, file_format):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
+        The elemental ID of the object.
 
-        :param file_format: The file_format of this MediaTypeSpec.
+        :param elemental_id: The elemental_id of this LocalizationTypeSpec.
         :type: str
         """
+
+        self._elemental_id = elemental_id
+
+    @property
+    def grouping_default(self):
+        """
+        Whether to group elements in the UI by default.
+
+        :return: The grouping_default of this LocalizationTypeSpec. 
+        :rtype: bool
+        """
+        return self._grouping_default
+
+    @grouping_default.setter
+    def grouping_default(self, grouping_default):
+        """
+        Whether to group elements in the UI by default.
+
+        :param grouping_default: The grouping_default of this LocalizationTypeSpec.
+        :type: bool
+        """
+
+        self._grouping_default = grouping_default
+
+    @property
+    def line_width(self):
+        """
+        Width of the line used to draw the localization.
+
+        :return: The line_width of this LocalizationTypeSpec. 
+        :rtype: int
+        """
+        return self._line_width
+
+    @line_width.setter
+    def line_width(self, line_width):
+        """
+        Width of the line used to draw the localization.
+
+        :param line_width: The line_width of this LocalizationTypeSpec.
+        :type: int
+        """
         if (self.local_vars_configuration.client_side_validation and
-                file_format is not None and len(file_format) > 4):
-            raise ValueError("Invalid value for `file_format`, length must be less than or equal to `4`")  # noqa: E501
+                line_width is not None and line_width < 1):  # noqa: E501
+            raise ValueError("Invalid value for `line_width`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._file_format = file_format
+        self._line_width = line_width
 
     @property
-    def name(self):
+    def media_types(self):
         """
-        Name of the media type.
+        List of integers identifying media types that this localization type may apply to.
 
-        :return: The name of this MediaTypeSpec. 
-        :rtype: str
+        :return: The media_types of this LocalizationTypeSpec. 
+        :rtype: list[int]
         """
-        return self._name
+        return self._media_types
 
-    @name.setter
-    def name(self, name):
+    @media_types.setter
+    def media_types(self, media_types):
         """
-        Name of the media type.
+        List of integers identifying media types that this localization type may apply to.
 
-        :param name: The name of this MediaTypeSpec.
-        :type: str
+        :param media_types: The media_types of this LocalizationTypeSpec.
+        :type: list[int]
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and media_types is None:  # noqa: E501
+            raise ValueError("Invalid value for `media_types`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._media_types = media_types
 
     @property
-    def overlay_config(self):
+    def name(self):
         """
-        Overlay configuration
+        Name of the localization type.
 
-        :return: The overlay_config of this MediaTypeSpec. 
-        :rtype: dict(str, object)
+        :return: The name of this LocalizationTypeSpec. 
+        :rtype: str
         """
-        return self._overlay_config
+        return self._name
 
-    @overlay_config.setter
-    def overlay_config(self, overlay_config):
+    @name.setter
+    def name(self, name):
         """
-        Overlay configuration
+        Name of the localization type.
 
-        :param overlay_config: The overlay_config of this MediaTypeSpec.
-        :type: dict(str, object)
+        :param name: The name of this LocalizationTypeSpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._overlay_config = overlay_config
+        self._name = name
 
     @property
-    def streaming_config(self):
+    def visible(self):
         """
-        Streaming config defintion. If null, the default will be used.
+        Whether this type should be displayed in the UI.
 
-        :return: The streaming_config of this MediaTypeSpec. 
-        :rtype: list[ResolutionConfig]
+        :return: The visible of this LocalizationTypeSpec. 
+        :rtype: bool
         """
-        return self._streaming_config
+        return self._visible
 
-    @streaming_config.setter
-    def streaming_config(self, streaming_config):
+    @visible.setter
+    def visible(self, visible):
         """
-        Streaming config defintion. If null, the default will be used.
+        Whether this type should be displayed in the UI.
 
-        :param streaming_config: The streaming_config of this MediaTypeSpec.
-        :type: list[ResolutionConfig]
+        :param visible: The visible of this LocalizationTypeSpec.
+        :type: bool
         """
 
-        self._streaming_config = streaming_config
+        self._visible = visible
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -325,18 +368,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MediaTypeSpec):
+        if not isinstance(other, LocalizationTypeSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MediaTypeSpec):
+        if not isinstance(other, LocalizationTypeSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_type_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/favorite_spec.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,172 +14,184 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class MediaTypeUpdate(object):
+class FavoriteSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'archive_config': 'list[ArchiveConfig]',
-        'description': 'str',
-        'file_format': 'str',
+        'entity_type_name': 'str',
         'name': 'str',
-        'streaming_config': 'list[ResolutionConfig]'
+        'page': 'int',
+        'type': 'int',
+        'values': 'dict(str, object)'
     }
 
     attribute_map = {
-        'archive_config': 'archive_config',
-        'description': 'description',
-        'file_format': 'file_format',
+        'entity_type_name': 'entity_type_name',
         'name': 'name',
-        'streaming_config': 'streaming_config'
+        'page': 'page',
+        'type': 'type',
+        'values': 'values'
     }
 
-    def __init__(self, archive_config=None, description='', file_format=None, name=None, streaming_config=None, local_vars_configuration=None):  # noqa: E501
-        """MediaTypeUpdate - a model defined in OpenAPI"""
+    def __init__(self, entity_type_name=None, name=None, page=1, type=None, values=None, local_vars_configuration=None):  # noqa: E501
+        """FavoriteSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._archive_config = None
-        self._description = None
-        self._file_format = None
+        self._entity_type_name = None
         self._name = None
-        self._streaming_config = None
+        self._page = None
+        self._type = None
+        self._values = None
         self.discriminator = None
 
-        if archive_config is not None:
-            self.archive_config = archive_config
-        if description is not None:
-            self.description = description
-        if file_format is not None:
-            self.file_format = file_format
+        if entity_type_name is not None:
+            self.entity_type_name = entity_type_name
         if name is not None:
             self.name = name
-        if streaming_config is not None:
-            self.streaming_config = streaming_config
+        if page is not None:
+            self.page = page
+        if type is not None:
+            self.type = type
+        if values is not None:
+            self.values = values
 
     @property
-    def archive_config(self):
+    def entity_type_name(self):
         """
-        Archive config definitions. If null, the raw file will be uploaded to Tator.
+        Name of entity type associated with the favorite
 
-        :return: The archive_config of this MediaTypeUpdate. 
-        :rtype: list[ArchiveConfig]
+        :return: The entity_type_name of this FavoriteSpec. 
+        :rtype: str
         """
-        return self._archive_config
+        return self._entity_type_name
 
-    @archive_config.setter
-    def archive_config(self, archive_config):
+    @entity_type_name.setter
+    def entity_type_name(self, entity_type_name):
         """
-        Archive config definitions. If null, the raw file will be uploaded to Tator.
+        Name of entity type associated with the favorite
 
-        :param archive_config: The archive_config of this MediaTypeUpdate.
-        :type: list[ArchiveConfig]
+        :param entity_type_name: The entity_type_name of this FavoriteSpec.
+        :type: str
         """
+        allowed_values = ["Localization", "State"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and entity_type_name not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `entity_type_name` ({0}), must be one of {1}"  # noqa: E501
+                .format(entity_type_name, allowed_values)
+            )
 
-        self._archive_config = archive_config
+        self._entity_type_name = entity_type_name
 
     @property
-    def description(self):
+    def name(self):
         """
-        Description of the media type.
+        Name of the favorite.
 
-        :return: The description of this MediaTypeUpdate. 
+        :return: The name of this FavoriteSpec. 
         :rtype: str
         """
-        return self._description
+        return self._name
 
-    @description.setter
-    def description(self, description):
+    @name.setter
+    def name(self, name):
         """
-        Description of the media type.
+        Name of the favorite.
 
-        :param description: The description of this MediaTypeUpdate.
+        :param name: The name of this FavoriteSpec.
         :type: str
         """
 
-        self._description = description
+        self._name = name
 
     @property
-    def file_format(self):
+    def page(self):
         """
-        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
+        Integer specifying page to display on. Should be 1-10.
 
-        :return: The file_format of this MediaTypeUpdate. 
-        :rtype: str
+        :return: The page of this FavoriteSpec. 
+        :rtype: int
         """
-        return self._file_format
+        return self._page
 
-    @file_format.setter
-    def file_format(self, file_format):
+    @page.setter
+    def page(self, page):
         """
-        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
+        Integer specifying page to display on. Should be 1-10.
 
-        :param file_format: The file_format of this MediaTypeUpdate.
-        :type: str
+        :param page: The page of this FavoriteSpec.
+        :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
-                file_format is not None and len(file_format) > 4):
-            raise ValueError("Invalid value for `file_format`, length must be less than or equal to `4`")  # noqa: E501
+                page is not None and page > 10):  # noqa: E501
+            raise ValueError("Invalid value for `page`, must be a value less than or equal to `10`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                page is not None and page < 1):  # noqa: E501
+            raise ValueError("Invalid value for `page`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._file_format = file_format
+        self._page = page
 
     @property
-    def name(self):
+    def type(self):
         """
-        Name of the media type.
+        Unique integer identifying an entity type.
 
-        :return: The name of this MediaTypeUpdate. 
-        :rtype: str
+        :return: The type of this FavoriteSpec. 
+        :rtype: int
         """
-        return self._name
+        return self._type
 
-    @name.setter
-    def name(self, name):
+    @type.setter
+    def type(self, type):
         """
-        Name of the media type.
+        Unique integer identifying an entity type.
 
-        :param name: The name of this MediaTypeUpdate.
-        :type: str
+        :param type: The type of this FavoriteSpec.
+        :type: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and type < 1):  # noqa: E501
+            raise ValueError("Invalid value for `type`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._name = name
+        self._type = type
 
     @property
-    def streaming_config(self):
+    def values(self):
         """
-        Streaming config defintion. If null, the default will be used.
+        Attribute name/value pairs.
 
-        :return: The streaming_config of this MediaTypeUpdate. 
-        :rtype: list[ResolutionConfig]
+        :return: The values of this FavoriteSpec. 
+        :rtype: dict(str, object)
         """
-        return self._streaming_config
+        return self._values
 
-    @streaming_config.setter
-    def streaming_config(self, streaming_config):
+    @values.setter
+    def values(self, values):
         """
-        Streaming config defintion. If null, the default will be used.
+        Attribute name/value pairs.
 
-        :param streaming_config: The streaming_config of this MediaTypeUpdate.
-        :type: list[ResolutionConfig]
+        :param values: The values of this FavoriteSpec.
+        :type: dict(str, object)
         """
 
-        self._streaming_config = streaming_config
+        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -207,18 +219,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MediaTypeUpdate):
+        if not isinstance(other, FavoriteSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MediaTypeUpdate):
+        if not isinstance(other, FavoriteSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/media_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_bulk_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,324 +14,303 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class MediaUpdate(object):
+class MediaBulkUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'archive_state': 'str',
         'attributes': 'dict(str, object)',
-        'codec': 'str',
-        'fps': 'float',
-        'height': 'int',
-        'last_edit_end': 'datetime',
-        'last_edit_start': 'datetime',
-        'media_files': 'MediaFiles',
-        'multi': 'MultiDefinition',
-        'name': 'str',
-        'num_frames': 'int',
-        'width': 'int'
+        'float_array': 'list[FloatArrayQuery]',
+        'ids': 'list[int]',
+        'localization_ids': 'list[int]',
+        'null_attributes': 'list[str]',
+        'object_search': 'AttributeOperationSpec',
+        'reset_attributes': 'list[str]',
+        'state_ids': 'list[int]',
+        'user_elemental_id': 'str'
     }
 
     attribute_map = {
+        'archive_state': 'archive_state',
         'attributes': 'attributes',
-        'codec': 'codec',
-        'fps': 'fps',
-        'height': 'height',
-        'last_edit_end': 'last_edit_end',
-        'last_edit_start': 'last_edit_start',
-        'media_files': 'media_files',
-        'multi': 'multi',
-        'name': 'name',
-        'num_frames': 'num_frames',
-        'width': 'width'
+        'float_array': 'float_array',
+        'ids': 'ids',
+        'localization_ids': 'localization_ids',
+        'null_attributes': 'null_attributes',
+        'object_search': 'object_search',
+        'reset_attributes': 'reset_attributes',
+        'state_ids': 'state_ids',
+        'user_elemental_id': 'user_elemental_id'
     }
 
-    def __init__(self, attributes=None, codec=None, fps=None, height=None, last_edit_end=None, last_edit_start=None, media_files=None, multi=None, name=None, num_frames=None, width=None, local_vars_configuration=None):  # noqa: E501
-        """MediaUpdate - a model defined in OpenAPI"""
+    def __init__(self, archive_state=None, attributes=None, float_array=None, ids=None, localization_ids=None, null_attributes=None, object_search=None, reset_attributes=None, state_ids=None, user_elemental_id=None, local_vars_configuration=None):  # noqa: E501
+        """MediaBulkUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._archive_state = None
         self._attributes = None
-        self._codec = None
-        self._fps = None
-        self._height = None
-        self._last_edit_end = None
-        self._last_edit_start = None
-        self._media_files = None
-        self._multi = None
-        self._name = None
-        self._num_frames = None
-        self._width = None
+        self._float_array = None
+        self._ids = None
+        self._localization_ids = None
+        self._null_attributes = None
+        self._object_search = None
+        self._reset_attributes = None
+        self._state_ids = None
+        self._user_elemental_id = None
         self.discriminator = None
 
+        if archive_state is not None:
+            self.archive_state = archive_state
         if attributes is not None:
             self.attributes = attributes
-        if codec is not None:
-            self.codec = codec
-        if fps is not None:
-            self.fps = fps
-        if height is not None:
-            self.height = height
-        if last_edit_end is not None:
-            self.last_edit_end = last_edit_end
-        if last_edit_start is not None:
-            self.last_edit_start = last_edit_start
-        if media_files is not None:
-            self.media_files = media_files
-        if multi is not None:
-            self.multi = multi
-        if name is not None:
-            self.name = name
-        if num_frames is not None:
-            self.num_frames = num_frames
-        if width is not None:
-            self.width = width
+        if float_array is not None:
+            self.float_array = float_array
+        if ids is not None:
+            self.ids = ids
+        if localization_ids is not None:
+            self.localization_ids = localization_ids
+        if null_attributes is not None:
+            self.null_attributes = null_attributes
+        if object_search is not None:
+            self.object_search = object_search
+        if reset_attributes is not None:
+            self.reset_attributes = reset_attributes
+        if state_ids is not None:
+            self.state_ids = state_ids
+        if user_elemental_id is not None:
+            self.user_elemental_id = user_elemental_id
 
     @property
-    def attributes(self):
-        """
-        Object containing attribute values.
-
-        :return: The attributes of this MediaUpdate. 
-        :rtype: dict(str, object)
-        """
-        return self._attributes
-
-    @attributes.setter
-    def attributes(self, attributes):
-        """
-        Object containing attribute values.
-
-        :param attributes: The attributes of this MediaUpdate.
-        :type: dict(str, object)
-        """
-
-        self._attributes = attributes
-
-    @property
-    def codec(self):
+    def archive_state(self):
         """
-        Codec of the original video.
+        Marks media for archival or retrieval. Media may not be set directly to `live` or `archived`, the system performs that transition for the user.
 
-        :return: The codec of this MediaUpdate. 
+        :return: The archive_state of this MediaBulkUpdate. 
         :rtype: str
         """
-        return self._codec
+        return self._archive_state
 
-    @codec.setter
-    def codec(self, codec):
+    @archive_state.setter
+    def archive_state(self, archive_state):
         """
-        Codec of the original video.
+        Marks media for archival or retrieval. Media may not be set directly to `live` or `archived`, the system performs that transition for the user.
 
-        :param codec: The codec of this MediaUpdate.
+        :param archive_state: The archive_state of this MediaBulkUpdate.
         :type: str
         """
+        allowed_values = ["to_archive", "to_live"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and archive_state not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `archive_state` ({0}), must be one of {1}"  # noqa: E501
+                .format(archive_state, allowed_values)
+            )
 
-        self._codec = codec
+        self._archive_state = archive_state
 
     @property
-    def fps(self):
+    def attributes(self):
         """
-        Frame rate of the video.
+        Attribute values to bulk update an entity list.
 
-        :return: The fps of this MediaUpdate. 
-        :rtype: float
+        :return: The attributes of this MediaBulkUpdate. 
+        :rtype: dict(str, object)
         """
-        return self._fps
+        return self._attributes
 
-    @fps.setter
-    def fps(self, fps):
+    @attributes.setter
+    def attributes(self, attributes):
         """
-        Frame rate of the video.
+        Attribute values to bulk update an entity list.
 
-        :param fps: The fps of this MediaUpdate.
-        :type: float
+        :param attributes: The attributes of this MediaBulkUpdate.
+        :type: dict(str, object)
         """
 
-        self._fps = fps
+        self._attributes = attributes
 
     @property
-    def height(self):
+    def float_array(self):
         """
-        Pixel height of the video.
+        Searches on `float_array` attributes.
 
-        :return: The height of this MediaUpdate. 
-        :rtype: int
+        :return: The float_array of this MediaBulkUpdate. 
+        :rtype: list[FloatArrayQuery]
         """
-        return self._height
+        return self._float_array
 
-    @height.setter
-    def height(self, height):
+    @float_array.setter
+    def float_array(self, float_array):
         """
-        Pixel height of the video.
+        Searches on `float_array` attributes.
 
-        :param height: The height of this MediaUpdate.
-        :type: int
+        :param float_array: The float_array of this MediaBulkUpdate.
+        :type: list[FloatArrayQuery]
         """
 
-        self._height = height
+        self._float_array = float_array
 
     @property
-    def last_edit_end(self):
+    def ids(self):
         """
-        Datetime of the end of the session when this media or its annotations were last edited.
+        Array of media IDs to retrieve.
 
-        :return: The last_edit_end of this MediaUpdate. 
-        :rtype: datetime
+        :return: The ids of this MediaBulkUpdate. 
+        :rtype: list[int]
         """
-        return self._last_edit_end
+        return self._ids
 
-    @last_edit_end.setter
-    def last_edit_end(self, last_edit_end):
+    @ids.setter
+    def ids(self, ids):
         """
-        Datetime of the end of the session when this media or its annotations were last edited.
+        Array of media IDs to retrieve.
 
-        :param last_edit_end: The last_edit_end of this MediaUpdate.
-        :type: datetime
+        :param ids: The ids of this MediaBulkUpdate.
+        :type: list[int]
         """
 
-        self._last_edit_end = last_edit_end
+        self._ids = ids
 
     @property
-    def last_edit_start(self):
+    def localization_ids(self):
         """
-        Datetime of the start of the session when this media or its annotations were last edited.
+        Array of child localization IDs for which media should be retrieved.
 
-        :return: The last_edit_start of this MediaUpdate. 
-        :rtype: datetime
+        :return: The localization_ids of this MediaBulkUpdate. 
+        :rtype: list[int]
         """
-        return self._last_edit_start
+        return self._localization_ids
 
-    @last_edit_start.setter
-    def last_edit_start(self, last_edit_start):
+    @localization_ids.setter
+    def localization_ids(self, localization_ids):
         """
-        Datetime of the start of the session when this media or its annotations were last edited.
+        Array of child localization IDs for which media should be retrieved.
 
-        :param last_edit_start: The last_edit_start of this MediaUpdate.
-        :type: datetime
+        :param localization_ids: The localization_ids of this MediaBulkUpdate.
+        :type: list[int]
         """
 
-        self._last_edit_start = last_edit_start
+        self._localization_ids = localization_ids
 
     @property
-    def media_files(self):
+    def null_attributes(self):
         """
+        Null a value in the attributes body
 
-        :return: The media_files of this MediaUpdate. 
-        :rtype: MediaFiles
+        :return: The null_attributes of this MediaBulkUpdate. 
+        :rtype: list[str]
         """
-        return self._media_files
+        return self._null_attributes
 
-    @media_files.setter
-    def media_files(self, media_files):
+    @null_attributes.setter
+    def null_attributes(self, null_attributes):
         """
+        Null a value in the attributes body
 
-        :param media_files: The media_files of this MediaUpdate.
-        :type: MediaFiles
+        :param null_attributes: The null_attributes of this MediaBulkUpdate.
+        :type: list[str]
         """
 
-        self._media_files = media_files
+        self._null_attributes = null_attributes
 
     @property
-    def multi(self):
+    def object_search(self):
         """
 
-        :return: The multi of this MediaUpdate. 
-        :rtype: MultiDefinition
+        :return: The object_search of this MediaBulkUpdate. 
+        :rtype: AttributeOperationSpec
         """
-        return self._multi
+        return self._object_search
 
-    @multi.setter
-    def multi(self, multi):
+    @object_search.setter
+    def object_search(self, object_search):
         """
 
-        :param multi: The multi of this MediaUpdate.
-        :type: MultiDefinition
+        :param object_search: The object_search of this MediaBulkUpdate.
+        :type: AttributeOperationSpec
         """
 
-        self._multi = multi
+        self._object_search = object_search
 
     @property
-    def name(self):
+    def reset_attributes(self):
         """
-        Name of the media.
+        Reset an attribute to the default value specified in the Type object
 
-        :return: The name of this MediaUpdate. 
-        :rtype: str
+        :return: The reset_attributes of this MediaBulkUpdate. 
+        :rtype: list[str]
         """
-        return self._name
+        return self._reset_attributes
 
-    @name.setter
-    def name(self, name):
+    @reset_attributes.setter
+    def reset_attributes(self, reset_attributes):
         """
-        Name of the media.
+        Reset an attribute to the default value specified in the Type object
 
-        :param name: The name of this MediaUpdate.
-        :type: str
+        :param reset_attributes: The reset_attributes of this MediaBulkUpdate.
+        :type: list[str]
         """
 
-        self._name = name
+        self._reset_attributes = reset_attributes
 
     @property
-    def num_frames(self):
+    def state_ids(self):
         """
-        Number of frames in the video.
+        Array of child state IDs for which media should be retrieved.
 
-        :return: The num_frames of this MediaUpdate. 
-        :rtype: int
+        :return: The state_ids of this MediaBulkUpdate. 
+        :rtype: list[int]
         """
-        return self._num_frames
+        return self._state_ids
 
-    @num_frames.setter
-    def num_frames(self, num_frames):
+    @state_ids.setter
+    def state_ids(self, state_ids):
         """
-        Number of frames in the video.
+        Array of child state IDs for which media should be retrieved.
 
-        :param num_frames: The num_frames of this MediaUpdate.
-        :type: int
+        :param state_ids: The state_ids of this MediaBulkUpdate.
+        :type: list[int]
         """
-        if (self.local_vars_configuration.client_side_validation and
-                num_frames is not None and num_frames < 0):  # noqa: E501
-            raise ValueError("Invalid value for `num_frames`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._num_frames = num_frames
+        self._state_ids = state_ids
 
     @property
-    def width(self):
+    def user_elemental_id(self):
         """
-        Pixel width of the video.
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
 
-        :return: The width of this MediaUpdate. 
-        :rtype: int
+        :return: The user_elemental_id of this MediaBulkUpdate. 
+        :rtype: str
         """
-        return self._width
+        return self._user_elemental_id
 
-    @width.setter
-    def width(self, width):
+    @user_elemental_id.setter
+    def user_elemental_id(self, user_elemental_id):
         """
-        Pixel width of the video.
+        Unique ID of the original user who created this. If permissions allow, will change the creating user to the one referenced by this elemental_id
 
-        :param width: The width of this MediaUpdate.
-        :type: int
+        :param user_elemental_id: The user_elemental_id of this MediaBulkUpdate.
+        :type: str
         """
 
-        self._width = width
+        self._user_elemental_id = user_elemental_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -359,18 +338,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MediaUpdate):
+        if not isinstance(other, MediaBulkUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MediaUpdate):
+        if not isinstance(other, MediaBulkUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/membership.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/membership_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,182 +14,132 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Membership(object):
+class MembershipSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'default_version': 'int',
-        'id': 'int',
         'permission': 'str',
-        'user': 'int',
-        'username': 'str'
+        'user': 'int'
     }
 
     attribute_map = {
         'default_version': 'default_version',
-        'id': 'id',
         'permission': 'permission',
-        'user': 'user',
-        'username': 'username'
+        'user': 'user'
     }
 
-    def __init__(self, default_version=None, id=None, permission=None, user=None, username=None, local_vars_configuration=None):  # noqa: E501
-        """Membership - a model defined in OpenAPI"""
+    def __init__(self, default_version=None, permission=None, user=None, local_vars_configuration=None):  # noqa: E501
+        """MembershipSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._default_version = None
-        self._id = None
         self._permission = None
         self._user = None
-        self._username = None
         self.discriminator = None
 
         if default_version is not None:
             self.default_version = default_version
-        if id is not None:
-            self.id = id
-        if permission is not None:
-            self.permission = permission
-        if user is not None:
-            self.user = user
-        if username is not None:
-            self.username = username
+        self.permission = permission
+        self.user = user
 
     @property
     def default_version(self):
         """
         Unique integer identifying a version.
 
-        :return: The default_version of this Membership. 
+        :return: The default_version of this MembershipSpec. 
         :rtype: int
         """
         return self._default_version
 
     @default_version.setter
     def default_version(self, default_version):
         """
         Unique integer identifying a version.
 
-        :param default_version: The default_version of this Membership.
+        :param default_version: The default_version of this MembershipSpec.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 default_version is not None and default_version < 1):  # noqa: E501
             raise ValueError("Invalid value for `default_version`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._default_version = default_version
 
     @property
-    def id(self):
-        """
-        Unique integer identifying a membership.
-
-        :return: The id of this Membership. 
-        :rtype: int
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """
-        Unique integer identifying a membership.
-
-        :param id: The id of this Membership.
-        :type: int
-        """
-
-        self._id = id
-
-    @property
     def permission(self):
         """
         User permission level for the project.
 
-        :return: The permission of this Membership. 
+        :return: The permission of this MembershipSpec. 
         :rtype: str
         """
         return self._permission
 
     @permission.setter
     def permission(self, permission):
         """
         User permission level for the project.
 
-        :param permission: The permission of this Membership.
+        :param permission: The permission of this MembershipSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and permission is None:  # noqa: E501
+            raise ValueError("Invalid value for `permission`, must not be `None`")  # noqa: E501
         allowed_values = ["View Only", "Can Edit", "Can Transfer", "Can Execute", "Full Control"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and permission not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `permission` ({0}), must be one of {1}"  # noqa: E501
                 .format(permission, allowed_values)
             )
 
         self._permission = permission
 
     @property
     def user(self):
         """
         Unique integer identifying a user.
 
-        :return: The user of this Membership. 
+        :return: The user of this MembershipSpec. 
         :rtype: int
         """
         return self._user
 
     @user.setter
     def user(self, user):
         """
         Unique integer identifying a user.
 
-        :param user: The user of this Membership.
+        :param user: The user of this MembershipSpec.
         :type: int
         """
+        if self.local_vars_configuration.client_side_validation and user is None:  # noqa: E501
+            raise ValueError("Invalid value for `user`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 user is not None and user < 1):  # noqa: E501
             raise ValueError("Invalid value for `user`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._user = user
 
-    @property
-    def username(self):
-        """
-        Username for the membership.
-
-        :return: The username of this Membership. 
-        :rtype: str
-        """
-        return self._username
-
-    @username.setter
-    def username(self, username):
-        """
-        Username for the membership.
-
-        :param username: The username of this Membership.
-        :type: str
-        """
-
-        self._username = username
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -216,18 +166,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Membership):
+        if not isinstance(other, MembershipSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Membership):
+        if not isinstance(other, MembershipSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/membership_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/organization_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,131 +14,123 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class MembershipSpec(object):
+class OrganizationUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'default_version': 'int',
-        'permission': 'str',
-        'user': 'int'
+        'default_membership_permission': 'str',
+        'name': 'str',
+        'thumb': 'str'
     }
 
     attribute_map = {
-        'default_version': 'default_version',
-        'permission': 'permission',
-        'user': 'user'
+        'default_membership_permission': 'default_membership_permission',
+        'name': 'name',
+        'thumb': 'thumb'
     }
 
-    def __init__(self, default_version=None, permission=None, user=None, local_vars_configuration=None):  # noqa: E501
-        """MembershipSpec - a model defined in OpenAPI"""
+    def __init__(self, default_membership_permission=None, name=None, thumb=None, local_vars_configuration=None):  # noqa: E501
+        """OrganizationUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._default_version = None
-        self._permission = None
-        self._user = None
+        self._default_membership_permission = None
+        self._name = None
+        self._thumb = None
         self.discriminator = None
 
-        if default_version is not None:
-            self.default_version = default_version
-        self.permission = permission
-        self.user = user
+        if default_membership_permission is not None:
+            self.default_membership_permission = default_membership_permission
+        if name is not None:
+            self.name = name
+        if thumb is not None:
+            self.thumb = thumb
 
     @property
-    def default_version(self):
+    def default_membership_permission(self):
         """
-        Unique integer identifying a version.
+        Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
 
-        :return: The default_version of this MembershipSpec. 
-        :rtype: int
+        :return: The default_membership_permission of this OrganizationUpdate. 
+        :rtype: str
         """
-        return self._default_version
+        return self._default_membership_permission
 
-    @default_version.setter
-    def default_version(self, default_version):
+    @default_membership_permission.setter
+    def default_membership_permission(self, default_membership_permission):
         """
-        Unique integer identifying a version.
+        Default user permission level for all projects in this organization. If specified, users in this organizaiton will be automatically added to all projects in this organization with at least this permission level.
 
-        :param default_version: The default_version of this MembershipSpec.
-        :type: int
+        :param default_membership_permission: The default_membership_permission of this OrganizationUpdate.
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                default_version is not None and default_version < 1):  # noqa: E501
-            raise ValueError("Invalid value for `default_version`, must be a value greater than or equal to `1`")  # noqa: E501
+        allowed_values = ["No Access", "View Only", "Can Edit", "Can Transfer", "Can Execute", "Full Control"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and default_membership_permission not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `default_membership_permission` ({0}), must be one of {1}"  # noqa: E501
+                .format(default_membership_permission, allowed_values)
+            )
 
-        self._default_version = default_version
+        self._default_membership_permission = default_membership_permission
 
     @property
-    def permission(self):
+    def name(self):
         """
-        User permission level for the project.
+        Name of the organization.
 
-        :return: The permission of this MembershipSpec. 
+        :return: The name of this OrganizationUpdate. 
         :rtype: str
         """
-        return self._permission
+        return self._name
 
-    @permission.setter
-    def permission(self, permission):
+    @name.setter
+    def name(self, name):
         """
-        User permission level for the project.
+        Name of the organization.
 
-        :param permission: The permission of this MembershipSpec.
+        :param name: The name of this OrganizationUpdate.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and permission is None:  # noqa: E501
-            raise ValueError("Invalid value for `permission`, must not be `None`")  # noqa: E501
-        allowed_values = ["View Only", "Can Edit", "Can Transfer", "Can Execute", "Full Control"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and permission not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `permission` ({0}), must be one of {1}"  # noqa: E501
-                .format(permission, allowed_values)
-            )
 
-        self._permission = permission
+        self._name = name
 
     @property
-    def user(self):
+    def thumb(self):
         """
-        Unique integer identifying a user.
+        S3 key of thumbnail used to represent the organization.
 
-        :return: The user of this MembershipSpec. 
-        :rtype: int
+        :return: The thumb of this OrganizationUpdate. 
+        :rtype: str
         """
-        return self._user
+        return self._thumb
 
-    @user.setter
-    def user(self, user):
+    @thumb.setter
+    def thumb(self, thumb):
         """
-        Unique integer identifying a user.
+        S3 key of thumbnail used to represent the organization.
 
-        :param user: The user of this MembershipSpec.
-        :type: int
+        :param thumb: The thumb of this OrganizationUpdate.
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and user is None:  # noqa: E501
-            raise ValueError("Invalid value for `user`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                user is not None and user < 1):  # noqa: E501
-            raise ValueError("Invalid value for `user`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._user = user
+        self._thumb = thumb
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -166,18 +158,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MembershipSpec):
+        if not isinstance(other, OrganizationUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MembershipSpec):
+        if not isinstance(other, OrganizationUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/membership_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/membership_update.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/message_response.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/message_response.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/multi_definition.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/live_update_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,117 +14,91 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class MultiDefinition(object):
+class LiveUpdateDefinition(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'ids': 'list[int]',
         'layout': 'list[int]',
-        'quality': 'int'
+        'streams': 'list[LiveDefinition]'
     }
 
     attribute_map = {
-        'ids': 'ids',
         'layout': 'layout',
-        'quality': 'quality'
+        'streams': 'streams'
     }
 
-    def __init__(self, ids=None, layout=None, quality=None, local_vars_configuration=None):  # noqa: E501
-        """MultiDefinition - a model defined in OpenAPI"""
+    def __init__(self, layout=None, streams=None, local_vars_configuration=None):  # noqa: E501
+        """LiveUpdateDefinition - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._ids = None
         self._layout = None
-        self._quality = None
+        self._streams = None
         self.discriminator = None
 
-        if ids is not None:
-            self.ids = ids
-        if layout is not None:
-            self.layout = layout
-        if quality is not None:
-            self.quality = quality
-
-    @property
-    def ids(self):
-        """
-        If multi-stream list of ids of sub-videos
-
-        :return: The ids of this MultiDefinition. 
-        :rtype: list[int]
-        """
-        return self._ids
-
-    @ids.setter
-    def ids(self, ids):
-        """
-        If multi-stream list of ids of sub-videos
-
-        :param ids: The ids of this MultiDefinition.
-        :type: list[int]
-        """
-
-        self._ids = ids
+        self.layout = layout
+        self.streams = streams
 
     @property
     def layout(self):
         """
         2-element array to define rxc layout
 
-        :return: The layout of this MultiDefinition. 
+        :return: The layout of this LiveUpdateDefinition. 
         :rtype: list[int]
         """
         return self._layout
 
     @layout.setter
     def layout(self, layout):
         """
         2-element array to define rxc layout
 
-        :param layout: The layout of this MultiDefinition.
+        :param layout: The layout of this LiveUpdateDefinition.
         :type: list[int]
         """
+        if self.local_vars_configuration.client_side_validation and layout is None:  # noqa: E501
+            raise ValueError("Invalid value for `layout`, must not be `None`")  # noqa: E501
 
         self._layout = layout
 
     @property
-    def quality(self):
+    def streams(self):
         """
-        Resolution to fetch on each sub-video
 
-        :return: The quality of this MultiDefinition. 
-        :rtype: int
+        :return: The streams of this LiveUpdateDefinition. 
+        :rtype: list[LiveDefinition]
         """
-        return self._quality
+        return self._streams
 
-    @quality.setter
-    def quality(self, quality):
+    @streams.setter
+    def streams(self, streams):
         """
-        Resolution to fetch on each sub-video
 
-        :param quality: The quality of this MultiDefinition.
-        :type: int
+        :param streams: The streams of this LiveUpdateDefinition.
+        :type: list[LiveDefinition]
         """
+        if self.local_vars_configuration.client_side_validation and streams is None:  # noqa: E501
+            raise ValueError("Invalid value for `streams`, must not be `None`")  # noqa: E501
 
-        self._quality = quality
+        self._streams = streams
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -152,18 +126,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MultiDefinition):
+        if not isinstance(other, LiveUpdateDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MultiDefinition):
+        if not isinstance(other, LiveUpdateDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/not_found_response.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/transcode.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,65 +14,87 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class NotFoundResponse(object):
+class Transcode(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'message': 'str'
+        'job': 'Job',
+        'spec': 'TranscodeSpec'
     }
 
     attribute_map = {
-        'message': 'message'
+        'job': 'job',
+        'spec': 'spec'
     }
 
-    def __init__(self, message=None, local_vars_configuration=None):  # noqa: E501
-        """NotFoundResponse - a model defined in OpenAPI"""
+    def __init__(self, job=None, spec=None, local_vars_configuration=None):  # noqa: E501
+        """Transcode - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._message = None
+        self._job = None
+        self._spec = None
         self.discriminator = None
 
-        if message is not None:
-            self.message = message
+        if job is not None:
+            self.job = job
+        if spec is not None:
+            self.spec = spec
 
     @property
-    def message(self):
+    def job(self):
         """
-        Message explaining not found error.
 
-        :return: The message of this NotFoundResponse. 
-        :rtype: str
+        :return: The job of this Transcode. 
+        :rtype: Job
         """
-        return self._message
+        return self._job
 
-    @message.setter
-    def message(self, message):
+    @job.setter
+    def job(self, job):
         """
-        Message explaining not found error.
 
-        :param message: The message of this NotFoundResponse.
-        :type: str
+        :param job: The job of this Transcode.
+        :type: Job
         """
 
-        self._message = message
+        self._job = job
+
+    @property
+    def spec(self):
+        """
+
+        :return: The spec of this Transcode. 
+        :rtype: TranscodeSpec
+        """
+        return self._spec
+
+    @spec.setter
+    def spec(self, spec):
+        """
+
+        :param spec: The spec of this Transcode.
+        :type: TranscodeSpec
+        """
+
+        self._spec = spec
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -100,18 +122,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NotFoundResponse):
+        if not isinstance(other, Transcode):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, NotFoundResponse):
+        if not isinstance(other, Transcode):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/notify_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/invitation_spec.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,92 +14,99 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class NotifySpec(object):
+class InvitationSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'message': 'str',
-        'send_as_file': 'int'
+        'email': 'str',
+        'permission': 'str'
     }
 
     attribute_map = {
-        'message': 'message',
-        'send_as_file': 'sendAsFile'
+        'email': 'email',
+        'permission': 'permission'
     }
 
-    def __init__(self, message=None, send_as_file=None, local_vars_configuration=None):  # noqa: E501
-        """NotifySpec - a model defined in OpenAPI"""
+    def __init__(self, email=None, permission=None, local_vars_configuration=None):  # noqa: E501
+        """InvitationSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._message = None
-        self._send_as_file = None
+        self._email = None
+        self._permission = None
         self.discriminator = None
 
-        self.message = message
-        if send_as_file is not None:
-            self.send_as_file = send_as_file
+        self.email = email
+        self.permission = permission
 
     @property
-    def message(self):
+    def email(self):
         """
-        Message to send to administrators.
+        Email address of invitee.
 
-        :return: The message of this NotifySpec. 
+        :return: The email of this InvitationSpec. 
         :rtype: str
         """
-        return self._message
+        return self._email
 
-    @message.setter
-    def message(self, message):
+    @email.setter
+    def email(self, email):
         """
-        Message to send to administrators.
+        Email address of invitee.
 
-        :param message: The message of this NotifySpec.
+        :param email: The email of this InvitationSpec.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and message is None:  # noqa: E501
-            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and email is None:  # noqa: E501
+            raise ValueError("Invalid value for `email`, must not be `None`")  # noqa: E501
 
-        self._message = message
+        self._email = email
 
     @property
-    def send_as_file(self):
+    def permission(self):
         """
-        Whether to send message as a file. (0 or 1)
+        User permission level for the organization.
 
-        :return: The send_as_file of this NotifySpec. 
-        :rtype: int
+        :return: The permission of this InvitationSpec. 
+        :rtype: str
         """
-        return self._send_as_file
+        return self._permission
 
-    @send_as_file.setter
-    def send_as_file(self, send_as_file):
+    @permission.setter
+    def permission(self, permission):
         """
-        Whether to send message as a file. (0 or 1)
+        User permission level for the organization.
 
-        :param send_as_file: The send_as_file of this NotifySpec.
-        :type: int
+        :param permission: The permission of this InvitationSpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and permission is None:  # noqa: E501
+            raise ValueError("Invalid value for `permission`, must not be `None`")  # noqa: E501
+        allowed_values = ["Member", "Admin"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and permission not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `permission` ({0}), must be one of {1}"  # noqa: E501
+                .format(permission, allowed_values)
+            )
 
-        self._send_as_file = send_as_file
+        self._permission = permission
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -127,18 +134,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NotifySpec):
+        if not isinstance(other, InvitationSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, NotifySpec):
+        if not isinstance(other, InvitationSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/organization.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/concat_definition.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,91 +14,91 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Organization(object):
+class ConcatDefinition(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'id': 'int',
-        'name': 'str'
+        'timestamp_offset': 'float'
     }
 
     attribute_map = {
         'id': 'id',
-        'name': 'name'
+        'timestamp_offset': 'timestampOffset'
     }
 
-    def __init__(self, id=None, name=None, local_vars_configuration=None):  # noqa: E501
-        """Organization - a model defined in OpenAPI"""
+    def __init__(self, id=None, timestamp_offset=None, local_vars_configuration=None):  # noqa: E501
+        """ConcatDefinition - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
-        self._name = None
+        self._timestamp_offset = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
-        if name is not None:
-            self.name = name
+        if timestamp_offset is not None:
+            self.timestamp_offset = timestamp_offset
 
     @property
     def id(self):
         """
-        Unique integer identifying the organization.
+        Primary key of video in append series
 
-        :return: The id of this Organization. 
+        :return: The id of this ConcatDefinition. 
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """
-        Unique integer identifying the organization.
+        Primary key of video in append series
 
-        :param id: The id of this Organization.
+        :param id: The id of this ConcatDefinition.
         :type: int
         """
 
         self._id = id
 
     @property
-    def name(self):
+    def timestamp_offset(self):
         """
-        Name of the organization.
+        Insertion point for this video
 
-        :return: The name of this Organization. 
-        :rtype: str
+        :return: The timestamp_offset of this ConcatDefinition. 
+        :rtype: float
         """
-        return self._name
+        return self._timestamp_offset
 
-    @name.setter
-    def name(self, name):
+    @timestamp_offset.setter
+    def timestamp_offset(self, timestamp_offset):
         """
-        Name of the organization.
+        Insertion point for this video
 
-        :param name: The name of this Organization.
-        :type: str
+        :param timestamp_offset: The timestamp_offset of this ConcatDefinition.
+        :type: float
         """
 
-        self._name = name
+        self._timestamp_offset = timestamp_offset
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -126,18 +126,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Organization):
+        if not isinstance(other, ConcatDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Organization):
+        if not isinstance(other, ConcatDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/organization_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state_delete.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,66 +14,71 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class OrganizationSpec(object):
+class StateDelete(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str'
+        'prune': 'int'
     }
 
     attribute_map = {
-        'name': 'name'
+        'prune': 'prune'
     }
 
-    def __init__(self, name=None, local_vars_configuration=None):  # noqa: E501
-        """OrganizationSpec - a model defined in OpenAPI"""
+    def __init__(self, prune=0, local_vars_configuration=None):  # noqa: E501
+        """StateDelete - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
+        self._prune = None
         self.discriminator = None
 
-        self.name = name
+        if prune is not None:
+            self.prune = prune
 
     @property
-    def name(self):
+    def prune(self):
         """
-        Name of the organization.
+        If set to 1 will purge the object from the database entirely. This removes any record, change-log, that this metadatum ever existed.
 
-        :return: The name of this OrganizationSpec. 
-        :rtype: str
+        :return: The prune of this StateDelete. 
+        :rtype: int
         """
-        return self._name
+        return self._prune
 
-    @name.setter
-    def name(self, name):
+    @prune.setter
+    def prune(self, prune):
         """
-        Name of the organization.
+        If set to 1 will purge the object from the database entirely. This removes any record, change-log, that this metadatum ever existed.
 
-        :param name: The name of this OrganizationSpec.
-        :type: str
+        :param prune: The prune of this StateDelete.
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                prune is not None and prune > 1):  # noqa: E501
+            raise ValueError("Invalid value for `prune`, must be a value less than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                prune is not None and prune < 0):  # noqa: E501
+            raise ValueError("Invalid value for `prune`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._name = name
+        self._prune = prune
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -101,18 +106,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, OrganizationSpec):
+        if not isinstance(other, StateDelete):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, OrganizationSpec):
+        if not isinstance(other, StateDelete):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/project.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_type_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,354 +14,333 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Project(object):
+class MediaTypeUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'created': 'str',
-        'duration': 'int',
-        'enable_downloads': 'bool',
-        'id': 'int',
+        'archive_config': 'list[ArchiveConfig]',
+        'default_box': 'int',
+        'default_dot': 'int',
+        'default_line': 'int',
+        'default_volume': 'int',
+        'description': 'str',
+        'elemental_id': 'str',
+        'file_format': 'str',
         'name': 'str',
-        'num_files': 'int',
-        'organization': 'int',
-        'permission': 'str',
-        'size': 'int',
-        'summary': 'str',
-        'thumb': 'str',
-        'usernames': 'list[str]'
+        'streaming_config': 'list[ResolutionConfig]',
+        'visible': 'bool'
     }
 
     attribute_map = {
-        'created': 'created',
-        'duration': 'duration',
-        'enable_downloads': 'enable_downloads',
-        'id': 'id',
+        'archive_config': 'archive_config',
+        'default_box': 'default_box',
+        'default_dot': 'default_dot',
+        'default_line': 'default_line',
+        'default_volume': 'default_volume',
+        'description': 'description',
+        'elemental_id': 'elemental_id',
+        'file_format': 'file_format',
         'name': 'name',
-        'num_files': 'num_files',
-        'organization': 'organization',
-        'permission': 'permission',
-        'size': 'size',
-        'summary': 'summary',
-        'thumb': 'thumb',
-        'usernames': 'usernames'
+        'streaming_config': 'streaming_config',
+        'visible': 'visible'
     }
 
-    def __init__(self, created=None, duration=None, enable_downloads=True, id=None, name=None, num_files=None, organization=None, permission=None, size=None, summary='', thumb=None, usernames=None, local_vars_configuration=None):  # noqa: E501
-        """Project - a model defined in OpenAPI"""
+    def __init__(self, archive_config=None, default_box=None, default_dot=None, default_line=None, default_volume=None, description=None, elemental_id=None, file_format=None, name=None, streaming_config=None, visible=None, local_vars_configuration=None):  # noqa: E501
+        """MediaTypeUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._created = None
-        self._duration = None
-        self._enable_downloads = None
-        self._id = None
+        self._archive_config = None
+        self._default_box = None
+        self._default_dot = None
+        self._default_line = None
+        self._default_volume = None
+        self._description = None
+        self._elemental_id = None
+        self._file_format = None
         self._name = None
-        self._num_files = None
-        self._organization = None
-        self._permission = None
-        self._size = None
-        self._summary = None
-        self._thumb = None
-        self._usernames = None
+        self._streaming_config = None
+        self._visible = None
         self.discriminator = None
 
-        if created is not None:
-            self.created = created
-        if duration is not None:
-            self.duration = duration
-        if enable_downloads is not None:
-            self.enable_downloads = enable_downloads
-        if id is not None:
-            self.id = id
+        if archive_config is not None:
+            self.archive_config = archive_config
+        if default_box is not None:
+            self.default_box = default_box
+        if default_dot is not None:
+            self.default_dot = default_dot
+        if default_line is not None:
+            self.default_line = default_line
+        if default_volume is not None:
+            self.default_volume = default_volume
+        if description is not None:
+            self.description = description
+        self.elemental_id = elemental_id
+        if file_format is not None:
+            self.file_format = file_format
         if name is not None:
             self.name = name
-        if num_files is not None:
-            self.num_files = num_files
-        if organization is not None:
-            self.organization = organization
-        if permission is not None:
-            self.permission = permission
-        if size is not None:
-            self.size = size
-        if summary is not None:
-            self.summary = summary
-        if thumb is not None:
-            self.thumb = thumb
-        if usernames is not None:
-            self.usernames = usernames
+        if streaming_config is not None:
+            self.streaming_config = streaming_config
+        if visible is not None:
+            self.visible = visible
 
     @property
-    def created(self):
+    def archive_config(self):
         """
-        Datetime when this project was created.
+        Archive config definitions. If null, the raw file will be uploaded to Tator.
 
-        :return: The created of this Project. 
-        :rtype: str
+        :return: The archive_config of this MediaTypeUpdate. 
+        :rtype: list[ArchiveConfig]
         """
-        return self._created
+        return self._archive_config
 
-    @created.setter
-    def created(self, created):
+    @archive_config.setter
+    def archive_config(self, archive_config):
         """
-        Datetime when this project was created.
+        Archive config definitions. If null, the raw file will be uploaded to Tator.
 
-        :param created: The created of this Project.
-        :type: str
+        :param archive_config: The archive_config of this MediaTypeUpdate.
+        :type: list[ArchiveConfig]
         """
 
-        self._created = created
+        self._archive_config = archive_config
 
     @property
-    def duration(self):
+    def default_box(self):
         """
-        Total duration of all video in the project.
+        Unique integer identifying default box type for drawing.
 
-        :return: The duration of this Project. 
+        :return: The default_box of this MediaTypeUpdate. 
         :rtype: int
         """
-        return self._duration
+        return self._default_box
 
-    @duration.setter
-    def duration(self, duration):
+    @default_box.setter
+    def default_box(self, default_box):
         """
-        Total duration of all video in the project.
+        Unique integer identifying default box type for drawing.
 
-        :param duration: The duration of this Project.
+        :param default_box: The default_box of this MediaTypeUpdate.
         :type: int
         """
 
-        self._duration = duration
-
-    @property
-    def enable_downloads(self):
-        """
-        Whether the UI should allow downloads for this project.
-
-        :return: The enable_downloads of this Project. 
-        :rtype: bool
-        """
-        return self._enable_downloads
-
-    @enable_downloads.setter
-    def enable_downloads(self, enable_downloads):
-        """
-        Whether the UI should allow downloads for this project.
-
-        :param enable_downloads: The enable_downloads of this Project.
-        :type: bool
-        """
-
-        self._enable_downloads = enable_downloads
+        self._default_box = default_box
 
     @property
-    def id(self):
+    def default_dot(self):
         """
-        Unique integer identifying the project.
+        Unique integer identifying default dot type for drawing.
 
-        :return: The id of this Project. 
+        :return: The default_dot of this MediaTypeUpdate. 
         :rtype: int
         """
-        return self._id
+        return self._default_dot
 
-    @id.setter
-    def id(self, id):
+    @default_dot.setter
+    def default_dot(self, default_dot):
         """
-        Unique integer identifying the project.
+        Unique integer identifying default dot type for drawing.
 
-        :param id: The id of this Project.
+        :param default_dot: The default_dot of this MediaTypeUpdate.
         :type: int
         """
 
-        self._id = id
+        self._default_dot = default_dot
 
     @property
-    def name(self):
+    def default_line(self):
         """
-        Name of the project.
+        Unique integer identifying default line type for drawing.
 
-        :return: The name of this Project. 
-        :rtype: str
+        :return: The default_line of this MediaTypeUpdate. 
+        :rtype: int
         """
-        return self._name
+        return self._default_line
 
-    @name.setter
-    def name(self, name):
+    @default_line.setter
+    def default_line(self, default_line):
         """
-        Name of the project.
+        Unique integer identifying default line type for drawing.
 
-        :param name: The name of this Project.
-        :type: str
+        :param default_line: The default_line of this MediaTypeUpdate.
+        :type: int
         """
 
-        self._name = name
+        self._default_line = default_line
 
     @property
-    def num_files(self):
+    def default_volume(self):
         """
-        Number of files in the project.
+        Default audio volume for this media type.
 
-        :return: The num_files of this Project. 
+        :return: The default_volume of this MediaTypeUpdate. 
         :rtype: int
         """
-        return self._num_files
+        return self._default_volume
 
-    @num_files.setter
-    def num_files(self, num_files):
+    @default_volume.setter
+    def default_volume(self, default_volume):
         """
-        Number of files in the project.
+        Default audio volume for this media type.
 
-        :param num_files: The num_files of this Project.
+        :param default_volume: The default_volume of this MediaTypeUpdate.
         :type: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                default_volume is not None and default_volume > 100):  # noqa: E501
+            raise ValueError("Invalid value for `default_volume`, must be a value less than or equal to `100`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                default_volume is not None and default_volume < 0):  # noqa: E501
+            raise ValueError("Invalid value for `default_volume`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._num_files = num_files
+        self._default_volume = default_volume
 
     @property
-    def organization(self):
+    def description(self):
         """
-        Unique integer identifying an organization.
+        Description of the media type.
 
-        :return: The organization of this Project. 
-        :rtype: int
+        :return: The description of this MediaTypeUpdate. 
+        :rtype: str
         """
-        return self._organization
+        return self._description
 
-    @organization.setter
-    def organization(self, organization):
+    @description.setter
+    def description(self, description):
         """
-        Unique integer identifying an organization.
+        Description of the media type.
 
-        :param organization: The organization of this Project.
-        :type: int
+        :param description: The description of this MediaTypeUpdate.
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                organization is not None and organization < 1):  # noqa: E501
-            raise ValueError("Invalid value for `organization`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._organization = organization
+        self._description = description
 
     @property
-    def permission(self):
+    def elemental_id(self):
         """
-        Permission level of user making request.
+        The elemental ID of the object.
 
-        :return: The permission of this Project. 
+        :return: The elemental_id of this MediaTypeUpdate. 
         :rtype: str
         """
-        return self._permission
+        return self._elemental_id
 
-    @permission.setter
-    def permission(self, permission):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        Permission level of user making request.
+        The elemental ID of the object.
 
-        :param permission: The permission of this Project.
+        :param elemental_id: The elemental_id of this MediaTypeUpdate.
         :type: str
         """
 
-        self._permission = permission
+        self._elemental_id = elemental_id
 
     @property
-    def size(self):
+    def file_format(self):
         """
-        Size of the project in bytes.
+        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
 
-        :return: The size of this Project. 
-        :rtype: int
+        :return: The file_format of this MediaTypeUpdate. 
+        :rtype: str
         """
-        return self._size
+        return self._file_format
 
-    @size.setter
-    def size(self, size):
+    @file_format.setter
+    def file_format(self, file_format):
         """
-        Size of the project in bytes.
+        File extension. If omitted, any recognized file extension for the given dtype is accepted for upload. Do not include a dot prefix.
 
-        :param size: The size of this Project.
-        :type: int
+        :param file_format: The file_format of this MediaTypeUpdate.
+        :type: str
         """
+        if (self.local_vars_configuration.client_side_validation and
+                file_format is not None and len(file_format) > 4):
+            raise ValueError("Invalid value for `file_format`, length must be less than or equal to `4`")  # noqa: E501
 
-        self._size = size
+        self._file_format = file_format
 
     @property
-    def summary(self):
+    def name(self):
         """
-        Summary of the project.
+        Name of the media type.
 
-        :return: The summary of this Project. 
+        :return: The name of this MediaTypeUpdate. 
         :rtype: str
         """
-        return self._summary
+        return self._name
 
-    @summary.setter
-    def summary(self, summary):
+    @name.setter
+    def name(self, name):
         """
-        Summary of the project.
+        Name of the media type.
 
-        :param summary: The summary of this Project.
+        :param name: The name of this MediaTypeUpdate.
         :type: str
         """
 
-        self._summary = summary
+        self._name = name
 
     @property
-    def thumb(self):
+    def streaming_config(self):
         """
-        S3 key of thumbnail used to represent the project.
+        Streaming config definition. If null, the default will be used.
 
-        :return: The thumb of this Project. 
-        :rtype: str
+        :return: The streaming_config of this MediaTypeUpdate. 
+        :rtype: list[ResolutionConfig]
         """
-        return self._thumb
+        return self._streaming_config
 
-    @thumb.setter
-    def thumb(self, thumb):
+    @streaming_config.setter
+    def streaming_config(self, streaming_config):
         """
-        S3 key of thumbnail used to represent the project.
+        Streaming config definition. If null, the default will be used.
 
-        :param thumb: The thumb of this Project.
-        :type: str
+        :param streaming_config: The streaming_config of this MediaTypeUpdate.
+        :type: list[ResolutionConfig]
         """
 
-        self._thumb = thumb
+        self._streaming_config = streaming_config
 
     @property
-    def usernames(self):
+    def visible(self):
         """
-        List of usernames of project members.
+        Visible configuration
 
-        :return: The usernames of this Project. 
-        :rtype: list[str]
+        :return: The visible of this MediaTypeUpdate. 
+        :rtype: bool
         """
-        return self._usernames
+        return self._visible
 
-    @usernames.setter
-    def usernames(self, usernames):
+    @visible.setter
+    def visible(self, visible):
         """
-        List of usernames of project members.
+        Visible configuration
 
-        :param usernames: The usernames of this Project.
-        :type: list[str]
+        :param visible: The visible of this MediaTypeUpdate.
+        :type: bool
         """
 
-        self._usernames = usernames
+        self._visible = visible
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -389,18 +368,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Project):
+        if not isinstance(other, MediaTypeUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Project):
+        if not isinstance(other, MediaTypeUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/project_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/bucket_oci_native_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,148 +14,174 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class ProjectSpec(object):
+class BucketOCINativeConfig(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'enable_downloads': 'bool',
-        'name': 'str',
-        'organization': 'int',
-        'summary': 'str'
+        'fingerprint': 'str',
+        'key_content': 'str',
+        'region': 'str',
+        'tenancy': 'str',
+        'user': 'str'
     }
 
     attribute_map = {
-        'enable_downloads': 'enable_downloads',
-        'name': 'name',
-        'organization': 'organization',
-        'summary': 'summary'
+        'fingerprint': 'fingerprint',
+        'key_content': 'key_content',
+        'region': 'region',
+        'tenancy': 'tenancy',
+        'user': 'user'
     }
 
-    def __init__(self, enable_downloads=True, name=None, organization=None, summary='', local_vars_configuration=None):  # noqa: E501
-        """ProjectSpec - a model defined in OpenAPI"""
+    def __init__(self, fingerprint=None, key_content=None, region=None, tenancy=None, user=None, local_vars_configuration=None):  # noqa: E501
+        """BucketOCINativeConfig - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._enable_downloads = None
-        self._name = None
-        self._organization = None
-        self._summary = None
+        self._fingerprint = None
+        self._key_content = None
+        self._region = None
+        self._tenancy = None
+        self._user = None
         self.discriminator = None
 
-        if enable_downloads is not None:
-            self.enable_downloads = enable_downloads
-        self.name = name
-        self.organization = organization
-        if summary is not None:
-            self.summary = summary
+        self.fingerprint = fingerprint
+        self.key_content = key_content
+        self.region = region
+        self.tenancy = tenancy
+        self.user = user
 
     @property
-    def enable_downloads(self):
+    def fingerprint(self):
         """
-        Whether the UI should allow downloads for this project.
+        Public key fingerprint.
 
-        :return: The enable_downloads of this ProjectSpec. 
-        :rtype: bool
+        :return: The fingerprint of this BucketOCINativeConfig. 
+        :rtype: str
+        """
+        return self._fingerprint
+
+    @fingerprint.setter
+    def fingerprint(self, fingerprint):
+        """
+        Public key fingerprint.
+
+        :param fingerprint: The fingerprint of this BucketOCINativeConfig.
+        :type: str
+        """
+        if self.local_vars_configuration.client_side_validation and fingerprint is None:  # noqa: E501
+            raise ValueError("Invalid value for `fingerprint`, must not be `None`")  # noqa: E501
+
+        self._fingerprint = fingerprint
+
+    @property
+    def key_content(self):
+        """
+        Private key content.
+
+        :return: The key_content of this BucketOCINativeConfig. 
+        :rtype: str
         """
-        return self._enable_downloads
+        return self._key_content
 
-    @enable_downloads.setter
-    def enable_downloads(self, enable_downloads):
+    @key_content.setter
+    def key_content(self, key_content):
         """
-        Whether the UI should allow downloads for this project.
+        Private key content.
 
-        :param enable_downloads: The enable_downloads of this ProjectSpec.
-        :type: bool
+        :param key_content: The key_content of this BucketOCINativeConfig.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and key_content is None:  # noqa: E501
+            raise ValueError("Invalid value for `key_content`, must not be `None`")  # noqa: E501
 
-        self._enable_downloads = enable_downloads
+        self._key_content = key_content
 
     @property
-    def name(self):
+    def region(self):
         """
-        Name of the project.
+        OCI region.
 
-        :return: The name of this ProjectSpec. 
+        :return: The region of this BucketOCINativeConfig. 
         :rtype: str
         """
-        return self._name
+        return self._region
 
-    @name.setter
-    def name(self, name):
+    @region.setter
+    def region(self, region):
         """
-        Name of the project.
+        OCI region.
 
-        :param name: The name of this ProjectSpec.
+        :param region: The region of this BucketOCINativeConfig.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and region is None:  # noqa: E501
+            raise ValueError("Invalid value for `region`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._region = region
 
     @property
-    def organization(self):
+    def tenancy(self):
         """
-        Unique integer identifying an organization.
+        Tenancy OCID.
 
-        :return: The organization of this ProjectSpec. 
-        :rtype: int
+        :return: The tenancy of this BucketOCINativeConfig. 
+        :rtype: str
         """
-        return self._organization
+        return self._tenancy
 
-    @organization.setter
-    def organization(self, organization):
+    @tenancy.setter
+    def tenancy(self, tenancy):
         """
-        Unique integer identifying an organization.
+        Tenancy OCID.
 
-        :param organization: The organization of this ProjectSpec.
-        :type: int
+        :param tenancy: The tenancy of this BucketOCINativeConfig.
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and organization is None:  # noqa: E501
-            raise ValueError("Invalid value for `organization`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                organization is not None and organization < 1):  # noqa: E501
-            raise ValueError("Invalid value for `organization`, must be a value greater than or equal to `1`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and tenancy is None:  # noqa: E501
+            raise ValueError("Invalid value for `tenancy`, must not be `None`")  # noqa: E501
 
-        self._organization = organization
+        self._tenancy = tenancy
 
     @property
-    def summary(self):
+    def user(self):
         """
-        Summary of the project.
+        User OCID.
 
-        :return: The summary of this ProjectSpec. 
+        :return: The user of this BucketOCINativeConfig. 
         :rtype: str
         """
-        return self._summary
+        return self._user
 
-    @summary.setter
-    def summary(self, summary):
+    @user.setter
+    def user(self, user):
         """
-        Summary of the project.
+        User OCID.
 
-        :param summary: The summary of this ProjectSpec.
+        :param user: The user of this BucketOCINativeConfig.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and user is None:  # noqa: E501
+            raise ValueError("Invalid value for `user`, must not be `None`")  # noqa: E501
 
-        self._summary = summary
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -183,18 +209,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectSpec):
+        if not isinstance(other, BucketOCINativeConfig):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProjectSpec):
+        if not isinstance(other, BucketOCINativeConfig):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/project_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/leaf_id_query.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,143 +14,115 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class ProjectUpdate(object):
+class LeafIdQuery(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'enable_downloads': 'bool',
-        'name': 'str',
-        'summary': 'str',
-        'thumb': 'str'
+        'float_array': 'list[FloatArrayQuery]',
+        'ids': 'list[int]',
+        'object_search': 'AttributeOperationSpec'
     }
 
     attribute_map = {
-        'enable_downloads': 'enable_downloads',
-        'name': 'name',
-        'summary': 'summary',
-        'thumb': 'thumb'
+        'float_array': 'float_array',
+        'ids': 'ids',
+        'object_search': 'object_search'
     }
 
-    def __init__(self, enable_downloads=True, name=None, summary='', thumb=None, local_vars_configuration=None):  # noqa: E501
-        """ProjectUpdate - a model defined in OpenAPI"""
+    def __init__(self, float_array=None, ids=None, object_search=None, local_vars_configuration=None):  # noqa: E501
+        """LeafIdQuery - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._enable_downloads = None
-        self._name = None
-        self._summary = None
-        self._thumb = None
+        self._float_array = None
+        self._ids = None
+        self._object_search = None
         self.discriminator = None
 
-        if enable_downloads is not None:
-            self.enable_downloads = enable_downloads
-        if name is not None:
-            self.name = name
-        if summary is not None:
-            self.summary = summary
-        if thumb is not None:
-            self.thumb = thumb
+        if float_array is not None:
+            self.float_array = float_array
+        if ids is not None:
+            self.ids = ids
+        if object_search is not None:
+            self.object_search = object_search
 
     @property
-    def enable_downloads(self):
+    def float_array(self):
         """
-        Whether the UI should allow downloads for this project.
+        Searches on `float_array` attributes.
 
-        :return: The enable_downloads of this ProjectUpdate. 
-        :rtype: bool
+        :return: The float_array of this LeafIdQuery. 
+        :rtype: list[FloatArrayQuery]
         """
-        return self._enable_downloads
+        return self._float_array
 
-    @enable_downloads.setter
-    def enable_downloads(self, enable_downloads):
+    @float_array.setter
+    def float_array(self, float_array):
         """
-        Whether the UI should allow downloads for this project.
+        Searches on `float_array` attributes.
 
-        :param enable_downloads: The enable_downloads of this ProjectUpdate.
-        :type: bool
+        :param float_array: The float_array of this LeafIdQuery.
+        :type: list[FloatArrayQuery]
         """
 
-        self._enable_downloads = enable_downloads
+        self._float_array = float_array
 
     @property
-    def name(self):
+    def ids(self):
         """
-        Name of the project.
+        Array of leaf IDs to retrieve.
 
-        :return: The name of this ProjectUpdate. 
-        :rtype: str
+        :return: The ids of this LeafIdQuery. 
+        :rtype: list[int]
         """
-        return self._name
+        return self._ids
 
-    @name.setter
-    def name(self, name):
+    @ids.setter
+    def ids(self, ids):
         """
-        Name of the project.
+        Array of leaf IDs to retrieve.
 
-        :param name: The name of this ProjectUpdate.
-        :type: str
+        :param ids: The ids of this LeafIdQuery.
+        :type: list[int]
         """
 
-        self._name = name
+        self._ids = ids
 
     @property
-    def summary(self):
+    def object_search(self):
         """
-        Summary of the project.
 
-        :return: The summary of this ProjectUpdate. 
-        :rtype: str
+        :return: The object_search of this LeafIdQuery. 
+        :rtype: AttributeOperationSpec
         """
-        return self._summary
+        return self._object_search
 
-    @summary.setter
-    def summary(self, summary):
+    @object_search.setter
+    def object_search(self, object_search):
         """
-        Summary of the project.
 
-        :param summary: The summary of this ProjectUpdate.
-        :type: str
+        :param object_search: The object_search of this LeafIdQuery.
+        :type: AttributeOperationSpec
         """
 
-        self._summary = summary
-
-    @property
-    def thumb(self):
-        """
-        S3 key of thumbnail used to represent the project.
-
-        :return: The thumb of this ProjectUpdate. 
-        :rtype: str
-        """
-        return self._thumb
-
-    @thumb.setter
-    def thumb(self, thumb):
-        """
-        S3 key of thumbnail used to represent the project.
-
-        :param thumb: The thumb of this ProjectUpdate.
-        :type: str
-        """
-
-        self._thumb = thumb
+        self._object_search = object_search
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -178,18 +150,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectUpdate):
+        if not isinstance(other, LeafIdQuery):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProjectUpdate):
+        if not isinstance(other, LeafIdQuery):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/resolution_config.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/resolution_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,37 +27,42 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'crf': 'int',
+        'preset': 'str',
         'resolution': 'int',
         'vcodec': 'str'
     }
 
     attribute_map = {
         'crf': 'crf',
+        'preset': 'preset',
         'resolution': 'resolution',
         'vcodec': 'vcodec'
     }
 
-    def __init__(self, crf=23, resolution=None, vcodec='h264', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, crf=23, preset='', resolution=None, vcodec='h264', local_vars_configuration=None):  # noqa: E501
         """ResolutionConfig - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._crf = None
+        self._preset = None
         self._resolution = None
         self._vcodec = None
         self.discriminator = None
 
         if crf is not None:
             self.crf = crf
+        if preset is not None:
+            self.preset = preset
         if resolution is not None:
             self.resolution = resolution
         if vcodec is not None:
             self.vcodec = vcodec
 
     @property
     def crf(self):
@@ -74,23 +79,44 @@
         """
         Constant rate factor.
 
         :param crf: The crf of this ResolutionConfig.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
-                crf is not None and crf > 51):  # noqa: E501
-            raise ValueError("Invalid value for `crf`, must be a value less than or equal to `51`")  # noqa: E501
+                crf is not None and crf > 63):  # noqa: E501
+            raise ValueError("Invalid value for `crf`, must be a value less than or equal to `63`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 crf is not None and crf < 0):  # noqa: E501
             raise ValueError("Invalid value for `crf`, must be a value greater than or equal to `0`")  # noqa: E501
 
         self._crf = crf
 
     @property
+    def preset(self):
+        """
+        Codec Specific Preset (e.g. fast, medium, or 0,1,2)
+
+        :return: The preset of this ResolutionConfig. 
+        :rtype: str
+        """
+        return self._preset
+
+    @preset.setter
+    def preset(self, preset):
+        """
+        Codec Specific Preset (e.g. fast, medium, or 0,1,2)
+
+        :param preset: The preset of this ResolutionConfig.
+        :type: str
+        """
+
+        self._preset = preset
+
+    @property
     def resolution(self):
         """
         Vertical Resolution
 
         :return: The resolution of this ResolutionConfig. 
         :rtype: int
         """
@@ -101,16 +127,16 @@
         """
         Vertical Resolution
 
         :param resolution: The resolution of this ResolutionConfig.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
-                resolution is not None and resolution > 4096):  # noqa: E501
-            raise ValueError("Invalid value for `resolution`, must be a value less than or equal to `4096`")  # noqa: E501
+                resolution is not None and resolution > 8192):  # noqa: E501
+            raise ValueError("Invalid value for `resolution`, must be a value less than or equal to `8192`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 resolution is not None and resolution < 0):  # noqa: E501
             raise ValueError("Invalid value for `resolution`, must be a value greater than or equal to `0`")  # noqa: E501
 
         self._resolution = resolution
 
     @property
@@ -127,15 +153,15 @@
     def vcodec(self, vcodec):
         """
         Video codec.
 
         :param vcodec: The vcodec of this ResolutionConfig.
         :type: str
         """
-        allowed_values = ["h264"]  # noqa: E501
+        allowed_values = ["h264", "av1"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and vcodec not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `vcodec` ({0}), must be one of {1}"  # noqa: E501
                 .format(vcodec, allowed_values)
             )
 
         self._vcodec = vcodec
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/s3_storage_config.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/s3_storage_config.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/section.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/section.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,88 +26,87 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'annotation_bools': 'list[dict(str, object)]',
+        'elemental_id': 'str',
         'id': 'int',
-        'lucene_string': 'str',
-        'media_bools': 'list[dict(str, object)]',
         'name': 'str',
+        'object_search': 'AttributeOperationSpec',
         'project': 'int',
+        'related_search': 'AttributeOperationSpec',
         'tator_user_sections': 'str',
         'visible': 'bool'
     }
 
     attribute_map = {
-        'annotation_bools': 'annotation_bools',
+        'elemental_id': 'elemental_id',
         'id': 'id',
-        'lucene_string': 'lucene_string',
-        'media_bools': 'media_bools',
         'name': 'name',
+        'object_search': 'object_search',
         'project': 'project',
+        'related_search': 'related_search',
         'tator_user_sections': 'tator_user_sections',
         'visible': 'visible'
     }
 
-    def __init__(self, annotation_bools=None, id=None, lucene_string=None, media_bools=None, name=None, project=None, tator_user_sections=None, visible=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, elemental_id=None, id=None, name=None, object_search=None, project=None, related_search=None, tator_user_sections=None, visible=None, local_vars_configuration=None):  # noqa: E501
         """Section - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._annotation_bools = None
+        self._elemental_id = None
         self._id = None
-        self._lucene_string = None
-        self._media_bools = None
         self._name = None
+        self._object_search = None
         self._project = None
+        self._related_search = None
         self._tator_user_sections = None
         self._visible = None
         self.discriminator = None
 
-        if annotation_bools is not None:
-            self.annotation_bools = annotation_bools
+        self.elemental_id = elemental_id
         if id is not None:
             self.id = id
-        if lucene_string is not None:
-            self.lucene_string = lucene_string
-        if media_bools is not None:
-            self.media_bools = media_bools
         if name is not None:
             self.name = name
+        if object_search is not None:
+            self.object_search = object_search
         if project is not None:
             self.project = project
+        if related_search is not None:
+            self.related_search = related_search
         if tator_user_sections is not None:
             self.tator_user_sections = tator_user_sections
         if visible is not None:
             self.visible = visible
 
     @property
-    def annotation_bools(self):
+    def elemental_id(self):
         """
-        List of elasticsearch boolean queries that should be applied to annotations. These are applied to the boolean query \"filter\" list.
+        The elemental ID of the object.
 
-        :return: The annotation_bools of this Section. 
-        :rtype: list[dict(str, object)]
+        :return: The elemental_id of this Section. 
+        :rtype: str
         """
-        return self._annotation_bools
+        return self._elemental_id
 
-    @annotation_bools.setter
-    def annotation_bools(self, annotation_bools):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        List of elasticsearch boolean queries that should be applied to annotations. These are applied to the boolean query \"filter\" list.
+        The elemental ID of the object.
 
-        :param annotation_bools: The annotation_bools of this Section.
-        :type: list[dict(str, object)]
+        :param elemental_id: The elemental_id of this Section.
+        :type: str
         """
 
-        self._annotation_bools = annotation_bools
+        self._elemental_id = elemental_id
 
     @property
     def id(self):
         """
         Unique integer identifying the section.
 
         :return: The id of this Section. 
@@ -123,75 +122,52 @@
         :param id: The id of this Section.
         :type: int
         """
 
         self._id = id
 
     @property
-    def lucene_string(self):
+    def name(self):
         """
-        Lucene query syntax search string.
+        Unique name of the section.
 
-        :return: The lucene_string of this Section. 
+        :return: The name of this Section. 
         :rtype: str
         """
-        return self._lucene_string
+        return self._name
 
-    @lucene_string.setter
-    def lucene_string(self, lucene_string):
+    @name.setter
+    def name(self, name):
         """
-        Lucene query syntax search string.
+        Unique name of the section.
 
-        :param lucene_string: The lucene_string of this Section.
+        :param name: The name of this Section.
         :type: str
         """
 
-        self._lucene_string = lucene_string
-
-    @property
-    def media_bools(self):
-        """
-        List of elasticsearch boolean queries that should be applied to media. These are applied to the boolean query \"filter\" list.
-
-        :return: The media_bools of this Section. 
-        :rtype: list[dict(str, object)]
-        """
-        return self._media_bools
-
-    @media_bools.setter
-    def media_bools(self, media_bools):
-        """
-        List of elasticsearch boolean queries that should be applied to media. These are applied to the boolean query \"filter\" list.
-
-        :param media_bools: The media_bools of this Section.
-        :type: list[dict(str, object)]
-        """
-
-        self._media_bools = media_bools
+        self._name = name
 
     @property
-    def name(self):
+    def object_search(self):
         """
-        Unique name of the algorithm workflow.
 
-        :return: The name of this Section. 
-        :rtype: str
+        :return: The object_search of this Section. 
+        :rtype: AttributeOperationSpec
         """
-        return self._name
+        return self._object_search
 
-    @name.setter
-    def name(self, name):
+    @object_search.setter
+    def object_search(self, object_search):
         """
-        Unique name of the algorithm workflow.
 
-        :param name: The name of this Section.
-        :type: str
+        :param object_search: The object_search of this Section.
+        :type: AttributeOperationSpec
         """
 
-        self._name = name
+        self._object_search = object_search
 
     @property
     def project(self):
         """
         Unique integer identifying the project associated with the section.
 
         :return: The project of this Section. 
@@ -207,14 +183,33 @@
         :param project: The project of this Section.
         :type: int
         """
 
         self._project = project
 
     @property
+    def related_search(self):
+        """
+
+        :return: The related_search of this Section. 
+        :rtype: AttributeOperationSpec
+        """
+        return self._related_search
+
+    @related_search.setter
+    def related_search(self, related_search):
+        """
+
+        :param related_search: The related_search of this Section.
+        :type: AttributeOperationSpec
+        """
+
+        self._related_search = related_search
+
+    @property
     def tator_user_sections(self):
         """
         Attribute that is applied to media to identify membership to a section.
 
         :return: The tator_user_sections of this Section. 
         :rtype: str
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/section_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/section_spec.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,142 +26,137 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'annotation_bools': 'list[dict(str, object)]',
-        'lucene_string': 'str',
-        'media_bools': 'list[dict(str, object)]',
+        'elemental_id': 'str',
         'name': 'str',
+        'object_search': 'AttributeOperationSpec',
+        'related_search': 'AttributeOperationSpec',
         'tator_user_sections': 'str',
         'visible': 'bool'
     }
 
     attribute_map = {
-        'annotation_bools': 'annotation_bools',
-        'lucene_string': 'lucene_string',
-        'media_bools': 'media_bools',
+        'elemental_id': 'elemental_id',
         'name': 'name',
+        'object_search': 'object_search',
+        'related_search': 'related_search',
         'tator_user_sections': 'tator_user_sections',
         'visible': 'visible'
     }
 
-    def __init__(self, annotation_bools=None, lucene_string=None, media_bools=None, name=None, tator_user_sections=None, visible=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, elemental_id=None, name=None, object_search=None, related_search=None, tator_user_sections=None, visible=None, local_vars_configuration=None):  # noqa: E501
         """SectionSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._annotation_bools = None
-        self._lucene_string = None
-        self._media_bools = None
+        self._elemental_id = None
         self._name = None
+        self._object_search = None
+        self._related_search = None
         self._tator_user_sections = None
         self._visible = None
         self.discriminator = None
 
-        if annotation_bools is not None:
-            self.annotation_bools = annotation_bools
-        if lucene_string is not None:
-            self.lucene_string = lucene_string
-        if media_bools is not None:
-            self.media_bools = media_bools
+        self.elemental_id = elemental_id
         self.name = name
+        if object_search is not None:
+            self.object_search = object_search
+        if related_search is not None:
+            self.related_search = related_search
         if tator_user_sections is not None:
             self.tator_user_sections = tator_user_sections
         if visible is not None:
             self.visible = visible
 
     @property
-    def annotation_bools(self):
+    def elemental_id(self):
         """
-        List of elasticsearch boolean queries that should be applied to annotations. These are applied to the boolean query \"filter\" list.
+        The elemental ID of the object.
 
-        :return: The annotation_bools of this SectionSpec. 
-        :rtype: list[dict(str, object)]
+        :return: The elemental_id of this SectionSpec. 
+        :rtype: str
         """
-        return self._annotation_bools
+        return self._elemental_id
 
-    @annotation_bools.setter
-    def annotation_bools(self, annotation_bools):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        List of elasticsearch boolean queries that should be applied to annotations. These are applied to the boolean query \"filter\" list.
+        The elemental ID of the object.
 
-        :param annotation_bools: The annotation_bools of this SectionSpec.
-        :type: list[dict(str, object)]
+        :param elemental_id: The elemental_id of this SectionSpec.
+        :type: str
         """
 
-        self._annotation_bools = annotation_bools
+        self._elemental_id = elemental_id
 
     @property
-    def lucene_string(self):
+    def name(self):
         """
-        Lucene query syntax search string.
+        Unique name of the section.
 
-        :return: The lucene_string of this SectionSpec. 
+        :return: The name of this SectionSpec. 
         :rtype: str
         """
-        return self._lucene_string
+        return self._name
 
-    @lucene_string.setter
-    def lucene_string(self, lucene_string):
+    @name.setter
+    def name(self, name):
         """
-        Lucene query syntax search string.
+        Unique name of the section.
 
-        :param lucene_string: The lucene_string of this SectionSpec.
+        :param name: The name of this SectionSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._lucene_string = lucene_string
+        self._name = name
 
     @property
-    def media_bools(self):
+    def object_search(self):
         """
-        List of elasticsearch boolean queries that should be applied to media. These are applied to the boolean query \"filter\" list.
 
-        :return: The media_bools of this SectionSpec. 
-        :rtype: list[dict(str, object)]
+        :return: The object_search of this SectionSpec. 
+        :rtype: AttributeOperationSpec
         """
-        return self._media_bools
+        return self._object_search
 
-    @media_bools.setter
-    def media_bools(self, media_bools):
+    @object_search.setter
+    def object_search(self, object_search):
         """
-        List of elasticsearch boolean queries that should be applied to media. These are applied to the boolean query \"filter\" list.
 
-        :param media_bools: The media_bools of this SectionSpec.
-        :type: list[dict(str, object)]
+        :param object_search: The object_search of this SectionSpec.
+        :type: AttributeOperationSpec
         """
 
-        self._media_bools = media_bools
+        self._object_search = object_search
 
     @property
-    def name(self):
+    def related_search(self):
         """
-        Unique name of the algorithm workflow.
 
-        :return: The name of this SectionSpec. 
-        :rtype: str
+        :return: The related_search of this SectionSpec. 
+        :rtype: AttributeOperationSpec
         """
-        return self._name
+        return self._related_search
 
-    @name.setter
-    def name(self, name):
+    @related_search.setter
+    def related_search(self, related_search):
         """
-        Unique name of the algorithm workflow.
 
-        :param name: The name of this SectionSpec.
-        :type: str
+        :param related_search: The related_search of this SectionSpec.
+        :type: AttributeOperationSpec
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._related_search = related_search
 
     @property
     def tator_user_sections(self):
         """
         Attribute that is applied to media to identify membership to a section.
 
         :return: The tator_user_sections of this SectionSpec.
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/section_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,195 +14,273 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class SectionUpdate(object):
+class Version(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'annotation_bools': 'list[dict(str, object)]',
-        'lucene_string': 'str',
-        'media_bools': 'list[dict(str, object)]',
+        'bases': 'list[int]',
+        'created_by': 'str',
+        'description': 'str',
+        'elemental_id': 'str',
+        'id': 'int',
         'name': 'str',
-        'tator_user_sections': 'str',
-        'visible': 'bool'
+        'number': 'int',
+        'project': 'int',
+        'show_empty': 'bool'
     }
 
     attribute_map = {
-        'annotation_bools': 'annotation_bools',
-        'lucene_string': 'lucene_string',
-        'media_bools': 'media_bools',
+        'bases': 'bases',
+        'created_by': 'created_by',
+        'description': 'description',
+        'elemental_id': 'elemental_id',
+        'id': 'id',
         'name': 'name',
-        'tator_user_sections': 'tator_user_sections',
-        'visible': 'visible'
+        'number': 'number',
+        'project': 'project',
+        'show_empty': 'show_empty'
     }
 
-    def __init__(self, annotation_bools=None, lucene_string=None, media_bools=None, name=None, tator_user_sections=None, visible=None, local_vars_configuration=None):  # noqa: E501
-        """SectionUpdate - a model defined in OpenAPI"""
+    def __init__(self, bases=None, created_by=None, description='', elemental_id=None, id=None, name=None, number=None, project=None, show_empty=True, local_vars_configuration=None):  # noqa: E501
+        """Version - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._annotation_bools = None
-        self._lucene_string = None
-        self._media_bools = None
+        self._bases = None
+        self._created_by = None
+        self._description = None
+        self._elemental_id = None
+        self._id = None
         self._name = None
-        self._tator_user_sections = None
-        self._visible = None
+        self._number = None
+        self._project = None
+        self._show_empty = None
         self.discriminator = None
 
-        if annotation_bools is not None:
-            self.annotation_bools = annotation_bools
-        if lucene_string is not None:
-            self.lucene_string = lucene_string
-        if media_bools is not None:
-            self.media_bools = media_bools
+        if bases is not None:
+            self.bases = bases
+        if created_by is not None:
+            self.created_by = created_by
+        if description is not None:
+            self.description = description
+        if elemental_id is not None:
+            self.elemental_id = elemental_id
+        if id is not None:
+            self.id = id
         if name is not None:
             self.name = name
-        if tator_user_sections is not None:
-            self.tator_user_sections = tator_user_sections
-        if visible is not None:
-            self.visible = visible
+        if number is not None:
+            self.number = number
+        if project is not None:
+            self.project = project
+        if show_empty is not None:
+            self.show_empty = show_empty
 
     @property
-    def annotation_bools(self):
+    def bases(self):
         """
-        List of elasticsearch boolean queries that should be applied to annotations. These are applied to the boolean query \"filter\" list.
+        Array of other version IDs that are dependencies of this version.
 
-        :return: The annotation_bools of this SectionUpdate. 
-        :rtype: list[dict(str, object)]
+        :return: The bases of this Version. 
+        :rtype: list[int]
         """
-        return self._annotation_bools
+        return self._bases
 
-    @annotation_bools.setter
-    def annotation_bools(self, annotation_bools):
+    @bases.setter
+    def bases(self, bases):
         """
-        List of elasticsearch boolean queries that should be applied to annotations. These are applied to the boolean query \"filter\" list.
+        Array of other version IDs that are dependencies of this version.
 
-        :param annotation_bools: The annotation_bools of this SectionUpdate.
-        :type: list[dict(str, object)]
+        :param bases: The bases of this Version.
+        :type: list[int]
         """
 
-        self._annotation_bools = annotation_bools
+        self._bases = bases
 
     @property
-    def lucene_string(self):
+    def created_by(self):
         """
-        Lucene query syntax search string.
+        Name of user who created the last unmodified annotation in this version.
 
-        :return: The lucene_string of this SectionUpdate. 
+        :return: The created_by of this Version. 
         :rtype: str
         """
-        return self._lucene_string
+        return self._created_by
 
-    @lucene_string.setter
-    def lucene_string(self, lucene_string):
+    @created_by.setter
+    def created_by(self, created_by):
         """
-        Lucene query syntax search string.
+        Name of user who created the last unmodified annotation in this version.
 
-        :param lucene_string: The lucene_string of this SectionUpdate.
+        :param created_by: The created_by of this Version.
         :type: str
         """
 
-        self._lucene_string = lucene_string
+        self._created_by = created_by
 
     @property
-    def media_bools(self):
+    def description(self):
         """
-        List of elasticsearch boolean queries that should be applied to media. These are applied to the boolean query \"filter\" list.
+        Description of the version.
 
-        :return: The media_bools of this SectionUpdate. 
-        :rtype: list[dict(str, object)]
+        :return: The description of this Version. 
+        :rtype: str
+        """
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """
+        Description of the version.
+
+        :param description: The description of this Version.
+        :type: str
+        """
+
+        self._description = description
+
+    @property
+    def elemental_id(self):
+        """
+        Unique ID of an element
+
+        :return: The elemental_id of this Version. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        Unique ID of an element
+
+        :param elemental_id: The elemental_id of this Version.
+        :type: str
         """
-        return self._media_bools
 
-    @media_bools.setter
-    def media_bools(self, media_bools):
+        self._elemental_id = elemental_id
+
+    @property
+    def id(self):
         """
-        List of elasticsearch boolean queries that should be applied to media. These are applied to the boolean query \"filter\" list.
+        Unique integer identifying a membership.
 
-        :param media_bools: The media_bools of this SectionUpdate.
-        :type: list[dict(str, object)]
+        :return: The id of this Version. 
+        :rtype: int
         """
+        return self._id
 
-        self._media_bools = media_bools
+    @id.setter
+    def id(self, id):
+        """
+        Unique integer identifying a membership.
+
+        :param id: The id of this Version.
+        :type: int
+        """
+
+        self._id = id
 
     @property
     def name(self):
         """
-        Unique name of the algorithm workflow.
+        Name of the version.
 
-        :return: The name of this SectionUpdate. 
+        :return: The name of this Version. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Unique name of the algorithm workflow.
+        Name of the version.
 
-        :param name: The name of this SectionUpdate.
+        :param name: The name of this Version.
         :type: str
         """
 
         self._name = name
 
     @property
-    def tator_user_sections(self):
+    def number(self):
         """
-        Attribute that is applied to media to identify membership to a section.
+        Version number.
 
-        :return: The tator_user_sections of this SectionUpdate. 
-        :rtype: str
+        :return: The number of this Version. 
+        :rtype: int
         """
-        return self._tator_user_sections
+        return self._number
 
-    @tator_user_sections.setter
-    def tator_user_sections(self, tator_user_sections):
+    @number.setter
+    def number(self, number):
         """
-        Attribute that is applied to media to identify membership to a section.
+        Version number.
 
-        :param tator_user_sections: The tator_user_sections of this SectionUpdate.
-        :type: str
+        :param number: The number of this Version.
+        :type: int
+        """
+
+        self._number = number
+
+    @property
+    def project(self):
+        """
+        Unique integer identifying a project.
+
+        :return: The project of this Version. 
+        :rtype: int
+        """
+        return self._project
+
+    @project.setter
+    def project(self, project):
+        """
+        Unique integer identifying a project.
+
+        :param project: The project of this Version.
+        :type: int
         """
 
-        self._tator_user_sections = tator_user_sections
+        self._project = project
 
     @property
-    def visible(self):
+    def show_empty(self):
         """
-        Determines the visibility in the UI.
+        Whether to show this version on media for which no annotations exist.
 
-        :return: The visible of this SectionUpdate. 
+        :return: The show_empty of this Version. 
         :rtype: bool
         """
-        return self._visible
+        return self._show_empty
 
-    @visible.setter
-    def visible(self, visible):
+    @show_empty.setter
+    def show_empty(self, show_empty):
         """
-        Determines the visibility in the UI.
+        Whether to show this version on media for which no annotations exist.
 
-        :param visible: The visible of this SectionUpdate.
+        :param show_empty: The show_empty of this Version.
         :type: bool
         """
 
-        self._visible = visible
+        self._show_empty = show_empty
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -230,18 +308,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SectionUpdate):
+        if not isinstance(other, Version):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SectionUpdate):
+        if not isinstance(other, Version):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/state.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,82 +29,95 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'attributes': 'dict(str, object)',
         'created_by': 'int',
         'created_datetime': 'datetime',
+        'elemental_id': 'str',
         'frame': 'int',
         'id': 'int',
         'localizations': 'list[int]',
         'media': 'list[int]',
-        'meta': 'int',
         'modified_by': 'int',
         'modified_datetime': 'datetime',
+        'parent': 'float',
         'segments': 'list[list[int]]',
+        'type': 'int',
+        'variant_deleted': 'bool',
         'version': 'int'
     }
 
     attribute_map = {
         'attributes': 'attributes',
         'created_by': 'created_by',
         'created_datetime': 'created_datetime',
+        'elemental_id': 'elemental_id',
         'frame': 'frame',
         'id': 'id',
         'localizations': 'localizations',
         'media': 'media',
-        'meta': 'meta',
         'modified_by': 'modified_by',
         'modified_datetime': 'modified_datetime',
+        'parent': 'parent',
         'segments': 'segments',
+        'type': 'type',
+        'variant_deleted': 'variant_deleted',
         'version': 'version'
     }
 
-    def __init__(self, attributes=None, created_by=None, created_datetime=None, frame=None, id=None, localizations=None, media=None, meta=None, modified_by=None, modified_datetime=None, segments=None, version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, created_by=None, created_datetime=None, elemental_id=None, frame=None, id=None, localizations=None, media=None, modified_by=None, modified_datetime=None, parent=None, segments=None, type=None, variant_deleted=None, version=None, local_vars_configuration=None):  # noqa: E501
         """State - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
         self._created_by = None
         self._created_datetime = None
+        self._elemental_id = None
         self._frame = None
         self._id = None
         self._localizations = None
         self._media = None
-        self._meta = None
         self._modified_by = None
         self._modified_datetime = None
+        self._parent = None
         self._segments = None
+        self._type = None
+        self._variant_deleted = None
         self._version = None
         self.discriminator = None
 
         if attributes is not None:
             self.attributes = attributes
         if created_by is not None:
             self.created_by = created_by
         if created_datetime is not None:
             self.created_datetime = created_datetime
+        self.elemental_id = elemental_id
         if frame is not None:
             self.frame = frame
         if id is not None:
             self.id = id
         if localizations is not None:
             self.localizations = localizations
         if media is not None:
             self.media = media
-        if meta is not None:
-            self.meta = meta
         if modified_by is not None:
             self.modified_by = modified_by
         if modified_datetime is not None:
             self.modified_datetime = modified_datetime
+        self.parent = parent
         if segments is not None:
             self.segments = segments
+        if type is not None:
+            self.type = type
+        if variant_deleted is not None:
+            self.variant_deleted = variant_deleted
         if version is not None:
             self.version = version
 
     @property
     def attributes(self):
         """
         Object containing attribute values.
@@ -164,14 +177,35 @@
         :param created_datetime: The created_datetime of this State.
         :type: datetime
         """
 
         self._created_datetime = created_datetime
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this State. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this State.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def frame(self):
         """
         Frame number this state applies to.
 
         :return: The frame of this State. 
         :rtype: int
         """
@@ -248,35 +282,14 @@
         :param media: The media of this State.
         :type: list[int]
         """
 
         self._media = media
 
     @property
-    def meta(self):
-        """
-        Unique integer identifying the entity type.
-
-        :return: The meta of this State. 
-        :rtype: int
-        """
-        return self._meta
-
-    @meta.setter
-    def meta(self, meta):
-        """
-        Unique integer identifying the entity type.
-
-        :param meta: The meta of this State.
-        :type: int
-        """
-
-        self._meta = meta
-
-    @property
     def modified_by(self):
         """
         Unique integer identifying the user who last modified this state.
 
         :return: The modified_by of this State. 
         :rtype: int
         """
@@ -311,14 +324,35 @@
         :param modified_datetime: The modified_datetime of this State.
         :type: datetime
         """
 
         self._modified_datetime = modified_datetime
 
     @property
+    def parent(self):
+        """
+        If a clone, the pk of the parent.
+
+        :return: The parent of this State. 
+        :rtype: float
+        """
+        return self._parent
+
+    @parent.setter
+    def parent(self, parent):
+        """
+        If a clone, the pk of the parent.
+
+        :param parent: The parent of this State.
+        :type: float
+        """
+
+        self._parent = parent
+
+    @property
     def segments(self):
         """
         List of contiguous frame ranges where a localization associated state has localization data.
 
         :return: The segments of this State. 
         :rtype: list[list[int]]
         """
@@ -332,14 +366,56 @@
         :param segments: The segments of this State.
         :type: list[list[int]]
         """
 
         self._segments = segments
 
     @property
+    def type(self):
+        """
+        Unique integer identifying the entity type.
+
+        :return: The type of this State. 
+        :rtype: int
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """
+        Unique integer identifying the entity type.
+
+        :param type: The type of this State.
+        :type: int
+        """
+
+        self._type = type
+
+    @property
+    def variant_deleted(self):
+        """
+        Unique integer identifying the user who created this localization.
+
+        :return: The variant_deleted of this State. 
+        :rtype: bool
+        """
+        return self._variant_deleted
+
+    @variant_deleted.setter
+    def variant_deleted(self, variant_deleted):
+        """
+        Unique integer identifying the user who created this localization.
+
+        :param variant_deleted: The variant_deleted of this State.
+        :type: bool
+        """
+
+        self._variant_deleted = variant_deleted
+
+    @property
     def version(self):
         """
         Unique integer identifying the version.
 
         :return: The version of this State. 
         :rtype: int
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/state_merge_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state_merge_update.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/state_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/section_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,171 +14,190 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class StateSpec(object):
+class SectionUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'frame': 'int',
-        'localization_ids': 'list[int]',
-        'media_ids': 'list[int]',
-        'type': 'int',
-        'version': 'int'
+        'elemental_id': 'str',
+        'name': 'str',
+        'object_search': 'AttributeOperationSpec',
+        'related_search': 'AttributeOperationSpec',
+        'tator_user_sections': 'str',
+        'visible': 'bool'
     }
 
     attribute_map = {
-        'frame': 'frame',
-        'localization_ids': 'localization_ids',
-        'media_ids': 'media_ids',
-        'type': 'type',
-        'version': 'version'
+        'elemental_id': 'elemental_id',
+        'name': 'name',
+        'object_search': 'object_search',
+        'related_search': 'related_search',
+        'tator_user_sections': 'tator_user_sections',
+        'visible': 'visible'
     }
 
-    def __init__(self, frame=None, localization_ids=None, media_ids=None, type=None, version=None, local_vars_configuration=None):  # noqa: E501
-        """StateSpec - a model defined in OpenAPI"""
+    def __init__(self, elemental_id=None, name=None, object_search=None, related_search=None, tator_user_sections=None, visible=None, local_vars_configuration=None):  # noqa: E501
+        """SectionUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._frame = None
-        self._localization_ids = None
-        self._media_ids = None
-        self._type = None
-        self._version = None
+        self._elemental_id = None
+        self._name = None
+        self._object_search = None
+        self._related_search = None
+        self._tator_user_sections = None
+        self._visible = None
         self.discriminator = None
 
-        if frame is not None:
-            self.frame = frame
-        if localization_ids is not None:
-            self.localization_ids = localization_ids
-        self.media_ids = media_ids
-        self.type = type
-        if version is not None:
-            self.version = version
+        self.elemental_id = elemental_id
+        if name is not None:
+            self.name = name
+        if object_search is not None:
+            self.object_search = object_search
+        if related_search is not None:
+            self.related_search = related_search
+        if tator_user_sections is not None:
+            self.tator_user_sections = tator_user_sections
+        if visible is not None:
+            self.visible = visible
 
     @property
-    def frame(self):
+    def elemental_id(self):
         """
-        Frame number this state applies to.
+        The elemental ID of the object.
 
-        :return: The frame of this StateSpec. 
-        :rtype: int
+        :return: The elemental_id of this SectionUpdate. 
+        :rtype: str
         """
-        return self._frame
+        return self._elemental_id
 
-    @frame.setter
-    def frame(self, frame):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        Frame number this state applies to.
+        The elemental ID of the object.
 
-        :param frame: The frame of this StateSpec.
-        :type: int
+        :param elemental_id: The elemental_id of this SectionUpdate.
+        :type: str
         """
 
-        self._frame = frame
+        self._elemental_id = elemental_id
 
     @property
-    def localization_ids(self):
+    def name(self):
         """
-        List of localization IDs that this state applies to.
+        Unique name of the section.
 
-        :return: The localization_ids of this StateSpec. 
-        :rtype: list[int]
+        :return: The name of this SectionUpdate. 
+        :rtype: str
         """
-        return self._localization_ids
+        return self._name
 
-    @localization_ids.setter
-    def localization_ids(self, localization_ids):
+    @name.setter
+    def name(self, name):
         """
-        List of localization IDs that this state applies to.
+        Unique name of the section.
 
-        :param localization_ids: The localization_ids of this StateSpec.
-        :type: list[int]
+        :param name: The name of this SectionUpdate.
+        :type: str
         """
 
-        self._localization_ids = localization_ids
+        self._name = name
 
     @property
-    def media_ids(self):
+    def object_search(self):
         """
-        List of media IDs that this state applies to.
 
-        :return: The media_ids of this StateSpec. 
-        :rtype: list[int]
+        :return: The object_search of this SectionUpdate. 
+        :rtype: AttributeOperationSpec
         """
-        return self._media_ids
+        return self._object_search
 
-    @media_ids.setter
-    def media_ids(self, media_ids):
+    @object_search.setter
+    def object_search(self, object_search):
         """
-        List of media IDs that this state applies to.
 
-        :param media_ids: The media_ids of this StateSpec.
-        :type: list[int]
+        :param object_search: The object_search of this SectionUpdate.
+        :type: AttributeOperationSpec
         """
-        if self.local_vars_configuration.client_side_validation and media_ids is None:  # noqa: E501
-            raise ValueError("Invalid value for `media_ids`, must not be `None`")  # noqa: E501
 
-        self._media_ids = media_ids
+        self._object_search = object_search
 
     @property
-    def type(self):
+    def related_search(self):
         """
-        Unique integer identifying a state type.
 
-        :return: The type of this StateSpec. 
-        :rtype: int
+        :return: The related_search of this SectionUpdate. 
+        :rtype: AttributeOperationSpec
         """
-        return self._type
+        return self._related_search
 
-    @type.setter
-    def type(self, type):
+    @related_search.setter
+    def related_search(self, related_search):
         """
-        Unique integer identifying a state type.
 
-        :param type: The type of this StateSpec.
-        :type: int
+        :param related_search: The related_search of this SectionUpdate.
+        :type: AttributeOperationSpec
         """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
-        self._type = type
+        self._related_search = related_search
 
     @property
-    def version(self):
+    def tator_user_sections(self):
         """
-        Unique integer identifying the version.
+        Attribute that is applied to media to identify membership to a section.
 
-        :return: The version of this StateSpec. 
-        :rtype: int
+        :return: The tator_user_sections of this SectionUpdate. 
+        :rtype: str
         """
-        return self._version
+        return self._tator_user_sections
 
-    @version.setter
-    def version(self, version):
+    @tator_user_sections.setter
+    def tator_user_sections(self, tator_user_sections):
         """
-        Unique integer identifying the version.
+        Attribute that is applied to media to identify membership to a section.
 
-        :param version: The version of this StateSpec.
-        :type: int
+        :param tator_user_sections: The tator_user_sections of this SectionUpdate.
+        :type: str
         """
 
-        self._version = version
+        self._tator_user_sections = tator_user_sections
+
+    @property
+    def visible(self):
+        """
+        Determines the visibility in the UI.
+
+        :return: The visible of this SectionUpdate. 
+        :rtype: bool
+        """
+        return self._visible
+
+    @visible.setter
+    def visible(self, visible):
+        """
+        Determines the visibility in the UI.
+
+        :param visible: The visible of this SectionUpdate.
+        :type: bool
+        """
+
+        self._visible = visible
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -206,18 +225,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StateSpec):
+        if not isinstance(other, SectionUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, StateSpec):
+        if not isinstance(other, SectionUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/state_trim_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state_trim_update.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/state_type.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,71 +28,80 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'association': 'str',
         'attribute_types': 'list[AttributeType]',
+        'default_localization': 'int',
         'delete_child_localizations': 'bool',
         'description': 'str',
         'dtype': 'str',
+        'elemental_id': 'str',
         'grouping_default': 'bool',
         'id': 'int',
         'interpolation': 'str',
         'media': 'list[int]',
         'name': 'str',
         'project': 'int',
         'visible': 'bool'
     }
 
     attribute_map = {
         'association': 'association',
         'attribute_types': 'attribute_types',
+        'default_localization': 'default_localization',
         'delete_child_localizations': 'delete_child_localizations',
         'description': 'description',
         'dtype': 'dtype',
+        'elemental_id': 'elemental_id',
         'grouping_default': 'grouping_default',
         'id': 'id',
         'interpolation': 'interpolation',
         'media': 'media',
         'name': 'name',
         'project': 'project',
         'visible': 'visible'
     }
 
-    def __init__(self, association=None, attribute_types=None, delete_child_localizations=False, description=None, dtype=None, grouping_default=True, id=None, interpolation='latest', media=None, name=None, project=None, visible=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, association=None, attribute_types=None, default_localization=None, delete_child_localizations=False, description=None, dtype=None, elemental_id=None, grouping_default=True, id=None, interpolation='latest', media=None, name=None, project=None, visible=None, local_vars_configuration=None):  # noqa: E501
         """StateType - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._association = None
         self._attribute_types = None
+        self._default_localization = None
         self._delete_child_localizations = None
         self._description = None
         self._dtype = None
+        self._elemental_id = None
         self._grouping_default = None
         self._id = None
         self._interpolation = None
         self._media = None
         self._name = None
         self._project = None
         self._visible = None
         self.discriminator = None
 
         if association is not None:
             self.association = association
         if attribute_types is not None:
             self.attribute_types = attribute_types
+        if default_localization is not None:
+            self.default_localization = default_localization
         if delete_child_localizations is not None:
             self.delete_child_localizations = delete_child_localizations
         if description is not None:
             self.description = description
         if dtype is not None:
             self.dtype = dtype
+        self.elemental_id = elemental_id
         if grouping_default is not None:
             self.grouping_default = grouping_default
         if id is not None:
             self.id = id
         if interpolation is not None:
             self.interpolation = interpolation
         if media is not None:
@@ -149,14 +158,35 @@
         :param attribute_types: The attribute_types of this StateType.
         :type: list[AttributeType]
         """
 
         self._attribute_types = attribute_types
 
     @property
+    def default_localization(self):
+        """
+        If this is a track type, this is a unique integer identifying the default localization type that is created when a track is created via the web interface.
+
+        :return: The default_localization of this StateType. 
+        :rtype: int
+        """
+        return self._default_localization
+
+    @default_localization.setter
+    def default_localization(self, default_localization):
+        """
+        If this is a track type, this is a unique integer identifying the default localization type that is created when a track is created via the web interface.
+
+        :param default_localization: The default_localization of this StateType.
+        :type: int
+        """
+
+        self._default_localization = default_localization
+
+    @property
     def delete_child_localizations(self):
         """
         True if child localizations should be deleted when this state is deleted. Localizations will only be deleted if they are not associated with another state. 
 
         :return: The delete_child_localizations of this StateType. 
         :rtype: bool
         """
@@ -212,14 +242,35 @@
         :param dtype: The dtype of this StateType.
         :type: str
         """
 
         self._dtype = dtype
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this StateType. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this StateType.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def grouping_default(self):
         """
         Whether to group elements in the UI by default.
 
         :return: The grouping_default of this StateType. 
         :rtype: bool
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/state_type_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/state_type_spec.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,59 +28,68 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'association': 'str',
         'attribute_types': 'list[AttributeType]',
+        'default_localization': 'int',
         'delete_child_localizations': 'bool',
         'description': 'str',
+        'elemental_id': 'str',
         'grouping_default': 'bool',
         'interpolation': 'str',
         'media_types': 'list[int]',
         'name': 'str',
         'visible': 'bool'
     }
 
     attribute_map = {
         'association': 'association',
         'attribute_types': 'attribute_types',
+        'default_localization': 'default_localization',
         'delete_child_localizations': 'delete_child_localizations',
         'description': 'description',
+        'elemental_id': 'elemental_id',
         'grouping_default': 'grouping_default',
         'interpolation': 'interpolation',
         'media_types': 'media_types',
         'name': 'name',
         'visible': 'visible'
     }
 
-    def __init__(self, association=None, attribute_types=None, delete_child_localizations=False, description=None, grouping_default=True, interpolation='latest', media_types=None, name=None, visible=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, association=None, attribute_types=None, default_localization=None, delete_child_localizations=False, description=None, elemental_id=None, grouping_default=True, interpolation='latest', media_types=None, name=None, visible=None, local_vars_configuration=None):  # noqa: E501
         """StateTypeSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._association = None
         self._attribute_types = None
+        self._default_localization = None
         self._delete_child_localizations = None
         self._description = None
+        self._elemental_id = None
         self._grouping_default = None
         self._interpolation = None
         self._media_types = None
         self._name = None
         self._visible = None
         self.discriminator = None
 
         self.association = association
         if attribute_types is not None:
             self.attribute_types = attribute_types
+        if default_localization is not None:
+            self.default_localization = default_localization
         if delete_child_localizations is not None:
             self.delete_child_localizations = delete_child_localizations
         if description is not None:
             self.description = description
+        self.elemental_id = elemental_id
         if grouping_default is not None:
             self.grouping_default = grouping_default
         if interpolation is not None:
             self.interpolation = interpolation
         self.media_types = media_types
         self.name = name
         if visible is not None:
@@ -133,14 +142,35 @@
         :param attribute_types: The attribute_types of this StateTypeSpec.
         :type: list[AttributeType]
         """
 
         self._attribute_types = attribute_types
 
     @property
+    def default_localization(self):
+        """
+        If this is a track type, this is a unique integer identifying the default localization type that is created when a track is created via the web interface.
+
+        :return: The default_localization of this StateTypeSpec. 
+        :rtype: int
+        """
+        return self._default_localization
+
+    @default_localization.setter
+    def default_localization(self, default_localization):
+        """
+        If this is a track type, this is a unique integer identifying the default localization type that is created when a track is created via the web interface.
+
+        :param default_localization: The default_localization of this StateTypeSpec.
+        :type: int
+        """
+
+        self._default_localization = default_localization
+
+    @property
     def delete_child_localizations(self):
         """
         True if child localizations should be deleted when this state is deleted. Localizations will only be deleted if they are not associated with another state. 
 
         :return: The delete_child_localizations of this StateTypeSpec. 
         :rtype: bool
         """
@@ -175,14 +205,35 @@
         :param description: The description of this StateTypeSpec.
         :type: str
         """
 
         self._description = description
 
     @property
+    def elemental_id(self):
+        """
+        The elemental ID of the object.
+
+        :return: The elemental_id of this StateTypeSpec. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        The elemental ID of the object.
+
+        :param elemental_id: The elemental_id of this StateTypeSpec.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def grouping_default(self):
         """
         Whether to group elements in the UI by default.
 
         :return: The grouping_default of this StateTypeSpec. 
         :rtype: bool
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/state_type_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/job_cluster_spec.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,169 +14,174 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class StateTypeUpdate(object):
+class JobClusterSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'delete_child_localizations': 'bool',
-        'description': 'str',
-        'grouping_default': 'bool',
+        'cert': 'str',
+        'host': 'str',
         'name': 'str',
-        'visible': 'bool'
+        'port': 'int',
+        'token': 'str'
     }
 
     attribute_map = {
-        'delete_child_localizations': 'delete_child_localizations',
-        'description': 'description',
-        'grouping_default': 'grouping_default',
+        'cert': 'cert',
+        'host': 'host',
         'name': 'name',
-        'visible': 'visible'
+        'port': 'port',
+        'token': 'token'
     }
 
-    def __init__(self, delete_child_localizations=False, description=None, grouping_default=True, name=None, visible=None, local_vars_configuration=None):  # noqa: E501
-        """StateTypeUpdate - a model defined in OpenAPI"""
+    def __init__(self, cert=None, host=None, name=None, port=None, token=None, local_vars_configuration=None):  # noqa: E501
+        """JobClusterSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._delete_child_localizations = None
-        self._description = None
-        self._grouping_default = None
+        self._cert = None
+        self._host = None
         self._name = None
-        self._visible = None
+        self._port = None
+        self._token = None
         self.discriminator = None
 
-        if delete_child_localizations is not None:
-            self.delete_child_localizations = delete_child_localizations
-        if description is not None:
-            self.description = description
-        if grouping_default is not None:
-            self.grouping_default = grouping_default
-        if name is not None:
-            self.name = name
-        if visible is not None:
-            self.visible = visible
+        self.cert = cert
+        self.host = host
+        self.name = name
+        self.port = port
+        self.token = token
 
     @property
-    def delete_child_localizations(self):
+    def cert(self):
         """
-        True if child localizations should be deleted when this state is deleted. Localizations will only be deleted if they are not associated with another state. 
+        Certificate for accessing the job cluster.
 
-        :return: The delete_child_localizations of this StateTypeUpdate. 
-        :rtype: bool
+        :return: The cert of this JobClusterSpec. 
+        :rtype: str
         """
-        return self._delete_child_localizations
+        return self._cert
 
-    @delete_child_localizations.setter
-    def delete_child_localizations(self, delete_child_localizations):
+    @cert.setter
+    def cert(self, cert):
         """
-        True if child localizations should be deleted when this state is deleted. Localizations will only be deleted if they are not associated with another state. 
+        Certificate for accessing the job cluster.
 
-        :param delete_child_localizations: The delete_child_localizations of this StateTypeUpdate.
-        :type: bool
+        :param cert: The cert of this JobClusterSpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and cert is None:  # noqa: E501
+            raise ValueError("Invalid value for `cert`, must not be `None`")  # noqa: E501
 
-        self._delete_child_localizations = delete_child_localizations
+        self._cert = cert
 
     @property
-    def description(self):
+    def host(self):
         """
-        Description of the state type.
+        Hostname where the cluster can be accessed.
 
-        :return: The description of this StateTypeUpdate. 
+        :return: The host of this JobClusterSpec. 
         :rtype: str
         """
-        return self._description
+        return self._host
 
-    @description.setter
-    def description(self, description):
+    @host.setter
+    def host(self, host):
         """
-        Description of the state type.
+        Hostname where the cluster can be accessed.
 
-        :param description: The description of this StateTypeUpdate.
+        :param host: The host of this JobClusterSpec.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and host is None:  # noqa: E501
+            raise ValueError("Invalid value for `host`, must not be `None`")  # noqa: E501
 
-        self._description = description
+        self._host = host
 
     @property
-    def grouping_default(self):
+    def name(self):
         """
-        Whether to group elements in the UI by default.
+        Unique name of the job cluster.
 
-        :return: The grouping_default of this StateTypeUpdate. 
-        :rtype: bool
+        :return: The name of this JobClusterSpec. 
+        :rtype: str
         """
-        return self._grouping_default
+        return self._name
 
-    @grouping_default.setter
-    def grouping_default(self, grouping_default):
+    @name.setter
+    def name(self, name):
         """
-        Whether to group elements in the UI by default.
+        Unique name of the job cluster.
 
-        :param grouping_default: The grouping_default of this StateTypeUpdate.
-        :type: bool
+        :param name: The name of this JobClusterSpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._grouping_default = grouping_default
+        self._name = name
 
     @property
-    def name(self):
+    def port(self):
         """
-        Name of the state type.
+        Port where the cluster can be accessed.
 
-        :return: The name of this StateTypeUpdate. 
-        :rtype: str
+        :return: The port of this JobClusterSpec. 
+        :rtype: int
         """
-        return self._name
+        return self._port
 
-    @name.setter
-    def name(self, name):
+    @port.setter
+    def port(self, port):
         """
-        Name of the state type.
+        Port where the cluster can be accessed.
 
-        :param name: The name of this StateTypeUpdate.
-        :type: str
+        :param port: The port of this JobClusterSpec.
+        :type: int
         """
+        if self.local_vars_configuration.client_side_validation and port is None:  # noqa: E501
+            raise ValueError("Invalid value for `port`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._port = port
 
     @property
-    def visible(self):
+    def token(self):
         """
-        Whether this state type should be displayed.
+        Token for accessing the job cluster.
 
-        :return: The visible of this StateTypeUpdate. 
-        :rtype: bool
+        :return: The token of this JobClusterSpec. 
+        :rtype: str
         """
-        return self._visible
+        return self._token
 
-    @visible.setter
-    def visible(self, visible):
+    @token.setter
+    def token(self, token):
         """
-        Whether this state type should be displayed.
+        Token for accessing the job cluster.
 
-        :param visible: The visible of this StateTypeUpdate.
-        :type: bool
+        :param token: The token of this JobClusterSpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and token is None:  # noqa: E501
+            raise ValueError("Invalid value for `token`, must not be `None`")  # noqa: E501
 
-        self._visible = visible
+        self._token = token
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -204,18 +209,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StateTypeUpdate):
+        if not isinstance(other, JobClusterSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, StateTypeUpdate):
+        if not isinstance(other, JobClusterSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/state_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/media_id_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,143 +14,167 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class StateUpdate(object):
+class MediaIdQuery(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'attributes': 'dict(str, object)',
-        'frame': 'int',
-        'localization_ids_add': 'list[int]',
-        'localization_ids_remove': 'list[int]'
+        'float_array': 'list[FloatArrayQuery]',
+        'ids': 'list[int]',
+        'localization_ids': 'list[int]',
+        'object_search': 'AttributeOperationSpec',
+        'state_ids': 'list[int]'
     }
 
     attribute_map = {
-        'attributes': 'attributes',
-        'frame': 'frame',
-        'localization_ids_add': 'localization_ids_add',
-        'localization_ids_remove': 'localization_ids_remove'
+        'float_array': 'float_array',
+        'ids': 'ids',
+        'localization_ids': 'localization_ids',
+        'object_search': 'object_search',
+        'state_ids': 'state_ids'
     }
 
-    def __init__(self, attributes=None, frame=None, localization_ids_add=None, localization_ids_remove=None, local_vars_configuration=None):  # noqa: E501
-        """StateUpdate - a model defined in OpenAPI"""
+    def __init__(self, float_array=None, ids=None, localization_ids=None, object_search=None, state_ids=None, local_vars_configuration=None):  # noqa: E501
+        """MediaIdQuery - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._attributes = None
-        self._frame = None
-        self._localization_ids_add = None
-        self._localization_ids_remove = None
+        self._float_array = None
+        self._ids = None
+        self._localization_ids = None
+        self._object_search = None
+        self._state_ids = None
         self.discriminator = None
 
-        if attributes is not None:
-            self.attributes = attributes
-        if frame is not None:
-            self.frame = frame
-        if localization_ids_add is not None:
-            self.localization_ids_add = localization_ids_add
-        if localization_ids_remove is not None:
-            self.localization_ids_remove = localization_ids_remove
+        if float_array is not None:
+            self.float_array = float_array
+        if ids is not None:
+            self.ids = ids
+        if localization_ids is not None:
+            self.localization_ids = localization_ids
+        if object_search is not None:
+            self.object_search = object_search
+        if state_ids is not None:
+            self.state_ids = state_ids
 
     @property
-    def attributes(self):
+    def float_array(self):
         """
-        Object containing attribute values.
+        Searches on `float_array` attributes.
 
-        :return: The attributes of this StateUpdate. 
-        :rtype: dict(str, object)
+        :return: The float_array of this MediaIdQuery. 
+        :rtype: list[FloatArrayQuery]
         """
-        return self._attributes
+        return self._float_array
 
-    @attributes.setter
-    def attributes(self, attributes):
+    @float_array.setter
+    def float_array(self, float_array):
         """
-        Object containing attribute values.
+        Searches on `float_array` attributes.
 
-        :param attributes: The attributes of this StateUpdate.
-        :type: dict(str, object)
+        :param float_array: The float_array of this MediaIdQuery.
+        :type: list[FloatArrayQuery]
         """
 
-        self._attributes = attributes
+        self._float_array = float_array
 
     @property
-    def frame(self):
+    def ids(self):
         """
-        Frame number this state applies to.
+        Array of media IDs to retrieve.
 
-        :return: The frame of this StateUpdate. 
-        :rtype: int
+        :return: The ids of this MediaIdQuery. 
+        :rtype: list[int]
         """
-        return self._frame
+        return self._ids
 
-    @frame.setter
-    def frame(self, frame):
+    @ids.setter
+    def ids(self, ids):
         """
-        Frame number this state applies to.
+        Array of media IDs to retrieve.
 
-        :param frame: The frame of this StateUpdate.
-        :type: int
+        :param ids: The ids of this MediaIdQuery.
+        :type: list[int]
         """
 
-        self._frame = frame
+        self._ids = ids
 
     @property
-    def localization_ids_add(self):
+    def localization_ids(self):
         """
-        List of new localization IDs that this state applies to.
+        Array of child localization IDs for which media should be retrieved.
 
-        :return: The localization_ids_add of this StateUpdate. 
+        :return: The localization_ids of this MediaIdQuery. 
         :rtype: list[int]
         """
-        return self._localization_ids_add
+        return self._localization_ids
 
-    @localization_ids_add.setter
-    def localization_ids_add(self, localization_ids_add):
+    @localization_ids.setter
+    def localization_ids(self, localization_ids):
         """
-        List of new localization IDs that this state applies to.
+        Array of child localization IDs for which media should be retrieved.
 
-        :param localization_ids_add: The localization_ids_add of this StateUpdate.
+        :param localization_ids: The localization_ids of this MediaIdQuery.
         :type: list[int]
         """
 
-        self._localization_ids_add = localization_ids_add
+        self._localization_ids = localization_ids
+
+    @property
+    def object_search(self):
+        """
+
+        :return: The object_search of this MediaIdQuery. 
+        :rtype: AttributeOperationSpec
+        """
+        return self._object_search
+
+    @object_search.setter
+    def object_search(self, object_search):
+        """
+
+        :param object_search: The object_search of this MediaIdQuery.
+        :type: AttributeOperationSpec
+        """
+
+        self._object_search = object_search
 
     @property
-    def localization_ids_remove(self):
+    def state_ids(self):
         """
-        List of new localization IDs that this state applies to.
+        Array of child state IDs for which media should be retrieved.
 
-        :return: The localization_ids_remove of this StateUpdate. 
+        :return: The state_ids of this MediaIdQuery. 
         :rtype: list[int]
         """
-        return self._localization_ids_remove
+        return self._state_ids
 
-    @localization_ids_remove.setter
-    def localization_ids_remove(self, localization_ids_remove):
+    @state_ids.setter
+    def state_ids(self, state_ids):
         """
-        List of new localization IDs that this state applies to.
+        Array of child state IDs for which media should be retrieved.
 
-        :param localization_ids_remove: The localization_ids_remove of this StateUpdate.
+        :param state_ids: The state_ids of this MediaIdQuery.
         :type: list[int]
         """
 
-        self._localization_ids_remove = localization_ids_remove
+        self._state_ids = state_ids
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -178,18 +202,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StateUpdate):
+        if not isinstance(other, MediaIdQuery):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, StateUpdate):
+        if not isinstance(other, MediaIdQuery):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/temporary_file.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/affiliation.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,247 +14,259 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class TemporaryFile(object):
+class Affiliation(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'created_datetime': 'str',
-        'eol_datetime': 'str',
+        'email': 'str',
+        'first_name': 'str',
         'id': 'int',
-        'lookup': 'str',
-        'name': 'str',
-        'path': 'str',
-        'project': 'int',
-        'user': 'int'
+        'last_name': 'str',
+        'organization': 'int',
+        'permission': 'str',
+        'user': 'int',
+        'username': 'str'
     }
 
     attribute_map = {
-        'created_datetime': 'created_datetime',
-        'eol_datetime': 'eol_datetime',
+        'email': 'email',
+        'first_name': 'first_name',
         'id': 'id',
-        'lookup': 'lookup',
-        'name': 'name',
-        'path': 'path',
-        'project': 'project',
-        'user': 'user'
+        'last_name': 'last_name',
+        'organization': 'organization',
+        'permission': 'permission',
+        'user': 'user',
+        'username': 'username'
     }
 
-    def __init__(self, created_datetime=None, eol_datetime=None, id=None, lookup=None, name=None, path=None, project=None, user=None, local_vars_configuration=None):  # noqa: E501
-        """TemporaryFile - a model defined in OpenAPI"""
+    def __init__(self, email=None, first_name=None, id=None, last_name=None, organization=None, permission=None, user=None, username=None, local_vars_configuration=None):  # noqa: E501
+        """Affiliation - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._created_datetime = None
-        self._eol_datetime = None
+        self._email = None
+        self._first_name = None
         self._id = None
-        self._lookup = None
-        self._name = None
-        self._path = None
-        self._project = None
+        self._last_name = None
+        self._organization = None
+        self._permission = None
         self._user = None
+        self._username = None
         self.discriminator = None
 
-        if created_datetime is not None:
-            self.created_datetime = created_datetime
-        if eol_datetime is not None:
-            self.eol_datetime = eol_datetime
+        if email is not None:
+            self.email = email
+        if first_name is not None:
+            self.first_name = first_name
         if id is not None:
             self.id = id
-        if lookup is not None:
-            self.lookup = lookup
-        if name is not None:
-            self.name = name
-        if path is not None:
-            self.path = path
-        if project is not None:
-            self.project = project
+        if last_name is not None:
+            self.last_name = last_name
+        if organization is not None:
+            self.organization = organization
+        if permission is not None:
+            self.permission = permission
         if user is not None:
             self.user = user
+        if username is not None:
+            self.username = username
 
     @property
-    def created_datetime(self):
+    def email(self):
         """
-        Datetime when this temporary file was created.
+        Email address of user.
 
-        :return: The created_datetime of this TemporaryFile. 
+        :return: The email of this Affiliation. 
         :rtype: str
         """
-        return self._created_datetime
+        return self._email
 
-    @created_datetime.setter
-    def created_datetime(self, created_datetime):
+    @email.setter
+    def email(self, email):
         """
-        Datetime when this temporary file was created.
+        Email address of user.
 
-        :param created_datetime: The created_datetime of this TemporaryFile.
+        :param email: The email of this Affiliation.
         :type: str
         """
 
-        self._created_datetime = created_datetime
+        self._email = email
 
     @property
-    def eol_datetime(self):
+    def first_name(self):
         """
-        Datetime when this temporary file may be deleted.
+        First name of user.
 
-        :return: The eol_datetime of this TemporaryFile. 
+        :return: The first_name of this Affiliation. 
         :rtype: str
         """
-        return self._eol_datetime
+        return self._first_name
 
-    @eol_datetime.setter
-    def eol_datetime(self, eol_datetime):
+    @first_name.setter
+    def first_name(self, first_name):
         """
-        Datetime when this temporary file may be deleted.
+        First name of user.
 
-        :param eol_datetime: The eol_datetime of this TemporaryFile.
+        :param first_name: The first_name of this Affiliation.
         :type: str
         """
 
-        self._eol_datetime = eol_datetime
+        self._first_name = first_name
 
     @property
     def id(self):
         """
-        Unique integer identifying a temporary file.
+        Unique integer identifying a affiliation.
 
-        :return: The id of this TemporaryFile. 
+        :return: The id of this Affiliation. 
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """
-        Unique integer identifying a temporary file.
+        Unique integer identifying a affiliation.
 
-        :param id: The id of this TemporaryFile.
+        :param id: The id of this Affiliation.
         :type: int
         """
 
         self._id = id
 
     @property
-    def lookup(self):
+    def last_name(self):
         """
-        md5hash of lookup parameters
+        Last name of user.
 
-        :return: The lookup of this TemporaryFile. 
+        :return: The last_name of this Affiliation. 
         :rtype: str
         """
-        return self._lookup
+        return self._last_name
 
-    @lookup.setter
-    def lookup(self, lookup):
+    @last_name.setter
+    def last_name(self, last_name):
         """
-        md5hash of lookup parameters
+        Last name of user.
 
-        :param lookup: The lookup of this TemporaryFile.
+        :param last_name: The last_name of this Affiliation.
         :type: str
         """
 
-        self._lookup = lookup
+        self._last_name = last_name
 
     @property
-    def name(self):
+    def organization(self):
         """
-        Unique name for the temporary file
+        Unique integer identifying an organization.
 
-        :return: The name of this TemporaryFile. 
-        :rtype: str
+        :return: The organization of this Affiliation. 
+        :rtype: int
         """
-        return self._name
+        return self._organization
 
-    @name.setter
-    def name(self, name):
+    @organization.setter
+    def organization(self, organization):
         """
-        Unique name for the temporary file
+        Unique integer identifying an organization.
 
-        :param name: The name of this TemporaryFile.
-        :type: str
+        :param organization: The organization of this Affiliation.
+        :type: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                organization is not None and organization < 1):  # noqa: E501
+            raise ValueError("Invalid value for `organization`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._name = name
+        self._organization = organization
 
     @property
-    def path(self):
+    def permission(self):
         """
-        Full URL to the temporary file.
+        User permission level for the organization.
 
-        :return: The path of this TemporaryFile. 
+        :return: The permission of this Affiliation. 
         :rtype: str
         """
-        return self._path
+        return self._permission
 
-    @path.setter
-    def path(self, path):
+    @permission.setter
+    def permission(self, permission):
         """
-        Full URL to the temporary file.
+        User permission level for the organization.
 
-        :param path: The path of this TemporaryFile.
+        :param permission: The permission of this Affiliation.
         :type: str
         """
+        allowed_values = ["Member", "Admin"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and permission not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `permission` ({0}), must be one of {1}"  # noqa: E501
+                .format(permission, allowed_values)
+            )
 
-        self._path = path
+        self._permission = permission
 
     @property
-    def project(self):
+    def user(self):
         """
-        Unique integer identifying a project.
+        Unique integer identifying a user.
 
-        :return: The project of this TemporaryFile. 
+        :return: The user of this Affiliation. 
         :rtype: int
         """
-        return self._project
+        return self._user
 
-    @project.setter
-    def project(self, project):
+    @user.setter
+    def user(self, user):
         """
-        Unique integer identifying a project.
+        Unique integer identifying a user.
 
-        :param project: The project of this TemporaryFile.
+        :param user: The user of this Affiliation.
         :type: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                user is not None and user < 1):  # noqa: E501
+            raise ValueError("Invalid value for `user`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._project = project
+        self._user = user
 
     @property
-    def user(self):
+    def username(self):
         """
-        Unique integer identifying user who created this file.
+        Username for the membership.
 
-        :return: The user of this TemporaryFile. 
-        :rtype: int
+        :return: The username of this Affiliation. 
+        :rtype: str
         """
-        return self._user
+        return self._username
 
-    @user.setter
-    def user(self, user):
+    @username.setter
+    def username(self, username):
         """
-        Unique integer identifying user who created this file.
+        Username for the membership.
 
-        :param user: The user of this TemporaryFile.
-        :type: int
+        :param username: The username of this Affiliation.
+        :type: str
         """
 
-        self._user = user
+        self._username = username
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -282,18 +294,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TemporaryFile):
+        if not isinstance(other, Affiliation):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TemporaryFile):
+        if not isinstance(other, Affiliation):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/token.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/localization_delete.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,65 +14,71 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Token(object):
+class LocalizationDelete(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'token': 'str'
+        'prune': 'int'
     }
 
     attribute_map = {
-        'token': 'token'
+        'prune': 'prune'
     }
 
-    def __init__(self, token=None, local_vars_configuration=None):  # noqa: E501
-        """Token - a model defined in OpenAPI"""
+    def __init__(self, prune=0, local_vars_configuration=None):  # noqa: E501
+        """LocalizationDelete - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._token = None
+        self._prune = None
         self.discriminator = None
 
-        if token is not None:
-            self.token = token
+        if prune is not None:
+            self.prune = prune
 
     @property
-    def token(self):
+    def prune(self):
         """
-        API token.
+        If set to 1 will purge the object from the database entirely. This removes any record, change-log, that this metadatum ever existed.
 
-        :return: The token of this Token. 
-        :rtype: str
+        :return: The prune of this LocalizationDelete. 
+        :rtype: int
         """
-        return self._token
+        return self._prune
 
-    @token.setter
-    def token(self, token):
+    @prune.setter
+    def prune(self, prune):
         """
-        API token.
+        If set to 1 will purge the object from the database entirely. This removes any record, change-log, that this metadatum ever existed.
 
-        :param token: The token of this Token.
-        :type: str
+        :param prune: The prune of this LocalizationDelete.
+        :type: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                prune is not None and prune > 1):  # noqa: E501
+            raise ValueError("Invalid value for `prune`, must be a value less than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                prune is not None and prune < 0):  # noqa: E501
+            raise ValueError("Invalid value for `prune`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._token = token
+        self._prune = prune
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -100,18 +106,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Token):
+        if not isinstance(other, LocalizationDelete):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Token):
+        if not isinstance(other, LocalizationDelete):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/transcode.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/create_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,117 +14,117 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Transcode(object):
+class CreateResponse(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'gid': 'str',
+        'id': 'object',
         'message': 'str',
-        'uid': 'str'
+        'object': 'dict(str, object)'
     }
 
     attribute_map = {
-        'gid': 'gid',
+        'id': 'id',
         'message': 'message',
-        'uid': 'uid'
+        'object': 'object'
     }
 
-    def __init__(self, gid=None, message=None, uid=None, local_vars_configuration=None):  # noqa: E501
-        """Transcode - a model defined in OpenAPI"""
+    def __init__(self, id=None, message=None, object=None, local_vars_configuration=None):  # noqa: E501
+        """CreateResponse - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._gid = None
+        self._id = None
         self._message = None
-        self._uid = None
+        self._object = None
         self.discriminator = None
 
-        if gid is not None:
-            self.gid = gid
+        if id is not None:
+            self.id = id
         if message is not None:
             self.message = message
-        if uid is not None:
-            self.uid = uid
+        if object is not None:
+            self.object = object
 
     @property
-    def gid(self):
+    def id(self):
         """
-        UUID identifying the job group.
+        Unique integer identifying the created object.
 
-        :return: The gid of this Transcode. 
-        :rtype: str
+        :return: The id of this CreateResponse. 
+        :rtype: object
         """
-        return self._gid
+        return self._id
 
-    @gid.setter
-    def gid(self, gid):
+    @id.setter
+    def id(self, id):
         """
-        UUID identifying the job group.
+        Unique integer identifying the created object.
 
-        :param gid: The gid of this Transcode.
-        :type: str
+        :param id: The id of this CreateResponse.
+        :type: object
         """
 
-        self._gid = gid
+        self._id = id
 
     @property
     def message(self):
         """
-        Message indicating transcode started successfully.
+        Message indicating successful creation.
 
-        :return: The message of this Transcode. 
+        :return: The message of this CreateResponse. 
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
         """
-        Message indicating transcode started successfully.
+        Message indicating successful creation.
 
-        :param message: The message of this Transcode.
+        :param message: The message of this CreateResponse.
         :type: str
         """
 
         self._message = message
 
     @property
-    def uid(self):
+    def object(self):
         """
-        UUID identifying the job.
+        The created objects.
 
-        :return: The uid of this Transcode. 
-        :rtype: str
+        :return: The object of this CreateResponse. 
+        :rtype: dict(str, object)
         """
-        return self._uid
+        return self._object
 
-    @uid.setter
-    def uid(self, uid):
+    @object.setter
+    def object(self, object):
         """
-        UUID identifying the job.
+        The created objects.
 
-        :param uid: The uid of this Transcode.
-        :type: str
+        :param object: The object of this CreateResponse.
+        :type: dict(str, object)
         """
 
-        self._uid = uid
+        self._object = object
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -152,18 +152,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Transcode):
+        if not isinstance(other, CreateResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Transcode):
+        if not isinstance(other, CreateResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/transcode_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/transcode_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/upload_completion_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/upload_completion_spec.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/upload_info.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/feed_definition.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,117 +14,93 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class UploadInfo(object):
+class FeedDefinition(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'key': 'str',
-        'upload_id': 'str',
-        'urls': 'list[str]'
+        'name': 'str',
+        'resolution': 'list[int]'
     }
 
     attribute_map = {
-        'key': 'key',
-        'upload_id': 'upload_id',
-        'urls': 'urls'
+        'name': 'name',
+        'resolution': 'resolution'
     }
 
-    def __init__(self, key=None, upload_id=None, urls=None, local_vars_configuration=None):  # noqa: E501
-        """UploadInfo - a model defined in OpenAPI"""
+    def __init__(self, name=None, resolution=None, local_vars_configuration=None):  # noqa: E501
+        """FeedDefinition - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._key = None
-        self._upload_id = None
-        self._urls = None
+        self._name = None
+        self._resolution = None
         self.discriminator = None
 
-        if key is not None:
-            self.key = key
-        if upload_id is not None:
-            self.upload_id = upload_id
-        if urls is not None:
-            self.urls = urls
+        self.name = name
+        self.resolution = resolution
 
     @property
-    def key(self):
+    def name(self):
         """
-        An object key that can be supplied to the `Transcode` or `Media` endpoint after the file has been uploaded.
+        Name of the feed.
 
-        :return: The key of this UploadInfo. 
+        :return: The name of this FeedDefinition. 
         :rtype: str
         """
-        return self._key
+        return self._name
 
-    @key.setter
-    def key(self, key):
+    @name.setter
+    def name(self, name):
         """
-        An object key that can be supplied to the `Transcode` or `Media` endpoint after the file has been uploaded.
+        Name of the feed.
 
-        :param key: The key of this UploadInfo.
+        :param name: The name of this FeedDefinition.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._key = key
+        self._name = name
 
     @property
-    def upload_id(self):
+    def resolution(self):
         """
-        An upload ID that can be supplied to the `UploadCompletion` endpoint after the file has been uploaded. Only contains a value if `num_parts` > 1.
+        Resolution of the video in pixels (height, width).
 
-        :return: The upload_id of this UploadInfo. 
-        :rtype: str
-        """
-        return self._upload_id
-
-    @upload_id.setter
-    def upload_id(self, upload_id):
-        """
-        An upload ID that can be supplied to the `UploadCompletion` endpoint after the file has been uploaded. Only contains a value if `num_parts` > 1.
-
-        :param upload_id: The upload_id of this UploadInfo.
-        :type: str
-        """
-
-        self._upload_id = upload_id
-
-    @property
-    def urls(self):
-        """
-        One or more URLs for upload via one PUT request per URL.
-
-        :return: The urls of this UploadInfo. 
-        :rtype: list[str]
+        :return: The resolution of this FeedDefinition. 
+        :rtype: list[int]
         """
-        return self._urls
+        return self._resolution
 
-    @urls.setter
-    def urls(self, urls):
+    @resolution.setter
+    def resolution(self, resolution):
         """
-        One or more URLs for upload via one PUT request per URL.
+        Resolution of the video in pixels (height, width).
 
-        :param urls: The urls of this UploadInfo.
-        :type: list[str]
+        :param resolution: The resolution of this FeedDefinition.
+        :type: list[int]
         """
+        if self.local_vars_configuration.client_side_validation and resolution is None:  # noqa: E501
+            raise ValueError("Invalid value for `resolution`, must not be `None`")  # noqa: E501
 
-        self._urls = urls
+        self._resolution = resolution
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -152,18 +128,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UploadInfo):
+        if not isinstance(other, FeedDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UploadInfo):
+        if not isinstance(other, FeedDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/upload_part.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/upload_part.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/user.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/generic_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,169 +14,143 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class User(object):
+class GenericFile(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'email': 'str',
-        'first_name': 'str',
-        'id': 'int',
-        'last_name': 'str',
-        'username': 'str'
+        'name': 'str',
+        'project': 'int',
+        'upload_url': 'str',
+        'url': 'str'
     }
 
     attribute_map = {
-        'email': 'email',
-        'first_name': 'first_name',
-        'id': 'id',
-        'last_name': 'last_name',
-        'username': 'username'
+        'name': 'name',
+        'project': 'project',
+        'upload_url': 'upload_url',
+        'url': 'url'
     }
 
-    def __init__(self, email=None, first_name=None, id=None, last_name=None, username=None, local_vars_configuration=None):  # noqa: E501
-        """User - a model defined in OpenAPI"""
+    def __init__(self, name=None, project=None, upload_url=None, url=None, local_vars_configuration=None):  # noqa: E501
+        """GenericFile - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._email = None
-        self._first_name = None
-        self._id = None
-        self._last_name = None
-        self._username = None
+        self._name = None
+        self._project = None
+        self._upload_url = None
+        self._url = None
         self.discriminator = None
 
-        if email is not None:
-            self.email = email
-        if first_name is not None:
-            self.first_name = first_name
-        if id is not None:
-            self.id = id
-        if last_name is not None:
-            self.last_name = last_name
-        if username is not None:
-            self.username = username
+        if name is not None:
+            self.name = name
+        if project is not None:
+            self.project = project
+        if upload_url is not None:
+            self.upload_url = upload_url
+        if url is not None:
+            self.url = url
 
     @property
-    def email(self):
+    def name(self):
         """
-        Email address of user.
+        Name of generic, non-media file
 
-        :return: The email of this User. 
+        :return: The name of this GenericFile. 
         :rtype: str
         """
-        return self._email
+        return self._name
 
-    @email.setter
-    def email(self, email):
+    @name.setter
+    def name(self, name):
         """
-        Email address of user.
+        Name of generic, non-media file
 
-        :param email: The email of this User.
+        :param name: The name of this GenericFile.
         :type: str
         """
 
-        self._email = email
+        self._name = name
 
     @property
-    def first_name(self):
+    def project(self):
         """
-        First name of user.
+        Unique integer identifying project to store the file in
 
-        :return: The first_name of this User. 
-        :rtype: str
-        """
-        return self._first_name
-
-    @first_name.setter
-    def first_name(self, first_name):
-        """
-        First name of user.
-
-        :param first_name: The first_name of this User.
-        :type: str
-        """
-
-        self._first_name = first_name
-
-    @property
-    def id(self):
-        """
-        Unique integer identifying a user.
-
-        :return: The id of this User. 
+        :return: The project of this GenericFile. 
         :rtype: int
         """
-        return self._id
+        return self._project
 
-    @id.setter
-    def id(self, id):
+    @project.setter
+    def project(self, project):
         """
-        Unique integer identifying a user.
+        Unique integer identifying project to store the file in
 
-        :param id: The id of this User.
+        :param project: The project of this GenericFile.
         :type: int
         """
 
-        self._id = id
+        self._project = project
 
     @property
-    def last_name(self):
+    def upload_url(self):
         """
-        Last name of user.
+        URL of the uploaded file
 
-        :return: The last_name of this User. 
+        :return: The upload_url of this GenericFile. 
         :rtype: str
         """
-        return self._last_name
+        return self._upload_url
 
-    @last_name.setter
-    def last_name(self, last_name):
+    @upload_url.setter
+    def upload_url(self, upload_url):
         """
-        Last name of user.
+        URL of the uploaded file
 
-        :param last_name: The last_name of this User.
+        :param upload_url: The upload_url of this GenericFile.
         :type: str
         """
 
-        self._last_name = last_name
+        self._upload_url = upload_url
 
     @property
-    def username(self):
+    def url(self):
         """
-        Username of user.
+        Name of generic, non-media file
 
-        :return: The username of this User. 
+        :return: The url of this GenericFile. 
         :rtype: str
         """
-        return self._username
+        return self._url
 
-    @username.setter
-    def username(self, username):
+    @url.setter
+    def url(self, url):
         """
-        Username of user.
+        Name of generic, non-media file
 
-        :param username: The username of this User.
+        :param url: The url of this GenericFile.
         :type: str
         """
 
-        self._username = username
+        self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -204,18 +178,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, User):
+        if not isinstance(other, GenericFile):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, User):
+        if not isinstance(other, GenericFile):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/user_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/attribute_type_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,143 +14,118 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class UserUpdate(object):
+class AttributeTypeUpdate(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'email': 'str',
-        'first_name': 'str',
-        'last_name': 'str',
-        'username': 'str'
+        'attribute_type_update': 'AttributeTypeUpdateAttributeTypeUpdate',
+        'current_name': 'str',
+        'entity_type': 'str'
     }
 
     attribute_map = {
-        'email': 'email',
-        'first_name': 'first_name',
-        'last_name': 'last_name',
-        'username': 'username'
+        'attribute_type_update': 'attribute_type_update',
+        'current_name': 'current_name',
+        'entity_type': 'entity_type'
     }
 
-    def __init__(self, email=None, first_name=None, last_name=None, username=None, local_vars_configuration=None):  # noqa: E501
-        """UserUpdate - a model defined in OpenAPI"""
+    def __init__(self, attribute_type_update=None, current_name=None, entity_type=None, local_vars_configuration=None):  # noqa: E501
+        """AttributeTypeUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._email = None
-        self._first_name = None
-        self._last_name = None
-        self._username = None
+        self._attribute_type_update = None
+        self._current_name = None
+        self._entity_type = None
         self.discriminator = None
 
-        if email is not None:
-            self.email = email
-        if first_name is not None:
-            self.first_name = first_name
-        if last_name is not None:
-            self.last_name = last_name
-        if username is not None:
-            self.username = username
+        self.attribute_type_update = attribute_type_update
+        self.current_name = current_name
+        self.entity_type = entity_type
 
     @property
-    def email(self):
+    def attribute_type_update(self):
         """
-        Email address of user.
 
-        :return: The email of this UserUpdate. 
-        :rtype: str
-        """
-        return self._email
-
-    @email.setter
-    def email(self, email):
-        """
-        Email address of user.
-
-        :param email: The email of this UserUpdate.
-        :type: str
-        """
-
-        self._email = email
-
-    @property
-    def first_name(self):
+        :return: The attribute_type_update of this AttributeTypeUpdate. 
+        :rtype: AttributeTypeUpdateAttributeTypeUpdate
         """
-        First name of user.
+        return self._attribute_type_update
 
-        :return: The first_name of this UserUpdate. 
-        :rtype: str
+    @attribute_type_update.setter
+    def attribute_type_update(self, attribute_type_update):
         """
-        return self._first_name
 
-    @first_name.setter
-    def first_name(self, first_name):
-        """
-        First name of user.
-
-        :param first_name: The first_name of this UserUpdate.
-        :type: str
+        :param attribute_type_update: The attribute_type_update of this AttributeTypeUpdate.
+        :type: AttributeTypeUpdateAttributeTypeUpdate
         """
+        if self.local_vars_configuration.client_side_validation and attribute_type_update is None:  # noqa: E501
+            raise ValueError("Invalid value for `attribute_type_update`, must not be `None`")  # noqa: E501
 
-        self._first_name = first_name
+        self._attribute_type_update = attribute_type_update
 
     @property
-    def last_name(self):
+    def current_name(self):
         """
-        Last name of user.
+        The attribute to rename.
 
-        :return: The last_name of this UserUpdate. 
+        :return: The current_name of this AttributeTypeUpdate. 
         :rtype: str
         """
-        return self._last_name
+        return self._current_name
 
-    @last_name.setter
-    def last_name(self, last_name):
+    @current_name.setter
+    def current_name(self, current_name):
         """
-        Last name of user.
+        The attribute to rename.
 
-        :param last_name: The last_name of this UserUpdate.
+        :param current_name: The current_name of this AttributeTypeUpdate.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and current_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `current_name`, must not be `None`")  # noqa: E501
 
-        self._last_name = last_name
+        self._current_name = current_name
 
     @property
-    def username(self):
+    def entity_type(self):
         """
-        Username of user.
+        The entity type containing the attribute to rename.
 
-        :return: The username of this UserUpdate. 
+        :return: The entity_type of this AttributeTypeUpdate. 
         :rtype: str
         """
-        return self._username
+        return self._entity_type
 
-    @username.setter
-    def username(self, username):
+    @entity_type.setter
+    def entity_type(self, entity_type):
         """
-        Username of user.
+        The entity type containing the attribute to rename.
 
-        :param username: The username of this UserUpdate.
+        :param entity_type: The entity_type of this AttributeTypeUpdate.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and entity_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `entity_type`, must not be `None`")  # noqa: E501
 
-        self._username = username
+        self._entity_type = entity_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -178,18 +153,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserUpdate):
+        if not isinstance(other, AttributeTypeUpdate):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UserUpdate):
+        if not isinstance(other, AttributeTypeUpdate):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/version.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/file_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,248 +14,195 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Version(object):
+class FileType(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'bases': 'list[int]',
-        'created_by': 'str',
+        'attribute_types': 'list[AttributeType]',
         'description': 'str',
+        'elemental_id': 'str',
         'id': 'int',
         'name': 'str',
-        'number': 'int',
-        'project': 'int',
-        'show_empty': 'bool'
+        'project': 'int'
     }
 
     attribute_map = {
-        'bases': 'bases',
-        'created_by': 'created_by',
+        'attribute_types': 'attribute_types',
         'description': 'description',
+        'elemental_id': 'elemental_id',
         'id': 'id',
         'name': 'name',
-        'number': 'number',
-        'project': 'project',
-        'show_empty': 'show_empty'
+        'project': 'project'
     }
 
-    def __init__(self, bases=None, created_by=None, description='', id=None, name=None, number=None, project=None, show_empty=True, local_vars_configuration=None):  # noqa: E501
-        """Version - a model defined in OpenAPI"""
+    def __init__(self, attribute_types=None, description='', elemental_id=None, id=None, name=None, project=None, local_vars_configuration=None):  # noqa: E501
+        """FileType - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._bases = None
-        self._created_by = None
+        self._attribute_types = None
         self._description = None
+        self._elemental_id = None
         self._id = None
         self._name = None
-        self._number = None
         self._project = None
-        self._show_empty = None
         self.discriminator = None
 
-        if bases is not None:
-            self.bases = bases
-        if created_by is not None:
-            self.created_by = created_by
+        if attribute_types is not None:
+            self.attribute_types = attribute_types
         if description is not None:
             self.description = description
+        self.elemental_id = elemental_id
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
-        if number is not None:
-            self.number = number
         if project is not None:
             self.project = project
-        if show_empty is not None:
-            self.show_empty = show_empty
 
     @property
-    def bases(self):
+    def attribute_types(self):
         """
-        Array of other version IDs that are dependencies of this version.
+        Attribute type definitions.
 
-        :return: The bases of this Version. 
-        :rtype: list[int]
+        :return: The attribute_types of this FileType. 
+        :rtype: list[AttributeType]
         """
-        return self._bases
+        return self._attribute_types
 
-    @bases.setter
-    def bases(self, bases):
+    @attribute_types.setter
+    def attribute_types(self, attribute_types):
         """
-        Array of other version IDs that are dependencies of this version.
+        Attribute type definitions.
 
-        :param bases: The bases of this Version.
-        :type: list[int]
+        :param attribute_types: The attribute_types of this FileType.
+        :type: list[AttributeType]
         """
 
-        self._bases = bases
+        self._attribute_types = attribute_types
 
     @property
-    def created_by(self):
+    def description(self):
         """
-        Name of user who created the last unmodified annotation in this version.
+        Description of the file type.
 
-        :return: The created_by of this Version. 
+        :return: The description of this FileType. 
         :rtype: str
         """
-        return self._created_by
+        return self._description
 
-    @created_by.setter
-    def created_by(self, created_by):
+    @description.setter
+    def description(self, description):
         """
-        Name of user who created the last unmodified annotation in this version.
+        Description of the file type.
 
-        :param created_by: The created_by of this Version.
+        :param description: The description of this FileType.
         :type: str
         """
 
-        self._created_by = created_by
+        self._description = description
 
     @property
-    def description(self):
+    def elemental_id(self):
         """
-        Description of the version.
+        The elemental ID of the object.
 
-        :return: The description of this Version. 
+        :return: The elemental_id of this FileType. 
         :rtype: str
         """
-        return self._description
+        return self._elemental_id
 
-    @description.setter
-    def description(self, description):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        Description of the version.
+        The elemental ID of the object.
 
-        :param description: The description of this Version.
+        :param elemental_id: The elemental_id of this FileType.
         :type: str
         """
 
-        self._description = description
+        self._elemental_id = elemental_id
 
     @property
     def id(self):
         """
-        Unique integer identifying a membership.
+        Unique integer identifying a file type.
 
-        :return: The id of this Version. 
+        :return: The id of this FileType. 
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """
-        Unique integer identifying a membership.
+        Unique integer identifying a file type.
 
-        :param id: The id of this Version.
+        :param id: The id of this FileType.
         :type: int
         """
 
         self._id = id
 
     @property
     def name(self):
         """
-        Name of the version.
+        Name of the file type.
 
-        :return: The name of this Version. 
+        :return: The name of this FileType. 
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Name of the version.
+        Name of the file type.
 
-        :param name: The name of this Version.
+        :param name: The name of this FileType.
         :type: str
         """
 
         self._name = name
 
     @property
-    def number(self):
-        """
-        Version number.
-
-        :return: The number of this Version. 
-        :rtype: int
-        """
-        return self._number
-
-    @number.setter
-    def number(self, number):
-        """
-        Version number.
-
-        :param number: The number of this Version.
-        :type: int
-        """
-
-        self._number = number
-
-    @property
     def project(self):
         """
-        Unique integer identifying a project.
+        Unique integer identifying project for this file type.
 
-        :return: The project of this Version. 
+        :return: The project of this FileType. 
         :rtype: int
         """
         return self._project
 
     @project.setter
     def project(self, project):
         """
-        Unique integer identifying a project.
+        Unique integer identifying project for this file type.
 
-        :param project: The project of this Version.
+        :param project: The project of this FileType.
         :type: int
         """
 
         self._project = project
 
-    @property
-    def show_empty(self):
-        """
-        Whether to show this version on media for which no annotations exist.
-
-        :return: The show_empty of this Version. 
-        :rtype: bool
-        """
-        return self._show_empty
-
-    @show_empty.setter
-    def show_empty(self, show_empty):
-        """
-        Whether to show this version on media for which no annotations exist.
-
-        :param show_empty: The show_empty of this Version.
-        :type: bool
-        """
-
-        self._show_empty = show_empty
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -282,18 +229,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Version):
+        if not isinstance(other, FileType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Version):
+        if not isinstance(other, FileType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/version_spec.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/version_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,41 +28,46 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'bases': 'list[int]',
         'description': 'str',
+        'elemental_id': 'str',
         'name': 'str',
         'show_empty': 'bool'
     }
 
     attribute_map = {
         'bases': 'bases',
         'description': 'description',
+        'elemental_id': 'elemental_id',
         'name': 'name',
         'show_empty': 'show_empty'
     }
 
-    def __init__(self, bases=None, description='', name=None, show_empty=True, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, bases=None, description='', elemental_id=None, name=None, show_empty=True, local_vars_configuration=None):  # noqa: E501
         """VersionSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._bases = None
         self._description = None
+        self._elemental_id = None
         self._name = None
         self._show_empty = None
         self.discriminator = None
 
         if bases is not None:
             self.bases = bases
         if description is not None:
             self.description = description
+        if elemental_id is not None:
+            self.elemental_id = elemental_id
         self.name = name
         if show_empty is not None:
             self.show_empty = show_empty
 
     @property
     def bases(self):
         """
@@ -102,14 +107,35 @@
         :param description: The description of this VersionSpec.
         :type: str
         """
 
         self._description = description
 
     @property
+    def elemental_id(self):
+        """
+        Unique ID of an element
+
+        :return: The elemental_id of this VersionSpec. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        Unique ID of an element
+
+        :param elemental_id: The elemental_id of this VersionSpec.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def name(self):
         """
         Name of the version.
 
         :return: The name of this VersionSpec. 
         :rtype: str
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/version_update.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/version_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,41 +28,46 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'bases': 'list[int]',
         'description': 'str',
+        'elemental_id': 'str',
         'name': 'str',
         'show_empty': 'bool'
     }
 
     attribute_map = {
         'bases': 'bases',
         'description': 'description',
+        'elemental_id': 'elemental_id',
         'name': 'name',
         'show_empty': 'show_empty'
     }
 
-    def __init__(self, bases=None, description='', name=None, show_empty=True, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, bases=None, description='', elemental_id=None, name=None, show_empty=True, local_vars_configuration=None):  # noqa: E501
         """VersionUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._bases = None
         self._description = None
+        self._elemental_id = None
         self._name = None
         self._show_empty = None
         self.discriminator = None
 
         if bases is not None:
             self.bases = bases
         if description is not None:
             self.description = description
+        if elemental_id is not None:
+            self.elemental_id = elemental_id
         if name is not None:
             self.name = name
         if show_empty is not None:
             self.show_empty = show_empty
 
     @property
     def bases(self):
@@ -103,14 +108,35 @@
         :param description: The description of this VersionUpdate.
         :type: str
         """
 
         self._description = description
 
     @property
+    def elemental_id(self):
+        """
+        Unique ID of an element
+
+        :return: The elemental_id of this VersionUpdate. 
+        :rtype: str
+        """
+        return self._elemental_id
+
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
+        """
+        Unique ID of an element
+
+        :param elemental_id: The elemental_id of this VersionUpdate.
+        :type: str
+        """
+
+        self._elemental_id = elemental_id
+
+    @property
     def name(self):
         """
         Name of the version.
 
         :return: The name of this VersionUpdate. 
         :rtype: str
         """
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/video_clip.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/video_clip.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/models/video_definition.py` & `tator-1.0.0/tator/openapi/tator_openapi/models/video_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,25 +197,25 @@
         """
 
         self._host = host
 
     @property
     def http_auth(self):
         """
-        If specified will be used for HTTP authorization in request for media, i.e. \"bearer <token>\".
+        If specified will be used for HTTP authorization in request for media, i.e. \"bearer TOKEN\".
 
         :return: The http_auth of this VideoDefinition. 
         :rtype: str
         """
         return self._http_auth
 
     @http_auth.setter
     def http_auth(self, http_auth):
         """
-        If specified will be used for HTTP authorization in request for media, i.e. \"bearer <token>\".
+        If specified will be used for HTTP authorization in request for media, i.e. \"bearer TOKEN\".
 
         :param http_auth: The http_auth of this VideoDefinition.
         :type: str
         """
 
         self._http_auth = http_auth
```

### Comparing `tator-0.9.6/tator/openapi/tator_openapi/rest.py` & `tator-1.0.0/tator/openapi/tator_openapi/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,33 @@
         # ca_certs
         if configuration.ssl_ca_cert:
             ca_certs = configuration.ssl_ca_cert
         else:
             # if not set certificate file, use Mozilla's root certificates.
             ca_certs = certifi.where()
 
+        # Retries (see https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#urllib3.util.Retry)
+        retries = urllib3.util.Retry(total=None,
+                                     connect=5,
+                                     read=3,
+                                     redirect=10,
+                                     status=0,
+                                     other=3,
+                                     allowed_methods=frozenset({'HEAD',
+                                                                'GET',
+                                                                'PATCH',
+                                                                'PUT',
+                                                                'DELETE',
+                                                                'OPTIONS',
+                                                                'TRACE'}),
+                                     backoff_factor=10,
+                                     raise_on_redirect=False,
+                                     raise_on_status=False,
+                                     remove_headers_on_redirect=frozenset({}))
+
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
@@ -89,30 +108,32 @@
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=ca_certs,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
                 proxy_headers=configuration.proxy_headers,
+                retries=retries,
                 **addition_pool_args
             )
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=ca_certs,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
+                retries=retries,
                 **addition_pool_args
             )
 
     def request(self, method, url, query_params=None, headers=None,
                 body=None, post_params=None, _preload_content=True,
-                _request_timeout=None):
+                _request_timeout=300):
         """Perform requests.
 
         :param method: http request method
         :param url: http request url
         :param query_params: query parameters in the url
         :param headers: http request headers
         :param body: request json body, for `application/json`
@@ -121,15 +142,15 @@
                             and `multipart/form-data`
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
+                                 (connection, read) timeouts. Default is 300.
         """
         method = method.upper()
         assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
                           'PATCH', 'OPTIONS']
 
         if post_params and body:
             raise ApiValueError(
@@ -222,70 +243,70 @@
 
         if not 200 <= r.status <= 299:
             raise ApiException(http_resp=r)
 
         return r
 
     def GET(self, url, headers=None, query_params=None, _preload_content=True,
-            _request_timeout=None):
+            _request_timeout=300):
         return self.request("GET", url,
                             headers=headers,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             query_params=query_params)
 
     def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
-             _request_timeout=None):
+             _request_timeout=300):
         return self.request("HEAD", url,
                             headers=headers,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             query_params=query_params)
 
     def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
-                body=None, _preload_content=True, _request_timeout=None):
+                body=None, _preload_content=True, _request_timeout=300):
         return self.request("OPTIONS", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
     def DELETE(self, url, headers=None, query_params=None, body=None,
-               _preload_content=True, _request_timeout=None):
+               _preload_content=True, _request_timeout=300):
         return self.request("DELETE", url,
                             headers=headers,
                             query_params=query_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
     def POST(self, url, headers=None, query_params=None, post_params=None,
-             body=None, _preload_content=True, _request_timeout=None):
+             body=None, _preload_content=True, _request_timeout=300):
         return self.request("POST", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
     def PUT(self, url, headers=None, query_params=None, post_params=None,
-            body=None, _preload_content=True, _request_timeout=None):
+            body=None, _preload_content=True, _request_timeout=300):
         return self.request("PUT", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
     def PATCH(self, url, headers=None, query_params=None, post_params=None,
-              body=None, _preload_content=True, _request_timeout=None):
+              body=None, _preload_content=True, _request_timeout=300):
         return self.request("PATCH", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
```

### Comparing `tator-0.9.6/tator/transcode/__main__.py` & `tator-1.0.0/tator/transcode/prepare.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,95 @@
 #!/usr/bin/env python
 
+""" Prepares media for transcode."""
+
 import argparse
 import os
-from uuid import uuid1
+import sys
+import json
+import subprocess
 import logging
+from urllib.parse import urlparse
 
 from progressbar import progressbar
 
 from ..util import md5sum
 
 from .create_media import create_media
 from .determine_transcode import determine_transcode
-from .transcode import convert_streaming
-from .transcode import convert_archival
-from .transcode import convert_audio
-from .delete_media import delete_media
 from .make_thumbnails import make_thumbnails
 
 logger = logging.getLogger(__name__)
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Full transcode pipeline on a directory of files.')
-    parser.add_argument('path', type=str, help='Path to directory containing video files, or a video file.')
-    parser.add_argument('--extension', type=str, default='mp4', help='File extension to upload. '
-                                                                     'Ignored if path is a file.')
-    parser.add_argument('--host', type=str, default='https://www.tatorapp.com', help='Host URL.')
+    parser.add_argument('--url', type=str, help='URL where original file is hosted.')
+    parser.add_argument('--work_dir', type=str, help='Directory where info should be saved.')
+    parser.add_argument('--host', type=str, default='https://cloud.tator.io', help='Host URL.')
     parser.add_argument('--token', type=str, help='REST API token.')
     parser.add_argument('--project', type=int, help='Unique integer specifying project ID.')
     parser.add_argument('--type', type=int, help='Unique integer specifying a media type.')
+    parser.add_argument('--name', type=str, help='Name of the media.')
     parser.add_argument('--section', type=str, help='Media section name.')
-    parser.add_argument('--work_dir', type=str, help='Path to working directory. If not given, '
-                                                     'the path containing videos will be used.')
+    parser.add_argument('--attributes', type=str, help="Attributes for media")
+    parser.add_argument('--media_id', type=int, help="Existing media ID, if applicable",
+                        default=-1)
+    parser.add_argument('--gid', type=str, help="Upload group ID.")
+    parser.add_argument('--uid', type=str, help="Upload unique ID.")
+    parser.add_argument('--group_to', type=int, default=480,
+                         help='Vertical resolutions below this will be transcoded with '
+                              'multi-headed ffmpeg.')
+    parser.add_argument('--size', type=int, help="Size in bytes of the uploaded file.")
     return parser.parse_args()
 
-def get_file_paths(path, base):
+def get_file_paths(url, work_dir):
+    name = os.path.basename(urlparse(url).path)
     paths = {
-        'original': path,
-        'transcoded': base + '_transcoded',
-        'thumbnail': base + '_thumbnail.jpg',
-        'thumbnail_gif': base + '_thumbnail_gif.gif',
-        'segments': base + '_segments.json',
+        'original': url,
+        'thumbnail': os.path.join(work_dir, 'thumbnail.jpg'),
+        'thumbnail_gif': os.path.join(work_dir, 'thumbnail_gif.gif'),
+        'media_id': os.path.join(work_dir, 'media_id.txt'),
+        'workloads': os.path.join(work_dir, 'workloads.json'),
     }
     return paths
 
-def transcode_single(path, args, gid):
-    """Transcodes a single file.
-    """
+if __name__ == '__main__':
+    logging.basicConfig(stream=sys.stdout, level=logging.INFO)
+
+    # Parse arguments.
+    args = parse_args()
+
     # Get file paths.
-    if args.work_dir:
-        base = os.path.join(args.work_dir, os.path.splitext(os.path.basename(path))[0])
-    else:
-        base, _ = os.path.splitext(path)
-    paths = get_file_paths(path, base)
+    paths = get_file_paths(args.url, args.work_dir)
 
     # Get md5 for the file.
-    md5 = md5sum(paths['original'])
+    md5 = md5sum(args.url, args.size)
 
     # Get base filename.
-    name = os.path.basename(paths['original'])
-
-    # Generate a UID for this file.
-    uid = str(uuid1())
+    if args.name:
+        name = args.name
+    else:
+        name = os.path.basename(paths['original'])
 
     # Create the media object.
-    media_id = create_media(args.host, args.token, args.project, args.type, args.section, name, md5,
-                            gid, uid)
-
-    try:
-        # Make thumbnails.
-        make_thumbnails(args.host, args.token, media_id, paths['original'], paths['thumbnail'],
-                        paths['thumbnail_gif'])
-
-        # Determine transcodes that need to be done.
-        workloads = determine_transcode(args.host, args.token, args.type, path, group_to=1080)
-
-        # Transcode the video file.
-        for workload in workloads:
-            category = workload['category']
-            del workload['category']
-            del workload['id']
-            if category == 'streaming':
-                convert_streaming(**workload, host=args.host, token=args.token, media=media_id,
-                                  outpath=paths['transcoded'])
-            elif category == 'archival':
-                del workload['configs']
-                convert_archival(**workload, host=args.host, token=args.token, media=media_id,
-                                 outpath=paths['transcoded'])
-            elif category == 'audio':
-                del workload['configs']
-                del workload['raw_width']
-                del workload['raw_height']
-                convert_audio(**workload, host=args.host, token=args.token, media=media_id,
-                              outpath=paths['transcoded'])
-    except:
-        logging.exception('')
-        delete_media(args.host, args.token, media_id)
-        raise RuntimeError(f"Transcode of file {path} failed!")
-    
-if __name__ == '__main__':
-    args = parse_args()
-    gid = str(uuid1())
-    if os.path.isdir(args.path):
-        file_list = []
-        for root, dirs, files in os.walk(args.path):
-            for fname in files:
-                if fname.endswith(args.extension):
-                    path = os.path.join(root, fname)
-                    file_list.append(path)
-        for path in progressbar(file_list):
-            transcode_single(path, args, gid)
+    if args.media_id == -1:
+        media_id = create_media(args.host, args.token, args.project, args.type, args.section,
+                                name, md5, args.gid, args.uid, args.attributes, args.url)
     else:
-        transcode_single(args.path, args, gid)
+        media_id = args.media_id
+
+    # Determine transcodes that need to be done.
+    workloads = determine_transcode(
+        args.host, args.token, args.type, media_id, paths['original'], args.group_to
+    )
+    for workload in workloads:
+        workload['configs'] = ','.join(workload['configs'])
+    with open(paths['workloads'], 'w') as f:
+        json.dump(workloads, f)
+
+    with open(paths['media_id'], 'w') as f:
+        f.write(str(media_id))
+
+    # Make thumbnails.
+    make_thumbnails(args.host, args.token, media_id, paths['original'], paths['thumbnail'],
+                    paths['thumbnail_gif'])
+
```

### Comparing `tator-0.9.6/tator/transcode/black.mp4` & `tator-1.0.0/tator/transcode/black.mp4`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/transcode/create_media.py` & `tator-1.0.0/tator/transcode/create_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
     parser.add_argument('--media_type', type=int, help="Unique integer identifying a media type.")
     parser.add_argument('--section', type=str, help="Name of section to upload to.")
     parser.add_argument('--name', type=str, help="Name of file.")
     parser.add_argument('--md5', type=str, help="md5 sum of file.")
     parser.add_argument('--gid', type=str, help="Upload group ID.")
     parser.add_argument('--uid', type=str, help="Upload unique ID.")
     parser.add_argument('--output', type=str, help="Where to dump media ID.")
-    parser.add_argument('--attributes', type=str, help="Attributes for media")
+    parser.add_argument('--attributes', type=str, help="Attributes for media as a JSON string.")
     return parser.parse_args()
 
-def create_media(host, token, project, media_type, section, name, md5, gid, uid, attributes=None):
+def create_media(host, token, project, media_type, section, name, md5, gid, uid,
+                 attributes=None, url=None):
     """ Creates a media object and returns the ID.
 
     :param host: Host URL.
     :param token: API token.
     :param project: Unique integer identifying a project.
     :param media_type: Unique integer identifying a media type.
     :param section: Section name.
@@ -37,15 +38,17 @@
         'name': name,
         'md5': md5,
         'gid': gid,
         'uid': uid
     }
     if attributes:
         spec.update({'attributes': json.loads(attributes)})
-    response = api.create_media(project, media_spec=spec)
+    if url:
+        spec.update({'url': url})
+    response = api.create_media_list(project, body=[spec])
 
     assert isinstance(response, CreateResponse)
     media_id = response.id
 
     return media_id
 
 if __name__ == '__main__':
```

### Comparing `tator-0.9.6/tator/transcode/delete_media.py` & `tator-1.0.0/tator/transcode/delete_media.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/transcode/determine_transcode.py` & `tator-1.0.0/tator/transcode/determine_transcode.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import argparse
 import logging
 import os
 
 from ..openapi.tator_openapi.models import MediaType
 from ..util.get_api import get_api
 from ..util.get_parser import get_parser
-from .transcode import get_length_info
+from .transcode import find_best_encoder, get_length_info
 from collections import defaultdict
 
 STREAMING_RESOLUTIONS=[144, 360, 480, 720, 1080]
 
 logger = logging.getLogger(__name__)
 
 def parse_args():
@@ -22,29 +22,32 @@
     parser.add_argument('--project', type=int, help='Unique integer identifying a project. This is '
                                                     'only needed if media_type is -1.')
     parser.add_argument('--media_type', type=int, help='Unique integer identifying a media type.')
     parser.add_argument('--group_to', type=int, default=480,
                          help='Vertical resolutions below this will be transcoded with '
                               'multi-headed ffmpeg.')
     parser.add_argument('--output', help='Path to output json file.')
+    parser.add_argument('--media-id', type=int, help="Existing media ID, if applicable", default=-1)
     return parser.parse_args()
 
-def determine_transcode(host, token, media_type, path, group_to):
+def determine_transcode(host, token, media_type, media_id, path, group_to):
     """ Determine transcode workloads to be performed.
 
     :param host: URL of host.
     :param token: API token.
     :param media_type: Unique integer identifying a media type.
+    :param media_id: Unique integer identifying the media object for which the transcode workloads
+                     need to be determined.
     :param path: Path to original file.
     :param group_to: Resolutions less or equal to this will be grouped into one workload.
     """
     cmd = [
         "ffprobe",
         "-v","error",
-        "-show_entries", "stream",
+        "-show_entries", "stream:format=duration",
         "-print_format", "json",
         "-count_frames",
         "-skip_frame", "nokey",
         path,
     ]
     output = subprocess.run(cmd, stdout=subprocess.PIPE, check=True).stdout
     video_info = json.loads(output)
@@ -53,14 +56,15 @@
     for idx, stream in enumerate(video_info["streams"]):
         if stream["codec_type"] == "video":
             stream_idx=idx
         if stream["codec_type"] == "audio":
             logger.info("Found Audio Track")
             audio=True
     stream = video_info["streams"][stream_idx]
+    stream = {**video_info.get("format", {}), **stream}
     fps, num_frames = get_length_info(stream)
 
     # Handle up to but not exceeding FHD
     height = int(stream["height"])
     width = int(stream["width"])
 
     # Handle rotated videos
@@ -79,67 +83,139 @@
     if media_type == -1:
         media_types = api.get_media_type_list(args.project)
         for media_type_obj in media_types:
             if media_type_obj.dtype == 'video':
                 break
     else:
         media_type_obj = api.get_media_type(media_type)
+
     assert isinstance(media_type_obj, MediaType)
 
+    # Get media object
+    try:
+        media_obj = api.get_media(media_id)
+    except:
+        media_obj = None
+
+    if media_obj:
+        # Get existing streaming/archival/audio file info
+        if media_obj.media_files and media_obj.media_files.streaming:
+            existing_streaming_resolutions = set(
+                [
+                    (stream_info.resolution[0], find_best_encoder(stream_info.codec))
+                    for stream_info in media_obj.media_files.streaming
+                ]
+            )
+        else:
+            existing_streaming_resolutions = []
+
+        if media_obj.media_files and media_obj.media_files.archival:
+            existing_archival_resolutions = set(
+                [
+                    (archival_info.resolution[0], find_best_encoder(archival_info.codec))
+                    for archival_info in media_obj.media_files.archival
+                ]
+            )
+        else:
+            existing_archival_resolutions = []
+
+        # If at least one audio track exists, don't retranscode it
+        if audio and media_obj.media_files and media_obj.media_files.audio:
+            audio = False
+    else:
+        existing_streaming_resolutions = set()
+        existing_archival_resolutions = set()
+
     available_resolutions = STREAMING_RESOLUTIONS
     crf_map = defaultdict(lambda: 23)
     codec_map = defaultdict(lambda: 'libx264')
+    preset_map = defaultdict(lambda: '')
     try:
         if media_type_obj.streaming_config:
             available_resolutions = []
             for config in media_type_obj.streaming_config:
                 available_resolutions.append(config.resolution)
                 crf_map[config.resolution] = config.crf
                 codec_map[config.resolution] = config.vcodec
+                preset_map[config.resolution] = config.preset
     except Exception as e:
         # Likely an old version of the server
         # TODO: Remove me someday
         print(e)
         print("Defaulting to STREAMING_RESOLUTIONS")
     print(f"Selected Resolutions {available_resolutions}")
+
+    # Returns `True` if the resolution is smaller than the source video and it does not exist
+    # already in the media object
+    def _is_resolution_needed(resolution):
+        if resolution > height:
+            return False
+        if (resolution, codec_map[resolution]) in existing_streaming_resolutions:
+            return False
+        return True
+
     # Make a list of resolutions needed
-    resolutions = [resolution for resolution in available_resolutions if resolution < height]
-    if height <= max(available_resolutions) and not height in resolutions:
-        resolutions.append(height)
-
-    # Streaming workloads (low res)
-    workloads = [{
-        'category': 'streaming',
-        'path': path,
-        'raw_height': height,
-        'raw_width': width,
-        'configs': [f"{resolution}:{crf_map[resolution]}:{codec_map[resolution]}"
-                    for resolution in resolutions if resolution <= group_to],
-    }]
+    resolutions = [res for res in available_resolutions if _is_resolution_needed(res)]
+    if height < max(available_resolutions) and not height in resolutions:
+        smallest_higher_res = min(r for r in available_resolutions if r > height)
+
+        if not (height, codec_map[smallest_higher_res]) in existing_streaming_resolutions:
+            # copy personality form the nearest higher resolution
+            crf_map[height] = crf_map[smallest_higher_res]
+            codec_map[height] = codec_map[smallest_higher_res]
+            preset_map[height] = preset_map[smallest_higher_res]
+            resolutions.append(height)
+
+    # Streaming workloads (lower res)
+    if any(res <= group_to for res in resolutions):
+        workloads = [
+            {
+                "category": "streaming",
+                "path": path,
+                "raw_height": height,
+                "raw_width": width,
+                "configs": [
+                    f"{res}:{crf_map[res]}:{codec_map[res]}:{preset_map[res]}"
+                    for res in resolutions
+                    if res <= group_to
+                ],
+            }
+        ]
+    else:
+        workloads = []
 
     # Streaming workloads (higher res)
-    workloads += [{
-        'category': 'streaming',
-        'path': path,
-        'raw_height': height,
-        'raw_width': width,
-        'configs': [f"{resolution}:{crf_map[resolution]}:{codec_map[resolution]}"],
-    } for resolution in resolutions if resolution > group_to]
+    workloads.extend(
+        {
+            "category": "streaming",
+            "path": path,
+            "raw_height": height,
+            "raw_width": width,
+            "configs": [
+                f"{res}:{crf_map[res]}:{codec_map[res]}:{preset_map[res]}"
+            ],
+        }
+        for res in resolutions
+        if res > group_to
+    )
 
     # Archival workloads
     # This will force all transcodes to run `convert_archival` on the raw video,
     # which will fetch the media type and take action based on the returned 
     # archive config.
-    workloads += [{
-        'category': 'archival',
-        'path': path,
-        'raw_height': height,
-        'raw_width': width,
-        'configs': [],
-    }]
+    if not existing_archival_resolutions:
+        workloads.append(
+            {
+                'category': 'archival',
+                'path': path,
+                'raw_height': height,
+                'raw_width': width,
+                'configs': [],
+            }
+        )
 
     # Audio workloads
     if audio:
         workloads += [{
             'category': 'audio',
             'path': path,
             'raw_height': height,
@@ -151,13 +227,14 @@
     for idx in range(len(workloads)):
         workloads[idx]['id'] = idx
 
     return workloads
 
 if __name__ == '__main__':
     args = parse_args()
-    workloads = determine_transcode(args.host, args.token, args.media_type, args.path,
-                                    args.group_to)
+    workloads = determine_transcode(
+        args.host, args.token, args.media_type, args.media_id, args.path, args.group_to
+    )
     for workload in workloads:
         workload['configs'] = ','.join(workload['configs'])
     with open(args.output, 'w') as f:
         json.dump(workloads, f)
```

### Comparing `tator-0.9.6/tator/transcode/make_fragment_info.py` & `tator-1.0.0/tator/transcode/make_fragment_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,16 +63,16 @@
                     if child['name'] == 'traf':
                         for grandchild in child['children']:
                             if grandchild['name'] == 'trun':
                                 block['frame_start'] = currentFrame
                                 block['frame_samples'] = grandchild['sample count']
                                 currentFrame += grandchild['sample count']
             info['segments'].append(block)
-            
+
             currentOffset+=block['size']
 
 
     json.dump(info, outputFile)
-            
+
 if __name__=="__main__":
     args = parse_args()
-    make_fragment_info(args['input'], args['output'])
+    make_fragment_info(args.input, args.output)
```

### Comparing `tator-0.9.6/tator/transcode/make_thumbnails.py` & `tator-1.0.0/tator/transcode/make_thumbnails.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,106 +16,156 @@
 from ..openapi.tator_openapi.models import MessageResponse
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Makes thumbnails for a video.')
-    parser.add_argument('--host', type=str, default='https://www.tatorapp.com', help='Host URL.')
+    parser.add_argument('--host', type=str, default='https://cloud.tator.io', help='Host URL.')
     parser.add_argument('--token', type=str, help='REST API token.')
     parser.add_argument('--media', type=int, help='Unique integer identifying a media.')
     parser.add_argument('input', type=str, help='Path to input file.')
     parser.add_argument("-o", "--output", type=str, help='Path to output thumbnail.')
     parser.add_argument("-g", "--gif", type=str, help='Path to output thumbnail gif.')
     return parser.parse_args()
 
 def get_metadata(path):
     cmd = [
         "ffprobe",
         "-v","error",
-        "-show_entries", "stream",
+        "-show_entries", "stream:format=duration",
         "-print_format", "json",
         "-select_streams", "v",
         "{}".format(path)
     ]
     output = subprocess.run(cmd, stdout=subprocess.PIPE, check=True).stdout
 
     logger.info("Got info = {}".format(output))
     video_info = json.loads(output)
-    stream = video_info["streams"][0]
+    stream_idx=0
+    for idx, stream in enumerate(video_info["streams"]):
+        if stream["codec_type"] == "video":
+            stream_idx=idx
+            break
+    stream = video_info["streams"][stream_idx]
+    stream = {**video_info.get("format", {}), **stream}
 
     fps, num_frames = get_length_info(stream)
     # Fill in object information based on probe
     codec = stream["codec_name"]
     width = stream["width"]
     height = stream["height"]
 
     return (codec, fps, num_frames, width, height)
 
-def make_thumbnails(host, token, media_id, video_path, thumb_path, thumb_gif_path):
+def make_thumbnails(host, token, media_id, video_path, thumb_path, thumb_gif_path, only_keyframes=False):
     """ Makes thumbnails and gets metadata for original file.
     """
+    # Check for the existence of thumbnails
+    api = get_api(host, token)
+    media_obj = api.get_media(media_id)
+
+    needs_thumb_img = not (media_obj.media_files and media_obj.media_files.thumbnail)
+    needs_thumb_gif = not (media_obj.media_files and media_obj.media_files.thumbnail_gif)
+
+    if not (needs_thumb_img or needs_thumb_gif):
+        logger.info(f"Thumbnail upload skipped for media '{media_id}', they already exist")
+        return
+
     # Get metadata for original file.
     codec, fps, num_frames, width, height = get_metadata(video_path)
 
     # Create thumbnail.
-    cmd = ["ffmpeg", "-y", "-i", video_path, "-vf", "scale=256:-1", "-vframes", "1", thumb_path]
-    subprocess.run(cmd, check=True)
-
-    with tempfile.TemporaryDirectory() as dirname:
-        pts_scale = (fps / 3) * (10 / num_frames)
-
-        # Create gif thumbnail.
-        cmd1 = ["ffmpeg", "-y"]
-        if num_frames > 10000:
-            cmd2 = ["-skip_frame", "nokey"]
-        else:
-            cmd2 = []
-        cmd3 = ["-i", video_path, "-vf", f"scale=256:-1:flags=lanczos,setpts={pts_scale}*PTS",
-                "-r", "3", os.path.join(dirname, "%09d.jpg")]
-        cmd = cmd1 + cmd2 + cmd3
-        subprocess.run(cmd, check=True)
-        cmd = [
-            "ffmpeg", "-y", "-r", "3", "-i", os.path.join(dirname, '%09d.jpg'), "-vf",
-            "split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse",
-            "-r", "3",
-            thumb_gif_path
-        ]
+    if needs_thumb_img:
+        cmd = ["ffmpeg", "-y", "-i", video_path, "-vf", "scale=256:-1", "-vframes", "1", thumb_path]
         subprocess.run(cmd, check=True)
 
+    if needs_thumb_gif:
+        with tempfile.TemporaryDirectory() as dirname:
+            pts_scale = (fps / 3) * (10 / num_frames)
+
+            # Create gif thumbnail.
+            cmd1 = ["ffmpeg", "-y"]
+            if only_keyframes or num_frames > 10000:
+                cmd2 = ["-skip_frame", "nokey"]
+            else:
+                cmd2 = []
+            cmd3 = [
+                "-i",
+                video_path,
+                "-vf",
+                f"scale=256:-1:flags=lanczos,setpts={pts_scale}*PTS",
+                "-r",
+                "3",
+                os.path.join(dirname, "%09d.jpg"),
+            ]
+            cmd = cmd1 + cmd2 + cmd3
+            subprocess.run(cmd, check=True)
+            cmd = [
+                "ffmpeg",
+                "-y",
+                "-r",
+                "3",
+                "-i",
+                os.path.join(dirname, "%09d.jpg"),
+                "-vf",
+                "split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse",
+                "-r",
+                "3",
+                thumb_gif_path,
+            ]
+            subprocess.run(cmd, check=True)
+
     # Upload thumbnail and thumbnail gif.
-    api = get_api(host, token)
-    media_obj = api.get_media(media_id)
-    for progress, thumbnail_info in _upload_file(api, media_obj.project, thumb_path,
-                                                 media_id=media_id,
-                                                 filename=os.path.basename(thumb_path)):
-        pass
-    for progress, thumbnail_gif_info in _upload_file(api, media_obj.project, thumb_gif_path,
-                                                     media_id=media_id,
-                                                     filename=os.path.basename(thumb_gif_path)):
-        pass
-
-    # Open images to get output resolution.
-    thumb_image = Image.open(thumb_path)
-    thumb_gif_image = Image.open(thumb_gif_path)
-
-    # Create image definitions for thumbnails.
-    thumb_def = {'path': thumbnail_info.key,
-                 'size': os.stat(thumb_path).st_size,
-                 'resolution': [thumb_image.height, thumb_image.width],
-                 'mime': f'image/{thumb_image.format.lower()}'}
-    thumb_gif_def = {'path': thumbnail_gif_info.key,
-                     'size': os.stat(thumb_gif_path).st_size,
-                     'resolution': [thumb_gif_image.height, thumb_gif_image.width],
-                     'mime': f'image/{thumb_gif_image.format.lower()}'}
-
-    response = api.create_image_file(media_id, role='thumbnail', image_definition=thumb_def)
-    assert isinstance(response, MessageResponse)
-    response = api.create_image_file(media_id, role='thumbnail_gif', image_definition=thumb_gif_def)
-    assert isinstance(response, MessageResponse)
+    if needs_thumb_img:
+        for progress, thumbnail_info in _upload_file(
+            api,
+            media_obj.project,
+            thumb_path,
+            media_id=media_id,
+            filename=os.path.basename(thumb_path),
+        ):
+            pass
+
+    if needs_thumb_gif:
+        for progress, thumbnail_gif_info in _upload_file(
+            api,
+            media_obj.project,
+            thumb_gif_path,
+            media_id=media_id,
+            filename=os.path.basename(thumb_gif_path),
+        ):
+            pass
+
+    # Open images to get output resolution and create image definitions for thumbnails.
+    if needs_thumb_img:
+        thumb_image = Image.open(thumb_path)
+        thumb_def = {
+            "path": thumbnail_info.key,
+            "size": os.stat(thumb_path).st_size,
+            "resolution": [thumb_image.height, thumb_image.width],
+            "mime": f"image/{thumb_image.format.lower()}",
+        }
+
+        response = api.create_image_file(media_id, role="thumbnail", image_definition=thumb_def)
+        assert isinstance(response, MessageResponse)
+
+    if needs_thumb_gif:
+        thumb_gif_image = Image.open(thumb_gif_path)
+        thumb_gif_def = {
+            "path": thumbnail_gif_info.key,
+            "size": os.stat(thumb_gif_path).st_size,
+            "resolution": [thumb_gif_image.height, thumb_gif_image.width],
+            "mime": f"image/{thumb_gif_image.format.lower()}",
+        }
+
+        response = api.create_image_file(
+            media_id, role="thumbnail_gif", image_definition=thumb_gif_def
+        )
+        assert isinstance(response, MessageResponse)
 
     # Update the media object.
     response = api.update_media(media_id, media_update={
         'num_frames': num_frames,
         'fps': fps,
         'codec': codec,
         'width': width,
```

### Comparing `tator-0.9.6/tator/transcode/transcode.py` & `tator-1.0.0/tator/transcode/transcode.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,55 +20,83 @@
 encoder_lookup=None
 
 def find_best_encoder(codec):
     """ Find the best encoder based on what is available on the system """
     global encoder_lookup
     if encoder_lookup is None:
         # Default codecs
-        encoder_lookup={"hevc": "libsvt_hevc",
-                        "h264": "libx264"}
+        encoder_lookup={"hevc": "libx265",
+                        "h264": "libx264",
+                        "av1": "libsvtav1"}
         cmd = [
             "ffmpeg",
             "-encoders" ]
         output=subprocess.run(cmd,stdout=subprocess.PIPE,check=True).stdout.decode()
+        # Look for QSV, but use VAAPI frontend
+        # TODO: Use `vainfo` directly to query available hardware entry points
+        if output.find("libsvt_hevc") >= 0:
+            encoder_lookup["hevc"] = "libsvt_hevc"
         if output.find("hevc_qsv") >= 0:
-            encoder_lookup["hevc"] = "hevc_qsv"
+            encoder_lookup["hevc"] = "hevc_vaapi"
         if output.find("h264_qsv") >= 0:
-            encoder_lookup["h264"] = "h264_qsv"
+            encoder_lookup["h264"] = "h264_vaapi"
+        if output.find("av1_qsv") >= 0:
+            encoder_lookup["av1"] = "av1_vaapi"
         print(f"encoder_lookup = {encoder_lookup}")
     return encoder_lookup.get(codec,codec)
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Transcodes a raw video.')
     parser.add_argument('--url', type=str, help='URL where original file is hosted.')
     parser.add_argument('--work_dir', type=str, help='Directory where info should be saved.')
-    parser.add_argument('--host', type=str, default='https://www.tatorapp.com', help='Host URL.')
+    parser.add_argument('--host', type=str, default='https://cloud.tator.io', help='Host URL.')
     parser.add_argument('--token', type=str, help='REST API token.')
     parser.add_argument('--media', type=int, help='Unique integer identifying a media.')
     parser.add_argument('--category', required=True, help='One of streaming, archival, or audio.')
     parser.add_argument('--raw_width', type=int, help='Pixel width of original video.')
     parser.add_argument('--raw_height', type=int, help='Pixel height of original video.')
     parser.add_argument('--configs', type=str, help='Comma separated list of output configs, '
                                                     'format is resolution:crf:codec.')
     parser.add_argument('--size', type=int, help='Size of the file, if not inferrable')
     return parser.parse_args()
 
+def get_length_of_file(path):
+    cmd = [
+        "ffprobe",
+        "-v","error",
+        "-show_entries", "stream:format=duration",
+        "-print_format", "json",
+        "-select_streams", "v",
+        path,
+    ]
+    output = subprocess.run(cmd, stdout=subprocess.PIPE, check=True).stdout
+    video_info = json.loads(output)
+    stream_idx=0
+    for idx, stream in enumerate(video_info["streams"]):
+        if stream["codec_type"] == "video":
+            stream_idx=idx
+            break
+    stream = video_info["streams"][stream_idx]
+    stream = {**video_info.get("format", {}), **stream}
+    fps, length = get_length_info(stream)
+    return fps, length
+
 def make_video_definition(path, size=None):
     cmd = [
         "ffprobe",
         "-v","error",
         "-show_entries", "stream",
         "-print_format", "json",
         "-select_streams", "v",
         path,
     ]
     output = subprocess.run(cmd, stdout=subprocess.PIPE, check=True).stdout
     video_info = json.loads(output)
     stream_idx=0
-    if size is None:
+    if size is None or size <= 0:
         size = os.stat(path).st_size
     for idx, stream in enumerate(video_info["streams"]):
         if stream["codec_type"] == "video":
             stream_idx=idx
             break
     stream = video_info["streams"][stream_idx]
     video_def = {"resolution": (stream["height"], stream["width"]),
@@ -83,68 +111,96 @@
     # Get workload parameters.
     os.makedirs(outpath, exist_ok=True)
 
     # Convert settings into resolution/crf/codec.
     resolutions = [int(config.split(':')[0]) for config in configs]
     crfs = [config.split(':')[1] for config in configs]
     codecs = [config.split(':')[2] for config in configs]
+    presets = [config.split(':')[3] for config in configs]
 
     # Need to get avg_framerate
     cmd = [
         "ffprobe",
         "-v","error",
         "-show_entries", "stream",
         "-print_format", "json",
         "-select_streams", "v",
         path,
     ]
     output = subprocess.run(cmd, stdout=subprocess.PIPE, check=True).stdout
     video_info = json.loads(output)
     avg_frame_rate=video_info['streams'][0]['avg_frame_rate']
+    input_pixel_format=video_info['streams'][0]['pix_fmt']
 
     vid_dims = [raw_height, raw_width]
     cmd = [
         "ffmpeg", "-y",
         "-i", path,
         "-i", os.path.join(os.path.dirname(os.path.abspath(__file__)), "black.mp4"),
     ]
 
-    per_res = ["-an",
-        "-metadata:s", "handler_name=tator",
-        "-g", "25",
-        "-preset", "fast",
-        "-movflags",
-        "faststart+frag_keyframe+empty_moov+default_base_moof",
-        "-tune", "fastdecode",]
+    vaapi_present = [c for c in codecs if find_best_encoder(c).find('vaapi') >= 0]
+    print(codecs)
+    print(vaapi_present)
+    if vaapi_present:
+        cmd.extend(['-init_hw_device', 'vaapi=hw',
+                    '-filter_hw_device', 'hw'])
 
     print(f"Transcoding to {resolutions}")
     for ridx, resolution in enumerate(resolutions):
+        per_res = ["-an",
+            "-metadata:s", "handler_name=tator",
+            "-g", "25",
+            "-movflags",
+            "faststart+frag_keyframe+empty_moov+default_base_moof"]
         logger.info(f"Generating resolution @ {resolution}")
         output_file = os.path.join(outpath, f"{resolution}.mp4")
         codec = find_best_encoder(codecs[ridx])
         quality_flag = "-crf"
         pixel_format = "yuv420p"
-        if codec.find("qsv") >= 0:
+        hw_upload = ''
+        preset = presets[ridx]
+        if codec.find("vaapi") >= 0:
             quality_flag = "-global_quality"
             pixel_format = "nv12"
+            # add format filter for vaapi + add hwupload to incantation
+            hw_upload=f'[uf{ridx}];[uf{ridx}]format={pixel_format}[format{ridx}];[format{ridx}]hwupload'
+
+        if codec.find('264') > 0:
+            preset = preset if preset else 'fast'
+            per_res.extend(["-preset", preset,
+                            "-tune", "fastdecode"])
+        if codec.find('libsvtav1') >= 0:
+            preset = preset if preset else '5'
+            per_res.extend(['-preset', preset])
+
         cmd.extend([*per_res,
                     "-vcodec", codec,
                     "-pix_fmt", pixel_format,
                     quality_flag, crfs[ridx],
                     "-filter_complex",
                     # Scale the black mp4 to the input resolution prior to concating and scaling back down.
-                    f"[0:v:0]yadif[a{ridx}];[a{ridx}]setsar=1[vid{ridx}];[1:v:0]scale={vid_dims[1]}:{vid_dims[0]},setsar=1[bv{ridx}];[vid{ridx}][bv{ridx}]concat=n=2:v=1:a=0[rv{ridx}];[rv{ridx}]scale=-2:{resolution}[catv{ridx}];[catv{ridx}]pad=ceil(iw/2)*2:ceil(ih/2)*2[norate{ridx}];[norate{ridx}]fps={avg_frame_rate}[outv{ridx}]",
+                    f"[0:v:0]yadif[a{ridx}];[a{ridx}]setsar=1[vid{ridx}];[1:v:0]scale={vid_dims[1]}:{vid_dims[0]},setsar=1[bv{ridx}];[vid{ridx}][bv{ridx}]concat=n=2:v=1:a=0[rv{ridx}];[rv{ridx}]scale=-2:{resolution}[catv{ridx}];[catv{ridx}]pad=ceil(iw/2)*2:ceil(ih/2)*2[norate{ridx}];[norate{ridx}]fps={avg_frame_rate}{hw_upload}[outv{ridx}]",
                     "-map", f"[outv{ridx}]",
                     output_file])
 
     logger.info('ffmpeg cmd = {}'.format(cmd))
     subprocess.run(cmd, check=True)
+
     api = get_api(host, token)
     media_obj = api.get_media(media)
 
+    for ridx, resolution in enumerate(resolutions):
+        output_file = os.path.join(outpath, f"{resolution}.mp4")
+        _, res_length = get_length_of_file(output_file)
+        length_delta = abs((media_obj.num_frames - res_length)/media_obj.num_frames)
+        assert length_delta < 0.1 # Assert length delta is less than 10 percent.
+
+    
+
     for resolution in resolutions:
         output_file = os.path.join(outpath, f"{resolution}.mp4")
 
         segments_file = os.path.join(outpath, f"{resolution}.json")
         make_fragment_info(output_file, segments_file)
 
         logger.info("Uploading transcoded file...")
@@ -169,15 +225,15 @@
         assert isinstance(response, MessageResponse)
 
 def default_archival_upload(api, host, media, path, encoded, size):
     # Default action if no archive config is upload raw video.
     media_obj = api.get_media(media)
     logger.info(f"Uploading original file as archival...")
     for progress, upload_info in _upload_file(api, media_obj.project, path,
-                                              media_id=media, filename=os.path.basename(path),file_size=size):
+                                              media_id=media, filename=os.path.basename(path), file_size=size):
         logger.info(f"Progress: {progress}%")
     video_def = make_video_definition(path, size)
 
     # If video was encoded, set codec_mime to video/mp4; otherwise do
     # not set codec_mime.
     if encoded:
         video_def['codec_mime'] = 'video/mp4'
@@ -190,36 +246,37 @@
 def convert_archival(host,
                      token,
                      media,
                      path,
                      outpath,
                      raw_width,
                      raw_height,
-                     size=None):
+                     size=None,
+                     explicit_config=None):
     # Retrieve this media's type to inspect archive config.
     api = get_api(host, token)
     media_obj = api.get_media(media)
-    media_type = api.get_media_type(media_obj.meta)
-
-    if media_type.archive_config is None:
-        default_archival_upload(api, host, media, path, False, size)
-    else:
-        for idx, archive_config in enumerate(media_type.archive_config):
-            if archive_config.encode is None:
+    media_type = api.get_media_type(media_obj.type)
+    config = explicit_config or media_type.archive_config
+    if config is not None:
+        for idx, archive_config in enumerate(config):
+            os.makedirs(outpath, exist_ok=True)
+            output_file = os.path.join(outpath, f"archival_{idx}.mp4")
+            if archive_config.encode.vcodec == 'copy':
                 # If no encode, just use the original file.
                 output_file = path
             else:
                 # Encode the media to archival format.
-                os.makedirs(outpath, exist_ok=True)
-                output_file = os.path.join(outpath, f"archival_{idx}.mp4")
                 codec = find_best_encoder(archive_config.encode.vcodec)
                 quality_flag = "-crf"
                 pixel_format = "yuv420p"
                 tune_settings = ["-preset", archive_config.encode.preset,
                                  "-tune", archive_config.encode.tune]
+                if archive_config.encode.movflags:
+                    tune_settings.extend(['-movflags', archive_config.encode.movflags])
                 if codec.find("qsv") >= 0:
                     quality_flag = "-global_quality"
                     pixel_format = "nv12"
                     tune_settings=[] #QSV doesn't do tuning
                 elif codec == "libsvt_hevc":
                     # SVT for HEVC does not do tuning or CRF
                     tune_settings=[]
@@ -239,15 +296,15 @@
                     cmd += ["-tag:v", "avc1"]
                 cmd.append(output_file)
                     
                 logger.info('ffmpeg cmd = {}'.format(cmd))
                 subprocess.run(cmd, check=True)
 
             if archive_config.s3_storage is None:
-                default_archival_upload(api, host, media, output_file, True)
+                default_archival_upload(api, host, media, output_file, True, size)
             else:
                 import boto3
                 # Get credentials from config object.
                 aws_access_key = archive_config.s3_storage.aws_access_key
                 aws_secret_access_key = archive_config.s3_storage.aws_secret_access_key
                 bucket_name = archive_config.s3_storage.bucket_name
                 logger.info(f"Uploading {output_file} to S3 bucket {bucket_name}...")
@@ -310,43 +367,37 @@
     """ Given a json dump of the stream return the length of the video """
     fps_fractional = stream["avg_frame_rate"].split("/")
     fps = float(fps_fractional[0]) / float(fps_fractional[1])
 
     start_time = float(stream["start_time"])
     if 'duration' in stream:
         seconds = float(stream["duration"])
-    elif 'tags' in stream:
-        if 'DURATION' in stream['tags']:
-            length = stream['tags']['DURATION'].split(':')
-            seconds = float(length[0])*3600
-            seconds += float(length[1])*60
-            seconds += float(length[2])
+    elif 'tags' in stream and 'DURATION' in stream['tags']:
+        length = stream['tags']['DURATION'].split(':')
+        seconds = float(length[0])*3600
+        seconds += float(length[1])*60
+        seconds += float(length[2])
     else:
         raise Exception('No way to determine file length!')
 
     num_frames = float(fps * seconds)
     return fps,int(num_frames)
 
 if __name__ == '__main__':
+    logging.basicConfig(stream=sys.stdout, level=logging.INFO)
+
     # Parse arguments.
     args = parse_args()
 
-    # Get path to save file.
-    fname = os.path.basename(urlparse(args.url).path)
-    path = os.path.join(args.work_dir, fname)
-
-    # Download the file.
-    subprocess.run(['wget', '-O', path, args.url])
-
     if args.category == 'streaming':
         if args.configs == '':
             configs = []
         else:
             configs = [res for res in args.configs.split(',')]
-        convert_streaming(args.host, args.token, args.media, path, args.work_dir,
+        convert_streaming(args.host, args.token, args.media, args.url, args.work_dir,
                           args.raw_width, args.raw_height, configs)
     elif args.category == 'archival':
-        convert_archival(args.host, args.token, args.media, path, args.work_dir,
+        convert_archival(args.host, args.token, args.media, args.url, args.work_dir,
                          args.raw_width, args.raw_height, args.size)
     elif args.category == 'audio':
-        convert_audio(args.host, args.token, args.media, path, args.work_dir)
+        convert_audio(args.host, args.token, args.media, args.url, args.work_dir)
```

### Comparing `tator-0.9.6/tator/util/__init__.py` & `tator-1.0.0/tator/util/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 """ Utility functions for interacting with the Tator platform """
-from tator.util.chunked_create import chunked_create as chunked_create
 from tator.util.get_api import get_api
 from tator.util.chunked_create import chunked_create
+from tator.util.download_attachment import download_attachment
 from tator.util.download_media import download_media
 from tator.util.download_temporary_file import download_temporary_file
+from tator.util.upload_attachment import upload_attachment
 from tator.util.upload_media import upload_media
-from tator.util.upload_media_archive import upload_media_archive
 from tator.util.chunked_file_list import chunked_file_list
 from tator.util.upload_temporary_file import upload_temporary_file
 from tator.util.import_media import import_media
+from tator.util.live_stream import make_live_stream
 from tator.util.md5sum import md5sum
 from tator.util.multi_stream import make_multi_stream
 from tator.util.get_images import get_images
 from tator.util.full_state_graphic import full_state_graphic
 from tator.util.to_dataframe import to_dataframe
 from tator.util.register_algorithm import register_algorithm
+from tator.util.register_applet import register_applet
+from tator.util.update_applet import update_applet
 from tator.util.clone_media_list import clone_media_list
 from tator.util.clone_localization_list import clone_localization_list
 from tator.util.clone_state_list import clone_state_list
 from tator.util.clone_leaf_list import clone_leaf_list
 from tator.util.clone_media_type import clone_media_type
 from tator.util.clone_localization_type import clone_localization_type
 from tator.util.clone_state_type import clone_state_type
 from tator.util.clone_leaf_type import clone_leaf_type
 from tator.util.clone_section import clone_section
 from tator.util.clone_version import clone_version
 from tator.util.clone_membership import clone_membership
+from tator.util.concat import make_concat
+from tator.util.find_single_change import find_single_change
+from tator.util.get_paginator import get_paginator
+from tator.util.media_util import MediaUtil
+from tator.util.media_manipulation import supplement_video_to_media
+
```

### Comparing `tator-0.9.6/tator/util/_download_file.py` & `tator-1.0.0/tator/util/_download_file.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/chunked_create.py` & `tator-1.0.0/tator/util/chunked_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,15 @@
     """ Breaks a create_*_list operation into chunks.
 
     Example:
 
     .. code-block:: python
 
         created_ids = []
-        for response in tator.util.chunked_create(api.create_localization_list, 1,
-                                                  localization_spec=my_long_list):
+        for response in tator.util.chunked_create(api.create_localization_list, 1, body=my_long_list):
             created_ids += response.id
 
     :param func: Function to call on each chunk.
     :param project: Unique integer identifying a project.
     :returns: Generator that yields a response.
     """
     for key in kwargs:
```

### Comparing `tator-0.9.6/tator/util/chunked_file_list.py` & `tator-1.0.0/tator/util/chunked_file_list.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/clone_leaf_list.py` & `tator-1.0.0/tator/util/clone_leaf_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     parent_id = leaf.parent
     if parent_id:
         if parent_id in parent_mapping:
              parent_id = parent_mapping[parent_id]
         else:
             raise ValueError(f"Source parent ID {parent_id} missing from parent_mapping!")
     # Swap leaf type IDs.
-    leaf_type_id = leaf.meta
+    leaf_type_id = leaf.type
     if leaf_type_id in leaf_type_mapping:
         leaf_type_id = leaf_type_mapping[leaf_type_id]
     else:
         raise ValueError(f"Source leaf_type ID {leaf_type_id} missing from "
                           "leaf_type_mapping!")
     # Fill in required fields for post.
     spec = {'name': leaf.name,
@@ -92,13 +92,12 @@
     spec = [_convert_for_post(leaf, leaf_type_mapping, parent_mapping)
             for leaf in leafs]
 
     # Create the leafs.
     created_ids = []
     total_leafs = len(spec)
     for idx in range(0, total_leafs, 500):
-        response = dest_api.create_leaf_list(dest_project,
-                                              leaf_spec=spec[idx:idx+500])
+        response = dest_api.create_leaf_list(dest_project, body=spec[idx:idx+500])
         created_ids += response.id
         id_map = {src.id: dest_id for src, dest_id in zip(leafs[idx:idx+500], response.id)}
         yield (len(created_ids), total_leafs, response, id_map)
```

### Comparing `tator-0.9.6/tator/util/clone_leaf_type.py` & `tator-1.0.0/tator/util/clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/clone_localization_list.py` & `tator-1.0.0/tator/util/clone_localization_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # Check for media mapping.
     media_id = loc.media
     if media_id in media_mapping:
         media_id = media_mapping[media_id]
     else:
         raise ValueError(f"Source media ID {media_id} missing from media_mapping!")
     # Swap localization type IDs.
-    localization_type_id = loc.meta
+    localization_type_id = loc.type
     if localization_type_id in localization_type_mapping:
         localization_type_id = localization_type_mapping[localization_type_id]
     else:
         raise ValueError(f"Source localization_type ID {localization_type_id} missing from "
                           "localization_type_mapping!")
     # Check for parent mapping.
     parent_id = loc.parent
@@ -117,15 +117,18 @@
         raise Exception("Query parameters must include a project!")
 
     # Set the dest_api if not given.
     if dest_api is None:
         dest_api = src_api
 
     # Start by getting list of localizations to be cloned.
-    locs = src_api.get_localization_list(**query_params)
+    if 'localization_id_query' in query_params:
+        locs = src_api.get_localization_list_by_id(**query_params)
+    else:
+        locs = src_api.get_localization_list(**query_params)
 
     # Find parent localizations.
     parent_ids = [int(loc.parent) for loc in locs if loc.parent]
     parent_locs = [loc for loc in locs if loc.id in parent_ids]
     child_locs = [loc for loc in locs if loc.id not in parent_ids]
 
     # Create spec for parent localizations.
@@ -134,27 +137,25 @@
                    for loc in parent_locs]
 
     # Create parent localizations first.
     created_ids = []
     total_localizations = len(locs)
     parent_mapping = {}
     for idx in range(0, len(parent_locs), 500):
-        response = dest_api.create_localization_list(dest_project,
-                                                     localization_spec=parent_spec[idx:idx+500])
+        response = dest_api.create_localization_list(dest_project, body=parent_spec[idx:idx+500])
         created_ids += response.id
         id_map = {src.id: dest_id for src, dest_id in zip(parent_locs[idx:idx+500], response.id)}
         parent_mapping = {**parent_mapping, **id_map}
         yield (len(created_ids), total_localizations, response, id_map)
 
     # Convert spec for child localizations.
     child_spec = [_convert_for_post(loc, localization_type_mapping, version_mapping,
                                     media_mapping, parent_mapping)
                   for loc in child_locs]
 
     # Create the localizations.
     for idx in range(0, len(child_locs), 500):
-        response = dest_api.create_localization_list(dest_project,
-                                                     localization_spec=child_spec[idx:idx+500])
+        response = dest_api.create_localization_list(dest_project, body=child_spec[idx:idx+500])
         created_ids += response.id
         id_map = {src.id: dest_id for src, dest_id in zip(locs[idx:idx+500], response.id)}
         yield (len(created_ids), total_localizations, response, id_map)
```

### Comparing `tator-0.9.6/tator/util/clone_localization_type.py` & `tator-1.0.0/tator/util/clone_localization_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,17 @@
             'description': type_obj.description,
             'dtype': type_obj.dtype,
             'grouping_default': type_obj.grouping_default,
             'color_map': type_obj.color_map,
             'line_width': type_obj.line_width,
             'visible': type_obj.visible,
             'attribute_types': type_obj.attribute_types}
-    dest_media_types = []
+    dest_media_types = set()
     for src_media_type in type_obj.media:
         if src_media_type in media_type_mapping:
-            dest_media_types.append(media_type_mapping[src_media_type])
+            dest_media_types.add(media_type_mapping[src_media_type])
         else:
             raise ValueError(f"Media type mapping does not contain source media ID {src_media_type}!")
-    spec['media_types'] = dest_media_types
+    spec['media_types'] = list(dest_media_types)
     if dest_api is None:
         dest_api = src_api
     return dest_api.create_localization_type(dest_project, localization_type_spec=spec)
```

### Comparing `tator-0.9.6/tator/util/clone_media_list.py` & `tator-1.0.0/tator/util/clone_media_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         # Set up destination.
         self.dest_api = dest_api
         self.dest_project = dest_project
 
     def __call__(self, src_url, media_id=None, return_url=False):
         """ Downloads a file from one host and uploads it to another.
-        
+
         :param src_url: Relative URL of source file to download.
         :param media_id: Destination media ID.
         :param return_url: Return download URL if true.
         :returns: URL or path of destination file.
         """
         parsed = urlparse(src_url)
         filename = os.path.basename(parsed.path)
@@ -57,15 +57,15 @@
             out = upload_info.key
         if return_url:
             out = self.dest_api.get_download_info(self.dest_project,
                                                   {'keys': [upload_info.key]})[0].url
         return out
 
 def clone_media_list(src_api, query_params, dest_project, media_mapping={}, dest_type=-1,
-                     dest_section='', dest_api=None):
+                     dest_section='', dest_api=None, ignore_transfer=False):
     """ Clone media list.
 
     This can be used to clone media from one project to another or from one
     host to another. In the case of the same host, the media files are not
     copied. If the destination host is different (`dest_api` is a :class:`tator.TatorApi`
     object), the transcoded files for each media object is downloaded and then
     uploaded to the other host, and a new :class:`tator.Media` object is created.
@@ -110,14 +110,16 @@
     :param media_mapping: Mapping between source and destination media IDs. Only used
         if the media list contains multi media types and the clone is being done for
         different hosts.
     :param dest_type: Unique integer identifying destination media type. If set to
         -1, the media type is set to the first media type in the project.
     :param dest_section: Name of destination section.
     :param dest_api: :class:`tator.TatorApi` object corresponding to destination host.
+    :param ignore_transfer: True if media files should not be transferred. Media object will still be created.
+        Paths in media_files will be invalid.
     :returns: Generator containing number of files created, number of files total,
         most recent response from media creation operation, and mapping between original IDs
         and created IDs.
     """
     # Make sure query has a project.
     if 'project' not in query_params:
         raise Exception("Query parameters must include a project!")
@@ -155,15 +157,16 @@
                                                     'dest_type': dest_type,
                                                 })
             created_ids += response.id
             id_map = {src_id: dest_id for src_id, dest_id in zip(media_ids, response.id)}
             yield (len(created_ids), total_files, response, id_map)
     else:
         # Clone media to another host.
-        transfer = HostTransfer(src_api, src_project, dest_api, dest_project)
+        if not ignore_transfer:
+            transfer = HostTransfer(src_api, src_project, dest_api, dest_project)
         for media in medias:
             # Set up media spec.
             attributes = media.attributes
             if 'tator_user_sections' in attributes:
                 attributes.pop('tator_user_sections', None)
             media_spec = {
                 'type': dest_type,
@@ -179,21 +182,23 @@
             }
             if media.gid:
                 media_spec['gid'] = media.gid
             if media.uid:
                 media_spec['uid'] = media.uid
 
             # Create the media object.
-            response = dest_api.create_media(dest_project, media_spec=media_spec)
+            response = dest_api.create_media_list(dest_project, body=[media_spec])
             id_map = {media.id: response.id}
 
             # Transfer videos.
             if media.media_files:
                 media_files = media.media_files.to_dict()
                 for key in ['streaming', 'archival', 'audio', 'image', 'thumbnail', 'thumbnail_gif']:
+                    if ignore_transfer:
+                        continue
                     if media_files.get(key):
                         for item in media_files[key]:
                             media_def = {k: v for k, v in item.items()
                                          if v is not None}
                             src_path = media_def.pop('path', None)
                             media_def['path'] = transfer(src_path, media_id=response.id)
                             if key == 'streaming':
```

### Comparing `tator-0.9.6/tator/util/clone_media_type.py` & `tator-1.0.0/tator/util/clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/clone_membership.py` & `tator-1.0.0/tator/util/clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/clone_section.py` & `tator-1.0.0/tator/util/clone_section.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,18 +30,14 @@
     :param src_section_id: Unique integer identifying section to clone.
     :param dest_project: Unique integer identifying destination project.
     :param dest_api: :class:`tator.TatorApi` object corresponding to destination host.
     :returns: Response from section creation request.
     """
     section_obj = src_api.get_section(src_section_id)
     spec = {'name': section_obj.name}
-    if section_obj.annotation_bools:
-        spec['annotation_bools'] = section_obj.annotation_bools
-    if section_obj.media_bools:
-        spec['media_bools'] = section_obj.media_bools
-    if section_obj.lucene_string:
-        spec['lucene_string'] = section_obj.lucene_string
+    if section_obj.object_search:
+        spec['object_search'] = section_obj.object_search
     if section_obj.tator_user_sections:
         spec['tator_user_sections'] = section_obj.tator_user_sections
     if dest_api is None:
         dest_api = src_api
     return dest_api.create_section(dest_project, section_spec=spec)
```

### Comparing `tator-0.9.6/tator/util/clone_state_list.py` & `tator-1.0.0/tator/util/clone_state_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     for idx, localization_id in enumerate(localization_ids):
         if localization_id in localization_mapping:
             localization_ids[idx] = localization_mapping[localization_id]
         else:
             raise ValueError(f"Source localization ID {localization_id} missing from "
                               "localization_mapping!")
     # Swap state type IDs.
-    state_type_id = state.meta
+    state_type_id = state.type
     if state_type_id in state_type_mapping:
         state_type_id = state_type_mapping[state_type_id]
     else:
         raise ValueError(f"Source state_type ID {state_type_id} missing from "
                           "state_type_mapping!")
     # Fill in required fields for post.
     spec = {'type': state_type_id,
@@ -113,23 +113,25 @@
         raise Exception("Query parameters must include a project!")
 
     # Set the dest_api if not given.
     if dest_api is None:
         dest_api = src_api
 
     # Start by getting list of states to be cloned.
-    states = src_api.get_state_list(**query_params)
+    if 'state_id_query' in query_params:
+        states = src_api.get_state_list_by_id(**query_params)
+    else:
+        states = src_api.get_state_list(**query_params)
 
     # Convert to new spec.
     spec = [_convert_for_post(state, version_mapping, media_mapping, localization_mapping,
                               state_type_mapping) for state in states]
 
     # Create the states.
     created_ids = []
     total_states = len(spec)
     for idx in range(0, total_states, 500):
-        response = dest_api.create_state_list(dest_project,
-                                              state_spec=spec[idx:idx+500])
+        response = dest_api.create_state_list(dest_project, body=spec[idx:idx+500])
         created_ids += response.id
         id_map = {src.id: dest_id for src, dest_id in zip(states[idx:idx+500], response.id)}
         yield (len(created_ids), total_states, response, id_map)
```

### Comparing `tator-0.9.6/tator/util/clone_state_type.py` & `tator-1.0.0/tator/util/clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/clone_version.py` & `tator-1.0.0/tator/util/clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/download_media.py` & `tator-1.0.0/tator/util/download_media.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 import os
 import math
 
 import requests
 
 from ._download_file import _download_file
+from ..openapi.tator_openapi.models import ImageDefinition, VideoDefinition
 
 def _is_none_or_eq(variable, match):
     """  :returns: True if `variable` is None or equals `match` """
     return variable is None or variable == match
 
-def _find_best_match(media_list, quality):
+def _find_best_match(media_list, quality, codec_or_mime=None):
     """ Given a media list find the closest quality
         :param media_list: list of Media definitons either
                            :class:`tator.models.ImageDefinition` or
                            :class:`tator.models.VideoDefinition`.
         :param int quality: Vertical resolution to match (or None for best)
-
+        :param str codec_or_mime: Specified codec or mime if multiple versions
+                                  of 1 resolution exist. E.g. h264 or image/avif
     """
     # Without pulling in numpy we have to do this in an explicit loop
     available = [x.resolution[0] for x in media_list]
+
     match_idx = -1
     best_quality = max(available)
     quality = best_quality if quality is None else quality
     best_distance = best_quality+1
     for idx,val in enumerate(available):
+        # Bounce out of any non matching codecs
+        if codec_or_mime:
+            media_info = media_list[idx]
+            if type(media_info) == ImageDefinition and media_info.mime != codec_or_mime:
+                continue
+            if type(media_info) == VideoDefinition and media_info.codec != codec_or_mime:
+                continue
         distance = abs(val-quality)
         if distance < best_distance:
             best_distance = distance
             match_idx = idx
 
     assert match_idx >= 0, "Unable to find match"
 
     return match_idx
 
-def download_media(api, media, out_path, quality=None,media_type=None):
+def download_media(api, media, out_path, quality=None,media_type=None, codec_or_mime=None):
     """ Download a media file from Tator to an off-line location.
 
     Example:
 
     .. code-block:: python
 
         api = tator.get_api(host, token)
@@ -58,14 +68,16 @@
     :param api: :class:`tator.TatorApi` object.
     :param media: :class:`tator.Media` object.
     :param path-like out_path: Path to where to download.
     :param int quality: Attempts to fetch this resolution (defaults to best)
     :param str media_type: The desired item to download (archival, streaming,
                            image, thumbnail, or thumbnail_gif). Not all types
                            are valid for all media.
+    :param str codec_or_mime: The desired codec or mime if multiple exist at
+                              the same resolution. e.g. h264 for video or image/jpeg for images.
     :returns: Generator the yields progress (0-100).
     """
     assert media_type in [None,
                           'streaming',
                           'archival',
                           'image',
                           'thumbnail',
@@ -77,19 +89,19 @@
         streaming = media.media_files.streaming
         streaming = streaming if streaming else []
         image = media.media_files.image
         thumbnail = media.media_files.thumbnail
         thumbnail_gif = media.media_files.thumbnail_gif
 
         if _is_none_or_eq(media_type,"archival") and len(archival) > 0:
-            url = archival[_find_best_match(archival,quality)].path
+            url = archival[_find_best_match(archival,quality, codec_or_mime)].path
         elif _is_none_or_eq(media_type,"streaming") and len(streaming) > 0:
-            url = streaming[_find_best_match(streaming,quality)].path
+            url = streaming[_find_best_match(streaming,quality, codec_or_mime)].path
         elif _is_none_or_eq(media_type,"image") and image:
-            url = image[_find_best_match(image,quality)].path
+            url = image[_find_best_match(image,quality, codec_or_mime)].path
         elif media_type == "thumbnail":
             url = thumbnail[_find_best_match(thumbnail,quality)].path
         elif media_type == "thumbnail_gif":
             url = thumbnail_gif[_find_best_match(thumbnail_gif,quality)].path
         else:
             assert False, f"Unable to deduce download file media={media.id}"
     else:
```

### Comparing `tator-0.9.6/tator/util/download_temporary_file.py` & `tator-1.0.0/tator/util/download_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/full_state_graphic.py` & `tator-1.0.0/tator/util/full_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/get_images.py` & `tator-1.0.0/tator/util/get_images.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/import_media.py` & `tator-1.0.0/tator/util/import_media.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,32 +68,29 @@
     :param attributes: [Optional] Attributes to apply to media object.
     :param media_id: [Optional] Unique ID of existing media object.
     :param size: [Optional] Size of the file in bytes. Required if the
         given URL does not accept HEAD requests.
     :param _request_timeout: [Optional] Timeout setting for API requests in seconds.
     :returns: Generator that yields tuple containing progress (0-100) and a
         response. The response is `None` until the last yield, when the response
-        is the response object from :meth:`tator.TatorApi.create_media` or 
+        is the response object from :meth:`tator.TatorApi.create_media_list` or
         :meth:`tator.TatorApi.transcode`.
     """
     if md5==None:
         # To compute md5, download the first 10MB to temporary file.
         md5 = _hosted_md5(url)
     if upload_uid is None:
         upload_uid = str(uuid1())
     if upload_gid is None:
         upload_gid = str(uuid1())
     if fname is None:
         fname = os.path.basename(urlsplit(url).path)
     if section is None:
         section="Imported Files"
 
-    host = api.api_client.configuration.host
-    token = api.api_client.configuration.api_key['Authorization']
-    prefix = api.api_client.configuration.api_key_prefix['Authorization']
     media_type = api.get_media_type(type_id, _request_timeout=_request_timeout)
     project_id = media_type.project
     spec = {
         'type': type_id,
         'uid': upload_uid,
         'gid': upload_gid,
         'url': url,
@@ -106,10 +103,11 @@
     if size is not None:
         spec['size'] = size
     # Create video or image.
     if media_type.dtype == 'video':
         response = api.transcode(project_id, transcode_spec=spec,
                                  _request_timeout=_request_timeout)
     else:
-        response = api.create_media(project_id, media_spec=spec,
-                                    _request_timeout=_request_timeout)
+        response = api.create_media_list(
+            project_id, body=[spec], _request_timeout=_request_timeout
+        )
     return response
```

### Comparing `tator-0.9.6/tator/util/md5sum.py` & `tator-1.0.0/tator/util/md5sum.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,27 @@
         # if it doesn't work
         try:
             r = requests.head(fname)
             proposed_size = int(r.headers.get('content-length',0))
             if proposed_size:
                 size = proposed_size
         except:
-            if size is None:
+            if size is None or size <= 0:
                 raise Exception("Must supply size if HTTP server doesn't support HEAD requests for size.")
     else:
         with open(fname, 'rb') as f:
             for chunk in iter(lambda: f.read(CHUNK_SIZE), b''):
                 md5.update(chunk)
                 break # Exit after one chunk
 
     # Compute file size if not given. (Already set for HTTP files)
-    if size is None:
+    if (size is None or size <= 0) and os.path.exists(fname):
         size = os.stat(fname).st_size
 
+    # If size still not computed, raise an exception.
+    if size is None or size <= 0:
+        raise Exception(f"Could not determine size of file {fname}!")
+
     # Salt in file size.
     out = hashlib.md5()
     out.update(md5.hexdigest().encode('utf-8') + str(size).encode('utf-8'))
     return out.hexdigest()
```

### Comparing `tator-0.9.6/tator/util/multi_stream.py` & `tator-1.0.0/tator/util/multi_stream.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 from .md5sum import md5sum
 from ._upload_file import _upload_file
 from ._download_file import _download_file
 from ..openapi.tator_openapi.models import MessageResponse
 
 logger = logging.getLogger(__name__)
 
-def make_multi_stream(api, type_id, layout, name, media_ids, section, quality=None):
+def make_multi_stream(api, type_id, layout, name, media_ids, section,
+                      quality=None, frame_offset=None):
     """ Uploads a single media file.
 
     :param api: :class:`tator.TatorApi` object.
     :param type_id: Unique integer identifying a multi-stream media type.
     :param layout: 2 element list of integers defining layout as [rows, cols].
     :param name: Name of the file to use
     :param media_ids: List of media_ids to multi-stream
     :param section: Section name. If this section does not exist it will be created.
     :param quality: [Optional] Media section to upload to.
+    :param frame_offset: [Optional] Frame offsets to apply to each stream.
     :returns: Response from media object creation.
     """
 
     # Fetch the stuff we need to download files
     config = api.api_client.configuration
     host = config.host
     token = config.api_key['Authorization']
@@ -67,84 +69,85 @@
         'Authorization': f'{prefix} {token}',
         'Content-Type': f'application/json',
         'Accept-Encoding': 'gzip',
     }
 
     # Download the thumbnails into a temporary
     with tempfile.TemporaryDirectory() as d:
-        for pos, media_id in enumerate(media_ids):
-            media = media_lookup[media_id]
-            thumbnails = media.media_files.thumbnail
-            if thumbnails:
-                thumb = thumbnails[0].path
-            thumbnail_gifs = media.media_files.thumbnail_gif
-            if thumbnail_gifs:
-                thumb_gif = thumbnail_gifs[0].path
-            for _ in _download_file(api, media.project, thumb,
-                                    os.path.join(d, f"thumb_{pos:09d}.jpg")):
-                pass
-            for _ in _download_file(api, media.project, thumb_gif,
-                                    os.path.join(d, f"gif_{pos:09d}.gif")):
-                pass
-
-        cmd = ["ffmpeg",
-               "-y",
-               "-i", "thumb_%09d.jpg",
-               "-vf",f"tile={layout[1]}x{layout[0]},scale=256:-1",
-               os.path.join(d,"tiled_thumb.jpg")]
-        subprocess.run(cmd,cwd=d,check=True)
-
-        input_files=[]
-        rows=layout[0]
-        cols=layout[1]
-        filter_graph=""
-        idx = 0
-        for row in range(rows):
-            for col in range(cols):
-                filter_graph += f"[{idx}:v]"
-                idx+=1
-                if cols > 1 and col + 1 == cols:
-                    filter_graph += f"hstack=inputs={cols}[r{row}];"
-        for row in range(rows):
-            if cols > 1:
-                filter_graph += f"[r{row}]"
-        if rows > 1 and row + 1 == rows:
-            filter_graph+=f'vstack=inputs={rows}[tiled_gif];[tiled_gif]'
-        filter_graph+=f'scale=256:-1[raw];[raw]split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse[final]'
-        print(filter_graph)
-        for pos,_ in enumerate(media_ids):
-            input_files.extend(['-i', f'gif_{pos:09d}.gif'])
-        cmd = ["ffmpeg",
-               "-y",
-               *input_files,
-               "-filter_complex", filter_graph,
-               "-map", "[final]",
-               "-shortest",
-               "tiled_gif.gif"]
-
-        subprocess.run(cmd, cwd=d, check=True)
-
-        md5=md5sum(os.path.join(d,'tiled_gif.gif'))
+        try:
+            for pos, media_id in enumerate(media_ids):
+                media = media_lookup[media_id]
+                md5=media.md5
+                thumbnail_gifs = media.media_files.thumbnail_gif
+                if thumbnail_gifs:
+                    thumb_gif = thumbnail_gifs[0].path
+                for _ in _download_file(api, media.project, thumb_gif,
+                                        os.path.join(d, f"gif_{pos:09d}.gif")):
+                    pass
+
+            input_files=[]
+            rows=layout[0]
+            cols=layout[1]
+            filter_graph=""
+            for row in range(rows):
+                # Resize each input to a square prior to grid
+                for col in range(cols):
+                    filter_graph += f"[{col}:v]scale=256:256[resize{col}];"
+                for col in range(cols):
+                    filter_graph += f"[resize{col}]"
+                    if cols > 1 and col + 1 == cols:
+                        filter_graph += f"hstack=inputs={cols}[r{row}];"
+            for row in range(rows):
+                if cols > 1:
+                    filter_graph += f"[r{row}]"
+            if rows > 1 and row + 1 == rows:
+                filter_graph+=f'vstack=inputs={rows}[tiled_gif];[tiled_gif]'
+            filter_graph+=f'scale=256:-1[raw];[raw]split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse[final]'
+            print(filter_graph)
+            for pos,_ in enumerate(media_ids):
+                input_files.extend(['-i', f'gif_{pos:09d}.gif'])
+
+            # Create GIF
+            cmd = ["ffmpeg",
+                "-y",
+                *input_files,
+                "-filter_complex", filter_graph,
+                "-map", "[final]",
+                "-shortest",
+                "tiled_gif.gif"]
+            subprocess.run(cmd, cwd=d, check=True)
+
+            # Create thumbnail from first frame of GIF
+            cmd = ["ffmpeg",
+                "-y",
+                "-i", "tiled_gif.gif",
+                "-vf",f"select=eq(n\\,0)",
+                "-q:v", "3",
+                os.path.join(d,"tiled_thumb.jpg")]
+            subprocess.run(cmd,cwd=d,check=True)
+
+            thumb_path = os.path.join(d,'tiled_thumb.jpg')
+            thumb_gif_path = os.path.join(d,'tiled_gif.gif')
+        except:
+            thumb_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "tator-symbol.png")
+            thumb_gif_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "tator-symbol.gif")
 
         media_spec = {'attributes': attributes,
-                      'name': name,
-                      'md5': md5,
-                      'section': section_obj.name,
-                      'type': type_id}
-
-        resp = api.create_media(project, media_spec)
+                'name': name,
+                'md5': md5,
+                'section': section_obj.name,
+                'type': type_id}
+        resp = api.create_media_list(project, [media_spec])
         print(f"Created {resp.id}")
-
-        thumb_path = os.path.join(d,'tiled_thumb.jpg')
-        thumb_gif_path = os.path.join(d,'tiled_gif.gif')
+        
         for progress, thumbnail_info in _upload_file(api, project, thumb_path,
-                                                     media_id=resp.id, filename='tiled_thumb.jpg'):
-            logger.info(f"Thumbnail upload progress: {progress}%")
+                                                        media_id=resp.id, filename='tiled_thumb.jpg'):
+                logger.info(f"Thumbnail upload progress: {progress}%")
         for progress, thumbnail_gif_info in _upload_file(api, project, thumb_gif_path,
-                                                         media_id=resp.id, filename='tiled_gif.gif'):
+                                                        media_id=resp.id, filename='tiled_gif.gif'):
             logger.info(f"Thumbnail gif upload progress: {progress}%")
 
         # Open images to get output resolution.
         thumb_image = Image.open(thumb_path)
         thumb_gif_image = Image.open(thumb_gif_path)
 
         # Create image definitions for thumbnails.
@@ -163,11 +166,14 @@
         assert isinstance(response, MessageResponse)
 
         # Add the multi definition.
         multi_def = {"layout": layout,
                      "ids": media_ids}
         if quality:
             multi_def.update({"quality": quality})
+        if frame_offset:
+            assert len(frame_offset) == len(media_ids), "Length of frame offsets did not match length of media IDs!"
+            multi_def.update({"frameOffset": frame_offset})
         api.update_media(resp.id, {"multi": multi_def})
 
         return resp
```

### Comparing `tator-0.9.6/tator/util/register_algorithm.py` & `tator-1.0.0/tator/util/register_algorithm.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def register_algorithm(
     host: str,
     token: str,
     project: int,
     manifest: str,
     algorithm_name: str,
     files_per_job: int,
+    categories: list=[],
     description: str='',
     cluster_id: int=None) -> None:
     """ Registers an algorithm argo workflow using the provided parameters
 
     This will upload the given manifest file, save it to tator, and the new
     server side URL will be used when registering the workflow. This may change
     the filename of the manifest file.
@@ -55,13 +56,14 @@
     spec = tator.models.Algorithm(
         name=algorithm_name,
         project=project,
         user=user_id,
         description=description,
         manifest=response.url,
         cluster=cluster_id,
-        files_per_job=files_per_job)
+        files_per_job=files_per_job,
+        categories=categories)
 
     response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
 
     log_msg = f"Algorithm registered with ID: {response.id}"
     logger.info(log_msg)
```

### Comparing `tator-0.9.6/tator/util/to_dataframe.py` & `tator-1.0.0/tator/util/to_dataframe.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator/util/upload_media.py` & `tator-1.0.0/tator/util/upload_media.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from urllib.parse import urljoin
 
 from ._upload_file import _upload_file
 from .md5sum import md5sum
 
 def upload_media(api, type_id, path, md5=None, section=None, fname=None,
                  upload_gid=None, upload_uid=None, chunk_size=10*1024*1024,
-                 attributes=None, media_id=None):
+                 attributes=None, media_id=None, timeout=30, max_workers=10):
     """ Uploads a single media file.
 
     Example:
 
     .. code-block:: python
 
         api = tator.get_api(host, token)
@@ -22,46 +22,53 @@
             print(f"Upload progress: {progress}%")
         print(response.message)
 
     :param api: :class:`tator.TatorApi` object.
     :param type_id: Unique integer identifying a media type.
     :param path: Path to the media file.
     :param md5: [Optional] md5 sum of the media.
-    :param section: [Optional] Media section to upload to.
+    :param section: [Optional] Section name. If a section with this name does
+        not exist it will be created.
     :param fname: [Optional] Filename to use for upload.
     :param upload_gid: [Optional] Group ID of the upload.
     :param upload_uid: [Optional] Unique ID of the upload.
     :param chunk_size: [Optional] Chunk size in bytes. Default is 2MB.
     :param attributes: [Optional] Attributes to apply to media object.
     :param media_id: [Optional] Unique ID of existing media object.
+    :param timeout: [Optional] Request timeout for each upload chunk in seconds. Default is 30.
+    :param max_workers: [Optional] Max workers for concurrent requests.
     :returns: Generator that yields tuple containing progress (0-100) and a
         response. The response is `None` until the last yield, when the response
-        is the response object from :meth:`tator.TatorApi.create_media` or 
+        is the response object from :meth:`tator.TatorApi.create_media_list` or
         :meth:`tator.TatorApi.transcode`.
     """
     if md5==None:
         md5 = md5sum(path)
     if upload_uid is None:
         upload_uid = str(uuid1())
     if upload_gid is None:
         upload_gid = str(uuid1())
     if fname is None:
         fname=os.path.basename(path)
     if section is None:
         section="New Files"
 
-    host = api.api_client.configuration.host
-    token = api.api_client.configuration.api_key['Authorization']
-    prefix = api.api_client.configuration.api_key_prefix['Authorization']
-
-    mime,_ = mimetypes.guess_type(fname)
+    mime, _ = mimetypes.guess_type(fname)
+    if mime is None:
+        ext = os.path.splitext(fname)[1].lower()
+        if ext in [".mts", ".m2ts"]:
+            mime = "video/MP2T"
+        elif ext in [".avif"]:
+            mime = "image/avif"
+        elif ext in [".dng"]:
+            mime = "image/dng"
     response = api.get_media_type(type_id)
     project_id = response.project
 
-    for progress, upload_info in _upload_file(api, project_id, path, chunk_size=chunk_size):
+    for progress, upload_info in _upload_file(api, project_id, path, chunk_size=chunk_size, timeout=timeout):
         yield (progress, None)
 
     url = api.get_download_info(project_id, download_info_spec={'keys': [upload_info.key]},
                                 expiration=86400)[0].url
 
     spec = {
         'type': type_id,
@@ -69,14 +76,15 @@
         'gid': upload_gid,
         'url': url,
         'name': fname,
         'section': section,
         'md5': md5,
         'attributes': attributes,
         'media_id': media_id,
+        'size': os.stat(path).st_size,
     }
     # Initiate transcode or save image.
     if mime.find('video') >= 0:
         response = api.transcode(project_id, transcode_spec=spec)
     else:
-        response = api.create_media(project_id, media_spec=spec)
+        response = api.create_media_list(project_id, body=[spec])
     yield (100, response)
```

### Comparing `tator-0.9.6/tator/util/upload_media_archive.py` & `tator-1.0.0/tator/util/download_attachment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,40 @@
-from uuid import uuid1
-import mimetypes
 import os
 import math
-import io
-import tarfile
-import tempfile
 
-from urllib.parse import urljoin
-from urllib.parse import urlsplit
+from ._download_file import _download_file
 
-from ._upload_file import _upload_file
-from .md5sum import md5sum
+def _is_none_or_eq(variable, match):
+    """  :returns: True if `variable` is None or equals `match` """
+    return variable is None or variable == match
 
-def upload_media_archive(api, project, paths, section="Test Section", chunk_size=10*1024*1024):
-    """ Uploads multiple media files as an archive.
+def download_attachment(api, media, out_path, index=0):
+    """ Download an attachment from Tator to an off-line location.
 
     Example:
 
     .. code-block:: python
 
         api = tator.get_api(host, token)
-        for progress, response in tator.util.upload_media_archive(api, project_id, paths):
-            print(f"Upload progress: {progress}%")
-        print(response.message)
+        media = api.get_media(media_id)
+        out_path = f'/tmp/{media.name}'
+        for progress in tator.util.download_attachment(api, media, out_path):
+            print(f"Download progress: {progress}%")
+
+        #download second attachment
+        for progress in tator.util.download_attachment(api, media, out_path, index=1):
+            print(f"Download progress: {progress}%")
 
     :param api: :class:`tator.TatorApi` object.
-    :param project: Unique integer identifying a project.
-    :param paths: Path to a media archive or list of paths to media files.
-    :param section: [Optional] Media section to upload to.
-    :param chunk_size: [Optional] Chunk size in bytes. Default is 2MB.
-    :returns: Generator that yields tuple containing progress (0-100) and a
-        response. The response is `None` until the last yield, when the response
-        is the response object from :meth:`tator.TatorApi.transcode`.
+    :param media: :class:`tator.Media` object.
+    :param path-like out_path: Path to where to download.
+    :param index: Integer indicating which attachment to download.
+    :returns: Generator that yields progress (0-100).
     """
-    upload_uid = str(uuid1())
-    upload_gid = str(uuid1())
-    if isinstance(paths, list):
-        fobj = tempfile.NamedTemporaryFile(delete=False)    
-        in_mem_tar = tarfile.TarFile(mode='w', fileobj=fobj)
-        for idx, fp in enumerate(paths):
-            in_mem_tar.add(fp, os.path.basename(fp))
-        fobj.close()
-        path = fobj.name
-    else:
-        path = paths
-    for progress, upload_info in _upload_file(api, project, path):
-        yield (progress, None)
-    url = api.get_download_info(project, {'keys': [upload_info.key]})[0].url
-
-    # Initiate transcode.
-    spec = {
-        'type': -1, #Tar-based import
-        'uid': upload_uid,
-        'gid': upload_gid,
-        'url': url,
-        'name': "archive.tar",
-        'section': section,
-        'md5': "N/A",
-    }
-    response = api.transcode(project, transcode_spec=spec)
-    yield (100, response)
+    if media.media_files is not None:
+        attachment = media.media_files.attachment
+        if (attachment is None) or (len(attachment) <= index):
+            raise ValueError(f"Media {media.id} does not have an attachment at index {index}!")
+        else:
+            url = attachment[index].path
+    return _download_file(api, media.project, url, out_path)
+
```

### Comparing `tator-0.9.6/tator/util/upload_temporary_file.py` & `tator-1.0.0/tator/util/upload_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/tator.egg-info/SOURCES.txt` & `tator-1.0.0/tator.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,67 +22,109 @@
 tator/openapi/tator_openapi/api/__init__.py
 tator/openapi/tator_openapi/api/tator_api.py
 tator/openapi/tator_openapi/models/__init__.py
 tator/openapi/tator_openapi/models/affiliation.py
 tator/openapi/tator_openapi/models/affiliation_spec.py
 tator/openapi/tator_openapi/models/affiliation_update.py
 tator/openapi/tator_openapi/models/algorithm.py
-tator/openapi/tator_openapi/models/algorithm_launch.py
-tator/openapi/tator_openapi/models/algorithm_launch_spec.py
 tator/openapi/tator_openapi/models/algorithm_manifest.py
 tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
 tator/openapi/tator_openapi/models/algorithm_parameter.py
 tator/openapi/tator_openapi/models/algorithm_spec.py
 tator/openapi/tator_openapi/models/analysis.py
 tator/openapi/tator_openapi/models/analysis_spec.py
+tator/openapi/tator_openapi/models/announcement.py
+tator/openapi/tator_openapi/models/applet.py
+tator/openapi/tator_openapi/models/applet_spec.py
 tator/openapi/tator_openapi/models/archive_config.py
-tator/openapi/tator_openapi/models/attribute_bulk_update.py
+tator/openapi/tator_openapi/models/attribute_combinator_spec.py
+tator/openapi/tator_openapi/models/attribute_filter_spec.py
+tator/openapi/tator_openapi/models/attribute_operation_spec.py
 tator/openapi/tator_openapi/models/attribute_type.py
 tator/openapi/tator_openapi/models/attribute_type_delete.py
 tator/openapi/tator_openapi/models/attribute_type_spec.py
 tator/openapi/tator_openapi/models/attribute_type_update.py
-tator/openapi/tator_openapi/models/attribute_type_update_new_attribute_type.py
+tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
 tator/openapi/tator_openapi/models/audio_definition.py
 tator/openapi/tator_openapi/models/autocomplete_service.py
+tator/openapi/tator_openapi/models/auxiliary_file_definition.py
 tator/openapi/tator_openapi/models/bad_request_response.py
 tator/openapi/tator_openapi/models/bookmark.py
 tator/openapi/tator_openapi/models/bookmark_spec.py
 tator/openapi/tator_openapi/models/bookmark_update.py
+tator/openapi/tator_openapi/models/bucket.py
+tator/openapi/tator_openapi/models/bucket_gcp_config.py
+tator/openapi/tator_openapi/models/bucket_oci_config.py
+tator/openapi/tator_openapi/models/bucket_oci_native_config.py
+tator/openapi/tator_openapi/models/bucket_s3_config.py
+tator/openapi/tator_openapi/models/bucket_spec.py
+tator/openapi/tator_openapi/models/bucket_update.py
+tator/openapi/tator_openapi/models/change_log.py
+tator/openapi/tator_openapi/models/change_log_description_of_change.py
+tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
 tator/openapi/tator_openapi/models/clone_media_spec.py
 tator/openapi/tator_openapi/models/color_map.py
+tator/openapi/tator_openapi/models/concat_definition.py
 tator/openapi/tator_openapi/models/create_list_response.py
 tator/openapi/tator_openapi/models/create_response.py
 tator/openapi/tator_openapi/models/credentials.py
 tator/openapi/tator_openapi/models/download_info.py
 tator/openapi/tator_openapi/models/download_info_spec.py
 tator/openapi/tator_openapi/models/email_attachment_spec.py
 tator/openapi/tator_openapi/models/email_spec.py
 tator/openapi/tator_openapi/models/encode_config.py
 tator/openapi/tator_openapi/models/favorite.py
 tator/openapi/tator_openapi/models/favorite_spec.py
 tator/openapi/tator_openapi/models/favorite_update.py
+tator/openapi/tator_openapi/models/feed_definition.py
+tator/openapi/tator_openapi/models/file.py
+tator/openapi/tator_openapi/models/file_spec.py
+tator/openapi/tator_openapi/models/file_type.py
+tator/openapi/tator_openapi/models/file_type_spec.py
+tator/openapi/tator_openapi/models/file_type_update.py
+tator/openapi/tator_openapi/models/file_update.py
 tator/openapi/tator_openapi/models/fill.py
+tator/openapi/tator_openapi/models/float_array_query.py
+tator/openapi/tator_openapi/models/generic_file.py
+tator/openapi/tator_openapi/models/generic_file_spec.py
+tator/openapi/tator_openapi/models/get_cloned_media_response.py
 tator/openapi/tator_openapi/models/image_definition.py
+tator/openapi/tator_openapi/models/invitation.py
+tator/openapi/tator_openapi/models/invitation_spec.py
+tator/openapi/tator_openapi/models/invitation_update.py
 tator/openapi/tator_openapi/models/job.py
+tator/openapi/tator_openapi/models/job_cluster.py
+tator/openapi/tator_openapi/models/job_cluster_spec.py
 tator/openapi/tator_openapi/models/job_node.py
+tator/openapi/tator_openapi/models/job_spec.py
 tator/openapi/tator_openapi/models/leaf.py
+tator/openapi/tator_openapi/models/leaf_bulk_update.py
+tator/openapi/tator_openapi/models/leaf_id_query.py
 tator/openapi/tator_openapi/models/leaf_spec.py
 tator/openapi/tator_openapi/models/leaf_suggestion.py
 tator/openapi/tator_openapi/models/leaf_type.py
 tator/openapi/tator_openapi/models/leaf_type_spec.py
 tator/openapi/tator_openapi/models/leaf_type_update.py
 tator/openapi/tator_openapi/models/leaf_update.py
+tator/openapi/tator_openapi/models/live_definition.py
+tator/openapi/tator_openapi/models/live_update_definition.py
 tator/openapi/tator_openapi/models/localization.py
+tator/openapi/tator_openapi/models/localization_bulk_delete.py
+tator/openapi/tator_openapi/models/localization_bulk_update.py
+tator/openapi/tator_openapi/models/localization_delete.py
+tator/openapi/tator_openapi/models/localization_id_query.py
 tator/openapi/tator_openapi/models/localization_spec.py
 tator/openapi/tator_openapi/models/localization_type.py
 tator/openapi/tator_openapi/models/localization_type_spec.py
 tator/openapi/tator_openapi/models/localization_type_update.py
 tator/openapi/tator_openapi/models/localization_update.py
 tator/openapi/tator_openapi/models/media.py
+tator/openapi/tator_openapi/models/media_bulk_update.py
 tator/openapi/tator_openapi/models/media_files.py
+tator/openapi/tator_openapi/models/media_id_query.py
 tator/openapi/tator_openapi/models/media_next.py
 tator/openapi/tator_openapi/models/media_prev.py
 tator/openapi/tator_openapi/models/media_spec.py
 tator/openapi/tator_openapi/models/media_stats.py
 tator/openapi/tator_openapi/models/media_type.py
 tator/openapi/tator_openapi/models/media_type_spec.py
 tator/openapi/tator_openapi/models/media_type_update.py
@@ -92,23 +134,29 @@
 tator/openapi/tator_openapi/models/membership_update.py
 tator/openapi/tator_openapi/models/message_response.py
 tator/openapi/tator_openapi/models/multi_definition.py
 tator/openapi/tator_openapi/models/not_found_response.py
 tator/openapi/tator_openapi/models/notify_spec.py
 tator/openapi/tator_openapi/models/organization.py
 tator/openapi/tator_openapi/models/organization_spec.py
+tator/openapi/tator_openapi/models/organization_update.py
+tator/openapi/tator_openapi/models/password_reset_spec.py
 tator/openapi/tator_openapi/models/project.py
 tator/openapi/tator_openapi/models/project_spec.py
 tator/openapi/tator_openapi/models/project_update.py
 tator/openapi/tator_openapi/models/resolution_config.py
 tator/openapi/tator_openapi/models/s3_storage_config.py
 tator/openapi/tator_openapi/models/section.py
 tator/openapi/tator_openapi/models/section_spec.py
 tator/openapi/tator_openapi/models/section_update.py
 tator/openapi/tator_openapi/models/state.py
+tator/openapi/tator_openapi/models/state_bulk_delete.py
+tator/openapi/tator_openapi/models/state_bulk_update.py
+tator/openapi/tator_openapi/models/state_delete.py
+tator/openapi/tator_openapi/models/state_id_query.py
 tator/openapi/tator_openapi/models/state_merge_update.py
 tator/openapi/tator_openapi/models/state_spec.py
 tator/openapi/tator_openapi/models/state_trim_update.py
 tator/openapi/tator_openapi/models/state_type.py
 tator/openapi/tator_openapi/models/state_type_spec.py
 tator/openapi/tator_openapi/models/state_type_update.py
 tator/openapi/tator_openapi/models/state_update.py
@@ -117,14 +165,15 @@
 tator/openapi/tator_openapi/models/token.py
 tator/openapi/tator_openapi/models/transcode.py
 tator/openapi/tator_openapi/models/transcode_spec.py
 tator/openapi/tator_openapi/models/upload_completion_spec.py
 tator/openapi/tator_openapi/models/upload_info.py
 tator/openapi/tator_openapi/models/upload_part.py
 tator/openapi/tator_openapi/models/user.py
+tator/openapi/tator_openapi/models/user_spec.py
 tator/openapi/tator_openapi/models/user_update.py
 tator/openapi/tator_openapi/models/version.py
 tator/openapi/tator_openapi/models/version_spec.py
 tator/openapi/tator_openapi/models/version_update.py
 tator/openapi/tator_openapi/models/video_clip.py
 tator/openapi/tator_openapi/models/video_definition.py
 tator/transcode/__init__.py
@@ -149,52 +198,82 @@
 tator/util/clone_media_list.py
 tator/util/clone_media_type.py
 tator/util/clone_membership.py
 tator/util/clone_section.py
 tator/util/clone_state_list.py
 tator/util/clone_state_type.py
 tator/util/clone_version.py
+tator/util/concat.py
+tator/util/download_attachment.py
 tator/util/download_media.py
 tator/util/download_temporary_file.py
+tator/util/find_single_change.py
 tator/util/full_state_graphic.py
 tator/util/get_api.py
 tator/util/get_images.py
+tator/util/get_paginator.py
 tator/util/get_parser.py
 tator/util/import_media.py
+tator/util/live_stream.py
 tator/util/md5sum.py
+tator/util/media_manipulation.py
+tator/util/media_util.py
 tator/util/multi_stream.py
 tator/util/register_algorithm.py
+tator/util/register_applet.py
+tator/util/tator-symbol.png
 tator/util/to_dataframe.py
+tator/util/update_applet.py
+tator/util/upload_attachment.py
 tator/util/upload_media.py
-tator/util/upload_media_archive.py
 tator/util/upload_temporary_file.py
+test/test_a_float_array.py
 test/test_algorithm.py
 test/test_algorithm_launch.py
-test/test_analysis.py
-test/test_attribute_addition.py
-test/test_attribute_deletion.py
-test/test_attribute_mutation.py
+test/test_applet.py
+test/test_archive_date.py
+test/test_attachment.py
+test/test_attribute_type_addition.py
+test/test_attribute_type_deletion.py
+test/test_attribute_type_mutation.py
+test/test_attributes.py
+test/test_change_log.py
 test/test_clone_leaf_type.py
 test/test_clone_localization_type.py
 test/test_clone_media.py
 test/test_clone_media_type.py
 test/test_clone_membership.py
 test/test_clone_section.py
 test/test_clone_state_type.py
 test/test_clone_version.py
+test/test_collection.py
 test/test_download_media.py
 test/test_extract.py
+test/test_file.py
+test/test_file_type.py
+test/test_get_clip.py
 test/test_getframe.py
 test/test_import_media.py
 test/test_job_cancel.py
+test/test_job_cluster.py
 test/test_leaf.py
+test/test_leaf_type.py
 test/test_local_transcode.py
 test/test_localization.py
 test/test_localization_graphic.py
+test/test_localization_type.py
 test/test_media.py
+test/test_media_type.py
+test/test_pagination.py
+test/test_poly.py
 test/test_project_thumbnail.py
+test/test_search.py
 test/test_state.py
+test/test_state_graphic.py
+test/test_state_type.py
 test/test_stategraphic.py
 test/test_temporary_file.py
+test/test_tracks.py
 test/test_transcode.py
-test/test_upload_archive.py
+test/test_util_media_manipulation.py
+test/test_util_media_util.py
 test/test_version.py
```

### Comparing `tator-0.9.6/test/test_algorithm.py` & `tator-1.0.0/test/test_algorithm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import shutil
 import tempfile
 import uuid
 from textwrap import dedent
 
+import pytest
 import tator
 from tator.util._upload_file import _upload_file
 
 logger = logging.getLogger(__name__)
 
 def _create_yaml_file_str() -> str:
     """ Creates a argo manifest file used by the unit tests in this file
@@ -97,23 +98,17 @@
     Args:
         host: Project URL
         token: User token used for connecting to the host
         project: Unique identifier of test project
     """
 
     tator_api = tator.get_api(host=host, token=token)
-
-    try:
-        caught_exception = False
-        spec = tator.models.AlgorithmManifestSpec(name='test.yaml', upload_url='not_there')
+    spec = tator.models.AlgorithmManifestSpec(name='test.yaml', upload_url='not_there')
+    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException):
         tator_api.save_algorithm_manifest(project = project, algorithm_manifest_spec=spec)
-    except:
-        caught_exception = True
-
-    assert caught_exception
 
 def _upload_test_algorithm_manifest(
         host: str,
         token: str,
         project: int,
         manifest_name: str='test_manifest.yaml',
         break_yaml_file: bool=False) -> tator.models.AlgorithmManifest:
@@ -180,18 +175,15 @@
         host=host, token=token, project=project, manifest_name='test_nodupe.yaml')
     assert os.path.basename(response_1.url) == 'test_nodupe.yaml'
 
     response_2 = _upload_test_algorithm_manifest(
         host=host, token=token, project=project, manifest_name='test_nodupe.yaml')
     assert os.path.basename(response_2.url) == 'test_nodupe_0.yaml'
 
-def test_register_algorithm(
-        host: str,
-        token: str,
-        project: int) -> None:
+def test_register_algorithm(host: str, token: str, project: int, algo_project: int) -> None:
     """ Unit test for the RegisterAlgorithm endpoint
 
     Unit testing of the algorithm registration endpoint involves the following:
     - Create a request body that's fine, but has bad syntax for the .yaml file
     - Create a request body for a .yaml file that doesn't exist
     - Normal request body
 
@@ -206,86 +198,82 @@
 
     # Get the user ID
     tator_api = tator.get_api(host=host, token=token)
     user = tator_api.whoami()
     user_id = user.id
 
     # Create a request body that's fine but has bad syntax for the .yaml file
-    caught_exception = False
-    try:
-        response = _upload_test_algorithm_manifest(
-            host=host, token=token, project=project, manifest_name='test.yaml', break_yaml_file=True)
+    response = _upload_test_algorithm_manifest(
+        host=host, token=token, project=project, manifest_name='test.yaml', break_yaml_file=True)
 
-        spec = tator.models.Algorithm(
-            name=ALGO_NAME,
-            project=project,
-            user=user_id,
-            description='test_description',
-            manifest=response.url,
-            cluster=None,
-            files_per_job=1)
+    spec = tator.models.Algorithm(
+        name=ALGO_NAME,
+        project=project,
+        user=user_id,
+        description='test_description',
+        manifest=response.url,
+        cluster=None,
+        files_per_job=1)
 
+    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException):
         response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
 
-    except:
-        caught_exception = True
-
-    assert caught_exception
-
     # Create a request body for a .yaml file that doesn't exist
-    caught_exception = False
-    try:
-        spec = tator.models.Algorithm(
-            name=ALGO_NAME,
-            project=project,
-            user=user_id,
-            description='test_description',
-            manifest='ghost',
-            cluster=None,
-            files_per_job=1)
+    spec = tator.models.Algorithm(
+        name=ALGO_NAME,
+        project=project,
+        user=user_id,
+        description='test_description',
+        manifest='ghost',
+        cluster=None,
+        files_per_job=1)
 
+    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException):
         response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
 
-    except:
-        caught_exception = True
-
-    assert caught_exception
-
     # Create a normal algorithm workflow
     response = _upload_test_algorithm_manifest(
         host=host, token=token, project=project, manifest_name='test.yaml')
 
     manifest_url = response.url
 
     spec = tator.models.Algorithm(
         name=ALGO_NAME,
         project=project,
         user=user_id,
         description='test_description',
         manifest=manifest_url,
         cluster=None,
-        files_per_job=1)
+        files_per_job=1,
+        categories=['category1, category2, category3'],
+        parameters=[{'name':'param1', 'value':'bool'}])
 
     response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
 
     # Get the algorithm info
     algorithm_id = response.id
     algorithm_info = tator_api.get_algorithm(id=algorithm_id)
     spec.id = algorithm_id
     assert algorithm_info == spec
 
+    # Try to register a second algorithm with the same name
+    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException):
+        tator_api.register_algorithm(project=project, algorithm_spec=spec)
+
     # Attempt to patch the algorithm info and make sure it has been updated
     # Note: the cluster field is ignored in the patch operation
     spec = tator.models.Algorithm(
         name=str(uuid.uuid1()),
         project=project,
         user=user_id,
         description='new_test_description',
         manifest='coolfile.yaml',
-        files_per_job=2)
+        files_per_job=2,
+        categories=['categoryA, categoryB'],
+        parameters=[{'name': 'paramA', 'value':'int'}, {'name':'paramB', 'value':'string'}])
     response = tator_api.update_algorithm(id=algorithm_id, algorithm_spec=spec)
     algorithm_info = tator_api.get_algorithm(id=algorithm_id)
     spec.id = algorithm_id
     assert algorithm_info == spec
 
     # Create another algorithm workflow and verify retrieving both algorithm objects
     # using the get list method
@@ -312,23 +300,45 @@
         for spec in spec_list:
             if spec == alg:
                 found_match = True
                 break
 
         assert found_match
 
+    # Register algorithm with the same name for a different project
+    response = _upload_test_algorithm_manifest(
+        host=host, token=token, project=algo_project, manifest_name='test.yaml')
+
+    manifest_url = response.url
+
+    spec = tator.models.Algorithm(
+        name=ALGO_NAME,
+        project=algo_project,
+        user=user_id,
+        description='test_description',
+        manifest=manifest_url,
+        cluster=None,
+        files_per_job=1)
+
+    response = tator_api.register_algorithm(project=algo_project, algorithm_spec=spec)
+
     # Finally delete all the algorithms
+    tator_api.delete_algorithm(response.id)
+    algorithm_list = tator_api.get_algorithm_list(project=algo_project)
+    assert len(algorithm_list) == 0
+
     current_number_of_algs = len(algorithm_ids)
     for alg_id in algorithm_ids:
         _ = tator_api.delete_algorithm(id=alg_id)
         algorithm_list = tator_api.get_algorithm_list(project=project)
 
         current_number_of_algs -= 1
         assert len(algorithm_list) == current_number_of_algs
 
+
 def test_register_algorithm_with_missing_fields(
         host: str,
         token: str,
         project: int) -> None:
     """ Unit test for the RegisterAlgorithm endpoint focused on missing request body fields
 
     Request bodies are created with missing required fields and a workflow tries
@@ -352,91 +362,45 @@
 
     # Upload a manifest file
     response = _upload_test_algorithm_manifest(
         host=host, token=token, project=project, manifest_name='test.yaml')
     manifest_url = response.url
 
     # Missing name field
-    caught_exception = False
-    try:
-        spec = tator.models.Algorithm(
-            project=project,
-            user=user_id,
-            description=DESCRIPTION,
-            manifest=manifest_url,
-            cluster=CLUSTER,
-            files_per_job=FILES_PER_JOB)
-
-        response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
-    except:
-        caught_exception = True
+    spec = tator.models.Algorithm(
+        project=project,
+        user=user_id,
+        manifest=manifest_url,
+        files_per_job=FILES_PER_JOB)
 
-    assert caught_exception
+    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException):
+        tator_api.register_algorithm(project=project, algorithm_spec=spec)
 
     # Missing user field
-    caught_exception = False
-    try:
-        spec = tator.models.Algorithm(
-            name=NAME,
-            project=project,
-            description=DESCRIPTION,
-            manifest=manifest_url,
-            cluster=CLUSTER,
-            files_per_job=FILES_PER_JOB)
-
-        response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
-    except:
-        caught_exception = True
-
-    assert caught_exception
-
-    # Missing description field
-    caught_exception = False
-    try:
-        spec = tator.models.Algorithm(
-            name=NAME,
-            project=project,
-            user=user_id,
-            description=DESCRIPTION,
-            manifest=manifest_url,
-            cluster=CLUSTER,
-            files_per_job=FILES_PER_JOB)
-
-        response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
-    except:
-        caught_exception = True
+    spec = tator.models.Algorithm(
+        name=NAME,
+        project=project,
+        manifest=manifest_url,
+        files_per_job=FILES_PER_JOB)
 
-    assert caught_exception
+    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException):
+        tator_api.register_algorithm(project=project, algorithm_spec=spec)
 
     # Missing manifest
-    caught_exception = False
-    try:
-        spec = tator.models.Algorithm(
-            name=NAME,
-            project=project,
-            user=user_id,
-            description=DESCRIPTION,
-            cluster=CLUSTER,
-            files_per_job=FILES_PER_JOB)
-
-        response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
-    except:
-        caught_exception = True
+    spec = tator.models.Algorithm(
+        name=NAME,
+        project=project,
+        user=user_id,
+        files_per_job=FILES_PER_JOB)
 
-    assert caught_exception
+    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException):
+        tator_api.register_algorithm(project=project, algorithm_spec=spec)
 
     # Missing fields per job
-    caught_exception = False
-    try:
-        spec = tator.models.Algorithm(
-            name=NAME,
-            project=project,
-            user=user_id,
-            description=DESCRIPTION,
-            manifest=manifest_url,
-            cluster=CLUSTER)
-
-        response = tator_api.register_algorithm(project=project, algorithm_spec=spec)
-    except:
-        caught_exception = True
+    spec = tator.models.Algorithm(
+        name=NAME,
+        project=project,
+        user=user_id,
+        manifest=manifest_url)
 
-    assert caught_exception
+    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException):
+        tator_api.register_algorithm(project=project, algorithm_spec=spec)
```

### Comparing `tator-0.9.6/test/test_algorithm_launch.py` & `tator-1.0.0/test/test_algorithm_launch.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,19 +78,18 @@
             media_ids = os.getenv('TATOR_MEDIA_IDS')
             media_ids = [int(m) for m in media_ids.split(',')]
 
             tator_api = tator.get_api(host=host, token=token)
 
             print(f'{host} {token} {project} {media_ids}')
 
-            for media in media_ids:
-                name = f'test_media_{media}'
-                dq = f'test_media_id:{media}'
-                spec = tator.models.AnalysisSpec(name=name, data_query=dq)
-                _ = tator_api.create_analysis(project=project, analysis_spec=spec)
+            for media_id in media_ids:
+                media=tator_api.get_media(media_id)
+                increment = media.attributes.get('test_int',0)+1
+                tator_api.update_media(media.id, {'attributes':{'test_int': increment}})
 
         if __name__ == '__main__':
             main()
         """)
 
 def _create_workflow_manifest(
         host: str,
@@ -166,15 +165,16 @@
     # Once we're done with the tests in this module, delete the algorithm
     # (and subsequently its unique name)
     _ = tator_api.delete_algorithm(id=response.id)
 
 def _assert_algorithm_workflow_results(
     tator_api: tator.api,
     project: int,
-    expected_analysis_count: int) -> None:
+    expected_count: int,
+    media_ids: list) -> None:
     """ Polls the tator database waiting for the argo workflow to complete its database inserts
 
     Performs assert on if the count of analysis entries matches the provided expected count
 
     Args:
         tator_api: Interface to tator
         project: Unique identifier of test project
@@ -182,47 +182,46 @@
     """
 
     MAX_RETRIES = 10
     num_retries = 0
     matched_analysis_count = False
 
     while True:
-
-        analysis_list = tator_api.get_analysis_list(project=project)
+        media = tator_api.get_media_list(project, media_id=media_ids)
         analysis_count = 0
         log_msg = f'num_retries: {num_retries}'
         print(log_msg)
-        for analysis in analysis_list:
-            if 'test_media_id' in analysis.data_query:
-                print(str(analysis))
-                analysis_count += 1
+        all_good=True
+        for m in media:
+          if m.attributes.get('test_int',0) != expected_count:
+            all_good = False
 
-        matched_analysis_count = analysis_count == expected_analysis_count
-        if matched_analysis_count:
-            break
+        if all_good:
+          break
 
         num_retries += 1
         if num_retries < MAX_RETRIES:
             time.sleep(10)
         else:
             log_msg = f'Number of detected analysis entries from workflow: {analysis_count}'
             logger.error(log_msg)
             logger.error('Reached maximum retries')
             break
 
-    assert matched_analysis_count
+    for m in media:
+      assert m.attributes.get('test_int',0) == expected_count
 
 def test_algorithm_launch(
         host: str,
         token: str,
         project: int,
         algorithm_name: str,
         image_type: int,
         image_set: str) -> None:
-    """ Unit tests the LaunchAlgorithm endpoint
+    """ Unit tests the Jobs POST method
 
     Performs the following unit tests:
     - Add a bunch of images, register the workflow that writes entries to the Analysis model
       and check to see if the number of entries match in a given amount of processing time.
     - Provide a specific media list, launch the workflow, 
       and perform the analysis entry counting as above
     - Provide a blank media list and ensure no workflow was launched (using the uid)
@@ -233,26 +232,25 @@
         host: Project URL
         token: User token used for connecting to the host
         project: Unique identifier of test project
         algorithm_name: Unique algorithm name of a registered workflow to be used by this test
         image_type: Unique identifier of the media type related to images saved to this project
         image_set: List of paths to temporary images that can be uploaded to tator
     """
-
     tator_api = tator.get_api(host=host, token=token)
     number_of_media = 10
 
     # Get the media that's already in the project (perhaps added from other tests)
     medias = tator_api.get_media_list(project=project)
     number_of_media += len(medias)
 
     # Add some media to the project
     paths = glob.glob(image_set + '/**/*.jpg', recursive=True)
     paths = [os.path.join(image_set, path) for path in paths]
-    paths = paths[:number_of_media]
+    paths = paths[:10]
 
     for image_file in paths:
         for progress, response in tator.util.upload_media(tator_api, image_type, image_file):
             log_msg = f"Upload image {image_file} - progress: {progress}%"
             logger.info(log_msg)
 
     num_retries = 0
@@ -264,56 +262,27 @@
 
         num_retries += 1
         if num_retries >= max_retries:
             break
         time.sleep(0.5)
 
     assert len(medias) == number_of_media
-
-    # Now, launch the algorithm using all the media in the project
-    spec = tator.models.AlgorithmLaunchSpec(algorithm_name=algorithm_name)
-    response = tator_api.algorithm_launch(project=project, algorithm_launch_spec=spec)
-    assert len(response.uid) == 1
-
-    # The algorithm workflow doesn't do much but saves an analysis object for each media ID
-    # that was passed along to it in the data query field. So we assume the workflow
-    # will be done soon (tm) and these analysis entries should pop up. Count them up and
-    # once we have one entry per media, we're good to go.
-    expected_analysis_count = number_of_media
-    _assert_algorithm_workflow_results(
-        tator_api=tator_api,
-        project=project,
-        expected_analysis_count=expected_analysis_count)
+    all_ids = [m.id for m in medias]
 
     # Now, launch the algorithm again with an arbitrary set of media and test the results
     media_ids = [medias[0].id, medias[1].id]
     print(f"Providing following media list: {media_ids}")
-    expected_analysis_count += len(media_ids)
-    spec = tator.models.AlgorithmLaunchSpec(algorithm_name=algorithm_name, media_ids=media_ids)
-    response = tator_api.algorithm_launch(project=project, algorithm_launch_spec=spec)
-    assert len(response.uid) == 1
+    spec = tator.models.JobSpec(algorithm_name=algorithm_name, media_ids=media_ids)
+    response = tator_api.create_job_list(project=project, job_spec=spec)
+    assert len(response.id) == 1
     _assert_algorithm_workflow_results(
         tator_api=tator_api,
         project=project,
-        expected_analysis_count=expected_analysis_count)
+        expected_count=1,
+        media_ids=media_ids)
 
     # Next, launch the algorithm again with a blank set of media ids and test the results
     # - This shouldn't launch the argo workflow
     media_ids = []
-    expected_analysis_count += len(media_ids)
-    spec = tator.models.AlgorithmLaunchSpec(algorithm_name=algorithm_name, media_ids=media_ids)
-    response = tator_api.algorithm_launch(project=project, algorithm_launch_spec=spec)
-    assert len(response.uid) == 0
-
-    # Use the media query to get media of a specific name
-    target_name = os.path.basename(paths[0])
-    medias = tator_api.get_media_list(project=project, name=target_name)
-    print(f"Providing following media name query: {target_name} (Medias matching this name: {len(medias)})")
-
-    spec = tator.models.AlgorithmLaunchSpec(algorithm_name=algorithm_name, media_query=f"?name={target_name}")
-    response = tator_api.algorithm_launch(project=project, algorithm_launch_spec=spec)
-    assert len(response.uid) == 1
-    expected_analysis_count += len(medias)
-    _assert_algorithm_workflow_results(
-        tator_api=tator_api,
-        project=project,
-        expected_analysis_count=expected_analysis_count)
+    spec = tator.models.JobSpec(algorithm_name=algorithm_name, media_ids=media_ids)
+    response = tator_api.create_job_list(project=project, job_spec=spec)
+    assert len(response.id) == 0
```

### Comparing `tator-0.9.6/test/test_attribute_addition.py` & `tator-1.0.0/test/test_attribute_type_addition.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,45 +16,46 @@
         "test_bool": random.choice([False, True]),
         "test_int": random.randint(-1000, 1000),
         "test_float": random.uniform(-1000.0, 1000.0),
         "test_enum": random.choice(["a", "b", "c"]),
         "test_string": str(uuid4()),
         "test_datetime": datetime.now().isoformat(),
         "test_geopos": [random.uniform(-180.0, 180.0), random.uniform(-90.0, 90.0)],
+        'test_float_array': [random.uniform(-1.0, 1.0) for _ in range(3)],
     }
     out = {
         "x": x,
         "y": y,
         "width": w,
         "height": h,
         "project": project,
         "type": box_type,
         "media_id": video_obj.id,
         "frame": random.randint(0, video_obj.num_frames - 1),
+        "attributes": attributes
     }
-    if post:
-        out = {**out, **attributes}
-    else:
-        out["attributes"] = attributes
-    return out
+
+    return {**out}
 
 
 def add_attribute_helper(tator_api, type_getter, type_id, dtype):
     new_attr_name = f"New {dtype} {uuid4()}"
     entity_type = type_getter(type_id)
 
     # Make sure the new attribute does not exist already
     assert all(attr.name != new_attr_name for attr in entity_type.attribute_types)
     addition = {
         "entity_type": f"{type(entity_type).__name__}",
         "addition": {"name": new_attr_name, "dtype": dtype},
     }
     if dtype == "enum":
         addition["addition"]["choices"] = ["a", "b", "c"]
-    tator_api.add_attribute(id=type_id, attribute_type_spec=addition)
+    if dtype == "float_array":
+        addition["addition"]["size"] = 3
+    tator_api.create_attribute_type(id=type_id, attribute_type_spec=addition)
     entity_type = type_getter(type_id)
 
     # Check for added attribute
     assert any(attr.name == new_attr_name for attr in entity_type.attribute_types)
 
 
 def add_invalid_attribute_helper(tator_api, type_getter, type_id):
@@ -66,19 +67,19 @@
     addition = {
         "entity_type": f"{type(entity_type).__name__}",
         "addition": {"name": new_attr_name, "dtype": "unknown"},
     }
 
     # Adding an attribute with an invalid `dtype` should raise an exception
     with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException) as excinfo:
-        tator_api.add_attribute(id=type_id, attribute_type_spec=addition)
+        tator_api.create_attribute_type(id=type_id, attribute_type_spec=addition)
 
     # Check the exeption message for expected content
     assert (
-        "ValidationError: \\\"'unknown' is not one of ['bool', 'int', 'float', 'enum', 'string', 'datetime', 'geopos']\\\""
+        "ValidationError: \\\"'unknown' is not one of ['bool', 'int', 'float', 'enum', 'string', 'datetime', 'geopos', 'float_array']\\\""
         in str(excinfo.value)
     )
 
 
 def test_box_type_add_invalid_attribute(host, token, project, attribute_box_type):
     tator_api = tator.get_api(host, token)
     add_invalid_attribute_helper(tator_api, tator_api.get_localization_type, attribute_box_type)
@@ -90,15 +91,15 @@
 
 
 def test_video_type_add_invalid_attribute(host, token, project, attribute_video_type):
     tator_api = tator.get_api(host, token)
     add_invalid_attribute_helper(tator_api, tator_api.get_media_type, attribute_video_type)
 
 
-dtypes = ["int", "bool", "float", "string", "enum", "datetime", "geopos"]
+dtypes = ["int", "bool", "float", "string", "enum", "datetime", "geopos", "float_array"]
 
 
 @pytest.mark.parametrize("dtype", dtypes)
 def test_box_type_add_attribute(host, token, project, attribute_box_type, dtype):
     tator_api = tator.get_api(host, token)
     add_attribute_helper(tator_api, tator_api.get_localization_type, attribute_box_type, dtype)
 
@@ -126,15 +127,15 @@
     addition = {
         "entity_type": "MediaType",
         "addition": {"name": new_attr_name, "dtype": dtype},
     }
 
     # Adding an enum attribute without a `choices` field should raise an exception
     with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException) as excinfo:
-        tator_api.add_attribute(id=attribute_video_type, attribute_type_spec=addition)
+        tator_api.create_attribute_type(id=attribute_video_type, attribute_type_spec=addition)
 
     # Check the exeption message for expected content
     assert "ValueError: enum attribute type definition missing 'choices' field" in str(
         excinfo.value
     )
 
 
@@ -145,59 +146,26 @@
     # Make sure the new attribute does not exist already
     entity_type = tator_api.get_localization_type(line_type)
     assert all(attr.name != new_attr_name for attr in entity_type.attribute_types)
     addition = {
         "entity_type": "LocalizationType",
         "addition": {"name": new_attr_name, "dtype": "int"},
     }
-    tator_api.add_attribute(id=line_type, attribute_type_spec=addition)
+    tator_api.create_attribute_type(id=line_type, attribute_type_spec=addition)
     entity_type = tator_api.get_localization_type(line_type)
 
     # Check for added attribute
     assert any(attr.name == new_attr_name for attr in entity_type.attribute_types)
 
     # Adding the same attribute a second time should raise an exception
     with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException) as excinfo:
-        tator_api.add_attribute(id=line_type, attribute_type_spec=addition)
+        tator_api.create_attribute_type(id=line_type, attribute_type_spec=addition)
 
     # Check the exeption message for expected content
-    assert "but one with that name already exists" in str(excinfo.value)
-
-
-def test_add_same_attribute_with_different_dtypes(
-    host, token, project, line_type, attribute_box_type
-):
-    tator_api = tator.get_api(host, token)
-    new_attr_name = f"New attribute {uuid4()}"
-
-    # Make sure the new attribute does not exist already
-    entity_type = tator_api.get_localization_type(line_type)
-    assert all(attr.name != new_attr_name for attr in entity_type.attribute_types)
-    entity_type = tator_api.get_localization_type(attribute_box_type)
-    assert all(attr.name != new_attr_name for attr in entity_type.attribute_types)
-    addition = {
-        "entity_type": "LocalizationType",
-        "addition": {"name": new_attr_name, "dtype": "int"},
-    }
-    tator_api.add_attribute(id=line_type, attribute_type_spec=addition)
-    entity_type = tator_api.get_localization_type(line_type)
-
-    # Check for added attribute
-    assert any(attr.name == new_attr_name for attr in entity_type.attribute_types)
-
-    # Adding the same attribute with a different `dtype` should raise an exception
-    addition["addition"]["dtype"] = "string"
-    with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException) as excinfo:
-        tator_api.add_attribute(id=attribute_box_type, attribute_type_spec=addition)
-
-    # Check the exeption message for expected content
-    assert (
-        "but another entity type has already defined this attribute name with a different dtype"
-        in str(excinfo.value)
-    )
+    assert "is already an attribute." in str(excinfo.value)
 
 
 # @pytest.mark.skip(reason="Disabled")
 @pytest.mark.parametrize("dtype", ["string", "bool"])
 def test_box_type_attribute_addition_es(
     host, token, project, attribute_video, attribute_box_type, dtype
 ):
@@ -208,15 +176,15 @@
     boxes = [
         random_localization(project, attribute_box_type, video_obj, post=True)
         for _ in range(num_localizations)
     ]
     box_ids = [
         box_id
         for response in tator.util.chunked_create(
-            tator_api.create_localization_list, project, localization_spec=boxes
+            tator_api.create_localization_list, project, body=boxes
         )
         for box_id in response.id
     ]
 
     assert len(box_ids) == len(boxes)
 
     # ES can be slow at indexing so wait for a bit.
@@ -231,29 +199,28 @@
         new_attr_name = f"New bool {uuid4()}"
     entity_type = tator_api.get_localization_type(attribute_box_type)
     assert all(attr.name != new_attr_name for attr in entity_type.attribute_types)
     addition = {
         "entity_type": "LocalizationType",
         "addition": {"name": new_attr_name, "dtype": dtype, "default": value},
     }
-    tator_api.add_attribute(id=attribute_box_type, attribute_type_spec=addition)
+    tator_api.create_attribute_type(id=attribute_box_type, attribute_type_spec=addition)
 
     entity_type = tator_api.get_localization_type(attribute_box_type)
 
     # Check for added attribute
     assert any(attr.name == new_attr_name for attr in entity_type.attribute_types)
 
     # ES can be slow at indexing so wait for a bit.
     sleep(2)
 
     # Check for default value on existing instances
     params = {
         "type": attribute_box_type,
-        "attribute": [f"{new_attr_name}::{str(value).lower()}"],
-        "force_es": 1,
+        "attribute": [f"{new_attr_name}::{str(value).lower()}"]
     }
     boxes = tator_api.get_localization_list(project, **params)
 
     assert len(box_ids) == len(boxes)
 
     for box in boxes:
         assert box.attributes[new_attr_name] == value
```

### Comparing `tator-0.9.6/test/test_attribute_deletion.py` & `tator-1.0.0/test/test_attribute_type_deletion.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
     addition = {
         "entity_type": f"{type(entity_type).__name__}",
         "addition": {"name": new_attr_name, "dtype": dtype},
     }
     if dtype == "enum":
         addition["addition"]["choices"] = ["a", "b", "c"]
-    tator_api.add_attribute(id=type_id, attribute_type_spec=addition)
+    tator_api.create_attribute_type(id=type_id, attribute_type_spec=addition)
     entity_type = type_getter(type_id)
 
     # Check for added attribute
     assert any(attr.name == new_attr_name for attr in entity_type.attribute_types)
 
     # Delete attribute
     deletion = {
         "entity_type": f"{type(entity_type).__name__}",
-        "attribute_to_delete": new_attr_name,
+        "name": new_attr_name,
     }
-    tator_api.delete_attribute(id=type_id, attribute_type_delete=deletion)
+    tator_api.delete_attribute_type(id=type_id, attribute_type_delete=deletion)
     entity_type = type_getter(type_id)
 
     # Check that the attribute is gone
     assert all(attr.name != new_attr_name for attr in entity_type.attribute_types)
 
 
 def delete_invalid_attribute_helper(tator_api, type_getter, type_id):
@@ -38,18 +38,18 @@
 
     # Check that the attribute does not exist
     assert all(attr.name != new_attr_name for attr in entity_type.attribute_types)
 
     # Delete attribute
     deletion = {
         "entity_type": f"{type(entity_type).__name__}",
-        "attribute_to_delete": new_attr_name,
+        "name": new_attr_name,
     }
     with pytest.raises(tator.openapi.tator_openapi.exceptions.ApiException) as excinfo:
-        tator_api.delete_attribute(id=type_id, attribute_type_delete=deletion)
+        tator_api.delete_attribute_type(id=type_id, attribute_type_delete=deletion)
 
     # Check the exeption message for expected content
     assert "Could not find attribute name" in str(excinfo.value)
 
 
 def test_box_type_delete_invalid_attribute(host, token, project, attribute_box_type):
     tator_api = tator.get_api(host, token)
```

### Comparing `tator-0.9.6/test/test_clone_leaf_type.py` & `tator-1.0.0/test/test_clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_clone_localization_type.py` & `tator-1.0.0/test/test_clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_clone_media.py` & `tator-1.0.0/test/test_clone_media.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_clone_media_type.py` & `tator-1.0.0/test/test_clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_clone_membership.py` & `tator-1.0.0/test/test_clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_clone_section.py` & `tator-1.0.0/test/test_clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_clone_state_type.py` & `tator-1.0.0/test/test_clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_clone_version.py` & `tator-1.0.0/test/test_clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_download_media.py` & `tator-1.0.0/test/test_download_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         with tempfile.TemporaryDirectory() as td:
             image_path = os.path.join(td, image_obj.name)
             for progress in tator.download_media(
                     tator_api,
                     image_obj,
                     image_path,
                     quality=image_file.resolution[0],
-                    media_type=None):
+                    media_type=None,
+                    codec_or_mime=image_file.mime):
                 print(f"Media download progress: {progress}%")
             assert os.path.exists(image_path)
             assert os.stat(image_path).st_size == image_file.size
 
 def test_download_video(host, token, video):
     tator_api = tator.get_api(host, token)
     video_obj = tator_api.get_media(video)
```

### Comparing `tator-0.9.6/test/test_extract.py` & `tator-1.0.0/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_getframe.py` & `tator-1.0.0/test/test_getframe.py`

 * *Files identical despite different names*

### Comparing `tator-0.9.6/test/test_job_cancel.py` & `tator-1.0.0/test/test_job_cancel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import time
 import tempfile
 from textwrap import dedent
 
 import tator
 import uuid
+import pytest
 
+@pytest.mark.flaky(reruns=3)
 def test_algorithm_cancel(host, token, project, image):
     ALGORITHM_NAME = f'Sleepy time {uuid.uuid1()}'
 
     # Register an algorithm that sleeps.
     workflow_spec = dedent("""\
 apiVersion: argoproj.io/v1alpha1
 kind: Workflow
@@ -43,45 +45,47 @@
         files_per_job=1,
         description='sleeps for testing purposes',
         cluster_id=None)
     os.remove(manifest_file.name)
 
     # Launch some workflows.
     tator_api = tator.get_api(host=host, token=token)
-    spec = tator.models.AlgorithmLaunchSpec(
+    spec = tator.models.JobSpec(
         algorithm_name=ALGORITHM_NAME,
         media_ids=[image])
-    responses = [tator_api.algorithm_launch(project=project,
-                                            algorithm_launch_spec=spec)
+    responses = [tator_api.create_job_list(project=project,
+                                            job_spec=spec)
                  for _ in range(10)]
 
     # Cancel by UID.
-    uid = responses[0].uid[0]
+    uid = responses[0].id[0]
     job = tator_api.get_job(uid)
     assert isinstance(job, tator.models.Job)
     print(f"Cancelling job with uid {uid}...")
     response = tator_api.delete_job(uid)
     try:
         found = True
         response = tator_api.get_job(uid)
     except tator.exceptions.ApiException as exc:
         found = False
         assert exc.status == 404
     assert found == False
 
     # Cancel by GID.
-    gid = responses[1].gid
+    job_detail = tator_api.get_job(responses[1].id[0])
+    gid = job_detail.gid
     jobs = tator_api.get_job_list(project, gid=gid)
     assert isinstance(jobs[0], tator.models.Job)
     print(f"Cancelling job with gid {gid}...")
     tator_api.delete_job_list(project, gid=gid)
     jobs = tator_api.get_job_list(project, gid=gid)
     assert len(jobs) == 0
 
     # Cancel all jobs in project.
+    time.sleep(5.0)
     jobs = tator_api.get_job_list(project)
     assert len(jobs) >= 8
     print("Cancelling all jobs in project...")
     tator_api.delete_job_list(project)
     jobs = tator_api.get_job_list(project)
     assert len(jobs) == 0
```

### Comparing `tator-0.9.6/test/test_leaf.py` & `tator-1.0.0/test/test_leaf.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,62 +11,65 @@
         'test_bool': random.choice([False, True]),
         'test_int': random.randint(-1000, 1000),
         'test_float': random.uniform(-1000.0, 1000.0),
         'test_enum': random.choice(['a', 'b', 'c']),
         'test_string': str(uuid.uuid1()),
         'test_datetime': datetime.datetime.now().isoformat(),
         'test_geopos': [random.uniform(-180.0, 180.0), random.uniform(-90.0, 90.0)],
+        'test_float_array': [random.uniform(-1.0, 1.0) for _ in range(3)],
     }
     name = "".join(random.choice(string.ascii_letters) for _ in range(10))
     out = {
         'project': project,
         'type': leaf_type,
         'name': name,
+        'attributes': attributes
     }
     if parent_obj:
         out['parent'] = parent_obj.id
-    if post:
-        out = {**out, **attributes}
-    else:
-        out['attributes'] = attributes
-    return out
+    return {**out}
 
 def test_leaf_crud(host, token, project, clone_project, leaf_type, clone_leaf_type):
     tator_api = tator.get_api(host, token)
 
     # Create root leaf.
     root_spec = random_leaf(project, leaf_type, None, True)
-    response = tator_api.create_leaf_list(project=project, leaf_spec=[root_spec])
+    response = tator_api.create_leaf_list(project=project, body=root_spec)
     assert(isinstance(response, tator.models.CreateListResponse))
     prev_ids = response.id
 
     # Create three additional layers.
     for _ in range(3):
         new_ids = []
         for parent_id in prev_ids:
             parent_obj = tator_api.get_leaf(parent_id)
             leaf_spec = [random_leaf(project, leaf_type, parent_obj, True)
                          for _ in range(3)] # 3 children per parent
-            response = tator_api.create_leaf_list(project=project, leaf_spec=leaf_spec)
+            response = tator_api.create_leaf_list(project=project, body=leaf_spec)
             assert(isinstance(response, tator.models.CreateListResponse))
             new_ids += response.id
         prev_ids = list(new_ids)
 
     # Clone the layers.
     parent_mapping = {}
     for depth in range(4):
         leaves = tator_api.get_leaf_list(project=project, depth=depth)
         # Check leaf retrieval by ID.
-        leaves_by_id = tator_api.get_leaf_list_by_id(project, [leaf.id for leaf in leaves])
+        leaves_by_id = tator_api.get_leaf_list_by_id(project, {'ids': [leaf.id for leaf in leaves]})
+        count = tator_api.get_leaf_count_by_id(project, {'ids': [leaf.id for leaf in leaves]})
+        assert(len(leaves_by_id) == count)
+        assert len(leaves) == len(leaves_by_id)
         for leaf, leaf_by_id in zip(leaves, leaves_by_id):
             assert_close_enough(leaf, leaf_by_id)
+        print(f"Cloning Depth {depth}: {leaves}")
         generator = tator.util.clone_leaf_list(tator_api, {'project': project, 'depth': depth},
                                                clone_project, parent_mapping,
                                                {leaf_type: leaf_type})
         created_ids = []
+        num_created = 0
         for num_created, num_total, response, id_map in generator:
             print(f"Created {num_created} of {num_total} leafs...")
             created_ids += response.id
         parent_mapping = {**parent_mapping,
                           **{src.id: dst for src, dst in zip(leaves, created_ids)}}
         print(f"Finished creating {num_created} leafs!")
     for src_id in parent_mapping:
```

### Comparing `tator-0.9.6/test/test_local_transcode.py` & `tator-1.0.0/test/test_local_transcode.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,9 +28,17 @@
         subprocess.run(cmd, check=True)
     except subprocess.CalledProcessError as cpe:
         failed = True
     assert(failed)
     time.sleep(2)
     # Make sure media file is gone.
     api = tator.get_api(host, token)
-    medias = api.get_media_list(project, attribute=['tator_user_sections::Bad transcodes'])
+    sections = api.get_section_list(project)
+    section_obj = [s for s in sections if s.name == 'Bad transcodes'][0]
+
+    medias = api.get_media_list(project, attribute=[f'tator_user_sections::{section_obj.tator_user_sections}'])
+    print(medias)
+    assert(len(medias) == 0)
+
+    medias = api.get_media_list(project, section=section_obj.id)
+    print(medias)
     assert(len(medias) == 0)
```

### Comparing `tator-0.9.6/test/test_localization.py` & `tator-1.0.0/test/test_localization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from pprint import pformat
 import datetime
 import random
+from time import sleep
 import uuid
+from collections import Counter
 
 import tator
 from ._common import assert_close_enough
 
 def random_localization(project, box_type, video_obj, post=False):
     x = random.uniform(0.0, 1.0)
     y = random.uniform(0.0, 1.0)
@@ -14,161 +17,211 @@
         'test_bool': random.choice([False, True]),
         'test_int': random.randint(-1000, 1000),
         'test_float': random.uniform(-1000.0, 1000.0),
         'test_enum': random.choice(['a', 'b', 'c']),
         'test_string': str(uuid.uuid1()),
         'test_datetime': datetime.datetime.now().isoformat(),
         'test_geopos': [random.uniform(-180.0, 180.0), random.uniform(-90.0, 90.0)],
+        'test_float_array': [random.uniform(-1.0, 1.0) for _ in range(3)],
     }
     out = {
         'x': x,
         'y': y,
         'width': w,
         'height': h,
         'project': project,
         'type': box_type,
         'media_id': video_obj.id,
         'frame': random.randint(0, video_obj.num_frames - 1),
+        'attributes': attributes
     }
-    if post:
-        out = {**out, **attributes}
-    else:
-        out['attributes'] = attributes
-    return out
 
-def comparison_query(tator_api, project, exclude):
+    return {**out}
+
+def comparison_query(tator_api, project, box_ids, exclude):
     """ Runs a random query and compares results with ES enabled and disabled.
     """
     bool_value = random.choice([True, False])
     int_lower = random.randint(-1000, 0)
     int_upper = random.randint(0, 1000)
     float_lower = random.uniform(-1000.0, 0.0)
     float_upper = random.uniform(0.0, 1000.0)
     enum_value = random.choice(['a', 'b', 'c'])
+    localization_id_query = {"ids": box_ids}
     attribute_filter = [f"test_bool::{'true' if bool_value else 'false'}", f"test_enum::{enum_value}"]
     attribute_lte_filter = [f"test_int::{int_upper}"]
     attribute_gte_filter = [f"test_int::{int_lower}"]
     attribute_lt_filter = [f"test_float::{float_upper}"]
     attribute_gt_filter = [f"test_float::{float_lower}"]
+    print("Starting PSQL query...")
     t0 = datetime.datetime.now()
-    from_psql = tator_api.get_localization_list(project,
-                                                attribute=attribute_filter,
-                                                attribute_lte=attribute_lte_filter,
-                                                attribute_gte=attribute_gte_filter,
-                                                attribute_lt=attribute_lt_filter,
-                                                attribute_gt=attribute_gt_filter)
+    from_psql = tator_api.get_localization_list_by_id(
+        project,
+        localization_id_query=localization_id_query,
+        attribute=attribute_filter,
+        attribute_lte=attribute_lte_filter,
+        attribute_gte=attribute_gte_filter,
+        attribute_lt=attribute_lt_filter,
+        attribute_gt=attribute_gt_filter,
+    )
     psql_time = datetime.datetime.now() - t0
+    print("Starting ES query...")
     t0 = datetime.datetime.now()
-    from_es = tator_api.get_localization_list(project,
-                                              attribute=attribute_filter,
-                                              attribute_lte=attribute_lte_filter,
-                                              attribute_gte=attribute_gte_filter,
-                                              attribute_lt=attribute_lt_filter,
-                                              attribute_gt=attribute_gt_filter,
-                                              force_es=1)
+    from_es = tator_api.get_localization_list_by_id(
+        project,
+        localization_id_query=localization_id_query,
+        attribute=attribute_filter,
+        attribute_lte=attribute_lte_filter,
+        attribute_gte=attribute_gte_filter,
+        attribute_lt=attribute_lt_filter,
+        attribute_gt=attribute_gt_filter
+    )
     es_time = datetime.datetime.now() - t0
+
+    print("Checking PSQL and ES ids...")
+    psql_ids = [ele.id for ele in from_psql]
+    es_ids = [ele.id for ele in from_es]
+    assert(Counter(psql_ids) == Counter(es_ids))
+
+    print("Checking PSQL and ES values...")
+    assert len(from_psql) == len(from_es)
     for psql, es in zip(from_psql, from_es):
         assert_close_enough(psql, es, exclude)
         assert(psql.attributes['test_bool'] == bool_value)
         assert(psql.attributes['test_int'] <= int_upper)
         assert(psql.attributes['test_int'] >= int_lower)
         assert(psql.attributes['test_float'] < float_upper)
         assert(psql.attributes['test_float'] > float_lower)
         assert(psql.attributes['test_enum'] == enum_value)
     return psql_time, es_time
 
-def test_localization_crud(host, token, project, video_type, video, box_type):
+def test_localization_crud(host, token, project, video_type, video_temp, box_type):
     tator_api = tator.get_api(host, token)
-    video_obj = tator_api.get_media(video)
+    video_obj = tator_api.get_media(video_temp)
 
     # These fields will not be checked for object equivalence after patch.
-    exclude = ['project', 'type', 'media_id', 'id', 'meta', 'user']
+    exclude = ['project', 'type', 'media_id', 'id', 'type', 'user', 'ids']
+    mapping = {'new_version': 'version'}
 
     # Test bulk create.
     num_localizations = random.randint(2000, 10000)
+    existing = len(tator_api.get_localization_list(project,type=box_type))
     boxes = [
         random_localization(project, box_type, video_obj, post=True)
         for _ in range(num_localizations)
     ]
     box_ids = []
-    for response in tator.util.chunked_create(tator_api.create_localization_list,
-                                         project, localization_spec=boxes):
+    for response in tator.util.chunked_create(
+            tator_api.create_localization_list, project, body=boxes
+    ):
         box_ids += response.id
     assert len(box_ids) == len(boxes)
     print(f"Created {len(box_ids)} boxes!")
 
     # Verify list is the right length
-    response = tator_api.get_localization_list(project,type=box_type)
-    assert len(response) == num_localizations
+    response = tator_api.get_localization_list(project,type=box_type, media_id=[video_temp])
+    assert len(response) == num_localizations + existing
+
+    # Test media retrieval by localization ID.
+    response = tator_api.get_media_list_by_id(project, {'localization_ids': box_ids})
+    assert len(response) == 1
+    assert response[0].id == video_temp
+
+    # Test box retrieval by media ID.
+    response = tator_api.get_localization_list_by_id(project, {'media_ids': [video_temp]})
+    assert(len(response) == len(box_ids))
 
     # Test single create.
     box = random_localization(project, box_type, video_obj, post=True)
-    response = tator_api.create_localization_list(project, localization_spec=[box])
+    response = tator_api.create_localization_list(project, body=box)
     assert isinstance(response, tator.models.CreateListResponse)
     box_id = response.id[0]
 
     # Patch single box.
     patch = random_localization(project, box_type, video_obj)
     response = tator_api.update_localization(box_id, localization_update=patch)
     assert isinstance(response, tator.models.MessageResponse)
     print(response.message)
 
     # Get single box.
     updated_box = tator_api.get_localization(box_id)
     assert_close_enough(patch, updated_box, exclude)
 
     # Get box by ID.
-    box_by_id = tator_api.get_localization_list_by_id(project, [box_id])[0]
+    box_by_id = tator_api.get_localization_list_by_id(project, {'ids': [box_id]})
+    assert(len(box_by_id) == 1)
+    box_by_id = box_by_id[0]
     assert_close_enough(updated_box, box_by_id, exclude)
 
     # Delete single box.
     response = tator_api.delete_localization(box_id)
     assert isinstance(response, tator.models.MessageResponse)
     print(response.message)
 
-    params = {'media_id': [video], 'type': box_type}
-    assert(tator_api.get_localization_count(project, **params) == len(boxes))
+    params = {'media_id': [video_temp], 'type': box_type}
+    assert(tator_api.get_localization_count(project, **params) == len(boxes) + existing)
 
     # Bulk update box attributes.
+    response = tator_api.create_version(
+        project,
+        version_spec={
+            "name": "Test Version",
+            "description": "A version for testing",
+        },
+    )
+    new_version = response.id
     bulk_patch = random_localization(project, box_type, video_obj)
-    bulk_patch = {'attributes': bulk_patch['attributes']}
+    bulk_patch = {"attributes": bulk_patch["attributes"], "new_version": new_version}
+    response = tator_api.update_localization_list(project, **params,
+                                                  localization_bulk_update=bulk_patch)
+    assert isinstance(response, tator.models.MessageResponse)
+    print(response.message)
+
+    # Bulk update specified boxes by ID.
+    id_bulk_patch = random_localization(project, box_type, video_obj)
+    update_ids = random.choices(box_ids, k=100)
+    id_bulk_patch = {
+        "attributes": id_bulk_patch["attributes"],
+        "ids": update_ids,
+        "new_version": new_version,
+    }
     response = tator_api.update_localization_list(project, **params,
-                                                  attribute_bulk_update=bulk_patch)
+                                                  localization_bulk_update=id_bulk_patch)
     assert isinstance(response, tator.models.MessageResponse)
     print(response.message)
 
     # Verify all boxes have been updated.
     boxes = tator_api.get_localization_list(project, **params)
     dataframe = tator.util.to_dataframe(boxes)
     assert(len(boxes)==len(dataframe))
     for box in boxes:
-        assert_close_enough(bulk_patch, box, exclude)
-
-    # Do random queries using psql and elasticsearch and compare results.
-    es_time = datetime.timedelta(seconds=0)
-    psql_time = datetime.timedelta(seconds=0)
-    NUM_QUERIES = 10
-    for _ in range(NUM_QUERIES):
-        psql, es = comparison_query(tator_api, project, exclude)
-        psql_time += psql
-        es_time += es
-    print(f"Over {NUM_QUERIES} random attribute queries:")
-    print(f"  Avg PSQL time: {psql_time / NUM_QUERIES}")
-    print(f"  Avg ES time: {es_time / NUM_QUERIES}")
+        if box.id in update_ids:
+            assert_close_enough(id_bulk_patch, box, exclude, mapping)
+        else:
+            assert_close_enough(bulk_patch, box, exclude, mapping)
 
     # Clone boxes to same media.
     version_mapping = {version.id: version.id for version in tator_api.get_version_list(project)}
     generator = tator.util.clone_localization_list(tator_api, {**params, 'project': project},
-                                                   project, version_mapping, {video:video},
+                                                   project, version_mapping, {video_temp:video_temp},
                                                    {box_type: box_type}, tator_api)
     for num_created, num_total, response, id_map in generator:
         print(f"Created {num_created} of {num_total} localizations...")
     print(f"Finished creating {num_created} localizations!")
-    assert(tator_api.get_localization_count(project, **params) == 2 * len(boxes))
+    assert(tator_api.get_localization_count(project, **params) == 2 * (len(boxes)+existing))
 
     # Delete all boxes.
     response = tator_api.delete_localization_list(project, **params)
     assert isinstance(response, tator.models.MessageResponse)
 
     # Verify all boxes are gone.
     boxes = tator_api.get_localization_list(project, **params)
     assert boxes == []
+
+    boxes = tator_api.get_localization_list(project, **params, show_deleted=1)
+    assert boxes != []
+
+    response = tator_api.delete_localization_list(project, **params, show_deleted=1, merge=0, localization_bulk_delete={'prune':1})
+    assert isinstance(response, tator.models.MessageResponse)
+
+    # Clean up test version
+    tator_api.delete_version(new_version)
```

### Comparing `tator-0.9.6/test/test_localization_graphic.py` & `tator-1.0.0/test/test_localization_graphic.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         'test_bool': random.choice([False, True]),
         'test_int': random.randint(-1000, 1000),
         'test_float': random.uniform(-1000.0, 1000.0),
         'test_enum': random.choice(['a', 'b', 'c']),
         'test_string': str(uuid.uuid1()),
         'test_datetime': datetime.datetime.now().isoformat(),
         'test_geopos': [random.uniform(-180.0, 180.0), random.uniform(-90.0, 90.0)],
+        'test_float_array': [random.uniform(-1.0, 1.0) for _ in range(3)],
     }
 
     datum = {**datum, **attributes}
 
     return datum
 
 def _generate_truth_info(
@@ -218,18 +219,19 @@
         'test_bool': random.choice([False, True]),
         'test_int': random.randint(-1000, 1000),
         'test_float': random.uniform(-1000.0, 1000.0),
         'test_enum': random.choice(['a', 'b', 'c']),
         'test_string': str(uuid.uuid1()),
         'test_datetime': datetime.datetime.now().isoformat(),
         'test_geopos': [random.uniform(-180.0, 180.0), random.uniform(-90.0, 90.0)],
+        'test_float_array': [random.uniform(-1.0, 1.0) for _ in range(3)],
     }
 
-    datum = {**datum, **attributes}
-    response = tator_api.create_localization_list(project, localization_spec=[datum])
+    datum = {**datum, 'attributes': {**attributes}}
+    response = tator_api.create_localization_list(project, body=datum)
 
     # Generate the truth information for unit testing
     truth_graphic_info = {}
     for localization_id in response.id:
         truth_graphic_info[localization_id] = _generate_truth_info(
             localization_datum=datum,
             media_width=media.width,
@@ -313,15 +315,15 @@
                 media_id=media_id,
                 dtype=LOCALIZATION_TYPES_INT_TO_DTYPE[localization_type],
                 type_id=localization_type,
                 frame=FRAME_NUMBER)
 
             localization_list.append(localization)
 
-    response = tator_api.create_localization_list(project, localization_spec=localization_list)
+    response = tator_api.create_localization_list(project, body=localization_list)
 
     # Generate the truth information for unit testing
     truth_graphic_info = {}
     for localization_id, localization in zip(response.id, localization_list):
         truth_graphic_info[localization_id] = _generate_truth_info(
             localization_datum=localization,
             media_width=media.width,
```

### Comparing `tator-0.9.6/test/test_media.py` & `tator-1.0.0/test/test_get_clip.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,17 @@
-import tempfile
 import os
+import tempfile
 
 import tator
 
-from._common import assert_vector_equal
-
-def test_get_file(host, token, project, video):
+def test_get_clip(host, token, project, video):
     tator_api = tator.get_api(host, token)
     video_obj = tator_api.get_media(video)
 
-    with tempfile.TemporaryDirectory() as temp_dir:
-        outpath = os.path.join(temp_dir, "video.mp4")
-        for progress in tator.download_media(tator_api, video_obj, outpath):
-            print(f"Video download progress: {progress}%")
-        assert(os.path.exists(outpath))
+    frame_ranges = ['0:100']
+    clip = tator_api.get_clip(video, frame_ranges=frame_ranges)
+    with tempfile.TemporaryDirectory() as td:
+        video_path = os.path.join(td, 'video_clip_test.mp4')
+        for progress in tator.util.download_temporary_file(tator_api, clip.file, video_path):
+            print(f"Video clip download progress: {progress}%")
+    tator_api.delete_temporary_file(clip.file.id)
 
-def test_get_audio(host, token, project, video):
-    tator_api = tator.get_api(host, token)
-    video_obj = tator_api.get_media(video)
-
-    audio = video_obj.media_files.audio
-    assert len(audio) > 0
-    assert audio[0].codec == 'aac'
-
-def test_get_by_id(host, token, project, video):
-    tator_api = tator.get_api(host, token)
-    video_obj = tator_api.get_media(video)
-    other_obj = tator_api.get_media_list_by_id(project, [video])[0]
-    assert video_obj.id == other_obj.id
```

### Comparing `tator-0.9.6/test/test_state.py` & `tator-1.0.0/test/test_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,159 +1,227 @@
+from pprint import pformat
 import datetime
 import random
+from time import sleep
 import uuid
+from collections import Counter
 
 import tator
 from ._common import assert_close_enough
 
+
+def wait_for_parity(tator_api, project, patch, expected_ids):
+    attribute_filter = [f"test_string::{patch['attributes']['test_string']}"]
+    state_id_query = {"ids": expected_ids}
+    total_timeout = 60.0 # seconds
+    wait_time = 2.0 # seconds
+
+    print(f"Using attribute filter:\n{pformat(attribute_filter)}")
+    from_psql = tator_api.get_state_list_by_id(
+        project,
+        state_id_query=state_id_query,
+        attribute=attribute_filter,
+    )
+    count = tator_api.get_state_count_by_id(
+        project,
+        state_id_query=state_id_query,
+        attribute=attribute_filter,
+    )
+    assert(len(from_psql) == count)
+    for idx in range(int(total_timeout / wait_time) + 1):
+        from_es = tator_api.get_state_list_by_id(
+            project,
+            state_id_query=state_id_query,
+            attribute=attribute_filter
+        )
+        count = tator_api.get_state_count_by_id(
+            project,
+            state_id_query=state_id_query,
+            attribute=attribute_filter
+        )
+        assert(len(from_es) == count)
+
+        if len(from_es) == len(from_psql):
+            print(f"Found expected number of results after {idx * wait_time} seconds")
+            return True
+
+        sleep(wait_time)
+
+    print(f"Did not find expected number of results after {idx * wait_time} seconds")
+    return False
+
 def random_state(project, state_type, video_obj, post=False):
     attributes = {
         'test_bool': random.choice([False, True]),
         'test_int': random.randint(-1000, 1000),
         'test_float': random.uniform(-1000.0, 1000.0),
         'test_enum': random.choice(['a', 'b', 'c']),
         'test_string': str(uuid.uuid1()),
         'test_datetime': datetime.datetime.now().isoformat(),
         'test_geopos': [random.uniform(-180.0, 180.0), random.uniform(-90.0, 90.0)],
+        'test_float_array': [random.uniform(-1.0, 1.0) for _ in range(3)],
     }
     out = {
         'project': project,
         'type': state_type,
         'media_ids': [video_obj.id],
         'frame': random.randint(0, video_obj.num_frames - 1),
+        'attributes':  attributes
     }
-    if post:
-        out = {**out, **attributes}
-    else:
-        out['attributes'] = attributes
-    return out
+    return {**out}
 
-def comparison_query(tator_api, project, exclude):
+def comparison_query(tator_api, project, state_ids, exclude):
     """ Runs a random query and compares results with ES enabled and disabled.
     """
     bool_value = random.choice([True, False])
     int_lower = random.randint(-1000, 0)
     int_upper = random.randint(0, 1000)
     float_lower = random.uniform(-1000.0, 0.0)
     float_upper = random.uniform(0.0, 1000.0)
     enum_value = random.choice(['a', 'b', 'c'])
+    state_id_query = {"ids": state_ids}
     attribute_filter = [f"test_bool::{'true' if bool_value else 'false'}", f"test_enum::{enum_value}"]
     attribute_lte_filter = [f"test_int::{int_upper}"]
     attribute_gte_filter = [f"test_int::{int_lower}"]
     attribute_lt_filter = [f"test_float::{float_upper}"]
     attribute_gt_filter = [f"test_float::{float_lower}"]
+    print("Starting PSQL query...")
     t0 = datetime.datetime.now()
-    from_psql = tator_api.get_state_list(project,
-                                         attribute=attribute_filter,
-                                         attribute_lte=attribute_lte_filter,
-                                         attribute_gte=attribute_gte_filter,
-                                         attribute_lt=attribute_lt_filter,
-                                         attribute_gt=attribute_gt_filter)
+    from_psql = tator_api.get_state_list_by_id(
+        project,
+        state_id_query=state_id_query,
+        attribute=attribute_filter,
+        attribute_lte=attribute_lte_filter,
+        attribute_gte=attribute_gte_filter,
+        attribute_lt=attribute_lt_filter,
+        attribute_gt=attribute_gt_filter,
+    )
     psql_time = datetime.datetime.now() - t0
+    print("Starting ES query...")
     t0 = datetime.datetime.now()
-    from_es = tator_api.get_state_list(project,
-                                       attribute=attribute_filter,
-                                       attribute_lte=attribute_lte_filter,
-                                       attribute_gte=attribute_gte_filter,
-                                       attribute_lt=attribute_lt_filter,
-                                       attribute_gt=attribute_gt_filter,
-                                       force_es=1)
+    from_es = tator_api.get_state_list_by_id(
+        project,
+        state_id_query=state_id_query,
+        attribute=attribute_filter,
+        attribute_lte=attribute_lte_filter,
+        attribute_gte=attribute_gte_filter,
+        attribute_lt=attribute_lt_filter,
+        attribute_gt=attribute_gt_filter,
+        force_es=1,
+    )
     es_time = datetime.datetime.now() - t0
+
+    print("Checking PSQL and ES ids...")
+    psql_ids = [ele.id for ele in from_psql]
+    es_ids = [ele.id for ele in from_es]
+    assert(Counter(psql_ids) == Counter(es_ids))
+
+    print("Checking PSQL and ES values...")
+    assert len(from_psql) == len(from_es)
     for psql, es in zip(from_psql, from_es):
         assert_close_enough(psql, es, exclude)
         assert(psql.attributes['test_bool'] == bool_value)
         assert(psql.attributes['test_int'] <= int_upper)
         assert(psql.attributes['test_int'] >= int_lower)
         assert(psql.attributes['test_float'] < float_upper)
         assert(psql.attributes['test_float'] > float_lower)
         assert(psql.attributes['test_enum'] == enum_value)
     return psql_time, es_time
 
-def test_state_crud(host, token, project, video_type, video, state_type):
+def test_state_crud(host, token, project, video_type, empty_video, state_type):
+    video = empty_video
     tator_api = tator.get_api(host, token)
     video_obj = tator_api.get_media(video)
 
     # These fields will not be checked for object equivalence after patch.
-    exclude = ['project', 'type', 'media_ids', 'id', 'meta', 'user', 'frame']
+    exclude = ['project', 'type', 'media_ids', 'id', 'type', 'user', 'frame', 'ids']
 
     # Test bulk create.
     num_states = random.randint(2000, 10000)
     states = [
         random_state(project, state_type, video_obj, post=True)
         for _ in range(num_states)
     ]
     state_ids = []
-    for response in tator.util.chunked_create(tator_api.create_state_list,
-                                         project, state_spec=states):
+    for response in tator.util.chunked_create(tator_api.create_state_list, project, body=states):
         state_ids += response.id
     assert len(state_ids) == len(states)
     print(f"Created {len(state_ids)} states!")
 
     # Verify list contains the number of entities created
     response = tator_api.get_state_list(project, type=state_type)
     assert len(response) == num_states
 
+    # Test media retrieval by state ID.
+    response = tator_api.get_media_list_by_id(project, {'state_ids': state_ids})
+    assert len(response) == 1
+    assert response[0].id == video
+
+    # Test state retrival by media ID.
+    response = tator_api.get_state_list_by_id(project, {'media_ids': [video]})
+    assert(len(response) == len(state_ids))
+
     # Test single create.
     state = random_state(project, state_type, video_obj, post=True)
-    response = tator_api.create_state_list(project, state_spec=[state])
+    response = tator_api.create_state_list(project, body=state)
     assert isinstance(response, tator.models.CreateListResponse)
     print(response.message)
     state_id = response.id[0]
 
-
-
     # Patch single state.
     patch = random_state(project, state_type, video_obj)
     response = tator_api.update_state(state_id, state_update=patch)
     assert isinstance(response, tator.models.MessageResponse)
     print(response.message)
 
     # Get single state.
     updated_state = tator_api.get_state(state_id)
     assert isinstance(updated_state, tator.models.State)
     assert_close_enough(patch, updated_state, exclude)
 
     # Get state by ID.
-    state_by_id = tator_api.get_state_list_by_id(project, [state_id])[0]
+    state_by_id = tator_api.get_state_list_by_id(project, {'ids': [state_id]})
+    assert(len(state_by_id) == 1)
+    state_by_id = state_by_id[0]
     assert_close_enough(updated_state, state_by_id, exclude)
 
     # Delete single state.
     response = tator_api.delete_state(state_id)
     assert isinstance(response, tator.models.MessageResponse)
     print(response.message)
 
     params = {'media_id': [video], 'type': state_type}
     assert(tator_api.get_state_count(project, **params) == len(states))
 
     # Bulk update state attributes.
     bulk_patch = random_state(project, state_type, video_obj)
     bulk_patch = {'attributes': bulk_patch['attributes']}
     response = tator_api.update_state_list(project, **params,
-                                           attribute_bulk_update=bulk_patch)
+                                           state_bulk_update=bulk_patch)
     assert isinstance(response, tator.models.MessageResponse)
     print(response.message)
 
-    # Do random queries using psql and elasticsearch and compare results.
-    es_time = datetime.timedelta(seconds=0)
-    psql_time = datetime.timedelta(seconds=0)
-    NUM_QUERIES = 10
-    for _ in range(NUM_QUERIES):
-        psql, es = comparison_query(tator_api, project, exclude)
-        psql_time += psql
-        es_time += es
-    print(f"Over {NUM_QUERIES} random attribute queries:")
-    print(f"  Avg PSQL time: {psql_time / NUM_QUERIES}")
-    print(f"  Avg ES time: {es_time / NUM_QUERIES}")
+    # Bulk update specified states by ID.
+    id_bulk_patch = random_state(project, state_type, video_obj)
+    update_ids = random.choices(state_ids, k=100)
+    id_bulk_patch = {'attributes': id_bulk_patch['attributes'], 'ids': update_ids}
+    response = tator_api.update_state_list(project, **params,
+                                           state_bulk_update=id_bulk_patch)
+    assert isinstance(response, tator.models.MessageResponse)
+    print(response.message)
 
     # Verify all states have been updated.
     states = tator_api.get_state_list(project, **params)
     dataframe = tator.util.to_dataframe(states)
     assert(len(states)==len(dataframe))
     for state in states:
-        assert_close_enough(bulk_patch, state, exclude)
+        if state.id in update_ids:
+            assert_close_enough(id_bulk_patch, state, exclude)
+        else:
+            assert_close_enough(bulk_patch, state, exclude)
 
     # Clone states to same media.
     version_mapping = {version.id: version.id for version in tator_api.get_version_list(project)}
     generator = tator.util.clone_state_list(tator_api, {**params, 'project': project},
                                             project, version_mapping, {video:video}, {},
                                             {state_type:state_type}, tator_api)
     for num_created, num_total, response, id_map in generator:
```

### Comparing `tator-0.9.6/test/test_stategraphic.py` & `tator-1.0.0/test/test_stategraphic.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,26 +19,29 @@
     TRACK_LENGTH=200
 
     tator_api = tator.get_api(host, token)
     video_obj = tator_api.get_media(video)
 
     # Make boxes for track.
     boxes = [_make_box(project, box_type, video, frame) for frame in range(TRACK_LENGTH)]
-    response = tator_api.create_localization_list(project, localization_spec=boxes)
+    response = tator_api.create_localization_list(project, boxes)
     assert isinstance(response, tator.models.CreateListResponse)
     print(response.message)
     box_ids = response.id
 
     # Make track.
-    response = tator_api.create_state_list(project, state_spec=[{
-        'project': project,
-        'type': track_type,
-        'media_ids': [video],
-        'localization_ids': box_ids,
-    }])
+    response = tator_api.create_state_list(
+        project,
+        body={
+            'project': project,
+            'type': track_type,
+            'media_ids': [video],
+            'localization_ids': box_ids,
+        },
+    )
     print(response.message)
     assert isinstance(response, tator.models.CreateListResponse)
     track_id = response.id[0]
 
     # Get state graphic.
     t0 = datetime.datetime.now()
     stategraphic = tator.util.full_state_graphic(tator_api, track_id)
```

### Comparing `tator-0.9.6/test/test_version.py` & `tator-1.0.0/test/test_version.py`

 * *Files identical despite different names*

