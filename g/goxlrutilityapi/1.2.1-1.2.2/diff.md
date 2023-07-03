# Comparing `tmp/goxlrutilityapi-1.2.1.tar.gz` & `tmp/goxlrutilityapi-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.2.1.tar", last modified: Mon Jul  3 14:59:55 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.2.2.tar", last modified: Mon Jul  3 15:32:28 2023, max compression
```

## Comparing `goxlrutilityapi-1.2.1.tar` & `goxlrutilityapi-1.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.695217 goxlrutilityapi-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 14:59:55.695217 goxlrutilityapi-1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.695217 goxlrutilityapi-1.2.1/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:59:55.695217 goxlrutilityapi-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:32:28.947908 goxlrutilityapi-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 15:32:28.947908 goxlrutilityapi-1.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:32:28.943908 goxlrutilityapi-1.2.2/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:32:28.943908 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:32:28.943908 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:32:28.943908 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:32:28.947908 goxlrutilityapi-1.2.2/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:32:28.943908 goxlrutilityapi-1.2.2/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 15:32:28.000000 goxlrutilityapi-1.2.2/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 15:32:28.000000 goxlrutilityapi-1.2.2/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:32:28.000000 goxlrutilityapi-1.2.2/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 15:32:28.000000 goxlrutilityapi-1.2.2/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 15:32:28.000000 goxlrutilityapi-1.2.2/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:32:28.947908 goxlrutilityapi-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 15:32:12.000000 goxlrutilityapi-1.2.2/setup.py
```

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/const.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/const.py`

 * *Files 21% similar despite different names*

