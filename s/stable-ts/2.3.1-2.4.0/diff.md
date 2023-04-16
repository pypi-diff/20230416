# Comparing `tmp/stable-ts-2.3.1.tar.gz` & `tmp/stable-ts-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.3.1.tar", last modified: Sat Apr  8 18:09:49 2023, max compression
+gzip compressed data, was "stable-ts-2.4.0.tar", last modified: Sun Apr 16 00:44:47 2023, max compression
```

## Comparing `stable-ts-2.3.1.tar` & `stable-ts-2.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 18:09:49.120530 stable-ts-2.3.1/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.3.1/LICENSE
--rw-rw-rw-   0        0        0     6890 2023-04-08 18:09:49.119530 stable-ts-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 18:09:49.120530 stable-ts-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 18:09:49.068530 stable-ts-2.3.1/stable_ts.egg-info/
--rw-rw-rw-   0        0        0     6890 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 18:09:49.117530 stable-ts-2.3.1/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.3.1/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.3.1/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-08 18:02:41.000000 stable-ts-2.3.1/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     4009 2023-03-25 19:51:29.000000 stable-ts-2.3.1/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4328 2023-03-22 02:57:30.000000 stable-ts-2.3.1/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.3.1/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    27797 2023-04-08 17:41:20.000000 stable-ts-2.3.1/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.3.1/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    12598 2023-04-05 01:42:52.000000 stable-ts-2.3.1/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0     9744 2023-04-08 16:34:45.000000 stable-ts-2.3.1/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.3.1/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    48446 2023-04-08 16:34:45.000000 stable-ts-2.3.1/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-04-16 00:44:47.079108 stable-ts-2.4.0/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0     6890 2023-04-16 00:44:47.078110 stable-ts-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 00:44:47.079108 stable-ts-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 00:44:47.026117 stable-ts-2.4.0/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0     6890 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 00:44:47.076108 stable-ts-2.4.0/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.4.0/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.4.0/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-04-16 00:28:38.000000 stable-ts-2.4.0/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     6525 2023-04-16 00:09:42.000000 stable-ts-2.4.0/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4328 2023-03-22 02:57:30.000000 stable-ts-2.4.0/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.4.0/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    28381 2023-04-15 17:10:33.000000 stable-ts-2.4.0/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.4.0/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    12598 2023-04-05 01:42:52.000000 stable-ts-2.4.0/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0     9744 2023-04-08 16:34:45.000000 stable-ts-2.4.0/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.4.0/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    48728 2023-04-16 00:31:11.000000 stable-ts-2.4.0/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.3.1/LICENSE` & `stable-ts-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/PKG-INFO` & `stable-ts-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.3.1
+Version: 2.4.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.3.1/README.md` & `stable-ts-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/setup.py` & `stable-ts-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.4.0/stable_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.3.1
+Version: 2.4.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.3.1/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.4.0/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/stable_whisper/decode.py` & `stable-ts-2.4.0/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/stable_whisper/quantization.py` & `stable-ts-2.4.0/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/stable_whisper/result.py` & `stable-ts-2.4.0/stable_whisper/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 
         return self_copy
 
     @property
     def duration(self):
         return self.end - self.start
 
+    def offset_time(self, offset_seconds: float):
+        self.start = self.start + offset_seconds
+        self.end = self.end + offset_seconds
+
     def to_dict(self):
         dict_ = deepcopy(self.__dict__)
         dict_.pop('left_locked')
         dict_.pop('right_locked')
         return dict_
 
     def lock_left(self):
@@ -130,14 +134,22 @@
         self_copy.temperature = (other.temperature + self_copy.temperature) / 2
         self_copy.avg_logprob = (other.avg_logprob + self_copy.avg_logprob) / 2
         self_copy.compression_ratio = (other.compression_ratio + self_copy.compression_ratio) / 2
         self_copy.no_speech_prob = (other.no_speech_prob + self_copy.no_speech_prob) / 2
 
         return self_copy
 
