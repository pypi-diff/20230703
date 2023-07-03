# Comparing `tmp/animethemes-beta-batch-encoder-1.2.tar.gz` & `tmp/animethemes-beta-batch-encoder-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-beta-batch-encoder-1.2.tar", last modified: Thu Jun 22 20:31:02 2023, max compression
+gzip compressed data, was "animethemes-beta-batch-encoder-1.3.tar", last modified: Mon Jul  3 04:42:14 2023, max compression
```

## Comparing `animethemes-beta-batch-encoder-1.2.tar` & `animethemes-beta-batch-encoder-1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 20:31:02.647549 animethemes-beta-batch-encoder-1.2/
--rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.2/LICENSE
--rw-rw-rw-   0        0        0     5014 2023-06-22 20:31:02.646547 animethemes-beta-batch-encoder-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4106 2023-06-22 20:14:45.000000 animethemes-beta-batch-encoder-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 20:31:02.631548 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     5014 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 20:31:02.645547 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/
--rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     7944 2023-06-22 19:10:50.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    13543 2023-06-22 18:39:34.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     4115 2023-06-22 08:05:47.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     6848 2023-06-22 20:08:15.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_interface.py
--rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     6874 2023-06-22 19:02:20.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2023-06-22 20:31:02.647549 animethemes-beta-batch-encoder-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-22 20:09:55.000000 animethemes-beta-batch-encoder-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:42:14.095469 animethemes-beta-batch-encoder-1.3/
+-rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.3/LICENSE
+-rw-rw-rw-   0        0        0     5410 2023-07-03 04:42:14.094469 animethemes-beta-batch-encoder-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4502 2023-07-03 04:40:29.000000 animethemes-beta-batch-encoder-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 04:42:13.914469 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/
+-rw-rw-rw-   0        0        0     5410 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-03 04:42:13.000000 animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 04:42:14.093488 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/
+-rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/__init__.py
+-rw-rw-rw-   0        0        0     8114 2023-07-02 21:46:33.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/__main__.py
+-rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_bitrate_mode.py
+-rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_colorspace.py
+-rw-rw-rw-   0        0        0    13543 2023-06-22 18:39:34.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_encode_webm.py
+-rw-rw-rw-   0        0        0     4115 2023-06-22 08:05:47.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_encoding_config.py
+-rw-rw-rw-   0        0        0     8234 2023-07-03 01:27:35.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_interface.py
+-rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_loudnorm_filter.py
+-rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_seek.py
+-rw-rw-rw-   0        0        0     5522 2023-07-03 04:36:38.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_seek_collector.py
+-rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_source_file.py
+-rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-03 04:42:14.095469 animethemes-beta-batch-encoder-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-07-03 04:37:51.000000 animethemes-beta-batch-encoder-1.3/setup.py
```

### Comparing `animethemes-beta-batch-encoder-1.2/LICENSE` & `animethemes-beta-batch-encoder-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/PKG-INFO` & `animethemes-beta-batch-encoder-1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.2
+Version: 1.3
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -79,14 +79,24 @@
 
 * `Exit` Saves audio filters if selected and continues script execution.
 * `Custom` Apply a custom audio filter string.
 * `Fade In` Select an exponential value to apply Fade In.
 * `Fade Out` Select a start position and an exponential value to Fade Out.
 * `Mute` Select a start and end position to leave the volume at 0.
 
+**Video Filters**
+
+* `scale=-1:720` Add downscale to 720p
+* `scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp` Add downscale to 720p and filters by AnimeThemes
+* `hqdn3d=0:0:3:3,gradfun,unsharp` Add filters by AnimeThemes
+* `hqdn3d=0:0:3:3` Add lightdenoise filter
+* `hqdn3d=1.5:1.5:6:6` Add heavydenoise filter
+* `unsharp` Add unsharp filter
+* `Custom` Apply a custom video filter string.
+
 **Encoding Properties**
 
 `AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
 
 `EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
 
 Available bitrate control modes are:
