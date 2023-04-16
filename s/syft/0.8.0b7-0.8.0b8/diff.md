# Comparing `tmp/syft-0.8.0b7.tar.gz` & `tmp/syft-0.8.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.0b7.tar", last modified: Fri Apr 14 05:00:31 2023, max compression
+gzip compressed data, was "syft-0.8.0b8.tar", last modified: Sun Apr 16 13:01:58 2023, max compression
```

## Comparing `syft-0.8.0b7.tar` & `syft-0.8.0b8.tar`

### file list

```diff
@@ -1,138 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.472833 syft-0.8.0b7/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-14 04:57:50.000000 syft-0.8.0b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 04:57:50.000000 syft-0.8.0b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-14 05:00:31.472833 syft-0.8.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-14 04:57:50.000000 syft-0.8.0b7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 04:57:50.000000 syft-0.8.0b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-14 05:00:31.476833 syft-0.8.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 04:57:50.000000 syft-0.8.0b7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.436833 syft-0.8.0b7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.444834 syft-0.8.0b7/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-14 04:58:05.000000 syft-0.8.0b7/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-14 04:58:05.000000 syft-0.8.0b7/src/syft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.448834 syft-0.8.0b7/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.448834 syft-0.8.0b7/src/syft/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.448834 syft-0.8.0b7/src/syft/core/node/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.468834 syft-0.8.0b7/src/syft/core/node/new/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/data_subject_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/dataset_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    19254 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/metadata_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/node_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    21086 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/project_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/sqlite_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16320 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/third_party.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_policy_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/user_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/new/worker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/core/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/experimental_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.468834 syft-0.8.0b7/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.472833 syft-0.8.0b7/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15416 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/gevent_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/user_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 04:57:50.000000 syft-0.8.0b7/src/syft/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:00:31.444834 syft-0.8.0b7/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 05:00:31.000000 syft-0.8.0b7/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.464810 syft-0.8.0b8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-16 12:59:41.000000 syft-0.8.0b8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-16 12:59:41.000000 syft-0.8.0b8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-16 13:01:58.464810 syft-0.8.0b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-16 12:59:41.000000 syft-0.8.0b8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-16 12:59:41.000000 syft-0.8.0b8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-16 13:01:58.464810 syft-0.8.0b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-16 12:59:41.000000 syft-0.8.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.448809 syft-0.8.0b8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-16 12:59:55.000000 syft-0.8.0b8/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-16 12:59:55.000000 syft-0.8.0b8/src/syft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft/core/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.464810 syft-0.8.0b8/src/syft/core/node/new/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/data_subject_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/dataset_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21597 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/metadata_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/node_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21086 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/project_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/sqlite_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/third_party.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_policy_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/user_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/new/worker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26120 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/core/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/experimental_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.464810 syft-0.8.0b8/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.464810 syft-0.8.0b8/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/gevent_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-16 12:59:41.000000 syft-0.8.0b8/src/syft/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:01:58.452809 syft-0.8.0b8/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 13:01:58.000000 syft-0.8.0b8/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.0b7/LICENSE` & `syft-0.8.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/PKG-INFO` & `syft-0.8.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b7
+Version: 0.8.0b8
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -321,7 +321,9 @@
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
 
 [Apache License 2.0](LICENSE)<br />
 <a href="https://www.flaticon.com/free-icons/person" title="person icons">Person icons created by Freepik - Flaticon</a>
+
+<!-- 🥇 -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b7 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.0b8 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.0b7/README.md` & `syft-0.8.0b8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -301,7 +301,9 @@
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
 
 [Apache License 2.0](LICENSE)<br />
 <a href="https://www.flaticon.com/free-icons/person" title="person icons">Person icons created by Freepik - Flaticon</a>
+
+<!-- 🥇 -->
```

### Comparing `syft-0.8.0b7/setup.cfg` & `syft-0.8.0b8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.0-beta.7"
+version = attr: "0.8.0-beta.8"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.0b7/src/syft/VERSION` & `syft-0.8.0b8/src/syft/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.0-beta.7"
+__version__ = "0.8.0-beta.8"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.0b7/src/syft/__init__.py` & `syft-0.8.0b8/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     IMPORTANT: syft.core should be very careful when importing functionality from outside of syft
     core!!! Since we plan to drop syft core down to a language (such as C++ or Rust)
     this can create future complications with lower level languages calling
     higher level ones.
 To begin your education in Syft, continue to the :py:mod:`syft.core.node.vm.vm` module...
 """
 
-__version__ = "0.8.0-beta.7"
+__version__ = "0.8.0-beta.8"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
```

### Comparing `syft-0.8.0b7/src/syft/core/node/__init__.py` & `syft-0.8.0b8/src/syft/core/node/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/action_object.py` & `syft-0.8.0b8/src/syft/core/node/new/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/action_service.py` & `syft-0.8.0b8/src/syft/core/node/new/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/action_types.py` & `syft-0.8.0b8/src/syft/core/node/new/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/api.py` & `syft-0.8.0b8/src/syft/core/node/new/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from result import OkErr
 from result import Result
 from typeguard import check_type
 
 # relative
 from ....telemetry import instrument
 from .connection import NodeConnection
+from .context import AuthedServiceContext
 from .credentials import SyftSigningKey
 from .credentials import SyftVerifyKey
 from .deserialize import _deserialize
 from .node import NewNode
 from .recursive import index_syft_by_module_name
 from .response import SyftAttributeError
 from .response import SyftError
@@ -333,15 +334,15 @@
                 doc_string=service_config.doc_string,
                 signature=service_config.signature,
                 has_self=False,
             )
             endpoints[path] = endpoint
 
         # 🟡 TODO 35: fix root context
-        context = None
+        context = AuthedServiceContext(credentials=user_verify_key)
         method = node.get_method_with_context(UserCodeService.get_all_for_user, context)
         code_items = method()
 
         for code_item in code_items:
             path = "code.call"
             endpoint = APIEndpoint(
                 path=path,
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/array.py` & `syft-0.8.0b8/src/syft/core/node/new/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/arrow.py` & `syft-0.8.0b8/src/syft/core/node/new/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/client.py` & `syft-0.8.0b8/src/syft/core/node/new/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/connection.py` & `syft-0.8.0b8/src/syft/core/node/new/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/context.py` & `syft-0.8.0b8/src/syft/core/node/new/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/credentials.py` & `syft-0.8.0b8/src/syft/core/node/new/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/data_subject.py` & `syft-0.8.0b8/src/syft/core/node/new/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/data_subject_member.py` & `syft-0.8.0b8/src/syft/core/node/new/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/data_subject_member_service.py` & `syft-0.8.0b8/src/syft/core/node/new/data_subject_member_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 # third party
 from result import Result
 
 # relative
 from ....telemetry import instrument
 from .context import AuthedServiceContext
+from .credentials import SyftVerifyKey
 from .data_subject_member import ChildPartitionKey
 from .data_subject_member import DataSubjectMemberRelationship
 from .data_subject_member import ParentPartitionKey
 from .document_store import BaseUIDStoreStash
 from .document_store import DocumentStore
 from .document_store import PartitionSettings
 from .document_store import QueryKeys
@@ -33,24 +34,24 @@
         object_type=DataSubjectMemberRelationship,
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
     def get_all_for_parent(
-        self, name: str
+        self, credentials: SyftVerifyKey, name: str
     ) -> Result[Optional[DataSubjectMemberRelationship], str]:
         qks = QueryKeys(qks=[ParentPartitionKey.with_obj(name)])
-        return self.query_all(qks=qks)
+        return self.query_all(credentials=credentials, qks=qks)
 
     def get_all_for_child(
-        self, name: str
+        self, credentials: SyftVerifyKey, name: str
     ) -> Result[Optional[DataSubjectMemberRelationship], str]:
         qks = QueryKeys(qks=[ChildPartitionKey.with_obj(name)])
-        return self.query_all(qks=qks)
+        return self.query_all(credentials=credentials, qks=qks)
 
 
 @instrument
 @serializable()
 class DataSubjectMemberService(AbstractService):
     store: DocumentStore
     stash: DataSubjectMemberStash
@@ -60,24 +61,26 @@
         self.stash = DataSubjectMemberStash(store=store)
 
     def add(
         self, context: AuthedServiceContext, parent: str, child: str
     ) -> Union[SyftSuccess, SyftError]:
         """Register relationship between data subject and it's member."""
         relation = DataSubjectMemberRelationship(parent=parent, child=child)
-        result = self.stash.set(relation, ignore_duplicates=True)
+        result = self.stash.set(context.credentials, relation, ignore_duplicates=True)
         if result.is_err():
             return SyftError(result.err())
         return SyftSuccess(message=f"Relationship added for: {parent} -> {child}")
 
     def get_relatives(
         self, context: AuthedServiceContext, data_subject_name: str
     ) -> Union[List[str], SyftError]:
         """Get all Members for given data subject"""
-        result = self.stash.get_all_for_parent(name=data_subject_name)
+        result = self.stash.get_all_for_parent(
+            context.credentials, name=data_subject_name
+        )
         if result.is_ok():
             data_subject_members = result.ok()
             return data_subject_members
         return SyftError(message=result.err())
 
 
 TYPE_TO_SERVICE[DataSubjectMemberRelationship] = DataSubjectMemberService
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/data_subject_service.py` & `syft-0.8.0b8/src/syft/core/node/new/data_subject_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 # third party
 from result import Result
 
 # relative
 from ....telemetry import instrument
 from .context import AuthedServiceContext
+from .credentials import SyftVerifyKey
 from .data_subject import DataSubject
 from .data_subject import DataSubjectCreate
 from .data_subject import NamePartitionKey
 from .data_subject_member_service import DataSubjectMemberService
 from .document_store import BaseUIDStoreStash
 from .document_store import DocumentStore
 from .document_store import PartitionSettings
@@ -33,20 +34,28 @@
     settings: PartitionSettings = PartitionSettings(
         name=DataSubject.__canonical_name__, object_type=DataSubject
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
-    def get_by_name(self, name: str) -> Result[Optional[DataSubject], str]:
+    def get_by_name(
+        self, credentials: SyftVerifyKey, name: str
+    ) -> Result[Optional[DataSubject], str]:
         qks = QueryKeys(qks=[NamePartitionKey.with_obj(name)])
-        return self.query_one(qks=qks)
+        return self.query_one(credentials, qks=qks)
 
-    def update(self, data_subject: DataSubject) -> Result[DataSubject, str]:
-        return self.check_type(data_subject, DataSubject).and_then(super().update)
+    def update(
+        self, credentials: SyftVerifyKey, data_subject: DataSubject
+    ) -> Result[DataSubject, str]:
+        res = self.check_type(data_subject, DataSubject)
+        # we dont use and_then logic here as it is hard because of the order of the arguments
+        if res.is_err():
+            return res
+        return super().update(credentials=credentials, obj=res.ok())
 
 
 @instrument
 @serializable()
 class DataSubjectService(AbstractService):
     store: DocumentStore
     stash: DataSubjectStash
@@ -66,15 +75,17 @@
         )
 
         member_relationships = data_subject.member_relationships
         for member_relationship in member_relationships:
             parent_ds, child_ds = member_relationship
             for ds in [parent_ds, child_ds]:
                 result = self.stash.set(
-                    ds.to(DataSubject, context=context), ignore_duplicates=True
+                    context.credentials,
+                    ds.to(DataSubject, context=context),
+                    ignore_duplicates=True,
                 )
                 if result.is_err():
                     return SyftError(message=str(result.err()))
             result = member_relationship_add(context, parent_ds.name, child_ds.name)
             if isinstance(result, SyftError):
                 return result
 
