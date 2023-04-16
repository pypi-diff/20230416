# Comparing `tmp/tts_arranger-0.1.3.tar.gz` & `tmp/tts_arranger-0.1.4.tar.gz`

## Comparing `tts_arranger-0.1.3.tar` & `tts_arranger-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    25903 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    15112 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/LICENSE
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    25903 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tts_arranger-0.1.4/PKG-INFO
```

### Comparing `tts_arranger-0.1.3/src/tts_arranger/tts_processor.py` & `tts_arranger-0.1.4/src/tts_arranger/tts_processor.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.1.4/src/tts_arranger/tts_processor_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.1.4/src/tts_arranger/tts_simple_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import datetime
 import os
 import sys
 import time
+from typing import Optional
 
 from pydub import AudioSegment  # type: ignore
 
 from .items.tts_item import TTS_Item
 from .tts_processor import TTS_Processor
 from .utils.log import LOG_TYPE, bcolors, log
 
 
 class TTS_Simple_Writer():
     """
     Simple writer class that takes a list of TTS items (in contrast to a more complex TTS_Project object), synthesizes, and writes them as a final audio file
     """
 
-    def __init__(self, tts_items: list[TTS_Item]):
+    def __init__(self, tts_items: list[TTS_Item], preferred_speakers: Optional[list[str]] = None):
         self.tts_items = tts_items
 
         self.final_segment: AudioSegment
+        self.preferred_speakers = preferred_speakers or []
 
     def synthesize_and_write(self, output_filename: str):
         """
         Synthesize and write list of items as an audio file
 
         :param tts_items: List of TTS items to be synthesized
         :type tts_items: list
@@ -47,15 +49,16 @@
         for tts_item in tts_items:
             characters_sum += len(tts_item.text)
 
         segments = AudioSegment.empty()
 
         for idx, tts_item in enumerate(tts_items):
             if tts_item.text:
-                log(LOG_TYPE.INFO, f'Synthesizing item {idx + 1} of {len(tts_items)} "({tts_item.speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
+                speaker = tts_item.speaker or self.preferred_speakers[tts_item.speaker_idx]
+                log(LOG_TYPE.INFO, f'Synthesizing item {idx + 1} of {len(tts_items)} "({speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
             else:
                 log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC} {tts_item.text}')
 
             if time_needed:
                 log(LOG_TYPE.INFO, f'(Remaining time: {str(datetime.timedelta(seconds=round(time_needed)))})')
 
             time_last = time.time()
```

### Comparing `tts_arranger-0.1.3/src/tts_arranger/tts_writer.py` & `tts_arranger-0.1.4/src/tts_arranger/tts_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import base64
 import io
 import math
 import os
 import subprocess
 import sys
 import tempfile
-from typing import Callable
+from typing import Callable, Optional
 
 import ffmpeg  # type: ignore
 from pathvalidate._filename import sanitize_filename
 from PIL import Image
 from pydub import AudioSegment  # type: ignore
 
 from .items.tts_chapter import TTS_Chapter  # type: ignore
@@ -20,15 +20,15 @@
 
 
 class TTS_Writer():
     """
     Class to process TTS projects (containing of chapters each containing a number of items) and to finally write an audio file including chapter metadata and chapter info
     """
 
-    def __init__(self, project: TTS_Project = TTS_Project(),  base_path: str = '', output_format='m4b', model: str = '', vocoder: str = '') -> None:
+    def __init__(self, project: TTS_Project = TTS_Project(),  base_path: str = '', output_format='m4b', model: str = '', vocoder: str = '', preferred_speakers: Optional[list[str]] = None) -> None:
         """
         Constructor for the TTS_Writer class.
 
         :param project: An instance of the TTS_Project class containing the project information.
         :type project: TTS_Project
 
         :param base_path: The path to the project directory.
@@ -49,14 +49,15 @@
         self.project = project
         self.project_path = base_path
         self.output_format = output_format
         self.model = model
         self.vocoder = vocoder
 
         self.temp_files: list[tuple[str, str]] = []
