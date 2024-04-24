# Comparing `tmp/transcribe-anything-2.7.8.tar.gz` & `tmp/transcribe-anything-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe-anything-2.7.8.tar", last modified: Sat Jan 13 02:32:34 2024, max compression
+gzip compressed data, was "transcribe-anything-2.7.9.tar", last modified: Sat Jan 13 04:35:45 2024, max compression
```

## Comparing `transcribe-anything-2.7.8.tar` & `transcribe-anything-2.7.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-01-13 02:32:34.885955 transcribe-anything-2.7.8/
--rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.7.8/LICENSE
--rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.7.8/MANIFEST.in
--rw-rw-rw-   0        0        0    10535 2024-01-13 02:32:34.884611 transcribe-anything-2.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     9295 2024-01-13 02:32:13.000000 transcribe-anything-2.7.8/README.md
--rw-rw-rw-   0        0        0       29 2023-10-20 00:08:26.000000 transcribe-anything-2.7.8/requirements.testing.txt
--rw-rw-rw-   0        0        0      102 2024-01-12 23:33:31.000000 transcribe-anything-2.7.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-01-13 02:32:34.885955 transcribe-anything-2.7.8/setup.cfg
--rw-rw-rw-   0        0        0     3110 2024-01-13 02:31:47.000000 transcribe-anything-2.7.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-13 02:32:34.858238 transcribe-anything-2.7.8/tests/
--rw-rw-rw-   0        0        0     1358 2023-10-20 00:10:38.000000 transcribe-anything-2.7.8/tests/test_embed_transcript.py
--rw-rw-rw-   0        0        0     1088 2024-01-12 03:36:35.000000 transcribe-anything-2.7.8/tests/test_insane_whisper_cmd_arg.py
--rw-rw-rw-   0        0        0     1482 2024-01-12 03:04:58.000000 transcribe-anything-2.7.8/tests/test_insanely_fast_whisper.py
--rw-rw-rw-   0        0        0     2271 2024-01-13 02:31:01.000000 transcribe-anything-2.7.8/tests/test_insanely_fast_whisper_json_to_srt_txt.py
--rw-rw-rw-   0        0        0      960 2024-01-12 04:20:30.000000 transcribe-anything-2.7.8/tests/test_local_file_cmd.py
--rw-rw-rw-   0        0        0     2833 2023-10-20 00:10:49.000000 transcribe-anything-2.7.8/tests/test_transcribe_anything.py
--rw-rw-rw-   0        0        0     2130 2024-01-12 02:47:37.000000 transcribe-anything-2.7.8/tests/test_transcribe_anything_api.py
--rw-rw-rw-   0        0        0      739 2024-01-12 04:05:48.000000 transcribe-anything-2.7.8/tests/test_whisper.py
-drwxrwxrwx   0        0        0        0 2024-01-13 02:32:34.872946 transcribe-anything-2.7.8/transcribe_anything/
--rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.7.8/transcribe_anything/__init__.py
--rw-rw-rw-   0        0        0     9300 2024-01-13 00:25:25.000000 transcribe-anything-2.7.8/transcribe_anything/api.py
--rw-rw-rw-   0        0        0     3123 2024-01-13 00:20:34.000000 transcribe-anything-2.7.8/transcribe_anything/audio.py
--rw-rw-rw-   0        0        0     3502 2024-01-13 01:58:18.000000 transcribe-anything-2.7.8/transcribe_anything/cmd.py
--rw-rw-rw-   0        0        0     3351 2024-01-12 05:45:19.000000 transcribe-anything-2.7.8/transcribe_anything/cuda_available.py
--rw-rw-rw-   0        0        0     6716 2024-01-13 02:31:32.000000 transcribe-anything-2.7.8/transcribe_anything/insanely_fast_whisper.py
--rw-rw-rw-   0        0        0     1071 2024-01-11 05:22:31.000000 transcribe-anything-2.7.8/transcribe_anything/install_whisper.py
--rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.7.8/transcribe_anything/logger.py
--rw-rw-rw-   0        0        0     1343 2024-01-11 05:42:49.000000 transcribe-anything-2.7.8/transcribe_anything/parse_whisper_options.py
--rw-rw-rw-   0        0        0     1298 2024-01-11 05:12:03.000000 transcribe-anything-2.7.8/transcribe_anything/util.py
--rw-rw-rw-   0        0        0     3278 2024-01-12 04:13:18.000000 transcribe-anything-2.7.8/transcribe_anything/whisper.py
--rw-rw-rw-   0        0        0      935 2023-07-11 21:54:33.000000 transcribe-anything-2.7.8/transcribe_anything/ytldp_download.py
-drwxrwxrwx   0        0        0        0 2024-01-13 02:32:34.883609 transcribe-anything-2.7.8/transcribe_anything.egg-info/
--rw-rw-rw-   0        0        0    10535 2024-01-13 02:32:34.000000 transcribe-anything-2.7.8/transcribe_anything.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1028 2024-01-13 02:32:34.000000 transcribe-anything-2.7.8/transcribe_anything.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-13 02:32:34.000000 transcribe-anything-2.7.8/transcribe_anything.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-01-13 02:32:34.000000 transcribe-anything-2.7.8/transcribe_anything.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2024-01-13 02:32:34.000000 transcribe-anything-2.7.8/transcribe_anything.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-01-13 02:32:34.000000 transcribe-anything-2.7.8/transcribe_anything.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-13 04:35:45.733976 transcribe-anything-2.7.9/
+-rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.7.9/LICENSE
+-rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.7.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    10641 2024-01-13 04:35:45.732975 transcribe-anything-2.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9378 2024-01-13 04:35:30.000000 transcribe-anything-2.7.9/README.md
+-rw-rw-rw-   0        0        0       29 2023-10-20 00:08:26.000000 transcribe-anything-2.7.9/requirements.testing.txt
+-rw-rw-rw-   0        0        0      108 2024-01-13 02:59:31.000000 transcribe-anything-2.7.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-01-13 04:35:45.733976 transcribe-anything-2.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     3110 2024-01-13 04:35:05.000000 transcribe-anything-2.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-13 04:35:45.707091 transcribe-anything-2.7.9/tests/
+-rw-rw-rw-   0        0        0     1358 2023-10-20 00:10:38.000000 transcribe-anything-2.7.9/tests/test_embed_transcript.py
+-rw-rw-rw-   0        0        0     1088 2024-01-12 03:36:35.000000 transcribe-anything-2.7.9/tests/test_insane_whisper_cmd_arg.py
+-rw-rw-rw-   0        0        0     1482 2024-01-12 03:04:58.000000 transcribe-anything-2.7.9/tests/test_insanely_fast_whisper.py
+-rw-rw-rw-   0        0        0     2281 2024-01-13 03:47:30.000000 transcribe-anything-2.7.9/tests/test_insanely_fast_whisper_json_to_srt_txt.py
+-rw-rw-rw-   0        0        0      960 2024-01-12 04:20:30.000000 transcribe-anything-2.7.9/tests/test_local_file_cmd.py
+-rw-rw-rw-   0        0        0     2833 2023-10-20 00:10:49.000000 transcribe-anything-2.7.9/tests/test_transcribe_anything.py
+-rw-rw-rw-   0        0        0     2130 2024-01-12 02:47:37.000000 transcribe-anything-2.7.9/tests/test_transcribe_anything_api.py
+-rw-rw-rw-   0        0        0      739 2024-01-12 04:05:48.000000 transcribe-anything-2.7.9/tests/test_whisper.py
+drwxrwxrwx   0        0        0        0 2024-01-13 04:35:45.722082 transcribe-anything-2.7.9/transcribe_anything/
+-rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.7.9/transcribe_anything/__init__.py
+-rw-rw-rw-   0        0        0     9300 2024-01-13 00:25:25.000000 transcribe-anything-2.7.9/transcribe_anything/api.py
+-rw-rw-rw-   0        0        0     3123 2024-01-13 00:20:34.000000 transcribe-anything-2.7.9/transcribe_anything/audio.py
+-rw-rw-rw-   0        0        0     3502 2024-01-13 01:58:18.000000 transcribe-anything-2.7.9/transcribe_anything/cmd.py
+-rw-rw-rw-   0        0        0     3351 2024-01-12 05:45:19.000000 transcribe-anything-2.7.9/transcribe_anything/cuda_available.py
+-rw-rw-rw-   0        0        0     7562 2024-01-13 04:26:44.000000 transcribe-anything-2.7.9/transcribe_anything/insanely_fast_whisper.py
+-rw-rw-rw-   0        0        0     1071 2024-01-11 05:22:31.000000 transcribe-anything-2.7.9/transcribe_anything/install_whisper.py
+-rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.7.9/transcribe_anything/logger.py
+-rw-rw-rw-   0        0        0     1343 2024-01-11 05:42:49.000000 transcribe-anything-2.7.9/transcribe_anything/parse_whisper_options.py
+-rw-rw-rw-   0        0        0     1298 2024-01-11 05:12:03.000000 transcribe-anything-2.7.9/transcribe_anything/util.py
+-rw-rw-rw-   0        0        0     3278 2024-01-12 04:13:18.000000 transcribe-anything-2.7.9/transcribe_anything/whisper.py
+-rw-rw-rw-   0        0        0      935 2023-07-11 21:54:33.000000 transcribe-anything-2.7.9/transcribe_anything/ytldp_download.py
+drwxrwxrwx   0        0        0        0 2024-01-13 04:35:45.731976 transcribe-anything-2.7.9/transcribe_anything.egg-info/
+-rw-rw-rw-   0        0        0    10641 2024-01-13 04:35:45.000000 transcribe-anything-2.7.9/transcribe_anything.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1028 2024-01-13 04:35:45.000000 transcribe-anything-2.7.9/transcribe_anything.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-13 04:35:45.000000 transcribe-anything-2.7.9/transcribe_anything.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-01-13 04:35:45.000000 transcribe-anything-2.7.9/transcribe_anything.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2024-01-13 04:35:45.000000 transcribe-anything-2.7.9/transcribe_anything.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-01-13 04:35:45.000000 transcribe-anything-2.7.9/transcribe_anything.egg-info/top_level.txt
```

### Comparing `transcribe-anything-2.7.8/LICENSE` & `transcribe-anything-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/PKG-INFO` & `transcribe-anything-2.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-anything
-Version: 2.7.8
+Version: 2.7.9
 Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
 Home-page: https://github.com/zackees/transcribe-anything
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: static-ffmpeg>=2.5
 Requires-Dist: yt-dlp>=2023.3.4
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: disklru>=1.0.7
 Requires-Dist: isolated-environment>=1.0.1