@@ -83,15 +94,15 @@
         )
 
     @service_method(path="data_subject.get_all", name="get_all")
     def get_all(
         self, context: AuthedServiceContext
     ) -> Union[List[DataSubject], SyftError]:
         """Get all Data subjects"""
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             data_subjects = result.ok()
             return data_subjects
         return SyftError(message=result.err())
 
     @service_method(path="data_subject.get_members", name="members_for")
     def get_members(
@@ -116,15 +127,15 @@
         return members
 
     @service_method(path="data_subject.get_by_name", name="get_by_name")
     def get_by_name(
         self, context: AuthedServiceContext, name: str
     ) -> Union[SyftSuccess, SyftError]:
         """Get a Data Subject by its name."""
-        result = self.stash.get_by_name(name=name)
+        result = self.stash.get_by_name(context.credentials, name=name)
         if result.is_ok():
             data_subject = result.ok()
             return data_subject
         return SyftError(message=result.err())
 
 
 TYPE_TO_SERVICE[DataSubject] = DataSubjectService
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/dataset.py` & `syft-0.8.0b8/src/syft/core/node/new/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/dataset_service.py` & `syft-0.8.0b8/src/syft/core/node/new/dataset_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # stdlib
 from typing import List
 from typing import Union
 
 # relative
 from ....telemetry import instrument
+from .action_permissions import ActionObjectPermission
+from .action_permissions import ActionPermission
 from .context import AuthedServiceContext
 from .dataset import Asset
 from .dataset import CreateDataset
 from .dataset import Dataset
 from .dataset_stash import DatasetStash
 from .document_store import DocumentStore
 from .response import SyftError
@@ -33,23 +35,32 @@
         self.stash = DatasetStash(store=store)
 
     @service_method(path="dataset.add", name="add", roles=DATA_OWNER_ROLE_LEVEL)
     def add(
         self, context: AuthedServiceContext, dataset: CreateDataset
     ) -> Union[SyftSuccess, SyftError]:
         """Add a Dataset"""
-        result = self.stash.set(dataset.to(Dataset, context=context))
+        dataset = dataset.to(Dataset, context=context)
+        result = self.stash.set(
+            context.credentials,
+            dataset,
+            add_permissions=[
+                ActionObjectPermission(
+                    uid=dataset.id, permission=ActionPermission.ALL_READ
+                ),
+            ],
+        )
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Dataset Added")
 
     @service_method(path="dataset.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
     def get_all(self, context: AuthedServiceContext) -> Union[List[Dataset], SyftError]:
         """Get a Dataset"""
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             datasets = result.ok()
             results = []
             for dataset in datasets:
                 dataset.node_uid = context.node.id
                 results.append(dataset)
             return results
@@ -69,27 +80,27 @@
         )
 
     @service_method(path="dataset.get_by_id", name="get_by_id")
     def get_by_id(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
         """Get a Dataset"""
-        result = self.stash.get_by_uid(uid=uid)
+        result = self.stash.get_by_uid(context.credentials, uid=uid)
         if result.is_ok():
             dataset = result.ok()
             dataset.node_uid = context.node.id
             return dataset
         return SyftError(message=result.err())
 
     @service_method(path="dataset.get_by_action_id", name="get_by_action_id")
     def get_by_action_id(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[List[Dataset], SyftError]:
         """Get Datasets by an Action ID"""
-        result = self.stash.search_action_ids(uid=uid)
+        result = self.stash.search_action_ids(context.credentials, uid=uid)
         if result.is_ok():
             datasets = result.ok()
             for dataset in datasets:
                 dataset.node_uid = context.node.id
             return datasets
         return SyftError(message=result.err())
 
@@ -110,15 +121,15 @@
             return assets
         elif isinstance(datasets, SyftError):
             return datasets
         return []
 
     @service_method(path="dataset.delete_by_id", name="dataset_delete_by_id")
     def delete_dataset(self, context: AuthedServiceContext, uid: UID):
-        result = self.stash.delete_by_uid(uid)
+        result = self.stash.delete_by_uid(context.credentials, uid)
         if result.is_ok():
             return result.ok()
         else:
             return SyftError(message=result.err())
 
 
 TYPE_TO_SERVICE[Dataset] = DatasetService
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/dataset_stash.py` & `syft-0.8.0b8/src/syft/core/node/new/dataset_stash.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional
 
 # third party
 from result import Result
 
 # relative
 from ....telemetry import instrument
+from .credentials import SyftVerifyKey
 from .dataset import Dataset
 from .dataset import DatasetUpdate
 from .document_store import BaseUIDStoreStash
 from .document_store import DocumentStore
 from .document_store import PartitionKey
 from .document_store import PartitionSettings
 from .document_store import QueryKeys
@@ -28,17 +29,27 @@
     settings: PartitionSettings = PartitionSettings(
         name=Dataset.__canonical_name__, object_type=Dataset
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
-    def get_by_name(self, name: str) -> Result[Optional[Dataset], str]:
+    def get_by_name(
+        self, credentials: SyftVerifyKey, name: str
+    ) -> Result[Optional[Dataset], str]:
         qks = QueryKeys(qks=[NamePartitionKey.with_obj(name)])
-        return self.query_one(qks=qks)
+        return self.query_one(credentials=credentials, qks=qks)
 
-    def update(self, dataset_update: DatasetUpdate) -> Result[Dataset, str]:
-        return self.check_type(dataset_update, DatasetUpdate).and_then(super().update)
-
-    def search_action_ids(self, uid: UID) -> Result[List[Dataset], str]:
+    def update(
+        self, credentials: SyftVerifyKey, dataset_update: DatasetUpdate
+    ) -> Result[Dataset, str]:
+        res = self.check_type(dataset_update, DatasetUpdate)
+        # we dont use and_then logic here as it is hard because of the order of the arguments
+        if res.is_err():
+            return res
+        return super().update(credentials=credentials, obj=res.ok())
+
+    def search_action_ids(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Result[List[Dataset], str]:
         qks = QueryKeys(qks=[ActionIDsPartitionKey.with_obj(uid)])
-        return self.query_all(qks=qks)
+        return self.query_all(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/datetime.py` & `syft-0.8.0b8/src/syft/core/node/new/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/decorators.py` & `syft-0.8.0b8/src/syft/core/node/new/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/deserialize.py` & `syft-0.8.0b8/src/syft/core/node/new/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/dict_document_store.py` & `syft-0.8.0b8/src/syft/core/node/new/dict_document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # stdlib
 from typing import Any
 from typing import Optional
 from typing import Type
 
 # relative
+from .credentials import SyftVerifyKey
 from .document_store import DocumentStore
 from .document_store import StoreConfig
 from .kv_document_store import KeyValueBackingStore
 from .kv_document_store import KeyValueStorePartition
 from .locks import LockingConfig
 from .locks import ThreadingLockingConfig
 from .serializable import serializable
@@ -57,18 +58,22 @@
     Parameters:
         `store_config`: DictStoreConfig
             Dictionary Store specific configuration, containing the store type and the backing store type
     """
 
     partition_type = DictStorePartition
 
-    def __init__(self, store_config: Optional[DictStoreConfig] = None) -> None:
+    def __init__(
+        self,
+        root_verify_key: Optional[SyftVerifyKey],
+        store_config: Optional[DictStoreConfig] = None,
+    ) -> None:
         if store_config is None:
             store_config = DictStoreConfig()
-        super().__init__(store_config=store_config)
+        super().__init__(root_verify_key=root_verify_key, store_config=store_config)
 
     def reset(self):
         for _, partition in self.partitions.items():
             partition.prune()
 
 
 @serializable()
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/document_store.py` & `syft-0.8.0b8/src/syft/core/node/new/document_store.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # future
 from __future__ import annotations
 
 # stdlib
-from functools import partial
 import sys
 import types
 import typing
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
@@ -20,15 +19,18 @@
 from result import Err
 from result import Ok
 from result import Result
 from typeguard import check_type
 
 # relative
 from ....telemetry import instrument
+from .action_permissions import ActionObjectPermission
 from .base import SyftBaseModel
+from .credentials import SyftSigningKey
+from .credentials import SyftVerifyKey
 from .locks import LockingConfig
 from .locks import NoLockingConfig
 from .locks import SyftLock
 from .response import SyftSuccess
 from .serializable import serializable
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftBaseObject
@@ -309,17 +311,21 @@
             PySyft specific settings
         store_config: StoreConfig
             Backend specific configuration
     """
 
     def __init__(
         self,
+        root_verify_key: SyftVerifyKey,
         settings: PartitionSettings,
         store_config: StoreConfig,
     ) -> None:
+        if root_verify_key is None:
+            root_verify_key = SyftSigningKey.generate().verify_key
+        self.root_verify_key = root_verify_key
         self.settings = settings
         self.store_config = store_config
         self.init_store()
 
         store_config.locking_config.lock_name = settings.name
         self.lock = SyftLock(store_config.locking_config)
 
@@ -355,49 +361,93 @@
         except BaseException as e:
             result = Err(str(e))
         self.lock.release()
 
         return result
 
     def set(
-        self, obj: SyftObject, ignore_duplicates: bool = False
+        self,
+        credentials: SyftVerifyKey,
+        obj: SyftObject,
+        add_permissions: Optional[List[ActionObjectPermission]] = None,
+        ignore_duplicates: bool = False,
+    ) -> Result[SyftObject, str]:
+        return self._thread_safe_cbk(
+            self._set,
+            credentials=credentials,
+            obj=obj,
+            add_permissions=add_permissions,
+            ignore_duplicates=ignore_duplicates,
+        )
+
+    def get(
+        self,
+        credentials: SyftVerifyKey,
+        uid: UID,
+        skip_permissions: bool = False,
     ) -> Result[SyftObject, str]:
         return self._thread_safe_cbk(
-            self._set, obj=obj, ignore_duplicates=ignore_duplicates
+            self._get,
+            uid=uid,
+            credentials=credentials,
+            skip_permissions=skip_permissions,
         )
 
     def find_index_or_search_keys(
-        self, index_qks: QueryKeys, search_qks: QueryKeys
+        self, credentials: SyftVerifyKey, index_qks: QueryKeys, search_qks: QueryKeys
     ) -> Result[List[SyftObject], str]:
         return self._thread_safe_cbk(
-            self._find_index_or_search_keys, index_qks=index_qks, search_qks=search_qks
+            self._find_index_or_search_keys,
+            credentials,
+            index_qks=index_qks,
+            search_qks=search_qks,
         )
 
     def remove_keys(
         self,
         unique_query_keys: QueryKeys,
         searchable_query_keys: QueryKeys,
     ) -> None:
         self._thread_safe_cbk(
             self._remove_keys,
             unique_query_keys=unique_query_keys,
             searchable_query_keys=searchable_query_keys,
         )
 
-    def update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
-        return self._thread_safe_cbk(self._update, qk=qk, obj=obj)
+    def update(
+        self,
+        credentials: SyftVerifyKey,
+        qk: QueryKey,
+        obj: SyftObject,
+        has_permission=False,
+    ) -> Result[SyftObject, str]:
+        return self._thread_safe_cbk(
+            self._update,
+            credentials=credentials,
+            qk=qk,
+            obj=obj,
+            has_permission=has_permission,
+        )
 
-    def get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
-        return self._thread_safe_cbk(self._get_all_from_store, qks)
+    def get_all_from_store(
+        self, credentials: SyftVerifyKey, qks: QueryKeys
+    ) -> Result[List[SyftObject], str]:
+        return self._thread_safe_cbk(self._get_all_from_store, credentials, qks)
 
-    def delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
-        return self._thread_safe_cbk(self._delete, qk)
+    def delete(
+        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission=False
+    ) -> Result[SyftSuccess, Err]:
+        return self._thread_safe_cbk(
+            self._delete, credentials, qk, has_permission=has_permission
+        )
 
-    def all(self) -> Result[List[BaseStash.object_type], str]:
-        return self._thread_safe_cbk(self._all)
+    def all(
+        self, credentials: SyftVerifyKey
+    ) -> Result[List[BaseStash.object_type], str]:
+        return self._thread_safe_cbk(self._all, credentials)
 
     # Potentially thread-unsafe methods.
     # CAUTION:
     #       * Don't use self.lock here.
     #       * Do not call the public thread-safe methods here(with locking).
     # These methods are called from the public thread-safe API, and will hang the process.
     def _set(
@@ -406,15 +456,17 @@
         ignore_duplicates: bool = False,
     ) -> Result[SyftObject, str]:
         raise NotImplementedError
 
     def _update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
         raise NotImplementedError
 
-    def _get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
+    def _get_all_from_store(
+        self, credentials: SyftVerifyKey, qks: QueryKeys
+    ) -> Result[List[SyftObject], str]:
         raise NotImplementedError
 
     def _delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
         raise NotImplementedError
 
     def _all(self) -> Result[List[BaseStash.object_type], str]:
         raise NotImplementedError
@@ -429,24 +481,29 @@
         store_config: StoreConfig
             Store specific configuration.
     """
 
     partitions: Dict[str, StorePartition]
     partition_type: Type[StorePartition]
 
-    def __init__(self, store_config: StoreConfig) -> None:
+    def __init__(
+        self, root_verify_key: Optional[SyftVerifyKey], store_config: StoreConfig
+    ) -> None:
         if store_config is None:
             raise Exception("must have store config")
         self.partitions = {}
         self.store_config = store_config
+        self.root_verify_key = root_verify_key
 
     def partition(self, settings: PartitionSettings) -> StorePartition:
         if settings.name not in self.partitions:
             self.partitions[settings.name] = self.partition_type(
-                settings=settings, store_config=self.store_config
+                root_verify_key=self.root_verify_key,
+                settings=settings,
+                store_config=self.store_config,
             )
         return self.partitions[settings.name]
 
 
 @instrument
 class BaseStash:
     object_type: Type[SyftObject]
@@ -460,29 +517,38 @@
     def check_type(self, obj: Any, type_: type) -> Result[Any, str]:
         return (
             Ok(obj)
             if isinstance(obj, type_)
             else Err(f"{type(obj)} does not match required type: {type_}")
         )
 
-    def get_all(self) -> Result[List[BaseStash.object_type], str]:
-        return self.partition.all()
+    def get_all(
+        self, credentials: SyftVerifyKey
+    ) -> Result[List[BaseStash.object_type], str]:
+        return self.partition.all(credentials)
 
     def __len__(self) -> int:
         return len(self.partition)
 
     def set(
         self,
+        credentials: SyftVerifyKey,
         obj: BaseStash.object_type,
+        add_permissions: Optional[List[ActionObjectPermission]] = None,
         ignore_duplicates: bool = False,
     ) -> Result[BaseStash.object_type, str]:
-        return self.partition.set(obj=obj, ignore_duplicates=ignore_duplicates)
+        return self.partition.set(
+            credentials=credentials,
+            obj=obj,
+            ignore_duplicates=ignore_duplicates,
+            add_permissions=add_permissions,
+        )
 
     def query_all(
-        self, qks: Union[QueryKey, QueryKeys]
+        self, credentials: SyftVerifyKey, qks: Union[QueryKey, QueryKeys]
     ) -> Result[List[BaseStash.object_type], str]:
         if isinstance(qks, QueryKey):
             qks = QueryKeys(qks=qks)
 
         unique_keys = []
         searchable_keys = []
 
@@ -495,89 +561,114 @@
             else:
                 return Err(
                     f"{qk} not in {type(self.partition)} unique or searchable keys"
                 )
 
         index_qks = QueryKeys(qks=unique_keys)
         search_qks = QueryKeys(qks=searchable_keys)
+
         return self.partition.find_index_or_search_keys(
-            index_qks=index_qks, search_qks=search_qks
+            credentials=credentials, index_qks=index_qks, search_qks=search_qks
         )
 
     def query_all_kwargs(
-        self, **kwargs: Dict[str, Any]
+        self, credentials: SyftVerifyKey, **kwargs: Dict[str, Any]
     ) -> Result[List[BaseStash.object_type], str]:
         qks = QueryKeys.from_dict(kwargs)
-        return self.query_all(qks=qks)
+        return self.query_all(credentials=credentials, qks=qks)
 
     def query_one(
-        self, qks: Union[QueryKey, QueryKeys]
+        self, credentials: SyftVerifyKey, qks: Union[QueryKey, QueryKeys]
     ) -> Result[Optional[BaseStash.object_type], str]:
-        return self.query_all(qks=qks).and_then(first_or_none)
+        return self.query_all(credentials=credentials, qks=qks).and_then(first_or_none)
 
     def query_one_kwargs(
         self,
+        credentials: SyftVerifyKey,
         **kwargs: Dict[str, Any],
     ) -> Result[Optional[BaseStash.object_type], str]:
-        return self.query_all_kwargs(**kwargs).and_then(first_or_none)
+        return self.query_all_kwargs(credentials, **kwargs).and_then(first_or_none)
 
     def find_all(
-        self, **kwargs: Dict[str, Any]
+        self, credentials: SyftVerifyKey, **kwargs: Dict[str, Any]
     ) -> Result[List[BaseStash.object_type], str]:
-        return self.query_all_kwargs(**kwargs)
+        return self.query_all_kwargs(credentials=credentials, **kwargs)
 
     def find_one(
-        self, **kwargs: Dict[str, Any]
+        self, credentials: SyftVerifyKey, **kwargs: Dict[str, Any]
     ) -> Result[Optional[BaseStash.object_type], str]:
-        return self.query_one_kwargs(**kwargs)
+        return self.query_one_kwargs(credentials=credentials, **kwargs)
 
-    def find_and_delete(self, **kwargs: Dict[str, Any]) -> Result[SyftSuccess, Err]:
-        obj = self.query_one_kwargs(**kwargs)
+    def find_and_delete(
+        self, credentials: SyftVerifyKey, **kwargs: Dict[str, Any]
+    ) -> Result[SyftSuccess, Err]:
+        obj = self.query_one_kwargs(credentials=credentials, **kwargs)
         if obj.is_err():
             return obj
         else:
             obj = obj.ok()
 
         if not obj:
             return Err(f"Object does not exists with kwargs: {kwargs}")
         qk = self.partition.store_query_key(obj)
-        return self.delete(qk=qk)
+        return self.delete(credentials=credentials, qk=qk)
 
-    def delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
-        return self.partition.delete(qk=qk)
+    def delete(
+        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission=False
+    ) -> Result[SyftSuccess, Err]:
+        return self.partition.delete(
+            credentials=credentials, qk=qk, has_permission=has_permission
+        )
 
     def update(
-        self, obj: BaseStash.object_type
+        self,
+        credentials: SyftVerifyKey,
+        obj: BaseStash.object_type,
+        has_permission=False,
     ) -> Optional[Result[BaseStash.object_type, str]]:
         qk = self.partition.store_query_key(obj)
-        return self.partition.update(qk=qk, obj=obj)
+        return self.partition.update(
+            credentials=credentials, qk=qk, obj=obj, has_permission=has_permission
+        )
 
 
 @instrument
 class BaseUIDStoreStash(BaseStash):
-    def delete_by_uid(self, uid: UID) -> Result[SyftSuccess, str]:
+    def delete_by_uid(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Result[SyftSuccess, str]:
         qk = UIDPartitionKey.with_obj(uid)
-        result = super().delete(qk=qk)
+        result = super().delete(credentials=credentials, qk=qk)
         if result.is_ok():
             return Ok(SyftSuccess(message=f"ID: {uid} deleted"))
         return result
 
     def get_by_uid(
-        self, uid: UID
+        self, credentials: SyftVerifyKey, uid: UID
     ) -> Result[Optional[BaseUIDStoreStash.object_type], str]:
         qks = QueryKeys(qks=[UIDPartitionKey.with_obj(uid)])
-        return self.query_one(qks=qks)
+        return self.query_one(credentials=credentials, qks=qks)
 
     def set(
         self,
+        credentials: SyftVerifyKey,
         obj: BaseUIDStoreStash.object_type,
+        add_permissions: Optional[List[ActionObjectPermission]] = None,
         ignore_duplicates: bool = False,
     ) -> Result[BaseUIDStoreStash.object_type, str]:
-        set_method = partial(super().set, ignore_duplicates=ignore_duplicates)
-        return self.check_type(obj, self.object_type).and_then(set_method)
+        res = self.check_type(obj, self.object_type)
+        # we dont use and_then logic here as it is hard because of the order of the arguments
+        if res.is_err():
+            return res
+        return super().set(
+            credentials=credentials,
+            obj=res.ok(),
+            ignore_duplicates=ignore_duplicates,
+            add_permissions=add_permissions,
+        )
 
 
 @serializable()
 class StoreConfig(SyftBaseObject):
     """Base Store configuration
 
     Parameters:
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/grid_url.py` & `syft-0.8.0b8/src/syft/core/node/new/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/kv_document_store.py` & `syft-0.8.0b8/src/syft/core/node/new/kv_document_store.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,21 +12,31 @@
 # third party
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
+from .action_permissions import ActionObjectEXECUTE
+from .action_permissions import ActionObjectOWNER
+from .action_permissions import ActionObjectPermission
+from .action_permissions import ActionObjectREAD
+from .action_permissions import ActionObjectWRITE
+from .action_permissions import ActionPermission
+from .credentials import SyftVerifyKey
 from .document_store import BaseStash
+from .document_store import PartitionSettings
 from .document_store import QueryKey
 from .document_store import QueryKeys
+from .document_store import StoreConfig
 from .document_store import StorePartition
 from .response import SyftSuccess
 from .serializable import serializable
 from .syft_object import SyftObject
+from .uid import UID
 
 
 @serializable()
 class UniqueKeyCheck(Enum):
     EMPTY = 0
     MATCHES = 1
     ERROR = 2
@@ -84,14 +94,22 @@
     Parameters:
         `settings`: PartitionSettings
             PySyft specific settings
         `store_config`: StoreConfig
             Backend specific configuration
     """
 
+    def __init__(
+        self,
+        root_verify_key: Optional[SyftVerifyKey],
+        settings: PartitionSettings,
+        store_config: StoreConfig,
+    ):
+        super().__init__(root_verify_key, settings, store_config)
+
     def init_store(self) -> Result[Ok, Err]:
         store_status = super().init_store()
         if store_status.is_err():
             return store_status
 
         try:
             self.data = self.store_config.backing_store(
@@ -99,14 +117,17 @@
             )
             self.unique_keys = self.store_config.backing_store(
                 "unique_keys", self.settings, self.store_config
             )
             self.searchable_keys = self.store_config.backing_store(
                 "searchable_keys", self.settings, self.store_config
             )
+            self.permissions = self.store_config.backing_store(
+                "permissions", self.settings, self.store_config, ddtype=set
+            )
 
             for partition_key in self.unique_cks:
                 pk_key = partition_key.key
                 if pk_key not in self.unique_keys:
                     self.unique_keys[pk_key] = {}
 
             for partition_key in self.searchable_cks:
@@ -117,43 +138,162 @@
             return Err(str(e))
 
         return Ok()
 
     def __len__(self) -> int:
         return len(self.data)
 
+    def _get(
+        self, uid: UID, credentials: SyftVerifyKey, skip_permission: bool = False
+    ) -> Result[SyftObject, str]:
+        # relative
+        from .action_store import ActionObjectREAD
+
+        # TODO 🟣 Temporarily added skip permission argument for enclave
+        # until permissions are fully integrated
+        # if you get something you need READ permission
+        read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
+        # if True:
+        if skip_permission or self.has_permission(read_permission):
+            syft_object = self.data[uid]
+            return Ok(syft_object)
+        return Err(f"Permission: {read_permission} denied")
+
     # Potentially thread-unsafe methods.
     # CAUTION:
     #       * Don't use self.lock here.
     #       * Do not call the public thread-safe methods here(with locking).
     # These methods are called from the public thread-safe API, and will hang the process.
 
     def _set(
-        self, obj: SyftObject, ignore_duplicates: bool = False
+        self,
+        credentials: SyftVerifyKey,
+        obj: SyftObject,
+        add_permissions: Optional[List[ActionObjectPermission]] = None,
+        ignore_duplicates: bool = False,
     ) -> Result[SyftObject, str]:
         try:
+            if obj.id is None:
+                obj.id = UID()
             store_query_key = self.settings.store_key.with_obj(obj)
+            uid = store_query_key.value
+            write_permission = ActionObjectWRITE(uid=uid, credentials=credentials)
+            can_write = self.has_permission(write_permission)
             unique_query_keys = self.settings.unique_keys.with_obj(obj)
+            store_key_exists = store_query_key.value in self.data
             searchable_query_keys = self.settings.searchable_keys.with_obj(obj)
-            ck_check = self._validate_partition_keys(
-                store_query_key=store_query_key, unique_query_keys=unique_query_keys
+
+            ck_check = self._check_partition_keys_unique(
+                unique_query_keys=unique_query_keys
             )
-            exists = store_query_key.value in self.data
-            if not exists and ck_check == UniqueKeyCheck.EMPTY:
+
+            if not store_key_exists and ck_check == UniqueKeyCheck.EMPTY:
+                # attempt to claim it for writing
+                ownership_result = self.take_ownership(uid=uid, credentials=credentials)
+                can_write = True if ownership_result.is_ok() else False
+            elif not ignore_duplicates:
+                return Err(f"Duplication Key Error: {obj}")
+            else:
+                # we are not throwing an error, because we are ignoring duplicates
+                # we are also not writing though
+                return Ok(obj)
+
+            if can_write:
                 self._set_data_and_keys(
                     store_query_key=store_query_key,
                     unique_query_keys=unique_query_keys,
                     searchable_query_keys=searchable_query_keys,
                     obj=obj,
                 )
-            elif not ignore_duplicates:
-                return Err(f"Duplication Key Error: {obj}")
+                self.data[uid] = obj
+                if uid not in self.permissions:
+                    # create default permissions
+                    self.permissions[uid] = set()
+                permission = f"{credentials.verify}_READ"
+                permissions = self.permissions[uid]
+                permissions.add(permission)
+                if add_permissions is not None:
+                    permissions.update([x.permission_string for x in add_permissions])
+                self.permissions[uid] = permissions
+                return Ok(obj)
+            else:
+                return Err(f"Permission: {write_permission} denied")
         except Exception as e:
             return Err(f"Failed to write obj {obj}. {e}")
-        return Ok(obj)
+
+    def take_ownership(
+        self, uid: UID, credentials: SyftVerifyKey
+    ) -> Result[SyftSuccess, str]:
+        # first person using this UID can claim ownership
+        if uid not in self.permissions and uid not in self.data:
+            self.add_permissions(
+                [
+                    ActionObjectOWNER(uid=uid, credentials=credentials),
+                    ActionObjectWRITE(uid=uid, credentials=credentials),
+                    ActionObjectREAD(uid=uid, credentials=credentials),
+                    ActionObjectEXECUTE(uid=uid, credentials=credentials),
+                ]
+            )
+            return Ok(SyftSuccess(message=f"Ownership of ID: {uid} taken."))
+        return Err(f"UID: {uid} already owned.")
+
+    def add_permission(self, permission: ActionObjectPermission) -> None:
+        permissions = self.permissions[permission.uid]
+        permissions.add(permission.permission_string)
+        self.permissions[permission.uid] = permissions
+
+    def remove_permission(self, permission: ActionObjectPermission):
+        permissions = self.permissions[permission.uid]
+        permissions.remove(permission.permission_string)
+        self.permissions[permission.uid] = permissions
+
+    def add_permissions(self, permissions: List[ActionObjectPermission]) -> None:
+        results = []
+        for permission in permissions:
+            results.append(self.add_permission(permission))
+
+    def has_permission(self, permission: ActionObjectPermission) -> bool:
+        if not isinstance(permission.permission, ActionPermission):
+            raise Exception(f"ObjectPermission type: {permission.permission} not valid")
+
+        # TODO: fix for other admins
+        if self.root_verify_key.verify == permission.credentials.verify:
+            return True
+
+        if (
+            permission.uid in self.permissions
+            and permission.permission_string in self.permissions[permission.uid]
+        ):
+            return True
+
+        # 🟡 TODO 14: add ALL_READ, ALL_EXECUTE etc
+        # third party
+        if permission.permission == ActionPermission.OWNER:
+            pass
+        elif (
+            permission.permission == ActionPermission.READ
+            and ActionObjectPermission(
+                permission.uid, ActionPermission.ALL_READ
+            ).permission_string
+            in self.permissions[permission.uid]
+        ):
+            return True
+        elif permission.permission == ActionPermission.WRITE:
+            pass
+        elif permission.permission == ActionPermission.EXECUTE:
+            pass
+
+        return False
+
+    def _all(
+        self, credentials: SyftVerifyKey
+    ) -> Result[List[BaseStash.object_type], str]:
+        # this checks permissions
+        res = [self._get(uid, credentials) for uid in self.data.keys()]
+        return Ok([x.ok() for x in res if x.is_ok()])
 
     def _remove_keys(
         self,
         unique_query_keys: QueryKeys,
         searchable_query_keys: QueryKeys,
     ) -> None:
         uqks = unique_query_keys.all
@@ -165,18 +305,19 @@
         sqks = searchable_query_keys.all
         for qk in sqks:
             pk_key, pk_value = qk.key, qk.value
             ck_col = self.searchable_keys[pk_key]
             ck_col.pop(pk_value, None)
 
     def _find_index_or_search_keys(
-        self, index_qks: QueryKeys, search_qks: QueryKeys
+        self, credentials: SyftVerifyKey, index_qks: QueryKeys, search_qks: QueryKeys
     ) -> Result[List[SyftObject], str]:
         ids: Optional[Set] = None
         errors = []
+        # third party
         if len(index_qks.all) > 0:
             index_results = self._get_keys_index(qks=index_qks)
             if index_results.is_ok():
                 if ids is None:
                     ids = index_results.ok()
                 ids = ids.intersection(index_results.ok())
             else:
@@ -195,68 +336,126 @@
 
         if len(errors) > 0:
             return Err(" ".join(errors))
 
         if ids is None:
             return Ok([])
 
-        qks = self.store_query_keys(ids)
-        return self._get_all_from_store(qks=qks)
+        qks: QueryKeys = self.store_query_keys(ids)
+        return self._get_all_from_store(credentials=credentials, qks=qks)
+
+    def remove_keys(
+        self,
+        unique_query_keys: QueryKeys,
+        searchable_query_keys: QueryKeys,
+    ) -> None:
+        uqks = unique_query_keys.all
+        for qk in uqks:
+            pk_key, pk_value = qk.key, qk.value
+            ck_col = self.unique_keys[pk_key]
+            ck_col.pop(pk_value, None)
+
+        sqks = searchable_query_keys.all
+        for qk in sqks:
+            pk_key, pk_value = qk.key, qk.value
+            ck_col = self.searchable_keys[pk_key]
+            ck_col.pop(pk_value, None)
 
-    def _update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
+    def _update(
+        self,
+        credentials: SyftVerifyKey,
+        qk: QueryKey,
+        obj: SyftObject,
+        has_permission=False,
+    ) -> Result[SyftObject, str]:
         try:
             if qk.value not in self.data:
                 return Err(f"No object exists for query key: {qk}")
 
-            _original_obj = self.data[qk.value]
-            _original_unique_keys = self.settings.unique_keys.with_obj(_original_obj)
-            _original_searchable_keys = self.settings.searchable_keys.with_obj(
-                _original_obj
-            )
+            if has_permission or self.has_permission(
+                ActionObjectWRITE(uid=qk.value, credentials=credentials)
+            ):
+                _original_obj = self.data[qk.value]
+                _original_unique_keys = self.settings.unique_keys.with_obj(
+                    _original_obj
+                )
+                _original_searchable_keys = self.settings.searchable_keys.with_obj(
+                    _original_obj
+                )
 
-            # remove old keys
-            self._remove_keys(
-                unique_query_keys=_original_unique_keys,
-                searchable_query_keys=_original_searchable_keys,
-            )
+                # remove old keys
+                self._remove_keys(
+                    unique_query_keys=_original_unique_keys,
+                    searchable_query_keys=_original_searchable_keys,
+                )
 
-            # update the object with new data
-            for key, value in obj.to_dict(exclude_none=True).items():
-                if key == "id":
-                    # protected field
-                    continue
-                setattr(_original_obj, key, value)
+                # update the object with new data
+                for key, value in obj.to_dict(exclude_none=True).items():
+                    if key == "id":
+                        # protected field
+                        continue
+                    setattr(_original_obj, key, value)
 
-            # update data and keys
-            self._set_data_and_keys(
-                store_query_key=qk,
-                unique_query_keys=self.settings.unique_keys.with_obj(_original_obj),
-                searchable_query_keys=self.settings.searchable_keys.with_obj(
-                    _original_obj
-                ),
-                obj=_original_obj,
-            )
+                # update data and keys
+                self._set_data_and_keys(
+                    store_query_key=qk,
+                    unique_query_keys=self.settings.unique_keys.with_obj(_original_obj),
+                    searchable_query_keys=self.settings.searchable_keys.with_obj(
+                        _original_obj
+                    ),
+                    # has been updated
+                    obj=_original_obj,
+                )
+
+                # 🟡 TODO 28: Add locking in this transaction
+
+                # update the object with new data
+                for key, value in obj.to_dict(exclude_none=True).items():
+                    if key == "id":
+                        # protected field
+                        continue
+                    setattr(_original_obj, key, value)
+
+                return Ok(_original_obj)
+            else:
+                return Err(f"Failed to update obj {obj}, you have no permission")
 
-            return Ok(_original_obj)
         except Exception as e:
             return Err(f"Failed to update obj {obj} with error: {e}")
 
-    def _get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
+    def _get_all_from_store(
+        self, credentials: SyftVerifyKey, qks: QueryKeys
+    ) -> Result[List[SyftObject], str]:
         matches = []
         for qk in qks.all:
             if qk.value in self.data:
-                matches.append(self.data[qk.value])
+                if self.has_permission(
+                    ActionObjectREAD(uid=qk.value, credentials=credentials)
+                ):
+                    matches.append(self.data[qk.value])
         return Ok(matches)
 
-    def _delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
+    def create(self, obj: SyftObject) -> Result[SyftObject, str]:
+        pass
+
+    def _delete(
+        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission=False
+    ) -> Result[SyftSuccess, Err]:
         try:
-            _obj = self.data.pop(qk.value)
-            self._delete_unique_keys_for(_obj)
-            self._delete_search_keys_for(_obj)
-            return Ok(SyftSuccess(message="Deleted"))
+            if has_permission or self.has_permission(
+                ActionObjectWRITE(uid=qk.value, credentials=credentials)
+            ):
+                _obj = self.data.pop(qk.value)
+                self._delete_unique_keys_for(_obj)
+                self._delete_search_keys_for(_obj)
+                return Ok(SyftSuccess(message="Deleted"))
+            else:
+                return Err(
+                    f"Failed to delete with query key {qk}, you have no permission"
+                )
         except Exception as e:
             return Err(f"Failed to delete with query key {qk} with error: {e}")
 
     def _delete_unique_keys_for(self, obj: SyftObject) -> Result[SyftSuccess, str]:
         for _unique_ck in self.unique_cks:
             qk = _unique_ck.with_obj(obj)
             self.unique_keys[qk.key].pop(qk.value, None)
@@ -264,15 +463,15 @@
 
     def _delete_search_keys_for(self, obj: SyftObject) -> Result[SyftSuccess, str]:
         for _search_ck in self.searchable_cks:
             qk = _search_ck.with_obj(obj)
             self.searchable_keys[qk.key].pop(qk.value, None)
         return Ok(SyftSuccess(message="Deleted"))
 
-    def _get_keys_index(self, qks: QueryKeys) -> Result[Set[QueryKey], str]:
+    def _get_keys_index(self, qks: QueryKeys) -> Result[Set[Any], str]:
         try:
             # match AND
             subsets = []
             for qk in qks.all:
                 subset = {}
                 pk_key, pk_value = qk.key, qk.value
                 if pk_key not in self.unique_keys:
@@ -335,27 +534,32 @@
             subset = subsets.pop()
             for s in subsets:
                 subset = subset.intersection(s)
             return Ok(subset)
         except Exception as e:
             return Err(f"Failed to query with {qks}. {e}")
 
-    def _validate_partition_keys(
-        self, store_query_key: QueryKey, unique_query_keys: QueryKeys
+    def _check_partition_keys_unique(
+        self, unique_query_keys: QueryKeys
     ) -> UniqueKeyCheck:
+        # dont check the store key
+        qks = [
+            x
+            for x in unique_query_keys.all
+            if x.partition_key != self.settings.store_key
+        ]
         matches = []
-        qks = unique_query_keys.all
         for qk in qks:
             pk_key, pk_value = qk.key, qk.value
             if pk_key not in self.unique_keys:
                 raise Exception(
                     f"pk_key: {pk_key} not in unique_keys: {self.unique_keys.keys()}"
                 )
             ck_col = self.unique_keys[pk_key]
-            if pk_value in ck_col or ck_col.get(pk_value) == store_query_key.value:
+            if pk_value in ck_col:
                 matches.append(pk_key)
 
         if len(matches) == 0:
             return UniqueKeyCheck.EMPTY
         elif len(matches) == len(qks):
             return UniqueKeyCheck.MATCHES
 
@@ -388,10 +592,7 @@
                 # coerce the list of objects to strings for a single key
                 pk_value = " ".join([str(obj) for obj in pk_value])
 
             ck_col[pk_value].append(store_query_key.value)
             self.searchable_keys[pk_key] = ck_col
 
         self.data[store_query_key.value] = obj
-
-    def _all(self) -> Result[List[BaseStash.object_type], str]:
-        return Ok(list(self.data.values()))
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/linked_obj.py` & `syft-0.8.0b8/src/syft/core/node/new/linked_obj.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import Type
 from typing import Union
 
 # third party
 from typing_extensions import Self
 
 # relative
+from .context import AuthedServiceContext
+from .context import ChangeContext
 from .context import NodeServiceContext
 from .response import SyftError
 from .response import SyftSuccess
 from .serializable import serializable
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftObject
 from .uid import UID
@@ -42,15 +44,23 @@
         return context.node.get_service(self.service_type).resolve_link(
             context=context, linked_obj=self
         )
 
     def update_with_context(
         self, context: NodeServiceContext, obj: Any
     ) -> Union[SyftSuccess, SyftError]:
-        result = context.node.get_service(self.service_type).stash.update(obj)
+        if isinstance(context, AuthedServiceContext):
+            credentials = context.credentials
+        elif isinstance(context, ChangeContext):
+            credentials = context.approving_user_credentials
+        else:
+            return SyftError(message="wrong context passed")
+        result = context.node.get_service(self.service_type).stash.update(
+            credentials, obj
+        )
         if result.is_ok():
             return result
 
     @classmethod
     def from_obj(
         cls,
         obj: SyftObject,
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/locks.py` & `syft-0.8.0b8/src/syft/core/node/new/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/message_service.py` & `syft-0.8.0b8/src/syft/core/node/new/message_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,61 +34,64 @@
     @service_method(path="messages.send", name="send")
     def send(
         self, context: AuthedServiceContext, message: CreateMessage
     ) -> Union[Message, SyftError]:
         """Send a new message"""
 
         new_message = message.to(Message, context=context)
-        result = self.stash.set(new_message)
+        result = self.stash.set(context.credentials, new_message)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
     @service_method(path="messages.get_all", name="get_all")
     def get_all(self, context: AuthedServiceContext) -> Union[List[Message], SyftError]:
-        result = self.stash.get_all_inbox_for_verify_key(verify_key=context.credentials)
+        result = self.stash.get_all_inbox_for_verify_key(
+            context.credentials, verify_key=context.credentials
+        )
         if result.err():
             return SyftError(message=str(result.err()))
         messages = result.ok()
         return messages
 
     @service_method(path="messages.get_all_sent", name="outbox")
     def get_all_sent(
         self, context: AuthedServiceContext
     ) -> Union[List[Message], SyftError]:
-        result = self.stash.get_all_sent_for_verify_key(verify_key=context.credentials)
+        result = self.stash.get_all_sent_for_verify_key(
+            context.credentials, context.credentials
+        )
         if result.err():
             return SyftError(message=str(result.err()))
         messages = result.ok()
-        print(messages)
         return messages
 
     @service_method(
         path="messages.get_all_for_status",
         name="get_all_for_status",
     )
     def get_all_for_status(
         self,
         context: AuthedServiceContext,
         status: MessageStatus,
     ) -> Union[List[Message], SyftError]:
         result = self.stash.get_all_by_verify_key_for_status(
-            verify_key=context.credentials, status=status
+            context.credentials, verify_key=context.credentials, status=status
         )
         if result.err():
             return SyftError(message=str(result.err()))
         messages = result.ok()
         return messages
 
     @service_method(path="messages.mark_as_delivered", name="mark_as_delivered")
     def mark_as_delivered(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[Message, SyftError]:
         result = self.stash.update_message_status(
-            uid=uid, status=MessageStatus.DELIVERED
+            context.credentials, uid=uid, status=MessageStatus.DELIVERED
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         return result.ok()
 
     @service_method(path="messages.resolve_object", name="resolve_object")
@@ -99,15 +102,17 @@
         result = service.resolve_link(context=context, linked_obj=linked_obj)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
     @service_method(path="messages.clear", name="clear")
     def clear(self, context: AuthedServiceContext) -> Union[SyftError, SyftSuccess]:
-        result = self.stash.delete_all_for_verify_key(verify_key=context.credentials)
+        result = self.stash.delete_all_for_verify_key(
+            credentials=context.credentials, verify_key=context.credentials
+        )
         if result.is_ok():
             return SyftSuccess(message="All messages cleared !!")
         return SyftError(message=str(result.err()))
 
 
 TYPE_TO_SERVICE[Message] = MessageService
 SERVICE_TO_TYPES[MessageService].update({Message})
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/message_stash.py` & `syft-0.8.0b8/src/syft/core/node/new/message_stash.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,71 +33,78 @@
     object_type = Message
     settings: PartitionSettings = PartitionSettings(
         name=Message.__canonical_name__,
         object_type=Message,
     )
 
     def get_all_inbox_for_verify_key(
-        self, verify_key: SyftVerifyKey
+        self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey
     ) -> Result[List[Message], str]:
         qks = QueryKeys(
             qks=[
                 ToUserVerifyKeyPartitionKey.with_obj(verify_key),
             ]
         )
-        return self.get_all_for_verify_key(verify_key=verify_key, qks=qks)
+        return self.get_all_for_verify_key(
+            credentials=credentials, verify_key=verify_key, qks=qks
+        )
 
     def get_all_sent_for_verify_key(
-        self, verify_key: SyftVerifyKey
+        self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey
     ) -> Result[List[Message], str]:
         qks = QueryKeys(
             qks=[
                 FromUserVerifyKeyPartitionKey.with_obj(verify_key),
             ]
         )
-        return self.get_all_for_verify_key(verify_key=verify_key, qks=qks)
+        return self.get_all_for_verify_key(credentials, verify_key=verify_key, qks=qks)
 
     def get_all_for_verify_key(
-        self, verify_key: SyftVerifyKey, qks: QueryKeys
+        self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey, qks: QueryKeys
     ) -> Result[List[Message], str]:
         if isinstance(verify_key, str):
             verify_key = SyftVerifyKey.from_string(verify_key)
-        return self.query_all(qks=qks)
+        return self.query_all(credentials, qks=qks)
 
     def get_all_by_verify_key_for_status(
-        self, verify_key: SyftVerifyKey, status: MessageStatus
+        self,
+        credentials: SyftVerifyKey,
+        verify_key: SyftVerifyKey,
+        status: MessageStatus,
     ) -> Result[List[Message], str]:
         qks = QueryKeys(
             qks=[
                 ToUserVerifyKeyPartitionKey.with_obj(verify_key),
                 StatusPartitionKey.with_obj(status),
             ]
         )
-        return self.query_all(qks=qks)
+        return self.query_all(credentials, qks=qks)
 
     def update_message_status(
-        self, uid: UID, status: MessageStatus
+        self, credentials: SyftVerifyKey, uid: UID, status: MessageStatus
     ) -> Result[Message, str]:
-        result = self.get_by_uid(uid=uid)
+        result = self.get_by_uid(credentials, uid=uid)
         if result.is_err():
             return result.err()
 
         message = result.ok()
         if message is None:
             return Err(f"No message exists for id: {uid}")
         message.status = status
-        return self.update(obj=message)
+        return self.update(credentials, obj=message)
 
-    def delete_all_for_verify_key(self, verify_key: SyftVerifyKey) -> Result[bool, str]:
-        result = self.get_all_inbox_for_verify_key(verify_key=verify_key)
+    def delete_all_for_verify_key(
+        self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey
+    ) -> Result[bool, str]:
+        result = self.get_all_inbox_for_verify_key(credentials, verify_key=verify_key)
         # If result is an error then return the error
         if result.is_err():
             return result
 
         # get the list of messages
         messages = result.ok()
 
         for message in messages:
-            result = self.delete_by_uid(uid=message.id)
+            result = self.delete_by_uid(credentials, uid=message.id)
             if result.is_err():
                 return result
         return Ok(True)
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/messages.py` & `syft-0.8.0b8/src/syft/core/node/new/messages.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/metadata_service.py` & `syft-0.8.0b8/src/syft/core/node/new/metadata_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = MetadataStash(store=store)
 
     @service_method(path="metadata.get", name="get")
     def get(self, context: AuthedServiceContext) -> Result[Ok, Err]:
         """Get Metadata"""
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             metadata = result.ok()
             # check if the metadata list is empty
             if len(metadata) == 0:
                 return SyftError(message="No metadata found")
             result = metadata[0]
             return Ok(result)
@@ -41,32 +41,32 @@
             return SyftError(message=result.err())
 
     @service_method(path="metadata.set", name="set")
     def set(
         self, context: AuthedServiceContext, metadata: NodeMetadata
     ) -> Result[Ok, Err]:
         """Set a new the Node Metadata"""
-        result = self.stash.set(metadata)
+        result = self.stash.set(context.credentials, metadata)
         if result.is_ok():
             return result
         else:
             return SyftError(message=result.err())
 
     @service_method(path="metadata.update", name="update")
     def update(
         self, context: AuthedServiceContext, metadata: NodeMetadataUpdate
     ) -> Result[Ok, Err]:
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             current_metadata = result.ok()
             if len(current_metadata) > 0:
                 new_metadata = current_metadata[0].copy(
                     update=metadata.dict(exclude_unset=True)
                 )
-                update_result = self.stash.update(new_metadata)
+                update_result = self.stash.update(context.credentials, new_metadata)
                 if update_result.is_ok():
                     return result
                 else:
                     return SyftError(message=update_result.err())
             else:
                 return SyftError(message="No metadata found")
         else:
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/mongo_client.py` & `syft-0.8.0b8/src/syft/core/node/new/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/mongo_codecs.py` & `syft-0.8.0b8/src/syft/core/node/new/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/mongo_document_store.py` & `syft-0.8.0b8/src/syft/core/node/new/mongo_document_store.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from pymongo.collection import Collection as MongoCollection
 from pymongo.errors import DuplicateKeyError
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
+from .action_permissions import ActionObjectPermission
+from .action_permissions import ActionObjectREAD
+from .action_permissions import ActionObjectWRITE
+from .credentials import SyftVerifyKey
 from .document_store import DocumentStore
 from .document_store import QueryKey
 from .document_store import QueryKeys
 from .document_store import StoreConfig
 from .document_store import StorePartition
 from .locks import LockingConfig
 from .locks import NoLockingConfig
@@ -186,107 +190,147 @@
             if res.is_err():
                 return res
 
         return Ok(self._collection)
 
     def _set(
         self,
+        credentials: SyftVerifyKey,
         obj: SyftObject,
+        add_permissions: Optional[List[ActionObjectPermission]] = None,
         ignore_duplicates: bool = False,
     ) -> Result[SyftObject, str]:
-        storage_obj = obj.to(self.storage_type)
+        write_permission = ActionObjectWRITE(uid=obj.id, credentials=credentials)
+        can_write = self.has_permission(write_permission)
+        if can_write:
+            storage_obj = obj.to(self.storage_type)
+
+            collection_status = self.collection
+            if collection_status.is_err():
+                return collection_status
+            collection = collection_status.ok()
 
-        collection_status = self.collection
-        if collection_status.is_err():
-            return collection_status
-        collection = collection_status.ok()
-
-        if ignore_duplicates:
-            collection = collection.with_options(write_concern=WriteConcern(w=0))
-        try:
-            collection.insert_one(storage_obj)
-        except DuplicateKeyError as e:
-            return Err(f"Duplicate Key Error for {obj}: {e}")
-
-        return Ok(obj)
+            if ignore_duplicates:
+                collection = collection.with_options(write_concern=WriteConcern(w=0))
+            try:
+                collection.insert_one(storage_obj)
+            except DuplicateKeyError as e:
+                return Err(f"Duplicate Key Error for {obj}: {e}")
+            if add_permissions is not None:
+                pass
+                # TODO: update permissions
+            return Ok(obj)
+        else:
+            return Err(f"No permission to write object with id {obj.id}")
 
-    def _update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
+    def _update(
+        self,
+        credentials: SyftVerifyKey,
+        qk: QueryKey,
+        obj: SyftObject,
+        has_permission: bool = False,
+    ) -> Result[SyftObject, str]:
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
         # TODO: optimize the update. The ID should not be overwritten,
         # but the qk doesn't necessarily have to include the `id` field either.
 
-        prev_obj_status = self._get_all_from_store(QueryKeys(qks=[qk]))
+        prev_obj_status = self._get_all_from_store(credentials, QueryKeys(qks=[qk]))
         if prev_obj_status.is_err():
             return Err(f"No object found with query key: {qk}")
 
         prev_obj = prev_obj_status.ok()
         if len(prev_obj) == 0:
             return Err(f"Missing values for query key: {qk}")
 
-        # we don't want to overwrite Mongo's "id_" or Syft's "id" on update
-        obj_id = obj["id"]
+        prev_obj = prev_obj[0]
+        if has_permission or self.has_permission(
+            ActionObjectWRITE(uid=prev_obj.id, credentials=credentials)
+        ):
+            # we don't want to overwrite Mongo's "id_" or Syft's "id" on update
+            obj_id = obj["id"]
 
-        # Set ID to the updated object value
-        setattr(obj, "id", prev_obj[0]["id"])
+            # Set ID to the updated object value
+            setattr(obj, "id", prev_obj["id"])
 
-        # Create the Mongo object
-        storage_obj = obj.to(self.storage_type)
+            # Create the Mongo object
+            storage_obj = obj.to(self.storage_type)
 
-        # revert the ID
-        setattr(obj, "id", obj_id)
+            # revert the ID
+            setattr(obj, "id", obj_id)
 
-        try:
-            collection.update_one(filter=qk.as_dict_mongo, update={"$set": storage_obj})
-        except Exception as e:
-            return Err(f"Failed to update obj: {obj} with qk: {qk}. Error: {e}")
+            try:
+                collection.update_one(
+                    filter=qk.as_dict_mongo, update={"$set": storage_obj}
+                )
+            except Exception as e:
+                return Err(f"Failed to update obj: {obj} with qk: {qk}. Error: {e}")
 
-        return Ok(obj)
+            return Ok(obj)
+        else:
+            return Err(f"Failed to update obj {obj}, you have no permission")
 
     def _find_index_or_search_keys(
-        self, index_qks: QueryKeys, search_qks: QueryKeys
+        self, credentials: SyftVerifyKey, index_qks: QueryKeys, search_qks: QueryKeys
     ) -> Result[List[SyftObject], str]:
         # TODO: pass index as hint to find method
         qks = QueryKeys(qks=(index_qks.all + search_qks.all))
-        return self._get_all_from_store(qks=qks)
+        return self._get_all_from_store(credentials=credentials, qks=qks)
 
-    def _get_all_from_store(self, qks: QueryKeys) -> Result[List[SyftObject], str]:
+    def _get_all_from_store(
+        self, credentials: SyftVerifyKey, qks: QueryKeys
+    ) -> Result[List[SyftObject], str]:
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
         storage_objs = collection.find(filter=qks.as_dict_mongo)
         syft_objs = []
         for storage_obj in storage_objs:
             obj = self.storage_type(storage_obj)
             transform_context = TransformContext(output={}, obj=obj)
             syft_objs.append(obj.to(self.settings.object_type, transform_context))
-        return Ok(syft_objs)
 
-    def _delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
+        # TODO: maybe do this in loop before this
+        res = []
+        for s in syft_objs:
+            if self.has_permission(ActionObjectREAD(uid=s.id, credentials=credentials)):
+                res.append(s)
+        return Ok(res)
+
+    def _delete(
+        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission: bool = False
+    ) -> Result[SyftSuccess, Err]:
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
-        qks = QueryKeys(qks=qk)
-        result = collection.delete_one(filter=qks.as_dict_mongo)
+        if has_permission or self.has_permission(
+            ActionObjectWRITE(uid=qk.value, credentials=credentials)
+        ):
+            qks = QueryKeys(qks=qk)
+            result = collection.delete_one(filter=qks.as_dict_mongo)
 
-        if result.deleted_count == 1:
-            return Ok(SyftSuccess(message="Deleted"))
+            if result.deleted_count == 1:
+                return Ok(SyftSuccess(message="Deleted"))
 
         return Err(f"Failed to delete object with qk: {qk}")
 
-    def _all(self):
+    def has_permission(self, permission: ActionObjectPermission) -> bool:
+        # TODO: implement
+        return True
+
+    def _all(self, credentials: SyftVerifyKey):
         qks = QueryKeys(qks=())
-        return self._get_all_from_store(qks=qks)
+        return self._get_all_from_store(credentials=credentials, qks=qks)
 
     def __len__(self):
         collection_status = self.collection
         if collection_status.is_err():
             return 0
         collection = collection_status.ok()
         return collection.count_documents(filter={})
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/network_service.py` & `syft-0.8.0b8/src/syft/core/node/new/network_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,40 +245,49 @@
     settings: PartitionSettings = PartitionSettings(
         name=NodePeer.__canonical_name__, object_type=NodePeer
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
-    def get_by_name(self, name: str) -> Result[Optional[NodePeer], str]:
+    def get_by_name(
+        self, credentials: SyftVerifyKey, name: str
+    ) -> Result[Optional[NodePeer], str]:
         qks = QueryKeys(qks=[NamePartitionKey.with_obj(name)])
-        return self.query_one(qks=qks)
+        return self.query_one(credentials=credentials, qks=qks)
 
-    def update(self, peer: NodePeer) -> Result[NodePeer, str]:
-        return self.check_type(peer, NodePeer).and_then(super().update)
+    def update(
+        self, credentials: SyftVerifyKey, peer: NodePeer
+    ) -> Result[NodePeer, str]:
+        valid = self.check_type(peer, NodePeer)
+        if valid.is_err():
+            return SyftError(message=valid.err())
+        return super().update(credentials, peer)
 
-    def update_peer(self, peer: NodePeer) -> Result[NodePeer, str]:
+    def update_peer(
+        self, credentials: SyftVerifyKey, peer: NodePeer
+    ) -> Result[NodePeer, str]:
         valid = self.check_type(peer, NodePeer)
         if valid.is_err():
             return SyftError(message=valid.err())
         existing = self.get_by_uid(peer.id)
         if existing.is_ok() and existing.ok():
             existing = existing.ok()
             existing.update_routes(peer.node_routes)
             result = self.update(existing)
             return result
         else:
-            result = self.set(peer)
+            result = self.set(credentials, peer)
             return result
 
     def get_for_verify_key(
-        self, verify_key: SyftVerifyKey
+        self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey
     ) -> Result[NodePeer, SyftError]:
         qks = QueryKeys(qks=[VerifyKeyPartitionKey.with_obj(verify_key)])
-        return self.query_one(qks)
+        return self.query_one(credentials, qks)
 
 
 @instrument
 @serializable()
 class NetworkService(AbstractService):
     store: DocumentStore
     stash: NetworkStash
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/node.py` & `syft-0.8.0b8/src/syft/core/node/new/node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/node_metadata.py` & `syft-0.8.0b8/src/syft/core/node/new/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/numpy.py` & `syft-0.8.0b8/src/syft/core/node/new/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/pandas.py` & `syft-0.8.0b8/src/syft/core/node/new/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/policy.py` & `syft-0.8.0b8/src/syft/core/node/new/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/policy_service.py` & `syft-0.8.0b8/src/syft/core/node/new/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/project.py` & `syft-0.8.0b8/src/syft/core/node/new/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/project_service.py` & `syft-0.8.0b8/src/syft/core/node/new/project_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 
     @service_method(path="project.submit", name="submit", roles=GUEST_ROLE_LEVEL)
     def submit(
         self, context: AuthedServiceContext, project: ProjectSubmit
     ) -> Union[SyftSuccess, SyftError]:
         """Submit a Project"""
         try:
-            result = self.stash.set(project.to(Project, context=context))
+            result = self.stash.set(
+                context.credentials, project.to(Project, context=context)
+            )
 
             if result.is_ok():
                 result = result.ok()
                 link = LinkedObject.with_context(result, context=context)
                 admin_verify_key = context.node.get_service_method(
                     UserService.admin_verify_key
                 )
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/project_stash.py` & `syft-0.8.0b8/src/syft/core/node/new/user_policy_stash.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 # stdlib
 from typing import List
 
 # third party
 from result import Result
 
 # relative
-from ....telemetry import instrument
 from .credentials import SyftVerifyKey
 from .document_store import BaseUIDStoreStash
-from .document_store import PartitionKey
+from .document_store import DocumentStore
 from .document_store import PartitionSettings
 from .document_store import QueryKeys
-from .project import Project
-from .request import Request
-from .response import SyftError
+from .policy import PolicyUserVerifyKeyPartitionKey
+from .policy import UserPolicy
 from .serializable import serializable
 
-ProjectUserVerifyKeyPartitionKey = PartitionKey(
-    key="user_verify_key", type_=SyftVerifyKey
-)
 
-
-@instrument
 @serializable()
-class ProjectStash(BaseUIDStoreStash):
-    object_type = Project
+class UserPolicyStash(BaseUIDStoreStash):
+    object_type = UserPolicy
     settings: PartitionSettings = PartitionSettings(
-        name=Project.__canonical_name__, object_type=Project
+        name=UserPolicy.__canonical_name__, object_type=UserPolicy
     )
 
-    def get_all_for_verify_key(
-        self, verify_key: ProjectUserVerifyKeyPartitionKey
-    ) -> Result[List[Request], SyftError]:
-        if isinstance(verify_key, str):
-            verify_key = SyftVerifyKey.from_string(verify_key)
-        qks = QueryKeys(qks=[ProjectUserVerifyKeyPartitionKey.with_obj(verify_key)])
-        return self.query_all(qks=qks)
+    def __init__(self, store: DocumentStore) -> None:
+        super().__init__(store=store)
+
+    def get_all_by_user_verify_key(
+        self, credentials: SyftVerifyKey, user_verify_key: SyftVerifyKey
+    ) -> Result[List[UserPolicy], str]:
+        qks = QueryKeys(qks=[PolicyUserVerifyKeyPartitionKey.with_obj(user_verify_key)])
+        return self.query_one(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/queue_stash.py` & `syft-0.8.0b8/src/syft/core/node/new/queue_stash.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # stdlib
 from typing import Any
+from typing import List
 from typing import Optional
 from typing import Union
 
 # third party
 from result import Ok
 from result import Result
 
 # relative
 from ....telemetry import instrument
+from .action_permissions import ActionObjectPermission
 from .api import APIRegistry
 from .api import SyftAPICall
+from .credentials import SyftVerifyKey
 from .document_store import BaseStash
 from .document_store import DocumentStore
 from .document_store import PartitionSettings
 from .document_store import QueryKeys
 from .document_store import UIDPartitionKey
+from .response import SyftError
 from .response import SyftNotReady
 from .response import SyftSuccess
 from .serializable import serializable
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftObject
 from .uid import UID
 
@@ -65,36 +69,58 @@
     settings: PartitionSettings = PartitionSettings(
         name=QueueItem.__canonical_name__, object_type=QueueItem
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
-    def set_result(self, item: QueueItem) -> Result[Optional[QueueItem], str]:
+    def set_result(
+        self,
+        credentials: SyftVerifyKey,
+        item: QueueItem,
+        add_permissions: Optional[List[ActionObjectPermission]] = None,
+    ) -> Result[Optional[QueueItem], str]:
         if item.resolved:
-            return self.check_type(item, self.object_type).and_then(super().set)
+            valid = self.check_type(item, self.object_type)
+            if valid.is_err():
+                return SyftError(message=valid.err())
+            return super().set(credentials, item, add_permissions)
         return None
 
-    def set_placeholder(self, item: QueueItem) -> Result[QueueItem, str]:
+    def set_placeholder(
+        self,
+        credentials: SyftVerifyKey,
+        item: QueueItem,
+        add_permissions: Optional[List[ActionObjectPermission]] = None,
+    ) -> Result[QueueItem, str]:
         # 🟡 TODO 36: Needs distributed lock
         if not item.resolved:
             exists = self.get_by_uid(item.id)
             if exists.is_ok() and exists.ok() is None:
-                return self.check_type(item, self.object_type).and_then(super().set)
+                valid = self.check_type(item, self.object_type)
+                if valid.is_err():
+                    return SyftError(message=valid.err())
+                return super().set(credentials, item, add_permissions)
         return item
 
-    def get_by_uid(self, uid: UID) -> Result[Optional[QueueItem], str]:
+    def get_by_uid(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Result[Optional[QueueItem], str]:
         qks = QueryKeys(qks=[UIDPartitionKey.with_obj(uid)])
-        item = self.query_one(qks=qks)
+        item = self.query_one(credentials=credentials, qks=qks)
         return item
 
-    def pop(self, uid: UID) -> Result[Optional[QueueItem], str]:
-        item = self.get_by_uid(uid)
-        self.delete_by_uid(uid)
+    def pop(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Result[Optional[QueueItem], str]:
+        item = self.get_by_uid(credentials=credentials, uid=uid)
+        self.delete_by_uid(credentials=credentials, uid=uid)
         return item
 
-    def delete_by_uid(self, uid: UID) -> Result[SyftSuccess, str]:
+    def delete_by_uid(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Result[SyftSuccess, str]:
         qk = UIDPartitionKey.with_obj(uid)
-        result = super().delete(qk=qk)
+        result = super().delete(credentials=credentials, qk=qk)
         if result.is_ok():
             return Ok(SyftSuccess(message=f"ID: {uid} deleted"))
         return result
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/recursive.py` & `syft-0.8.0b8/src/syft/core/node/new/recursive.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,18 @@
     bytes_value = b""
     for value in capnp_list:
         bytes_value += value
     return bytes_value
 
 
 def rs_object2proto(self: Any) -> _DynamicStructBuilder:
+    is_type = False
+    if isinstance(self, type):
+        is_type = True
+
     msg = recursive_scheme.new_message()
     fqn = get_fully_qualified_name(self)
     if fqn not in TYPE_BANK:
         raise Exception(f"{fqn} not in TYPE_BANK")
 
     msg.fullyQualifiedName = fqn
     (
@@ -130,15 +134,15 @@
         serialize,
         deserialize,
         attribute_list,
         serde_overrides,
         cls,
     ) = TYPE_BANK[fqn]
 
-    if nonrecursive:
+    if nonrecursive or is_type:
         if serialize is None:
             raise Exception(
                 f"Cant serialize {type(self)} nonrecursive without serialize."
             )
         chunk_bytes(serialize(self), "nonrecursiveBlob", msg)
         return msg
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/recursive_primitives.py` & `syft-0.8.0b8/src/syft/core/node/new/recursive_primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,14 +224,20 @@
 recursive_serde_register(
     set,
     serialize=serialize_iterable,
     deserialize=functools.partial(deserialize_iterable, set),
 )
 
 recursive_serde_register(
+    frozenset,
+    serialize=serialize_iterable,
+    deserialize=functools.partial(deserialize_iterable, frozenset),
+)
+
+recursive_serde_register(
     complex,
     serialize=lambda x: serialize_iterable((x.real, x.imag)),
     deserialize=lambda x: complex(*deserialize_iterable(tuple, x)),
 )
 
 recursive_serde_register(
     range,
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/request.py` & `syft-0.8.0b8/src/syft/core/node/new/request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/request_service.py` & `syft-0.8.0b8/src/syft/core/node/new/request_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 # third party
 from result import Err
 from result import Ok
 
 # relative
 from ....telemetry import instrument
+from .action_permissions import ActionObjectPermission
+from .action_permissions import ActionPermission
 from .context import AuthedServiceContext
 from .document_store import DocumentStore
 from .linked_obj import LinkedObject
 from .message_service import CreateMessage
 from .message_service import Message
 from .message_service import MessageService
 from .request import Request
@@ -44,15 +46,24 @@
         self,
         context: AuthedServiceContext,
         request: SubmitRequest,
         send_message: bool = True,
     ) -> Union[Request, SyftError]:
         """Submit a Request"""
         try:
-            result = self.stash.set(request.to(Request, context=context))
+            req = request.to(Request, context=context)
+            result = self.stash.set(
+                context.credentials,
+                req,
+                add_permissions=[
+                    ActionObjectPermission(
+                        uid=req.id, permission=ActionPermission.ALL_READ
+                    ),
+                ],
+            )
             if result.is_ok():
                 request = result.ok()
                 link = LinkedObject.with_context(request, context=context)
                 admin_verify_key = context.node.get_service_method(
                     UserService.admin_verify_key
                 )
 
@@ -78,15 +89,15 @@
             return result.ok()
         except Exception as e:
             print("Failed to submit Request", e)
             raise e
 
     @service_method(path="request.get_all", name="get_all")
     def get_all(self, context: AuthedServiceContext) -> Union[List[Request], SyftError]:
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_err():
             return SyftError(message=str(result.err()))
         requests = result.ok()
         return requests
 
     @service_method(path="request.get_all_for_status", name="get_all_for_status")
     def get_all_for_status(
@@ -98,15 +109,15 @@
         requests = result.ok()
         return requests
 
     @service_method(path="request.apply", name="apply")
     def apply(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
-        request = self.stash.get_by_uid(uid)
+        request = self.stash.get_by_uid(context.credentials, uid)
         if request.is_ok():
             request = request.ok()
             result = request.apply(context=context)
             return result.value
         return request.value
 
     @service_method(path="request.revert", name="revert")
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/request_stash.py` & `syft-0.8.0b8/src/syft/core/node/new/request_stash.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,17 +26,21 @@
 class RequestStash(BaseUIDStoreStash):
     object_type = Request
     settings: PartitionSettings = PartitionSettings(
         name=Request.__canonical_name__, object_type=Request
     )
 
     def get_all_for_verify_key(
-        self, verify_key: RequestingUserVerifyKeyPartitionKey
+        self,
+        credentials: SyftVerifyKey,
+        verify_key: SyftVerifyKey,
     ) -> Result[List[Request], str]:
         if isinstance(verify_key, str):
             verify_key = SyftVerifyKey.from_string(verify_key)
         qks = QueryKeys(qks=[RequestingUserVerifyKeyPartitionKey.with_obj(verify_key)])
-        return self.query_all(qks=qks)
+        return self.query_all(credentials=credentials, qks=qks)
 
-    def get_all_for_status(self, status: RequestStatus) -> Result[List[Request], str]:
+    def get_all_for_status(
+        self, credentials: SyftVerifyKey, status: RequestStatus
+    ) -> Result[List[Request], str]:
         qks = QueryKeys(qks=[StatusPartitionKey.with_obj(status)])
-        return self.query_all(qks=qks)
+        return self.query_all(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/response.py` & `syft-0.8.0b8/src/syft/core/node/new/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/serializable.py` & `syft-0.8.0b8/src/syft/core/node/new/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/service.py` & `syft-0.8.0b8/src/syft/core/node/new/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 # third party
 from result import Ok
 from result import OkErr
 
 # relative
 from .context import AuthedServiceContext
+from .context import ChangeContext
 from .linked_obj import LinkedObject
 from .response import SyftError
 from .serializable import serializable
 from .signature import Signature
 from .signature import signature_remove_context
 from .signature import signature_remove_self
 from .syft_object import SyftBaseObject
@@ -41,15 +42,22 @@
 class AbstractService:
     node: AbstractNode
     node_uid: UID
 
     def resolve_link(
         self, context: AuthedServiceContext, linked_obj: LinkedObject
     ) -> Union[Any, SyftError]:
-        obj = self.stash.get_by_uid(uid=linked_obj.object_uid)
+        if isinstance(context, AuthedServiceContext):
+            credentials = context.credentials
+        elif isinstance(context, ChangeContext):
+            credentials = context.approving_user_credentials
+        else:
+            return SyftError(message="wrong context passed")
+
+        obj = self.stash.get_by_uid(credentials, uid=linked_obj.object_uid)
         if isinstance(obj, OkErr) and obj.is_ok():
             obj = obj.ok()
         if hasattr(obj, "node_uid"):
             obj.node_uid = context.node.id
         if not isinstance(obj, OkErr):
             obj = Ok(obj)
         return obj
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/signature.py` & `syft-0.8.0b8/src/syft/core/node/new/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/sqlite_document_store.py` & `syft-0.8.0b8/src/syft/core/node/new/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/syft_object.py` & `syft-0.8.0b8/src/syft/core/node/new/syft_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 from pydantic.fields import Undefined
 from typeguard import check_type
 
 # relative
 from ....util import aggressive_set_attr
 from .credentials import SyftVerifyKey
 from .deserialize import _deserialize as deserialize
+from .recursive_primitives import recursive_serde_register_type
 from .serialize import _serialize as serialize
+from .syft_metaclass import Empty
+from .syft_metaclass import PartialModelMetaclass
 from .uid import UID
 from .util import full_name_with_qualname
 from .util import get_qualname_for
 
 SYFT_OBJECT_VERSION_1 = 1
 SYFT_OBJECT_VERSION_2 = 2
 
@@ -288,26 +291,30 @@
 
     # transform from one supported type to another
     def to(self, projection: type, context: Optional[Context] = None) -> Any:
         # 🟡 TODO 19: Could we do an mro style inheritence conversion? Risky?
         transform = SyftObjectRegistry.get_transform(type(self), projection)
         return transform(self, context)
 
-    def to_dict(self, exclude_none: bool = False) -> Dict[str, Any]:
+    def to_dict(
+        self, exclude_none: bool = False, exclude_empty: bool = False
+    ) -> Dict[str, Any]:
         warnings.warn(
             "`SyftObject.to_dict` is deprecated and will be removed in a future version",
             PendingDeprecationWarning,
         )
         # 🟡 TODO 18: Remove to_dict and replace usage with transforms etc
-        if not exclude_none:
+        if not exclude_none and not exclude_empty:
             return dict(self)
         else:
             new_dict = {}
             for k, v in dict(self).items():
-                if v is not None:
+                if exclude_empty and v is not Empty:
+                    new_dict[k] = v
+                if exclude_none and v is not None:
                     new_dict[k] = v
             return new_dict
 
     def __post_init__(self) -> None:
         pass
 
     def _syft_set_validate_private_attrs_(self, **kwargs):
@@ -440,7 +447,42 @@
 
 
 class StorableObjectType:
     def to(self, projection: type, context: Optional[Context] = None) -> Any:
         # 🟡 TODO 19: Could we do an mro style inheritence conversion? Risky?
         transform = SyftObjectRegistry.get_transform(type(self), projection)
         return transform(self, context)
+
+
+class PartialSyftObject(SyftObject, metaclass=PartialModelMetaclass):
+    """Syft Object to which partial arguments can be provided."""
+
+    __canonical_name__ = "PartialSyftObject"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    def __init__(self, *args, **kwargs) -> None:
+        # Filter out Empty values from args and kwargs
+        args_, kwargs_ = (), {}
+        for arg in args:
+            if arg is not Empty:
+                args_.append(arg)
+
+        for key, val in kwargs.items():
+            if val is not Empty:
+                kwargs_[key] = val
+
+        super().__init__(*args_, **kwargs_)
+
+        fields_with_default = set()
+        for _field_name, _field in self.__fields__.items():
+            if _field.default or _field.allow_none:
+                fields_with_default.add(_field_name)
+
+        # Exclude unset fields
+        unset_fields = set(self.__fields__) - set(self.__fields_set__)
+
+        empty_fields = unset_fields - fields_with_default
+        for field_name in empty_fields:
+            self.__dict__[field_name] = Empty
+
+
+recursive_serde_register_type(PartialSyftObject)
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/test_service.py` & `syft-0.8.0b8/src/syft/core/node/new/test_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/third_party.py` & `syft-0.8.0b8/src/syft/core/node/new/third_party.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 
 # result Ok and Err
 recursive_serde_register(Ok, serialize_attrs=["_value"])
 recursive_serde_register(Err, serialize_attrs=["_value"])
 
 recursive_serde_register_type(pydantic.main.ModelMetaclass)
-recursive_serde_register_type(Result, serialize_attrs=["_value"])
+recursive_serde_register(Result)
 
 # exceptions
 recursive_serde_register(cls=TypeError)
 
 # mongo collection
 recursive_serde_register_type(Collection)
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/transforms.py` & `syft-0.8.0b8/src/syft/core/node/new/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/twin_object.py` & `syft-0.8.0b8/src/syft/core/node/new/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/uid.py` & `syft-0.8.0b8/src/syft/core/node/new/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/unparse.py` & `syft-0.8.0b8/src/syft/core/node/new/unparse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/user.py` & `syft-0.8.0b8/src/syft/core/node/new/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pydantic
 from pydantic.networks import EmailStr
 
 # relative
 from .credentials import SyftSigningKey
 from .credentials import SyftVerifyKey
 from .serializable import serializable
+from .syft_object import PartialSyftObject
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftObject
 from .transforms import TransformContext
 from .transforms import drop
 from .transforms import generate_id
 from .transforms import keep
 from .transforms import make_set_default
@@ -46,15 +47,15 @@
     hashed_password: Optional[str]
     salt: Optional[str]
     signing_key: Optional[SyftSigningKey]
     verify_key: Optional[SyftVerifyKey]
     role: Optional[ServiceRole]
     institution: Optional[str]
     website: Optional[str] = None
-    created_at: Optional[str]
+    created_at: Optional[str] = None
 
     # serde / storage rules
     __attr_searchable__ = ["name", "email", "verify_key", "role"]
     __attr_unique__ = ["email", "signing_key", "verify_key"]
     __attr_repr_cols__ = ["name", "email"]
 
 
@@ -92,67 +93,68 @@
     return checkpw(
         password=password.encode("utf-8"),
         hashed_password=hashed_password.encode("utf-8"),
     )
 
 
 @serializable()
-class UserUpdate(SyftObject):
+class UserUpdate(PartialSyftObject):
     __canonical_name__ = "UserUpdate"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    id: Optional[UID] = None
-
-    @pydantic.validator("email", pre=True, always=True)
-    def make_email(cls, v: EmailStr) -> EmailStr:
+    @pydantic.validator("email", pre=True)
+    def make_email(cls, v: EmailStr) -> Optional[EmailStr]:
         return EmailStr(v) if v is not None else v
 
-    email: Optional[EmailStr]
-    name: Optional[str]
-    role: Optional[ServiceRole] = None  # make sure role cant be set without uid
-    password: Optional[str] = None
-    password_verify: Optional[str] = None
-    verify_key: Optional[SyftVerifyKey] = None
-    institution: Optional[str] = None
-    website: Optional[str] = None
+    email: EmailStr
+    name: str
+    role: ServiceRole  # make sure role cant be set without uid
+    password: str
+    password_verify: str
+    verify_key: SyftVerifyKey
+    institution: str
+    website: str
 
 
 @serializable()
 class UserCreate(UserUpdate):
     __canonical_name__ = "UserCreate"
     __version__ = SYFT_OBJECT_VERSION_1
 
     email: EmailStr
     name: str
     role: Optional[ServiceRole] = None  # make sure role cant be set without uid
     password: str
     password_verify: str
-    verify_key: Optional[SyftVerifyKey] = None
-    institution: Optional[str] = None
-    website: Optional[str] = None
+    verify_key: Optional[SyftVerifyKey]
+    institution: Optional[str]
+    website: Optional[str]
 
     __attr_repr_cols__ = ["name", "email"]
 
 
 @serializable()
-class UserSearch(SyftObject):
+class UserSearch(PartialSyftObject):
     __canonical_name__ = "UserSearch"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    id: Optional[UID]
-    email: Optional[EmailStr]
-    verify_key: Optional[SyftVerifyKey]
-    name: Optional[str]
+    id: UID
+    email: EmailStr
+    verify_key: SyftVerifyKey
+    name: str
 
 
 @serializable()
-class UserView(UserUpdate):
+class UserView(SyftObject):
     __canonical_name__ = "UserView"
     __version__ = SYFT_OBJECT_VERSION_1
 
+    email: EmailStr
+    name: str
+
     __attr_repr_cols__ = ["name", "email"]
 
 
 @transform(UserUpdate, User)
 def user_update_to_user() -> List[Callable]:
     return [
         validate_email,
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/user_code.py` & `syft-0.8.0b8/src/syft/core/node/new/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/user_code_parse.py` & `syft-0.8.0b8/src/syft/core/node/new/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/user_code_service.py` & `syft-0.8.0b8/src/syft/core/node/new/user_code_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,27 +46,26 @@
         self.stash = UserCodeStash(store=store)
 
     @service_method(path="code.submit", name="submit")
     def submit(
         self, context: AuthedServiceContext, code: SubmitUserCode
     ) -> Union[UserCode, SyftError]:
         """Add User Code"""
-        user_code = code.to(UserCode, context=context)
-        result = self.stash.set(user_code)
+        result = self.stash.set(context.credentials, code.to(UserCode, context=context))
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="User Code Submitted")
 
     def _code_execution(
         self,
         context: AuthedServiceContext,
         code: SubmitUserCode,
     ):
         user_code = code.to(UserCode, context=context)
-        result = self.stash.set(user_code)
+        result = self.stash.set(context.credentials, user_code)
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         linked_obj = LinkedObject.from_obj(user_code, node_uid=context.node.id)
 
         CODE_EXECUTE = UserCodeStatusChange(
             value=UserCodeStatus.EXECUTE, linked_obj=linked_obj
@@ -92,54 +91,54 @@
         return self._code_execution(context=context, code=code)
 
     @service_method(path="code.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
     def get_all(
         self, context: AuthedServiceContext
     ) -> Union[List[UserCode], SyftError]:
         """Get a Dataset"""
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             return result.ok()
         return SyftError(message=result.err())
 
     @service_method(path="code.get_by_id", name="get_by_id")
     def get_by_uid(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
         """Get a User Code Item"""
-        result = self.stash.get_by_uid(uid=uid)
+        result = self.stash.get_by_uid(context.credentials, uid=uid)
         if result.is_ok():
             user_code = result.ok()
-            if user_code.input_policy_state:
+            if user_code and user_code.input_policy_state:
                 # TODO replace with LinkedObject Context
                 user_code.node_uid = context.node.id
             return user_code
         return SyftError(message=result.err())
 
     @service_method(path="code.get_all_for_user", name="get_all_for_user")
     def get_all_for_user(
         self, context: AuthedServiceContext
     ) -> Union[SyftSuccess, SyftError]:
         """Get All User Code Items for User's VerifyKey"""
         # TODO: replace with incoming user context and key
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             return result.ok()
         return SyftError(message=result.err())
 
     def update_code_state(
         self, context: AuthedServiceContext, code_item: UserCode
     ) -> Union[SyftSuccess, SyftError]:
-        result = self.stash.update(code_item)
+        result = self.stash.update(context.credentials, code_item)
         if result.is_ok():
             return SyftSuccess(message="Code State Updated")
         return SyftError(message="Unable to Update Code State")
 
-    def load_user_code(self) -> None:
-        result = self.stash.get_all()
+    def load_user_code(self, context: AuthedServiceContext) -> None:
+        result = self.stash.get_all(credentials=context.credentials)
         if result.is_ok():
             user_code_items = result.ok()
             for user_code in user_code_items:
                 if user_code.status.approved:
                     if isinstance(user_code.input_policy_type, UserPolicy):
                         load_policy_code(user_code.input_policy_type)
                     if isinstance(user_code.output_policy_type, UserPolicy):
@@ -148,15 +147,15 @@
     @service_method(path="code.call", name="call", roles=GUEST_ROLE_LEVEL)
     def call(
         self, context: AuthedServiceContext, uid: UID, **kwargs: Any
     ) -> Union[SyftSuccess, SyftError]:
         """Call a User Code Function"""
         try:
             filtered_kwargs = filter_kwargs(kwargs)
-            result = self.stash.get_by_uid(uid=uid)
+            result = self.stash.get_by_uid(context.credentials, uid=uid)
             if not result.is_ok():
                 return SyftError(message=result.err())
 
             # Unroll variables
             code_item = result.ok()
             status = code_item.status
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/user_code_stash.py` & `syft-0.8.0b8/src/syft/core/node/new/user_code_stash.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,15 +26,17 @@
         name=UserCode.__canonical_name__, object_type=UserCode
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
     def get_all_by_user_verify_key(
-        self, user_verify_key: SyftVerifyKey
+        self, credentials: SyftVerifyKey, user_verify_key: SyftVerifyKey
     ) -> Result[List[UserCode], str]:
         qks = QueryKeys(qks=[UserVerifyKeyPartitionKey.with_obj(user_verify_key)])
-        return self.query_one(qks=qks)
+        return self.query_one(credentials=credentials, qks=qks)
 
-    def get_by_code_hash(self, code_hash: int) -> Result[Optional[UserCode], str]:
+    def get_by_code_hash(
+        self, credentials: SyftVerifyKey, code_hash: int
+    ) -> Result[Optional[UserCode], str]:
         qks = QueryKeys(qks=[CodeHashPartitionKey.with_obj(code_hash)])
-        return self.query_one(qks=qks)
+        return self.query_one(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/user_roles.py` & `syft-0.8.0b8/src/syft/core/node/new/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/user_service.py` & `syft-0.8.0b8/src/syft/core/node/new/user_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 # relative
 from ....telemetry import instrument
+from .action_permissions import ActionObjectPermission
+from .action_permissions import ActionPermission
 from .context import AuthedServiceContext
 from .context import NodeServiceContext
 from .context import UnauthedServiceContext
 from .credentials import SyftVerifyKey
 from .credentials import UserLoginCredentials
 from .document_store import DocumentStore
 from .response import SyftError
 from .response import SyftSuccess
 from .serializable import serializable
 from .service import AbstractService
 from .service import SERVICE_TO_TYPES
 from .service import TYPE_TO_SERVICE
 from .service import service_method
+from .syft_metaclass import Empty
 from .uid import UID
 from .user import User
 from .user import UserCreate
 from .user import UserPrivateKey
 from .user import UserSearch
 from .user import UserUpdate
 from .user import UserView
@@ -47,97 +50,110 @@
 
     @service_method(path="user.create", name="create")
     def create(
         self, context: AuthedServiceContext, user_create: UserCreate
     ) -> Union[UserView, SyftError]:
         """Create a new user"""
         user = user_create.to(User)
-        result = self.stash.get_by_email(email=user.email)
+        result = self.stash.get_by_email(
+            credentials=context.credentials, email=user.email
+        )
         if result.is_err():
             return SyftError(message=str(result.err()))
         user_exists = result.ok() is not None
         if user_exists:
             return SyftError(message=f"User already exists with email: {user.email}")
 
-        result = self.stash.set(user=user)
+        result = self.stash.set(
+            credentials=context.credentials,
+            user=user,
+            add_permissions=[
+                ActionObjectPermission(
+                    uid=user.id, permission=ActionPermission.ALL_READ
+                ),
+            ],
+        )
         if result.is_err():
             return SyftError(message=str(result.err()))
         user = result.ok()
         return user.to(UserView)
 
     @service_method(path="user.view", name="view")
     def view(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[Optional[UserView], SyftError]:
         """Get user for given uid"""
-        result = self.stash.get_by_uid(uid=uid)
+        result = self.stash.get_by_uid(credentials=context.credentials, uid=uid)
         if result.is_ok():
             user = result.ok()
             if user is None:
                 return SyftError(message=f"No user exists for given: {uid}")
             return user.to(UserView)
 
         return SyftError(message=str(result.err()))
 
     @service_method(path="user.get_all", name="get_all", roles=DATA_OWNER_ROLE_LEVEL)
     def get_all(
         self, context: AuthedServiceContext
     ) -> Union[Optional[UserView], SyftError]:
-        result = self.stash.get_all()
+        result = self.stash.get_all(context.credentials)
         if result.is_ok():
             return [user.to(UserView) for user in result.ok()]
 
         # 🟡 TODO: No user exists will happen when result.ok() is empty list
         return SyftError(message="No users exists")
 
     def get_role_for_credentials(
         self, credentials: SyftVerifyKey
     ) -> Union[Optional[ServiceRole], SyftError]:
-        result = self.stash.get_by_verify_key(verify_key=credentials)
+        # they could be different
+        result = self.stash.get_by_verify_key(
+            credentials=credentials, verify_key=credentials
+        )
         if result.is_ok():
             # this seems weird that we get back None as Ok(None)
             user = result.ok()
             if user:
                 return user.role
         return ServiceRole.GUEST
 
     @service_method(path="user.search", name="search", autosplat=["user_search"])
     def search(
         self,
         context: AuthedServiceContext,
         user_search: UserSearch,
     ) -> Union[List[UserView], SyftError]:
-        kwargs = user_search.to_dict(exclude_none=True)
+        kwargs = user_search.to_dict(exclude_empty=True)
 
         if len(kwargs) == 0:
             valid_search_params = list(UserSearch.__fields__.keys())
             return SyftError(
                 message=f"Invalid Search parameters. \
                 Allowed params: {valid_search_params}"
             )
-        result = self.stash.find_all(**kwargs)
+        result = self.stash.find_all(credentials=context.credentials, **kwargs)
         if result.is_err():
             return SyftError(message=str(result.err()))
         users = result.ok()
         return [user.to(UserView) for user in users] if users is not None else []
 
     @service_method(path="user.update", name="update", roles=GUEST_ROLE_LEVEL)
     def update(
         self, context: AuthedServiceContext, uid: UID, user_update: UserUpdate
     ) -> Union[UserView, SyftError]:
-        updates_role = user_update.role is not None
+        updates_role = user_update.role is not Empty
 
         if (
             updates_role
             and ServiceRoleCapability.CAN_EDIT_ROLES not in context.capabilities()
         ):
             return SyftError(message=f"{context.role} is not allowed to edit roles")
 
         # Get user to be updated by its UID
-        result = self.stash.get_by_uid(uid=uid)
+        result = self.stash.get_by_uid(credentials=context.credentials, uid=uid)
 
         # TODO: ADD Email Validation
         if result.is_err():
             error_msg = (
                 f"Failed to find user with UID: {uid}. Error: {str(result.err())}"
             )
             return SyftError(message=error_msg)
@@ -161,16 +177,16 @@
             else:
                 return SyftError(
                     message=f"As a {context.role}, you are not allowed to edit {user.role} to {user_update.role}"
                 )
 
         edits_non_role_attrs = any(
             [
-                getattr(user_update, attr) is not None
-                for attr in user_update.to_dict(exclude_none=True)
+                getattr(user_update, attr) is not Empty
+                for attr in dict(user_update)
                 if attr != "role"
             ]
         )
 
         if (
             edits_non_role_attrs
             and user.verify_key != context.credentials
@@ -178,48 +194,50 @@
         ):
             return SyftError(
                 message=f"As a {context.role}, you are not allowed to edit users"
             )
 
         # Fill User Update fields that will not be changed by replacing it
         # for the current values found in user obj.
-        for name, value in vars(user_update).items():
+        for name, value in user_update.to_dict(exclude_empty=True).items():
             if name == "password" and value:
                 salt, hashed = salt_and_hash_password(value, 12)
                 user.hashed_password = hashed
                 user.salt = salt
             elif not name.startswith("__") and value is not None:
                 setattr(user, name, value)
 
-        result = self.stash.update(user=user)
+        result = self.stash.update(
+            credentials=context.credentials, user=user, has_permission=True
+        )
 
         if result.is_err():
             error_msg = (
                 f"Failed to update user with UID: {uid}. Error: {str(result.err())}"
             )
             return SyftError(message=error_msg)
 
         user = result.ok()
 
         return user.to(UserView)
 
-    def get_target_object(self, uid: UID):
-        user_result = self.stash.get_by_uid(uid=uid)
+    def get_target_object(self, credentials: SyftVerifyKey, uid: UID):
+        user_result = self.stash.get_by_uid(credentials=credentials, uid=uid)
         if user_result.is_err():
             return SyftError(message=str(user_result.err()))
         user = user_result.ok()
         if user is None:
             return SyftError(message=f"No user exists for given id: {uid}")
         else:
             return user
 
     @service_method(path="user.delete", name="delete", roles=GUEST_ROLE_LEVEL)
     def delete(self, context: AuthedServiceContext, uid: UID) -> Union[bool, SyftError]:
         # third party
-        user = self.get_target_object(uid)
+        user = self.get_target_object(context.credentials, uid)
         if isinstance(user, SyftError):
             return user
 
         permission_error = SyftError(
             message=str(
                 f"As a {context.role} you have no permission to delete user with {user.role} permission"
             )
@@ -230,27 +248,31 @@
         ]:
             pass
         elif context.role == ServiceRole.ADMIN:
             pass
         else:
             return permission_error
 
-        result = self.stash.delete_by_uid(uid=uid)
+        result = self.stash.delete_by_uid(
+            credentials=context.credentials, uid=uid, has_permission=True
+        )
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         return result.ok()
 
     def exchange_credentials(
         self, context: UnauthedServiceContext
     ) -> Union[UserLoginCredentials, SyftError]:
         """Verify user
         TODO: We might want to use a SyftObject instead
         """
-        result = self.stash.get_by_email(email=context.login_credentials.email)
+        result = self.stash.get_by_email(
+            credentials=self.admin_verify_key(), email=context.login_credentials.email
+        )
         if result.is_ok():
             user = result.ok()
             if user is not None and check_pwd(
                 context.login_credentials.password,
                 user.hashed_password,
             ):
                 return user.to(UserPrivateKey)
@@ -262,42 +284,57 @@
 
         return SyftError(
             message="Failed to retrieve user with "
             f"{context.login_credentials.email} with error: {result.err()}"
         )
 
     def admin_verify_key(self) -> Union[SyftVerifyKey, SyftError]:
-        result = self.stash.get_by_role(role=ServiceRole.ADMIN)
-        if result.is_err():
-            return SyftError(message=str(result.err()))
-        return result.ok().verify_key
+        try:
+            result = self.stash.admin_verify_key()
+            if result.is_ok():
+                return result.ok()
+            else:
+                return SyftError(message="failed to get admin verify_key")
+
+        except Exception as e:
+            return SyftError(message=str(e))
 
     def register(
         self, context: NodeServiceContext, new_user: UserCreate
     ) -> Union[Tuple[SyftSuccess, UserPrivateKey], SyftError]:
         """Register new user"""
 
         user = new_user.to(User)
-        result = self.stash.get_by_email(email=user.email)
+        result = self.stash.get_by_email(credentials=user.verify_key, email=user.email)
         if result.is_err():
             return SyftError(message=str(result.err()))
         user_exists = result.ok() is not None
         if user_exists:
             return SyftError(message=f"User already exists with email: {user.email}")
 
-        result = self.stash.set(user=user)
+        result = self.stash.set(
+            credentials=user.verify_key,
+            user=user,
+            add_permissions=[
+                ActionObjectPermission(
+                    uid=user.id, permission=ActionPermission.ALL_READ
+                ),
+            ],
+        )
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         user = result.ok()
         msg = SyftSuccess(message=f"{user.email} User successfully registered !!!")
         return tuple([msg, user.to(UserPrivateKey)])
 
     def user_verify_key(self, email: str) -> Union[SyftVerifyKey, SyftError]:
-        result = self.stash.get_by_email(email=email)
+        # we are bypassing permissions here, so dont use to return a result directly to the user
+        credentials = self.admin_verify_key()
+        result = self.stash.get_by_email(credentials=credentials, email=email)
         if result.is_ok():
             return result.ok().verify_key
         return SyftError(message=f"No user with email: {email}")
 
 
 TYPE_TO_SERVICE[User] = UserService
 SERVICE_TO_TYPES[UserService].update({User})
```

### Comparing `syft-0.8.0b7/src/syft/core/node/new/util.py` & `syft-0.8.0b8/src/syft/core/node/new/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/verification.py` & `syft-0.8.0b8/src/syft/core/node/new/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/new/worker_settings.py` & `syft-0.8.0b8/src/syft/core/node/new/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/core/node/worker.py` & `syft-0.8.0b8/src/syft/core/node/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,30 +99,44 @@
 def gipc_decoder(obj_bytes):
     return _deserialize(obj_bytes, from_bytes=True)
 
 
 NODE_PRIVATE_KEY = "NODE_PRIVATE_KEY"
 NODE_UID = "NODE_UID"
 
+DEFAULT_ROOT_EMAIL = "DEFAULT_ROOT_EMAIL"
+DEFAULT_ROOT_PASSWORD = "DEFAULT_ROOT_PASSWORD"  # nosec
+
+
+def get_env(key: str, default: Optional[Any] = None) -> Optional[str]:
+    return os.environ.get(key, default)
+
 
 def get_private_key_env() -> Optional[str]:
     return get_env(NODE_PRIVATE_KEY)
 
 
 def get_node_uid_env() -> Optional[str]:
     return get_env(NODE_UID)
 
 
-def get_env(key: str) -> Optional[str]:
-    return os.environ.get(key, None)
+def get_default_root_email() -> Optional[str]:
+    return get_env(DEFAULT_ROOT_EMAIL, "info@openmined.org")
+
+
+def get_default_root_password() -> Optional[str]:
+    return get_env(DEFAULT_ROOT_PASSWORD, "changethis")  # nosec
 
 
 signing_key_env = get_private_key_env()
 node_uid_env = get_node_uid_env()
 
+default_root_email = get_default_root_email()
+default_root_password = get_default_root_password()
+
 
 @instrument
 @serializable()
 class Worker(NewNode):
     signing_key: Optional[SyftSigningKey]
     required_signed_calls: bool = True
 
@@ -131,16 +145,16 @@
         *,  # Trasterisk
         name: Optional[str] = None,
         id: Optional[UID] = None,
         services: Optional[List[Type[AbstractService]]] = None,
         signing_key: Optional[Union[SyftSigningKey, SigningKey]] = None,
         action_store_config: Optional[StoreConfig] = None,
         document_store_config: Optional[StoreConfig] = None,
-        root_email: str = "info@openmined.org",
-        root_password: str = "changethis",
+        root_email: str = default_root_email,
+        root_password: str = default_root_password,
         processes: int = 0,
         is_subprocess: bool = False,
         node_type: NodeType = NodeType.DOMAIN,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
     ):
         # 🟡 TODO 22: change our ENV variable format and default init args to make this
@@ -283,23 +297,31 @@
         connection = PythonConnection(node=self)
         return SyftClient(connection=connection, credentials=SyftSigningKey.generate())
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}: {self.name} - {self.id} - {self.node_type} - {self.services}"
 
     def post_init(self) -> None:
+        context = AuthedServiceContext(
+            node=self, credentials=self.signing_key.verify_key
+        )
+
         if UserCodeService in self.services:
             user_code_service = self.get_service(UserCodeService)
-            user_code_service.load_user_code()
+            user_code_service.load_user_code(context=context)
         if self.is_subprocess:
             # print(f"> Starting Subprocess {self}")
             pass
         else:
             print(f"> Starting {self}")
-        CODE_RELOADER[thread_ident()] = user_code_service.load_user_code
+
+        def reload_user_code() -> None:
+            user_code_service.load_user_code(context=context)
+
+        CODE_RELOADER[thread_ident()] = reload_user_code
         # super().post_init()
 
     def init_stores(
         self,
         document_store_config: Optional[StoreConfig] = None,
         action_store_config: Optional[StoreConfig] = None,
     ):
@@ -316,15 +338,18 @@
             document_store_config.client_config.filename = f"{self.id}.sqlite"
             print(
                 f"SQLite Store Path:\n!open file://{document_store_config.client_config.file_path}\n"
             )
         document_store = document_store_config.store_type
         self.document_store_config = document_store_config
 
-        self.document_store = document_store(store_config=document_store_config)
+        self.document_store = document_store(
+            root_verify_key=self.signing_key.verify_key,
+            store_config=document_store_config,
+        )
         if action_store_config is None:
             if self.local_db or (self.processes > 0 and not self.is_subprocess):
                 client_config = SQLiteStoreClientConfig(path=self.sqlite_path)
                 action_store_config = SQLiteStoreConfig(client_config=client_config)
             else:
                 action_store_config = DictStoreConfig()
 
@@ -515,15 +540,15 @@
 
             user_config_registry = UserServiceConfigRegistry.from_role(role)
 
             if api_call.path not in user_config_registry:
                 if ServiceConfigRegistry.path_exists(api_call.path):
                     return SyftError(
                         message=f"As a `{role}`,"
-                        "you have has no access to: {api_call.path}"
+                        f"you have has no access to: {api_call.path}"
                     )  # type: ignore
                 else:
                     return SyftError(message=f"API call not in registered services: {api_call.path}")  # type: ignore
 
             _private_api_path = user_config_registry.private_path_for(api_call.path)
             method = self.get_service_method(_private_api_path)
             try:
@@ -689,15 +714,17 @@
     name: str,
     email: str,
     password: str,
     node: NewNode,
 ) -> Optional[User]:
     try:
         user_stash = UserStash(store=node.document_store)
-        row_exists = user_stash.get_by_email(email=email).ok()
+        row_exists = user_stash.get_by_email(
+            credentials=node.signing_key.verify_key, email=email
+        ).ok()
         if row_exists:
             return None
         else:
             create_user = UserCreate(
                 name=name,
                 email=email,
                 password=password,
@@ -705,18 +732,19 @@
                 role=ServiceRole.ADMIN,
             )
             # New User Initialization
             # 🟡 TODO: change later but for now this gives the main user super user automatically
             user = create_user.to(User)
             user.signing_key = node.signing_key
             user.verify_key = user.signing_key.verify_key
-            result = user_stash.set(user=user)
+            result = user_stash.set(credentials=node.signing_key.verify_key, user=user)
             if result.is_ok():
                 return result.ok()
-            return None
+            else:
+                raise Exception(f"Could not create user: {result}")
     except Exception as e:
         print("Unable to create new admin", e)
 
 
 def create_oblv_key_pair(
     worker: Worker,
 ) -> Optional[str]:
@@ -727,15 +755,15 @@
         from ...external.oblv.oblv_service import generate_oblv_key
 
         oblv_keys_stash = OblvKeysStash(store=worker.document_store)
 
         if not len(oblv_keys_stash):
             public_key, private_key = generate_oblv_key(oblv_key_name=worker.name)
             oblv_keys = OblvKeys(public_key=public_key, private_key=private_key)
-            res = oblv_keys_stash.set(oblv_keys)
+            res = oblv_keys_stash.set(worker.signing_key.verify_key, oblv_keys)
             if res.is_ok():
                 print("Successfully generated Oblv Key pair at startup")
             return res.err()
         else:
             print(f"Using Existing Public/Private Key pair: {len(oblv_keys_stash)}")
     except Exception as e:
         print("Unable to create Oblv Keys.", e)
```

### Comparing `syft-0.8.0b7/src/syft/deploy.py` & `syft-0.8.0b8/src/syft/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/experimental_flags.py` & `syft-0.8.0b8/src/syft/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/external/__init__.py` & `syft-0.8.0b8/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/external/oblv/__init__.py` & `syft-0.8.0b8/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/external/oblv/deployment.py` & `syft-0.8.0b8/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/external/oblv/deployment_client.py` & `syft-0.8.0b8/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/external/oblv/exceptions.py` & `syft-0.8.0b8/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/external/oblv/oblv_keys.py` & `syft-0.8.0b8/src/syft/external/oblv/oblv_keys.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.0b8/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/external/oblv/oblv_service.py` & `syft-0.8.0b8/src/syft/external/oblv/oblv_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 from ...core.node.new.api import NodeView
 from ...core.node.new.api import SyftAPI
 from ...core.node.new.client import HTTPConnection
 from ...core.node.new.client import Routes
 from ...core.node.new.context import AuthedServiceContext
 from ...core.node.new.context import ChangeContext
 from ...core.node.new.credentials import SyftSigningKey
+from ...core.node.new.credentials import SyftVerifyKey
 from ...core.node.new.deserialize import _deserialize as deserialize
 from ...core.node.new.document_store import DocumentStore
+from ...core.node.new.response import SyftError
 from ...core.node.new.serializable import serializable
 from ...core.node.new.service import AbstractService
 from ...core.node.new.service import service_method
 from ...core.node.new.syft_object import SYFT_OBJECT_VERSION_1
 from ...core.node.new.syft_object import SyftObject
 from ...core.node.new.uid import UID
 from ...core.node.new.user_code import UserCode
@@ -67,29 +69,34 @@
 
     def __repr__(self) -> str:
         return self.base_dict.__repr__()
 
 
 def connect_to_enclave(
     oblv_keys_stash: OblvKeysStash,
+    verify_key: SyftVerifyKey,
     oblv_client: OblvClient,
     deployment_id: str,
     connection_port: int,
     oblv_key_name: str,
 ) -> Optional[subprocess.Popen]:
     global OBLV_PROCESS_CACHE
     if deployment_id in OBLV_PROCESS_CACHE:
         process = OBLV_PROCESS_CACHE[deployment_id][0]
         if process.poll() is None:
             return process
         # If the process has been terminated create a new connection
         del OBLV_PROCESS_CACHE[deployment_id]
 
     # Always create key file each time, which ensures consistency when there is key change in database
-    create_keys_from_db(oblv_keys_stash=oblv_keys_stash, oblv_key_name=oblv_key_name)
+    create_keys_from_db(
+        oblv_keys_stash=oblv_keys_stash,
+        verify_key=verify_key,
+        oblv_key_name=oblv_key_name,
+    )
     oblv_key_path = os.path.expanduser(os.getenv("OBLV_KEY_PATH", "~/.oblv"))
 
     public_file_name = oblv_key_path + "/" + oblv_key_name + "_public.der"
     private_file_name = oblv_key_path + "/" + oblv_key_name + "_private.der"
 
     depl = oblv_client.deployment_info(deployment_id)
     if depl.is_deleted:
@@ -158,28 +165,30 @@
 
     OBLV_PROCESS_CACHE[deployment_id] = [process, connection_port]
     return None
 
 
 def make_request_to_enclave(
     oblv_keys_stash: OblvKeysStash,
+    verify_key: SyftVerifyKey,
     deployment_id: str,
     oblv_client: OblvClient,
     request_method: Callable,
     connection_string: str,
     connection_port: int,
     oblv_key_name: str,
     params: Optional[Dict] = None,
     files: Optional[Dict] = None,
     data: Optional[Dict] = None,
     json: Optional[Dict] = None,
 ) -> Any:
     if not LOCAL_MODE:
         _ = connect_to_enclave(
             oblv_keys_stash=oblv_keys_stash,
+            verify_key=verify_key,
             oblv_client=oblv_client,
             deployment_id=deployment_id,
             connection_port=connection_port,
             oblv_key_name=oblv_key_name,
         )
         req = request_method(
             connection_string,
@@ -199,21 +208,23 @@
             params=params,
             files=files,
             data=data,
             json=json,
         )
 
 
-def create_keys_from_db(oblv_keys_stash: OblvKeysStash, oblv_key_name: str):
+def create_keys_from_db(
+    oblv_keys_stash: OblvKeysStash, verify_key: SyftVerifyKey, oblv_key_name: str
+):
     oblv_key_path = os.path.expanduser(os.getenv("OBLV_KEY_PATH", "~/.oblv"))
 
     os.makedirs(oblv_key_path, exist_ok=True)
     # Temporary new key name for the new service
 
-    keys = oblv_keys_stash.get_all()
+    keys = oblv_keys_stash.get_all(verify_key)
     if keys.is_ok():
         keys = keys.ok()[0]
     else:
         return keys.err()
 
     f_private = open(oblv_key_path + "/" + oblv_key_name + "_private.der", "w+b")
     f_private.write(keys.private_key)
@@ -274,15 +285,15 @@
         # TODO 🟣 Check for permission after it is fully integrated
         public_key, private_key = generate_oblv_key()
 
         if override_existing_key:
             self.oblv_keys_stash.clear()
         oblv_keys = OblvKeys(public_key=public_key, private_key=private_key)
 
-        res = self.oblv_keys_stash.set(oblv_keys)
+        res = self.oblv_keys_stash.set(context.credentials, oblv_keys)
 
         if res.is_ok():
             return Ok(
                 "Successfully created a new public/private RSA key-pair on the domain node"
             )
         return res.err()
 
@@ -292,15 +303,15 @@
     def get_public_key(
         self,
         context: AuthedServiceContext,
     ) -> Result[Ok, Err]:
         "Retrieves the public key present on the Domain Node."
 
         if len(self.oblv_keys_stash):
-            oblv_keys = self.oblv_keys_stash.get_all()
+            oblv_keys = self.oblv_keys_stash.get_all(context.credentials)
             if oblv_keys.is_ok():
                 oblv_keys = oblv_keys.ok()[0]
             else:
                 return oblv_keys.err()
 
             public_key_str = (
                 encodebytes(oblv_keys.public_key).decode("UTF-8").replace("\n", "")
@@ -344,14 +355,15 @@
 
         params = {"verify_key": str(signing_key.verify_key)}
         req = make_request_to_enclave(
             connection_string=connection_string + Routes.ROUTE_API.value,
             deployment_id=deployment_id,
             oblv_client=oblv_client,
             oblv_keys_stash=self.oblv_keys_stash,
+            verify_key=signing_key.verify_key,
             request_method=requests.get,
             connection_port=port,
             oblv_key_name=worker_name,
             params=params,
         )
 
         obj = deserialize(req.content, from_bytes=True)
@@ -374,15 +386,22 @@
     ) -> Result[Ok, Err]:
         if not context.node or not context.node.signing_key:
             return Err(f"{type(context)} has no node")
         signing_key = context.node.signing_key
 
         user_code_service = context.node.get_service("usercodeservice")
         action_service = context.node.get_service("actionservice")
-        user_code = user_code_service.get_by_uid(context, uid=user_code_id)
+        user_code = user_code_service.stash.get_by_uid(
+            context.node.signing_key.verify_key, uid=user_code_id
+        )
+        if user_code.is_err():
+            return SyftError(
+                message=f"Unable to find {user_code_id} in {type(user_code_service)}"
+            )
+        user_code = user_code.ok()
 
         res = user_code.status.mutate(
             value=UserCodeStatus.EXECUTE,
             node_name=node_name,
             verify_key=context.credentials,
         )
         if res.is_err():
```

### Comparing `syft-0.8.0b7/src/syft/filterwarnings.py` & `syft-0.8.0b8/src/syft/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/gevent_patch.py` & `syft-0.8.0b8/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/logger.py` & `syft-0.8.0b8/src/syft/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/registry.py` & `syft-0.8.0b8/src/syft/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/search.py` & `syft-0.8.0b8/src/syft/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/telemetry.py` & `syft-0.8.0b8/src/syft/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/trace_decorator.py` & `syft-0.8.0b8/src/syft/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/user_settings.py` & `syft-0.8.0b8/src/syft/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/util.py` & `syft-0.8.0b8/src/syft/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft/version_compare.py` & `syft-0.8.0b8/src/syft/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b7/src/syft.egg-info/PKG-INFO` & `syft-0.8.0b8/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b7
+Version: 0.8.0b8
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -321,7 +321,9 @@
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
 
 [Apache License 2.0](LICENSE)<br />
 <a href="https://www.flaticon.com/free-icons/person" title="person icons">Person icons created by Freepik - Flaticon</a>
+
+<!-- 🥇 -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b7 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.0b8 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.0b7/src/syft.egg-info/SOURCES.txt` & `syft-0.8.0b8/src/syft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/syft/capnp/recursive_serde.capnp
 src/syft/core/__init__.py
 src/syft/core/node/__init__.py
 src/syft/core/node/worker.py
 src/syft/core/node/new/__init__.py
 src/syft/core/node/new/action_data_empty.py
 src/syft/core/node/new/action_object.py
+src/syft/core/node/new/action_permissions.py
 src/syft/core/node/new/action_service.py
 src/syft/core/node/new/action_store.py
 src/syft/core/node/new/action_types.py
 src/syft/core/node/new/api.py
 src/syft/core/node/new/array.py
 src/syft/core/node/new/arrow.py
 src/syft/core/node/new/base.py
@@ -91,14 +92,15 @@
 src/syft/core/node/new/response.py
 src/syft/core/node/new/roles.py
 src/syft/core/node/new/serializable.py
 src/syft/core/node/new/serialize.py
 src/syft/core/node/new/service.py
 src/syft/core/node/new/signature.py
 src/syft/core/node/new/sqlite_document_store.py
+src/syft/core/node/new/syft_metaclass.py
 src/syft/core/node/new/syft_object.py
 src/syft/core/node/new/test_service.py
 src/syft/core/node/new/third_party.py
 src/syft/core/node/new/transforms.py
 src/syft/core/node/new/twin_object.py
 src/syft/core/node/new/uid.py
 src/syft/core/node/new/unparse.py
```

### Comparing `syft-0.8.0b7/src/syft.egg-info/requires.txt` & `syft-0.8.0b8/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

