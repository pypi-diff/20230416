# Comparing `tmp/fschat-0.2.1.tar.gz` & `tmp/fschat-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.2.1.tar", last modified: Wed Apr 12 23:05:55 2023, max compression
+gzip compressed data, was "fschat-0.2.2.tar", last modified: Sun Apr 16 13:22:37 2023, max compression
```

## Comparing `fschat-0.2.1.tar` & `fschat-0.2.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 23:05:55.546520 fschat-0.2.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12087 2023-04-12 23:05:55.546520 fschat-0.2.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11613 2023-04-12 23:05:33.000000 fschat-0.2.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 23:05:55.542520 fschat-0.2.1/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5440 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 23:05:55.542520 fschat-0.2.1/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/data/alpaca-converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5543 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5976 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/data/hardcoded_questions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      615 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/data/merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2684 2023-04-08 06:26:44.000000 fschat-0.2.1/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/data/sample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3188 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 23:05:55.542520 fschat-0.2.1/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-04-08 06:26:44.000000 fschat-0.2.1/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3661 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2986 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2345 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 23:05:55.542520 fschat-0.2.1/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1576 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/model/convert_fp16.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/model/make_delta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 23:05:55.546520 fschat-0.2.1/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11255 2023-04-10 08:26:53.000000 fschat-0.2.1/fastchat/serve/cacheflow_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4206 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-04-09 00:28:23.000000 fschat-0.2.1/fastchat/serve/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9943 2023-04-11 03:55:38.000000 fschat-0.2.1/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2717 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16276 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1897 2023-04-12 23:05:33.000000 fschat-0.2.1/fastchat/serve/huggingface_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6539 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/serve/inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7053 2023-04-11 17:38:03.000000 fschat-0.2.1/fastchat/serve/model_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-08 06:26:44.000000 fschat-0.2.1/fastchat/serve/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-03 18:06:47.000000 fschat-0.2.1/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-09 00:28:23.000000 fschat-0.2.1/fastchat/serve/serve_chatglm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2359 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/serve/test_message.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3867 2023-04-11 03:55:38.000000 fschat-0.2.1/fastchat/serve/test_throughput.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 23:05:55.546520 fschat-0.2.1/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3982 2023-04-08 06:26:44.000000 fschat-0.2.1/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8450 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/train/train.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3657 2023-04-08 06:26:44.000000 fschat-0.2.1/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-04-12 19:30:04.000000 fschat-0.2.1/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4186 2023-04-09 00:28:23.000000 fschat-0.2.1/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 23:05:55.546520 fschat-0.2.1/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12087 2023-04-12 23:05:55.000000 fschat-0.2.1/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1474 2023-04-12 23:05:55.000000 fschat-0.2.1/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-12 23:05:55.000000 fschat-0.2.1/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-04-12 23:05:55.000000 fschat-0.2.1/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-12 23:05:55.000000 fschat-0.2.1/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      979 2023-04-12 23:05:39.000000 fschat-0.2.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-12 23:05:55.546520 fschat-0.2.1/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.921172 fschat-0.2.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12292 2023-04-16 13:22:37.921172 fschat-0.2.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11818 2023-04-16 13:16:40.000000 fschat-0.2.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.913172 fschat-0.2.2/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6288 2023-04-16 09:48:12.000000 fschat-0.2.2/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.917172 fschat-0.2.2/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/alpaca-converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5543 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5976 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      615 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2684 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3188 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.917172 fschat-0.2.2/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3661 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3072 2023-04-16 12:58:41.000000 fschat-0.2.2/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2345 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.917172 fschat-0.2.2/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5704 2023-04-16 09:48:14.000000 fschat-0.2.2/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/model/make_delta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.921172 fschat-0.2.2/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11255 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5478 2023-04-16 09:48:14.000000 fschat-0.2.2/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9943 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2717 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16562 2023-04-16 12:58:41.000000 fschat-0.2.2/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2120 2023-04-16 12:58:41.000000 fschat-0.2.2/fastchat/serve/huggingface_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8321 2023-04-16 13:00:59.000000 fschat-0.2.2/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7202 2023-04-16 09:48:14.000000 fschat-0.2.2/fastchat/serve/model_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/serve_chatglm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2429 2023-04-16 12:58:41.000000 fschat-0.2.2/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3867 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.921172 fschat-0.2.2/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3982 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8450 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/train/train.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    15586 2023-04-16 09:48:12.000000 fschat-0.2.2/fastchat/train/train_flant5.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3649 2023-04-16 09:48:12.000000 fschat-0.2.2/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4999 2023-04-16 09:48:12.000000 fschat-0.2.2/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.921172 fschat-0.2.2/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12292 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1505 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-04-16 13:10:56.000000 fschat-0.2.2/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-16 13:22:37.921172 fschat-0.2.2/setup.cfg
```

### Comparing `fschat-0.2.1/LICENSE` & `fschat-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/PKG-INFO` & `fschat-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: fschat
-Version: 0.2.1
-Summary: An open platform for training, serving, and evaluating large language model based chatbots.
-Project-URL: Homepage, https://github.com/lm-sys/fastchat
-Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FastChat
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
@@ -35,19 +23,15 @@
 - [Fine-tuning](#fine-tuning)
 
 ## Install
 
 ### Method 1: With pip
 
 ```bash
-# Install FastChat
 pip3 install fschat
-
-# Install the latest main branch of huggingface/transformers
-pip3 install git+https://github.com/huggingface/transformers
 ```
 
 ### Method 2: From source
 
 1. Clone this repository and navigate to the FastChat folder
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
@@ -69,40 +53,46 @@
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
-Our released weights are only compatible with the latest main branch of huggingface/transformers.
-We install the correct version of transformers when fastchat is installed.
+Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
+Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
-If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
+See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-7b \
     --target /output/path/to/vicuna-7b \
     --delta lmsys/vicuna-7b-delta-v1.1
 ```
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
-If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
+See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-13b \
     --target /output/path/to/vicuna-13b \
     --delta lmsys/vicuna-13b-delta-v1.1
 ```
 
 ### Old weights
 See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
 
+
+### Low CPU Memory Conversion
+You can try these methods to reduce the CPU RAM requirement of weight conversion.
+1. Append `--low-cpu-mem` to the commands above, which will split large weight files into smaller ones and use the disk as temporary storage. This can keep the peak memory at less than 16GB.
+2. Create a large swap file and rely on the operating system to automatically utilize the disk as virtual memory.
+
 ## Inference with Command Line Interface
 
 (Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
 #### Single GPU
```

#### html2text {}

```diff
@@ -1,84 +1,81 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.1 Summary: An open platform for
-training, serving, and evaluating large language model based chatbots. Project-
-URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
-https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # FastChat An open platform for training, serving, and evaluating large
+# FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
 - ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
 ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
 [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
 (https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
 twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
 (#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-
-tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash # Install
-FastChat pip3 install fschat # Install the latest main branch of huggingface/
-transformers pip3 install git+https://github.com/huggingface/transformers ```
-### Method 2: From source 1. Clone this repository and navigate to the FastChat
-folder ```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ```
-If you are running on Mac: ```bash brew install rust cmake ``` 2. Install
-Package ```bash pip3 install --upgrade pip # enable PEP 660 support pip3
-install -e . ``` ## Vicuna Weights We release [Vicuna](https://
+tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash pip3 install
+fschat ``` ### Method 2: From source 1. Clone this repository and navigate to
+the FastChat folder ```bash git clone https://github.com/lm-sys/FastChat.git cd
+FastChat ``` If you are running on Mac: ```bash brew install rust cmake ``` 2.
+Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
+pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
 vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
 license. You can add our delta to the original LLaMA weights to obtain the
 Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
 huggingface format by following the instructions [here](https://huggingface.co/
 docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
 Vicuna weights by applying our delta. They will automatically download delta
 weights from our Hugging Face [account](https://huggingface.co/lmsys).
-**NOTE**: Our released weights are only compatible with the latest main branch
-of huggingface/transformers. We install the correct version of transformers
-when fastchat is installed. ### Vicuna-7B This conversion command needs around
-30 GB of CPU RAM. If you do not have enough memory, you can create a large swap
-file that allows the operating system to automatically utilize the disk as
-virtual memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/
-to/llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-
-delta-v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU
-RAM. If you do not have enough memory, you can create a large swap file that
-allows the operating system to automatically utilize the disk as virtual
+**NOTE**: Weights v1.1 are only compatible with ```transformers>=4.28.0``` and
+``fschat >= 0.2.0``. Please update your local packages accordingly. If you
+follow the above commands to do a fresh install, then you should get all the
+correct versions. ### Vicuna-7B This conversion command needs around 30 GB of
+CPU RAM. See the "Low CPU Memory Conversion" section below if you do not have
+enough memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/
+llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-
+v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM.
+See the "Low CPU Memory Conversion" section below if you do not have enough
 memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/llama-
 13b \ --target /output/path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1
 ``` ### Old weights See [docs/weights_version.md](docs/weights_version.md) for
-all versions of weights and their differences. ## Inference with Command Line
-Interface (Experimental Feature: You can specify `--style rich` to enable rich
-text output and better text streaming quality for some non-ASCII content. This
-may not work properly on certain terminals.) [assets/screenshot_cli.png] ####
-Single GPU The command below requires around 28GB of GPU memory for Vicuna-13B
-and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory" section below
-if you do not have enough memory. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/vicuna/weights ``` #### Multiple GPUs You can use model
-parallelism to aggregate GPU memory from multiple GPUs on the same machine. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
-``` #### CPU Only This runs on the CPU only and does not require GPU. It
-requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory
-for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/
-weights --device cpu ``` #### Metal Backend (Mac Computers with Apple Silicon
-or AMD GPUs) Use `--device mps` to enable GPU acceleration on Mac computers
-(requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit compression. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps
---load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words /
-second. #### No Enough Memory or Other Platforms If you do not have enough
-memory, you can enable 8-bit compression by adding `--load-8bit` to commands
-above. This can reduce memory usage by around half with slightly degraded model
-quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
-8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
-``` Besides, we are actively exploring more methods to make the model easier to
-run on more platforms. Contributions and pull requests are welcome. ## Serving
-with Web GUI [assets/screenshot_gui.png] To serve using the web UI, you need
-three main components: web servers that interface with users, model workers
-that host one or more models, and a controller to coordinate the webserver and
-model workers. Here are the commands to follow in your terminal: #### Launch
-the controller ```bash python3 -m fastchat.serve.controller ``` This controller
-manages the distributed workers. #### Launch the model worker ```bash python3 -
+all versions of weights and their differences. ### Low CPU Memory Conversion
+You can try these methods to reduce the CPU RAM requirement of weight
+conversion. 1. Append `--low-cpu-mem` to the commands above, which will split
+large weight files into smaller ones and use the disk as temporary storage.
+This can keep the peak memory at less than 16GB. 2. Create a large swap file
+and rely on the operating system to automatically utilize the disk as virtual
+memory. ## Inference with Command Line Interface (Experimental Feature: You can
+specify `--style rich` to enable rich text output and better text streaming
+quality for some non-ASCII content. This may not work properly on certain
+terminals.) [assets/screenshot_cli.png] #### Single GPU The command below
+requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
+Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
+memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
+from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
+the CPU only and does not require GPU. It requires around 60GB of CPU memory
+for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
+Other Platforms If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
+--model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+exploring more methods to make the model easier to run on more platforms.
+Contributions and pull requests are welcome. ## Serving with Web GUI [assets/
+screenshot_gui.png] To serve using the web UI, you need three main components:
+web servers that interface with users, model workers that host one or more
+models, and a controller to coordinate the webserver and model workers. Here
+are the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
```

### Comparing `fschat-0.2.1/README.md` & `fschat-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: fschat
+Version: 0.2.2
+Summary: An open platform for training, serving, and evaluating large language model based chatbots.
+Project-URL: Homepage, https://github.com/lm-sys/fastchat
+Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # FastChat
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
@@ -23,19 +35,15 @@
 - [Fine-tuning](#fine-tuning)
 
 ## Install
 
 ### Method 1: With pip
 
 ```bash
-# Install FastChat
 pip3 install fschat
-
-# Install the latest main branch of huggingface/transformers
-pip3 install git+https://github.com/huggingface/transformers
 ```
 
 ### Method 2: From source
 
 1. Clone this repository and navigate to the FastChat folder
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
@@ -57,40 +65,46 @@
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
-Our released weights are only compatible with the latest main branch of huggingface/transformers.
-We install the correct version of transformers when fastchat is installed.
+Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
+Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
-If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
+See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-7b \
     --target /output/path/to/vicuna-7b \
     --delta lmsys/vicuna-7b-delta-v1.1
 ```
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
-If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
+See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-13b \
     --target /output/path/to/vicuna-13b \
     --delta lmsys/vicuna-13b-delta-v1.1
 ```
 
 ### Old weights
 See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
 
+
+### Low CPU Memory Conversion
+You can try these methods to reduce the CPU RAM requirement of weight conversion.
+1. Append `--low-cpu-mem` to the commands above, which will split large weight files into smaller ones and use the disk as temporary storage. This can keep the peak memory at less than 16GB.
+2. Create a large swap file and rely on the operating system to automatically utilize the disk as virtual memory.
+
 ## Inference with Command Line Interface
 
 (Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
 #### Single GPU
```

#### html2text {}

```diff
@@ -1,78 +1,87 @@
-# FastChat An open platform for training, serving, and evaluating large
+Metadata-Version: 2.1 Name: fschat Version: 0.2.2 Summary: An open platform for
+training, serving, and evaluating large language model based chatbots. Project-
+URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
+https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE # FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
 - ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
 ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
 [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
 (https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
 twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
 (#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-
-tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash # Install
-FastChat pip3 install fschat # Install the latest main branch of huggingface/
-transformers pip3 install git+https://github.com/huggingface/transformers ```
-### Method 2: From source 1. Clone this repository and navigate to the FastChat
-folder ```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ```
-If you are running on Mac: ```bash brew install rust cmake ``` 2. Install
-Package ```bash pip3 install --upgrade pip # enable PEP 660 support pip3
-install -e . ``` ## Vicuna Weights We release [Vicuna](https://
+tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash pip3 install
+fschat ``` ### Method 2: From source 1. Clone this repository and navigate to
+the FastChat folder ```bash git clone https://github.com/lm-sys/FastChat.git cd
+FastChat ``` If you are running on Mac: ```bash brew install rust cmake ``` 2.
+Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
+pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
 vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
 license. You can add our delta to the original LLaMA weights to obtain the
 Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
 huggingface format by following the instructions [here](https://huggingface.co/
 docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
 Vicuna weights by applying our delta. They will automatically download delta
 weights from our Hugging Face [account](https://huggingface.co/lmsys).
-**NOTE**: Our released weights are only compatible with the latest main branch
-of huggingface/transformers. We install the correct version of transformers
-when fastchat is installed. ### Vicuna-7B This conversion command needs around
-30 GB of CPU RAM. If you do not have enough memory, you can create a large swap
-file that allows the operating system to automatically utilize the disk as
-virtual memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/
-to/llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-
-delta-v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU
-RAM. If you do not have enough memory, you can create a large swap file that
-allows the operating system to automatically utilize the disk as virtual
+**NOTE**: Weights v1.1 are only compatible with ```transformers>=4.28.0``` and
+``fschat >= 0.2.0``. Please update your local packages accordingly. If you
+follow the above commands to do a fresh install, then you should get all the
+correct versions. ### Vicuna-7B This conversion command needs around 30 GB of
+CPU RAM. See the "Low CPU Memory Conversion" section below if you do not have
+enough memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/
+llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-
+v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM.
+See the "Low CPU Memory Conversion" section below if you do not have enough
 memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/llama-
 13b \ --target /output/path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1
 ``` ### Old weights See [docs/weights_version.md](docs/weights_version.md) for
-all versions of weights and their differences. ## Inference with Command Line
-Interface (Experimental Feature: You can specify `--style rich` to enable rich
-text output and better text streaming quality for some non-ASCII content. This
-may not work properly on certain terminals.) [assets/screenshot_cli.png] ####
-Single GPU The command below requires around 28GB of GPU memory for Vicuna-13B
-and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory" section below
-if you do not have enough memory. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/vicuna/weights ``` #### Multiple GPUs You can use model
-parallelism to aggregate GPU memory from multiple GPUs on the same machine. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
-``` #### CPU Only This runs on the CPU only and does not require GPU. It
-requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory
-for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/
-weights --device cpu ``` #### Metal Backend (Mac Computers with Apple Silicon
-or AMD GPUs) Use `--device mps` to enable GPU acceleration on Mac computers
-(requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit compression. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps
---load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words /
-second. #### No Enough Memory or Other Platforms If you do not have enough
-memory, you can enable 8-bit compression by adding `--load-8bit` to commands
-above. This can reduce memory usage by around half with slightly degraded model
-quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
-8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
-``` Besides, we are actively exploring more methods to make the model easier to
-run on more platforms. Contributions and pull requests are welcome. ## Serving
-with Web GUI [assets/screenshot_gui.png] To serve using the web UI, you need
-three main components: web servers that interface with users, model workers
-that host one or more models, and a controller to coordinate the webserver and
-model workers. Here are the commands to follow in your terminal: #### Launch
-the controller ```bash python3 -m fastchat.serve.controller ``` This controller
-manages the distributed workers. #### Launch the model worker ```bash python3 -
+all versions of weights and their differences. ### Low CPU Memory Conversion
+You can try these methods to reduce the CPU RAM requirement of weight
+conversion. 1. Append `--low-cpu-mem` to the commands above, which will split
+large weight files into smaller ones and use the disk as temporary storage.
+This can keep the peak memory at less than 16GB. 2. Create a large swap file
+and rely on the operating system to automatically utilize the disk as virtual
+memory. ## Inference with Command Line Interface (Experimental Feature: You can
+specify `--style rich` to enable rich text output and better text streaming
+quality for some non-ASCII content. This may not work properly on certain
+terminals.) [assets/screenshot_cli.png] #### Single GPU The command below
+requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
+Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
+memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
+from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
+the CPU only and does not require GPU. It requires around 60GB of CPU memory
+for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
+Other Platforms If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
+--model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+exploring more methods to make the model easier to run on more platforms.
+Contributions and pull requests are welcome. ## Serving with Web GUI [assets/
+screenshot_gui.png] To serve using the web UI, you need three main components:
+web servers that interface with users, model workers that host one or more
+models, and a controller to coordinate the webserver and model workers. Here
+are the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
```

### Comparing `fschat-0.2.1/fastchat/conversation.py` & `fschat-0.2.2/fastchat/conversation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List, Tuple, Any
 
 
 class SeparatorStyle(Enum):
     """Different separator style."""
     SINGLE = auto()
     TWO = auto()
+    DOLLY = auto()
 
 
 @dataclasses.dataclass
 class Conversation:
     """A class that keeps all conversation history."""
     system: str
     roles: List[str]
@@ -38,14 +39,25 @@
             ret = self.system + seps[0]
             for i, (role, message) in enumerate(self.messages):
                 if message:
                     ret += role + ": " + message + seps[i % 2]
                 else:
                     ret += role + ":"
             return ret
+        elif self.sep_style == SeparatorStyle.DOLLY:
+            seps = [self.sep, self.sep2]
+            ret = self.system
+            for i, (role, message) in enumerate(self.messages):
+                if message:
+                    ret += role + ":\n" + message + seps[i % 2]
+                    if i % 2 == 1:
+                        ret += "\n\n"
+                else:
+                    ret += role + ":\n"
+            return ret
         else:
             raise ValueError(f"Invalid style: {self.sep_style}")
 
     def append_message(self, role, message):
         self.messages.append([role, message])
 
     def to_gradio_chatbot(self):
@@ -130,26 +142,39 @@
     messages=(),
     offset=0,
     sep_style=SeparatorStyle.TWO,
     sep=" ",
     sep2="</s>",
 )
 
+conv_dolly = Conversation(
+    system=
+    "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n",
+    roles=('### Instruction', '### Response'),
+    messages=(),
+    offset=0,
+    sep_style=SeparatorStyle.DOLLY,
+    sep="\n\n",
+    sep2="### End",
+)
 
 conv_templates = {
     "conv_one_shot": conv_one_shot,
     "vicuna_v1.1": conv_vicuna_v1_1,
     "koala_v1": conv_koala_v1,
+    "dolly": conv_dolly,
 }
 
 
 def get_default_conv_template(model_name):
     model_name = model_name.lower()
     if "vicuna" in model_name or "output" in model_name:
         return conv_vicuna_v1_1
     elif "koala" in model_name:
         return conv_koala_v1
+    elif "dolly" in model_name:
+        return conv_dolly
     return conv_one_shot
 
 
 if __name__ == "__main__":
     print(default_conversation.get_prompt())
```

### Comparing `fschat-0.2.1/fastchat/data/alpaca-converter.py` & `fschat-0.2.2/fastchat/data/alpaca-converter.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/data/clean_sharegpt.py` & `fschat-0.2.2/fastchat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/data/hardcoded_questions.py` & `fschat-0.2.2/fastchat/data/hardcoded_questions.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/data/inspect.py` & `fschat-0.2.2/fastchat/data/inspect.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/data/merge.py` & `fschat-0.2.2/fastchat/data/merge.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/data/optional_clean.py` & `fschat-0.2.2/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/data/sample.py` & `fschat-0.2.2/fastchat/data/sample.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/data/split_long_conversation.py` & `fschat-0.2.2/fastchat/data/split_long_conversation.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.2/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.2/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/eval/get_model_answer.py` & `fschat-0.2.2/fastchat/eval/get_model_answer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import argparse
-from transformers import AutoTokenizer, AutoModelForCausalLM
+from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaForCausalLM
 import torch
 import os
 import json
 from tqdm import tqdm
 import shortuuid
 import ray
 
 from fastchat.conversation import get_default_conv_template
+from fastchat.serve.inference import compute_skip_echo_len
 from fastchat.utils import disable_torch_init
 
 
 def run_eval(model_path, model_id, question_file, answer_file, num_gpus):
     # split question file into num_gpus files
     ques_jsons = []
     with open(os.path.expanduser(question_file), "r") as ques_file:
@@ -53,15 +54,15 @@
         inputs = tokenizer([prompt])
         output_ids = model.generate(
             torch.as_tensor(inputs.input_ids).cuda(),
             do_sample=True,
             temperature=0.7,
             max_new_tokens=1024)
         outputs = tokenizer.batch_decode(output_ids, skip_special_tokens=True)[0]
-        skip_echo_len = len(prompt.replace("</s>", " ")) + 1
+        skip_echo_len = compute_skip_echo_len(model_id, conv, prompt)
 
         outputs = outputs[skip_echo_len:].strip()
         ans_id = shortuuid.uuid()
         ans_jsons.append({"question_id": idx,
                           "text": outputs,
                           "answer_id": ans_id,
                           "model_id": model_id,
```

### Comparing `fschat-0.2.1/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.2/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/model/convert_fp16.py` & `fschat-0.2.2/fastchat/model/convert_fp16.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/model/make_delta.py` & `fschat-0.2.2/fastchat/model/make_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/cacheflow_worker.py` & `fschat-0.2.2/fastchat/serve/cacheflow_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/cli.py` & `fschat-0.2.2/fastchat/serve/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,42 +67,62 @@
         with Live(console=self._console, refresh_per_second=4) as live:
             # Read lines from the stream
             for outputs in output_stream:
                 accumulated_text = outputs[skip_echo_len:]
                 if not accumulated_text:
                     continue
                 # Render the accumulated text as Markdown
-                markdown = Markdown(accumulated_text)
+                # NOTE: this is a workaround for the rendering "unstandard markdown"
+                #  in rich. The chatbots output treat "\n" as a new line for
+                #  better compatibility with real-world text. However, rendering
+                #  in markdown would break the format. It is because standard markdown
+                #  treat a single "\n" in normal text as a space.
+                #  Our workaround is adding two spaces at the end of each line.
+                #  This is not a perfect solution, as it would
+                #  introduce trailing spaces (only) in code block, but it works well
+                #  especially for console output, because in general the console does not
+                #  care about trailing spaces.
+                lines = []
+                for line in accumulated_text.splitlines():
+                    lines.append(line)
+                    if line.startswith("```"):
+                        # Code block marker - do not add trailing spaces, as it would
+                        #  break the syntax highlighting
+                        lines.append("\n")
+                    else:
+                        lines.append("  \n")
+                markdown = Markdown("".join(lines))
                 # Update the Live console output
                 live.update(markdown)
         self._console.print()
         return outputs[skip_echo_len:]
 
 
 def main(args):
     if args.style == "simple":
         chatio = SimpleChatIO()
     elif args.style == "rich":
         chatio = RichChatIO()
     else:
         raise ValueError(f"Invalid style for console: {args.style}")
     try:
-        chat_loop(args.model_path, args.device, args.num_gpus, args.load_8bit,
-                args.conv_template, args.temperature, args.max_new_tokens,
-                chatio, args.debug)
+        chat_loop(args.model_path, args.device, args.num_gpus, args.max_gpu_memory,
+            args.load_8bit, args.conv_template, args.temperature, args.max_new_tokens,
+            chatio, args.debug)
     except KeyboardInterrupt:
         print("exit...")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--model-path", type=str, default="facebook/opt-350m",
         help="The path to the weights")
     parser.add_argument("--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda")
     parser.add_argument("--num-gpus", type=str, default="1")
+    parser.add_argument("--max-gpu-memory", type=str, default="13GiB")
     parser.add_argument("--load-8bit", action="store_true",
         help="Use 8-bit quantization.")
     parser.add_argument("--conv-template", type=str, default=None,
         help="Conversation prompt template.")
     parser.add_argument("--temperature", type=float, default=0.7)
     parser.add_argument("--max-new-tokens", type=int, default=512)
     parser.add_argument("--style", type=str, default="simple",
```

### Comparing `fschat-0.2.1/fastchat/serve/compression.py` & `fschat-0.2.2/fastchat/serve/compression.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/controller.py` & `fschat-0.2.2/fastchat/serve/controller.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/gradio_css.py` & `fschat-0.2.2/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/gradio_patch.py` & `fschat-0.2.2/fastchat/serve/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/gradio_web_server.py` & `fschat-0.2.2/fastchat/serve/gradio_web_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 from fastchat.conversation import (get_default_conv_template,
                                    SeparatorStyle)
 from fastchat.constants import LOGDIR
 from fastchat.utils import (build_logger, server_error_msg,
     violates_moderation, moderation_msg)
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_css import code_highlight_css
+from fastchat.serve.inference import compute_skip_echo_len
 
 
 logger = build_logger("gradio_web_server", "gradio_web_server.log")
 
 headers = {"User-Agent": "fastchat Client"}
 
 no_change_btn = gr.Button.update()
 enable_btn = gr.Button.update(interactive=True)
 disable_btn = gr.Button.update(interactive=False)
 
 priority = {
     "vicuna-13b": "aaaaaaa",
     "koala-13b": "aaaaaab",
-    "chatglm-6b": "aaaaaac",
+    "dolly-v2-12b": "aaaaaac",
+    "chatglm-6b": "aaaaaad",
 }
 
 
 def get_conv_log_filename():
     t = datetime.datetime.now()
     name = os.path.join(LOGDIR, f"{t.year}-{t.month:02d}-{t.day:02d}-conv.json")
     return name
@@ -134,27 +136,29 @@
     logger.info(f"clear_history. ip: {request.client.host}")
     state = None
     return (state, [], "") + (disable_btn,) * 5
 
 
 def add_text(state, text, request: gr.Request):
     logger.info(f"add_text. ip: {request.client.host}. len: {len(text)}")
+
+    if state is None:
+        state = get_default_conv_template("vicuna").copy()
+
     if len(text) <= 0:
         state.skip_next = True
         return (state, state.to_gradio_chatbot(), "") + (no_change_btn,) * 5
     if args.moderate:
         flagged = violates_moderation(text)
         if flagged:
+            logger.info(f"violate moderation. ip: {request.client.host}. text: {text}")
             state.skip_next = True
             return (state, state.to_gradio_chatbot(), moderation_msg) + (
                 no_change_btn,) * 5
 
-    if state is None:
-        state = get_default_conv_template("vicuna").copy()
-
     text = text[:1536]  # Hard cut-off
     state.append_message(state.roles[0], text)
     state.append_message(state.roles[1], None)
     state.skip_next = False
     return (state, state.to_gradio_chatbot(), "") + (disable_btn,) * 5
 
 
@@ -199,18 +203,17 @@
         state.messages[-1][-1] = server_error_msg
         yield (state, state.to_gradio_chatbot(), disable_btn, disable_btn, disable_btn, enable_btn, enable_btn)
         return
 
     # Construct prompt
     if "chatglm" in model_name:
         prompt = state.messages[state.offset:]
-        skip_echo_len = len(state.messages[-2][1]) + 1
     else:
         prompt = state.get_prompt()
-        skip_echo_len = len(prompt.replace("</s>", " ")) + 1
+    skip_echo_len = compute_skip_echo_len(model_name, state, prompt)
 
     # Make requests
     pload = {
         "model": model_name,
         "prompt": prompt,
         "temperature": float(temperature),
         "max_new_tokens": int(max_new_tokens),
@@ -261,29 +264,28 @@
             "ip": request.client.host,
         }
         fout.write(json.dumps(data) + "\n")
 
 
 notice_markdown = ("""
 # 🏔️ Chat with Open Large Language Models
-- Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://vicuna.lmsys.org) [[GitHub]](https://github.com/lm-sys/FastChat)
+- Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://vicuna.lmsys.org) [[GitHub]](https://github.com/lm-sys/FastChat) [[Evaluation]](https://vicuna.lmsys.org/eval/)
 - Koala: A Dialogue Model for Academic Research. [[Blog post]](https://bair.berkeley.edu/blog/2023/04/03/koala/) [[GitHub]](https://github.com/young-geng/EasyLM)
 - This demo server. [[GitHub]](https://github.com/lm-sys/FastChat)
 
 ### Terms of use
 By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. The service may collect user dialogue data for future research.
 
 ### Choose a model to chat with
 - [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations. This one is expected to perform best according to our evaluation.
 - [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a chatbot fine-tuned from LLaMA on user-shared conversations and open-source datasets. This one performs similarly to Vicuna.
+- [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open LLM by Databricks.
 - [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model | 开源双语对话语言模型
 - [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on 52K instruction-following demonstrations.
-- [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models
-
-Note: If you are waiting in the queue, check out more benchmark results from GPT-4 on a static website [here](https://vicuna.lmsys.org/eval).
+- [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models.
 """)
 
 
 learn_more_markdown = ("""
 ### License
 The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
 """)
@@ -347,14 +349,16 @@
             [state, model_selector], [textbox, upvote_btn, downvote_btn, flag_btn])
         regenerate_btn.click(regenerate, state,
             [state, chatbot, textbox] + btn_list).then(
             http_bot, [state, model_selector, temperature, max_output_tokens],
             [state, chatbot] + btn_list)
         clear_btn.click(clear_history, None, [state, chatbot, textbox] + btn_list)
 
+        model_selector.change(clear_history, None, [state, chatbot, textbox] + btn_list)
+
         textbox.submit(add_text, [state, textbox], [state, chatbot, textbox] + btn_list
             ).then(http_bot, [state, model_selector, temperature, max_output_tokens],
                    [state, chatbot] + btn_list)
         submit_btn.click(add_text, [state, textbox], [state, chatbot, textbox] + btn_list
             ).then(http_bot, [state, model_selector, temperature, max_output_tokens],
                    [state, chatbot] + btn_list)
```

### Comparing `fschat-0.2.1/fastchat/serve/huggingface_api.py` & `fschat-0.2.2/fastchat/serve/huggingface_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+"""
+Usage:
+python3 -m fastchat.serve.huggingface_api --model ~/model_weights/vicuna-7b/
+"""
 import argparse
 import json
 
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
 from fastchat.conversation import get_default_conv_template
-from fastchat.serve.inference import load_model
+from fastchat.serve.inference import load_model, compute_skip_echo_len
 
 
 @torch.inference_mode()
 def main(args):
     model, tokenizer = load_model(args.model_path, args.device,
-        args.num_gpus, args.load_8bit, debug=args.debug)
+        args.num_gpus, args.max_gpu_memory, args.load_8bit, debug=args.debug)
 
     msg = args.message
 
     conv = get_default_conv_template(args.model_path).copy()
     conv.append_message(conv.roles[0], msg)
     conv.append_message(conv.roles[1], None)
     prompt = conv.get_prompt()
@@ -23,27 +27,28 @@
     inputs = tokenizer([prompt])
     output_ids = model.generate(
         torch.as_tensor(inputs.input_ids).cuda(),
         do_sample=True,
         temperature=0.7,
         max_new_tokens=1024)
     outputs = tokenizer.batch_decode(output_ids, skip_special_tokens=True)[0]
-    skip_echo_len = len(prompt.replace("</s>", " ")) + 1
+    skip_echo_len = compute_skip_echo_len(args.model_path, conv, prompt)
     outputs = outputs[skip_echo_len:]
 
     print(f"{conv.roles[0]}: {msg}")
     print(f"{conv.roles[1]}: {outputs}")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--model-path", type=str, default="facebook/opt-350m",
         help="The path to the weights")
     parser.add_argument("--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda")
     parser.add_argument("--num-gpus", type=str, default="1")
+    parser.add_argument("--max-gpu-memory", type=str, default="13GiB")
     parser.add_argument("--load-8bit", action="store_true",
         help="Use 8-bit quantization.")
     parser.add_argument("--conv-template", type=str, default=None,
         help="Conversation prompt template.")
     parser.add_argument("--temperature", type=float, default=0.7)
     parser.add_argument("--max-new-tokens", type=int, default=512)
     parser.add_argument("--debug", action="store_true")
```

### Comparing `fschat-0.2.1/fastchat/serve/inference.py` & `fschat-0.2.2/fastchat/serve/inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,91 @@
 """Inference for FastChat models."""
 import abc
 from typing import Optional
+import warnings
 
 import torch
 try:
-    from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer, AutoModel
+    from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer, LlamaForCausalLM, AutoModel, LlamaForCausalLM
 except ImportError:
-    from transformers import AutoTokenizer, AutoModelForCausalLM, LLaMATokenizer, AutoModel
+    from transformers import AutoTokenizer, AutoModelForCausalLM, LLaMATokenizer, LLamaForCausalLM, AutoModel
 
 from fastchat.conversation import conv_templates, get_default_conv_template, SeparatorStyle
 from fastchat.serve.compression import compress_module
 from fastchat.serve.monkey_patch_non_inplace import replace_llama_attn_with_non_inplace_operations
 from fastchat.serve.serve_chatglm import chatglm_generate_stream
 
 
-def load_model(model_path, device, num_gpus, load_8bit=False, debug=False):
+def raise_warning_for_old_weights(model_path, model):
+    if "vicuna" in model_path.lower():
+        try:
+            is_vicuna = isinstance(model, LlamaForCausalLM)
+        except Exception:
+            is_vicuna = isinstance(model, LLamaForCausalLM)
+        if is_vicuna and model.model.vocab_size > 32000:
+            warnings.warn(
+                "\nYou are probably using the old Vicuna-v0 model, "
+                "which will generate unexpected results with the "
+                "current fschat.\nYou can try one of the following methods:\n"
+                "1. Upgrade your weights to the new Vicuna-v1.1: https://github.com/lm-sys/FastChat#vicuna-weights.\n"
+                "2. Use the old conversation template by `python3 -m fastchat.serve.cli --model-path /path/to/vicuna-v0 --conv-template conv_one_shot`\n"
+                "3. Downgrade fschat to fschat==0.1.10 (Not recommonded).\n")
+
+
+def compute_skip_echo_len(model_name, conv, prompt):
+    model_name = model_name.lower()
+    if "chatglm" in model_name:
+        skip_echo_len = len(conv.messages[-2][1]) + 1
+    elif "dolly" in model_name:
+        special_toks = ["### Instruction:", "### Response:", "### End"]
+        prompt_tmp = prompt
+        for tok in special_toks:
+            prompt_tmp = prompt_tmp.replace(tok, "")
+        skip_echo_len = len(prompt_tmp)
+    else:
+        skip_echo_len = len(prompt) + 1 - prompt.count("</s>") * 3
+    return skip_echo_len
+
+
+def load_model(model_path, device, num_gpus, max_gpu_memory="13GiB",
+               load_8bit=False, debug=False):
     if device == "cpu":
         kwargs = {}
     elif device == "cuda":
         kwargs = {"torch_dtype": torch.float16}
         if num_gpus == "auto":
             kwargs["device_map"] = "auto"
         else:
             num_gpus = int(num_gpus)
             if num_gpus != 1:
                 kwargs.update({
                     "device_map": "auto",
-                    "max_memory": {i: "13GiB" for i in range(num_gpus)},
+                    "max_memory": {i: max_gpu_memory for i in range(num_gpus)},
                 })
     elif device == "mps":
         kwargs = {"torch_dtype": torch.float16}
         # Avoid bugs in mps backend by not using in-place operations.
         replace_llama_attn_with_non_inplace_operations()
     else:
         raise ValueError(f"Invalid device: {device}")
 
     if "chatglm" in model_path:
         tokenizer = AutoTokenizer.from_pretrained(model_path, trust_remote_code=True)
         model = AutoModel.from_pretrained(model_path, trust_remote_code=True).half().cuda()
+    elif "dolly" in model_path:
+        kwargs.update({"torch_dtype": torch.bfloat16})
+        tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
+        # 50277 means "### End"
+        tokenizer.eos_token_id = 50277
+        model = AutoModelForCausalLM.from_pretrained(model_path, low_cpu_mem_usage=True, **kwargs)
     else:
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
         model = AutoModelForCausalLM.from_pretrained(model_path,
             low_cpu_mem_usage=True, **kwargs)
+        raise_warning_for_old_weights(model_path, model)
 
     if load_8bit:
         compress_module(model, device)
 
     if (device == "cuda" and num_gpus == 1) or device == "mps":
         model.to(device)
 
@@ -75,19 +115,16 @@
     for i in range(max_new_tokens):
         if i == 0:
             out = model(
                 torch.as_tensor([input_ids], device=device), use_cache=True)
             logits = out.logits
             past_key_values = out.past_key_values
         else:
-            attention_mask = torch.ones(
-                1, past_key_values[0][0].shape[-2] + 1, device=device)
             out = model(input_ids=torch.as_tensor([[token]], device=device),
                         use_cache=True,
-                        attention_mask=attention_mask,
                         past_key_values=past_key_values)
             logits = out.logits
             past_key_values = out.past_key_values
 
         last_token_logits = logits[0][-1]
 
         if device == "mps":
@@ -132,21 +169,22 @@
         """Prompt for output from a role."""
 
     @abc.abstractmethod
     def stream_output(self, output_stream, skip_echo_len: int):
         """Stream output."""
 
 
-def chat_loop(model_path: str, device: str, num_gpus: str, load_8bit: bool,
+def chat_loop(model_path: str, device: str, num_gpus: str,
+              max_gpu_memory: str, load_8bit: bool,
               conv_template: Optional[str], temperature: float,
               max_new_tokens: int, chatio: ChatIO,
               debug: bool):
     # Model
     model, tokenizer = load_model(model_path, device,
-        num_gpus, load_8bit, debug)
+        num_gpus, max_gpu_memory, load_8bit, debug)
     is_chatglm = "chatglm" in str(type(model)).lower()
 
     # Chat
     if conv_template:
         conv = conv_templates[conv_template].copy()
     else:
         conv = get_default_conv_template(model_path).copy()
@@ -162,19 +200,19 @@
 
         conv.append_message(conv.roles[0], inp)
         conv.append_message(conv.roles[1], None)
 
         if is_chatglm:
             prompt = conv.messages[conv.offset:]
             generate_stream_func = chatglm_generate_stream
-            skip_echo_len = len(conv.messages[-2][1]) + 1
         else:
             generate_stream_func = generate_stream
             prompt = conv.get_prompt()
-            skip_echo_len = len(prompt.replace("</s>", " ")) + 1
+
+        skip_echo_len = compute_skip_echo_len(model_path, conv, prompt)
 
         params = {
             "model": model_path,
             "prompt": prompt,
             "temperature": temperature,
             "max_new_tokens": max_new_tokens,
             "stop": conv.sep if conv.sep_style == SeparatorStyle.SINGLE else conv.sep2,
```

### Comparing `fschat-0.2.1/fastchat/serve/model_worker.py` & `fschat-0.2.2/fastchat/serve/model_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,26 +42,26 @@
         time.sleep(WORKER_HEART_BEAT_INTERVAL)
         controller.send_heart_beat()
 
 
 class ModelWorker:
     def __init__(self, controller_addr, worker_addr,
                  worker_id, no_register, model_path, model_name,
-                 device, num_gpus, load_8bit=False):
+                 device, num_gpus, max_gpu_memory, load_8bit=False):
         self.controller_addr = controller_addr
         self.worker_addr = worker_addr
         self.worker_id = worker_id
         if model_path.endswith("/"):
             model_path = model_path[:-1]
         self.model_name = model_name or model_path.split("/")[-1]
         self.device = device
 
         logger.info(f"Loading the model {self.model_name} on worker {worker_id} ...")
         self.model, self.tokenizer = load_model(
-            model_path, device, num_gpus, load_8bit)
+            model_path, device, num_gpus, max_gpu_memory, load_8bit)
 
         if hasattr(self.model.config, "max_sequence_length"):
             self.context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
             self.context_len = self.model.config.max_position_embeddings
         else:
             self.context_len = 2048
@@ -179,14 +179,15 @@
         default="http://localhost:21001")
     parser.add_argument("--model-path", type=str, default="facebook/opt-350m",
         help="The path to the weights")
     parser.add_argument("--model-name", type=str,
         help="Optional name")
     parser.add_argument("--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda")
     parser.add_argument("--num-gpus", type=int, default=1)
+    parser.add_argument("--max-gpu-memory", type=str, default="13GiB")
     parser.add_argument("--load-8bit", action="store_true")
     parser.add_argument("--limit-model-concurrency", type=int, default=5)
     parser.add_argument("--stream-interval", type=int, default=2)
     parser.add_argument("--no-register", action="store_true")
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
@@ -194,9 +195,10 @@
                          args.worker_address,
                          worker_id,
                          args.no_register,
                          args.model_path,
                          args.model_name,
                          args.device,
                          args.num_gpus,
+                         args.max_gpu_memory,
                          args.load_8bit)
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
```

### Comparing `fschat-0.2.1/fastchat/serve/monkey_patch_non_inplace.py` & `fschat-0.2.2/fastchat/serve/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/register_worker.py` & `fschat-0.2.2/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/serve_chatglm.py` & `fschat-0.2.2/fastchat/serve/serve_chatglm.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/serve/test_message.py` & `fschat-0.2.2/fastchat/serve/test_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import json
 
 import requests
 
 from fastchat.conversation import get_default_conv_template, SeparatorStyle
+from fastchat.serve.inference import compute_skip_echo_len
 
 
 def main():
     model_name = args.model_name
 
     if args.worker_address:
         worker_addr = args.worker_address
@@ -43,15 +44,15 @@
     response = requests.post(worker_addr + "/worker_generate_stream", headers=headers,
             json=pload, stream=True)
 
     print(f"{conv.roles[0]}: {args.message}")
     for chunk in response.iter_lines(chunk_size=8192, decode_unicode=False, delimiter=b"\0"):
         if chunk:
             data = json.loads(chunk.decode("utf-8"))
-            skip_echo_len = len(prompt.replace("</s>", " ")) + 1
+            skip_echo_len = compute_skip_echo_len(model_name, conv, prompt)
             output = data["text"][skip_echo_len:].strip()
             print(f"{conv.roles[1]}: {output}", end="\r")
     print("")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
```

### Comparing `fschat-0.2.1/fastchat/serve/test_throughput.py` & `fschat-0.2.2/fastchat/serve/test_throughput.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.2/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/train/train.py` & `fschat-0.2.2/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.1/fastchat/train/train_lora.py` & `fschat-0.2.2/fastchat/train/train_lora.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import pathlib
 import typing
 
 from peft import (
     LoraConfig,
     get_peft_model,
 )
@@ -33,21 +33,21 @@
 
 IGNORE_INDEX = -100
 DEFAULT_PAD_TOKEN = "[PAD]"
 DEFAULT_EOS_TOKEN = "</s>"
 DEFAULT_BOS_TOKEN = "</s>"
 DEFAULT_UNK_TOKEN = "</s>"
 
-# TODO: the lora_target_modules cannot support list
+
 @dataclass
 class LoraArguments:
-    lora_r: int = 8,
-    lora_alpha: int = 16,
-    lora_dropout: float = 0.05,
-    lora_target_modules: typing.List[str] = ["q_proj", "v_proj"],
+    lora_r: int = 8
+    lora_alpha: int = 16
+    lora_dropout: float = 0.05
+    lora_target_modules: typing.List[str] = field(default_factory=lambda: ["q_proj", "v_proj"])
     lora_weight_path: str = ""
 
 def train():
     parser = transformers.HfArgumentParser(
         (ModelArguments, DataArguments, TrainingArguments, LoraArguments))
     (model_args, data_args, training_args,
      lora_args) = parser.parse_args_into_dataclasses()
@@ -55,15 +55,15 @@
     model = transformers.LlamaForCausalLM.from_pretrained(
         model_args.model_name_or_path,
         cache_dir=training_args.cache_dir,
     )
     lora_config = LoraConfig(
         r=lora_args.lora_r,
         lora_alpha=lora_args.lora_alpha,
-        target_modules=["q_proj", "v_proj"],
+        target_modules=lora_args.lora_target_modules,
         lora_dropout=lora_args.lora_dropout,
         bias="none",
         task_type="CAUSAL_LM",
     )
     model = get_peft_model(model, lora_config)
     model.print_trainable_parameters()
```

### Comparing `fschat-0.2.1/fastchat/utils.py` & `fschat-0.2.2/fastchat/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
 import logging
 import logging.handlers
 import os
 import sys
+import json
 
 import requests
+import torch
 
 from fastchat.constants import LOGDIR
 
 server_error_msg = "**NETWORK ERROR DUE TO HIGH TRAFFIC. PLEASE REGENERATE OR REFRESH THIS PAGE.**"
 moderation_msg = "YOUR INPUT VIOLATES OUR CONTENT MODERATION GUIDELINES. PLEASE TRY AGAIN."
 
 handler = None
@@ -117,12 +119,28 @@
     except requests.exceptions.RequestException as e:
         flagged = False
     except KeyError as e:
         flagged = False
 
     return flagged
 
+# Flan-t5 trained with HF+FSDP saves corrupted  weights for shared embeddings,
+# Use this function to make sure it can be correctly loaded.
+def clean_flant5_ckpt(ckpt_path):
+    index_file = os.path.join(ckpt_path, "pytorch_model.bin.index.json")
+    index_json = json.load(open(index_file, "r"))
+
+    weightmap = index_json["weight_map"]
+
+    share_weight_file = weightmap["shared.weight"]
+    share_weight = torch.load(os.path.join(ckpt_path, share_weight_file))["shared.weight"]
+
+    for weight_name in ["decoder.embed_tokens.weight","encoder.embed_tokens.weight"]:
+        weight_file = weightmap[weight_name]
+        weight = torch.load(os.path.join(ckpt_path, weight_file))
+        weight[weight_name] = share_weight
+        torch.save(weight, os.path.join(ckpt_path, weight_file))
 
 def pretty_print_semaphore(semaphore):
     if semaphore is None:
         return "None"
     return f"Semaphore(value={semaphore._value}, locked={semaphore.locked()})"
```

### Comparing `fschat-0.2.1/fschat.egg-info/PKG-INFO` & `fschat-0.2.2/fschat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.1
+Version: 0.2.2
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -35,19 +35,15 @@
 - [Fine-tuning](#fine-tuning)
 
 ## Install
 
 ### Method 1: With pip
 
 ```bash
-# Install FastChat
 pip3 install fschat
-
-# Install the latest main branch of huggingface/transformers
-pip3 install git+https://github.com/huggingface/transformers
 ```
 
 ### Method 2: From source
 
 1. Clone this repository and navigate to the FastChat folder
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
@@ -69,40 +65,46 @@
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
-Our released weights are only compatible with the latest main branch of huggingface/transformers.
-We install the correct version of transformers when fastchat is installed.
+Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
+Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
-If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
+See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-7b \
     --target /output/path/to/vicuna-7b \
     --delta lmsys/vicuna-7b-delta-v1.1
 ```
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
-If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
+See the "Low CPU Memory Conversion" section below if you do not have enough memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-13b \
     --target /output/path/to/vicuna-13b \
     --delta lmsys/vicuna-13b-delta-v1.1
 ```
 
 ### Old weights
 See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
 
+
+### Low CPU Memory Conversion
+You can try these methods to reduce the CPU RAM requirement of weight conversion.
+1. Append `--low-cpu-mem` to the commands above, which will split large weight files into smaller ones and use the disk as temporary storage. This can keep the peak memory at less than 16GB.
+2. Create a large swap file and rely on the operating system to automatically utilize the disk as virtual memory.
+
 ## Inference with Command Line Interface
 
 (Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
 #### Single GPU
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.1 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.2 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
@@ -11,74 +11,77 @@
 ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
 [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
 (https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
 twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
 (#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-
-tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash # Install
-FastChat pip3 install fschat # Install the latest main branch of huggingface/
-transformers pip3 install git+https://github.com/huggingface/transformers ```
-### Method 2: From source 1. Clone this repository and navigate to the FastChat
-folder ```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ```
-If you are running on Mac: ```bash brew install rust cmake ``` 2. Install
-Package ```bash pip3 install --upgrade pip # enable PEP 660 support pip3
-install -e . ``` ## Vicuna Weights We release [Vicuna](https://
+tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash pip3 install
+fschat ``` ### Method 2: From source 1. Clone this repository and navigate to
+the FastChat folder ```bash git clone https://github.com/lm-sys/FastChat.git cd
+FastChat ``` If you are running on Mac: ```bash brew install rust cmake ``` 2.
+Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
+pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
 vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
 license. You can add our delta to the original LLaMA weights to obtain the
 Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
 huggingface format by following the instructions [here](https://huggingface.co/
 docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
 Vicuna weights by applying our delta. They will automatically download delta
 weights from our Hugging Face [account](https://huggingface.co/lmsys).
-**NOTE**: Our released weights are only compatible with the latest main branch
-of huggingface/transformers. We install the correct version of transformers
-when fastchat is installed. ### Vicuna-7B This conversion command needs around
-30 GB of CPU RAM. If you do not have enough memory, you can create a large swap
-file that allows the operating system to automatically utilize the disk as
-virtual memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/
-to/llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-
-delta-v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU
-RAM. If you do not have enough memory, you can create a large swap file that
-allows the operating system to automatically utilize the disk as virtual
+**NOTE**: Weights v1.1 are only compatible with ```transformers>=4.28.0``` and
+``fschat >= 0.2.0``. Please update your local packages accordingly. If you
+follow the above commands to do a fresh install, then you should get all the
+correct versions. ### Vicuna-7B This conversion command needs around 30 GB of
+CPU RAM. See the "Low CPU Memory Conversion" section below if you do not have
+enough memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/
+llama-7b \ --target /output/path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-
+v1.1 ``` ### Vicuna-13B This conversion command needs around 60 GB of CPU RAM.
+See the "Low CPU Memory Conversion" section below if you do not have enough
 memory. ```bash python3 -m fastchat.model.apply_delta \ --base /path/to/llama-
 13b \ --target /output/path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1
 ``` ### Old weights See [docs/weights_version.md](docs/weights_version.md) for
-all versions of weights and their differences. ## Inference with Command Line
-Interface (Experimental Feature: You can specify `--style rich` to enable rich
-text output and better text streaming quality for some non-ASCII content. This
-may not work properly on certain terminals.) [assets/screenshot_cli.png] ####
-Single GPU The command below requires around 28GB of GPU memory for Vicuna-13B
-and 14GB of GPU memory for Vicuna-7B. See the "No Enough Memory" section below
-if you do not have enough memory. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/vicuna/weights ``` #### Multiple GPUs You can use model
-parallelism to aggregate GPU memory from multiple GPUs on the same machine. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
-``` #### CPU Only This runs on the CPU only and does not require GPU. It
-requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory
-for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/
-weights --device cpu ``` #### Metal Backend (Mac Computers with Apple Silicon
-or AMD GPUs) Use `--device mps` to enable GPU acceleration on Mac computers
-(requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit compression. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps
---load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words /
-second. #### No Enough Memory or Other Platforms If you do not have enough
-memory, you can enable 8-bit compression by adding `--load-8bit` to commands
-above. This can reduce memory usage by around half with slightly degraded model
-quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
-8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU. ```
-python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
-``` Besides, we are actively exploring more methods to make the model easier to
-run on more platforms. Contributions and pull requests are welcome. ## Serving
-with Web GUI [assets/screenshot_gui.png] To serve using the web UI, you need
-three main components: web servers that interface with users, model workers
-that host one or more models, and a controller to coordinate the webserver and
-model workers. Here are the commands to follow in your terminal: #### Launch
-the controller ```bash python3 -m fastchat.serve.controller ``` This controller
-manages the distributed workers. #### Launch the model worker ```bash python3 -
+all versions of weights and their differences. ### Low CPU Memory Conversion
+You can try these methods to reduce the CPU RAM requirement of weight
+conversion. 1. Append `--low-cpu-mem` to the commands above, which will split
+large weight files into smaller ones and use the disk as temporary storage.
+This can keep the peak memory at less than 16GB. 2. Create a large swap file
+and rely on the operating system to automatically utilize the disk as virtual
+memory. ## Inference with Command Line Interface (Experimental Feature: You can
+specify `--style rich` to enable rich text output and better text streaming
+quality for some non-ASCII content. This may not work properly on certain
+terminals.) [assets/screenshot_cli.png] #### Single GPU The command below
+requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
+Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
+memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
+from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
+the CPU only and does not require GPU. It requires around 60GB of CPU memory
+for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
+Other Platforms If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
+--model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+exploring more methods to make the model easier to run on more platforms.
+Contributions and pull requests are welcome. ## Serving with Web GUI [assets/
+screenshot_gui.png] To serve using the web UI, you need three main components:
+web servers that interface with users, model workers that host one or more
+models, and a controller to coordinate the webserver and model workers. Here
+are the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
```

### Comparing `fschat-0.2.1/fschat.egg-info/SOURCES.txt` & `fschat-0.2.2/fschat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 fastchat/serve/monkey_patch_non_inplace.py
 fastchat/serve/register_worker.py
 fastchat/serve/serve_chatglm.py
 fastchat/serve/test_message.py
 fastchat/serve/test_throughput.py
 fastchat/train/llama_flash_attn_monkey_patch.py
 fastchat/train/train.py
+fastchat/train/train_flant5.py
 fastchat/train/train_lora.py
 fastchat/train/train_mem.py
 fschat.egg-info/PKG-INFO
 fschat.egg-info/SOURCES.txt
 fschat.egg-info/dependency_links.txt
 fschat.egg-info/requires.txt
 fschat.egg-info/top_level.txt
```

### Comparing `fschat-0.2.1/pyproject.toml` & `fschat-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.2.1"
+version = "0.2.2"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "accelerate", "fastapi", "gradio==3.23", "markdown2[all]", "numpy",
-    "requests", "sentencepiece", "tokenizers>=0.12.1",
-    "torch", "uvicorn", "wandb", "prompt_toolkit>=3.0.0", "rich>=10.0.0",
+    "prompt_toolkit>=3.0.0", "requests", "rich>=10.0.0", "sentencepiece",
+    "shortuuid", "transformers>=4.28.0", "tokenizers>=0.12.1", "torch",
+    "uvicorn", "wandb",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lm-sys/fastchat"
 "Bug Tracker" = "https://github.com/lm-sys/fastchat/issues"
 
 [tool.setuptools.packages.find]
```

