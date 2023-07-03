# Comparing `tmp/interaction-devkit-0.1.4.tar.gz` & `tmp/interaction-devkit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interaction-devkit-0.1.4.tar", last modified: Sun Jul  2 09:36:04 2023, max compression
+gzip compressed data, was "interaction-devkit-0.1.6.tar", last modified: Mon Jul  3 08:01:20 2023, max compression
```

## Comparing `interaction-devkit-0.1.4.tar` & `interaction-devkit-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.444399 interaction-devkit-0.1.4/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.444399 interaction-devkit-0.1.4/interaction/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32670 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/map_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.444399 interaction-devkit-0.1.4/interaction/dataset/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/speed_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/track_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/interaction/dataset/tracks/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/tracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20488 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/tracks/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/tracks/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/interaction_devkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/test_map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/test_map_components.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/test_track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/test_track_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:20.403439 interaction-devkit-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-03 08:01:20.403439 interaction-devkit-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:20.403439 interaction-devkit-0.1.6/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:20.403439 interaction-devkit-0.1.6/interaction/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32670 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/map_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:20.403439 interaction-devkit-0.1.6/interaction/dataset/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/maps/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/maps/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/maps/speed_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/maps/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/maps/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/track_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:20.403439 interaction-devkit-0.1.6/interaction/dataset/tracks/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/tracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21881 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/tracks/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/tracks/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/interaction/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:20.403439 interaction-devkit-0.1.6/interaction_devkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-03 08:01:20.000000 interaction-devkit-0.1.6/interaction_devkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-03 08:01:20.000000 interaction-devkit-0.1.6/interaction_devkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:01:20.000000 interaction-devkit-0.1.6/interaction_devkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 08:01:20.000000 interaction-devkit-0.1.6/interaction_devkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 08:01:20.000000 interaction-devkit-0.1.6/interaction_devkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 08:01:20.407439 interaction-devkit-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:20.403439 interaction-devkit-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/tests/test_map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/tests/test_map_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/tests/test_track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-03 08:01:12.000000 interaction-devkit-0.1.6/tests/test_track_components.py
```

### Comparing `interaction-devkit-0.1.4/LICENSE` & `interaction-devkit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/PKG-INFO` & `interaction-devkit-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interaction-devkit
-Version: 0.1.4
+Version: 0.1.6
 Summary: A toolkit for building interactive applications.
 Author-email: Juanwu Lu <juanwu@purdue.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Juanwu Lu
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `interaction-devkit-0.1.4/README.md` & `interaction-devkit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/__init__.py` & `interaction-devkit-0.1.6/interaction/__init__.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/__init__.py` & `interaction-devkit-0.1.6/interaction/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/map_api.py` & `interaction-devkit-0.1.6/interaction/dataset/map_api.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/maps/__init__.py` & `interaction-devkit-0.1.6/interaction/dataset/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/maps/elements.py` & `interaction-devkit-0.1.6/interaction/dataset/maps/elements.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/maps/projector.py` & `interaction-devkit-0.1.6/interaction/dataset/maps/projector.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/maps/speed_limit.py` & `interaction-devkit-0.1.6/interaction/dataset/maps/speed_limit.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/maps/typing.py` & `interaction-devkit-0.1.6/interaction/dataset/maps/typing.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/maps/utils.py` & `interaction-devkit-0.1.6/interaction/dataset/maps/utils.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/track_api.py` & `interaction-devkit-0.1.6/interaction/dataset/track_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,29 @@
 """
 # Copyright (c) 2023, Juanwu Lu <juanwu@purdue.edu>.
 # Released under the BSD-3-Clause license.
 # See https://opensource.org/license/bsd-3-clause/ for licensing details.
 from collections import defaultdict
 from enum import IntEnum
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional
 
 import geopandas as gpd
 import matplotlib.pyplot as plt
 import pandas as pd
 
 from .tracks.container import (
     MOTION_STATE_FIELD_MAPPING,
     INTERACTIONCase,
     MotionState,
     Track,
+    TrackFrame,
 )
 from .tracks.typing import AgentType
 
-# type aliases
-TrackFrame = Union[gpd.GeoDataFrame, pd.DataFrame]
-
 
 class INTERACTIONScenarioLayers(IntEnum):
     """Enum for the layers in the INTERACTION scenario track data."""
 
     MOTION_STATE = 0
     """Data layer of all the agent motion states."""
     TRACK = 1
@@ -103,25 +101,31 @@
         if self._split == "test":
             filename = f"{self._location}_obs.csv"
         else:
             filename = f"{self._location}_{self._split}.csv"
 
         return str(Path(self._root).joinpath(filename))
 
-    def get_case(self, case_id: int) -> INTERACTIONCase:
-        history_tracks = self.get_tracks_from_frame(self._get_history(case_id))
-        current_tracks = self.get_tracks_from_frame(self._get_current(case_id))
-        futural_tracks = self.get_tracks_from_frame(self._get_futural(case_id))
+    @property
+    def tracks_to_predict(self) -> dict[int, list[int]]:
+        """dict[int, list[int]]: the tracks to predict for each case."""
+        return self._tracks_to_predict
+
+    @property
+    def interesting_agents(self) -> dict[int, list[int]]:
+        """dict[int, list[int]]: the interesting agents for each case."""
+        return self._interesting_agents
 
+    def get_case(self, case_id: int) -> INTERACTIONCase:
         return INTERACTIONCase(
             location=self._location,
             case_id=int(case_id),
-            history_tracks=history_tracks,
-            current_tracks=current_tracks,
-            futural_tracks=futural_tracks,
+            history_frame=self._get_history(int(case_id)),
+            current_frame=self._get_current(int(case_id)),
+            futural_frame=self._get_futural(int(case_id)),
             tracks_to_predict=self._tracks_to_predict[int(case_id)],
             interesting_agents=self._interesting_agents[int(case_id)],
         )
 
     def render(
         self,
         case_id: int,
@@ -132,33 +136,14 @@
         if case_id >= self._num_cases:
             raise ValueError(
                 f"Invalid case_id {case_id} for scenario {self._location}."
             )
 
         return self.get_case(case_id).render(anchor=anchor, ax=ax, mode=mode)
 
-    @staticmethod
-    def get_tracks_from_frame(frame: TrackFrame) -> list[Track]:
-        track_dict = defaultdict(list)
-        track_type = {}
-        for track_id, row in frame.iterrows():
-            motion_state = MotionState(
-                agent_id=int(track_id),
-                **row.rename(index=MOTION_STATE_FIELD_MAPPING)[
-                    list(MOTION_STATE_FIELD_MAPPING.values())
-                ],
-            )
-            track_dict[track_id].append(motion_state)
-            track_type[track_id] = AgentType.deserialize(row["agent_type"])
-
-        return [
-            Track(agent_id=key, type=track_type[key], motion_states=value)
-            for key, value in track_dict.items()
-        ]
-
     def _get_history(self, case_id: int) -> TrackFrame:
         df = self._frames[INTERACTIONScenarioLayers.MOTION_STATE].loc[case_id]
         return df.loc[df["timestamp_ms"] <= 1000]
 
     def _get_current(self, case_id: int) -> TrackFrame:
         df = self._frames[INTERACTIONScenarioLayers.MOTION_STATE].loc[case_id]
         return df.loc[df["timestamp_ms"] == 1000]
```

