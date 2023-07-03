# Comparing `tmp/goxlrutilityapi-1.1.3.dev0.tar.gz` & `tmp/goxlrutilityapi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.1.3.dev0.tar", last modified: Thu May  4 20:40:33 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.2.0.tar", last modified: Mon Jul  3 10:46:19 2023, max compression
```

## Comparing `goxlrutilityapi-1.1.3.dev0.tar` & `goxlrutilityapi-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:40:33.528545 goxlrutilityapi-1.1.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 20:40:33.528545 goxlrutilityapi-1.1.3.dev0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:40:33.524545 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 20:40:31.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:40:33.524545 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:40:33.524545 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:40:33.524545 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:40:33.528545 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:40:33.524545 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 20:40:33.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-04 20:40:33.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:40:33.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 20:40:33.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 20:40:33.000000 goxlrutilityapi-1.1.3.dev0/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 20:40:33.528545 goxlrutilityapi-1.1.3.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 20:40:16.000000 goxlrutilityapi-1.1.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.474359 goxlrutilityapi-1.2.0/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.474359 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.474359 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:46:19.474359 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 10:46:19.000000 goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:46:19.478359 goxlrutilityapi-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 10:46:01.000000 goxlrutilityapi-1.2.0/setup.py
```

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 asyncio.set_event_loop(loop)
 websocket_client = WebsocketClient()
 
 
 def setup_websocket(
     callback: Optional[Callable[[Response[Patch]], Awaitable[None]]] = None
 ) -> bool:
-    """Listen for messages on another thread"""
+    """Listen for messages in the background"""
     try:
         loop.run_until_complete(websocket_client.connect())
         loop.create_task(
             websocket_client.listen(callback),
             name="Websocket Listener",
         )
     except (
@@ -210,14 +210,133 @@
 
     typer.secho(
         f"{button} color set to {color_one} and {color_two}",
         fg=typer.colors.GREEN,
     )
 
 
+@app.command(name="set_volume", short_help="Set Volume of Channel")
+def set_volume(
+    channel: str = typer.Argument(..., help="Channel Name"),
+    volume: int = typer.Argument(..., help="Volume (0-100)"),
+    debug: bool = False,
+) -> None:
+    """Set Volume of Channel"""
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
+            websocket_client.set_volume(
+                channel,
+                volume,
+            )
+        )
+    except BadMessageException as error:
+        typer.secho(
+            f"Failed to set volume: {error}",
+            fg=typer.colors.RED,
+        )
+        return
+
+    typer.secho(
+        f"{channel} volume set to {volume}",
+        fg=typer.colors.GREEN,
+    )
+
+
+@app.command(name="load_profile", short_help="Load Profile")
+def load_profile(
+    profile: str = typer.Argument(..., help="Profile Name"),
+    debug: bool = False,
+) -> None:
+    """Load Profile"""
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
+            websocket_client.load_profile(
+                profile,
+            )
+        )
+    except BadMessageException as error:
+        typer.secho(
+            f"Failed to load profile: {error}",
+            fg=typer.colors.RED,
+        )
+        return
+
+    typer.secho(
+        f"Profile {profile} loaded",
+        fg=typer.colors.GREEN,
+    )
+
+
+@app.command(name="load_profile_colours", short_help="Load Profile Colours")
+def load_profile_colours(
+    profile: str = typer.Argument(..., help="Profile Name"),
+    debug: bool = False,
+) -> None:
+    """Load Profile Colours"""
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
+            websocket_client.load_profile_colours(
+                profile,
+            )
+        )
+    except BadMessageException as error:
+        typer.secho(
+            f"Failed to load profile colours: {error}",
+            fg=typer.colors.RED,
+        )
+        return
+
+    typer.secho(
+        f"Profile colours {profile} loaded",
+        fg=typer.colors.GREEN,
+    )
+
+
 @app.command(name="version", short_help="Module Version")
 def version() -> None:
     """Module Version"""
     typer.secho(__version__.public(), fg=typer.colors.CYAN)
 
 
 if __name__ == "__main__":
```

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/const.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,26 +40,29 @@
 RESPONSE_TYPE_ERROR: Final[str] = "Error"
 RESPONSE_TYPE_HTTP_STATE: Final[str] = "HttpState"
 RESPONSE_TYPE_OK: Final[str] = "Ok"
 RESPONSE_TYPE_PATCH: Final[str] = "Patch"
 RESPONSE_TYPE_STATUS: Final[str] = "Status"
 
 # Command Types (https://github.com/GoXLR-on-Linux/goxlr-utility/blob/c2c876dd83ddcd4681b1a674c5cb975796726dd8/ipc/src/lib.rs#LL65C17-L65C17)
