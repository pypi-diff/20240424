# Comparing `tmp/stream-translator-gpt-2024.3.9.dev2.tar.gz` & `tmp/stream_translator_gpt-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stream-translator-gpt-2024.3.9.dev2.tar", last modified: Sat Mar  9 12:05:14 2024, max compression
+gzip compressed data, was "stream_translator_gpt-2024.4.24.tar", last modified: Wed Apr 24 15:26:35 2024, max compression
```

## Comparing `stream-translator-gpt-2024.3.9.dev2.tar` & `stream_translator_gpt-2024.4.24.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 12:05:14.553668 stream-translator-gpt-2024.3.9.dev2/
--rw-rw-rw-   0        0        0     1089 2023-03-12 08:56:05.000000 stream-translator-gpt-2024.3.9.dev2/LICENSE
--rw-rw-rw-   0        0        0     6004 2024-03-09 12:05:14.553668 stream-translator-gpt-2024.3.9.dev2/PKG-INFO
--rw-rw-rw-   0        0        0    14574 2024-03-09 11:53:16.000000 stream-translator-gpt-2024.3.9.dev2/README.md
--rw-rw-rw-   0        0        0     4520 2024-03-09 12:03:50.000000 stream-translator-gpt-2024.3.9.dev2/README_PyPI.md
--rw-rw-rw-   0        0        0     1749 2024-03-09 12:05:03.000000 stream-translator-gpt-2024.3.9.dev2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-09 12:05:14.553668 stream-translator-gpt-2024.3.9.dev2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-09 12:05:14.543701 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/
--rw-rw-rw-   0        0        0        0 2024-03-03 09:46:32.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/__init__.py
--rw-rw-rw-   0        0        0       68 2024-03-03 10:18:23.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/__main__.py
--rw-rw-rw-   0        0        0     5928 2024-03-03 10:23:01.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/audio_getter.py
--rw-rw-rw-   0        0        0     4102 2024-03-03 13:47:24.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/audio_slicer.py
--rw-rw-rw-   0        0        0     3342 2024-03-03 10:22:46.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/audio_transcriber.py
--rw-rw-rw-   0        0        0      753 2024-01-17 17:23:19.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/common.py
--rw-rw-rw-   0        0        0     1328 2024-01-22 20:14:03.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/filters.py
--rw-rw-rw-   0        0        0     8300 2024-03-05 13:52:21.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/llm_translator.py
--rw-rw-rw-   0        0        0     1960 2024-03-09 11:45:58.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/result_exporter.py
--rw-rw-rw-   0        0        0  1439299 2024-03-05 16:52:38.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/silero_vad.jit
--rw-rw-rw-   0        0        0    16566 2024-03-09 11:47:19.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/translator.py
-drwxrwxrwx   0        0        0        0 2024-03-09 12:05:14.552671 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/
--rw-rw-rw-   0        0        0     6004 2024-03-09 12:05:14.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2024-03-09 12:05:14.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 12:05:14.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-03-09 12:05:14.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2024-03-09 12:05:14.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-03-09 12:05:14.000000 stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 15:26:35.378684 stream_translator_gpt-2024.4.24/
+-rw-rw-rw-   0        0        0     1089 2023-03-12 08:56:05.000000 stream_translator_gpt-2024.4.24/LICENSE
+-rw-rw-rw-   0        0        0     6293 2024-04-24 15:26:35.377685 stream_translator_gpt-2024.4.24/PKG-INFO
+-rw-rw-rw-   0        0        0    15478 2024-04-24 15:23:39.000000 stream_translator_gpt-2024.4.24/README.md
+-rw-rw-rw-   0        0        0     4813 2024-03-26 11:06:30.000000 stream_translator_gpt-2024.4.24/README_PyPI.md
+-rw-rw-rw-   0        0        0     1745 2024-04-24 15:25:58.000000 stream_translator_gpt-2024.4.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:26:35.378684 stream_translator_gpt-2024.4.24/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 15:26:35.360503 stream_translator_gpt-2024.4.24/stream_translator_gpt/
+-rw-rw-rw-   0        0        0        0 2024-03-03 09:46:32.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-03-03 10:18:23.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/__main__.py
+-rw-rw-rw-   0        0        0     5572 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_getter.py
+-rw-rw-rw-   0        0        0     4102 2024-03-03 13:47:24.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_slicer.py
+-rw-rw-rw-   0        0        0     3821 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_transcriber.py
+-rw-rw-rw-   0        0        0      970 2024-03-25 19:53:37.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/common.py
+-rw-rw-rw-   0        0        0     1384 2024-03-14 15:15:25.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/filters.py
+-rw-rw-rw-   0        0        0     8300 2024-03-05 13:52:21.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/llm_translator.py
+-rw-rw-rw-   0        0        0     2731 2024-04-16 06:16:00.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/result_exporter.py
+-rw-rw-rw-   0        0        0  1439299 2024-03-05 16:52:38.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/silero_vad.jit
+-rw-rw-rw-   0        0        0    17087 2024-04-16 06:16:00.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/translator.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:26:35.377685 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/
+-rw-rw-rw-   0        0        0     6293 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/top_level.txt
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/LICENSE` & `stream_translator_gpt-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `stream-translator-gpt-2024.3.9.dev2/PKG-INFO` & `stream_translator_gpt-2024.4.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-translator-gpt
-Version: 2024.3.9.dev2
+Version: 2024.4.24
 Summary: Command line tool to transcribe & translate audio from livestreams in real time
 Author-email: ion <ionicbond3@gmail.com>
 Project-URL: Homepage, https://github.com/ionic-bond/stream-translator-gpt
 Project-URL: Issues, https://github.com/ionic-bond/stream-translator-gpt/issues
 Keywords: translator,translation,translate,transcribe,yt-dlp,vad,whisper,faster-whisper,whisper-api,gpt,gemini
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,15 @@
 Try it on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ionic-bond/stream-translator-gpt/blob/main/stream_translator.ipynb)
 
 ## Prerequisites
 
 **Linux or Windows:**
 
 1. Python >= 3.8 (Recommend >= 3.10)
-2. [**Install CUDA on your system.**](https://developer.nvidia.com/cuda-downloads) You can check the installed CUDA version with ```nvcc --version```.
+2. [**Install CUDA 11 on your system.**](https://developer.nvidia.com/cuda-11-8-0-download-archive) (Faster-Whisper is not compatible with CUDA 12 for now).
 3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cuda-downloads) if you want to use **Faseter-Whisper**.
 4. [**Install PyTorch (with CUDA) to your Python.**](https://pytorch.org/get-started/locally/)
 5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Recommend, Free 60 requests / minute)
 6. [**Create a OpenAI API key**](https://platform.openai.com/api-keys) if you want to use **Whisper API** for transcription or **GPT API** for translation.
 
 **If you are in Windows, you also need to:**
 
@@ -119,7 +119,11 @@
 - Sending result to Cqhttp:
 
     ```stream-translator-gpt {URL} --model large --language {input_language} --cqhttp_url {your_cqhttp_url} --cqhttp_token {your_cqhttp_token}```
 
 - Sending result to Discord:
 
     ```stream-translator-gpt {URL} --model large --language {input_language} --discord_webhook_url {your_discord_webhook_url}```
+
+- Saving result to a .srt subtitle file:
+
+    ```stream-translator-gpt {URL} --model large --language ja --gpt_translation_prompt "Translate from Japanese to Chinese" --google_api_key {your_google_key} --hide_transcribe_result --output_timestamps --output_file_path ./result.srt```
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/README.md` & `stream_translator_gpt-2024.4.24/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         da("`**GPT API**`")
         db("`**Gemini API**`")
     end
     subgraph ge["`**Output**`"]
         direction LR
         ea("`**Print to stdout**`")
         eb("`**Cqhttp**`")
+        ec("`**Discord**`")
+        ed("`**Telegram**`")
+        ee("`**Save to file**`")
     end
     aa --> gb
     ab --> gb
     gb ==> gc
     gc ==> gd
     gd ==> ge
 ```