### Comparing `interaction-devkit-0.1.4/interaction/dataset/tracks/container.py` & `interaction-devkit-0.1.6/interaction/dataset/tracks/container.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 - :class:`Track`: A single track.
 - :class:`INTERACTIONCase`: A single case of observation in a scenario.
 """
 # Copyright (c) 2023, Juanwu Lu <juanwu@purdue.edu>.
 # Released under the BSD-3-Clause license.
 # See https://opensource.org/license/bsd-3-clause/ for licensing details.
 import math
+from collections import defaultdict
 from collections.abc import Iterable, Iterator
 from dataclasses import dataclass
 from functools import cached_property
 from itertools import chain
 from typing import Any, Optional, Union
+from collections.abc import Generator
 
 import geopandas as gpd
 import matplotlib.pyplot as plt
+from pandas import DataFrame
 from shapely.affinity import rotate, translate
 from shapely.geometry import LineString, Point, Polygon
 
 from ..utils import LOCATIONS
 from .typing import AgentType
 
 # Constants
@@ -32,14 +35,17 @@
     "vx": "velocity_x",
     "vy": "velocity_y",
     "psi_rad": "heading",
     "length": "length",
     "width": "width",
 }
 
+# type aliases
+TrackFrame = Union[gpd.GeoDataFrame, DataFrame]
+
 
 @dataclass(frozen=True)
 class MotionState:
     """A single motion state of an agent at a time step."""
 
     agent_id: int
     """int: The ID of the agent in a case."""
@@ -329,40 +335,65 @@
 class INTERACTIONCase:
     """A single case of observation in a scenario."""
 
     location: str
     """str: The location name of the case."""
     case_id: int
     """int: The ID of the case."""
-    history_tracks: tuple[Track] = ()
-    """Tuple[Track, ...]: The history tracks of the case."""
-    current_tracks: tuple[Track] = ()
-    """Tuple[Track, ...]: The current tracks of the case."""
-    futural_tracks: tuple[Track] = ()
-    """Tuple[Track, ...]: The futural tracks of the case."""
-    tracks_to_predict: tuple[int] = ()
-    """Tuple[int, ...]: The IDs of the tracks to predict."""
-    interesting_agents: tuple[int] = ()
-    """Tuple[int, ...]: The IDs of the interesting agents (ego vehicles)."""
+    history_frame: TrackFrame
+    """TrackFrame: The history frame of the case."""
+    current_frame: TrackFrame
+    """TrackFrame: The current frame of the case."""
+    futural_frame: TrackFrame
+    """TrackFrame: The futural frame of the case."""
+    tracks_to_predict: list[int]
+    """List[int]: The IDs of the tracks to predict."""
+    interesting_agents: list[int]
+    """List[int]: The IDs of the interesting agents in the case."""
 
     def __post_init__(self) -> None:
         """Post-initialization hook."""
         assert self.location in LOCATIONS, "Invalid location name"
         assert (
             isinstance(self.case_id, int) and self.case_id >= 0
         ), "Expected a non-negative integer for case ID."
 
-        self.history_tracks = sorted(self.history_tracks)
-        self._history_ids = [track.agent_id for track in self.history_tracks]
-        self.current_tracks = sorted(self.current_tracks)
-        self._current_ids = [track.agent_id for track in self.current_tracks]
-        self.futural_tracks = sorted(self.futural_tracks)
-        self._futural_ids = [track.agent_id for track in self.futural_tracks]
-        self.tracks_to_predict = tuple(self.tracks_to_predict)
-        self.interesting_agents = tuple(self.interesting_agents)
+        self.history_frame.sort_values(
+            by=["track_id", "timestamp_ms"], inplace=True
+        )
+        self.current_frame.sort_values(
+            by=["track_id", "timestamp_ms"], inplace=True
+        )
+        self.futural_frame.sort_values(
+            by=["track_id", "timestamp_ms"], inplace=True
+        )
+
+    @cached_property
+    def history_ids(self) -> list[int]:
+        return self.history_frame["track_id"].unique().tolist()
+
+    @cached_property
+    def history_tracks(self) -> list[Track]:
+        return self.get_tracks_from_frame(self.history_frame)
+
+    @cached_property
+    def current_ids(self) -> list[int]:
+        return self.current_frame["track_id"].unique().tolist()
+
+    @cached_property
+    def current_tracks(self) -> list[Track]:
+        return self.get_tracks_from_frame(self.current_frame)
+
+    @cached_property
+    def futural_ids(self) -> list[int]:
+        return self.futural_frame["track_id"].unique().tolist()
+
+    @cached_property
+    def futural_tracks(self) -> list[Track]:
+        return self.get_tracks_from_frame(self.futural_frame)
 
     @cached_property
     def num_agents(self) -> int:
         """int: The number of agents in the case."""
         return len(
             {
                 track.agent_id
@@ -371,39 +402,39 @@
                     self.current_tracks,
                     self.futural_tracks,
                 )
             }
         )
 
     def get_history_track(self, agent_id: int) -> Optional[Track]:
-        if agent_id not in self._history_ids:
+        if agent_id not in self.history_ids:
             return None
-        _index = self._history_ids.index(agent_id)
+        _index = self.history_ids.index(agent_id)
         return self.history_tracks[_index]
 
-    def get_history_tracks(self) -> Iterator[Track]:
+    def get_history_tracks(self) -> Generator[Track, None, None]:
         yield from self.history_tracks
 
     def get_current_motion_state(self, agent_id: int) -> Optional[MotionState]:
-        if agent_id not in self._current_ids:
+        if agent_id not in self.current_ids:
             return None
-        _index = self._current_ids.index(agent_id)
+        _index = self.current_ids.index(agent_id)
         return self.current_tracks[_index][-1]
 
-    def get_current_motion_states(self) -> Iterator[MotionState]:
+    def get_current_motion_states(self) -> Generator[MotionState, None, None]:
         for track in self.current_tracks:
             yield track[-1]
 
     def get_futural_track(self, agent_id: int) -> Optional[Track]:
-        if agent_id not in self._futural_ids:
+        if agent_id not in self.futural_ids:
             return None
-        _index = self._futural_ids.index(agent_id)
+        _index = self.futural_ids.index(agent_id)
         return self.futural_tracks[_index]
 
-    def get_futural_tracks(self) -> Iterator[Track]:
+    def get_futural_tracks(self) -> Generator[Track, None, None]:
         yield from self.futural_tracks
 
     def render(
         self,
         anchor: Optional[tuple[float, float, float]] = None,
         ax: Optional[plt.Axes] = None,
         mode: str = "tail-box",
@@ -507,14 +538,33 @@
         elif mode == "full-box":
             # TODO: render the full tracks as boxes
             raise NotImplementedError
         elif mode == "animation":
             # TODO: implement the animation mode
             raise NotImplementedError
 
+    @staticmethod
+    def get_tracks_from_frame(frame: TrackFrame) -> list[Track]:
+        track_dict = defaultdict(list)
+        track_type = {}
+        for track_id, row in frame.iterrows():
+            motion_state = MotionState(
+                agent_id=int(track_id),
+                **row.rename(index=MOTION_STATE_FIELD_MAPPING)[
+                    list(MOTION_STATE_FIELD_MAPPING.values())
+                ],
+            )
+            track_dict[track_id].append(motion_state)
+            track_type[track_id] = AgentType.deserialize(row["agent_type"])
+
+        return [
+            Track(agent_id=key, type=track_type[key], motion_states=value)
+            for key, value in track_dict.items()
+        ]
+
     def __eq__(self, __value: Any) -> bool:
         if isinstance(__value, INTERACTIONCase):
             return (
                 self.location == __value.location
                 and self.case_id == __value.case_id
             )
         return NotImplemented
```

### Comparing `interaction-devkit-0.1.4/interaction/dataset/tracks/typing.py` & `interaction-devkit-0.1.6/interaction/dataset/tracks/typing.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction/dataset/utils.py` & `interaction-devkit-0.1.6/interaction/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/interaction_devkit.egg-info/PKG-INFO` & `interaction-devkit-0.1.6/interaction_devkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interaction-devkit
-Version: 0.1.4
+Version: 0.1.6
 Summary: A toolkit for building interactive applications.
 Author-email: Juanwu Lu <juanwu@purdue.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Juanwu Lu
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `interaction-devkit-0.1.4/interaction_devkit.egg-info/SOURCES.txt` & `interaction-devkit-0.1.6/interaction_devkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/pyproject.toml` & `interaction-devkit-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "interaction-devkit"
-version = "0.1.4"
+version = "0.1.6"
 description = "A toolkit for building interactive applications."
 readme = "README.md"
 authors = [{name="Juanwu Lu", email="juanwu@purdue.edu"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 dependencies = [
     "defusedxml",
@@ -28,15 +28,15 @@
 [tool.isort]
 known_first_party = "interaction-devkit"
 
 line_length = 79
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.1.4"
+current_version = "0.1.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `interaction-devkit-0.1.4/tests/test_map_api.py` & `interaction-devkit-0.1.6/tests/test_map_api.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/tests/test_map_components.py` & `interaction-devkit-0.1.6/tests/test_map_components.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.4/tests/test_track_components.py` & `interaction-devkit-0.1.6/tests/test_track_components.py`

 * *Files identical despite different names*

