# Comparing `tmp/goxlrutilityapi-1.2.0.tar.gz` & `tmp/goxlrutilityapi-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.2.0.tar", last modified: Mon Jul  3 10:46:19 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.2.1.tar", last modified: Mon Jul  3 14:59:55 2023, max compression
```

## Comparing `goxlrutilityapi-1.2.0.tar` & `goxlrutilityapi-1.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.474359 goxlrutilityapi-1.2.0/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.474359 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.474359 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.474359 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.695217 goxlrutilityapi-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 14:59:55.695217 goxlrutilityapi-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.695217 goxlrutilityapi-1.2.1/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:59:55.691217 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 14:59:55.000000 goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:59:55.695217 goxlrutilityapi-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 14:59:40.000000 goxlrutilityapi-1.2.1/setup.py
```

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,55 @@
 
     typer.secho(
         f"{button} color set to {color_one} and {color_two}",
         fg=typer.colors.GREEN,
     )
 
 
+@app.command(name="set_muted", short_help="Set Muted of Channel")
+def set_muted(
+    channel: str = typer.Argument(..., help="Channel Name"),
+    muted: bool = typer.Argument(..., help="Muted (True/False)"),
+    debug: bool = False,
+) -> None:
+    """Set Muted of Channel"""
+    if debug:
+        setup_logger("DEBUG")
+    if setup_websocket() is False:
+        typer.secho("Failed to connect to GoXLR", fg=typer.colors.RED)
+        return
+    try:
+        loop.run_until_complete(websocket_client.get_status())
+    except BadMessageException as error:
+        typer.secho(
+            f"Failed to get status from GoXLR: {error}",
+            fg=typer.colors.RED,
+        )
+        return
+
+    try:
+        loop.run_until_complete(
+            websocket_client.set_muted(
+                channel,
+                muted,
+            )
+        )
+    except BadMessageException as error:
+        typer.secho(
+            f"Failed to set muted: {error}",
+            fg=typer.colors.RED,
+        )
+        return
+
+    typer.secho(
+        f"{channel} muted set to {muted}",
+        fg=typer.colors.GREEN,
+    )
+
+
 @app.command(name="set_volume", short_help="Set Volume of Channel")
 def set_volume(
     channel: str = typer.Argument(..., help="Channel Name"),
     volume: int = typer.Argument(..., help="Volume (0-100)"),
     debug: bool = False,
 ) -> None:
     """Set Volume of Channel"""
```

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/const.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 COMMAND_TYPE_SET_BUTTON_COLOURS: Final[str] = "SetButtonColours"
 COMMAND_TYPE_SET_BUTTON_GROUP_COLOURS: Final[str] = "SetButtonGroupColours"
 COMMAND_TYPE_SET_BUTTON_GROUP_OFF_STYLE: Final[str] = "SetButtonGroupOffStyle"
 COMMAND_TYPE_SET_BUTTON_OFF_STYLE: Final[str] = "SetButtonOffStyle"
 COMMAND_TYPE_SET_ENCODER_COLOUR: Final[str] = "SetEncoderColour"
 COMMAND_TYPE_SET_FADER_COLOURS: Final[str] = "SetFaderColours"
 COMMAND_TYPE_SET_FADER_DISPLAY_STYLE: Final[str] = "SetFaderDisplayStyle"
+COMMAND_TYPE_SET_MUTE_STATE: Final[str] = "SetFaderMuteState"
 COMMAND_TYPE_SET_SAMPLE_COLOUR: Final[str] = "SetSampleColour"
 COMMAND_TYPE_SET_SAMPLE_OFF_STYLE: Final[str] = "SetSampleOffStyle"
 COMMAND_TYPE_SET_SIMPLE_COLOUR: Final[str] = "SetSimpleColour"
 COMMAND_TYPE_SET_VOLUME: Final[str] = "SetVolume"
 
 # Buttons
 BUTTON_BLEEP: Final[str] = "Bleep"
```

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/__init__.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/__init__.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/map_item.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/map_item.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/patch.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/patch.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/request.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/request.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/response.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/response.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/status.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/helpers/tests/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.2.1/goxlrutilityapi/websocket_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 from .base import Base
 from .const import (
     ACCENT,
     COMMAND_TYPE_LOAD_PROFILE,
     COMMAND_TYPE_LOAD_PROFILE_COLOURS,
     COMMAND_TYPE_SET_BUTTON_COLOURS,
     COMMAND_TYPE_SET_FADER_COLOURS,
+    COMMAND_TYPE_SET_MUTE_STATE,
     COMMAND_TYPE_SET_SIMPLE_COLOUR,
     COMMAND_TYPE_SET_VOLUME,
     DEFAULT_HOST,
     DEFAULT_PORT,
     KEY_DATA,
     KEY_ID,
     KEY_TYPE,
     MODEL_MAP,
+    MUTED_STATE,
     REQUEST_TYPE_COMMAND,
     REQUEST_TYPE_GET_STATUS,
     RESPONSE_TYPE_OK,
     RESPONSE_TYPE_PATCH,
     RESPONSE_TYPE_STATUS,
+    UNMUTED_STATE,
 )
 from .exceptions import (
     BadMessageException,
     ConnectionClosedException,
     ConnectionErrorException,
 )
 from .models.patch import Patch
@@ -245,14 +248,49 @@
                             ],
                         },
                     ]
                 }
             ),
             wait_for_response=False,
             response_type=RESPONSE_TYPE_OK,
+        )
+
+    async def set_muted(
+        self,
+        channel: str,
+        muted: bool,
+    ) -> None:
+        """Set muted state of channel"""
+        if self._mixer_serial_number is None:
+            raise BadMessageException(
+                "Mixer serial number is missing. Call get_status to set this."
+            )
+
+        self._logger.info(
+            "Setting muted state of '%s' to '%s' for mixer '%s'",
+            channel,
+            muted,
+            self._mixer_serial_number,
+        )
+        await self._send_message(
+            Request(
+                data={
+                    REQUEST_TYPE_COMMAND: [
+                        self._mixer_serial_number,
+                        {
+                            COMMAND_TYPE_SET_MUTE_STATE: [
+                                channel,
+                                MUTED_STATE if muted else UNMUTED_STATE,
+                            ],
+                        },
+                    ]
+                }
+            ),
+            wait_for_response=False,
+            response_type=RESPONSE_TYPE_OK,
         )
 
     async def set_volume(
         self,
         channel: str,
         volume: int,
     ) -> None:
```

### Comparing `goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.2.1/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/pyproject.toml` & `goxlrutilityapi-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.2.0/setup.py` & `goxlrutilityapi-1.2.1/setup.py`

 * *Files identical despite different names*