@@ -53,15 +56,15 @@
 Try it on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ionic-bond/stream-translator-gpt/blob/main/stream_translator.ipynb)
 
 ## Prerequisites
 
 **Linux or Windows:**
 
 1. Python >= 3.8 (Recommend >= 3.10)
-2. [**Install CUDA on your system.**](https://developer.nvidia.com/cuda-downloads) You can check the installed CUDA version with ```nvcc --version```.
+2. [**Install CUDA 11 on your system.**](https://developer.nvidia.com/cuda-11-8-0-download-archive) (Faster-Whisper is not compatible with CUDA 12 for now).
 3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cuda-downloads) if you want to use **Faseter-Whisper**.
 4. [**Install PyTorch (with CUDA) to your Python.**](https://pytorch.org/get-started/locally/)
 5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Recommend, Free 60 requests / minute)
 6. [**Create a OpenAI API key**](https://platform.openai.com/api-keys) if you want to use **Whisper API** for transcription or **GPT API** for translation.
 
 **If you are in Windows, you also need to:**
 
@@ -131,31 +134,34 @@
 
     ```stream-translator-gpt {URL} --model large --language {input_language} --cqhttp_url {your_cqhttp_url} --cqhttp_token {your_cqhttp_token}```
 
 - Sending result to Discord:
 
     ```stream-translator-gpt {URL} --model large --language {input_language} --discord_webhook_url {your_discord_webhook_url}```
 
+- Saving result to a .srt subtitle file:
+
+    ```stream-translator-gpt {URL} --model large --language ja --gpt_translation_prompt "Translate from Japanese to Chinese" --google_api_key {your_google_key} --hide_transcribe_result --output_timestamps --output_file_path ./result.srt```
+
 ## All options
 
 | Option                             | Default Value | Description                                                                                                                                                                                              |
 | :--------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | **Input Options**                  |
 | `URL`                              |               | The URL of the stream. If a local file path is filled in, it will be used as input. If fill in "device", the input will be obtained from your PC device.                                                 |
 | `--format`                         | wa*           | Stream format code, this parameter will be passed directly to yt-dlp.                                                                                                                                    |
 | `--cookies`                        |               | Used to open member-only stream, this parameter will be passed directly to yt-dlp.                                                                                                                       |
-| `--direct_url`                     |               | Set this flag to pass the URL directly to ffmpeg. Otherwise, yt-dlp is used to obtain the stream URL.                                                                                                    |
 | `--device_index`                   |               | The index of the device that needs to be recorded. If not set, the system default recording device will be used.                                                                                         |
 | **Audio Slicing Options**          |
 | `--frame_duration`                 | 0.1           | The unit that processes live streaming data in seconds.                                                                                                                                                  |
-| `--continuous_no_speech_threshold` | 0.8           | Slice if there is no speech for a continuous period in second.                                                                                                                                           |
+| `--continuous_no_speech_threshold` | 0.5           | Slice if there is no speech for a continuous period in second.                                                                                                                                           |
 | `--min_audio_length`               | 3.0           | Minimum slice audio length in seconds.                                                                                                                                                                   |
 | `--max_audio_length`               | 30.0          | Maximum slice audio length in seconds.                                                                                                                                                                   |
-| `--prefix_retention_length`        | 0.8           | The length of the retention prefix audio during slicing.                                                                                                                                                 |
-| `--vad_threshold`                  | 0.5           | The threshold of Voice activity detection. if the speech probability of a frame is higher than this value, then this frame is speech.                                                                    |
+| `--prefix_retention_length`        | 0.5           | The length of the retention prefix audio during slicing.                                                                                                                                                 |
+| `--vad_threshold`                  | 0.35          | The threshold of Voice activity detection. if the speech probability of a frame is higher than this value, then this frame is speech.                                                                    |
 | **Transcription Options**          |
 | `--model`                          | small         | Select model size. See [here](https://github.com/openai/whisper#available-models-and-languages) for available models.                                                                                    |
 | `--language`                       | auto          | Language spoken in the stream. See [here](https://github.com/openai/whisper#available-models-and-languages) for available languages.                                                                     |
 | `--beam_size`                      | 5             | Number of beams in beam search. Set to 0 to use greedy algorithm instead (faster but less accurate).                                                                                                     |
 | `--best_of`                        | 5             | Number of candidates when sampling with non-zero temperature.                                                                                                                                            |
 | `--use_faster_whisper`             |               | Set this flag to use Faster Whisper implementation instead of the original OpenAI implementation                                                                                                         |
 | `--use_whisper_api`                |               | Set this flag to use OpenAI Whisper API instead of the original local Whipser.                                                                                                                           |
@@ -168,17 +174,20 @@
 | `--gpt_translation_history_size`   | 0             | The number of previous messages sent when calling the GPT / Gemini API. If the history size is 0, the translation will be run parallelly. If the history size > 0, the translation will be run serially. |
 | `--gpt_translation_timeout`        | 10            | If the GPT / Gemini translation exceeds this number of seconds, the translation will be discarded.                                                                                                       |
 | `--gpt_base_url`                   |               | Customize the API endpoint of GPT.                                                                                                                                                                       |
 | `--retry_if_translation_fails`     |               | Retry when translation times out/fails. Used to generate subtitles offline.                                                                                                                              |
 | **Output Options**                 |
 | `--output_timestamps`              |               | Output the timestamp of the text when outputting the text.                                                                                                                                               |
 | `--hide_transcribe_result`         |               | Hide the result of Whisper transcribe.                                                                                                                                                                   |
+| `--output_file_path`               |               | If set, will save the result text to this path.                                                                                                                                                          |
 | `--cqhttp_url`                     |               | If set, will send the result text to the cqhttp server.                                                                                                                                                  |
 | `--cqhttp_token`                   |               | Token of cqhttp, if it is not set on the server side, it does not need to fill in.                                                                                                                       |
 | `--discord_webhook_url`            |               | If set, will send the result text to the discord channel.                                                                                                                                                |
+| `--telegram_token`                 |               | Token of Telegram bot.                                                                                                                                                                                   |
+| `--telegram_chat_id`               |               | If set, will send the result text to this Telegram chat. Needs to be used with \"--telegram_token\".                                                                                                     |
 
 ## Contact me
 
 Telegram: [@ionic_bond](https://t.me/ionic_bond)
 
 ## Donate
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/README_PyPI.md` & `stream_translator_gpt-2024.4.24/README_PyPI.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Try it on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ionic-bond/stream-translator-gpt/blob/main/stream_translator.ipynb)
 
 ## Prerequisites
 
 **Linux or Windows:**
 
 1. Python >= 3.8 (Recommend >= 3.10)
-2. [**Install CUDA on your system.**](https://developer.nvidia.com/cuda-downloads) You can check the installed CUDA version with ```nvcc --version```.
+2. [**Install CUDA 11 on your system.**](https://developer.nvidia.com/cuda-11-8-0-download-archive) (Faster-Whisper is not compatible with CUDA 12 for now).
 3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cuda-downloads) if you want to use **Faseter-Whisper**.
 4. [**Install PyTorch (with CUDA) to your Python.**](https://pytorch.org/get-started/locally/)
 5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Recommend, Free 60 requests / minute)
 6. [**Create a OpenAI API key**](https://platform.openai.com/api-keys) if you want to use **Whisper API** for transcription or **GPT API** for translation.
 
 **If you are in Windows, you also need to:**
 
@@ -86,7 +86,11 @@
 - Sending result to Cqhttp:
 
     ```stream-translator-gpt {URL} --model large --language {input_language} --cqhttp_url {your_cqhttp_url} --cqhttp_token {your_cqhttp_token}```
 
 - Sending result to Discord:
 
     ```stream-translator-gpt {URL} --model large --language {input_language} --discord_webhook_url {your_discord_webhook_url}```
+
+- Saving result to a .srt subtitle file:
+
+    ```stream-translator-gpt {URL} --model large --language ja --gpt_translation_prompt "Translate from Japanese to Chinese" --google_api_key {your_google_key} --hide_transcribe_result --output_timestamps --output_file_path ./result.srt```
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/pyproject.toml` & `stream_translator_gpt-2024.4.24/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stream-translator-gpt"
-version = "2024.3.9.dev2"
+version = "2024.4.24"
 authors = [
   { name="ion", email="ionicbond3@gmail.com" },
 ]
 description = "Command line tool to transcribe & translate audio from livestreams in real time"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/audio_getter.py` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_getter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import queue
 import signal
 import subprocess
 import sys
 import threading
 
 import ffmpeg
@@ -17,28 +18,15 @@
             ffmpeg_proc.stdin.write(chunk)
         except (BrokenPipeError, OSError):
             pass
     ytdlp_proc.kill()
     ffmpeg_proc.kill()
 
 
-def _open_stream(url: str, direct_url: bool, format: str, cookies: str):
-    if direct_url:
-        try:
-            process = (ffmpeg.input(
-                url, loglevel='panic').output('pipe:',
-                                              format='s16le',
-                                              acodec='pcm_s16le',
-                                              ac=1,
-                                              ar=SAMPLE_RATE).run_async(pipe_stdout=True))
-        except ffmpeg.Error as e:
-            raise RuntimeError(f'Failed to load audio: {e.stderr.decode()}') from e
-
-        return process, None
-
+def _open_stream(url: str, format: str, cookies: str):
     cmd = ['yt-dlp', url, '-f', format, '-o', '-', '-q']
     if cookies:
         cmd.extend(['--cookies', cookies])
     ytdlp_process = subprocess.Popen(cmd, stdout=subprocess.PIPE)
 
     try:
         ffmpeg_process = (ffmpeg.input('pipe:', loglevel='panic').output('pipe:',
@@ -54,28 +42,37 @@
     thread = threading.Thread(target=_transport, args=(ytdlp_process, ffmpeg_process))
     thread.start()
     return ffmpeg_process, ytdlp_process
 
 
 class StreamAudioGetter(LoopWorkerBase):
 
-    def __init__(self, url: str, direct_url: bool, format: str, cookies: str,
-                 frame_duration: float) -> None:
+    def __init__(self, url: str, format: str, cookies: str, frame_duration: float) -> None:
+        self._cleanup_ytdlp_cache()
+
         print('Opening stream: {}'.format(url))
-        self.ffmpeg_process, self.ytdlp_process = _open_stream(url, direct_url, format, cookies)
+        self.ffmpeg_process, self.ytdlp_process = _open_stream(url, format, cookies)
         self.byte_size = round(frame_duration * SAMPLE_RATE *
                                2)  # Factor 2 comes from reading the int16 stream as bytes
         signal.signal(signal.SIGINT, self._exit_handler)
 
+    def __del__(self):
+        self._cleanup_ytdlp_cache()
+
     def _exit_handler(self, signum, frame):
         self.ffmpeg_process.kill()
         if self.ytdlp_process:
             self.ytdlp_process.kill()
         sys.exit(0)
 
+    def _cleanup_ytdlp_cache(self):
+        for file in os.listdir('./'):
+            if file.startswith('--Frag'):
+                os.remove(file)
+
     def loop(self, output_queue: queue.SimpleQueue[np.array]):
         while self.ffmpeg_process.poll() is None:
             in_bytes = self.ffmpeg_process.stdout.read(self.byte_size)
             if not in_bytes:
                 break
             if len(in_bytes) != self.byte_size:
                 continue
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/audio_slicer.py` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_slicer.py`

 * *Files identical despite different names*

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/audio_transcriber.py` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_transcriber.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import queue
 from scipy.io.wavfile import write as write_audio
 
 import numpy as np
 from openai import OpenAI
 
 from . import filters
-from .common import TranslationTask, SAMPLE_RATE, LoopWorkerBase
+from .common import TranslationTask, SAMPLE_RATE, LoopWorkerBase, sec2str
 
-TEMP_AUDIO_FILE_NAME = 'temp.wav'
+TEMP_AUDIO_FILE_NAME = '_whisper_api_temp.wav'
 
 
 def _filter_text(text: str, whisper_filters: str):
     filter_name_list = whisper_filters.split(',')
     for filter_name in filter_name_list:
         filter = getattr(filters, filter_name)
         if not filter:
@@ -34,25 +34,30 @@
                                        without_timestamps=True,
                                        language=self.language,
                                        **transcribe_options)
         return result.get('text')
 
     def loop(self, input_queue: queue.SimpleQueue[TranslationTask],
              output_queue: queue.SimpleQueue[TranslationTask], whisper_filters: str,
-             print_result: bool, **transcribe_options):
+             print_result: bool, output_timestamps: bool, **transcribe_options):
         while True:
             task = input_queue.get()
             task.transcribed_text = _filter_text(self.transcribe(task.audio, **transcribe_options),
                                                  whisper_filters).strip()
             if not task.transcribed_text:
                 if print_result:
                     print('skip...')
                 continue
             if print_result:
-                print(task.transcribed_text)
+                if output_timestamps:
+                    timestamp_text = '{} --> {}'.format(sec2str(task.time_range[0]),
+                                                        sec2str(task.time_range[1]))
+                    print(timestamp_text + ' ' + task.transcribed_text)
+                else:
+                    print(task.transcribed_text)
             output_queue.put(task)
 
 
 class FasterWhisper(OpenaiWhisper):
 
     def __init__(self, model: str, language: str) -> None:
         print('Loading faster-whisper model: {}'.format(model))
@@ -71,14 +76,18 @@
 class RemoteOpenaiWhisper(OpenaiWhisper):
     # https://platform.openai.com/docs/api-reference/audio/createTranscription?lang=python
 
     def __init__(self, language: str) -> None:
         self.client = OpenAI()
         self.language = language
 
+    def __del__(self):
+        if os.path.exists(TEMP_AUDIO_FILE_NAME):
+            os.remove(TEMP_AUDIO_FILE_NAME)
+
     def transcribe(self, audio: np.array, **transcribe_options) -> str:
         with open(TEMP_AUDIO_FILE_NAME, 'wb') as audio_file:
             write_audio(audio_file, SAMPLE_RATE, audio)
         with open(TEMP_AUDIO_FILE_NAME, 'rb') as audio_file:
             result = self.client.audio.transcriptions.create(model='whisper-1',
                                                              file=audio_file,
                                                              language=self.language).text
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/common.py` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import numpy as np
 from abc import ABC, abstractmethod
+from datetime import datetime
+
+import numpy as np
 from whisper.audio import SAMPLE_RATE
 
 
 class TranslationTask:
 
     def __init__(self, audio: np.array, time_range: tuple[float, float]):
         self.audio = audio
@@ -24,7 +26,14 @@
     def loop(self):
         pass
 
     @classmethod
     def work(cls, **kwargs):
         obj = cls(**_auto_args(cls.__init__, kwargs))
         obj.loop(**_auto_args(obj.loop, kwargs))
+
+
+def sec2str(second: float):
+    dt = datetime.utcfromtimestamp(second)
+    result = dt.strftime('%H:%M:%S')
+    result += ',' + str(round(second * 10 % 10))
+    return result
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/filters.py` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def japanese_stream_filter(text: str):
     for filter_pattern in [
             r'【.+】', r'ご視聴ありがとうございました', r'チャンネル登録をお願いいたします', r'ご視聴いただきありがとうございます', r'チャンネル登録してね',
             r'字幕視聴ありがとうございました', r'動画をご覧頂きましてありがとうございました', r'次の動画でお会いしましょう', r'最後までご視聴頂きありがとうございました',
             r'次の動画もお楽しみに', r'次回もお楽しみに', r'また次回の動画でお会いしましょう', r'ご覧いただきありがとうございます',
-            r'最後までご視聴頂き有難うございました', r'最後までご視聴頂き有難う御座いました'
+            r'最後までご視聴頂き有難うございました', r'最後までご視聴頂き有難う御座いました', r'チャンネル登録よろしくお願いします'
     ]:
         text = re.sub(filter_pattern, '', text)
 
     for filter_text in ['エンディング', '字幕作成', 'この動画の字幕']:
         if filter_text in text:
             print('filter', text)
             return ''
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/llm_translator.py` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/llm_translator.py`

 * *Files identical despite different names*

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/result_exporter.py` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/result_exporter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,70 @@
+import os
 import queue
 import requests
-from datetime import datetime
 
-from .common import TranslationTask, LoopWorkerBase
+from .common import TranslationTask, LoopWorkerBase, sec2str
 
 
 def _send_to_cqhttp(url: str, token: str, text: str):
     headers = {'Authorization': 'Bearer {}'.format(token)} if token else None
     data = {'message': text}
-    requests.post(url, headers=headers, data=data, timeout=10)
+    try:
+        requests.post(url, headers=headers, data=data, timeout=10)
+    except Exception as e:
+        print(e)
 
 
 def _send_to_discord(webhook_url: str, text: str):
     data = {'content': text}
-    requests.post(webhook_url, json=data, timeout=10)
-
-
-def _sec2str(second: float):
-    dt = datetime.utcfromtimestamp(second)
-    result = dt.strftime('%H:%M:%S')
-    result += ',' + str(round(second * 10 % 10))
-    return result
+    try:
+        requests.post(webhook_url, json=data, timeout=10)
+    except Exception as e:
+        print(e)
+
+
+def _send_to_telegram(token: str, chat_id: int, text: str):
+    url = 'https://api.telegram.org/bot{}/sendMessage?chat_id={}&text={}'.format(
+        token, chat_id, text)
+    try:
+        requests.post(url, timeout=10)
+    except Exception as e:
+        print(e)
+
+
+def _output_to_file(file_path: str, text: str):
+    with open(file_path, 'a') as f:
+        f.write(text + '\n\n')
 
 
 class ResultExporter(LoopWorkerBase):
 
-    def __init__(self) -> None:
-        pass
+    def __init__(self, output_file_path: str) -> None:
+        if output_file_path:
+            if os.path.exists(output_file_path):
+                os.remove(output_file_path)
 
     def loop(self, input_queue: queue.SimpleQueue[TranslationTask], output_whisper_result: bool,
-             output_timestamps: bool, cqhttp_url: str, cqhttp_token: str, discord_webhook_url: str):
+             output_timestamps: bool, output_file_path: str, cqhttp_url: str, cqhttp_token: str,
+             discord_webhook_url: str, telegram_token: str, telegram_chat_id: int):
         while True:
             task = input_queue.get()
-            timestamp_text = '{} --> {}'.format(_sec2str(task.time_range[0]),
-                                                _sec2str(task.time_range[1]))
+            timestamp_text = '{} --> {}'.format(sec2str(task.time_range[0]),
+                                                sec2str(task.time_range[1]))
             text_to_send = (task.transcribed_text + '\n') if output_whisper_result else ''
             if output_timestamps:
                 text_to_send = timestamp_text + '\n' + text_to_send
             if task.translated_text:
                 text_to_print = task.translated_text
                 if output_timestamps:
                     text_to_print = timestamp_text + ' ' + text_to_print
                 print('\033[1m{}\033[0m'.format(text_to_print))
                 text_to_send += task.translated_text
             text_to_send = text_to_send.strip()
+            if output_file_path:
+                _output_to_file(output_file_path, text_to_send)
             if cqhttp_url:
                 _send_to_cqhttp(cqhttp_url, cqhttp_token, text_to_send)
             if discord_webhook_url:
-                _send_to_discord(discord_webhook_url, text_to_send)
+                _send_to_discord(discord_webhook_url, text_to_send)
+            if telegram_token and telegram_chat_id:
+                _send_to_telegram(telegram_token, telegram_chat_id, text_to_send)
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/silero_vad.jit` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt/translator.py` & `stream_translator_gpt-2024.4.24/stream_translator_gpt/translator.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 def _start_daemon_thread(func, *args, **kwargs):
     thread = threading.Thread(target=func, args=args, kwargs=kwargs)
     thread.daemon = True
     thread.start()
 
 
-def main(url, format, cookies, direct_url, device_index, frame_duration,
-         continuous_no_speech_threshold, min_audio_length, max_audio_length,
-         prefix_retention_length, vad_threshold, model, language, use_faster_whisper,
-         use_whisper_api, whisper_filters, openai_api_key, google_api_key, gpt_translation_prompt,
-         gpt_translation_history_size, gpt_model, gpt_translation_timeout, gpt_base_url,
-         retry_if_translation_fails, output_timestamps, hide_transcribe_result, cqhttp_url,
-         cqhttp_token, discord_webhook_url, **transcribe_options):
+def main(url, format, cookies, device_index, frame_duration, continuous_no_speech_threshold,
+         min_audio_length, max_audio_length, prefix_retention_length, vad_threshold, model,
+         language, use_faster_whisper, use_whisper_api, whisper_filters, openai_api_key,
+         google_api_key, gpt_translation_prompt, gpt_translation_history_size, gpt_model,
+         gpt_translation_timeout, gpt_base_url, retry_if_translation_fails, output_timestamps,
+         hide_transcribe_result, output_file_path, cqhttp_url, cqhttp_token, discord_webhook_url,
+         telegram_token, telegram_chat_id, **transcribe_options):
 
     if openai_api_key:
         os.environ['OPENAI_API_KEY'] = openai_api_key
     if gpt_base_url:
         os.environ['OPENAI_BASE_URL'] = gpt_base_url
     if google_api_key:
         genai.configure(api_key=google_api_key)
@@ -40,17 +40,20 @@
     transcriber_to_translator_queue = queue.SimpleQueue()
     translator_to_exporter_queue = queue.SimpleQueue(
     ) if gpt_translation_prompt else transcriber_to_translator_queue
 
     _start_daemon_thread(ResultExporter.work,
                          output_whisper_result=not hide_transcribe_result,
                          output_timestamps=output_timestamps,
+                         output_file_path=output_file_path,
                          cqhttp_url=cqhttp_url,
                          cqhttp_token=cqhttp_token,
                          discord_webhook_url=discord_webhook_url,
+                         telegram_token=telegram_token,
+                         telegram_chat_id=telegram_chat_id,
                          input_queue=translator_to_exporter_queue)
     if gpt_translation_prompt:
         if google_api_key:
             llm_client = LLMClint(llm_type=LLMClint.LLM_TYPE.GEMINI,
                                   model='gemini-pro',
                                   prompt=gpt_translation_prompt,
                                   history_size=gpt_translation_history_size)
@@ -74,31 +77,34 @@
                                  input_queue=transcriber_to_translator_queue,
                                  output_queue=translator_to_exporter_queue)
     if use_faster_whisper:
         _start_daemon_thread(FasterWhisper.work,
                              model=model,
                              language=language,
                              print_result=not hide_transcribe_result,
+                             output_timestamps=output_timestamps,
                              input_queue=slicer_to_transcriber_queue,
                              output_queue=transcriber_to_translator_queue,
                              whisper_filters=whisper_filters,
                              **transcribe_options)
     elif use_whisper_api:
         _start_daemon_thread(RemoteOpenaiWhisper.work,
                              language=language,
                              print_result=not hide_transcribe_result,
+                             output_timestamps=output_timestamps,
                              input_queue=slicer_to_transcriber_queue,
                              output_queue=transcriber_to_translator_queue,
                              whisper_filters=whisper_filters,
                              **transcribe_options)
     else:
         _start_daemon_thread(OpenaiWhisper.work,
                              model=model,
                              language=language,
                              print_result=not hide_transcribe_result,
+                             output_timestamps=output_timestamps,
                              input_queue=slicer_to_transcriber_queue,
                              output_queue=transcriber_to_translator_queue,
                              whisper_filters=whisper_filters,
                              **transcribe_options)
     _start_daemon_thread(AudioSlicer.work,
                          frame_duration=frame_duration,
                          continuous_no_speech_threshold=continuous_no_speech_threshold,
@@ -114,15 +120,14 @@
                                output_queue=getter_to_slicer_queue)
     elif os.path.isabs(url):
         LocalFileAudioGetter.work(file_path=url,
                                   frame_duration=frame_duration,
                                   output_queue=getter_to_slicer_queue)
     else:
         StreamAudioGetter.work(url=url,
-                               direct_url=direct_url,
                                format=format,
                                cookies=cookies,
                                frame_duration=frame_duration,
                                output_queue=getter_to_slicer_queue)
 
     # Wait for others process finish.
     while (not getter_to_slicer_queue.empty() or not slicer_to_transcriber_queue.empty() or
@@ -144,49 +149,45 @@
                         help='Stream format code, '
                         'this parameter will be passed directly to yt-dlp.')
     parser.add_argument('--cookies',
                         type=str,
                         default=None,
                         help='Used to open member-only stream, '
                         'this parameter will be passed directly to yt-dlp.')
-    parser.add_argument('--direct_url',
-                        action='store_true',
-                        help='Set this flag to pass the URL directly to ffmpeg. '
-                        'Otherwise, yt-dlp is used to obtain the stream URL.')
     parser.add_argument('--device_index',
                         type=int,
                         default=None,
                         help='The index of the device that needs to be recorded. '
                         'If not set, the system default recording device will be used.')
     parser.add_argument('--print_all_devices',
                         action='store_true',
                         help='Print all audio devices info then exit.')
     parser.add_argument('--frame_duration',
                         type=float,
                         default=0.1,
                         help='The unit that processes live streaming data in seconds.')
     parser.add_argument('--continuous_no_speech_threshold',
                         type=float,
-                        default=0.8,
+                        default=0.5,
                         help='Slice if there is no speech for a continuous period in second.')
     parser.add_argument('--min_audio_length',
                         type=float,
                         default=3.0,
                         help='Minimum slice audio length in seconds.')
     parser.add_argument('--max_audio_length',
                         type=float,
                         default=30.0,
                         help='Maximum slice audio length in seconds.')
     parser.add_argument('--prefix_retention_length',
                         type=float,
-                        default=0.8,
+                        default=0.5,
                         help='The length of the retention prefix audio during slicing.')
     parser.add_argument('--vad_threshold',
                         type=float,
-                        default=0.5,
+                        default=0.35,
                         help='The threshold of Voice activity detection.'
                         'if the speech probability of a frame is higher than this value, '
                         'then this frame is speech.')
     parser.add_argument('--model',
                         type=str,
                         choices=[
                             'tiny', 'tiny.en', 'small', 'small.en', 'medium', 'medium.en', 'large',
@@ -265,27 +266,39 @@
         help='Retry when translation times out/fails. Used to generate subtitles offline.')
     parser.add_argument('--output_timestamps',
                         action='store_true',
                         help='Output the timestamp of the text when outputting the text.')
     parser.add_argument('--hide_transcribe_result',
                         action='store_true',
                         help='Hide the result of Whisper transcribe.')
+    parser.add_argument('--output_file_path',
+                        type=str,
+                        default=None,
+                        help='If set, will save the result text to this path.')
     parser.add_argument('--cqhttp_url',
                         type=str,
                         default=None,
-                        help='If set, will send the result text to the cqhttp server.')
+                        help='If set, will send the result text to this Cqhttp server.')
     parser.add_argument('--cqhttp_token',
                         type=str,
                         default=None,
                         help='Token of cqhttp, if it is not set on the server side, '
                         'it does not need to fill in.')
     parser.add_argument('--discord_webhook_url',
                         type=str,
                         default=None,
-                        help='If set, will send the result text to the discord channel.')
+                        help='If set, will send the result text to this Discord channel.')
+    parser.add_argument('--telegram_token', type=str, default=None, help='Token of Telegram bot.')
+    parser.add_argument(
+        '--telegram_chat_id',
+        type=int,
+        default=None,
+        help=
+        'If set, will send the result text to this Telegram chat. Needs to be used with \"--telegram_token\".'
+    )
 
     args = parser.parse_args().__dict__
     url = args.pop('URL')
 
     if args['print_all_devices']:
         import sounddevice as sd
         print(sd.query_devices())
@@ -321,13 +334,8 @@
 
     if args['language'] == 'auto':
         args['language'] = None
 
     if args['beam_size'] == 0:
         args['beam_size'] = None
 
-    # Remove yt-dlp cache
-    for file in os.listdir('./'):
-        if file.startswith('--Frag'):
-            os.remove(file)
-
     main(url, **args)
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/PKG-INFO` & `stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-translator-gpt
-Version: 2024.3.9.dev2
+Version: 2024.4.24
 Summary: Command line tool to transcribe & translate audio from livestreams in real time
 Author-email: ion <ionicbond3@gmail.com>
 Project-URL: Homepage, https://github.com/ionic-bond/stream-translator-gpt
 Project-URL: Issues, https://github.com/ionic-bond/stream-translator-gpt/issues
 Keywords: translator,translation,translate,transcribe,yt-dlp,vad,whisper,faster-whisper,whisper-api,gpt,gemini
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,15 @@
 Try it on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ionic-bond/stream-translator-gpt/blob/main/stream_translator.ipynb)
 
 ## Prerequisites
 
 **Linux or Windows:**
 
 1. Python >= 3.8 (Recommend >= 3.10)
-2. [**Install CUDA on your system.**](https://developer.nvidia.com/cuda-downloads) You can check the installed CUDA version with ```nvcc --version```.
+2. [**Install CUDA 11 on your system.**](https://developer.nvidia.com/cuda-11-8-0-download-archive) (Faster-Whisper is not compatible with CUDA 12 for now).
 3. [**Install cuDNN to your CUDA dir**](https://developer.nvidia.com/cuda-downloads) if you want to use **Faseter-Whisper**.
 4. [**Install PyTorch (with CUDA) to your Python.**](https://pytorch.org/get-started/locally/)
 5. [**Create a Google API key**](https://aistudio.google.com/app/apikey) if you want to use **Gemini API** for translation. (Recommend, Free 60 requests / minute)
 6. [**Create a OpenAI API key**](https://platform.openai.com/api-keys) if you want to use **Whisper API** for transcription or **GPT API** for translation.
 
 **If you are in Windows, you also need to:**
 
@@ -119,7 +119,11 @@
 - Sending result to Cqhttp:
 
     ```stream-translator-gpt {URL} --model large --language {input_language} --cqhttp_url {your_cqhttp_url} --cqhttp_token {your_cqhttp_token}```
 
 - Sending result to Discord:
 
     ```stream-translator-gpt {URL} --model large --language {input_language} --discord_webhook_url {your_discord_webhook_url}```
+
+- Saving result to a .srt subtitle file:
+
+    ```stream-translator-gpt {URL} --model large --language ja --gpt_translation_prompt "Translate from Japanese to Chinese" --google_api_key {your_google_key} --hide_transcribe_result --output_timestamps --output_file_path ./result.srt```
```

### Comparing `stream-translator-gpt-2024.3.9.dev2/stream_translator_gpt.egg-info/SOURCES.txt` & `stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