```

### Comparing `animethemes-beta-batch-encoder-1.2/README.md` & `animethemes-beta-batch-encoder-1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,24 @@
 
 * `Exit` Saves audio filters if selected and continues script execution.
 * `Custom` Apply a custom audio filter string.
 * `Fade In` Select an exponential value to apply Fade In.
 * `Fade Out` Select a start position and an exponential value to Fade Out.
 * `Mute` Select a start and end position to leave the volume at 0.
 
+**Video Filters**
+
+* `scale=-1:720` Add downscale to 720p
+* `scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp` Add downscale to 720p and filters by AnimeThemes
+* `hqdn3d=0:0:3:3,gradfun,unsharp` Add filters by AnimeThemes
+* `hqdn3d=0:0:3:3` Add lightdenoise filter
+* `hqdn3d=1.5:1.5:6:6` Add heavydenoise filter
+* `unsharp` Add unsharp filter
+* `Custom` Apply a custom video filter string.
+
 **Encoding Properties**
 
 `AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
 
 `EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
 
 Available bitrate control modes are:
```

### Comparing `animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/PKG-INFO` & `animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.2
+Version: 1.3
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -79,14 +79,24 @@
 
 * `Exit` Saves audio filters if selected and continues script execution.
 * `Custom` Apply a custom audio filter string.
 * `Fade In` Select an exponential value to apply Fade In.
 * `Fade Out` Select a start position and an exponential value to Fade Out.
 * `Mute` Select a start and end position to leave the volume at 0.
 
+**Video Filters**
+
+* `scale=-1:720` Add downscale to 720p
+* `scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp` Add downscale to 720p and filters by AnimeThemes
+* `hqdn3d=0:0:3:3,gradfun,unsharp` Add filters by AnimeThemes
+* `hqdn3d=0:0:3:3` Add lightdenoise filter
+* `hqdn3d=1.5:1.5:6:6` Add heavydenoise filter
+* `unsharp` Add unsharp filter
+* `Custom` Apply a custom video filter string.
+
 **Encoding Properties**
 
 `AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
 
 `EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
 
 Available bitrate control modes are:
```

### Comparing `animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/SOURCES.txt` & `animethemes-beta-batch-encoder-1.3/animethemes_beta_batch_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/__main__.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,18 @@
                 while not is_collector_valid:
                     print(f'\033[92mSource File: {file}\033[0m')
                     seek_collector = SeekCollector(file_value)
                     is_collector_valid = seek_collector.is_valid()
 
                 for seek in seek_collector.get_seek_list():
                     new_encoding_config = copy.copy(encoding_config)
+
+                    print(f'\033[92mOutput Name: {seek.output_name}\033[0m')
+                    new_encoding_config = Interface.video_filters(new_encoding_config)
+
                     if args.custom:
                         print(f'\033[92mOutput Name: {seek.output_name}\033[0m')
                         new_encoding_config = Interface.custom_options(new_encoding_config)
                         
                     logging.info(f'Generating commands with seek ss: \'{seek.ss}\', to: \'{seek.to}\'')
                     encode_webm = EncodeWebM(file_value, seek)
                     load_commands = encode_webm.get_commands(new_encoding_config)
