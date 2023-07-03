# Comparing `tmp/lyrics_transcriber-0.3.5.tar.gz` & `tmp/lyrics_transcriber-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.3.5.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.4.1.tar", max compression
```

## Comparing `lyrics_transcriber-0.3.5.tar` & `lyrics_transcriber-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.3.5/LICENSE
--rw-r--r--   0        0        0     3460 2023-07-02 17:33:07.092697 lyrics_transcriber-0.3.5/README.md
--rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.3.5/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0     9842 2023-07-02 17:14:48.003079 lyrics_transcriber-0.3.5/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.3.5/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     3247 2023-07-01 07:57:15.589521 lyrics_transcriber-0.3.5/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0     1054 2023-07-03 03:25:19.197843 lyrics_transcriber-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4480 1970-01-01 00:00:00.000000 lyrics_transcriber-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3523 2023-07-03 03:34:02.162763 lyrics_transcriber-0.4.1/README.md
+-rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.4.1/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0    10321 2023-07-03 04:09:45.243605 lyrics_transcriber-0.4.1/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.4.1/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     3532 2023-07-03 04:10:21.670806 lyrics_transcriber-0.4.1/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0     1206 2023-07-03 03:33:02.897814 lyrics_transcriber-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 lyrics_transcriber-0.4.1/PKG-INFO
```

### Comparing `lyrics_transcriber-0.3.5/LICENSE` & `lyrics_transcriber-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.3.5/README.md` & `lyrics_transcriber-0.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Lyrics Transcriber 🎶
 
-Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using OpenAI Whisper and lyrics from Genius and Spotify.
+Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using OpenAI Whisper and lyrics from Genius and Spotify, for convenience in use cases such as karaoke video production.
 
 ## Features 🌟
 
 - Automatically transcribe lyrics with word-level timestamps.
 - Outputs lyrics in ASS and MidiCo LRC formats.
 - Can fetch lyrics from with Genius and Spotify.
 - Command Line Interface (CLI) for easy usage.
```

### Comparing `lyrics_transcriber-0.3.5/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.4.1/lyrics_transcriber/transcriber.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 import json
+import logging
 import shutil
 import hashlib
-import datetime
 import subprocess
 import slugify
 import whisper_timestamped as whisper
 import lyricsgenius
 
 
 class LyricsTranscriber:
@@ -15,16 +15,26 @@
         self,
         audio_filepath,
         song_artist=None,
         song_title=None,
         genius_api_token=None,
         output_dir=None,
         cache_dir="/tmp/lyrics-transcriber-cache/",
+        log_level=logging.DEBUG,
+        log_format="%(asctime)s - %(module)s - %(levelname)s - %(message)s",
     ):
-        log(f"LyricsTranscriber instantiating with input file: {audio_filepath}")
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(log_level)
+
+        log_handler = logging.StreamHandler()
+        log_formatter = logging.Formatter(log_format)
+        log_handler.setFormatter(log_formatter)
+        self.logger.addHandler(log_handler)
+
+        self.logger.debug(f"LyricsTranscriber instantiating with input file: {audio_filepath}")
 
         self.cache_dir = cache_dir
         self.output_dir = output_dir
         self.audio_filepath = audio_filepath
         self.song_artist = song_artist
         self.song_title = song_title
         self.genius_api_token = genius_api_token
@@ -43,32 +53,32 @@
 
         if self.audio_filepath is None:
             raise Exception("audio_filepath must be specified as the input source to transcribe")
 
         self.create_folders()
 
     def generate(self):
-        log(f"audio_filepath is set: {self.audio_filepath}, beginning initial whisper transcription")
+        self.logger.debug(f"audio_filepath is set: {self.audio_filepath}, beginning initial whisper transcription")
 
         self.result_metadata["whisper_json_filepath"] = self.get_cache_filepath(".json")
         self.whisper_result_dict = self.transcribe()
 
         self.result_metadata["midico_lrc_filepath"] = self.get_cache_filepath(".lrc")
         self.write_midico_lrc_file()
 
         self.calculate_singing_percentage()
 
         if self.genius_api_token and self.song_artist and self.song_title:
-            log(
+            self.logger.debug(
                 f"fetching lyrics from Genius as genius_api_token: {self.genius_api_token}, song_artist: {self.song_artist} and song_title: {self.song_title} were set"
             )
             self.result_metadata["genius_lyrics_filepath"] = self.get_cache_filepath("-genius.txt")
             self.write_genius_lyrics_file()
         else:
-            log(
+            self.logger.debug(
                 f"not fetching lyrics from Genius as not all genius params were set: genius_api_token: {self.genius_api_token}, song_artist: {self.song_artist} and song_title: {self.song_title}"
             )
 
         # TODO: attempt to match up segments from genius lyrics with whisper segments
 
         # TODO: output synced lyrics from self.whisper_result_dict in ASS format too, using code from the_tuul
 
@@ -83,31 +93,31 @@
 
         return self.result_metadata
 
     def write_genius_lyrics_file(self):
         genius_lyrics_cache_filepath = os.path.join(self.cache_dir, self.get_song_slug() + "-genius.txt")
 
         if os.path.isfile(genius_lyrics_cache_filepath):
-            log(f"found existing file at genius_lyrics_cache_filepath, reading: {genius_lyrics_cache_filepath}")
+            self.logger.debug(f"found existing file at genius_lyrics_cache_filepath, reading: {genius_lyrics_cache_filepath}")
 
             with open(genius_lyrics_cache_filepath, "r") as cached_lyrics:
                 self.result_metadata["genius_lyrics_filepath"] = genius_lyrics_cache_filepath
                 self.result_metadata["genius_lyrics"] = cached_lyrics
                 return cached_lyrics
 
-        log(f"no cached lyrics found at genius_lyrics_cache_filepath: {genius_lyrics_cache_filepath}, fetching from Genius")
+        self.logger.debug(f"no cached lyrics found at genius_lyrics_cache_filepath: {genius_lyrics_cache_filepath}, fetching from Genius")
         genius = lyricsgenius.Genius(self.genius_api_token)
 
         song = genius.search_song(self.song_title, self.song_artist)
         if song is None:
-            print(f'Could not find lyrics on Genius for "{self.song_title}" by {self.song_artist}')
+            self.logger.warning(f'Could not find lyrics on Genius for "{self.song_title}" by {self.song_artist}')
             return
         lyrics = self.clean_genius_lyrics(song.lyrics)
 
-        log(f"writing clean lyrics to genius_lyrics_cache_filepath: {genius_lyrics_cache_filepath}")
+        self.logger.debug(f"writing clean lyrics to genius_lyrics_cache_filepath: {genius_lyrics_cache_filepath}")
         with open(genius_lyrics_cache_filepath, "w") as f:
             f.write(lyrics)
 
         self.result_metadata["genius_lyrics_filepath"] = genius_lyrics_cache_filepath
         self.result_metadata["genius_lyrics"] = lyrics
         return lyrics
 
@@ -123,15 +133,15 @@
         # add any additional cleaning rules here
         return lyrics
 
     def calculate_singing_percentage(self):
         # Calculate total seconds of singing using timings from whisper transcription results
         total_singing_duration = sum(segment["end"] - segment["start"] for segment in self.whisper_result_dict["segments"])
 
-        log(f"calculated total_singing_duration: {int(total_singing_duration)} seconds, now running ffprobe")
+        self.logger.debug(f"calculated total_singing_duration: {int(total_singing_duration)} seconds, now running ffprobe")
 
         # Calculate total song duration using ffprobe
         duration_command = [
             "ffprobe",
             "-i",
             self.audio_filepath,
             "-show_entries",
@@ -154,15 +164,15 @@
         return singing_percentage, total_singing_duration, song_duration
 
     # Loops through lyrics segments (typically sentences) from whisper_timestamps JSON output,
     # then loops over each word and writes all words with MidiCo segment start/end formatting
     # and word-level timestamps to a MidiCo-compatible LRC file
     def write_midico_lrc_file(self):
         lrc_filename = self.result_metadata["midico_lrc_filepath"]
-        log(f"writing midico formatted word timestamps to LRC file: {lrc_filename}")
+        self.logger.debug(f"writing midico formatted word timestamps to LRC file: {lrc_filename}")
         with open(lrc_filename, "w") as f:
             f.write("[re:MidiCo]\n")
             for segment in self.whisper_result_dict["segments"]:
                 for i, word in enumerate(segment["words"]):
                     start_time = self.format_time_lrc(word["start"])
                     if i != len(segment["words"]) - 1:
                         word["text"] += " "
@@ -175,35 +185,35 @@
         milliseconds = int((duration % 1) * 1000)
         formatted_time = f"{minutes:02d}:{seconds:02d}.{milliseconds:03d}"
         return formatted_time
 
     def transcribe(self):
         whisper_cache_filepath = self.result_metadata["whisper_json_filepath"]
         if os.path.isfile(whisper_cache_filepath):
-            log(f"transcribe found existing file at whisper_cache_filepath, reading: {whisper_cache_filepath}")
+            self.logger.debug(f"transcribe found existing file at whisper_cache_filepath, reading: {whisper_cache_filepath}")
             with open(whisper_cache_filepath, "r") as cache_file:
                 return json.load(cache_file)
 
-        log(f"no cached transcription file found, running whisper transcribe")
+        self.logger.debug(f"no cached transcription file found, running whisper transcribe")
         audio = whisper.load_audio(self.audio_filepath)
         model = whisper.load_model("medium.en", device="cpu")
         result = whisper.transcribe(model, audio, language="en")
 
-        log(f"whisper transcription complete, writing JSON to cache file: {whisper_cache_filepath}")
+        self.logger.debug(f"whisper transcription complete, writing JSON to cache file: {whisper_cache_filepath}")
         with open(whisper_cache_filepath, "w") as cache_file:
             json.dump(result, cache_file, indent=2)
 
         return result
 
     def get_cache_filepath(self, extension):
         filename = os.path.split(self.audio_filepath)[1]
         filename_slug = slugify.slugify(filename)
         hash_value = self.get_file_hash(self.audio_filepath)
         cache_filepath = os.path.join(self.cache_dir, filename_slug + "_" + hash_value + extension)
-        log(f"get_cache_filepath returning cache_filepath: {cache_filepath}")
+        self.logger.debug(f"get_cache_filepath returning cache_filepath: {cache_filepath}")
         return cache_filepath
 
     def get_song_slug(self):
         song_artist_slug = slugify.slugify(self.song_artist)
         song_title_slug = slugify.slugify(self.song_title)
         return song_artist_slug + "_" + song_title_slug
 
@@ -212,12 +222,7 @@
 
     def create_folders(self):
         if self.cache_dir is not None:
             os.makedirs(self.cache_dir, exist_ok=True)
 
         if self.output_dir is not None:
             os.makedirs(self.output_dir, exist_ok=True)
-
-
-def log(message):
-    timestamp = datetime.datetime.now().isoformat()
-    print(f"{timestamp} - {message}")
```

### Comparing `lyrics_transcriber-0.3.5/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.4.1/lyrics_transcriber/utils/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 #!/usr/bin/env python
 import argparse
-import datetime
+import logging
 import pkg_resources
 from lyrics_transcriber import LyricsTranscriber
 
 
-def log(message):
-    timestamp = datetime.datetime.now().isoformat()
-    print(f"{timestamp} - {message}")
+def main():
+    logger = logging.getLogger(__name__)
+    logger.setLevel(logging.DEBUG)
 
+    log_handler = logging.StreamHandler()
+    log_formatter = logging.Formatter("%(asctime)s - %(module)s - %(levelname)s - %(message)s")
+    log_handler.setFormatter(log_formatter)
+    logger.addHandler(log_handler)
+
+    logger.debug("Parsing CLI args")
 
-def main():
     parser = argparse.ArgumentParser(
         description="Create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, from any input song file"
     )
 
     parser.add_argument("audio_filepath", nargs="?", help="The audio file path to transcribe lyrics for.", default=argparse.SUPPRESS)
 
     parser.add_argument(
@@ -54,39 +59,39 @@
         exit(1)
 
     if 1 <= [args.genius_api_token, args.song_title, args.song_artist].count(True) < 3:
         print(f"To use genius lyrics auto-correction, all 3 args genius_api_token, song_artist, song_title must be provided")
         print(args)
         exit(1)
 
+    logger.debug("Loading LyricsTranscriber class")
+
     transcriber = LyricsTranscriber(
         args.audio_filepath,
         genius_api_token=args.genius_api_token,
         song_artist=args.song_artist,
         song_title=args.song_title,
         output_dir=args.output_dir,
         cache_dir=args.cache_dir,
     )
 
-    log("LyricsTranscriber beginning transcription")
-
     result_metadata = transcriber.generate()
 
-    log(f"*** Success! ***")
+    logger.info(f"*** Success! ***")
 
     formatted_duration = f'{int(result_metadata["song_duration"] // 60):02d}:{int(result_metadata["song_duration"] % 60):02d}'
-    log(f"Total Song Duration: {formatted_duration}")
+    logger.info(f"Total Song Duration: {formatted_duration}")
 
     formatted_singing_duration = (
         f'{int(result_metadata["total_singing_duration"] // 60):02d}:{int(result_metadata["total_singing_duration"] % 60):02d}'
     )
-    log(f"Total Singing Duration: {formatted_singing_duration}")
-    log(f"Singing Percentage: {result_metadata['singing_percentage']}%")
+    logger.info(f"Total Singing Duration: {formatted_singing_duration}")
+    logger.info(f"Singing Percentage: {result_metadata['singing_percentage']}%")
 
-    log(f"*** Outputs: ***")
-    log(f"Whisper transcription output JSON file: {result_metadata['whisper_json_filepath']}")
-    log(f"MidiCo LRC output file: {result_metadata['midico_lrc_filepath']}")
-    log(f"Genius lyrics output file: {result_metadata['genius_lyrics_filepath']}")
+    logger.info(f"*** Outputs: ***")
+    logger.info(f"Whisper transcription output JSON file: {result_metadata['whisper_json_filepath']}")
+    logger.info(f"MidiCo LRC output file: {result_metadata['midico_lrc_filepath']}")
+    logger.info(f"Genius lyrics output file: {result_metadata['genius_lyrics_filepath']}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lyrics_transcriber-0.3.5/PKG-INFO` & `lyrics_transcriber-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.3.5
+Version: 0.4.1
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 Requires-Dist: torch (>=1,<2)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: whisper-timestamped (>=1,<2)
 Description-Content-Type: text/markdown
 
 # Lyrics Transcriber 🎶
 
-Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using OpenAI Whisper and lyrics from Genius and Spotify.
+Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using OpenAI Whisper and lyrics from Genius and Spotify, for convenience in use cases such as karaoke video production.
 
 ## Features 🌟
 
 - Automatically transcribe lyrics with word-level timestamps.
 - Outputs lyrics in ASS and MidiCo LRC formats.
 - Can fetch lyrics from with Genius and Spotify.
 - Command Line Interface (CLI) for easy usage.
```