+    def offset_time(self, offset_seconds: float):
+        self.seek = self.seek + offset_seconds
+        self.start = self.start + offset_seconds
+        self.end = self.end + offset_seconds
+        if self.has_words:
+            for w in self.words:
+                w.offset_time(offset_seconds)
+
     def add_words(self, index0: int, index1: int, inplace: bool = False):
         new_word = self.words[index0] + self.words[index1]
         if inplace:
             i0, i1 = sorted([index0, index1])
             self.words[i0] = new_word
             del self.words[i1]
         return new_word
@@ -435,14 +447,18 @@
                         result.add_segments(i, i+1, inplace=True)
                 max_i -= 1
         result.reassign_ids()
         for s in result.segments:
             s.apply_min_dur(min_dur, inplace=True)
         return result
 
+    def offset_time(self, offset_seconds: float):
+        for s in self.segments:
+            s.offset_time(offset_seconds)
+
     def suppress_silence(
             self,
             silent_starts: np.ndarray,
             silent_ends: np.ndarray,
             min_word_dur: float = 0.1,
             word_level: bool = True
     ):
```

### Comparing `stable-ts-2.3.1/stable_whisper/stabilization.py` & `stable-ts-2.4.0/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/stable_whisper/text_output.py` & `stable-ts-2.4.0/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/stable_whisper/timing.py` & `stable-ts-2.4.0/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/stable_whisper/video_output.py` & `stable-ts-2.4.0/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.1/stable_whisper/whisper_word_level.py` & `stable-ts-2.4.0/stable_whisper/whisper_word_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     SAMPLE_RATE, N_FRAMES, HOP_LENGTH, N_SAMPLES, N_SAMPLES_PER_TOKEN, TOKENS_PER_SECOND, FRAMES_PER_SECOND, N_FFT,
     pad_or_trim, log_mel_spectrogram
 )
 from whisper.utils import exact_div, format_timestamp, make_safe
 from whisper.tokenizer import get_tokenizer, LANGUAGES, TO_LANGUAGE_CODE
 from whisper.decoding import DecodingOptions, DecodingResult
 
+from .audio import load_audio
 from .decode import decode_stable
 from .result import WhisperResult, Segment
 from .timing import add_word_timestamps_stable
 from .stabilization import get_vad_silence_func, wav2mask, mask2timing, timing2mask
 
 if TYPE_CHECKING:
     from whisper.model import Whisper