```

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_bitrate_mode.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_colorspace.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_encode_webm.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_encode_webm.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_encoding_config.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_encoding_config.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_interface.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,34 +2,57 @@
 import logging
 import re
 
 class Interface:
     # Time Duration Specification: https://ffmpeg.org/ffmpeg-utils.html#time-duration-syntax
     time_pattern = re.compile('^([0-5]?\d:){1,2}[0-5]?\d(?=\.\d+$|$)|\d+(?=\.\d+$|$)')
 
-    # Prompt the mode options to run to the user
+    # Validations
+    validate_time = lambda _, x: all(Interface.time_pattern.match(y) for y in x.split(','))
+    validate_crfs = lambda _, x: all(y.strip().isdigit() for y in x.split(','))
+    validate_encoding_modes = lambda _, x: all(y.strip().upper() in ['VBR', 'CBR', 'CQ'] for y in x.split(','))
+
+    # Prompt the user for text questions
+    def prompt_text(message, validate=lambda _, x: x):
+        question = [inquirer.Text('text', message=message, validate=validate)]
+        answer = inquirer.prompt(question)
+
+        logging.debug(f'[Interface.prompt_text] answer["text"]: \'{answer["text"]}\'')
+
+        return answer['text']
+    
+    # Prompt the user for time questions
+    def prompt_time(message):
+        question = [inquirer.Text('time', message=message, validate=Interface.validate_time)]
+        answer = inquirer.prompt(question)
+
+        logging.debug(f'[Interface.prompt_time] answer["time"]: \'{answer["time"]}\'')
+
+        return answer['time']
+
+    # Prompt the user for our mode options to run to the user
     def choose_mode():
         modes = [('Generate commands', 1), ('Execute commands', 2), ('Generate and execute commands', 3)]
         question = [inquirer.List('mode', message='Mode (Enter)', choices=modes)]
         answer = inquirer.prompt(question)
 
         logging.debug(f'[Interface.choose_mode] answer["mode"]: \'{answer["mode"]}\'')
 
         return answer['mode']
     
-    # Prompt the source files to choose
+    # Prompt the user for source files to choose
     def choose_source_files(source_files):
         question = [inquirer.Checkbox('source_files', message='Source Files (Space to select)', choices=source_files)]
         answer = inquirer.prompt(question)
 
         logging.debug(f'[Interface.choose_source_files] answer["source_files"]: \'{answer["source_files"]}\'')
 
         return answer['source_files']
-    
-    # Prompt the audio filters options
+      
+    # Prompt the user for audio filters options
     def audio_filters_options(output_name):
         audio_filters = {
             'Exit': False,
             'Custom': '',
             'Fade In': 0,
             'Fade Out': {
                 'Start Time': 0,
@@ -43,49 +66,26 @@
 
         while not audio_filters['Exit']:
             print(f'\n\033[92mOutput Name: {output_name}\033[0m')
             question = [inquirer.List('audio_filters', message='Audio Filters (Enter)', choices=list(audio_filters.keys()))]
             answer = inquirer.prompt(question)
 
             if answer['audio_filters'] == 'Fade In':
-                while True:
-                    exp_value = input('Exponential Value: ').strip() or '0'
+                audio_filters['Fade In'] = Interface.prompt_time('Exponential Value').strip() or '0'
 
-                    if exp_value == 0 or Interface.time_pattern.match(exp_value):
-                        audio_filters['Fade In'] = exp_value
-                        break
-                    else:
-                        logging.error('Invalid Time')
-    
             elif answer['audio_filters'] == 'Fade Out':
-                while True:
-                    start_time = input('Start Time: ').strip() or '0'
-                    exp_value = input('Exponential Value: ').strip() or '0'
-
-                    if Interface.time_pattern.match(start_time) and Interface.time_pattern.match(exp_value):
-                        audio_filters['Fade Out']['Start Time'] = start_time
-                        audio_filters['Fade Out']['Exp'] = exp_value
-                        break
-                    else:
-                        logging.error('Invalid Time')
-
+                audio_filters['Fade Out']['Start Time'] = Interface.prompt_time('Start Time').strip() or '0'
+                audio_filters['Fade Out']['Exp'] = Interface.prompt_time('Exponential Value').strip() or '0'
+                     
             elif answer['audio_filters'] == 'Mute':
-                while True:
-                    start_time = input('Start Time: ').strip() or '0'
-                    end_time = input('End Time: ').strip() or '0'
-
-                    if Interface.time_pattern.match(start_time) and Interface.time_pattern.match(end_time):
-                        audio_filters['Mute']['Start Time'] = start_time
-                        audio_filters['Mute']['End Time'] = end_time
-                        break
-                    else:
-                        logging.error('Invalid Time')
+                audio_filters['Mute']['Start Time'] = Interface.prompt_time('Start Time').strip() or '0'
+                audio_filters['Mute']['End Time'] = Interface.prompt_time('End Time').strip() or '0'
 
             elif answer['audio_filters'] == 'Custom':
-                custom_audio_filter = input('Custom Audio Filter(s): ').strip()
+                custom_audio_filter = Interface.prompt_text('Custom Audio Filter(s)').strip()
                 audio_filters['Custom'] = custom_audio_filter
 
             else:
                 audio_filters['Exit'] = True
 
         audio_filters_list = []
 
@@ -105,30 +105,56 @@
             f'audio_filters["Fade Out"]["Exp"]: \'{audio_filters["Fade Out"]["Exp"]}\', '
             f'audio_filters["Mute"]["Start Time"]: \'{audio_filters["Mute"]["Start Time"]}\', '
             f'audio_filters["Mute"]["End Time"]: \'{audio_filters["Mute"]["End Time"]}\', '
             f'audio_filters["Custom"]: \'{audio_filters["Custom"]}\''
         )
 
         return ','.join(audio_filters_list)
+    
+    # Prompt the user for our list of video filters
+    def video_filters(encoding_config):
+        video_filters_options = {
+            'scale=-1:720': '720p',
+            'scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp': 'filtered-720p',
+            'hqdn3d=0:0:3:3,gradfun,unsharp': 'filtered',
+            'hqdn3d=0:0:3:3': 'lightdenoise',
+            'hqdn3d=1.5:1.5:6:6': 'heavydenoise',
+            'unsharp': 'unsharp',
+            'Custom': 'custom'
+        }
+
+        question = [inquirer.Checkbox('video_filters', message='Select Video Filters (Space to select)',
+                                      choices=video_filters_options.keys(), default=[tp[1] for tp in encoding_config.video_filters])]
+        answer = inquirer.prompt(question)
+
+        tp_list = [(name, filter_string) for filter_string, name in video_filters_options.items() if filter_string in answer['video_filters']]
 
-    # Prompt custom options if requested
+        if 'Custom' in answer['video_filters']:
+            tp_list.remove(('custom', 'Custom'))
+            custom_video_filters = Interface.prompt_text('Custom Video Filters (Separate with ",," if more than one)').split(',,')
+            tp_list.extend([(f'custom{i + 1}', value) for i, value in enumerate(custom_video_filters)])
+
+        encoding_config.video_filters = tp_list
+
+        logging.debug(f'[Interface.video_filters] tp_list: \'{tp_list}\'')
+
+        return encoding_config
+
+    # Prompt the user for custom options if requested
     def custom_options(encoding_config):
         create_preview = encoding_config.create_preview
         limit_size_enable = encoding_config.limit_size_enable
         crfs = encoding_config.crfs
         encoding_modes = encoding_config.encoding_modes
 
-        validate_crfs = lambda _, x: all(y.strip().isdigit() for y in x.split(','))
-        validate_encoding_modes = lambda _, x: all(y.strip().upper() in ['VBR', 'CBR', 'CQ'] for y in x.split(','))
-
         questions = [
             inquirer.Confirm('create_preview', message=f'Create Preview?', default=create_preview),
             inquirer.Confirm('limit_size_enable', message=f'Limit Size Enable?', default=limit_size_enable),
-            inquirer.Text('crfs', message='CRFs', default=','.join(crfs), validate=validate_crfs),
-            inquirer.Text('encoding_modes', message='Encoding Modes', default=','.join(encoding_modes), validate=validate_encoding_modes)
+            inquirer.Text('crfs', message='CRFs', default=','.join(crfs), validate=Interface.validate_crfs),
+            inquirer.Text('encoding_modes', message='Encoding Modes', default=','.join(encoding_modes), validate=Interface.validate_encoding_modes)
         ]
 
         answer = inquirer.prompt(questions)
 
         encoding_config.create_preview = answer['create_preview']
         encoding_config.limit_size_enable = answer['limit_size_enable']
         encoding_config.crfs = answer['crfs'].split(',')
```

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_loudnorm_filter.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_seek.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_seek_collector.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_seek_collector.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,69 +12,67 @@
     # Time Duration Specification: https://ffmpeg.org/ffmpeg-utils.html#time-duration-syntax
     time_pattern = re.compile('^([0-5]?\d:){1,2}[0-5]?\d(?=\.\d+$|$)|\d+(?=\.\d+$|$)')
 
     # AnimeThemes File Name Convention: '[Title]-{OP|ED}#v#'
     # Examples: Tamayura-OP1, PlanetWith-ED1v2
     filename_pattern = re.compile('^[a-zA-Z0-9\-]+$')
 
