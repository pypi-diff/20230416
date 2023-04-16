# Comparing `tmp/whisper-ctranslate2-0.1.8.tar.gz` & `tmp/whisper-ctranslate2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.1.8.tar", last modified: Fri Apr 14 15:18:48 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.1.9.tar", last modified: Sun Apr 16 15:31:45 2023, max compression
```

## Comparing `whisper-ctranslate2-0.1.8.tar` & `whisper-ctranslate2-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-14 15:18:48.537725 whisper-ctranslate2-0.1.8/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.8/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-14 15:18:48.537725 whisper-ctranslate2-0.1.8/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3558 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.8/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-14 15:18:48.537725 whisper-ctranslate2-0.1.8/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-14 14:47:47.000000 whisper-ctranslate2-0.1.8/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-14 15:18:48.533725 whisper-ctranslate2-0.1.8/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-14 15:18:48.533725 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4620 2023-04-14 12:45:32.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4674 2023-04-10 14:05:51.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6124 2023-04-14 14:47:43.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-12 17:52:10.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13134 2023-04-14 14:38:43.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-14 15:18:48.533725 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      554 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       98 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-16 15:31:45.129989 whisper-ctranslate2-0.1.9/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.9/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5510 2023-04-16 15:31:45.129989 whisper-ctranslate2-0.1.9/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4859 2023-04-16 12:50:08.000000 whisper-ctranslate2-0.1.9/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-16 15:31:45.129989 whisper-ctranslate2-0.1.9/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-14 14:47:47.000000 whisper-ctranslate2-0.1.9/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-16 15:31:45.125990 whisper-ctranslate2-0.1.9/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-16 15:31:45.125990 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4620 2023-04-14 12:45:32.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4674 2023-04-16 13:14:32.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6124 2023-04-16 13:29:56.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-14 15:20:03.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13377 2023-04-16 13:34:29.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-16 13:22:55.000000 whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-16 15:31:45.129989 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5510 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      554 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       98 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-16 15:31:45.000000 whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.1.8/LICENSE` & `whisper-ctranslate2-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.8/PKG-INFO` & `whisper-ctranslate2-0.1.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: whisper-ctranslate2
-Version: 0.1.8
-Summary: Whisper command line client that uses CTranslate2
-Home-page: https://github.com/jordimas/whisper-ctranslate2
-Author: Jordi Mas
-Author-email: jmas@softcatala.org
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 [![PyPI version](https://img.shields.io/pypi/v/whisper-ctranslate2.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/whisper-ctranslate2/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/whisper-ctranslate2.svg)](https://pypistats.org/packages/whisper-ctranslate2)
 
 # Introduction
 
 Whisper command line client compatible with original [OpenAI client](https://github.com/openai/whisper) based on CTranslate2.
 
@@ -28,25 +9,35 @@
 
 Goals of the project:
 * Provide an easy way to use the CTranslate2 Whisper implementation
 * Ease the migration for people using OpenAI Whisper CLI
 
 # Installation
 
-Just type:
+To install the latest stable version, just type:
 
     pip install -U whisper-ctranslate2
 
-Alternatively, the following command will pull and install the latest commit from this repository, along with its Python dependencies:
+Alternatively, if you are interested the latest development (non-stable) version from this repository, just tpe:
 
     pip install git+https://github.com/jordimas/whisper-ctranslate2.git
+
+# CPU and GPU support
+
+GPU and CPU support are provided by [CTranslate2](https://github.com/OpenNMT/CTranslate2/).
+
+It has compatibility with x86-64 and AArch64/ARM64 CPU and integrates multiple backends that are optimized for these platforms: Intel MKL, oneDNN, OpenBLAS, Ruy, and Apple Accelerate.
+
+GPU execution requires the NVIDIA libraries cuBLAS 11.x and cuDNN 8.x to be installed on the system. Please refer to the [CTranslate2 documentation](https://opennmt.net/CTranslate2/installation.html)
+
+By default the best hardware available is selected for inference. You can use the options `--device` and `--device_index` to control manually the selection.
     
 # Usage
 
-Same command line that OpenAI whisper.
+Same command line that OpenAI Whisper.
 
 To transcribe:
 
     whisper-ctranslate2 inaguracio2011.mp3 --model medium
     
 <img alt="image" src="https://user-images.githubusercontent.com/309265/226923541-8326c575-7f43-4bba-8235-2a4a8bdfb161.png">
 
@@ -60,55 +51,63 @@
 
     whisper-ctranslate2 --help
 
 All the supported options with their help are shown.
 
 # CTranslate2 specific options
 
-On top of the OpenAI Whisper command line options, there are some specific options provided by CTranslate2 .
+On top of the OpenAI Whisper command line options, there are some specific options provided by CTranslate2 or whiper-ctranslate2.
+
+## Quantization
 
-    --compute_type {default,auto,int8,int8_float16,int16,float16,float32}
+`--compute_type` option which accepts _default,auto,int8,int8_float16,int16,float16,float32_ values indicates the type of [quantization](https://opennmt.net/CTranslate2/quantization.html) to use. On CPU _int8_ will give the best performance:
 
-Type of [quantization](https://opennmt.net/CTranslate2/quantization.html) to use. On CPU _int8_ will give the best performance.
+    whisper-ctranslate2 myfile.mp3 --compute_type int8
 
-    --model_directory MODEL_DIRECTORY
+## Loading the model from a directory
 
-Directory where to find a CTranslate Whisper model, for example a fine-tunned Whisper model. The model should be in CTranslate2 format.
+`--model_directory` option allows to specify the directory from which you want to load a CTranslate2 Whisper model. For example, if you want to load your own quantified [Whisper model](https://opennmt.net/CTranslate2/conversion.html) version or using your own [Whisper fine-tunned](https://github.com/huggingface/community-events/tree/main/whisper-fine-tuning-event) version. The model must be in CTranslate2 format.
 
-    --device_index [DEVICE_INDEX ...]
+## Using Voice Activity Detection (VAD) filter
 
-Device IDs where to place this model on
+`--vad_filter` option enables the voice activity detection (VAD) to filter out parts of the audio without speech. This step uses the [Silero VAD model](https://github.com/snakers4/silero-vad):
 
-    --vad_filter VAD_FILTER
+    whisper-ctranslate2 myfile.mp3 --vad_filter True
 
-Enable the voice activity detection (VAD) to filter out parts of the audio without speech. This step is using the Silero VAD model https://github.com/snakers4/silero-vad.
+The VAD filter accepts multiple additional options to determine the filter behavior:
 
-    --vad_min_silence_duration_ms VAD_MIN_SILENCE_DURATION_MS
+    --vad_threshold VALUE (float)
 
-When `vad_filter` is enabled, audio segments without speech for at least this number of milliseconds will be ignored.
+Probabilities above this value are considered as speech.
 
+    --vad_min_speech_duration_ms (int)
 
-# Whisper-ctranslate2 specific options
+Final speech chunks shorter min_speech_duration_ms are thrown out.
 
-On top of the OpenAI Whisper and CTranslate2, whisper-ctranslate2 provides some additional specific options:
+    --vad_max_speech_duration_s VALUE (int)
 
-    --print-colors PRINT_COLORS
+Maximum duration of speech chunks in seconds. Longer will be split at the timestamp of the last silence.
 
-Adding the `--print_colors True` argument will print the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
+
+## Print colors
+
+`--print_colors True` options prints the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
+
+    whisper-ctranslate2 myfile.mp3 --print_colors True
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
-    --live_transcribe
+## Live transcribe from your microphone
 
-Adding the `----live_transcribe True` will activate the live transcription mode from your microphone.
+`----live_transcribe True` option activates the live transcription mode from your microphone:
+
+    whisper-ctranslate2 myfile.mp3 --print_colors True
 
 https://user-images.githubusercontent.com/309265/231533784-e58c4b92-e9fb-4256-b4cd-12f1864131d9.mov
 
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
 
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
-
-
```

### Comparing `whisper-ctranslate2-0.1.8/setup.py` & `whisper-ctranslate2-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/live.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/models.py` & `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/models.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,22 @@
         "--append_punctuations",
         type=str,
         default="\"'.。,，!！?？:：”)]}、",
         help="if word_timestamps is True, merge these punctuation symbols with the previous word",
     )
 
     parser.add_argument(
-        "--device", default="auto", help="device to use for CTranslate2 inference"
+        "--device",
+        choices=[
+            "auto",
+            "cpu",
+            "cuda",
+        ],
+        default="auto",
+        help="device to use for CTranslate2 inference",
     )
 
     parser.add_argument(
         "--vad_filter",
         type=bool,
         default=False,
         help="Enable the voice activity detection (VAD) to filter out parts of the audio without speech. This step is using the Silero VAD model https://github.com/snakers4/silero-vad.",
@@ -349,14 +356,15 @@
         )
 
     if options.print_colors and output_dir and not options.word_timestamps:
         print(
             "Print colors requires word-level time stamps. Generated files in output directory will have word-level timestamps"
         )
 
+    output_dir = os.path.abspath(output_dir)
     if model_directory:
         model_filename = os.path.join(model_directory, "model.bin")
         if not os.path.exists(model_filename):
             raise RuntimeError(f"Model file '{model_filename}' does not exists")
         model_dir = model_directory
     else:
         model_dir = Models(cache_directory).get_model_dir(model)
@@ -393,10 +401,13 @@
             verbose,
             False,
             options,
         )
         writer = get_writer(output_format, output_dir)
         writer(result, audio_path)
 
+    if verbose:
+        print(f"Transcription results written to '{output_dir}' directory")
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.1.9/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.8
+Version: 0.1.9
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -28,25 +28,35 @@
 
 Goals of the project:
 * Provide an easy way to use the CTranslate2 Whisper implementation
 * Ease the migration for people using OpenAI Whisper CLI
 
 # Installation
 
-Just type:
+To install the latest stable version, just type:
 
     pip install -U whisper-ctranslate2
 
-Alternatively, the following command will pull and install the latest commit from this repository, along with its Python dependencies:
+Alternatively, if you are interested the latest development (non-stable) version from this repository, just tpe:
 
     pip install git+https://github.com/jordimas/whisper-ctranslate2.git
+
+# CPU and GPU support
+
+GPU and CPU support are provided by [CTranslate2](https://github.com/OpenNMT/CTranslate2/).
+
+It has compatibility with x86-64 and AArch64/ARM64 CPU and integrates multiple backends that are optimized for these platforms: Intel MKL, oneDNN, OpenBLAS, Ruy, and Apple Accelerate.
+
+GPU execution requires the NVIDIA libraries cuBLAS 11.x and cuDNN 8.x to be installed on the system. Please refer to the [CTranslate2 documentation](https://opennmt.net/CTranslate2/installation.html)
+
+By default the best hardware available is selected for inference. You can use the options `--device` and `--device_index` to control manually the selection.
     
 # Usage
 
-Same command line that OpenAI whisper.
+Same command line that OpenAI Whisper.
 
 To transcribe:
 
     whisper-ctranslate2 inaguracio2011.mp3 --model medium
     
 <img alt="image" src="https://user-images.githubusercontent.com/309265/226923541-8326c575-7f43-4bba-8235-2a4a8bdfb161.png">
 
@@ -60,50 +70,60 @@
 
     whisper-ctranslate2 --help
 
 All the supported options with their help are shown.
 
 # CTranslate2 specific options
 
-On top of the OpenAI Whisper command line options, there are some specific options provided by CTranslate2 .
+On top of the OpenAI Whisper command line options, there are some specific options provided by CTranslate2 or whiper-ctranslate2.
 
-    --compute_type {default,auto,int8,int8_float16,int16,float16,float32}
+## Quantization
 
-Type of [quantization](https://opennmt.net/CTranslate2/quantization.html) to use. On CPU _int8_ will give the best performance.
+`--compute_type` option which accepts _default,auto,int8,int8_float16,int16,float16,float32_ values indicates the type of [quantization](https://opennmt.net/CTranslate2/quantization.html) to use. On CPU _int8_ will give the best performance:
 
-    --model_directory MODEL_DIRECTORY
+    whisper-ctranslate2 myfile.mp3 --compute_type int8
 
-Directory where to find a CTranslate Whisper model, for example a fine-tunned Whisper model. The model should be in CTranslate2 format.
+## Loading the model from a directory
 
-    --device_index [DEVICE_INDEX ...]
+`--model_directory` option allows to specify the directory from which you want to load a CTranslate2 Whisper model. For example, if you want to load your own quantified [Whisper model](https://opennmt.net/CTranslate2/conversion.html) version or using your own [Whisper fine-tunned](https://github.com/huggingface/community-events/tree/main/whisper-fine-tuning-event) version. The model must be in CTranslate2 format.
 
-Device IDs where to place this model on
+## Using Voice Activity Detection (VAD) filter
 
-    --vad_filter VAD_FILTER
+`--vad_filter` option enables the voice activity detection (VAD) to filter out parts of the audio without speech. This step uses the [Silero VAD model](https://github.com/snakers4/silero-vad):
 
-Enable the voice activity detection (VAD) to filter out parts of the audio without speech. This step is using the Silero VAD model https://github.com/snakers4/silero-vad.
+    whisper-ctranslate2 myfile.mp3 --vad_filter True
 
-    --vad_min_silence_duration_ms VAD_MIN_SILENCE_DURATION_MS
+The VAD filter accepts multiple additional options to determine the filter behavior:
 
-When `vad_filter` is enabled, audio segments without speech for at least this number of milliseconds will be ignored.
+    --vad_threshold VALUE (float)
 
+Probabilities above this value are considered as speech.
 
-# Whisper-ctranslate2 specific options
+    --vad_min_speech_duration_ms (int)
 
-On top of the OpenAI Whisper and CTranslate2, whisper-ctranslate2 provides some additional specific options:
+Final speech chunks shorter min_speech_duration_ms are thrown out.
 
-    --print-colors PRINT_COLORS
+    --vad_max_speech_duration_s VALUE (int)
 
-Adding the `--print_colors True` argument will print the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
+Maximum duration of speech chunks in seconds. Longer will be split at the timestamp of the last silence.
+
+
+## Print colors
+
+`--print_colors True` options prints the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
+
+    whisper-ctranslate2 myfile.mp3 --print_colors True
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
-    --live_transcribe
+## Live transcribe from your microphone
+
+`----live_transcribe True` option activates the live transcription mode from your microphone:
 
-Adding the `----live_transcribe True` will activate the live transcription mode from your microphone.
+    whisper-ctranslate2 myfile.mp3 --print_colors True
 
 https://user-images.githubusercontent.com/309265/231533784-e58c4b92-e9fb-4256-b4cd-12f1864131d9.mov
 
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
```

### Comparing `whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.1.9/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