@@ -28,15 +29,15 @@
 
 warnings.filterwarnings('ignore', module='whisper', message='.*Triton.*', category=UserWarning)
 
 
 # modified version of whisper.transcribe.transcribe
 def transcribe_stable(
         model: "Whisper",
-        audio: Union[str, np.ndarray, torch.Tensor],
+        audio: Union[str, np.ndarray, torch.Tensor, bytes],
         *,
         verbose: Optional[bool] = False,
         temperature: Union[float, Tuple[float, ...]] = (0.0, 0.2, 0.4, 0.6, 0.8, 1.0),
         compression_ratio_threshold: Optional[float] = 2.4,
         logprob_threshold: Optional[float] = -1.0,
         no_speech_threshold: Optional[float] = 0.6,
         condition_on_previous_text: bool = True,
@@ -67,16 +68,16 @@
     Transcribe an audio file using Whisper
 
     Parameters
     ----------
     model: Whisper
         The Whisper model modified instance
 
-    audio: Union[str, np.ndarray, torch.Tensor]
-        The path to the audio file to open, or the audio waveform
+    audio: Union[str, np.ndarray, torch.Tensor, bytes]
+        The path/URL to the audio file, the audio waveform, or bytes of audio file.
 
     verbose: bool
         Whether to display the text being decoded to the console. If True, displays all the details,
         If False, displays progressbar. If None, does not display anything (Default: False)
 
     temperature: Union[float, Tuple[float, ...]]
         Temperature for sampling. It can be a tuple of temperatures, which will be successfully used
@@ -204,56 +205,60 @@
 
     device = model.device
 
     if time_scale == 1:
         time_scale = None
 
     curr_sr = SAMPLE_RATE if time_scale is None else SAMPLE_RATE * time_scale
-    if isinstance(audio, str):
+    if isinstance(audio, (str, bytes)):
         if demucs:
             from .audio import demucs_audio
             audio = demucs_audio(audio,
                                  output_sr=curr_sr,
                                  device=device,
-                                 verbose=verbose is not None,
+                                 verbose=verbose,
                                  save_path=demucs_output)
         else:
-            audio = torch.from_numpy(whisper.load_audio(audio, sr=curr_sr))
+            audio = torch.from_numpy(load_audio(audio, sr=curr_sr, verbose=verbose))
     else:
         if isinstance(audio, np.ndarray):
             audio = torch.from_numpy(audio)
         input_sr = decode_options.pop('input_sr', SAMPLE_RATE)
         if demucs:
             from .audio import demucs_audio
             audio = demucs_audio(audio,
                                  input_sr=input_sr,
                                  output_sr=curr_sr,
                                  device=device,
-                                 verbose=verbose is not None,
+                                 verbose=verbose,
                                  save_path=demucs_output)
         elif input_sr != curr_sr:
             from torchaudio.functional import resample
             if isinstance(audio, np.ndarray):
                 audio = torch.from_numpy(audio)
             audio = resample(audio, input_sr, curr_sr, resampling_method="kaiser_window")
     if only_voice_freq:
         from .audio import voice_freq_filter
         audio = voice_freq_filter(audio, curr_sr)
     sample_padding = int(N_FFT // 2) + 1
     whole_mel = log_mel_spectrogram(audio, padding=sample_padding) if mel_first else None
 
-    if decode_options.get("language", None) is None:
-        if verbose:
-            print("Detecting language using up to the first 30 seconds. Use `--language` to specify the language")
-        mel_segment = log_mel_spectrogram(audio[..., :N_SAMPLES], padding=sample_padding) \
-            if whole_mel is None else whole_mel[..., :N_FRAMES]
-        mel_segment = pad_or_trim(mel_segment, N_FRAMES).to(device=model.device, dtype=dtype)
-        _, probs = model.detect_language(mel_segment)
-        decode_options["language"] = max(probs, key=probs.get)
-        print(f"Detected language: {LANGUAGES[decode_options['language']]}")
+    if decode_options.get("language", None) is None and model:
+        if not model.is_multilingual:
+            decode_options["language"] = "en"
+        else:
+            if verbose:
+                print("Detecting language using up to the first 30 seconds. Use `--language` to specify the language")
+            mel_segment = log_mel_spectrogram(audio[..., :N_SAMPLES], padding=sample_padding) \
+                if whole_mel is None else whole_mel[..., :N_FRAMES]
+            mel_segment = pad_or_trim(mel_segment, N_FRAMES).to(device=model.device, dtype=dtype)
+            _, probs = model.detect_language(mel_segment)
+            decode_options["language"] = max(probs, key=probs.get)
+            if verbose is not None:
+                print(f"Detected language: {LANGUAGES[decode_options['language']]}")
 
     language = decode_options["language"]
     task = decode_options.get("task", "transcribe")
     tokenizer = get_tokenizer(model.is_multilingual, language=language, task=task)
 
     if word_timestamps and task == "translate":
         warnings.warn("Word-level timestamps on translations may not be reliable.")
@@ -632,15 +637,16 @@
             return str2val[string]
         raise ValueError(f"Expected one of {set(str2val.keys())}, got {string}")
 
     output_formats = {"srt", "ass", "json", "vtt"}
 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("inputs", nargs="+", type=str,
-                        help="audio/video file(s) to transcribe or json file(s) to process into [output_format]")
+                        help="audio/video filepath/URL(s) to transcribe "
+                             "or json file(s) to process into [output_format]")
     parser.add_argument("--output", "-o", nargs="+", type=str,
                         help="output filepaths(s);"
                              "if not specified, auto-named output file(s) will be saved to "
                              "[output_dir] or current dir if not specified.")
     parser.add_argument("--model", '-m', default="base", choices=available_models(),
                         help="name of the Whisper model to use")
     parser.add_argument("--model_dir", type=str, default=None,
```