-    # List for all output_files
+    # Lists for integrity tests
     all_output_names = []
+    start_positions = 0
+
+    # Validations for our prompts
+    validate_seek = lambda _, x: \
+        len(x.strip()) == 0 \
+        or all(SeekCollector.time_pattern.match(y) for y in x.split(',')) \
+        and SeekCollector.start_positions in [len(x.split(',')), 0]
+
+    validate_output_name = lambda _, x: \
+        len(x.strip()) == 0 \
+        or all(SeekCollector.filename_pattern.match(y) and not y.strip() in SeekCollector.all_output_names for y in x.split(',')) \
+        and SeekCollector.start_positions == len(x.split(',')) \
+        and len(set(x)) == len(x)
 
     def __init__(self, source_file):
         self.source_file = source_file
-        self.start_positions = SeekCollector.prompt_time('Start time(s): ')
-        self.end_positions = SeekCollector.prompt_time('End time(s): ')
+        self.start_positions = SeekCollector.prompt_time('Start time(s)')
+        self.end_positions = SeekCollector.prompt_time('End time(s)')
         self.output_names = SeekCollector.prompt_output_name()
         self.new_audio_filters = SeekCollector.prompt_new_audio_filters(self)
 
     # Prompt the user for our list of starting/ending positions of our WebMs
     # For starting positions, a blank input value is the 0 position of the source file
     # For ending positions, a blank input value is the end position of the source file
     @staticmethod
     def prompt_time(prompt_text):