+COMMAND_TYPE_LOAD_PROFILE_COLOURS: Final[str] = "LoadProfileColours"
+COMMAND_TYPE_LOAD_PROFILE: Final[str] = "LoadProfile"
 COMMAND_TYPE_SET_ALL_FADER_COLOURS: Final[str] = "SetAllFaderColours"
 COMMAND_TYPE_SET_ALL_FADER_DISPLAY_STYLE: Final[str] = "SetAllFaderDisplayStyle"
 COMMAND_TYPE_SET_BUTTON_COLOURS: Final[str] = "SetButtonColours"
 COMMAND_TYPE_SET_BUTTON_GROUP_COLOURS: Final[str] = "SetButtonGroupColours"
 COMMAND_TYPE_SET_BUTTON_GROUP_OFF_STYLE: Final[str] = "SetButtonGroupOffStyle"
 COMMAND_TYPE_SET_BUTTON_OFF_STYLE: Final[str] = "SetButtonOffStyle"
 COMMAND_TYPE_SET_ENCODER_COLOUR: Final[str] = "SetEncoderColour"
 COMMAND_TYPE_SET_FADER_COLOURS: Final[str] = "SetFaderColours"
 COMMAND_TYPE_SET_FADER_DISPLAY_STYLE: Final[str] = "SetFaderDisplayStyle"
 COMMAND_TYPE_SET_SAMPLE_COLOUR: Final[str] = "SetSampleColour"
 COMMAND_TYPE_SET_SAMPLE_OFF_STYLE: Final[str] = "SetSampleOffStyle"
 COMMAND_TYPE_SET_SIMPLE_COLOUR: Final[str] = "SetSimpleColour"
+COMMAND_TYPE_SET_VOLUME: Final[str] = "SetVolume"
 
 # Buttons
 BUTTON_BLEEP: Final[str] = "Bleep"
 BUTTON_COUGH: Final[str] = "Cough"
 BUTTON_EFFECT_FX: Final[str] = "EffectFx"
 BUTTON_EFFECT_HARD_TUNE: Final[str] = "EffectHardTune"
 BUTTON_EFFECT_MEGAPHONE: Final[str] = "EffectMegaphone"
```

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/__init__.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/__init__.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/map_item.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/map_item.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/patch.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/patch.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/request.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/request.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/helpers/tests/models/response.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/helpers/tests/models/response.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/models/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 class Config(DefaultBaseModel):
     """Config Model"""
 
     daemon_version: Optional[str] = Field(None)
     autostart_enabled: Optional[bool] = Field(None)
     show_tray_icon: Optional[bool] = Field(None)
     tts_enabled: Optional[bool] = Field(None)
+    allow_network_access: Optional[bool] = Field(None)
+    log_level: Optional[str] = Field(None)
 
 
 class Versions(DefaultBaseModel):
     """Versions Model"""
 
     firmware: Optional[list[int]] = Field(None)
     fpga_count: Optional[int] = Field(None)
@@ -184,15 +186,16 @@
     mic_monitor: int = Field(..., alias="MicMonitor")
     line_out: int = Field(..., alias="LineOut")
 
 
 class Levels(DefaultBaseModel):
     """Levels Model"""
 
-    submix_supported: Optional[bool] = Field(None)
+    submix_supported: bool = Field(None)
+    output_monitor: str
     volumes: Volumes
     submix: Optional[Any] = Field(None)
     bleep: Optional[int] = Field(None)
     deess: Optional[int] = Field(None)
 
 
 class RouterItem(DefaultBaseModel):
@@ -236,14 +239,24 @@
 class Fader(DefaultBaseModel):
     """Fader Model"""
 
     style: Optional[str] = Field(None)
     colours: Colours = Field(None)
 
 
+class Animation(DefaultBaseModel):
+    """Animation Model"""
+
+    supported: Optional[bool] = Field(None)
+    mode: Optional[str] = Field(None)
+    mod1: Optional[int] = Field(None)
+    mod2: Optional[int] = Field(None)
+    waterfall_direction: Optional[str] = Field(None)
+
+
 class Faders(DefaultBaseModel):
     """Faders Model"""
 
     a: Fader = Field(..., alias="A")
     b: Fader = Field(..., alias="B")
     c: Fader = Field(..., alias="C")
     d: Fader = Field(..., alias="D")
@@ -285,14 +298,15 @@
     global_: Optional[Global] = Field(None, alias="Global")
     accent: Accent = Field(None, alias="Accent")
 
 
 class Lighting(DefaultBaseModel):
     """Lighting Model"""
 
+    animation: Animation
     faders: Faders
     buttons: Buttons
     simple: Simple
     sampler: Optional[dict[str, Any]]
     encoders: Optional[dict[str, Any]]
 
 
@@ -370,19 +384,19 @@
     presets_directory: Optional[str]
     icons_directory: Optional[str]
 
 
 class Files(DefaultBaseModel):
     """Files Model"""
 
-    profiles: Optional[list[str]]
-    mic_profiles: Optional[list[str]]
-    presets: Optional[list[str]]
-    samples: Optional[dict[str, Any]]
-    icons: Optional[list[str]]
+    profiles: list[str]
+    mic_profiles: list[str]
+    presets: list[str]
+    samples: dict[str, Any]
+    icons: list[str]
 
 
 class Status(DefaultBaseModel):
     """Status Model"""
 
     config: Config
     mixers: dict[str, Mixer]
```

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.2.0/goxlrutilityapi/websocket_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 import aiohttp
 import async_timeout
 from pydantic import ValidationError
 
 from .base import Base
 from .const import (
     ACCENT,
+    COMMAND_TYPE_LOAD_PROFILE,
+    COMMAND_TYPE_LOAD_PROFILE_COLOURS,
     COMMAND_TYPE_SET_BUTTON_COLOURS,
     COMMAND_TYPE_SET_FADER_COLOURS,
     COMMAND_TYPE_SET_SIMPLE_COLOUR,
+    COMMAND_TYPE_SET_VOLUME,
     DEFAULT_HOST,
     DEFAULT_PORT,
     KEY_DATA,
     KEY_ID,
     KEY_TYPE,
     MODEL_MAP,
     REQUEST_TYPE_COMMAND,
@@ -243,14 +246,112 @@
                         },
                     ]
                 }
             ),
             wait_for_response=False,
             response_type=RESPONSE_TYPE_OK,
         )