```diff
@@ -132,80 +132,170 @@
     "sampler_select_b": BUTTON_SAMPLER_SELECT_B,
     "sampler_select_c": BUTTON_SAMPLER_SELECT_C,
     "sampler_top_left": BUTTON_SAMPLER_TOP_LEFT,
     "sampler_top_right": BUTTON_SAMPLER_TOP_RIGHT,
 }
 
 NAME_MAP: Final[dict[str, MapItem]] = {
-    "a": MapItem(name="Fader 1", icon="mdi:tune-vertical-variant"),
-    "A": MapItem(name="Fader 1", icon="mdi:tune-vertical-variant"),
-    "b": MapItem(name="Fader 2", icon="mdi:tune-vertical-variant"),
-    "B": MapItem(name="Fader 2", icon="mdi:tune-vertical-variant"),
-    "bleep": MapItem(name=BUTTON_BLEEP, icon="mdi:exclamation"),
-    "c": MapItem(name="Fader 3", icon="mdi:tune-vertical-variant"),
-    "C": MapItem(name="Fader 3", icon="mdi:tune-vertical-variant"),
-    "chat": MapItem(name="Chat", icon="mdi:chat"),
-    "console": MapItem(name="Console", icon="mdi:gamepad-variant"),
-    "cough": MapItem(name=BUTTON_COUGH, icon="mdi:microphone-off"),
-    "d": MapItem(name="Fader 4", icon="mdi:tune-vertical-variant"),
-    "D": MapItem(name="Fader 4", icon="mdi:tune-vertical-variant"),
-    "effect_fx": MapItem(name="Effect FX", icon="mdi:equalizer-outline"),
-    "effect_hard_tune": MapItem(name="Effect Hard Tune", icon="mdi:knob"),
-    "effect_megaphone": MapItem(name="Effect Megaphone", icon="mdi:bullhorn-outline"),
-    "effect_robot": MapItem(name="Effect Robot", icon="mdi:robot-outline"),
-    "effect_select_1": MapItem(name="Effect Select 1", icon="mdi:sawtooth-wave"),
-    "effect_select_2": MapItem(name="Effect Select 2", icon="mdi:sawtooth-wave"),
-    "effect_select_3": MapItem(name="Effect Select 3", icon="mdi:sawtooth-wave"),
-    "effect_select_4": MapItem(name="Effect Select 4", icon="mdi:sawtooth-wave"),
-    "effect_select_5": MapItem(name="Effect Select 5", icon="mdi:sawtooth-wave"),
-    "effect_select_6": MapItem(name="Effect Select 6", icon="mdi:sawtooth-wave"),
-    "effect_select1": MapItem(name="Effect Select 1", icon="mdi:sawtooth-wave"),
-    "effect_select2": MapItem(name="Effect Select 2", icon="mdi:sawtooth-wave"),
-    "effect_select3": MapItem(name="Effect Select 3", icon="mdi:sawtooth-wave"),
-    "effect_select4": MapItem(name="Effect Select 4", icon="mdi:sawtooth-wave"),
-    "effect_select5": MapItem(name="Effect Select 5", icon="mdi:sawtooth-wave"),
-    "effect_select6": MapItem(name="Effect Select 6", icon="mdi:sawtooth-wave"),
-    "fader_1_mute": MapItem(name="Fader 1 Mute", icon="mdi:microphone-off"),
-    "fader_1": MapItem(name="Fader 1", icon="mdi:volume-high"),
-    "fader_2_mute": MapItem(name="Fader 2 Mute", icon="mdi:microphone-off"),
-    "fader_2": MapItem(name="Fader 2", icon="mdi:volume-high"),
-    "fader_3_mute": MapItem(name="Fader 3 Mute", icon="mdi:microphone-off"),
-    "fader_3": MapItem(name="Fader 3", icon="mdi:volume-high"),
-    "fader_4_mute": MapItem(name="Fader 4 Mute", icon="mdi:microphone-off"),
-    "fader_4": MapItem(name="Fader 4", icon="mdi:volume-high"),
-    "fader1_mute": MapItem(name="Fader 1 Mute", icon="mdi:microphone-off"),
-    "fader2_mute": MapItem(name="Fader 2 Mute", icon="mdi:microphone-off"),
-    "fader3_mute": MapItem(name="Fader 3 Mute", icon="mdi:microphone-off"),
-    "fader4_mute": MapItem(name="Fader 4 Mute", icon="mdi:microphone-off"),
-    "headphones": MapItem(name="Headphones", icon="mdi:headphones"),
-    "line_in": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
-    "line_out": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
-    "LineIn": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
-    "LineOut": MapItem(name="Line In", icon="mdi:audio-input-stereo-minijack"),
-    "mic_monitor": MapItem(name="Microphone Monitor", icon="mdi:microphone-outline"),
-    "mic": MapItem(name="Microphone", icon="mdi:microphone"),
-    "Mic": MapItem(name="Microphone", icon="mdi:microphone"),
-    "MicMonitor": MapItem(name="Microphone Monitor", icon="mdi:microphone-outline"),
-    "music": MapItem(name="Music", icon="mdi:music"),
-    "Music": MapItem(name="Music", icon="mdi:music"),
-    "mute_all": MapItem(name="Mute All", icon="mdi:microphone-off"),
-    "mute_chat": MapItem(name="Mute Chat", icon="mdi:microphone-off"),
-    "mute_console": MapItem(name="Mute Console", icon="mdi:microphone-off"),
-    "mute_line_in": MapItem(name="Mute Line In", icon="mdi:microphone-off"),
-    "mute_line_out": MapItem(name="Mute Line Out", icon="mdi:microphone-off"),
-    "mute_mic": MapItem(name="Mute Microphone", icon="mdi:microphone-off"),
-    "mute_microphone": MapItem(name="Mute Microphone", icon="mdi:microphone-off"),
-    "mute_music": MapItem(name="Mute Music", icon="mdi:microphone-off"),
-    "mute_system": MapItem(name="Mute System", icon="mdi:microphone-off"),
-    "mute": MapItem(name="Mute", icon="mdi:microphone-off"),
-    "sample": MapItem(name="Sample", icon="mdi:music-note"),
-    "sampler_bottom_left": MapItem(name="Sampler Bottom Left", icon="mdi:music-note"),
-    "sampler_bottom_right": MapItem(name="Sampler Bottom Right", icon="mdi:music-note"),
-    "sampler_clear": MapItem(name="Sampler Clear", icon="mdi:music-note"),
-    "sampler_select_a": MapItem(name="Sampler Select A", icon="mdi:music-note"),
-    "sampler_select_b": MapItem(name="Sampler Select B", icon="mdi:music-note"),
-    "sampler_select_c": MapItem(name="Sampler Select C", icon="mdi:music-note"),
-    "sampler_top_left": MapItem(name="Sampler Top Left", icon="mdi:music-note"),
-    "sampler_top_right": MapItem(name="Sampler Top Right", icon="mdi:music-note"),
-    "system": MapItem(name="System", icon="mdi:music-box-outline"),
-    "System": MapItem(name="System", icon="mdi:music-box-outline"),
+    "a": MapItem(key="A", name="Fader 1", icon="mdi:tune-vertical-variant"),
+    "A": MapItem(key="A", name="Fader 1", icon="mdi:tune-vertical-variant"),
+    "b": MapItem(key="B", name="Fader 2", icon="mdi:tune-vertical-variant"),
+    "B": MapItem(key="B", name="Fader 2", icon="mdi:tune-vertical-variant"),
+    "bleep": MapItem(key="Bleep", name=BUTTON_BLEEP, icon="mdi:exclamation"),
+    "c": MapItem(key="C", name="Fader 3", icon="mdi:tune-vertical-variant"),
+    "C": MapItem(key="C", name="Fader 3", icon="mdi:tune-vertical-variant"),
+    "chat": MapItem(key="Chat", name="Chat", icon="mdi:chat"),
+    "console": MapItem(key="Console", name="Console", icon="mdi:gamepad-variant"),
+    "cough": MapItem(key="Cough", name=BUTTON_COUGH, icon="mdi:microphone-off"),
+    "d": MapItem(key="D", name="Fader 4", icon="mdi:tune-vertical-variant"),
+    "D": MapItem(key="D", name="Fader 4", icon="mdi:tune-vertical-variant"),
+    "effect_fx": MapItem(
+        key="effect_fx", name="Effect FX", icon="mdi:equalizer-outline"
+    ),
+    "effect_hard_tune": MapItem(
+        key="effect_hard_tune", name="Effect Hard Tune", icon="mdi:knob"
+    ),
+    "effect_megaphone": MapItem(
+        key="effect_megaphone", name="Effect Megaphone", icon="mdi:bullhorn-outline"
+    ),
+    "effect_robot": MapItem(
+        key="effect_robot", name="Effect Robot", icon="mdi:robot-outline"
+    ),
+    "effect_select_1": MapItem(
+        key="effect_select_1", name="Effect Select 1", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select_2": MapItem(
+        key="effect_select_2", name="Effect Select 2", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select_3": MapItem(
+        key="effect_select_3", name="Effect Select 3", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select_4": MapItem(
+        key="effect_select_4", name="Effect Select 4", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select_5": MapItem(
+        key="effect_select_5", name="Effect Select 5", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select_6": MapItem(
+        key="effect_select_6", name="Effect Select 6", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select1": MapItem(
+        key="effect_select1", name="Effect Select 1", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select2": MapItem(
+        key="effect_select2", name="Effect Select 2", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select3": MapItem(
+        key="effect_select3", name="Effect Select 3", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select4": MapItem(
+        key="effect_select4", name="Effect Select 4", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select5": MapItem(
+        key="effect_select5", name="Effect Select 5", icon="mdi:sawtooth-wave"
+    ),
+    "effect_select6": MapItem(
+        key="effect_select6", name="Effect Select 6", icon="mdi:sawtooth-wave"
+    ),
+    "fader_1_mute": MapItem(
+        key="fader_1_mute", name="Fader 1 Mute", icon="mdi:microphone-off"
+    ),
+    "fader_1": MapItem(key="fader_1", name="Fader 1", icon="mdi:volume-high"),
+    "fader_2_mute": MapItem(
+        key="fader_2_mute", name="Fader 2 Mute", icon="mdi:microphone-off"
+    ),
+    "fader_2": MapItem(key="fader_2", name="Fader 2", icon="mdi:volume-high"),
+    "fader_3_mute": MapItem(
+        key="fader_3_mute", name="Fader 3 Mute", icon="mdi:microphone-off"
+    ),
+    "fader_3": MapItem(key="fader_3", name="Fader 3", icon="mdi:volume-high"),
+    "fader_4_mute": MapItem(
+        key="fader_4_mute", name="Fader 4 Mute", icon="mdi:microphone-off"
+    ),
+    "fader_4": MapItem(key="fader_4", name="Fader 4", icon="mdi:volume-high"),
+    "fader1_mute": MapItem(
+        key="fader1_mute", name="Fader 1 Mute", icon="mdi:microphone-off"
+    ),
+    "fader2_mute": MapItem(
+        key="fader2_mute", name="Fader 2 Mute", icon="mdi:microphone-off"
+    ),
+    "fader3_mute": MapItem(
+        key="fader3_mute", name="Fader 3 Mute", icon="mdi:microphone-off"
+    ),
+    "fader4_mute": MapItem(
+        key="fader4_mute", name="Fader 4 Mute", icon="mdi:microphone-off"
+    ),
+    "headphones": MapItem(key="Headphones", name="Headphones", icon="mdi:headphones"),
+    "line_in": MapItem(
+        key="LineIn", name="Line In", icon="mdi:audio-input-stereo-minijack"
+    ),
+    "line_out": MapItem(
+        key="LineOut", name="Line In", icon="mdi:audio-input-stereo-minijack"
+    ),
+    "LineIn": MapItem(
+        key="LineIn", name="Line In", icon="mdi:audio-input-stereo-minijack"
+    ),
+    "LineOut": MapItem(
+        key="LineOut", name="Line In", icon="mdi:audio-input-stereo-minijack"
+    ),
+    "mic_monitor": MapItem(
+        key="MicMonitor", name="Microphone Monitor", icon="mdi:microphone-outline"
+    ),
+    "mic": MapItem(key="Mic", name="Microphone", icon="mdi:microphone"),
+    "Mic": MapItem(key="Mic", name="Microphone", icon="mdi:microphone"),
+    "MicMonitor": MapItem(
+        key="MicMonitor", name="Microphone Monitor", icon="mdi:microphone-outline"
+    ),
+    "music": MapItem(key="Music", name="Music", icon="mdi:music"),
+    "Music": MapItem(key="Music", name="Music", icon="mdi:music"),
+    "mute_all": MapItem(key="mute_all", name="Mute All", icon="mdi:microphone-off"),
+    "mute_chat": MapItem(key="mute_chat", name="Mute Chat", icon="mdi:microphone-off"),
+    "mute_console": MapItem(
+        key="mute_console", name="Mute Console", icon="mdi:microphone-off"
+    ),
+    "mute_line_in": MapItem(
+        key="mute_line_in", name="Mute Line In", icon="mdi:microphone-off"
+    ),
+    "mute_line_out": MapItem(
+        key="mute_line_out", name="Mute Line Out", icon="mdi:microphone-off"
+    ),
+    "mute_mic": MapItem(
+        key="mute_mic", name="Mute Microphone", icon="mdi:microphone-off"
+    ),
+    "mute_microphone": MapItem(
+        key="mute_microphone", name="Mute Microphone", icon="mdi:microphone-off"
+    ),
+    "mute_music": MapItem(
+        key="mute_music", name="Mute Music", icon="mdi:microphone-off"
+    ),
+    "mute_system": MapItem(
+        key="mute_system", name="Mute System", icon="mdi:microphone-off"
+    ),
+    "mute": MapItem(key="Mute", name="Mute", icon="mdi:microphone-off"),
+    "sample": MapItem(key="Sample", name="Sample", icon="mdi:music-note"),
+    "sampler_bottom_left": MapItem(
+        key="sampler_bottom_left", name="Sampler Bottom Left", icon="mdi:music-note"
+    ),
+    "sampler_bottom_right": MapItem(
+        key="sampler_bottom_right", name="Sampler Bottom Right", icon="mdi:music-note"
+    ),
+    "sampler_clear": MapItem(
+        key="sampler_clear", name="Sampler Clear", icon="mdi:music-note"
+    ),
+    "sampler_select_a": MapItem(
+        key="sampler_select_a", name="Sampler Select A", icon="mdi:music-note"
+    ),
+    "sampler_select_b": MapItem(
+        key="sampler_select_b", name="Sampler Select B", icon="mdi:music-note"
+    ),
+    "sampler_select_c": MapItem(
+        key="sampler_select_c", name="Sampler Select C", icon="mdi:music-note"
+    ),
+    "sampler_top_left": MapItem(
+        key="sampler_top_left", name="Sampler Top Left", icon="mdi:music-note"
+    ),
+    "sampler_top_right": MapItem(
+        key="sampler_top_right", name="Sampler Top Right", icon="mdi:music-note"
+    ),
+    "system": MapItem(key="System", name="System", icon="mdi:music-box-outline"),
+    "System": MapItem(key="System", name="System", icon="mdi:music-box-outline"),
 }
```

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/__init__.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/__init__.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/map_item.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/map_item.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/patch.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/patch.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/request.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/request.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/response.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/response.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/status.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/helpers/tests/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.2.2/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.2.2/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/pyproject.toml` & `goxlrutilityapi-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.1/setup.py` & `goxlrutilityapi-1.2.2/setup.py`

 * *Files identical despite different names*