-        while True:
-            invalid_time = False
-            positions = input(prompt_text).split(',')
-            for position in positions:
-                if len(position) > 0 and not SeekCollector.time_pattern.match(position):
-                    logging.error(f'\'{position}\' is not a valid time duration')
-                    invalid_time = True
-                    break
-            if not invalid_time:
-                return positions
+        positions = Interface.prompt_text(prompt_text, validate=SeekCollector.validate_seek).split(',')
+        if prompt_text == 'Start time(s)':
+            SeekCollector.start_positions = len(positions)
+
+        return positions
 
     # Prompt the user for our list of name for our passlog/WebMs
     @staticmethod
     def prompt_output_name():
-        while True:
-            invalid_name = False
-            filenames = input('Output file name(s): ').split(',')
-            for filename in filenames:
-                if not SeekCollector.filename_pattern.match(filename):
-                    logging.error(f'\'{filename}\' is not a valid output file name')
-                    invalid_name = True
-                    break
-            if not invalid_name:
-                return filenames
+        filenames = Interface.prompt_text(message='Output file name(s)', validate=SeekCollector.validate_output_name).split(',')
+        SeekCollector.all_output_names.extend(filenames)
+        SeekCollector.start_positions = 0
+         
+        return filenames
           
     # Prompt the user for ours list of audio filters of ours WebMs
     @staticmethod
     def prompt_new_audio_filters(self):
         new_audio_filters = []
         for output_name in self.output_names:
             new_audio_filters.append(Interface.audio_filters_options(output_name))
 