+
+    async def set_volume(
+        self,
+        channel: str,
+        volume: int,
+    ) -> None:
+        """Set volume of channel"""
+        if self._mixer_serial_number is None:
+            raise BadMessageException(
+                "Mixer serial number is missing. Call get_status to set this."
+            )
+
+        self._logger.info(
+            "Setting volume of '%s' to '%s' for mixer '%s'",
+            channel,
+            volume,
+            self._mixer_serial_number,
+        )
+        await self._send_message(
+            Request(
+                data={
+                    REQUEST_TYPE_COMMAND: [
+                        self._mixer_serial_number,
+                        {
+                            COMMAND_TYPE_SET_VOLUME: [
+                                channel,
+                                volume,
+                            ],
+                        },
+                    ]
+                }
+            ),
+            wait_for_response=False,
+            response_type=RESPONSE_TYPE_OK,
+        )
+
+    async def load_profile(
+        self,
+        profile: str,
+    ) -> None:
+        """Load profile"""
+        if self._mixer_serial_number is None:
+            raise BadMessageException(
+                "Mixer serial number is missing. Call get_status to set this."
+            )
+
+        self._logger.info(
+            "Loading profile '%s' for mixer '%s'",
+            profile,
+            self._mixer_serial_number,
+        )
+        await self._send_message(
+            Request(
+                data={
+                    REQUEST_TYPE_COMMAND: [
+                        self._mixer_serial_number,
+                        {
+                            COMMAND_TYPE_LOAD_PROFILE: [
+                                profile,
+                                False,
+                            ],
+                        },
+                    ]
+                }
+            ),
+            wait_for_response=False,
+            response_type=RESPONSE_TYPE_OK,
+        )
+
+    async def load_profile_colours(
+        self,
+        profile: str,
+    ) -> None:
+        """Load profile colours"""
+        if self._mixer_serial_number is None:
+            raise BadMessageException(
+                "Mixer serial number is missing. Call get_status to set this."
+            )
+
+        self._logger.info(
+            "Loading profile colours '%s' for mixer '%s'",
+            profile,
+            self._mixer_serial_number,
+        )
+        await self._send_message(
+            Request(
+                data={
+                    REQUEST_TYPE_COMMAND: [
+                        self._mixer_serial_number,
+                        {
+                            COMMAND_TYPE_LOAD_PROFILE_COLOURS: profile,
+                        },
+                    ]
+                }
+            ),
+            wait_for_response=False,
+            response_type=RESPONSE_TYPE_OK,
+        )
 
     async def listen(
         self,
         patch_callback: Optional[Callable[[Response[Patch]], Awaitable[None]]] = None,
     ) -> None:
         """Listen for patches from GoXLR"""
```

### Comparing `goxlrutilityapi-1.1.3.dev0/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.2.0/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.3.dev0/pyproject.toml` & `goxlrutilityapi-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.3.dev0/setup.py` & `goxlrutilityapi-1.2.0/setup.py`

 * *Files identical despite different names*