+        self.preferred_speakers = preferred_speakers or []
 
     def _get_nanoseconds_for_file(self, file_name):
         """
         Get the duration of an audio file in nanoseconds.
 
         :param file_name: The file name (including the path) of the audio file to get the duration of.
         :type file_name: str
@@ -106,38 +107,41 @@
         for i, chapter in enumerate(chapters):
             audio = AudioSegment.empty()
 
             temp_format = 'wav'
 
             filename = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
 
-            log(LOG_TYPE.INFO, f'Synthesizing chapter {i + 1} of {len(chapters)}')
+            if len(chapters) > 1:
+                log(LOG_TYPE.INFO, f'Synthesizing chapter {i + 1} of {len(chapters)}')
 
-            for j, tts_item in enumerate(chapter.tts_items):
-                if tts_item.text:
-                    log(LOG_TYPE.INFO, f'Synthesizing item {j + 1} of {len(chapter.tts_items)} ("{tts_item.speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
-                else:
-                    log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC} {tts_item.text}')
+            if len(chapter.tts_items) > 0:
+                for j, tts_item in enumerate(chapter.tts_items):
+                    if tts_item.text:
+                        speaker = tts_item.speaker or self.preferred_speakers[tts_item.speaker_idx]
+                        log(LOG_TYPE.INFO, f'Synthesizing item {j + 1} of {len(chapter.tts_items)} ("{speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
+                    else:
+                        log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC} {tts_item.text}')
 
-                audio += tts_processor.synthesize_tts_item(tts_item)
+                    audio += tts_processor.synthesize_tts_item(tts_item)
 
-                if callback is not None:
-                    callback(100/(len(chapters) * len(chapter.tts_items)) * (i + j), tts_item)
+                    if callback is not None:
+                        callback(100/(len(chapters) * len(chapter.tts_items)) * (i + j), tts_item)
 
-            current_total_items += len(chapter.tts_items)
+                current_total_items += len(chapter.tts_items)
 
-            self._write_temp_audio(audio, filename)
+                self._write_temp_audio(audio, filename)
 
-            num_zeros = len(str(len(self.temp_files)))
-            chapter_title = f'{i + 1:0{num_zeros}} - {chapter.title}'
+                num_zeros = len(str(len(self.temp_files)))
+                chapter_title = f'{i + 1:0{num_zeros}} - {chapter.title}'
 
-            filename_out = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
+                filename_out = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
 
-            # Add temp files for concatenating later
-            self.temp_files.append((chapter_title, filename_out))
+                # Add temp files for concatenating later
+                self.temp_files.append((chapter_title, filename_out))
 
             chapter.start_time = cumulative_time
             chapter.end_time = cumulative_time + self._get_nanoseconds_for_file(filename)
             cumulative_time = chapter.end_time
 
         del tts_processor
 
@@ -252,27 +256,27 @@
             return
 
         with tempfile.TemporaryDirectory(prefix=temp_dir_prefix) as temp_dir:
             try:
                 log(LOG_TYPE.INFO, f'Synthesizing {self.project.title}')
 
                 if self.model and self.vocoder:
-                    t = TTS_Processor(self.model, self.vocoder)
+                    t = TTS_Processor(self.model, self.vocoder, self.preferred_speakers)
                 else:
                     match self.project.lang_code:
                         case 'en':
                             self.model = 'tts_models/en/vctk/vits'
                             self.vocoder = ''
                         case 'de':
                             self.model = 'tts_models/de/thorsten/tacotron2-DDC'
                             self.vocoder = 'vocoder_models/de/thorsten/hifigan_v1'
                         case _:
                             raise ValueError(f'Language code {self.project.lang_code} not supported')
 
-                    t = TTS_Processor(self.model, self.vocoder)
+                    t = TTS_Processor(self.model, self.vocoder, self.preferred_speakers)
 
                 self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback)
 
             except Exception as e:
                 log(LOG_TYPE.ERROR, f'Synthesizing {self.project.title} failed: {e}')
                 sys.exit(1)
 
@@ -330,15 +334,15 @@
                     os.makedirs(output_filename, exist_ok=True)
 
                     for name, file in self.temp_files:
                         output_chapter_filename = os.path.join(output_filename, name + output_extension)
 
                         output_args = {'metadata': f'title={self.project.title} - {name}', 'metadata:': f'album={self.project.subtitle}', 'metadata:g': f'artist={self.project.author}'}
 
-                        if self.output_format is 'mp3':
+                        if self.output_format == 'mp3':
                             output_args['audio_bitrate'] = '320k'
 
                         # Convert to target format, adding metadata
                         (
                             ffmpeg
                             .input(file)
                             .output(output_chapter_filename, **output_args, loglevel='error')
```

### Comparing `tts_arranger-0.1.3/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.1.4/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.1.4/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.1.4/src/tts_arranger/items/tts_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,9 +153,19 @@
         Opens the image from the given URL and adds it via the private function.
 
         :param image_url: The URL of the image to be added.
         :type image_url: str
 
         :return: None
         """
-        image = Image.open(requests.get(image_url, stream=True).raw)
-        self._add_image(image)
+        if image_url:
+            image = Image.open(requests.get(image_url, stream=True).raw)
+            self._add_image(image)
+
+    def clean_empty_chapters(self):
+        final_chapters: list[TTS_Chapter] = []
+
+        for chapter in self.tts_chapters:
+            if len(chapter.tts_items) > 0:
+                final_chapters.append(chapter)
+
+        self.tts_chapters = final_chapters
```

### Comparing `tts_arranger-0.1.3/src/tts_arranger/utils/audio.py` & `tts_arranger-0.1.4/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/src/tts_arranger/utils/log.py` & `tts_arranger-0.1.4/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/tests/tts_arranger_test.py` & `tts_arranger-0.1.4/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/LICENSE` & `tts_arranger-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/README.md` & `tts_arranger-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.3/pyproject.toml` & `tts_arranger-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.1.3"
+version = "0.1.4"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.1.3/PKG-INFO` & `tts_arranger-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