-        return new_audio_filters
-
-    # Integrity Test 1: Our lists should be of equal length
-    def is_length_consistent(self):
-        length = len(self.start_positions)
-        return all(len(lst) == length for lst in [self.end_positions, self.output_names])
+        return new_audio_filters       
 
-    # Integrity Test 2: Positions should be within source file duration
+    # Integrity Test 1: Positions should be within source file duration
     def is_within_source_duration(self):
         source_file_duration = float(self.source_file.file_format['format']['duration'])
 
         for start_position, end_position in zip(self.start_positions, self.end_positions):
             start_time = string_to_seconds(start_position) if start_position else 0
             end_time = string_to_seconds(end_position) if end_position else source_file_duration
 
@@ -84,15 +82,15 @@
                 f'source_file_duration: \'{source_file_duration}\'')
 
             if start_time > source_file_duration or end_time > source_file_duration:
                 return False
 
         return True
 
-    # Integrity Test 3: Start position is before end position
+    # Integrity Test 2: Start position is before end position
     def is_start_before_end(self):
         source_file_duration = float(self.source_file.file_format['format']['duration'])
         for start_position, end_position in zip(self.start_positions, self.end_positions):
             start_time = string_to_seconds(start_position) if start_position else 0
             end_time = string_to_seconds(end_position) if end_position else source_file_duration
 
             logging.debug(
@@ -101,64 +99,31 @@
                 f'source_file_duration: \'{source_file_duration}\'')
 
             if start_time >= end_time:
                 return False
 
         return True
 
-    # Integrity Test 4: Unique output names
-    def is_unique_output_names(self):
-        logging.debug(
-            f'[SeekCollector.is_unique_output_names] len(set): \'{len(set(self.output_names))}\', '
-            f'len: \'{len(self.output_names)}\'')
-
-        return len(set(self.output_names)) == len(self.output_names)
-
-    # Integrity Test 5: Unique output names in other source
-    def is_unique_output_names_other_source(self):
-        self.all_output_names.extend(self.output_names)
-
-        logging.debug(
-            f'[SeekCollector.is_unique_output_names_other_source] len(set): \'{len(set(self.all_output_names))}\', '
-            f'len: \'{len(self.all_output_names)}\'')
-        
-        return len(set(self.all_output_names)) == len(self.all_output_names)
-
     # Integrity Tests with feedback
     def is_valid(self):
         is_valid = True
 
-        if not self.is_length_consistent():
-            is_valid = False
-            logging.error('Collection not of equal length')
-
         if not self.is_within_source_duration():
             is_valid = False
             logging.error('Position greater than file duration')
 
         if not self.is_start_before_end():
             is_valid = False
             logging.error('Start Position is not before End Position')
 
-        if not self.is_unique_output_names():
-            is_valid = False
-            logging.error('Output Names are not unique')
-
-        if not self.is_unique_output_names_other_source():
-            is_valid = False
-            logging.error('Output Name is already being used')
-
-        if not is_valid:
-            self.all_output_names.pop()
-
         return is_valid
 
     # Our list of positions, validated if called after is_valid
     def get_seek_list(self):
         seek_list = []
 
         for start_position, end_position, output_name, new_audio_filter in zip(self.start_positions, self.end_positions,
                                                              self.output_names, self.new_audio_filters):
             seek = Seek(self.source_file, start_position, end_position, output_name, new_audio_filter)
             seek_list.append(seek)
 
-        return seek_list
+        return seek_list
```

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_source_file.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_source_file.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_utils.py` & `animethemes-beta-batch-encoder-1.3/beta_batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.2/setup.py` & `animethemes-beta-batch-encoder-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-beta-batch-encoder',
-    version='1.2',
+    version='1.3',
     author='AnimeThemes',
     author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