+Requires-Dist: json5
 Requires-Dist: FileLock
 
 # transcribe-anything
 [![MacOS_Tests](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
 [![Win_Tests](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
 [![Ubuntu_Tests](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
 [![Lint](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
@@ -164,14 +165,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.7.9: All SRT translation errors fixed for `--device insane`. All tests pass.
   * 2.7.8: During error of `--device insane`, write out the error.json file into the destination.
   * 2.7.7: Better error messages during failure.
   * 2.7.6: Improved generation of out.txt, removes linebreaks.
   * 2.7.5: `--device insane` now generates better conforming srt files.
   * 2.7.3: Various fixes for the `insane` mode backend.
   * 2.7.0: Introduces an `insanely-fast-whisper`, enable by using `--device insane`
   * 2.6.0: GPU acceleration now happens automatically on Windows thanks to `isolated-environment`. This will also prevent
```

### Comparing `transcribe-anything-2.7.8/README.md` & `transcribe-anything-2.7.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.7.9: All SRT translation errors fixed for `--device insane`. All tests pass.
   * 2.7.8: During error of `--device insane`, write out the error.json file into the destination.
   * 2.7.7: Better error messages during failure.
   * 2.7.6: Improved generation of out.txt, removes linebreaks.
   * 2.7.5: `--device insane` now generates better conforming srt files.
   * 2.7.3: Various fixes for the `insane` mode backend.
   * 2.7.0: Introduces an `insanely-fast-whisper`, enable by using `--device insane`
   * 2.6.0: GPU acceleration now happens automatically on Windows thanks to `isolated-environment`. This will also prevent
```

### Comparing `transcribe-anything-2.7.8/setup.py` & `transcribe-anything-2.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Uses whisper AI to transcribe speach from video and audio files. "
     "Also accepts urls for youtube, rumble, bitchute, clear file, etc."
 )
 URL = "https://github.com/zackees/transcribe-anything"
 EMAIL = "dont@email.me"
 AUTHOR = "Zach Vorhies"
 REQUIRES_PYTHON = ">=3.10.0"
-VERSION = "2.7.8"
+VERSION = "2.7.9"
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), encoding="utf-8", mode="r") as fd:
     README = fd.read()
 
 
 def parse_requirements(filename):
```

### Comparing `transcribe-anything-2.7.8/tests/test_embed_transcript.py` & `transcribe-anything-2.7.9/tests/test_embed_transcript.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/tests/test_insane_whisper_cmd_arg.py` & `transcribe-anything-2.7.9/tests/test_insane_whisper_cmd_arg.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/tests/test_insanely_fast_whisper.py` & `transcribe-anything-2.7.9/tests/test_insanely_fast_whisper.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/tests/test_insanely_fast_whisper_json_to_srt_txt.py` & `transcribe-anything-2.7.9/tests/test_insanely_fast_whisper_json_to_srt_txt.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,26 +77,26 @@
 
 class JsonToSrtTester(unittest.TestCase):
     """Tester for transcribe anything."""
 
     def test_json_to_srt(self) -> None:
         """Check that the command works on a local file."""
         data = json.loads(EXAMPLE_JSON)
-        out = convert_json_to_srt(data)
+        out = convert_json_to_srt(data, 9.0)
         self.assertIn(EXPECTED_SRT_FILE, out)
 
     def test_json_to_txt(self) -> None:
         """Check that the command works on a local file."""
         data = json.loads(EXAMPLE_JSON)
         out = convert_json_to_text(data)
         self.assertIn(EXPECTED_TXT_FILE, out)
 
     def test_problem_json_to_txt(self) -> None:
         """Check that the command works on a local file."""
         json_txt = PROBLEM_JSON.read_text()
         data = json.loads(json_txt)
-        _ = convert_json_to_text(data)
+        _ = convert_json_to_srt(data, 9999)
         print("Parsed problem json:")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `transcribe-anything-2.7.8/tests/test_local_file_cmd.py` & `transcribe-anything-2.7.9/tests/test_local_file_cmd.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/tests/test_transcribe_anything.py` & `transcribe-anything-2.7.9/tests/test_transcribe_anything.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/tests/test_transcribe_anything_api.py` & `transcribe-anything-2.7.9/tests/test_transcribe_anything_api.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/tests/test_whisper.py` & `transcribe-anything-2.7.9/tests/test_whisper.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/api.py` & `transcribe-anything-2.7.9/transcribe_anything/api.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/audio.py` & `transcribe-anything-2.7.9/transcribe_anything/audio.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/cmd.py` & `transcribe-anything-2.7.9/transcribe_anything/cmd.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/cuda_available.py` & `transcribe-anything-2.7.9/transcribe_anything/cuda_available.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/insanely_fast_whisper.py` & `transcribe-anything-2.7.9/transcribe_anything/insanely_fast_whisper.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 """
 Runs whisper api.
 """
 
 import shutil
 import sys
 import time
-import json
+import wave
+import json5 as json  # type: ignore
 from pathlib import Path
 import subprocess
 from typing import Optional, Any
 from filelock import FileLock
 
 from isolated_environment import IsolatedEnvironment  # type: ignore
 from transcribe_anything.cuda_available import CudaInfo
@@ -106,19 +107,26 @@
     hours, remainder = divmod(timestamp, 3600)
     minutes, seconds = divmod(remainder, 60)
     milliseconds = int((seconds % 1) * 1000)
     seconds = int(seconds)
     return f"{int(hours):02}:{int(minutes):02}:{seconds:02},{milliseconds:03}"
 
 
-def convert_json_to_srt(json_data: dict[str, Any]) -> str:
+def convert_json_to_srt(json_data: dict[str, Any], duration: float) -> str:
     """Converts JSON data from speech-to-text tool to SRT format."""
     srt_content = ""
+    num_chunks = len(json_data["chunks"])
     for index, chunk in enumerate(json_data["chunks"], start=1):
-        start_time, end_time = chunk["timestamp"]
+        # start_time, end_time = chunk["timestamp"]
+        time_pair = chunk["timestamp"]
+        start_time = time_pair[0]
+        end_time = time_pair[1]
+        if end_time is None:
+            assert index == num_chunks
+            end_time = duration  # Sometimes happens at the end
         try:
             start_time_str = convert_time_to_srt_format(start_time)
         except Exception as exc:
             print(f"Failed to convert start time {start_time} to srt format: {exc}")
             raise
         try:
             end_time_str = convert_time_to_srt_format(end_time)
@@ -131,14 +139,23 @@
 
 
 def convert_json_to_text(json_data: dict[str, Any]) -> str:
     """Converts JSON data from speech-to-text tool to text."""
     return json_data["text"]
 
 
+def get_wave_duration(wave_file: Path) -> float:
+    """Returns the duration of a wave file."""
+    with wave.open(str(wave_file), "rb") as wav:
+        frames = wav.getnframes()
+        rate = wav.getframerate()
+        duration = frames / float(rate)
+        return duration
+
+
 def run_insanely_fast_whisper(  # pylint: disable=too-many-arguments
     input_wav: Path,
     model: str,
     output_dir: Path,
     task: str,
     language: str,
     other_args: Optional[list[str]],
@@ -146,14 +163,15 @@
     """Runs insanely fast whisper."""
     iso_env = get_environment()
     device_id = get_device_id()
     cmd_list = []
     output_dir.mkdir(parents=True, exist_ok=True)
     outfile = output_dir / "out.json"
     model = f"openai/whisper-{model}"
+    wave_duration = get_wave_duration(input_wav)
     if sys.platform == "win32":
         # Set the text mode to UTF-8 on Windows.
         cmd_list.extend(["chcp", "65001", "&&"])
     cmd_list += [
         "insanely-fast-whisper",
         "--file-name",
         str(input_wav),
@@ -188,23 +206,26 @@
         if rtn != 0:
             msg = f"Failed to execute {cmd}\n "
             raise OSError(msg)
         break
     assert outfile.exists(), f"Expected {outfile} to exist."
     json_text = outfile.read_text(encoding="utf-8")
     json_data = json.loads(json_text)
+    json_data_str = json.dumps(json_data, indent=2)
     try:
-        srt_content = convert_json_to_srt(json_data)
+        srt_content = convert_json_to_srt(json_data, wave_duration)
         srt_file = output_dir / "out.srt"
     except Exception as exc:
         print(f"Failed to convert to srt: {exc}")
-        print("Json data: ", json_data)
+        print("Json data: ", json_data_str)
+        error_file = Path("transcribe-anything-error.json")
+        error_file.write_text(json_text, encoding="utf-8")
         raise
     try:
         txt_content = convert_json_to_text(json_data)
     except Exception as exc:
-        error_file = output_dir / "transcribe-anything-error.json"
+        error_file = Path("transcribe-anything-error.json")
         error_file.write_text(json_text, encoding="utf-8")
         raise
     srt_file.write_text(srt_content, encoding="utf-8")
     txt_file = output_dir / "out.txt"
     txt_file.write_text(txt_content, encoding="utf-8")
```

### Comparing `transcribe-anything-2.7.8/transcribe_anything/install_whisper.py` & `transcribe-anything-2.7.9/transcribe_anything/install_whisper.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/logger.py` & `transcribe-anything-2.7.9/transcribe_anything/logger.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/parse_whisper_options.py` & `transcribe-anything-2.7.9/transcribe_anything/parse_whisper_options.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/util.py` & `transcribe-anything-2.7.9/transcribe_anything/util.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/whisper.py` & `transcribe-anything-2.7.9/transcribe_anything/whisper.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything/ytldp_download.py` & `transcribe-anything-2.7.9/transcribe_anything/ytldp_download.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.7.8/transcribe_anything.egg-info/PKG-INFO` & `transcribe-anything-2.7.9/transcribe_anything.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-anything
-Version: 2.7.8
+Version: 2.7.9
 Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
 Home-page: https://github.com/zackees/transcribe-anything
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: static-ffmpeg>=2.5
 Requires-Dist: yt-dlp>=2023.3.4
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: disklru>=1.0.7
 Requires-Dist: isolated-environment>=1.0.1
+Requires-Dist: json5
 Requires-Dist: FileLock
 
 # transcribe-anything
 [![MacOS_Tests](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
 [![Win_Tests](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
 [![Ubuntu_Tests](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
 [![Lint](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
@@ -164,14 +165,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.7.9: All SRT translation errors fixed for `--device insane`. All tests pass.
   * 2.7.8: During error of `--device insane`, write out the error.json file into the destination.
   * 2.7.7: Better error messages during failure.
   * 2.7.6: Improved generation of out.txt, removes linebreaks.
   * 2.7.5: `--device insane` now generates better conforming srt files.
   * 2.7.3: Various fixes for the `insane` mode backend.
   * 2.7.0: Introduces an `insanely-fast-whisper`, enable by using `--device insane`
   * 2.6.0: GPU acceleration now happens automatically on Windows thanks to `isolated-environment`. This will also prevent
```

### Comparing `transcribe-anything-2.7.8/transcribe_anything.egg-info/SOURCES.txt` & `transcribe-anything-2.7.9/transcribe_anything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

